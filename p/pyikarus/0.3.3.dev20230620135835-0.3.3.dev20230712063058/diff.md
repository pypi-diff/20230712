# Comparing `tmp/pyikarus-0.3.3.dev20230620135835.tar.gz` & `tmp/pyikarus-0.3.3.dev20230712063058.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230620135835.tar", last modified: Tue Jun 20 13:58:35 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230712063058.tar", last modified: Wed Jul 12 06:30:59 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230620135835.tar` & `pyikarus-0.3.3.dev20230712063058.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.659860 pyikarus-0.3.3.dev20230620135835/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3335 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3213 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3418 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpectraFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.659860 pyikarus-0.3.3.dev20230620135835/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6164 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/
--rw-r--r--   0 root         (0) root         (0)   280461 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/BigLogo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)   441218 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png.license
--rw-r--r--   0 root         (0) root         (0)   482004 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1423 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5309 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    21360 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    11389 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh
--rw-r--r--   0 root         (0) root         (0)    14204 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     7995 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)    15979 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12678 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4371 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7858 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5271 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3989 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/kltest.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.691859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.691859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10515 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15149 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6762 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10214 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.699859 pyikarus-0.3.3.dev20230620135835/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.699859 pyikarus-0.3.3.dev20230620135835/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testAssembler.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)    14291 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testCommon.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testDependencies.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testDirichletValue.cpp
--rw-r--r--   0 root         (0) root         (0)     4795 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testEAS.hh
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testEnhancedAssumedStrains.cpp
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFEElement.hh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFactories.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFunctionTraits.cpp
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3190 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testLinearElasticity.cpp
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testManifolds.cpp
--rw-r--r--   0 root         (0) root         (0)     7949 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testMaterial.cpp
--rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticityNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticitySVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearOperator.cpp
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPathFollowing.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPolyFit.cpp
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPythonConversion.cpp
--rw-r--r--   0 root         (0) root         (0)    17531 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testTrustRegion.cpp
--rw-r--r--   0 root         (0) root         (0)     7005 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testklshell.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.035429 pyikarus-0.3.3.dev20230712063058/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.951429 pyikarus-0.3.3.dev20230712063058/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.967429 pyikarus-0.3.3.dev20230712063058/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.967429 pyikarus-0.3.3.dev20230712063058/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.967429 pyikarus-0.3.3.dev20230712063058/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.971428 pyikarus-0.3.3.dev20230712063058/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.971428 pyikarus-0.3.3.dev20230712063058/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-07-12 06:30:59.031429 pyikarus-0.3.3.dev20230712063058/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.971428 pyikarus-0.3.3.dev20230712063058/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.971428 pyikarus-0.3.3.dev20230712063058/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/AddSpectraFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.951429 pyikarus-0.3.3.dev20230712063058/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.975428 pyikarus-0.3.3.dev20230712063058/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.979429 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.983429 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.983429 pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.983429 pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.983429 pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.983429 pyikarus-0.3.3.dev20230712063058/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.987429 pyikarus-0.3.3.dev20230712063058/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.987429 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/
+-rw-r--r--   0 root         (0) root         (0)   280461 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/BigLogo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.991429 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)   441218 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_blue.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_blue.png.license
+-rw-r--r--   0 root         (0) root         (0)   482004 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_white.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_white.png.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.995429 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.999429 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:58.999429 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21464 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh
+-rw-r--r--   0 root         (0) root         (0)    14300 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    16075 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.003429 pyikarus-0.3.3.dev20230712063058/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4371 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7858 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/kltest.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.007429 pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.015429 pyikarus-0.3.3.dev20230712063058/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.015429 pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.019429 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10515 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.019429 pyikarus-0.3.3.dev20230712063058/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.019429 pyikarus-0.3.3.dev20230712063058/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.019429 pyikarus-0.3.3.dev20230712063058/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.019429 pyikarus-0.3.3.dev20230712063058/python/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/finiteElements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10214 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 06:30:59.035429 pyikarus-0.3.3.dev20230712063058/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-12 06:30:58.000000 pyikarus-0.3.3.dev20230712063058/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.023429 pyikarus-0.3.3.dev20230712063058/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.031429 pyikarus-0.3.3.dev20230712063058/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    15947 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:30:59.031429 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    16428 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17531 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testTrustRegion.cpp
+-rw-r--r--   0 root         (0) root         (0)     6859 2023-07-12 06:30:49.000000 pyikarus-0.3.3.dev20230712063058/tests/src/testklshell.cpp
```

### Comparing `pyikarus-0.3.3.dev20230620135835/.clang-format` & `pyikarus-0.3.3.dev20230712063058/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.cmake-format` & `pyikarus-0.3.3.dev20230712063058/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230712063058/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230712063058/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/.reuse/dep5` & `pyikarus-0.3.3.dev20230712063058/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/CHANGELOG.md` & `pyikarus-0.3.3.dev20230712063058/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230712063058/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSE.md` & `pyikarus-0.3.3.dev20230712063058/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230712063058/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230712063058/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230712063058/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230712063058/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230712063058/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/PKG-INFO` & `pyikarus-0.3.3.dev20230712063058/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230620135835
+Version: 0.3.3.dev20230712063058
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620135835 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230712063058 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230620135835/README.md` & `pyikarus-0.3.3.dev20230712063058/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpectraFlags.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/modules/AddSpectraFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230712063058/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/config.h.cmake` & `pyikarus-0.3.3.dev20230712063058/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230712063058/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/literature.bib` & `pyikarus-0.3.3.dev20230712063058/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230712063058/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230712063058/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230712063058/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/BigLogo.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/BigLogo.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_blue.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png` & `pyikarus-0.3.3.dev20230712063058/docs/website/auxiliaryImages/logo_white.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/download.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/docs/website/index.md` & `pyikarus-0.3.3.dev20230712063058/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230712063058/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files 1% similar despite different names*

