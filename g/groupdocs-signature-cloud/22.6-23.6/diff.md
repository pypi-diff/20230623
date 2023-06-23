# Comparing `tmp/groupdocs-signature-cloud-22.6.tar.gz` & `tmp/groupdocs-signature-cloud-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-signature-cloud-22.6.tar", last modified: Fri Jun 24 08:43:48 2022, max compression
+gzip compressed data, was "dist\groupdocs-signature-cloud-23.6.tar", last modified: Fri Jun 23 08:36:10 2023, max compression
```

## Comparing `groupdocs-signature-cloud-22.6.tar` & `groupdocs-signature-cloud-23.6.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:48.000000 groupdocs-signature-cloud-22.6/
--rw-rw-rw-   0        0        0     1107 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/LICENSE
--rw-rw-rw-   0        0        0     2879 2022-06-24 08:43:48.000000 groupdocs-signature-cloud-22.6/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/README.md
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/
--rw-rw-rw-   0        0        0     8202 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/__init__.py
--rw-rw-rw-   0        0        0    27395 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/
--rw-rw-rw-   0        0        0      524 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    38653 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36263 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    18368 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6591 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0     8868 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/preview_api.py
--rw-rw-rw-   0        0        0    30932 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/sign_api.py
--rw-rw-rw-   0        0        0    26576 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3306 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/auth.py
--rw-rw-rw-   0        0        0     7680 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/
--rw-rw-rw-   0        0        0     6832 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     5895 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcode_signature.py
--rw-rw-rw-   0        0        0     4063 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcode_type.py
--rw-rw-rw-   0        0        0     4329 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcodes_result.py
--rw-rw-rw-   0        0        0     4174 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/base_settings.py
--rw-rw-rw-   0        0        0     8339 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/border_line.py
--rw-rw-rw-   0        0        0     4249 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/brush.py
--rw-rw-rw-   0        0        0     4704 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py
--rw-rw-rw-   0        0        0     4840 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/color.py
--rw-rw-rw-   0        0        0     5228 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py
--rw-rw-rw-   0        0        0     5129 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     6315 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_options.py
--rw-rw-rw-   0        0        0     6513 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_result.py
--rw-rw-rw-   0        0        0     4520 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_settings.py
--rw-rw-rw-   0        0        0     4739 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_form_field_signature.py
--rw-rw-rw-   0        0        0     7413 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_signature.py
--rw-rw-rw-   0        0        0     6147 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_signature_appearance.py
--rw-rw-rw-   0        0        0     5187 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     6291 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6354 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5412 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     5612 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/form_field_signature.py
--rw-rw-rw-   0        0        0     4900 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/format.py
--rw-rw-rw-   0        0        0     4186 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     7876 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/image_appearance.py
--rw-rw-rw-   0        0        0     5172 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/image_signature.py
--rw-rw-rw-   0        0        0    12903 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/info_result.py
--rw-rw-rw-   0        0        0     5112 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/info_settings.py
--rw-rw-rw-   0        0        0     6082 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/linear_gradient_brush.py
--rw-rw-rw-   0        0        0     5178 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     7705 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/options_base.py
--rw-rw-rw-   0        0        0     7507 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/padding.py
--rw-rw-rw-   0        0        0     7879 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/page_info.py
--rw-rw-rw-   0        0        0     7966 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pages_setup.py
--rw-rw-rw-   0        0        0     9110 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_digital_signature.py
--rw-rw-rw-   0        0        0    11924 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py
--rw-rw-rw-   0        0        0    11570 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py
--rw-rw-rw-   0        0        0     8108 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py
--rw-rw-rw-   0        0        0     6566 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_page.py
--rw-rw-rw-   0        0        0     6502 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_result.py
--rw-rw-rw-   0        0        0     9611 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_settings.py
--rw-rw-rw-   0        0        0     5884 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_code_signature.py
--rw-rw-rw-   0        0        0     4059 2022-06-24 08:43:18.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_code_type.py
--rw-rw-rw-   0        0        0     4319 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_codes_result.py
--rw-rw-rw-   0        0        0     5331 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/radial_gradient_brush.py
--rw-rw-rw-   0        0        0     5238 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py
--rw-rw-rw-   0        0        0     6286 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/save_options.py
--rw-rw-rw-   0        0        0     6984 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_barcode_options.py
--rw-rw-rw-   0        0        0     3779 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_digital_options.py
--rw-rw-rw-   0        0        0     3733 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_options.py
--rw-rw-rw-   0        0        0     6972 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_qr_code_options.py
--rw-rw-rw-   0        0        0     5780 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_result.py
--rw-rw-rw-   0        0        0     4553 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_settings.py
--rw-rw-rw-   0        0        0     8267 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_barcode_options.py
--rw-rw-rw-   0        0        0    10300 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_digital_options.py
--rw-rw-rw-   0        0        0    21424 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_image_options.py
--rw-rw-rw-   0        0        0     4621 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_options.py
--rw-rw-rw-   0        0        0     9592 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_qr_code_options.py
--rw-rw-rw-   0        0        0     7283 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_result.py
--rw-rw-rw-   0        0        0     5389 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_settings.py
--rw-rw-rw-   0        0        0    11298 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_stamp_options.py
--rw-rw-rw-   0        0        0    31381 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_text_options.py
--rw-rw-rw-   0        0        0    13462 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature.py
--rw-rw-rw-   0        0        0     5115 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature_appearance.py
--rw-rw-rw-   0        0        0     7507 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature_font.py
--rw-rw-rw-   0        0        0     4409 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/solid_brush.py
--rw-rw-rw-   0        0        0    12435 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/stamp_line.py
--rw-rw-rw-   0        0        0     4276 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     4481 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/text_form_field_signature.py
--rw-rw-rw-   0        0        0     5394 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/text_signature.py
--rw-rw-rw-   0        0        0     4575 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/texture_brush.py
--rw-rw-rw-   0        0        0     5369 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/time_stamp.py
--rw-rw-rw-   0        0        0    11389 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_options.py
--rw-rw-rw-   0        0        0     6517 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_result.py
--rw-rw-rw-   0        0        0     4520 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_settings.py
--rw-rw-rw-   0        0        0     4619 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_barcode_options.py
--rw-rw-rw-   0        0        0    11057 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_digital_options.py
--rw-rw-rw-   0        0        0     3718 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_options.py
--rw-rw-rw-   0        0        0     4603 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_qr_code_options.py
--rw-rw-rw-   0        0        0     5980 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_result.py
--rw-rw-rw-   0        0        0     4522 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_settings.py
--rw-rw-rw-   0        0        0     5926 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_text_options.py
--rw-rw-rw-   0        0        0    13739 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/
--rw-rw-rw-   0        0        0     2879 2022-06-24 08:43:45.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6386 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-24 08:43:45.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-06-24 08:43:46.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2022-06-24 08:43:46.000000 groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-24 08:43:48.000000 groupdocs-signature-cloud-22.6/setup.cfg
--rw-rw-rw-   0        0        0     1665 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/test/
--rw-rw-rw-   0        0        0        0 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/test/apis/
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:47.000000 groupdocs-signature-cloud-22.6/test/apis/Search/
--rw-rw-rw-   0        0        0        0 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Search/__init__.py
--rw-rw-rw-   0        0        0     5189 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Search/test_search_barcode.py
--rw-rw-rw-   0        0        0     6450 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Search/test_search_collection.py
--rw-rw-rw-   0        0        0     4035 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Search/test_search_digital.py
--rw-rw-rw-   0        0        0     5171 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Search/test_search_qr_code.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:48.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/
--rw-rw-rw-   0        0        0        0 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/__init__.py
--rw-rw-rw-   0        0        0     5969 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_barcode.py
--rw-rw-rw-   0        0        0    16368 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_collection.py
--rw-rw-rw-   0        0        0     5009 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_digital.py
--rw-rw-rw-   0        0        0     5395 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_image.py
--rw-rw-rw-   0        0        0     5921 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_qr_code.py
--rw-rw-rw-   0        0        0     8163 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_stamp.py
--rw-rw-rw-   0        0        0     5929 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_text.py
-drwxrwxrwx   0        0        0        0 2022-06-24 08:43:48.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/
--rw-rw-rw-   0        0        0        0 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/__init__.py
--rw-rw-rw-   0        0        0     4121 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_barcode.py
--rw-rw-rw-   0        0        0     6232 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_collection.py
--rw-rw-rw-   0        0        0     3655 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_digital.py
--rw-rw-rw-   0        0        0     4107 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_qr_code.py
--rw-rw-rw-   0        0        0     3873 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_text.py
--rw-rw-rw-   0        0        0        0 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3022 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     3796 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3141 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     3658 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/test_info_api.py
--rw-rw-rw-   0        0        0     2732 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     4739 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/test_context.py
--rw-rw-rw-   0        0        0     4965 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/test_file.py
--rw-rw-rw-   0        0        0     1703 2022-06-24 08:43:19.000000 groupdocs-signature-cloud-22.6/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/
+-rw-rw-rw-   0        0        0     1107 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/LICENSE
+-rw-rw-rw-   0        0        0     2879 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/
+-rw-rw-rw-   0        0        0     8368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/__init__.py
+-rw-rw-rw-   0        0        0    27395 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/
+-rw-rw-rw-   0        0        0      524 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    38653 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36263 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    18368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6591 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0     8868 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/preview_api.py
+-rw-rw-rw-   0        0        0    30932 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/sign_api.py
+-rw-rw-rw-   0        0        0    26576 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3306 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/auth.py
+-rw-rw-rw-   0        0        0     7680 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/
+-rw-rw-rw-   0        0        0     6915 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     5895 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_signature.py
+-rw-rw-rw-   0        0        0     4063 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_type.py
+-rw-rw-rw-   0        0        0     4329 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcodes_result.py
+-rw-rw-rw-   0        0        0     4174 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/base_settings.py
+-rw-rw-rw-   0        0        0     8339 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/border_line.py
+-rw-rw-rw-   0        0        0     4249 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/brush.py
+-rw-rw-rw-   0        0        0     4704 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py
+-rw-rw-rw-   0        0        0     4043 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/color.py
+-rw-rw-rw-   0        0        0     5228 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py
+-rw-rw-rw-   0        0        0     5129 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     6315 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_options.py
+-rw-rw-rw-   0        0        0     6513 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_result.py
+-rw-rw-rw-   0        0        0     4520 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_settings.py
+-rw-rw-rw-   0        0        0     4739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_form_field_signature.py
+-rw-rw-rw-   0        0        0     7413 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature.py
+-rw-rw-rw-   0        0        0     6147 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature_appearance.py
+-rw-rw-rw-   0        0        0     5187 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     6291 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6354 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5412 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     5612 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/form_field_signature.py
+-rw-rw-rw-   0        0        0     4900 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4186 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     7876 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_appearance.py
+-rw-rw-rw-   0        0        0     5172 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_signature.py
+-rw-rw-rw-   0        0        0    12903 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0     5112 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_settings.py
+-rw-rw-rw-   0        0        0     6082 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/linear_gradient_brush.py
+-rw-rw-rw-   0        0        0    11168 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/metadata_signature.py
+-rw-rw-rw-   0        0        0     5178 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     7705 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/options_base.py
+-rw-rw-rw-   0        0        0     7507 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/padding.py
+-rw-rw-rw-   0        0        0     7879 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/page_info.py
+-rw-rw-rw-   0        0        0     7966 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pages_setup.py
+-rw-rw-rw-   0        0        0     9110 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature.py
+-rw-rw-rw-   0        0        0    11924 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py
+-rw-rw-rw-   0        0        0    11570 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py
+-rw-rw-rw-   0        0        0     8108 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py
+-rw-rw-rw-   0        0        0     6566 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_page.py
+-rw-rw-rw-   0        0        0     6502 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_result.py
+-rw-rw-rw-   0        0        0     9611 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_settings.py
+-rw-rw-rw-   0        0        0     5884 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_signature.py
+-rw-rw-rw-   0        0        0     4059 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_type.py
+-rw-rw-rw-   0        0        0     4319 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_codes_result.py
+-rw-rw-rw-   0        0        0     5331 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radial_gradient_brush.py
+-rw-rw-rw-   0        0        0     5238 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py
+-rw-rw-rw-   0        0        0     6286 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/save_options.py
+-rw-rw-rw-   0        0        0     6984 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_barcode_options.py
+-rw-rw-rw-   0        0        0     3779 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_digital_options.py
+-rw-rw-rw-   0        0        0     3733 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_options.py
+-rw-rw-rw-   0        0        0     6972 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_qr_code_options.py
+-rw-rw-rw-   0        0        0     5780 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_result.py
+-rw-rw-rw-   0        0        0     4553 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_settings.py
+-rw-rw-rw-   0        0        0     8267 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_barcode_options.py
+-rw-rw-rw-   0        0        0    10300 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_digital_options.py
+-rw-rw-rw-   0        0        0    21424 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_image_options.py
+-rw-rw-rw-   0        0        0     4621 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_options.py
+-rw-rw-rw-   0        0        0     9592 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_qr_code_options.py
+-rw-rw-rw-   0        0        0     7283 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_result.py
+-rw-rw-rw-   0        0        0     5389 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_settings.py
+-rw-rw-rw-   0        0        0    11298 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_stamp_options.py
+-rw-rw-rw-   0        0        0    31381 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_text_options.py
+-rw-rw-rw-   0        0        0    13462 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature.py
+-rw-rw-rw-   0        0        0     5115 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_appearance.py
+-rw-rw-rw-   0        0        0     7507 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_font.py
+-rw-rw-rw-   0        0        0     4409 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/solid_brush.py
+-rw-rw-rw-   0        0        0    12435 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/stamp_line.py
+-rw-rw-rw-   0        0        0     4276 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     4481 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_form_field_signature.py
+-rw-rw-rw-   0        0        0     5394 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_signature.py
+-rw-rw-rw-   0        0        0     4575 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/texture_brush.py
+-rw-rw-rw-   0        0        0     5369 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/time_stamp.py
+-rw-rw-rw-   0        0        0    11389 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_options.py
+-rw-rw-rw-   0        0        0     6517 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_result.py
+-rw-rw-rw-   0        0        0     4520 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_settings.py
+-rw-rw-rw-   0        0        0     4619 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_barcode_options.py
+-rw-rw-rw-   0        0        0    11057 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_digital_options.py
+-rw-rw-rw-   0        0        0     3718 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_options.py
+-rw-rw-rw-   0        0        0     4603 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_qr_code_options.py
+-rw-rw-rw-   0        0        0     5980 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_result.py
+-rw-rw-rw-   0        0        0     4522 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_settings.py
+-rw-rw-rw-   0        0        0     5926 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_text_options.py
+-rw-rw-rw-   0        0        0    13739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2879 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6441 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/setup.cfg
+-rw-rw-rw-   0        0        0     1665 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/
+-rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Search/
+-rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/__init__.py
+-rw-rw-rw-   0        0        0     5189 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_barcode.py
+-rw-rw-rw-   0        0        0     6450 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_collection.py
+-rw-rw-rw-   0        0        0     4035 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_digital.py
+-rw-rw-rw-   0        0        0     5171 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_qr_code.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/
+-rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/__init__.py
+-rw-rw-rw-   0        0        0     5969 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_barcode.py
+-rw-rw-rw-   0        0        0    16368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_collection.py
+-rw-rw-rw-   0        0        0     5009 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_digital.py
+-rw-rw-rw-   0        0        0     5395 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_image.py
+-rw-rw-rw-   0        0        0     5921 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_qr_code.py
+-rw-rw-rw-   0        0        0     8163 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_stamp.py
+-rw-rw-rw-   0        0        0     5929 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_text.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/
+-rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/__init__.py
+-rw-rw-rw-   0        0        0     4121 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_barcode.py
+-rw-rw-rw-   0        0        0     6232 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_collection.py
+-rw-rw-rw-   0        0        0     3655 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_digital.py
+-rw-rw-rw-   0        0        0     4107 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_qr_code.py
+-rw-rw-rw-   0        0        0     3873 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_text.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     3796 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3141 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     3658 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_info_api.py
+-rw-rw-rw-   0        0        0     2732 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     4739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_context.py
+-rw-rw-rw-   0        0        0     4965 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_file.py
+-rw-rw-rw-   0        0        0     1703 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_settings.py
```

### Comparing `groupdocs-signature-cloud-22.6/LICENSE` & `groupdocs-signature-cloud-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-22.6/PKG-INFO` & `groupdocs-signature-cloud-23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-signature-cloud
-Version: 22.6
+Version: 23.6
 Summary: GroupDocs.Signature Cloud Python SDK
 Home-page: http://github.com/groupdocs-signature-cloud/groupdocs-signature-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,signature,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-signature-cloud-22.6/README.md` & `groupdocs-signature-cloud-23.6/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/__init__.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # import models
 from groupdocs_signature_cloud.models.barcode_type import BarcodeType
 from groupdocs_signature_cloud.models.barcodes_result import BarcodesResult
 from groupdocs_signature_cloud.models.base_settings import BaseSettings
 from groupdocs_signature_cloud.models.border_line import BorderLine
 from groupdocs_signature_cloud.models.brush import Brush
 from groupdocs_signature_cloud.models.color import Color
