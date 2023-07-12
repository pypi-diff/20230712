# Comparing `tmp/timeseriesflattener-1.3.1.tar.gz` & `tmp/timeseriesflattener-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.3.1.tar", last modified: Fri Jun 30 08:23:44 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.4.0.tar", last modified: Wed Jul 12 10:44:44 2023, max compression
```

## Comparing `timeseriesflattener-1.3.1.tar` & `timeseriesflattener-1.4.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.668664 timeseriesflattener-1.3.1/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.676664 timeseriesflattener-1.3.1/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      948 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.680664 timeseriesflattener-1.3.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      868 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    56250 2023-06-30 08:23:32.000000 timeseriesflattener-1.3.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/Makefile
--rw-r--r--   0 root         (0) root         (0)    11520 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9122 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.684664 timeseriesflattener-1.3.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   118804 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50220 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    72388 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4298 2023-06-30 08:23:32.000000 timeseriesflattener-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.688664 timeseriesflattener-1.3.1/src/
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.692664 timeseriesflattener-1.3.1/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     7090 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     8488 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    36395 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.696664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8082 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.672664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.672664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.700664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1505 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.700664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      812 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     1392 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.720664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18309 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2688 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.724664 timeseriesflattener-1.3.1/src/timeseriesflattener/utils/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:23:44.692664 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11520 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-30 08:23:44.000000 timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9390 2023-06-30 08:23:31.000000 timeseriesflattener-1.3.1/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      868 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    56956 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   118804 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50220 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    72388 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-07-12 10:44:34.000000 timeseriesflattener-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     8765 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    36395 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18309 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/utils/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/tasks.py
```

### Comparing `timeseriesflattener-1.3.1/.cruft.json` & `timeseriesflattener-1.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/actions/test/action.yml` & `timeseriesflattener-1.4.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.4.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/dependabot.yml` & `timeseriesflattener-1.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/recommended_repo_setup.md` & `timeseriesflattener-1.4.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.4.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/cruft.yml` & `timeseriesflattener-1.4.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.4.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/documentation.yml` & `timeseriesflattener-1.4.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.4.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.4.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.4.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/stalebot.yml` & `timeseriesflattener-1.4.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.4.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.gitignore` & `timeseriesflattener-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.pre-commit-config.yaml` & `timeseriesflattener-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/.zenodo.json` & `timeseriesflattener-1.4.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/CHANGELOG.md` & `timeseriesflattener-1.4.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.0 (2023-07-12)
+
+### Feature
+
+* Change int detection for new version of pydantic ([`752d3bf`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/752d3bfd1702525bb30f285e4f3b8b0f4edf9a6d))
+
+### Fix
+
+* Remove autodoc pydantic requirements for docs ([`34ae391`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/34ae391303afc1ce57bb8f9fa60a78640d144314))
+* Handle non-coerceable values ([`557371f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/557371f19a5102795c8b87775468bb73448c9449))
+* Toml urls ([`385706d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/385706dcc2b0d64623841fc0047b1303880f4b22))
+
 ## v1.3.1 (2023-06-30)
 
 ### Fix
 
 * Create combinations not working for ([`8c3c343`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8c3c34314cf4f6e304d8f64c7118f57fa1ca1498))
 
 ## v1.3.0 (2023-06-29)
```

### Comparing `timeseriesflattener-1.3.1/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/CONTRIBUTING.md` & `timeseriesflattener-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/LICENSE` & `timeseriesflattener-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/PKG-INFO` & `timeseriesflattener-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -21,17 +21,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: homepage, https://github.com/MartinBernstorff/timeseriesflattener
-Project-URL: repository, https://github.com/MartinBernstorff/timeseriesflattener
-Project-URL: documentation, https://MartinBernstorff.github.io/timeseriesflattener/
+Project-URL: homepage, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: repository, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: documentation, https://aarhus-psychiatry-research.github.io/timeseriesflattener/
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.4.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -14,36 +14,37 @@
 copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: homepage,
