# Comparing `tmp/tropycal-1.0.1.tar.gz` & `tmp/tropycal-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tropycal-1.0.1.tar", last modified: Tue Jul 11 20:23:31 2023, max compression
+gzip compressed data, was "tropycal-1.0.2.tar", last modified: Tue Jul 11 22:25:38 2023, max compression
```

## Comparing `tropycal-1.0.1.tar` & `tropycal-1.0.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578859 tropycal-1.0.1/
--rw-r--r--   0 tomerburg   (501) staff       (20)       66 2023-07-02 20:17:03.000000 tropycal-1.0.1/.gitattributes
--rw-r--r--   0 tomerburg   (501) staff       (20)      113 2023-07-02 20:17:03.000000 tropycal-1.0.1/.gitignore
--rw-r--r--   0 tomerburg   (501) staff       (20)     2485 2023-07-02 20:17:03.000000 tropycal-1.0.1/.travis.yml
--rw-r--r--   0 tomerburg   (501) staff       (20)     1057 2023-07-02 20:17:03.000000 tropycal-1.0.1/LICENSE
--rw-r--r--   0 tomerburg   (501) staff       (20)       16 2023-07-02 20:17:03.000000 tropycal-1.0.1/MANIFEST.in
--rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 20:23:31.578991 tropycal-1.0.1/PKG-INFO
--rw-r--r--   0 tomerburg   (501) staff       (20)     4368 2023-07-11 20:14:34.000000 tropycal-1.0.1/README.md
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.507597 tropycal-1.0.1/ci/
--rw-r--r--   0 tomerburg   (501) staff       (20)     4452 2023-07-02 20:17:03.000000 tropycal-1.0.1/ci/deploy_key.enc
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.510573 tropycal-1.0.1/docs/
--rw-r--r--   0 tomerburg   (501) staff       (20)      642 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/Makefile
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.534414 tropycal-1.0.1/docs/_static/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.535685 tropycal-1.0.1/docs/_static/css/
--rw-r--r--   0 tomerburg   (501) staff       (20)     3275 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/badge_only.css
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.553894 tropycal-1.0.1/docs/_static/css/fonts/
--rw-r--r--   0 tomerburg   (501) staff       (20)    87624 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    67312 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)    86288 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    66444 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   165742 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 tomerburg   (501) staff       (20)   444379 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 tomerburg   (501) staff       (20)   165548 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 tomerburg   (501) staff       (20)    98024 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    77160 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   323344 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   193308 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   309728 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   184912 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   328412 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   195704 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   309192 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   182708 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   135191 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/theme.css
--rw-r--r--   0 tomerburg   (501) staff       (20)   530613 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/dorian.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   665534 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/grid_example_1.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.554759 tropycal-1.0.1/docs/_static/js/
--rw-r--r--   0 tomerburg   (501) staff       (20)      934 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/js/badge_only.js
--rw-r--r--   0 tomerburg   (501) staff       (20)     5023 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/js/theme.js
--rw-r--r--   0 tomerburg   (501) staff       (20)    11979 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/logo.png
--rw-r--r--   0 tomerburg   (501) staff       (20)    94302 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/logo_32.ico
--rw-r--r--   0 tomerburg   (501) staff       (20)   566670 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   612897 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   565722 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   583690 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_4.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   446960 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   401309 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   398432 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)      328 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/theme_override.css
--rw-r--r--   0 tomerburg   (501) staff       (20)   726348 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   307446 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   172063 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   152687 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_5.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   277793 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   357620 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   245771 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   217745 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_4.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.501813 tropycal-1.0.1/docs/_templates/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.555634 tropycal-1.0.1/docs/_templates/autosummary/
--rw-r--r--   0 tomerburg   (501) staff       (20)      181 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      699 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1210 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.555894 tropycal-1.0.1/docs/_templates/overrides/
--rw-r--r--   0 tomerburg   (501) staff       (20)      772 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/overrides/tropycal.utils.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.556150 tropycal-1.0.1/docs/api/
--rw-r--r--   0 tomerburg   (501) staff       (20)      698 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/api/index.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     7517 2023-07-11 20:15:12.000000 tropycal-1.0.1/docs/conf.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6077 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/data.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1622 2023-07-11 20:16:05.000000 tropycal-1.0.1/docs/index.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      935 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/install.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1108 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/make.bat
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.556950 tropycal-1.0.1/docs/options/
--rw-r--r--   0 tomerburg   (501) staff       (20)     2094 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/domain.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      102 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/gridded_stats.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)    10181 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/map_prop.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)       76 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/requirements.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      554 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/sample_usage.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.558647 tropycal-1.0.1/docs/samples/
--rw-r--r--   0 tomerburg   (501) staff       (20)     6253 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.TrackDataset.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)    10328 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.storm.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     4359 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.tornado.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      505 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/support.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      114 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/test.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7375 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/tropycal_full_logo.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.561911 tropycal-1.0.1/examples/
--rw-r--r--   0 tomerburg   (501) staff       (20)       96 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/README.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)     5534 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/analogs.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    10897 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/cartopy.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6171 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/customize_storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6297 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7105 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/recon.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     4456 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/ships.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     5164 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tc_rainfall.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     8733 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.TrackDataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     2757 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7465 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     4451 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.tornado.py
--rw-r--r--   0 tomerburg   (501) staff       (20)      997 2023-07-11 20:23:31.579309 tropycal-1.0.1/setup.cfg
--rw-r--r--   0 tomerburg   (501) staff       (20)      121 2023-07-02 20:17:03.000000 tropycal-1.0.1/setup.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.502295 tropycal-1.0.1/src/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.562511 tropycal-1.0.1/src/tropycal/
--rw-r--r--   0 tomerburg   (501) staff       (20)      159 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)      447 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/_version.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     5103 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/constants.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.563526 tropycal-1.0.1/src/tropycal/plot/
--rw-r--r--   0 tomerburg   (501) staff       (20)       23 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/plot/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    14158 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/plot/plot.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.564048 tropycal-1.0.1/src/tropycal/rain/
--rw-r--r--   0 tomerburg   (501) staff       (20)      184 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    11110 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    27902 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/plot.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.565214 tropycal-1.0.1/src/tropycal/realtime/
--rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/realtime/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    37999 2023-07-11 15:17:41.000000 tropycal-1.0.1/src/tropycal/realtime/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    47725 2023-07-11 18:29:30.000000 tropycal-1.0.1/src/tropycal/realtime/storm.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.568758 tropycal-1.0.1/src/tropycal/recon/
--rw-r--r--   0 tomerburg   (501) staff       (20)      240 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   122736 2023-07-02 22:24:35.000000 tropycal-1.0.1/src/tropycal/recon/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    39124 2023-07-02 22:16:19.000000 tropycal-1.0.1/src/tropycal/recon/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    39275 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    63621 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.570000 tropycal-1.0.1/src/tropycal/ships/
--rw-r--r--   0 tomerburg   (501) staff       (20)       85 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/ships/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    16078 2023-07-11 19:09:00.000000 tropycal-1.0.1/src/tropycal/ships/ships.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.570762 tropycal-1.0.1/src/tropycal/tornado/
--rw-r--r--   0 tomerburg   (501) staff       (20)      176 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    15765 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     8853 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     1941 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.574048 tropycal-1.0.1/src/tropycal/tracks/
--rw-r--r--   0 tomerburg   (501) staff       (20)      224 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/__init__.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.574495 tropycal-1.0.1/src/tropycal/tracks/data/
--rw-r--r--   0 tomerburg   (501) staff       (20)     1249 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/data/catarina.csv
--rw-r--r--   0 tomerburg   (501) staff       (20)     1924 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/data/pacific_2006.csv
--rw-r--r--   0 tomerburg   (501) staff       (20)   213904 2023-07-06 23:31:07.000000 tropycal-1.0.1/src/tropycal/tracks/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   130072 2023-07-10 15:18:51.000000 tropycal-1.0.1/src/tropycal/tracks/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    20570 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   123426 2023-07-11 16:57:39.000000 tropycal-1.0.1/src/tropycal/tracks/storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    31259 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.575624 tropycal-1.0.1/src/tropycal/utils/
--rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    10482 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/cartopy_utils.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    11465 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/colors.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    72336 2023-07-11 18:33:59.000000 tropycal-1.0.1/src/tropycal/utils/generic_utils.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.563157 tropycal-1.0.1/src/tropycal.egg-info/
--rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/PKG-INFO
--rw-r--r--   0 tomerburg   (501) staff       (20)     3897 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/SOURCES.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)        1 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/dependency_links.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      119 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/requires.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)        9 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/top_level.txt
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.503196 tropycal-1.0.1/tests/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.576777 tropycal-1.0.1/tests/data/
--rw-r--r--   0 tomerburg   (501) staff       (20)   136603 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/data/sample_hurdat.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      782 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/data/sample_storm.txt
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.577356 tropycal-1.0.1/tests/ships/
--rw-r--r--   0 tomerburg   (501) staff       (20)     3566 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/ships/test_ships.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578460 tropycal-1.0.1/tests/tracks/
--rw-r--r--   0 tomerburg   (501) staff       (20)     4840 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     1599 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6755 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_storm.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578681 tropycal-1.0.1/tests/utils/
--rw-r--r--   0 tomerburg   (501) staff       (20)    19452 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/utils/test_utils.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.630138 tropycal-1.0.2/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       66 2023-07-11 20:55:01.000000 tropycal-1.0.2/.gitattributes
+-rw-r--r--   0 tomerburg   (501) staff       (20)      113 2023-07-11 20:55:01.000000 tropycal-1.0.2/.gitignore
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2485 2023-07-11 20:55:02.000000 tropycal-1.0.2/.travis.yml
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1057 2023-07-11 20:55:01.000000 tropycal-1.0.2/LICENSE
+-rw-r--r--   0 tomerburg   (501) staff       (20)       16 2023-07-11 20:55:01.000000 tropycal-1.0.2/MANIFEST.in
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 22:25:38.630264 tropycal-1.0.2/PKG-INFO
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4368 2023-07-11 22:22:01.000000 tropycal-1.0.2/README.md
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.560681 tropycal-1.0.2/ci/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4452 2023-07-11 20:55:01.000000 tropycal-1.0.2/ci/deploy_key.enc
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.563239 tropycal-1.0.2/docs/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      642 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/Makefile
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.585649 tropycal-1.0.2/docs/_static/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.586677 tropycal-1.0.2/docs/_static/css/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3275 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/badge_only.css
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.606765 tropycal-1.0.2/docs/_static/css/fonts/
+-rw-r--r--   0 tomerburg   (501) staff       (20)    87624 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    67312 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)    86288 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    66444 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   165742 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 tomerburg   (501) staff       (20)   444379 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 tomerburg   (501) staff       (20)   165548 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 tomerburg   (501) staff       (20)    98024 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    77160 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   323344 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   193308 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   309728 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   184912 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   328412 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   195704 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   309192 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   182708 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   135191 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/css/theme.css
+-rw-r--r--   0 tomerburg   (501) staff       (20)   530613 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/dorian.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   665534 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/grid_example_1.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.609468 tropycal-1.0.2/docs/_static/js/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      934 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/js/badge_only.js
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5023 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/js/theme.js
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11979 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/logo.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)    94302 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/logo_32.ico
+-rw-r--r--   0 tomerburg   (501) staff       (20)   566670 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/michael_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   612897 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/michael_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   565722 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/michael_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   583690 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/michael_example_4.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   446960 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/storm_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   401309 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/storm_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   398432 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/storm_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)      328 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/theme_override.css
+-rw-r--r--   0 tomerburg   (501) staff       (20)   726348 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/tornado_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   307446 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/tornado_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   172063 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/tornado_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   152687 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/tornado_example_5.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   277793 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/trackdataset_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   357620 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/trackdataset_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   245771 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/trackdataset_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   217745 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_static/trackdataset_example_4.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.556810 tropycal-1.0.2/docs/_templates/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.610149 tropycal-1.0.2/docs/_templates/autosummary/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      181 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      699 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1210 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.610384 tropycal-1.0.2/docs/_templates/overrides/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      772 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/_templates/overrides/tropycal.utils.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.610590 tropycal-1.0.2/docs/api/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      698 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/api/index.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7517 2023-07-11 22:22:20.000000 tropycal-1.0.2/docs/conf.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6077 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/data.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1622 2023-07-11 22:22:08.000000 tropycal-1.0.2/docs/index.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      935 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/install.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1108 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/make.bat
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.611199 tropycal-1.0.2/docs/options/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2094 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/options/domain.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      102 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/options/gridded_stats.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10181 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/options/map_prop.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)       76 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/requirements.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      554 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/sample_usage.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.612422 tropycal-1.0.2/docs/samples/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6253 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/samples/tracks.TrackDataset.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10328 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/samples/tracks.storm.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4359 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/samples/tracks.tornado.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      505 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/support.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      114 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/test.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7375 2023-07-11 20:55:01.000000 tropycal-1.0.2/docs/tropycal_full_logo.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.615076 tropycal-1.0.2/examples/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       96 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/README.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5534 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/analogs.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10897 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/cartopy.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6171 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/customize_storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6297 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7105 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/recon.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4456 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/ships.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5164 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/tc_rainfall.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     8733 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/tracks.TrackDataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2757 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/tracks.season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7465 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/tracks.storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4451 2023-07-11 20:55:01.000000 tropycal-1.0.2/examples/tracks.tornado.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)      997 2023-07-11 22:25:38.630595 tropycal-1.0.2/setup.cfg
+-rw-r--r--   0 tomerburg   (501) staff       (20)      121 2023-07-11 20:55:01.000000 tropycal-1.0.2/setup.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.557378 tropycal-1.0.2/src/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.615667 tropycal-1.0.2/src/tropycal/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      159 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)      447 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/_version.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5103 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/constants.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.616630 tropycal-1.0.2/src/tropycal/plot/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       23 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/plot/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    14158 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/plot/plot.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.617369 tropycal-1.0.2/src/tropycal/rain/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      184 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/rain/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11110 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/rain/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    27902 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/rain/plot.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.618760 tropycal-1.0.2/src/tropycal/realtime/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/realtime/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    37999 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/realtime/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    47725 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/realtime/storm.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.620501 tropycal-1.0.2/src/tropycal/recon/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      240 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/recon/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   122736 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/recon/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    39124 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/recon/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    39275 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/recon/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    63621 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/recon/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.621439 tropycal-1.0.2/src/tropycal/ships/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       85 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/ships/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    16078 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/ships/ships.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.622736 tropycal-1.0.2/src/tropycal/tornado/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      176 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tornado/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    15765 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tornado/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     8853 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tornado/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1941 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tornado/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.625412 tropycal-1.0.2/src/tropycal/tracks/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      224 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/__init__.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.626332 tropycal-1.0.2/src/tropycal/tracks/data/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1249 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/data/catarina.csv
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1924 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/data/pacific_2006.csv
+-rw-r--r--   0 tomerburg   (501) staff       (20)   213904 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   130129 2023-07-11 22:20:51.000000 tropycal-1.0.2/src/tropycal/tracks/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    20570 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   123426 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    31259 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/tracks/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.627225 tropycal-1.0.2/src/tropycal/utils/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/utils/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10482 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/utils/cartopy_utils.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11465 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/utils/colors.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    72336 2023-07-11 20:55:02.000000 tropycal-1.0.2/src/tropycal/utils/generic_utils.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.616276 tropycal-1.0.2/src/tropycal.egg-info/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 22:25:38.000000 tropycal-1.0.2/src/tropycal.egg-info/PKG-INFO
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3897 2023-07-11 22:25:38.000000 tropycal-1.0.2/src/tropycal.egg-info/SOURCES.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)        1 2023-07-11 22:25:38.000000 tropycal-1.0.2/src/tropycal.egg-info/dependency_links.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      119 2023-07-11 22:25:38.000000 tropycal-1.0.2/src/tropycal.egg-info/requires.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)        9 2023-07-11 22:25:38.000000 tropycal-1.0.2/src/tropycal.egg-info/top_level.txt
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.558788 tropycal-1.0.2/tests/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.628909 tropycal-1.0.2/tests/data/
+-rw-r--r--   0 tomerburg   (501) staff       (20)   136603 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/data/sample_hurdat.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      782 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/data/sample_storm.txt
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.629242 tropycal-1.0.2/tests/ships/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3566 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/ships/test_ships.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.629687 tropycal-1.0.2/tests/tracks/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4840 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/tracks/test_dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1599 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/tracks/test_season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6755 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/tracks/test_storm.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 22:25:38.629939 tropycal-1.0.2/tests/utils/
+-rw-r--r--   0 tomerburg   (501) staff       (20)    19452 2023-07-11 20:55:01.000000 tropycal-1.0.2/tests/utils/test_utils.py
```

### Comparing `tropycal-1.0.1/.travis.yml` & `tropycal-1.0.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/LICENSE` & `tropycal-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/PKG-INFO` & `tropycal-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tropycal
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for retrieving and analyzing tropical cyclone data
 Home-page: https://github.com/tropycal/tropycal
 Author: Tomer Burg, Sam Lillo
 Project-URL: Documentation, https://tropycal.github.io/tropycal/
 Project-URL: Source Code, https://github.com/tropycal/tropycal
 Keywords: meteorology,weather
 Platform: any