+from groupdocs_signature_cloud.models.consumption_result import ConsumptionResult
 from groupdocs_signature_cloud.models.delete_options import DeleteOptions
 from groupdocs_signature_cloud.models.delete_result import DeleteResult
 from groupdocs_signature_cloud.models.disc_usage import DiscUsage
 from groupdocs_signature_cloud.models.error import Error
 from groupdocs_signature_cloud.models.error_details import ErrorDetails
 from groupdocs_signature_cloud.models.file_info import FileInfo
 from groupdocs_signature_cloud.models.file_versions import FileVersions
@@ -74,14 +75,15 @@
 from groupdocs_signature_cloud.models.digital_signature_appearance import DigitalSignatureAppearance
 from groupdocs_signature_cloud.models.file_version import FileVersion
 from groupdocs_signature_cloud.models.form_field_signature import FormFieldSignature
 from groupdocs_signature_cloud.models.image_appearance import ImageAppearance
 from groupdocs_signature_cloud.models.image_signature import ImageSignature
 from groupdocs_signature_cloud.models.info_settings import InfoSettings
 from groupdocs_signature_cloud.models.linear_gradient_brush import LinearGradientBrush
+from groupdocs_signature_cloud.models.metadata_signature import MetadataSignature
 from groupdocs_signature_cloud.models.pdf_digital_signature_appearance import PdfDigitalSignatureAppearance
 from groupdocs_signature_cloud.models.pdf_text_annotation_appearance import PdfTextAnnotationAppearance
 from groupdocs_signature_cloud.models.pdf_text_sticker_appearance import PdfTextStickerAppearance
 from groupdocs_signature_cloud.models.preview_settings import PreviewSettings
 from groupdocs_signature_cloud.models.qr_code_signature import QRCodeSignature
 from groupdocs_signature_cloud.models.radial_gradient_brush import RadialGradientBrush
 from groupdocs_signature_cloud.models.search_options import SearchOptions
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/api_client.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_client.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '22.6'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.6'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.6'
+        self.user_agent = 'python sdk 23.6'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/api_exception.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_exception.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/__init__.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/file_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -634,15 +634,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -678,15 +678,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -718,15 +718,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="download_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -758,15 +758,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -802,15 +802,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="upload_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/folder_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -610,15 +610,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
         self.dest_path = dest_path
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -690,15 +690,15 @@
         """Initializes new instance of CreateFolderRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -730,15 +730,15 @@
         self.path = path
         self.storage_name = storage_name
         self.recursive = recursive
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_files_list_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -768,15 +768,15 @@
         """Initializes new instance of GetFilesListRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/info_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/info_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -435,15 +435,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_info_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/license_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/license_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/preview_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/preview_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -180,15 +180,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="preview_document_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/sign_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/sign_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -544,15 +544,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_signatures_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -580,15 +580,15 @@
     def __init__(self, sign_settings):
         """Initializes new instance of CreateSignaturesRequest."""  # noqa: E501
         self.sign_settings = sign_settings
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_signatures_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -616,15 +616,15 @@
     def __init__(self, delete_settings):
         """Initializes new instance of DeleteSignaturesRequest."""  # noqa: E501
         self.delete_settings = delete_settings
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="search_signatures_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
     def __init__(self, search_settings):
         """Initializes new instance of SearchSignaturesRequest."""  # noqa: E501
         self.search_settings = search_settings
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="update_signatures_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -688,15 +688,15 @@
     def __init__(self, update_settings):
         """Initializes new instance of UpdateSignaturesRequest."""  # noqa: E501
         self.update_settings = update_settings
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="verify_signatures_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/apis/storage_api.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -471,15 +471,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_disc_usage_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -507,15 +507,15 @@
     def __init__(self, storage_name=None):
         """Initializes new instance of GetDiscUsageRequest."""  # noqa: E501
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_file_versions_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -545,15 +545,15 @@
         """Initializes new instance of GetFileVersionsRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="object_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -585,15 +585,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="storage_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/auth.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="auth.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/configuration.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="configuration.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 22.6\n"\
-               "SDK Package Version: 22.6".\
+               "Version of the API: 23.6\n"\
+               "SDK Package Version: 23.6".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/__init__.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from groupdocs_signature_cloud.models.digital_signature_appearance import DigitalSignatureAppearance
 from groupdocs_signature_cloud.models.file_version import FileVersion
 from groupdocs_signature_cloud.models.form_field_signature import FormFieldSignature
 from groupdocs_signature_cloud.models.image_appearance import ImageAppearance
 from groupdocs_signature_cloud.models.image_signature import ImageSignature
 from groupdocs_signature_cloud.models.info_settings import InfoSettings
 from groupdocs_signature_cloud.models.linear_gradient_brush import LinearGradientBrush
+from groupdocs_signature_cloud.models.metadata_signature import MetadataSignature
 from groupdocs_signature_cloud.models.pdf_digital_signature_appearance import PdfDigitalSignatureAppearance
 from groupdocs_signature_cloud.models.pdf_text_annotation_appearance import PdfTextAnnotationAppearance
 from groupdocs_signature_cloud.models.pdf_text_sticker_appearance import PdfTextStickerAppearance
 from groupdocs_signature_cloud.models.preview_settings import PreviewSettings
 from groupdocs_signature_cloud.models.qr_code_signature import QRCodeSignature
 from groupdocs_signature_cloud.models.radial_gradient_brush import RadialGradientBrush
 from groupdocs_signature_cloud.models.search_options import SearchOptions
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcode_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="BarcodeSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcode_type.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="BarcodeType.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/barcodes_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcodes_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="BarcodesResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/base_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/base_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="BaseSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/border_line.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/border_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="BorderLine.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/brush.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/brush.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Brush.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="CheckboxFormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/color.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
-# <copyright company="Aspose Pty Ltd" file="Color.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+# <copyright company="Aspose Pty Ltd" file="SearchSettings.py">
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -26,96 +26,73 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Color(object):
+from groupdocs_signature_cloud.models import BaseSettings
+
+class SearchSettings(BaseSettings):
     """