```diff
@@ -341,15 +341,16 @@
               const auto CEval = C(local);
               auto easStress   = (CEval * M * alpha).eval();
               typename ResultTypeMap<double>::ResultArray resultVector;
               if (req.isResultRequested(ResultType::linearStress)) {
                 resultVector.resize(3, 1);
                 resultVector = result.getResult(ResultType::linearStress) + easStress;
                 result.insertOrAssignResult(ResultType::linearStress, resultVector);
-              }
+              } else
+                DUNE_THROW(Dune::NotImplemented, "The requested result type is NOT implemented.");
             }
           },
           easVariant_);
     }
 
     void setEASType(int numberOfEASParameters_) {
       const auto& numNodes = DisplacementBasedElement::numberOfNodes;
```

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,16 @@
       auto cauchyStress = (C * epsVoigt).eval();
 
       typename ResultTypeMap<double>::ResultArray resultVector;
       if (req.isResultRequested(ResultType::linearStress)) {
         resultVector.resize(3, 1);
         resultVector = cauchyStress;
         result.insertOrAssignResult(ResultType::linearStress, resultVector);
-      }
+      } else
+        DUNE_THROW(Dune::NotImplemented, "The requested result type is NOT implemented.");
     }
 
     Dune::CachedLocalBasis<
         std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
         localBasis;
     std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
                                                           const double&)>
```

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,16 @@
       auto PK2             = mat.template stresses<StrainTags::greenLagrangian>(EVoigt);
 
       typename ResultTypeMap<double>::ResultArray resultVector;
       if (req.isResultRequested(ResultType::PK2Stress)) {
         resultVector.resizeLike(PK2);
         resultVector = PK2;
         result.insertOrAssignResult(ResultType::PK2Stress, resultVector);
-      }
+      } else
+        DUNE_THROW(Dune::NotImplemented, "The requested result type is NOT implemented.");
     }
 
     Dune::CachedLocalBasis<
         std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
         localBasis;
     std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
                                                           const double&)>
```

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/kltest.py` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/test/kltest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230712063058/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/__init__.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/finiteElements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230712063058/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230620135835
+Version: 0.3.3.dev20230712063058
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620135835 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230712063058 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230712063058/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/python/setup.py.in` & `pyikarus-0.3.3.dev20230712063058/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230712063058/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/setup.py` & `pyikarus-0.3.3.dev20230712063058/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230620135835"
+ikarusVersion = "0.3.3.dev20230712063058"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230712063058/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testAssembler.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testCommon.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testCommon.hh`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 #include <dune/grid/yaspgrid.hh>
 #include <dune/iga/nurbsgrid.hh>
 #include <dune/localfefunctions/cachedlocalBasis/cachedlocalBasis.hh>
 
 #include <ikarus/finiteElements/feBases/autodiffFE.hh>
 #include <ikarus/finiteElements/feBases/powerBasisFE.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