@@ -18,15 +18,15 @@
 License-File: LICENSE
 
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.1.
+The latest version of Tropycal is v1.0.2.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0.1/README.md` & `tropycal-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.1.
+The latest version of Tropycal is v1.0.2.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0.1/ci/deploy_key.enc` & `tropycal-1.0.2/ci/deploy_key.enc`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/Makefile` & `tropycal-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/badge_only.css` & `tropycal-1.0.2/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.eot` & `tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.svg` & `tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.ttf` & `tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff` & `tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff` & `tropycal-1.0.2/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff` & `tropycal-1.0.2/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff` & `tropycal-1.0.2/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff` & `tropycal-1.0.2/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff2` & `tropycal-1.0.2/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/css/theme.css` & `tropycal-1.0.2/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/dorian.png` & `tropycal-1.0.2/docs/_static/dorian.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/grid_example_1.png` & `tropycal-1.0.2/docs/_static/grid_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/js/badge_only.js` & `tropycal-1.0.2/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/js/theme.js` & `tropycal-1.0.2/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/logo.png` & `tropycal-1.0.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/logo_32.ico` & `tropycal-1.0.2/docs/_static/logo_32.ico`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/michael_example_1.png` & `tropycal-1.0.2/docs/_static/michael_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/michael_example_2.png` & `tropycal-1.0.2/docs/_static/michael_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/michael_example_3.png` & `tropycal-1.0.2/docs/_static/michael_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/michael_example_4.png` & `tropycal-1.0.2/docs/_static/michael_example_4.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/storm_example_1.png` & `tropycal-1.0.2/docs/_static/storm_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/storm_example_2.png` & `tropycal-1.0.2/docs/_static/storm_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/storm_example_3.png` & `tropycal-1.0.2/docs/_static/storm_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/tornado_example_1.png` & `tropycal-1.0.2/docs/_static/tornado_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/tornado_example_2.png` & `tropycal-1.0.2/docs/_static/tornado_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/tornado_example_3.png` & `tropycal-1.0.2/docs/_static/tornado_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/tornado_example_5.png` & `tropycal-1.0.2/docs/_static/tornado_example_5.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/trackdataset_example_1.png` & `tropycal-1.0.2/docs/_static/trackdataset_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/trackdataset_example_2.png` & `tropycal-1.0.2/docs/_static/trackdataset_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/trackdataset_example_3.png` & `tropycal-1.0.2/docs/_static/trackdataset_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_static/trackdataset_example_4.png` & `tropycal-1.0.2/docs/_static/trackdataset_example_4.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_templates/autosummary/class.rst` & `tropycal-1.0.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_templates/autosummary/module.rst` & `tropycal-1.0.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/_templates/overrides/tropycal.utils.rst` & `tropycal-1.0.2/docs/_templates/overrides/tropycal.utils.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/api/index.rst` & `tropycal-1.0.2/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/conf.py` & `tropycal-1.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 project = 'tropycal'
 copyright = '2023, Tropycal Developers'
 author = 'Tropycal Developers'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