-    Keep color value
+    Defines signatures search settings request
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'web': 'str',
-        'alpha': 'int'
+        'options': 'list[SearchOptions]'
     }
 
     attribute_map = {
-        'web': 'Web',
-        'alpha': 'Alpha'
+        'options': 'Options'
     }
 
-    def __init__(self, web=None, alpha=None, **kwargs):  # noqa: E501
-        """Initializes new instance of Color"""  # noqa: E501
-
-        self._web = None
-        self._alpha = None
-
-        if web is not None:
-            self.web = web
-        if alpha is not None:
-            self.alpha = alpha
-    
-    @property
-    def web(self):
-        """
-        Gets the web.  # noqa: E501
-
-        HTML string color representation  # noqa: E501
+    def __init__(self, options=None, **kwargs):  # noqa: E501
+        """Initializes new instance of SearchSettings"""  # noqa: E501
 
-        :return: The web.  # noqa: E501
-        :rtype: str
-        """
-        return self._web
+        self._options = None
 
-    @web.setter
-    def web(self, web):
-        """
-        Sets the web.
+        if options is not None:
+            self.options = options
 
-        HTML string color representation  # noqa: E501
+        base = super(SearchSettings, self)
+        base.__init__(**kwargs)
 
-        :param web: The web.  # noqa: E501
-        :type: str
-        """
-        self._web = web
+        self.swagger_types.update(base.swagger_types)
+        self.attribute_map.update(base.attribute_map)
     
     @property