-https://github.com/MartinBernstorff/timeseriesflattener Project-URL:
-repository, https://github.com/MartinBernstorff/timeseriesflattener Project-
-URL: documentation, https://MartinBernstorff.github.io/timeseriesflattener/
-Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
-MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python:
-<3.12.0,>=3.8.0 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: test Provides-Extra: docs Provides-Extra: tutorials Provides-
-Extra: text License-File: LICENSE [https://github.com/Aarhus-Psychiatry-
-Research/timeseriesflattener/blob/main/docs/_static/icon.png?raw=true] #
-Timeseriesflattener [![github actions docs](https://github.com/Aarhus-
-Psychiatry-Research/timeseriesflattener/actions/workflows/documentation.yml/
-badge.svg)](https://aarhus-psychiatry-research.github.io/timeseriesflattener/)
-[![github actions pytest](https://github.com/Aarhus-Psychiatry-Research/
-timeseriesflattener/actions/workflows/main_test_and_release.yml/badge.svg)]
-(https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions) [!
-[python versions](https://img.shields.io/pypi/pyversions/timeseriesflattener)]
-(https://pypi.org/project/timeseriesflattener/) [![Code style: black](https://
-img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/
-en/stable/the_black_code_style/current_style.html) [![PyPI version](https://
+https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener Project-URL:
+repository, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: documentation, https://aarhus-psychiatry-research.github.io/
+timeseriesflattener/ Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: <3.12.0,>=3.8.0 Description-Content-Type: text/markdown Provides-Extra:
+dev Provides-Extra: test Provides-Extra: docs Provides-Extra: tutorials
+Provides-Extra: text License-File: LICENSE [https://github.com/Aarhus-
+Psychiatry-Research/timeseriesflattener/blob/main/docs/_static/
+icon.png?raw=true] # Timeseriesflattener [![github actions docs](https://
+github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions/workflows/
+documentation.yml/badge.svg)](https://aarhus-psychiatry-research.github.io/
+timeseriesflattener/) [![github actions pytest](https://github.com/Aarhus-
+Psychiatry-Research/timeseriesflattener/actions/workflows/
+main_test_and_release.yml/badge.svg)](https://github.com/Aarhus-Psychiatry-
+Research/timeseriesflattener/actions) [![python versions](https://
+img.shields.io/pypi/pyversions/timeseriesflattener)](https://pypi.org/project/
+timeseriesflattener/) [![Code style: black](https://img.shields.io/badge/
+Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/
+the_black_code_style/current_style.html) [![PyPI version](https://
 badge.fury.io/py/timeseriesflattener.svg)](https://pypi.org/project/
 timeseriesflattener/) [![status](https://joss.theoj.org/papers/
 3bbea8745668d1aa40ff796c6fd3db87/status.svg)](https://joss.theoj.org/papers/
 3bbea8745668d1aa40ff796c6fd3db87) Time series from e.g. electronic health
 records often have a large number of variables, are sampled at irregular
 intervals and tend to have a large number of missing values. Before this type
 of data can be used for prediction modelling with machine learning methods such
```

### Comparing `timeseriesflattener-1.3.1/README.md` & `timeseriesflattener-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/citation.cff` & `timeseriesflattener-1.4.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/Makefile` & `timeseriesflattener-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/_static/favicon.ico` & `timeseriesflattener-1.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/_static/icon.png` & `timeseriesflattener-1.4.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/_static/icon_dark.png` & `timeseriesflattener-1.4.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/_static/terminology_figure.png` & `timeseriesflattener-1.4.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/conf.py` & `timeseriesflattener-1.4.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinxext.opengraph",
     "sphinx_copybutton",
     "sphinx.ext.githubpages",
     "myst_nb",
     "sphinx_design",  # for design feature such as tabs
-    "sphinxcontrib.autodoc_pydantic",
 ]
 
 add_module_names = False
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
```

### Comparing `timeseriesflattener-1.3.1/docs/faq.rst` & `timeseriesflattener-1.4.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/index.rst` & `timeseriesflattener-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.4.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.4.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.4.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.4.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.4.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.4.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.4.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/icon.png` & `timeseriesflattener-1.4.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/paper/paper.bib` & `timeseriesflattener-1.4.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/paper/paper.md` & `timeseriesflattener-1.4.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/pyproject.toml` & `timeseriesflattener-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.3.1"
+version = "1.4.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -53,15 +53,14 @@
 docs = [
     "sphinx>=5.3.0,<7.1.0",
     "furo==2023.3.27",
     "sphinx-copybutton>=0.5.1,<0.5.3",
     "sphinxext-opengraph>=0.7.3,<0.8.3",
     "myst-nb>=0.6.0,<1.17.0",
     "sphinx_design>=0.3.0,<0.3.1",
-    "autodoc_pydantic>=1.1.0,<1.9.0",
 ]
 tutorials = [
     "jupyter>=1.0.0,<1.1.0",
     "skimpy>=0.0.7,<0.1.0",
 ]
 text = [
     "transformers>=4.26.0",
@@ -70,17 +69,17 @@
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
-homepage = "https://github.com/MartinBernstorff/timeseriesflattener"
-repository = "https://github.com/MartinBernstorff/timeseriesflattener"
-documentation = "https://MartinBernstorff.github.io/timeseriesflattener/"
+homepage = "https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener"
+repository = "https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener"
+documentation = "https://aarhus-psychiatry-research.github.io/timeseriesflattener/"
 
 [tool.pyright]
 exclude = [
   ".*venv*/", 
   ".venv38/",
   ".tox"]
```

### Comparing `timeseriesflattener-1.3.1/src/conftest.py` & `timeseriesflattener-1.4.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,31 @@
 
 @dataclass(frozen=True)
 class CoercedFloats:
     lookwindow: Union[float, int]
     fallback: Union[float, int]
 
 
+def can_be_coerced_losslessly_to_int(value: float) -> bool:
+    try:
+        int_version = int(value)
+        return (int_version - value) == 0
+    except ValueError:
+        return False
+
+
 def coerce_floats(lookwindow: float, fallback: float) -> CoercedFloats:
-    lookwindow = lookwindow if not lookwindow.is_integer() else int(lookwindow)
-    fallback = fallback if not fallback.is_integer() else int(fallback)
+    lookwindow = (
+        lookwindow
+        if not can_be_coerced_losslessly_to_int(lookwindow)
+        else int(lookwindow)
+    )
+    fallback = (
+        fallback if not can_be_coerced_losslessly_to_int(fallback) else int(fallback)
+    )
 
     return CoercedFloats(lookwindow=lookwindow, fallback=fallback)
 
 
 class StaticSpec(BaseModel):
     """Specification for a static feature.
 
@@ -47,15 +61,15 @@
     feature_base_name: str,
     lookwindow: Union[float, int],
     aggregation_fn: AggregationFunType,
     fallback: Union[float, int],
 ) -> str:
     """Get the column name for the temporal feature."""
     coerced = coerce_floats(lookwindow=lookwindow, fallback=fallback)
-    col_str = f"{prefix}_{feature_base_name}_within_{str(coerced.lookwindow)}_days_{aggregation_fn.__name__}_fallback_{coerced.fallback}"
+    col_str = f"{prefix}_{feature_base_name}_within_{coerced.lookwindow!s}_days_{aggregation_fn.__name__}_fallback_{coerced.fallback}"
     return col_str
 
 
 class OutcomeSpec(BaseModel):
     """Specification for an outcome feature.
 
     Args:
```

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.4.0/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -21,17 +21,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: homepage, https://github.com/MartinBernstorff/timeseriesflattener
-Project-URL: repository, https://github.com/MartinBernstorff/timeseriesflattener
-Project-URL: documentation, https://MartinBernstorff.github.io/timeseriesflattener/
+Project-URL: homepage, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: repository, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: documentation, https://aarhus-psychiatry-research.github.io/timeseriesflattener/
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.4.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -14,36 +14,37 @@
 copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: homepage,
-https://github.com/MartinBernstorff/timeseriesflattener Project-URL:
-repository, https://github.com/MartinBernstorff/timeseriesflattener Project-
-URL: documentation, https://MartinBernstorff.github.io/timeseriesflattener/
-Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
-MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python:
-<3.12.0,>=3.8.0 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: test Provides-Extra: docs Provides-Extra: tutorials Provides-
-Extra: text License-File: LICENSE [https://github.com/Aarhus-Psychiatry-
-Research/timeseriesflattener/blob/main/docs/_static/icon.png?raw=true] #
-Timeseriesflattener [![github actions docs](https://github.com/Aarhus-
-Psychiatry-Research/timeseriesflattener/actions/workflows/documentation.yml/
-badge.svg)](https://aarhus-psychiatry-research.github.io/timeseriesflattener/)
-[![github actions pytest](https://github.com/Aarhus-Psychiatry-Research/
-timeseriesflattener/actions/workflows/main_test_and_release.yml/badge.svg)]
-(https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions) [!
-[python versions](https://img.shields.io/pypi/pyversions/timeseriesflattener)]
-(https://pypi.org/project/timeseriesflattener/) [![Code style: black](https://
-img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/
-en/stable/the_black_code_style/current_style.html) [![PyPI version](https://
+https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener Project-URL:
+repository, https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener
+Project-URL: documentation, https://aarhus-psychiatry-research.github.io/
+timeseriesflattener/ Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: <3.12.0,>=3.8.0 Description-Content-Type: text/markdown Provides-Extra:
+dev Provides-Extra: test Provides-Extra: docs Provides-Extra: tutorials
+Provides-Extra: text License-File: LICENSE [https://github.com/Aarhus-
+Psychiatry-Research/timeseriesflattener/blob/main/docs/_static/
+icon.png?raw=true] # Timeseriesflattener [![github actions docs](https://
+github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions/workflows/
+documentation.yml/badge.svg)](https://aarhus-psychiatry-research.github.io/
+timeseriesflattener/) [![github actions pytest](https://github.com/Aarhus-
+Psychiatry-Research/timeseriesflattener/actions/workflows/
+main_test_and_release.yml/badge.svg)](https://github.com/Aarhus-Psychiatry-
+Research/timeseriesflattener/actions) [![python versions](https://
+img.shields.io/pypi/pyversions/timeseriesflattener)](https://pypi.org/project/
+timeseriesflattener/) [![Code style: black](https://img.shields.io/badge/
+Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/
+the_black_code_style/current_style.html) [![PyPI version](https://
 badge.fury.io/py/timeseriesflattener.svg)](https://pypi.org/project/
 timeseriesflattener/) [![status](https://joss.theoj.org/papers/
 3bbea8745668d1aa40ff796c6fd3db87/status.svg)](https://joss.theoj.org/papers/
 3bbea8745668d1aa40ff796c6fd3db87) Time series from e.g. electronic health
 records often have a large number of variables, are sampled at irregular
 intervals and tend to have a large number of missing values. Before this type
 of data can be used for prediction modelling with machine learning methods such
```

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.3.1/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 [docs]
 sphinx<7.1.0,>=5.3.0
 furo==2023.3.27
 sphinx-copybutton<0.5.3,>=0.5.1
 sphinxext-opengraph<0.8.3,>=0.7.3
 myst-nb<1.17.0,>=0.6.0
 sphinx_design<0.3.1,>=0.3.0
-autodoc_pydantic<1.9.0,>=1.1.0
 
 [test]
 pytest<7.3.0,>=7.1.3
 pytest-cov<3.1.0,>=3.0.0
 pytest-xdist<3.2.0,>=3.0.0
 pytest-sugar<0.10.0,>=0.9.4
```

### Comparing `timeseriesflattener-1.3.1/tasks.py` & `timeseriesflattener-1.4.0/tasks.py`

 * *Files identical despite different names*