-release = '1.0.1'
+release = '1.0.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '2.1'
```

### Comparing `tropycal-1.0.1/docs/data.rst` & `tropycal-1.0.2/docs/data.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/index.rst` & `tropycal-1.0.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    api/index
    sample_usage
    data
 
 Latest Version
 ==============
 
-The latest version of Tropycal as of 11 July 2023 is v1.0.1. This documentation is valid for the latest version of Tropycal.
+The latest version of Tropycal as of 11 July 2023 is v1.0.2. This documentation is valid for the latest version of Tropycal.
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `tropycal-1.0.1/docs/install.rst` & `tropycal-1.0.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/make.bat` & `tropycal-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/options/domain.rst` & `tropycal-1.0.2/docs/options/domain.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/options/map_prop.rst` & `tropycal-1.0.2/docs/options/map_prop.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/sample_usage.rst` & `tropycal-1.0.2/docs/sample_usage.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/samples/tracks.TrackDataset.rst` & `tropycal-1.0.2/docs/samples/tracks.TrackDataset.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/samples/tracks.storm.rst` & `tropycal-1.0.2/docs/samples/tracks.storm.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/samples/tracks.tornado.rst` & `tropycal-1.0.2/docs/samples/tracks.tornado.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/docs/tropycal_full_logo.png` & `tropycal-1.0.2/docs/tropycal_full_logo.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/analogs.py` & `tropycal-1.0.2/examples/analogs.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/cartopy.py` & `tropycal-1.0.2/examples/cartopy.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/customize_storm.py` & `tropycal-1.0.2/examples/customize_storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/realtime.py` & `tropycal-1.0.2/examples/realtime.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/recon.py` & `tropycal-1.0.2/examples/recon.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/ships.py` & `tropycal-1.0.2/examples/ships.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/tc_rainfall.py` & `tropycal-1.0.2/examples/tc_rainfall.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/tracks.TrackDataset.py` & `tropycal-1.0.2/examples/tracks.TrackDataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/tracks.season.py` & `tropycal-1.0.2/examples/tracks.season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/tracks.storm.py` & `tropycal-1.0.2/examples/tracks.storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/examples/tracks.tornado.py` & `tropycal-1.0.2/examples/tracks.tornado.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/setup.cfg` & `tropycal-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tropycal
-version = 1.0.1
+version = 1.0.2
 description = Package for retrieving and analyzing tropical cyclone data
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Tomer Burg, Sam Lillo
 platform = any
 keywords = meteorology, weather
 classifiers =
```