-    def alpha(self):
+    def options(self):
         """
-        Gets the alpha.  # noqa: E501
+        Gets the options.  # noqa: E501
 
-        Alpha component of color structure  # noqa: E501
+        Gets or sets options collection to perform search in a document  # noqa: E501
 
-        :return: The alpha.  # noqa: E501
-        :rtype: int
+        :return: The options.  # noqa: E501
+        :rtype: list[SearchOptions]
         """
-        return self._alpha
+        return self._options
 
-    @alpha.setter
-    def alpha(self, alpha):
+    @options.setter
+    def options(self, options):
         """
-        Sets the alpha.
+        Sets the options.
 
-        Alpha component of color structure  # noqa: E501
+        Gets or sets options collection to perform search in a document  # noqa: E501
 
-        :param alpha: The alpha.  # noqa: E501
-        :type: int
+        :param options: The options.  # noqa: E501
+        :type: list[SearchOptions]
         """
-        if alpha is None:
-            raise ValueError("Invalid value for `alpha`, must not be `None`")  # noqa: E501
-        self._alpha = alpha
+        self._options = options
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -143,15 +120,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Color):
+        if not isinstance(other, SearchSettings):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ComboboxFormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/consumption_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/consumption_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ConsumptionResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DeleteOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DeleteResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/delete_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DeleteSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_form_field_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DigitalFormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DigitalSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/digital_signature_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DigitalSignatureAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/disc_usage.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/disc_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiscUsage.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/error.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Error.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/error_details.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ErrorDetails.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_info.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_version.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersion.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/file_versions.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/files_list.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesList.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/files_upload_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesUploadResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/form_field_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/format.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Format.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/formats_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/formats_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormatsResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/image_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_appearance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ImageAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/image_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ImageSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/info_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/info_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/linear_gradient_brush.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/linear_gradient_brush.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="LinearGradientBrush.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/object_exist.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/object_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ObjectExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/options_base.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/options_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="OptionsBase.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/padding.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/padding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Padding.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/page_info.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/page_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pages_setup.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pages_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PagesSetup.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_digital_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PdfDigitalSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PdfDigitalSignatureAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PdfTextAnnotationAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PdfTextStickerAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_page.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PreviewPage.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PreviewResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/preview_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PreviewSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_code_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="QRCodeSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_code_type.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="QRCodeType.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/qr_codes_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_codes_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="QRCodesResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/radial_gradient_brush.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radial_gradient_brush.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="RadialGradientBrush.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="RadioButtonFormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/save_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_barcode_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_barcode_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SearchBarcodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_digital_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_digital_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SearchDigitalOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SearchOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_qr_code_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_qr_code_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SearchQRCodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SearchResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/search_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/color.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
-# <copyright company="Aspose Pty Ltd" file="SearchSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+# <copyright company="Aspose Pty Ltd" file="Color.py">
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -26,73 +26,65 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from groupdocs_signature_cloud.models import BaseSettings
-
-class SearchSettings(BaseSettings):
+class Color(object):
     """
-    Defines signatures search settings request
+    Keep color value
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'options': 'list[SearchOptions]'
+        'web': 'str'
     }
 
     attribute_map = {
-        'options': 'Options'
+        'web': 'Web'
     }
 
-    def __init__(self, options=None, **kwargs):  # noqa: E501
-        """Initializes new instance of SearchSettings"""  # noqa: E501
-
-        self._options = None
-
-        if options is not None:
-            self.options = options
+    def __init__(self, web=None, **kwargs):  # noqa: E501
+        """Initializes new instance of Color"""  # noqa: E501
 
-        base = super(SearchSettings, self)
-        base.__init__(**kwargs)
+        self._web = None
 
-        self.swagger_types.update(base.swagger_types)
-        self.attribute_map.update(base.attribute_map)
+        if web is not None:
+            self.web = web
     
     @property
-    def options(self):
+    def web(self):
         """