+#include <ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh>
+#include <ikarus/finiteElements/mechanics/linearElastic.hh>
+#include <ikarus/io/resultFunction.hh>
+#include <ikarus/utils/basis.hh>
 #include <ikarus/utils/duneUtilities.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/functionSanityChecks.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
 
 namespace Grids {
   struct Yasp {};
@@ -213,19 +217,44 @@
 
   auto resultRequirements = Ikarus::ResultRequirements<>()
                                 .insertGlobalSolution(Ikarus::FESolutions::displacement, displacement)
                                 .addResultRequest(ResultType::linearStress);
 
   ResultTypeMap<double> result;
   auto gridView        = fe.localView().globalBasis().gridView();
+  using GridView       = decltype(gridView);
   auto scalarBasis     = makeConstSharedBasis(gridView, lagrangeDG<1>());
   auto localScalarView = scalarBasis->localView();
   std::vector<Dune::FieldVector<double, 3>> stressVector(scalarBasis->size());
-  auto ele = elements(gridView).begin();
 
+  using LinearElasticElement
+      = Ikarus::LinearElastic<Ikarus::Basis<std::remove_cvref_t<decltype(fe.localView().globalBasis().preBasis())>>>;
+  using EASElement = Ikarus::EnhancedAssumedStrains<
+      Ikarus::LinearElastic<Ikarus::Basis<std::remove_cvref_t<decltype(fe.localView().globalBasis().preBasis())>>>>;
+
+  if constexpr (std::is_same_v<LinearElasticElement, FiniteElement> or std::is_same_v<EASElement, FiniteElement>) {
+    auto resultRequirements2 = Ikarus::ResultRequirements<>()
+                                   .insertGlobalSolution(Ikarus::FESolutions::displacement, displacement)
+                                   .addResultRequest(ResultType::PK2Stress);
+    Dune::VtkWriter<GridView> vtkWriter(gridView);
+    std::vector<FiniteElement> fes;
+    fes.push_back(fe);
+    auto resultFunction
+        = std::make_shared<ResultFunction<std::remove_cvref_t<FiniteElement>>>(&fes, resultRequirements2);
+    try {
+      vtkWriter.addPointData(Dune::Vtk::Function<GridView>(resultFunction));
+      t.check(false) << "resultFunction5 should have failed for requesting PK2Stress here";
+    } catch (const Dune::NotImplemented&) {
+    }
+  } else
+    std::cout << "Result requirement check is skipped as " << Dune::className<FiniteElement>()
+              << " is not equivalent to " << Dune::className<LinearElasticElement>() << " or "
+              << Dune::className<EASElement>() << std::endl;
+
+  auto ele = elements(gridView).begin();
   localScalarView.bind(*ele);
   const auto& fe2              = localScalarView.tree().finiteElement();
   const auto& referenceElement = Dune::ReferenceElements<double, gridDim>::general(ele->type());
   for (auto c = 0UL; c < fe2.size(); ++c) {
     const auto fineKey                        = fe2.localCoefficients().localKey(c);
     const auto nodalPositionInChildCoordinate = referenceElement.position(fineKey.subEntity(), fineKey.codim());
     fe.calculateAt(resultRequirements, nodalPositionInChildCoordinate, result);
```

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testDependencies.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testDirichletValue.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testEAS.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testEAS.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testEnhancedAssumedStrains.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFactories.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFactories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testFunctionTraits.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testLinearElasticity.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testLinearElasticity.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testManifolds.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testManifolds.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testMaterial.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testMaterial.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticity.hh` & `pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticity.hh`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,24 @@
       = [](const auto& fe, const auto& req, const auto& pos, [[maybe_unused]] int comp) { return 7.0; };
   auto resultFunction4  = ResultFunction(&fes, resReq, OwnResultFunction{});
   auto resultFunction4S = std::make_shared<decltype(resultFunction4)>(resultFunction4);
 
   vtkWriter2.addPointData(Dune::Vtk::Function<GridView>(resultFunction4S));
 
   vtkWriter2.write("EndResult" + Dune::className<Grid>());
+  auto resReq5 = Ikarus::ResultRequirements()
+                     .insertGlobalSolution(Ikarus::FESolutions::displacement, d)
+                     .insertParameter(Ikarus::FEParameter::loadfactor, lambda)
+                     .addResultRequest(ResultType::linearStress);
+  auto resultFunction5 = std::make_shared<ResultFunction<ElementType>>(&fes, resReq5);
+  try {
+    vtkWriter2.addPointData(Dune::Vtk::Function<GridView>(resultFunction5));
+    t.check(false) << "resultFunction5 should have failed for requesting linearStress here";
+  } catch (const Dune::NotImplemented&) {
+  }
 
   nonLinOp.template update<1>();
   t.check(controlInfo.success, "Successful result");
   t.check(gradTol >= nonLinOp.derivative().norm(), "Gradient Tolerance should be larger than actual tolerance");
   return t;
 }
```

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticityNeoHooke.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticitySVK.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearElasticitySVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearOperator.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testNonLinearOperator.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testPathFollowing.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testPathFollowing.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testPolyFit.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testPythonConversion.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testPythonConversion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testTrustRegion.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testTrustRegion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620135835/tests/src/testklshell.cpp` & `pyikarus-0.3.3.dev20230712063058/tests/src/testklshell.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #include <ikarus/utils/drawing/griddrawer.hh>
 #include <ikarus/utils/init.hh>
 #include <ikarus/utils/observer/controlVTKWriter.hh>
 
 using Dune::TestSuite;
 
 auto NonLinearElasticityLoadControlNRandTRforKLShell() {
-  TestSuite t("NonLinearElasticityLoadControlNRandTRforKLShell ");
+  TestSuite t("NonLinearElasticityLoadControlNRandTRforKLShell");
   constexpr auto dimworld        = 3;
   const std::array<int, 2> order = {1, 1};
 
   const std::array<std::vector<double>, 2> knotSpans = {{{0, 0, 1, 1}, {0, 0, 1, 1}}};
 
   using ControlPoint = Dune::IGA::NURBSPatchData<2, dimworld>::ControlPointType;
 
@@ -143,26 +143,24 @@
              .corr_tol  = 1e-16,  // everything should converge to the gradient tolerance
              .useRand   = false,
              .rho_reg   = 1e8,
              .Delta0    = 1});
 
   auto vtkWriter = std::make_shared<ControlSubsamplingVertexVTKWriter<std::remove_cvref_t<decltype(basis.flat())>>>(
       basis.flat(), d, 2);
-  vtkWriter->setFileNamePrefix("Test2DSolid");
+  vtkWriter->setFileNamePrefix("TestKLShell");
   vtkWriter->setFieldInfo("Displacement", Dune::VTK::FieldInfo::Type::vector, 3);
 
   auto lc = Ikarus::LoadControl(tr, 1, {0, 1});
   lc.subscribeAll(vtkWriter);
   const auto controlInfo = lc.run();
 
   std::cout << std::setprecision(16) << std::ranges::max(d) << std::endl;
   t.check(Dune::FloatCmp::eq(0.2957393081676369, std::ranges::max(d)))
       << std::setprecision(16) << "The maximum displacement is " << std::ranges::max(d);
   return t;
 }
 
 int main(int argc, char** argv) {
   Ikarus::init(argc, argv);
-  //  const double E             = materialParameters.get<double>("E");
-  //  const double nu            = materialParameters.get<double>("nu");
   NonLinearElasticityLoadControlNRandTRforKLShell();
 }
```