### Comparing `tropycal-1.0.1/src/tropycal/constants.py` & `tropycal-1.0.2/src/tropycal/constants.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/plot/plot.py` & `tropycal-1.0.2/src/tropycal/plot/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/rain/dataset.py` & `tropycal-1.0.2/src/tropycal/rain/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/rain/plot.py` & `tropycal-1.0.2/src/tropycal/rain/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/realtime/realtime.py` & `tropycal-1.0.2/src/tropycal/realtime/realtime.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/realtime/storm.py` & `tropycal-1.0.2/src/tropycal/realtime/storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/recon/dataset.py` & `tropycal-1.0.2/src/tropycal/recon/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/recon/plot.py` & `tropycal-1.0.2/src/tropycal/recon/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/recon/realtime.py` & `tropycal-1.0.2/src/tropycal/recon/realtime.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/recon/tools.py` & `tropycal-1.0.2/src/tropycal/recon/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/ships/ships.py` & `tropycal-1.0.2/src/tropycal/ships/ships.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tornado/dataset.py` & `tropycal-1.0.2/src/tropycal/tornado/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tornado/plot.py` & `tropycal-1.0.2/src/tropycal/tornado/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tornado/tools.py` & `tropycal-1.0.2/src/tropycal/tornado/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/data/catarina.csv` & `tropycal-1.0.2/src/tropycal/tracks/data/catarina.csv`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/data/pacific_2006.csv` & `tropycal-1.0.2/src/tropycal/tracks/data/pacific_2006.csv`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/dataset.py` & `tropycal-1.0.2/src/tropycal/tracks/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/plot.py` & `tropycal-1.0.2/src/tropycal/tracks/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,29 +823,30 @@
         # Check for sufficiently many hours
         if len(check_duration) > 1:
 
             # Generate forecast cone for forecast data
             dateline = False
             if self.proj.proj4_params['lon_0'] == 180.0:
                 dateline = True