-        Gets the options.  # noqa: E501
+        Gets the web.  # noqa: E501
 
-        Gets or sets options collection to perform search in a document  # noqa: E501
+        HTML string color representation  # noqa: E501
 
-        :return: The options.  # noqa: E501
-        :rtype: list[SearchOptions]
+        :return: The web.  # noqa: E501
+        :rtype: str
         """
-        return self._options
+        return self._web
 
-    @options.setter
-    def options(self, options):
+    @web.setter
+    def web(self, web):
         """
-        Sets the options.
+        Sets the web.
 
-        Gets or sets options collection to perform search in a document  # noqa: E501
+        HTML string color representation  # noqa: E501
 
-        :param options: The options.  # noqa: E501
-        :type: list[SearchOptions]
+        :param web: The web.  # noqa: E501
+        :type: str
         """
-        self._options = options
+        self._web = web
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -120,15 +112,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchSettings):
+        if not isinstance(other, Color):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_barcode_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_barcode_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignBarcodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_digital_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_digital_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignDigitalOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_image_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_image_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignImageOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_qr_code_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_qr_code_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignQRCodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_stamp_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_stamp_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignStampOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/sign_text_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_text_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignTextOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Signature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature_appearance.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_appearance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignatureAppearance.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/signature_font.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_font.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SignatureFont.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/solid_brush.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/solid_brush.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SolidBrush.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/stamp_line.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/stamp_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StampLine.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/storage_exist.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/storage_file.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageFile.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/text_form_field_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_form_field_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextFormFieldSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/text_signature.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextSignature.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/texture_brush.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/texture_brush.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextureBrush.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/time_stamp.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/time_stamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TimeStamp.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="UpdateOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="UpdateResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/update_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="UpdateSettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_barcode_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_barcode_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyBarcodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_digital_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_digital_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyDigitalOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_qr_code_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_qr_code_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyQRCodeOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_result.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_settings.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifySettings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/models/verify_text_options.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_text_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="VerifyTextOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud/rest.py` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="rest.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/PKG-INFO` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-signature-cloud
-Version: 22.6
+Version: 23.6
 Summary: GroupDocs.Signature Cloud Python SDK
 Home-page: http://github.com/groupdocs-signature-cloud/groupdocs-signature-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,signature,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-signature-cloud-22.6/groupdocs_signature_cloud.egg-info/SOURCES.txt` & `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 groupdocs_signature_cloud/models/format.py
 groupdocs_signature_cloud/models/formats_result.py
 groupdocs_signature_cloud/models/image_appearance.py
 groupdocs_signature_cloud/models/image_signature.py
 groupdocs_signature_cloud/models/info_result.py
 groupdocs_signature_cloud/models/info_settings.py
 groupdocs_signature_cloud/models/linear_gradient_brush.py
+groupdocs_signature_cloud/models/metadata_signature.py
 groupdocs_signature_cloud/models/object_exist.py
 groupdocs_signature_cloud/models/options_base.py
 groupdocs_signature_cloud/models/padding.py
 groupdocs_signature_cloud/models/page_info.py
 groupdocs_signature_cloud/models/pages_setup.py
 groupdocs_signature_cloud/models/pdf_digital_signature.py
 groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py
```

### Comparing `groupdocs-signature-cloud-22.6/setup.py` & `groupdocs-signature-cloud-23.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-signature-cloud"
-VERSION = "22.6"
+VERSION = "23.6"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Search/test_search_barcode.py` & `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Search/test_search_collection.py` & `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Search/test_search_digital.py` & `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_digital.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Search/test_search_qr_code.py` & `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_qr_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_barcode.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_collection.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_digital.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_digital.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_image.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_qr_code.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_qr_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_stamp.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_stamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Sign/test_sign_text.py` & `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_barcode.py` & `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_qr_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -30,53 +30,53 @@
 import unittest
 import os
 
 from groupdocs_signature_cloud import *
 from test.test_context import TestContext
 from test.test_file import TestFile
 
-class TestVerifyBarcode(TestContext):
+class TestVerifyQRcode(TestContext):
 
-    def test_verify_barcode_image(self):
+    def test_verify_qr_code_image(self):
         test_file = TestFile.image_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_barcode_pdf(self):
+    def test_verify_qr_code_pdf(self):
         test_file = TestFile.pdf_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_barcode_presentation(self):
+    def test_verify_qr_code_presentation(self):
         test_file = TestFile.presentation_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_barcode_spreadsheet(self):
+    def test_verify_qr_code_spreadsheet(self):
         test_file = TestFile.spreadsheet_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_barcode_wordprocessing(self):
+    def test_verify_qr_code_wordprocessing(self):
         test_file = TestFile.wordprocessing_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)                       
 
     @staticmethod
     def populate_options(testFile):
-        opts = VerifyBarcodeOptions()
+        opts = VerifyQRCodeOptions()
         
-        opts.signature_type = 'Barcode'
-        opts.text = '123456789012'
-        opts.barcode_type = 'Code39Standard'
+        opts.signature_type = 'QRCode'
+        opts.text = 'John Smith'
+        opts.qr_code_type = 'Aztec'
         opts.match_type = 'Contains'
 
         opts.page = 1
         opts.all_pages = True
         ps = PagesSetup()
         ps.even_pages = False
         ps.first_page = True
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_collection.py` & `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_digital.py` & `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_digital.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_qr_code.py` & `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_barcode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -30,53 +30,53 @@
 import unittest
 import os
 
 from groupdocs_signature_cloud import *
 from test.test_context import TestContext
 from test.test_file import TestFile
 
-class TestVerifyQRcode(TestContext):
+class TestVerifyBarcode(TestContext):
 
-    def test_verify_qr_code_image(self):
+    def test_verify_barcode_image(self):
         test_file = TestFile.image_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_qr_code_pdf(self):
+    def test_verify_barcode_pdf(self):
         test_file = TestFile.pdf_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_qr_code_presentation(self):
+    def test_verify_barcode_presentation(self):
         test_file = TestFile.presentation_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_qr_code_spreadsheet(self):
+    def test_verify_barcode_spreadsheet(self):
         test_file = TestFile.spreadsheet_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)
 
-    def test_verify_qr_code_wordprocessing(self):
+    def test_verify_barcode_wordprocessing(self):
         test_file = TestFile.wordprocessing_signed()
         settings = self.populate_options(test_file)            
         response = self.sign_api.verify_signatures(VerifySignaturesRequest(settings))
         self.check_response(response, test_file)                       
 
     @staticmethod
     def populate_options(testFile):
-        opts = VerifyQRCodeOptions()
+        opts = VerifyBarcodeOptions()
         
-        opts.signature_type = 'QRCode'
-        opts.text = 'John Smith'
-        opts.qr_code_type = 'Aztec'
+        opts.signature_type = 'Barcode'
+        opts.text = '123456789012'
+        opts.barcode_type = 'Code39Standard'
         opts.match_type = 'Contains'
 
         opts.page = 1
         opts.all_pages = True
         ps = PagesSetup()
         ps.even_pages = False
         ps.first_page = True
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/Verify/test_verify_text.py` & `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/test_auth_api.py` & `groupdocs-signature-cloud-23.6/test/apis/test_auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_auth_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/test_file_api.py` & `groupdocs-signature-cloud-23.6/test/apis/test_file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/test_folder_api.py` & `groupdocs-signature-cloud-23.6/test/apis/test_folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/test_info_api.py` & `groupdocs-signature-cloud-23.6/test/apis/test_info_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/apis/test_storage_api.py` & `groupdocs-signature-cloud-23.6/test/apis/test_storage_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/test_context.py` & `groupdocs-signature-cloud-23.6/test/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-signature-cloud-22.6/test/test_file.py` & `groupdocs-signature-cloud-23.6/test/test_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-22.6/test/test_settings.py` & `groupdocs-signature-cloud-23.6/test/test_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_settings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