-            cone = generate_nhc_cone(
-                forecast, forecast['basin'], dateline, cone_days)
+            cone = generate_nhc_cone(forecast, forecast['basin'], dateline, cone_days)
 
             # Contour fill cone & account for dateline crossing
+            cone_lon = cone['lon']
+            cone_lat = cone['lat']
             if 'cone' in forecast.keys() and not forecast['cone']:
                 pass
             else:
                 if self.proj.proj4_params['lon_0'] == 180.0:
                     new_lons = np.array(cone['lon2d'])
                     new_lons[new_lons < 0] = new_lons[new_lons < 0] + 360.0
                     cone['lon2d'] = new_lons
                     center_lon = np.array(cone['center_lon'])
                     center_lon[center_lon < 0] = center_lon[center_lon < 0] + 360.0
                     cone['center_lon'] = center_lon
-                plot_cone(self.ax,cone,plot_center_line=True,center_linewidth=2.0,zorder=3)
+                plot_cone(self.ax, cone, plot_center_line=True, center_linewidth=2.0, zorder=3)
 
             # Retrieve forecast dots
             iter_hr = np.array(forecast['fhr'])[
                 (fcst_hr >= start_slice) & (fcst_hr <= cone_days * 24)]
             fcst_lon = np.array(forecast['lon'])[
                 (fcst_hr >= start_slice) & (fcst_hr <= cone_days * 24)]
             fcst_lat = np.array(forecast['lat'])[
```

### Comparing `tropycal-1.0.1/src/tropycal/tracks/season.py` & `tropycal-1.0.2/src/tropycal/tracks/season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/storm.py` & `tropycal-1.0.2/src/tropycal/tracks/storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/tracks/tools.py` & `tropycal-1.0.2/src/tropycal/tracks/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/utils/cartopy_utils.py` & `tropycal-1.0.2/src/tropycal/utils/cartopy_utils.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/utils/colors.py` & `tropycal-1.0.2/src/tropycal/utils/colors.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal/utils/generic_utils.py` & `tropycal-1.0.2/src/tropycal/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/src/tropycal.egg-info/PKG-INFO` & `tropycal-1.0.2/src/tropycal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tropycal
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for retrieving and analyzing tropical cyclone data
 Home-page: https://github.com/tropycal/tropycal
 Author: Tomer Burg, Sam Lillo
 Project-URL: Documentation, https://tropycal.github.io/tropycal/
 Project-URL: Source Code, https://github.com/tropycal/tropycal
 Keywords: meteorology,weather
 Platform: any
@@ -18,15 +18,15 @@
 License-File: LICENSE
 
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.1.
+The latest version of Tropycal is v1.0.2.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0.1/src/tropycal.egg-info/SOURCES.txt` & `tropycal-1.0.2/src/tropycal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/data/sample_hurdat.txt` & `tropycal-1.0.2/tests/data/sample_hurdat.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/data/sample_storm.txt` & `tropycal-1.0.2/tests/data/sample_storm.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/ships/test_ships.py` & `tropycal-1.0.2/tests/ships/test_ships.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/tracks/test_dataset.py` & `tropycal-1.0.2/tests/tracks/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/tracks/test_season.py` & `tropycal-1.0.2/tests/tracks/test_season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/tracks/test_storm.py` & `tropycal-1.0.2/tests/tracks/test_storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0.1/tests/utils/test_utils.py` & `tropycal-1.0.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

