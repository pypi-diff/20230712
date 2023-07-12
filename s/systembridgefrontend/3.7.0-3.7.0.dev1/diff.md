# Comparing `tmp/systembridgefrontend-3.7.0.tar.gz` & `tmp/systembridgefrontend-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgefrontend-3.7.0.tar", last modified: Wed Jul 12 10:23:18 2023, max compression
+gzip compressed data, was "systembridgefrontend-3.7.0.dev1.tar", last modified: Mon Jul  3 08:34:58 2023, max compression
```

## Comparing `systembridgefrontend-3.7.0.tar` & `systembridgefrontend-3.7.0.dev1.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.883567 systembridgefrontend-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 10:23:18.883567 systembridgefrontend-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:23:18.883567 systembridgefrontend-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.851567 systembridgefrontend-3.7.0/systembridgefrontend/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/systembridgefrontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/systembridgefrontend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.855567 systembridgefrontend-3.7.0/systembridgefrontend/out/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.847567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.851567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.855567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.871567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    60440 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/142-e96944db890d0712.js
--rw-r--r--   0 runner    (1001) docker     (123)    51206 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js
--rw-r--r--   0 runner    (1001) docker     (123)   116342 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js
--rw-r--r--   0 runner    (1001) docker     (123)    69763 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js
--rw-r--r--   0 runner    (1001) docker     (123)    54369 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/514-a199f049b736895b.js
--rw-r--r--   0 runner    (1001) docker     (123)    69859 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/699-e1dda1328195ce40.js
--rw-r--r--   0 runner    (1001) docker     (123)    56876 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/713-307f96321a681e2c.js
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/731-adbd7bf9e28fe493.js
--rw-r--r--   0 runner    (1001) docker     (123)    58330 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/767-13c0b6c8b2e638dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/839-49c1e145187c690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   141023 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js
--rw-r--r--   0 runner    (1001) docker     (123)    98360 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/main-bfbd70c9b9a5a25b.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.871567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    51899 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.871567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.871567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-6924375f59017114.js
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-0fcd948dd1ceee0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/data-bf9ec2c59e015b44.js
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/notification-b76a6b7af2e3a0c9.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.875567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-377fb73a175a7afa.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-dd8ee3c5bcd7fd5a.js
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/settings-734d9ba521512578.js
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
--rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.875567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.879567 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-12 10:23:03.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.879567 systembridgefrontend-3.7.0/systembridgefrontend/out/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.879567 systembridgefrontend-3.7.0/systembridgefrontend/out/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/bridges/openon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/bridges/setup.html
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/data.html
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/notification.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.883567 systembridgefrontend-3.7.0/systembridgefrontend/out/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/player/audio.html
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/player/video.html
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-12 10:23:04.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/app/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-12 10:23:02.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-12 10:23:01.000000 systembridgefrontend-3.7.0/systembridgefrontend/out/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:18.855567 systembridgefrontend-3.7.0/systembridgefrontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 10:23:18.000000 systembridgefrontend-3.7.0/systembridgefrontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-12 10:23:18.000000 systembridgefrontend-3.7.0/systembridgefrontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:23:18.000000 systembridgefrontend-3.7.0/systembridgefrontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 10:23:18.000000 systembridgefrontend-3.7.0/systembridgefrontend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:34:58.345780 systembridgefrontend-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 08:34:56.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.321779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.321779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.333779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    60440 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51206 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)   116342 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69766 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50639 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69782 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58330 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56873 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141023 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95829 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    51895 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/openon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/notification.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/audio.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/video.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/top_level.txt
```

### Comparing `systembridgefrontend-3.7.0/pyproject.toml` & `systembridgefrontend-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/setup.py` & `systembridgefrontend-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/404.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/404.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
-self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, d, n, f, u, b) {
+self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, n, b, d, f, u) {
     return {
         __rewrites: {
             beforeFiles: [],
             afterFiles: [],
             fallback: []
         },
         "/": [s, a, "static/chunks/pages/index-f934b9a030f633a0.js"],
         "/_error": ["static/chunks/pages/_error-54de1933a164a1ff.js"],
-        "/app/bridges/openon": [s, a, c, e, t, p, d, "static/chunks/pages/app/bridges/openon-6924375f59017114.js"],
-        "/app/bridges/setup": [s, a, c, e, t, p, n, "static/chunks/pages/app/bridges/setup-0fcd948dd1ceee0b.js"],
-        "/app/data": [s, a, e, i, "static/chunks/731-adbd7bf9e28fe493.js", "static/chunks/pages/app/data-bf9ec2c59e015b44.js"],
-        "/app/notification": [s, a, p, "static/chunks/pages/app/notification-b76a6b7af2e3a0c9.js"],
-        "/app/player/audio": [s, f, a, c, i, u, b, "static/chunks/pages/app/player/audio-377fb73a175a7afa.js"],
-        "/app/player/video": [s, f, a, c, i, u, b, "static/chunks/pages/app/player/video-dd8ee3c5bcd7fd5a.js"],
-        "/app/settings": [s, "static/chunks/29107295-809b6f0b05884bf7.js", a, c, e, t, d, n, "static/chunks/826-e44464776abed9eb.js", "static/chunks/pages/app/settings-734d9ba521512578.js"],
+        "/app/bridges/openon": [s, a, c, e, p, i, n, "static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js"],
+        "/app/bridges/setup": [s, a, c, e, p, i, b, "static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js"],
+        "/app/data": [s, t, a, e, "static/chunks/731-eb947eaba8f94f26.js", "static/chunks/pages/app/data-a3eeebdc39c5f892.js"],
+        "/app/notification": [s, a, i, "static/chunks/pages/app/notification-0384bbf9e77dbfb4.js"],
+        "/app/player/audio": [s, t, d, a, c, f, u, "static/chunks/pages/app/player/audio-8b29e9945ddce62c.js"],
+        "/app/player/video": [s, t, d, a, c, f, u, "static/chunks/pages/app/player/video-b8b2ae3418f95cef.js"],
+        "/app/settings": [s, t, a, c, e, p, n, b, "static/chunks/826-e44464776abed9eb.js", "static/chunks/pages/app/settings-0b5df1a27de4507f.js"],
         sortedPages: ["/", "/_app", "/_error", "/app/bridges/openon", "/app/bridges/setup", "/app/data", "/app/notification", "/app/player/audio", "/app/player/video", "/app/settings"]
     }
-}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-8b4cf5ad285047cd.js", "static/chunks/839-49c1e145187c690b.js", "static/chunks/498-112306b4f8cd81ec.js", "static/chunks/699-e1dda1328195ce40.js", "static/chunks/154-7942dd40332ec4bf.js", "static/chunks/361-70173883768cacf6.js", "static/chunks/713-307f96321a681e2c.js", "static/chunks/767-13c0b6c8b2e638dd.js", "static/chunks/75fc9c18-058f7f136d59a7a6.js", "static/chunks/514-a199f049b736895b.js", "static/chunks/142-e96944db890d0712.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
+}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-8b4cf5ad285047cd.js", "static/chunks/418-f078369e2fd2524e.js", "static/chunks/498-112306b4f8cd81ec.js", "static/chunks/29107295-8f8fd7e7e27aa6a2.js", "static/chunks/699-1a88a588882ce475.js", "static/chunks/154-7942dd40332ec4bf.js", "static/chunks/913-948b3bc7b49750f4.js", "static/chunks/767-b6df483a2f96f15d.js", "static/chunks/75fc9c18-058f7f136d59a7a6.js", "static/chunks/633-a2b446f38d34df6a.js", "static/chunks/142-b511304dc754f6ca.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/142-e96944db890d0712.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -244,119 +244,116 @@
                 }
             }
         },
         630: function(e, t, n) {
             let s;
             n.d(t, {
                 Z: function() {
-                    return I
+                    return E
                 }
             });
             var o = n(5893),
                 i = n(7294),
                 a = n(6885),
-                r = n(361),
-                l = n.n(r),
-                c = n(8446),
-                u = n.n(c),
-                d = n(8096),
-                p = n(8995),
-                m = n(6018),
-                h = n(2734),
-                y = n(6886),
-                x = n(7357),
-                g = n(2022),
-                v = n(6628),
-                b = n(5861),
-                k = n(3946),
-                f = n(5929),
-                w = n(8849),
-                j = n(5317),
-                S = n(381),
-                P = n.n(S),
-                E = n(6310),
-                C = function() {
-                    let [e, t] = (0, d.nn)(), [n, s] = (0, i.useState)(!1), [a, r] = (0, d.XI)(), l = (0, i.useRef)(null), {
-                        duration: c,
-                        playing: u,
-                        muted: p,
-                        loaded: m,
-                        position: S,
+                r = n(6486),
+                l = n(8096),
+                c = n(8995),
+                u = n(6018),
+                d = n(2734),
+                p = n(6886),
+                m = n(7357),
+                h = n(2022),
+                y = n(6628),
+                x = n(5861),
+                g = n(3946),
+                v = n(3754),
+                b = n(8849),
+                k = n(5317),
+                f = n(381),
+                w = n.n(f),
+                j = n(6310),
+                S = function() {
+                    let [e, t] = (0, l.nn)(), [n, s] = (0, i.useState)(!1), [a, r] = (0, l.XI)(), c = (0, i.useRef)(null), {
+                        duration: u,
+                        playing: f,
+                        muted: S,
+                        loaded: P,
+                        position: E,
                         volume: C
                     } = (0, i.useMemo)(() => e, [e]), Z = (0, i.useMemo)(() => "".concat((100 * C).toFixed(0), "%"), [C]), I = (0, i.useMemo)(() => {
-                        let e = P().duration(S, "seconds");
+                        let e = w().duration(E, "seconds");
                         return "".concat(e.minutes().toString().padStart(2, "0"), ":").concat(e.seconds().toString().padStart(2, "0"))
-                    }, [S]), M = (0, i.useMemo)(() => {
-                        let e = P().duration(c, "seconds");
+                    }, [E]), D = (0, i.useMemo)(() => {
+                        let e = w().duration(u, "seconds");
                         return "".concat(e.minutes().toString().padStart(2, "0"), ":").concat(e.seconds().toString().padStart(2, "0"))
-                    }, [c]), {
-                        artist: N,
-                        album: _,
-                        cover: A,
-                        source: D,
+                    }, [u]), {
+                        artist: M,
+                        album: N,
+                        cover: _,
+                        source: A,
                         title: O
                     } = (0, i.useMemo)(() => e.source, [e]), T = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             loaded: n
                         })
                     }, [e, t]), L = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             playing: n
                         })
                     }, [e, t]), U = (0, i.useCallback)(() => {
-                        L(!u)
-                    }, [u, L]), K = (0, i.useCallback)(n => {
+                        L(!f)
+                    }, [f, L]), K = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             muted: n
                         })
                     }, [e, t]), R = (0, i.useCallback)(() => {
-                        K(!p)
-                    }, [p, K]), W = (0, i.useCallback)((n, s) => {
+                        K(!S)
+                    }, [S, K]), W = (0, i.useCallback)((n, s) => {
                         let o = "down" === s ? C - n : "up" === s ? C + n : n;
                         o > 1 && (o = 1), o < 0 && (o = 0), t({
                             ...e,
                             volume: o
-                        }), p && K(!1)
-                    }, [p, C, e, t, K]), q = (0, i.useCallback)(n => {
+                        }), S && K(!1)
+                    }, [S, C, e, t, K]), q = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             duration: n
                         })
                     }, [e, t]), z = (0, i.useCallback)(n => {
-                        c && n > c && (n = c), n < 0 && (n = 0), t({
+                        u && n > u && (n = u), n < 0 && (n = 0), t({
                             ...e,
                             position: n
                         })
-                    }, [e, c, t]), F = (0, i.useCallback)(e => {
+                    }, [e, u, t]), F = (0, i.useCallback)(e => {
                         var t;
-                        null === (t = l.current) || void 0 === t || t.seekTo(e, "seconds"), s(!1), u || L(!0)
-                    }, [u, L]);
+                        null === (t = c.current) || void 0 === t || t.seekTo(e, "seconds"), s(!1), f || L(!0)
+                    }, [f, L]);
 
                     function G() {
                         L(!1), s(!0)
                     }
 
                     function B() {
-                        S && F(S)
+                        E && F(E)
                     }(0, i.useEffect)(() => {
-                        m || T(!0)
-                    }, [m, T, L]);
-                    let J = (0, h.Z)();
+                        P || T(!0)
+                    }, [P, T, L]);
+                    let J = (0, d.Z)();
                     return (0, o.jsxs)(o.Fragment, {
-                        children: [(0, o.jsx)(E.Z, {
-                            ref: l,
+                        children: [(0, o.jsx)(j.Z, {
+                            ref: c,
                             height: "0px",
                             width: "0px",
-                            muted: p,
-                            playing: u,
+                            muted: S,
+                            playing: f,
                             stopOnUnmount: !0,
-                            url: D,
+                            url: A,
                             volume: C,
                             onDuration: e => {
                                 q(e)
                             },
                             onPause: () => {
                                 L(!1)
                             },
@@ -368,203 +365,203 @@
                             },
                             onProgress: e => {
                                 let {
                                     playedSeconds: t
                                 } = e;
                                 n || z(t)
                             }
-                        }), (0, o.jsxs)(y.ZP, {
+                        }), (0, o.jsxs)(p.ZP, {
                             container: !0,
                             direction: "row",
                             alignItems: "center",
                             justifyItems: "center",
                             wrap: "nowrap",
                             sx: {
                                 height: 140,
                                 width: 540,
                                 overflow: "hidden"
                             },
-                            children: [(0, o.jsx)(y.ZP, {
+                            children: [(0, o.jsx)(p.ZP, {
                                 item: !0,
                                 sx: {
                                     width: 140,
                                     margin: J.spacing(0, 1, 0, 0)
                                 },
-                                children: (0, o.jsx)(x.Z, {
+                                children: (0, o.jsx)(m.Z, {
                                     ref: a,
-                                    children: (0, o.jsxs)(g.Z, {
-                                        "aria-label": u ? "Pause" : "Play",
+                                    children: (0, o.jsxs)(h.Z, {
+                                        "aria-label": f ? "Pause" : "Play",
                                         onClick: U,
                                         children: [(0, o.jsx)("img", {
-                                            alt: "".concat(N, " - ").concat(_),
-                                            src: A || "https://raw.githubusercontent.com/timmo001/system-bridge/master/resources/system-bridge-dimmed.svg",
+                                            alt: "".concat(M, " - ").concat(N),
+                                            src: _ || "https://raw.githubusercontent.com/timmo001/system-bridge/master/resources/system-bridge-dimmed.svg",
                                             width: 140
-                                        }), (0, o.jsx)(v.Z, {
+                                        }), (0, o.jsx)(y.Z, {
                                             in: !!r,
                                             timeout: {
                                                 enter: 200,
                                                 exit: 400
                                             },
-                                            children: (0, o.jsx)(x.Z, {
+                                            children: (0, o.jsx)(m.Z, {
                                                 sx: {
                                                     position: "absolute",
                                                     display: "flex",
                                                     height: "100%",
                                                     width: "100%",
                                                     zIndex: 100
                                                 },
-                                                children: (0, o.jsx)(w.Icon, {
-                                                    id: u ? "pause" : "play",
-                                                    path: u ? j.Wa1 : j._86,
+                                                children: (0, o.jsx)(b.Icon, {
+                                                    id: f ? "pause" : "play",
+                                                    path: f ? k.Wa1 : k._86,
                                                     size: 6,
                                                     style: {
                                                         position: "relative",
                                                         margin: "auto"
                                                     }
                                                 })
                                             })
                                         })]
                                     })
                                 })
-                            }), (0, o.jsx)(y.ZP, {
+                            }), (0, o.jsx)(p.ZP, {
                                 item: !0,
                                 xs: !0,
-                                children: (0, o.jsxs)(y.ZP, {
+                                children: (0, o.jsxs)(p.ZP, {
                                     container: !0,
                                     direction: "column",
                                     alignItems: "flex-start",
                                     justifyItems: "space-around",
-                                    children: [(0, o.jsx)(y.ZP, {
+                                    children: [(0, o.jsx)(p.ZP, {
                                         item: !0,
-                                        children: (0, o.jsxs)(b.Z, {
+                                        children: (0, o.jsxs)(x.Z, {
                                             color: "textPrimary",
                                             component: "span",
                                             variant: "subtitle1",
                                             noWrap: !0,
-                                            children: [N, " - ", O]
+                                            children: [M, " - ", O]
                                         })
-                                    }), (0, o.jsx)(y.ZP, {
+                                    }), (0, o.jsx)(p.ZP, {
                                         item: !0,
-                                        children: (0, o.jsx)(b.Z, {
+                                        children: (0, o.jsx)(x.Z, {
                                             color: "textSecondary",
                                             component: "span",
                                             variant: "subtitle2",
                                             noWrap: !0,
-                                            children: _
+                                            children: N
                                         })
-                                    }), (0, o.jsxs)(y.ZP, {
+                                    }), (0, o.jsxs)(p.ZP, {
                                         item: !0,
                                         container: !0,
                                         alignContent: "center",
-                                        children: [(0, o.jsx)(y.ZP, {
+                                        children: [(0, o.jsx)(p.ZP, {
                                             item: !0,
                                             xs: 4
-                                        }), (0, o.jsx)(y.ZP, {
+                                        }), (0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(0, 1, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(k.Z, {
+                                            children: (0, o.jsx)(g.Z, {
                                                 size: "small",
                                                 onClick: R,
-                                                children: p ? (0, o.jsx)(w.Icon, {
+                                                children: S ? (0, o.jsx)(b.Icon, {
                                                     id: "mute",
-                                                    path: j.PLS,
+                                                    path: k.PLS,
                                                     size: 1.25
-                                                }) : (0, o.jsx)(w.Icon, {
+                                                }) : (0, o.jsx)(b.Icon, {
                                                     id: "unmute",
-                                                    path: j.dw,
+                                                    path: k.dw,
                                                     size: 1.25
                                                 })
                                             })
-                                        }), (0, o.jsx)(y.ZP, {
+                                        }), (0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(.6, 2, 0, 0)
                                             },
                                             item: !0,
                                             xs: !0,
-                                            children: (0, o.jsx)(f.ZP, {
+                                            children: (0, o.jsx)(v.ZP, {
                                                 min: 0,
                                                 max: 1,
                                                 step: .01,
                                                 value: C,
                                                 onChange: (e, t) => {
                                                     "number" == typeof t && W(t)
                                                 }
                                             })
-                                        }), (0, o.jsx)(y.ZP, {
+                                        }), (0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(.9, C >= 1 ? 1 : 2, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(b.Z, {
+                                            children: (0, o.jsx)(x.Z, {
                                                 component: "span",
                                                 variant: "body2",
                                                 children: Z
                                             })
                                         })]
-                                    }), (0, o.jsxs)(y.ZP, {
+                                    }), (0, o.jsxs)(p.ZP, {
                                         container: !0,
-                                        children: [(0, o.jsx)(y.ZP, {
+                                        children: [(0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(.25, 2, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(b.Z, {
+                                            children: (0, o.jsx)(x.Z, {
                                                 component: "span",
                                                 variant: "body2",
                                                 children: I
                                             })
-                                        }), (0, o.jsx)(y.ZP, {
+                                        }), (0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(0, 2, 0, 0)
                                             },
                                             item: !0,
                                             xs: !0,
-                                            children: (0, o.jsx)(f.ZP, {
+                                            children: (0, o.jsx)(v.ZP, {
                                                 min: 0,
-                                                max: c,
+                                                max: u,
                                                 step: .1,
-                                                value: S,
+                                                value: E,
                                                 valueLabelDisplay: "off",
                                                 onMouseDown: G,
                                                 onKeyDown: G,
                                                 onChange: function(e, t) {
                                                     z(t)
                                                 },
                                                 onMouseUp: B,
                                                 onKeyUp: B
                                             })
-                                        }), (0, o.jsx)(y.ZP, {
+                                        }), (0, o.jsx)(p.ZP, {
                                             sx: {
                                                 margin: J.spacing(.25, 1, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(b.Z, {
+                                            children: (0, o.jsx)(x.Z, {
                                                 component: "span",
                                                 variant: "body2",
-                                                children: M
+                                                children: D
                                             })
                                         })]
                                     })]
                                 })
                             })]
                         })]
                     })
                 },
-                Z = function() {
-                    let [e, t] = (0, d.nn)(), {
+                P = function() {
+                    let [e, t] = (0, l.nn)(), {
                         autoplay: n,
                         duration: s,
                         playing: a,
                         muted: r,
-                        loaded: l,
-                        volume: c
+                        loaded: c,
+                        volume: u
                     } = (0, i.useMemo)(() => e, [e]), {
-                        source: u
+                        source: d
                     } = (0, i.useMemo)(() => e.source, [e]), p = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             loaded: n
                         })
                     }, [e, t]), m = (0, i.useCallback)(n => {
                         console.log("Set playing:", n), t({
@@ -574,43 +571,43 @@
                     }, [e, t]), h = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             muted: n
                         })
                     }, [e, t]);
                     (0, i.useCallback)((n, s) => {
-                        let o = "down" === s ? c - n : "up" === s ? c + n : n;
+                        let o = "down" === s ? u - n : "up" === s ? u + n : n;
                         o > 1 && (o = 1), o < 0 && (o = 0), t({
                             ...e,
                             volume: o
                         }), r && h(!1)
-                    }, [r, c, e, t, h]);
+                    }, [r, u, e, t, h]);
                     let y = (0, i.useCallback)(n => t({
                             ...e,
                             duration: n
                         }), [e, t]),
                         x = (0, i.useCallback)(n => {
                             s && n > s && (n = s), n < 0 && (n = 0), t({
                                 ...e,
                                 position: n
                             })
                         }, [e, s, t]);
                     return (0, i.useEffect)(() => {
-                        l || p(!0)
-                    }, [l, p]), (0, o.jsx)(o.Fragment, {
-                        children: (0, o.jsx)(E.Z, {
+                        c || p(!0)
+                    }, [c, p]), (0, o.jsx)(o.Fragment, {
+                        children: (0, o.jsx)(j.Z, {
                             autoPlay: n,
                             controls: !0,
                             height: "270px",
                             width: "480px",
                             playsinline: !0,
                             muted: r,
                             playing: a,
-                            url: u,
-                            volume: c,
+                            url: d,
+                            volume: u,
                             style: {
                                 position: "absolute",
                                 top: "0",
                                 left: "0",
                                 overflow: "hidden"
                             },
                             onReady: () => {
@@ -625,126 +622,126 @@
                                     playedSeconds: t
                                 } = e;
                                 return x(t)
                             }
                         })
                     })
                 },
-                I = function(e) {
+                E = function(e) {
                     let {
                         playerType: t
-                    } = e, [n, r] = (0, i.useState)(!1), [c, h] = (0, d.nn)(), y = (0, p.D)(c), x = (0, a.useRouter)(), g = x.query, v = (0, i.useCallback)(e => {
+                    } = e, [n, d] = (0, i.useState)(!1), [p, m] = (0, l.nn)(), h = (0, c.D)(p), y = (0, a.useRouter)(), x = y.query, g = (0, i.useCallback)(e => {
                         switch (console.log("Event:", e), e.type) {
                             case "MEDIA_PAUSE":
-                                h({
-                                    ...c,
+                                m({
+                                    ...p,
                                     playing: !1
                                 });
                                 break;
                             case "MEDIA_PLAY":
-                                h({
-                                    ...c,
+                                m({
+                                    ...p,
                                     playing: !0
                                 });
                                 break;
                             case "MEDIA_VOLUME_DOWN":
-                                e.volume && h({
-                                    ...c,
-                                    volume: c.volume - e.volume
+                                e.volume && m({
+                                    ...p,
+                                    volume: p.volume - e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_UP":
-                                e.volume && h({
-                                    ...c,
-                                    volume: c.volume + e.volume
+                                e.volume && m({
+                                    ...p,
+                                    volume: p.volume + e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_SET":
-                                e.volume && h({
-                                    ...c,
+                                e.volume && m({
+                                    ...p,
                                     volume: e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_SET":
-                                e.position && h({
-                                    ...c,
+                                e.position && m({
+                                    ...p,
                                     position: e.position
                                 })
                         }
-                    }, [c, h]), b = (0, i.useCallback)((e, t) => {
-                        console.log("Setup WebSocketConnection"), (s = new m.C(e, t, async () => {
+                    }, [p, m]), v = (0, i.useCallback)((e, t) => {
+                        console.log("Setup WebSocketConnection"), (s = new u.C(e, t, async () => {
                             console.log("Connected to WebSocket")
-                        })).onEvent = v
-                    }, [v]);
+                        })).onEvent = g
+                    }, [g]);
                     (0, i.useEffect)(() => {
-                        !n && g && g.apiKey && (r(!0), b(Number(g.apiPort) || 9170, String(g.apiKey)))
-                    }, [n, b, g]), (0, i.useEffect)(() => {
-                        if (!c && x.isReady) {
+                        !n && x && x.apiKey && (d(!0), v(Number(x.apiPort) || 9170, String(x.apiKey)))
+                    }, [n, v, x]), (0, i.useEffect)(() => {
+                        if (!p && y.isReady) {
                             var e, n;
-                            let s = Number(g.volume);
+                            let s = Number(x.volume);
                             switch (t) {
                                 default:
                                     break;
                                 case "audio":
-                                    h({
-                                        autoplay: (null === (e = g.autoplay) || void 0 === e ? void 0 : e.toLowerCase()) === "true",
+                                    m({
+                                        autoplay: (null === (e = x.autoplay) || void 0 === e ? void 0 : e.toLowerCase()) === "true",
                                         muted: !1,
                                         playing: !1,
                                         loaded: !1,
                                         position: 0,
                                         duration: 1,
                                         source: {
                                             type: "audio",
-                                            source: g.url,
-                                            album: g.album || "Unknown Album",
-                                            artist: g.artist || "Unknown Aritst",
-                                            cover: g.cover,
-                                            title: g.title || "Unknown Title",
+                                            source: x.url,
+                                            album: x.album || "Unknown Album",
+                                            artist: x.artist || "Unknown Aritst",
+                                            cover: x.cover,
+                                            title: x.title || "Unknown Title",
                                             volumeInitial: (s > 0 ? s : 40) / 100
                                         },
                                         volume: (s > 0 ? s : 40) / 100
                                     });
                                     break;
                                 case "video":
-                                    h({
-                                        autoplay: (null === (n = g.autoplay) || void 0 === n ? void 0 : n.toLowerCase()) === "true",
+                                    m({
+                                        autoplay: (null === (n = x.autoplay) || void 0 === n ? void 0 : n.toLowerCase()) === "true",
                                         muted: !1,
                                         playing: !1,
                                         loaded: !1,
                                         position: 0,
                                         duration: 1,
                                         source: {
                                             type: "video",
-                                            source: String(g.url),
+                                            source: String(x.url),
                                             volumeInitial: (s > 0 ? s : 40) / 100
                                         },
                                         volume: (s > 0 ? s : 40) / 100
                                     })
                             }
                         }
-                    }, [c, h, t, x, g]), (0, i.useEffect)(() => {
-                        if (c) {
+                    }, [p, m, t, y, x]), (0, i.useEffect)(() => {
+                        if (p) {
                             let e;
-                            y && "audio" === (e = l()(y)).source.type && delete e.source.cover;
-                            let t = l()(c);
-                            if ("audio" === t.source.type && delete t.source.cover, !u()(t, e)) {
+                            h && "audio" === (e = (0, r.cloneDeep)(h)).source.type && delete e.source.cover;
+                            let t = (0, r.cloneDeep)(p);
+                            if ("audio" === t.source.type && delete t.source.cover, !(0, r.isEqual)(t, e)) {
                                 if (console.log("Player update\n\npreviousStatus:", e, "\nnewStatus:", t), !t.loaded || !s) return;
                                 if (!s.isConnected()) {
-                                    r(!1), console.warn("WebSocket not connected");
+                                    d(!1), console.warn("WebSocket not connected");
                                     return
                                 }
                                 s.sendPlayerStatus(t)
                             }
                         }
-                    }, [c, y]);
-                    let k = (0, i.useMemo)(() => {
-                        if (c) return c.source.type
-                    }, [c]);
+                    }, [p, h]);
+                    let b = (0, i.useMemo)(() => {
+                        if (p) return p.source.type
+                    }, [p]);
                     return (0, o.jsx)(o.Fragment, {
-                        children: "audio" === k ? (0, o.jsx)(C, {}) : "video" === k ? (0, o.jsx)(Z, {}) : ""
+                        children: "audio" === b ? (0, o.jsx)(S, {}) : "video" === b ? (0, o.jsx)(P, {}) : ""
                     })
                 }
         },
         8096: function(e, t, n) {
             n.d(t, {
                 I0: function() {
                     return r
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1672,16 +1672,17 @@
                                 return t
                             }
                         }
 
                         function eQ(n) {
                             return function(t) {
                                 var r = tF(t = oi(t)) ? tV(t) : u,
-                                    e = r ? e$(r, 1).join("") : t.slice(1);
-                                return (r ? r[0] : t.charAt(0))[n]() + e
+                                    e = r ? r[0] : t.charAt(0),
+                                    i = r ? e$(r, 1).join("") : t.slice(1);
+                                return e[n]() + i
                             }
                         }
 
                         function eX(n) {
                             return function(t) {
                                 return ty(o$(oz(t).replace(nq, "")), n, "")
                             }
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/514-a199f049b736895b.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [514], {
-        5929: function(e, t, r) {
+    [633], {
+        3754: function(e, t, r) {
             "use strict";
             let n;
             r.d(t, {
                 ZP: function() {
                     return G
                 }
             });
-            var o = r(3366),
-                a = r(7462),
-                i = r(7294),
-                l = r(6010),
+            var a = r(3366),
+                o = r(7462),
+                l = r(7294),
+                i = r(6010),
                 u = r(4780),
-                s = r(6504),
-                c = r(8442),
-                f = r(2690),
-                d = r(9032),
+                s = r(3249),
+                c = r(3247),
+                d = r(2690),
+                f = r(9032),
                 p = r(9962),
                 y = r(3703),
                 h = r(3546),
-                v = r(9948),
-                m = {
+                m = r(9948),
+                v = {
                     border: 0,
                     clip: "rect(0 0 0 0)",
                     height: "1px",
                     margin: -1,
                     overflow: "hidden",
                     padding: 0,
                     position: "absolute",
@@ -42,17 +42,17 @@
             }
 
             function P(e, t) {
                 var r;
                 let {
                     index: n
                 } = null != (r = e.reduce((e, r, n) => {
-                    let o = Math.abs(t - r);
-                    return null === e || o < e.distance || o === e.distance ? {
-                        distance: o,
+                    let a = Math.abs(t - r);
+                    return null === e || a < e.distance || a === e.distance ? {
+                        distance: a,
                         index: n
                     } : e
                 }, null)) ? r : {};
                 return n
             }
 
             function w(e, t) {
@@ -77,30 +77,30 @@
                 newValue: t,
                 index: r
             }) {
                 let n = e.slice();
                 return n[r] = t, n.sort(b)
             }
 
-            function O({
+            function S({
                 sliderRef: e,
                 activeIndex: t,
                 setActive: r
             }) {
-                var n, o, a;
-                let i = (0, f.Z)(e.current);
-                null != (n = e.current) && n.contains(i.activeElement) && Number(null == i ? void 0 : null == (o = i.activeElement) ? void 0 : o.getAttribute("data-index")) === t || null == (a = e.current) || a.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
+                var n, a, o;
+                let l = (0, d.Z)(e.current);
+                null != (n = e.current) && n.contains(l.activeElement) && Number(null == l ? void 0 : null == (a = l.activeElement) ? void 0 : a.getAttribute("data-index")) === t || null == (o = e.current) || o.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
             }
 
-            function S(e, t) {
+            function O(e, t) {
                 return "number" == typeof e && "number" == typeof t ? e === t : "object" == typeof e && "object" == typeof t && function(e, t, r = (e, t) => e === t) {
                     return e.length === t.length && e.every((e, n) => r(e, t[n]))
                 }(e, t)
             }
-            let _ = {
+            let x = {
                     horizontal: {
                         offset: e => ({
                             left: `${e}%`
                         }),
                         leap: e => ({
                             width: `${e}%`
                         })
@@ -118,38 +118,38 @@
                             bottom: `${e}%`
                         }),
                         leap: e => ({
                             height: `${e}%`
                         })
                     }
                 },
-                x = e => e;
+                _ = e => e;
 
             function A() {
                 return void 0 === n && (n = "undefined" == typeof CSS || "function" != typeof CSS.supports || CSS.supports("touch-action", "none")), n
             }
             var T = r(1796),
-                j = r(1657),
+                C = r(1657),
                 E = r(948),
                 L = r(2734),
-                C = e => !e || !(0, c.Z)(e),
-                R = r(8216),
+                R = e => !e || !(0, c.Z)(e),
+                j = r(8216),
                 M = r(1588),
                 I = r(4867);
 
             function Z(e) {
                 return (0, I.Z)("MuiSlider", e)
             }
             let z = (0, M.Z)("MuiSlider", ["root", "active", "colorPrimary", "colorSecondary", "disabled", "dragging", "focusVisible", "mark", "markActive", "marked", "markLabel", "markLabelActive", "rail", "sizeSmall", "thumb", "thumbColorPrimary", "thumbColorSecondary", "track", "trackInverted", "trackFalse", "thumbSizeSmall", "valueLabel", "valueLabelOpen", "valueLabelCircle", "valueLabelLabel", "vertical"]);
             var D = r(5893);
             let N = e => {
                     let {
                         open: t
                     } = e, r = {
-                        offset: (0, l.Z)(t && z.valueLabelOpen),
+                        offset: (0, i.Z)(t && z.valueLabelOpen),
                         circle: z.valueLabelCircle,
                         label: z.valueLabelLabel
                     };
                     return r
                 },
                 U = ["aria-label", "aria-valuetext", "aria-labelledby", "component", "components", "componentsProps", "color", "classes", "className", "disableSwap", "disabled", "getAriaLabel", "getAriaValueText", "marks", "max", "min", "name", "onChange", "onChangeCommitted", "orientation", "size", "step", "scale", "slotProps", "slots", "tabIndex", "track", "value", "valueLabelDisplay", "valueLabelFormat"];
 
@@ -159,40 +159,40 @@
             let H = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: r
                         } = e;
-                        return [t.root, t[`color${(0,R.Z)(r.color)}`], "medium" !== r.size && t[`size${(0,R.Z)(r.size)}`], r.marked && t.marked, "vertical" === r.orientation && t.vertical, "inverted" === r.track && t.trackInverted, !1 === r.track && t.trackFalse]
+                        return [t.root, t[`color${(0,j.Z)(r.color)}`], "medium" !== r.size && t[`size${(0,j.Z)(r.size)}`], r.marked && t.marked, "vertical" === r.orientation && t.vertical, "inverted" === r.track && t.trackInverted, !1 === r.track && t.trackFalse]
                     }
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, a.Z)({
+                }) => (0, o.Z)({
                     borderRadius: 12,
                     boxSizing: "content-box",
                     display: "inline-block",
                     position: "relative",
                     cursor: "pointer",
                     touchAction: "none",
                     color: (e.vars || e).palette[t.color].main,
                     WebkitTapHighlightColor: "transparent"
-                }, "horizontal" === t.orientation && (0, a.Z)({
+                }, "horizontal" === t.orientation && (0, o.Z)({
                     height: 4,
                     width: "100%",
                     padding: "13px 0",
                     "@media (pointer: coarse)": {
                         padding: "20px 0"
                     }
                 }, "small" === t.size && {
                     height: 2
                 }, t.marked && {
                     marginBottom: 20
-                }), "vertical" === t.orientation && (0, a.Z)({
+                }), "vertical" === t.orientation && (0, o.Z)({
                     height: "100%",
                     width: 4,
                     padding: "0 13px",
                     "@media (pointer: coarse)": {
                         padding: "0 20px"
                     }
                 }, "small" === t.size && {
@@ -216,15 +216,15 @@
                 })),
                 V = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Rail",
                     overridesResolver: (e, t) => t.rail
                 })(({
                     ownerState: e
-                }) => (0, a.Z)({
+                }) => (0, o.Z)({
                     display: "block",
                     position: "absolute",
                     borderRadius: "inherit",
                     backgroundColor: "currentColor",
                     opacity: .38
                 }, "horizontal" === e.orientation && {
                     width: "100%",
@@ -244,15 +244,15 @@
                     slot: "Track",
                     overridesResolver: (e, t) => t.track
                 })(({
                     theme: e,
                     ownerState: t
                 }) => {
                     let r = "light" === e.palette.mode ? (0, T.$n)(e.palette[t.color].main, .62) : (0, T._j)(e.palette[t.color].main, .5);
-                    return (0, a.Z)({
+                    return (0, o.Z)({
                         display: "block",
                         position: "absolute",
                         borderRadius: "inherit",
                         border: "1px solid currentColor",
                         backgroundColor: "currentColor",
                         transition: e.transitions.create(["left", "width", "bottom", "height"], {
                             duration: e.transitions.duration.shortest
@@ -277,20 +277,20 @@
                 B = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Thumb",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: r
                         } = e;
-                        return [t.thumb, t[`thumbColor${(0,R.Z)(r.color)}`], "medium" !== r.size && t[`thumbSize${(0,R.Z)(r.size)}`]]
+                        return [t.thumb, t[`thumbColor${(0,j.Z)(r.color)}`], "medium" !== r.size && t[`thumbSize${(0,j.Z)(r.size)}`]]
                     }
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, a.Z)({
+                }) => (0, o.Z)({
                     position: "absolute",
                     width: 20,
                     height: 20,
                     boxSizing: "border-box",
                     borderRadius: "50%",
                     outline: 0,
                     backgroundColor: "currentColor",
@@ -306,15 +306,15 @@
                 }, "horizontal" === t.orientation && {
                     top: "50%",
                     transform: "translate(-50%, -50%)"
                 }, "vertical" === t.orientation && {
                     left: "50%",
                     transform: "translate(-50%, 50%)"
                 }, {
-                    "&:before": (0, a.Z)({
+                    "&:before": (0, o.Z)({
                         position: "absolute",
                         content: '""',
                         borderRadius: "inherit",
                         width: "100%",
                         height: "100%",
                         boxShadow: (e.vars || e).shadows[2]
                     }, "small" === t.size && {
@@ -346,38 +346,38 @@
                     }
                 })),
                 W = (0, E.ZP)(function(e) {
                     let {
                         children: t,
                         className: r,
                         value: n
-                    } = e, o = N(e);
-                    return t ? i.cloneElement(t, {
-                        className: (0, l.Z)(t.props.className)
-                    }, (0, D.jsxs)(i.Fragment, {
+                    } = e, a = N(e);
+                    return t ? l.cloneElement(t, {
+                        className: (0, i.Z)(t.props.className)
+                    }, (0, D.jsxs)(l.Fragment, {
                         children: [t.props.children, (0, D.jsx)("span", {
-                            className: (0, l.Z)(o.offset, r),
+                            className: (0, i.Z)(a.offset, r),
                             "aria-hidden": !0,
                             children: (0, D.jsx)("span", {
-                                className: o.circle,
+                                className: a.circle,
                                 children: (0, D.jsx)("span", {
-                                    className: o.label,
+                                    className: a.label,
                                     children: n
                                 })
                             })
                         })]
                     })) : null
                 }, {
                     name: "MuiSlider",
                     slot: "ValueLabel",
                     overridesResolver: (e, t) => t.valueLabel
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, a.Z)({
+                }) => (0, o.Z)({
                     [`&.${z.valueLabelOpen}`]: {
                         transform: `${"vertical"===t.orientation?"translateY(-50%)":"translateY(-100%)"} scale(1)`
                     },
                     zIndex: 1,
                     whiteSpace: "nowrap"
                 }, e.typography.body2, {
                     fontWeight: 500,
@@ -434,15 +434,15 @@
                         } = e;
                         return [t.mark, r && t.markActive]
                     }
                 })(({
                     theme: e,
                     ownerState: t,
                     markActive: r
-                }) => (0, a.Z)({
+                }) => (0, o.Z)({
                     position: "absolute",
                     width: 2,
                     height: 2,
                     borderRadius: 1,
                     backgroundColor: "currentColor"
                 }, "horizontal" === t.orientation && {
                     top: "50%",
@@ -459,15 +459,15 @@
                     slot: "MarkLabel",
                     shouldForwardProp: e => (0, E.Dz)(e) && "markLabelActive" !== e,
                     overridesResolver: (e, t) => t.markLabel
                 })(({
                     theme: e,
                     ownerState: t,
                     markLabelActive: r
-                }) => (0, a.Z)({}, e.typography.body2, {
+                }) => (0, o.Z)({}, e.typography.body2, {
                     color: (e.vars || e).palette.text.secondary,
                     position: "absolute",
                     whiteSpace: "nowrap"
                 }, "horizontal" === t.orientation && {
                     top: 30,
                     transform: "translateX(-50%)",
                     "@media (pointer: coarse)": {
@@ -483,87 +483,87 @@
                     color: (e.vars || e).palette.text.primary
                 })),
                 K = e => {
                     let {
                         disabled: t,
                         dragging: r,
                         marked: n,
-                        orientation: o,
-                        track: a,
-                        classes: i,
-                        color: l,
+                        orientation: a,
+                        track: o,
+                        classes: l,
+                        color: i,
                         size: s
                     } = e, c = {
-                        root: ["root", t && "disabled", r && "dragging", n && "marked", "vertical" === o && "vertical", "inverted" === a && "trackInverted", !1 === a && "trackFalse", l && `color${(0,R.Z)(l)}`, s && `size${(0,R.Z)(s)}`],
+                        root: ["root", t && "disabled", r && "dragging", n && "marked", "vertical" === a && "vertical", "inverted" === o && "trackInverted", !1 === o && "trackFalse", i && `color${(0,j.Z)(i)}`, s && `size${(0,j.Z)(s)}`],
                         rail: ["rail"],
                         track: ["track"],
                         mark: ["mark"],
                         markActive: ["markActive"],
                         markLabel: ["markLabel"],
                         markLabelActive: ["markLabelActive"],
                         valueLabel: ["valueLabel"],
-                        thumb: ["thumb", t && "disabled", s && `thumbSize${(0,R.Z)(s)}`, l && `thumbColor${(0,R.Z)(l)}`],
+                        thumb: ["thumb", t && "disabled", s && `thumbSize${(0,j.Z)(s)}`, i && `thumbColor${(0,j.Z)(i)}`],
                         active: ["active"],
                         disabled: ["disabled"],
                         focusVisible: ["focusVisible"]
                     };
-                    return (0, u.Z)(c, Z, i)
+                    return (0, u.Z)(c, Z, l)
                 },
                 q = ({
                     children: e
                 }) => e,
-                J = i.forwardRef(function(e, t) {
-                    var r, n, u, T, E, R, M, I, Z, z, N, J, G, Q, ee, et, er, en, eo, ea, ei, el, eu, es;
-                    let ec = (0, j.Z)({
+                J = l.forwardRef(function(e, t) {
+                    var r, n, u, T, E, j, M, I, Z, z, N, J, G, Q, ee, et, er, en, ea, eo, el, ei, eu, es;
+                    let ec = (0, C.Z)({
                             props: e,
                             name: "MuiSlider"
                         }),
-                        ef = (0, L.Z)(),
-                        ed = "rtl" === ef.direction,
+                        ed = (0, L.Z)(),
+                        ef = "rtl" === ed.direction,
                         {
                             "aria-label": ep,
                             "aria-valuetext": ey,
                             "aria-labelledby": eh,
-                            component: ev = "span",
-                            components: em = {},
+                            component: em = "span",
+                            components: ev = {},
                             componentsProps: eb = {},
                             color: eg = "primary",
                             classes: eP,
                             className: ew,
                             disableSwap: ek = !1,
-                            disabled: eO = !1,
-                            getAriaLabel: eS,
-                            getAriaValueText: e_,
-                            marks: ex = !1,
+                            disabled: eS = !1,
+                            getAriaLabel: eO,
+                            getAriaValueText: ex,
+                            marks: e_ = !1,
                             max: eA = 100,
                             min: eT = 0,
-                            orientation: ej = "horizontal",
+                            orientation: eC = "horizontal",
                             size: eE = "medium",
                             step: eL = 1,
-                            scale: eC = $,
-                            slotProps: eR,
+                            scale: eR = $,
+                            slotProps: ej,
                             slots: eM,
                             track: eI = "normal",
                             valueLabelDisplay: eZ = "off",
                             valueLabelFormat: ez = $
                         } = ec,
-                        eD = (0, o.Z)(ec, U),
-                        eN = (0, a.Z)({}, ec, {
-                            isRtl: ed,
+                        eD = (0, a.Z)(ec, U),
+                        eN = (0, o.Z)({}, ec, {
+                            isRtl: ef,
                             max: eA,
                             min: eT,
                             classes: eP,
-                            disabled: eO,
+                            disabled: eS,
                             disableSwap: ek,
-                            orientation: ej,
-                            marks: ex,
+                            orientation: eC,
+                            marks: e_,
                             color: eg,
                             size: eE,
                             step: eL,
-                            scale: eC,
+                            scale: eR,
                             track: eI,
                             valueLabelDisplay: eZ,
                             valueLabelFormat: ez
                         }),
                         {
                             axisProps: eU,
                             getRootProps: e$,
@@ -574,124 +574,123 @@
                             axis: eW,
                             focusedThumbIndex: eX,
                             range: eY,
                             dragging: eK,
                             marks: eq,
                             values: eJ,
                             trackOffset: eG,
-                            trackLeap: eQ,
-                            getThumbStyle: e0
+                            trackLeap: eQ
                         } = function(e) {
                             let {
                                 "aria-labelledby": t,
                                 defaultValue: r,
                                 disabled: n = !1,
-                                disableSwap: o = !1,
-                                isRtl: l = !1,
+                                disableSwap: a = !1,
+                                isRtl: i = !1,
                                 marks: u = !1,
                                 max: s = 100,
                                 min: c = 0,
                                 name: T,
-                                onChange: j,
+                                onChange: C,
                                 onChangeCommitted: E,
                                 orientation: L = "horizontal",
-                                rootRef: C,
-                                scale: R = x,
+                                rootRef: R,
+                                scale: j = _,
                                 step: M = 1,
                                 tabIndex: I,
                                 value: Z
-                            } = e, z = i.useRef(), [D, N] = i.useState(-1), [U, $] = i.useState(-1), [H, V] = i.useState(!1), F = i.useRef(0), [B, W] = (0, d.Z)({
+                            } = e, z = l.useRef(), [D, N] = l.useState(-1), [U, $] = l.useState(-1), [H, V] = l.useState(!1), F = l.useRef(0), [B, W] = (0, f.Z)({
                                 controlled: Z,
                                 default: null != r ? r : c,
                                 name: "Slider"
-                            }), X = j && ((e, t, r) => {
+                            }), X = C && ((e, t, r) => {
                                 let n = e.nativeEvent || e,
-                                    o = new n.constructor(n.type, n);
-                                Object.defineProperty(o, "target", {
+                                    a = new n.constructor(n.type, n);
+                                Object.defineProperty(a, "target", {
                                     writable: !0,
                                     value: {
                                         value: t,
                                         name: T
                                     }
-                                }), j(o, t, r)
+                                }), C(a, t, r)
                             }), Y = Array.isArray(B), K = Y ? B.slice().sort(b) : [B];
                             K = K.map(e => g(e, c, s));
                             let q = !0 === u && null !== M ? [...Array(Math.floor((s - c) / M) + 1)].map((e, t) => ({
                                     value: c + M * t
                                 })) : u || [],
                                 J = q.map(e => e.value),
                                 {
                                     isFocusVisibleRef: G,
                                     onBlur: Q,
                                     onFocus: ee,
                                     ref: et
                                 } = (0, p.Z)(),
-                                [er, en] = i.useState(-1),
-                                eo = i.useRef(),
-                                ea = (0, y.Z)(et, eo),
-                                ei = (0, y.Z)(C, ea),
-                                el = e => t => {
+                                [er, en] = l.useState(-1),
+                                ea = l.useRef(),
+                                eo = (0, y.Z)(et, ea),
+                                el = (0, y.Z)(R, eo),
+                                ei = e => t => {
                                     var r;
                                     let n = Number(t.currentTarget.getAttribute("data-index"));
                                     ee(t), !0 === G.current && en(n), $(n), null == e || null == (r = e.onFocus) || r.call(e, t)
                                 },
                                 eu = e => t => {
                                     var r;
                                     Q(t), !1 === G.current && en(-1), $(-1), null == e || null == (r = e.onBlur) || r.call(e, t)
                                 };
                             (0, h.Z)(() => {
-                                if (n && eo.current.contains(document.activeElement)) {
+                                if (n && ea.current.contains(document.activeElement)) {
                                     var e;
                                     null == (e = document.activeElement) || e.blur()
                                 }
                             }, [n]), n && -1 !== D && N(-1), n && -1 !== er && en(-1);
                             let es = e => t => {
                                     var r;
                                     null == (r = e.onChange) || r.call(e, t);
                                     let n = Number(t.currentTarget.getAttribute("data-index")),
-                                        a = K[n],
-                                        i = J.indexOf(a),
-                                        l = t.target.valueAsNumber;
+                                        o = K[n],
+                                        l = J.indexOf(o),
+                                        i = t.target.valueAsNumber;
                                     if (q && null == M) {
                                         let e = J[J.length - 1];
-                                        l = l > e ? e : l < J[0] ? J[0] : l < a ? J[i - 1] : J[i + 1]
+                                        i = i > e ? e : i < J[0] ? J[0] : i < o ? J[l - 1] : J[l + 1]
                                     }
-                                    if (l = g(l, c, s), Y) {
-                                        o && (l = g(l, K[n - 1] || -1 / 0, K[n + 1] || 1 / 0));
-                                        let e = l;
-                                        l = k({
+                                    if (i = g(i, c, s), Y) {
+                                        a && (i = g(i, K[n - 1] || -1 / 0, K[n + 1] || 1 / 0));
+                                        let e = i;
+                                        i = k({
                                             values: K,
-                                            newValue: l,
+                                            newValue: i,
                                             index: n
                                         });
                                         let t = n;
-                                        o || (t = l.indexOf(e)), O({
-                                            sliderRef: eo,
+                                        a || (t = i.indexOf(e)), S({
+                                            sliderRef: ea,
                                             activeIndex: t
                                         })
                                     }
-                                    W(l), en(n), X && !S(l, B) && X(t, l, n), E && E(t, l)
+                                    W(i), en(n), X && !O(i, B) && X(t, i, n), E && E(t, i)
                                 },
-                                ec = i.useRef(),
-                                ef = L;
-                            l && "horizontal" === L && (ef += "-reverse");
-                            let ed = ({
+                                ec = l.useRef(),
+                                ed = L;
+                            i && "horizontal" === L && (ed += "-reverse");
+                            let ef = ({
                                     finger: e,
                                     move: t = !1
                                 }) => {
                                     let r, n;
                                     let {
-                                        current: a
-                                    } = eo, {
-                                        width: i,
-                                        height: l,
+                                        current: o
+                                    } = ea, {
+                                        width: l,
+                                        height: i,
                                         bottom: u,
-                                        left: f
-                                    } = a.getBoundingClientRect();
-                                    if (r = 0 === ef.indexOf("vertical") ? (u - e.y) / l : (e.x - f) / i, -1 !== ef.indexOf("-reverse") && (r = 1 - r), n = (s - c) * r + c, M) n = function(e, t, r) {
+                                        left: d
+                                    } = o.getBoundingClientRect();
+                                    if (r = 0 === ed.indexOf("vertical") ? (u - e.y) / i : (e.x - d) / l, -1 !== ed.indexOf("-reverse") && (r = 1 - r), n = (s - c) * r + c, M) n = function(e, t, r) {
                                         let n = Math.round((e - r) / t) * t + r;
                                         return Number(n.toFixed(function(e) {
                                             if (1 > Math.abs(e)) {
                                                 let t = e.toExponential().split("e-"),
                                                     r = t[0].split(".")[1];
                                                 return (r ? r.length : 0) + parseInt(t[1], 10)
                                             }
@@ -700,122 +699,122 @@
                                         }(t)))
                                     }(n, M, c);
                                     else {
                                         let e = P(J, n);
                                         n = J[e]
                                     }
                                     n = g(n, c, s);
-                                    let d = 0;
+                                    let f = 0;
                                     if (Y) {
-                                        d = t ? ec.current : P(K, n), o && (n = g(n, K[d - 1] || -1 / 0, K[d + 1] || 1 / 0));
+                                        f = t ? ec.current : P(K, n), a && (n = g(n, K[f - 1] || -1 / 0, K[f + 1] || 1 / 0));
                                         let e = n;
                                         n = k({
                                             values: K,
                                             newValue: n,
-                                            index: d
-                                        }), o && t || (d = n.indexOf(e), ec.current = d)
+                                            index: f
+                                        }), a && t || (f = n.indexOf(e), ec.current = f)
                                     }
                                     return {
                                         newValue: n,
-                                        activeIndex: d
+                                        activeIndex: f
                                     }
                                 },
-                                ep = (0, v.Z)(e => {
+                                ep = (0, m.Z)(e => {
                                     let t = w(e, z);
                                     if (!t) return;
                                     if (F.current += 1, "mousemove" === e.type && 0 === e.buttons) {
                                         ey(e);
                                         return
                                     }
                                     let {
                                         newValue: r,
                                         activeIndex: n
-                                    } = ed({
+                                    } = ef({
                                         finger: t,
                                         move: !0
                                     });
-                                    O({
-                                        sliderRef: eo,
+                                    S({
+                                        sliderRef: ea,
                                         activeIndex: n,
                                         setActive: N
-                                    }), W(r), !H && F.current > 2 && V(!0), X && !S(r, B) && X(e, r, n)
+                                    }), W(r), !H && F.current > 2 && V(!0), X && !O(r, B) && X(e, r, n)
                                 }),
-                                ey = (0, v.Z)(e => {
+                                ey = (0, m.Z)(e => {
                                     let t = w(e, z);
                                     if (V(!1), !t) return;
                                     let {
                                         newValue: r
-                                    } = ed({
+                                    } = ef({
                                         finger: t,
                                         move: !0
                                     });
-                                    N(-1), "touchend" === e.type && $(-1), E && E(e, r), z.current = void 0, ev()
+                                    N(-1), "touchend" === e.type && $(-1), E && E(e, r), z.current = void 0, em()
                                 }),
-                                eh = (0, v.Z)(e => {
+                                eh = (0, m.Z)(e => {
                                     if (n) return;
                                     A() || e.preventDefault();
                                     let t = e.changedTouches[0];
                                     null != t && (z.current = t.identifier);
                                     let r = w(e, z);
                                     if (!1 !== r) {
                                         let {
                                             newValue: t,
                                             activeIndex: n
-                                        } = ed({
+                                        } = ef({
                                             finger: r
                                         });
-                                        O({
-                                            sliderRef: eo,
+                                        S({
+                                            sliderRef: ea,
                                             activeIndex: n,
                                             setActive: N
-                                        }), W(t), X && !S(t, B) && X(e, t, n)
+                                        }), W(t), X && !O(t, B) && X(e, t, n)
                                     }
                                     F.current = 0;
-                                    let o = (0, f.Z)(eo.current);
-                                    o.addEventListener("touchmove", ep), o.addEventListener("touchend", ey)
+                                    let a = (0, d.Z)(ea.current);
+                                    a.addEventListener("touchmove", ep), a.addEventListener("touchend", ey)
                                 }),
-                                ev = i.useCallback(() => {
-                                    let e = (0, f.Z)(eo.current);
+                                em = l.useCallback(() => {
+                                    let e = (0, d.Z)(ea.current);
                                     e.removeEventListener("mousemove", ep), e.removeEventListener("mouseup", ey), e.removeEventListener("touchmove", ep), e.removeEventListener("touchend", ey)
                                 }, [ey, ep]);
-                            i.useEffect(() => {
+                            l.useEffect(() => {
                                 let {
                                     current: e
-                                } = eo;
+                                } = ea;
                                 return e.addEventListener("touchstart", eh, {
                                     passive: A()
                                 }), () => {
                                     e.removeEventListener("touchstart", eh, {
                                         passive: A()
-                                    }), ev()
+                                    }), em()
                                 }
-                            }, [ev, eh]), i.useEffect(() => {
-                                n && ev()
-                            }, [n, ev]);
-                            let em = e => t => {
+                            }, [em, eh]), l.useEffect(() => {
+                                n && em()
+                            }, [n, em]);
+                            let ev = e => t => {
                                     var r;
                                     if (null == (r = e.onMouseDown) || r.call(e, t), n || t.defaultPrevented || 0 !== t.button) return;
                                     t.preventDefault();
-                                    let o = w(t, z);
-                                    if (!1 !== o) {
+                                    let a = w(t, z);
+                                    if (!1 !== a) {
                                         let {
                                             newValue: e,
                                             activeIndex: r
-                                        } = ed({
-                                            finger: o
+                                        } = ef({
+                                            finger: a
                                         });
-                                        O({
-                                            sliderRef: eo,
+                                        S({
+                                            sliderRef: ea,
                                             activeIndex: r,
                                             setActive: N
-                                        }), W(e), X && !S(e, B) && X(t, e, r)
+                                        }), W(e), X && !O(e, B) && X(t, e, r)
                                     }
                                     F.current = 0;
-                                    let a = (0, f.Z)(eo.current);
-                                    a.addEventListener("mousemove", ep), a.addEventListener("mouseup", ey)
+                                    let o = (0, d.Z)(ea.current);
+                                    o.addEventListener("mousemove", ep), o.addEventListener("mouseup", ey)
                                 },
                                 eb = ((Y ? K[0] : c) - c) * 100 / (s - c),
                                 eg = (K[K.length - 1] - c) * 100 / (s - c) - eb,
                                 eP = e => t => {
                                     var r;
                                     null == (r = e.onMouseOver) || r.call(e, t);
                                     let n = Number(t.currentTarget.getAttribute("data-index"));
@@ -823,200 +822,199 @@
                                 },
                                 ew = e => t => {
                                     var r;
                                     null == (r = e.onMouseLeave) || r.call(e, t), $(-1)
                                 };
                             return {
                                 active: D,
-                                axis: ef,
-                                axisProps: _,
+                                axis: ed,
+                                axisProps: x,
                                 dragging: H,
                                 focusedThumbIndex: er,
                                 getHiddenInputProps: (r = {}) => {
-                                    var o;
-                                    let i = {
+                                    var a;
+                                    let l = {
                                             onChange: es(r || {}),
-                                            onFocus: el(r || {}),
+                                            onFocus: ei(r || {}),
                                             onBlur: eu(r || {})
                                         },
-                                        u = (0, a.Z)({}, r, i);
-                                    return (0, a.Z)({
+                                        u = (0, o.Z)({}, r, l);
+                                    return (0, o.Z)({
                                         tabIndex: I,
                                         "aria-labelledby": t,
                                         "aria-orientation": L,
-                                        "aria-valuemax": R(s),
-                                        "aria-valuemin": R(c),
+                                        "aria-valuemax": j(s),
+                                        "aria-valuemin": j(c),
                                         name: T,
                                         type: "range",
                                         min: e.min,
                                         max: e.max,
-                                        step: null === e.step && e.marks ? "any" : null != (o = e.step) ? o : void 0,
+                                        step: null === e.step && e.marks ? "any" : null != (a = e.step) ? a : void 0,
                                         disabled: n
                                     }, u, {
-                                        style: (0, a.Z)({}, m, {
-                                            direction: l ? "rtl" : "ltr",
+                                        style: (0, o.Z)({}, v, {
+                                            direction: i ? "rtl" : "ltr",
                                             width: "100%",
                                             height: "100%"
                                         })
                                     })
                                 },
                                 getRootProps: (e = {}) => {
                                     let t = {
-                                            onMouseDown: em(e || {})
+                                            onMouseDown: ev(e || {})
                                         },
-                                        r = (0, a.Z)({}, e, t);
-                                    return (0, a.Z)({
-                                        ref: ei
+                                        r = (0, o.Z)({}, e, t);
+                                    return (0, o.Z)({
+                                        ref: el
                                     }, r)
                                 },
                                 getThumbProps: (e = {}) => {
                                     let t = {
                                         onMouseOver: eP(e || {}),
                                         onMouseLeave: ew(e || {})
                                     };
-                                    return (0, a.Z)({}, e, t)
+                                    return (0, o.Z)({}, e, t)
                                 },
                                 marks: q,
                                 open: U,
                                 range: Y,
-                                rootRef: ei,
+                                rootRef: el,
                                 trackLeap: eg,
                                 trackOffset: eb,
-                                values: K,
-                                getThumbStyle: e => ({
-                                    pointerEvents: -1 !== D && D !== e ? "none" : void 0
-                                })
+                                values: K
                             }
-                        }((0, a.Z)({}, eN, {
+                        }((0, o.Z)({}, eN, {
                             rootRef: t
                         }));
                     eN.marked = eq.length > 0 && eq.some(e => e.label), eN.dragging = eK, eN.focusedThumbIndex = eX;
-                    let e1 = K(eN),
-                        e9 = null != (r = null != (n = null == eM ? void 0 : eM.root) ? n : em.Root) ? r : H,
-                        e5 = null != (u = null != (T = null == eM ? void 0 : eM.rail) ? T : em.Rail) ? u : V,
-                        e4 = null != (E = null != (R = null == eM ? void 0 : eM.track) ? R : em.Track) ? E : F,
-                        e6 = null != (M = null != (I = null == eM ? void 0 : eM.thumb) ? I : em.Thumb) ? M : B,
-                        e2 = null != (Z = null != (z = null == eM ? void 0 : eM.valueLabel) ? z : em.ValueLabel) ? Z : W,
-                        e8 = null != (N = null != (J = null == eM ? void 0 : eM.mark) ? J : em.Mark) ? N : X,
-                        e3 = null != (G = null != (Q = null == eM ? void 0 : eM.markLabel) ? Q : em.MarkLabel) ? G : Y,
-                        e7 = null != (ee = null != (et = null == eM ? void 0 : eM.input) ? et : em.Input) ? ee : "input",
-                        te = null != (er = null == eR ? void 0 : eR.root) ? er : eb.root,
-                        tt = null != (en = null == eR ? void 0 : eR.rail) ? en : eb.rail,
-                        tr = null != (eo = null == eR ? void 0 : eR.track) ? eo : eb.track,
-                        tn = null != (ea = null == eR ? void 0 : eR.thumb) ? ea : eb.thumb,
-                        to = null != (ei = null == eR ? void 0 : eR.valueLabel) ? ei : eb.valueLabel,
-                        ta = null != (el = null == eR ? void 0 : eR.mark) ? el : eb.mark,
-                        ti = null != (eu = null == eR ? void 0 : eR.markLabel) ? eu : eb.markLabel,
-                        tl = null != (es = null == eR ? void 0 : eR.input) ? es : eb.input,
-                        tu = (0, s.Z)({
-                            elementType: e9,
+                    let e0 = K(eN),
+                        e1 = null != (r = null != (n = null == eM ? void 0 : eM.root) ? n : ev.Root) ? r : H,
+                        e5 = null != (u = null != (T = null == eM ? void 0 : eM.rail) ? T : ev.Rail) ? u : V,
+                        e9 = null != (E = null != (j = null == eM ? void 0 : eM.track) ? j : ev.Track) ? E : F,
+                        e2 = null != (M = null != (I = null == eM ? void 0 : eM.thumb) ? I : ev.Thumb) ? M : B,
+                        e6 = null != (Z = null != (z = null == eM ? void 0 : eM.valueLabel) ? z : ev.ValueLabel) ? Z : W,
+                        e4 = null != (N = null != (J = null == eM ? void 0 : eM.mark) ? J : ev.Mark) ? N : X,
+                        e3 = null != (G = null != (Q = null == eM ? void 0 : eM.markLabel) ? Q : ev.MarkLabel) ? G : Y,
+                        e8 = null != (ee = null != (et = null == eM ? void 0 : eM.input) ? et : ev.Input) ? ee : "input",
+                        e7 = null != (er = null == ej ? void 0 : ej.root) ? er : eb.root,
+                        te = null != (en = null == ej ? void 0 : ej.rail) ? en : eb.rail,
+                        tt = null != (ea = null == ej ? void 0 : ej.track) ? ea : eb.track,
+                        tr = null != (eo = null == ej ? void 0 : ej.thumb) ? eo : eb.thumb,
+                        tn = null != (el = null == ej ? void 0 : ej.valueLabel) ? el : eb.valueLabel,
+                        ta = null != (ei = null == ej ? void 0 : ej.mark) ? ei : eb.mark,
+                        to = null != (eu = null == ej ? void 0 : ej.markLabel) ? eu : eb.markLabel,
+                        tl = null != (es = null == ej ? void 0 : ej.input) ? es : eb.input,
+                        ti = (0, s.Z)({
+                            elementType: e1,
                             getSlotProps: e$,
-                            externalSlotProps: te,
+                            externalSlotProps: e7,
                             externalForwardedProps: eD,
-                            additionalProps: (0, a.Z)({}, C(e9) && {
-                                as: ev
+                            additionalProps: (0, o.Z)({}, R(e1) && {
+                                as: em
                             }),
-                            ownerState: (0, a.Z)({}, eN, null == te ? void 0 : te.ownerState),
-                            className: [e1.root, ew]
+                            ownerState: (0, o.Z)({}, eN, null == e7 ? void 0 : e7.ownerState),
+                            className: [e0.root, ew]
                         }),
-                        ts = (0, s.Z)({
+                        tu = (0, s.Z)({
                             elementType: e5,
-                            externalSlotProps: tt,
+                            externalSlotProps: te,
                             ownerState: eN,
-                            className: e1.rail
+                            className: e0.rail
                         }),
-                        tc = (0, s.Z)({
-                            elementType: e4,
-                            externalSlotProps: tr,
+                        ts = (0, s.Z)({
+                            elementType: e9,
+                            externalSlotProps: tt,
                             additionalProps: {
-                                style: (0, a.Z)({}, eU[eW].offset(eG), eU[eW].leap(eQ))
+                                style: (0, o.Z)({}, eU[eW].offset(eG), eU[eW].leap(eQ))
                             },
-                            ownerState: (0, a.Z)({}, eN, null == tr ? void 0 : tr.ownerState),
-                            className: e1.track
+                            ownerState: (0, o.Z)({}, eN, null == tt ? void 0 : tt.ownerState),
+                            className: e0.track
                         }),
-                        tf = (0, s.Z)({
-                            elementType: e6,
+                        tc = (0, s.Z)({
+                            elementType: e2,
                             getSlotProps: eV,
-                            externalSlotProps: tn,
-                            ownerState: (0, a.Z)({}, eN, null == tn ? void 0 : tn.ownerState),
-                            className: e1.thumb
+                            externalSlotProps: tr,
+                            ownerState: (0, o.Z)({}, eN, null == tr ? void 0 : tr.ownerState),
+                            className: e0.thumb
                         }),
                         td = (0, s.Z)({
-                            elementType: e2,
-                            externalSlotProps: to,
-                            ownerState: (0, a.Z)({}, eN, null == to ? void 0 : to.ownerState),
-                            className: e1.valueLabel
+                            elementType: e6,
+                            externalSlotProps: tn,
+                            ownerState: (0, o.Z)({}, eN, null == tn ? void 0 : tn.ownerState),
+                            className: e0.valueLabel
                         }),
-                        tp = (0, s.Z)({
-                            elementType: e8,
+                        tf = (0, s.Z)({
+                            elementType: e4,
                             externalSlotProps: ta,
                             ownerState: eN,
-                            className: e1.mark
+                            className: e0.mark
                         }),
-                        ty = (0, s.Z)({
+                        tp = (0, s.Z)({
                             elementType: e3,
-                            externalSlotProps: ti,
+                            externalSlotProps: to,
                             ownerState: eN,
-                            className: e1.markLabel
+                            className: e0.markLabel
                         }),
-                        th = (0, s.Z)({
-                            elementType: e7,
+                        ty = (0, s.Z)({
+                            elementType: e8,
                             getSlotProps: eH,
                             externalSlotProps: tl,
                             ownerState: eN
                         });
-                    return (0, D.jsxs)(e9, (0, a.Z)({}, tu, {
-                        children: [(0, D.jsx)(e5, (0, a.Z)({}, ts)), (0, D.jsx)(e4, (0, a.Z)({}, tc)), eq.filter(e => e.value >= eT && e.value <= eA).map((e, t) => {
+                    return (0, D.jsxs)(e1, (0, o.Z)({}, ti, {
+                        children: [(0, D.jsx)(e5, (0, o.Z)({}, tu)), (0, D.jsx)(e9, (0, o.Z)({}, ts)), eq.filter(e => e.value >= eT && e.value <= eA).map((e, t) => {
                             let r;
                             let n = (e.value - eT) * 100 / (eA - eT),
-                                o = eU[eW].offset(n);
-                            return r = !1 === eI ? -1 !== eJ.indexOf(e.value) : "normal" === eI && (eY ? e.value >= eJ[0] && e.value <= eJ[eJ.length - 1] : e.value <= eJ[0]) || "inverted" === eI && (eY ? e.value <= eJ[0] || e.value >= eJ[eJ.length - 1] : e.value >= eJ[0]), (0, D.jsxs)(i.Fragment, {
-                                children: [(0, D.jsx)(e8, (0, a.Z)({
+                                a = eU[eW].offset(n);
+                            return r = !1 === eI ? -1 !== eJ.indexOf(e.value) : "normal" === eI && (eY ? e.value >= eJ[0] && e.value <= eJ[eJ.length - 1] : e.value <= eJ[0]) || "inverted" === eI && (eY ? e.value <= eJ[0] || e.value >= eJ[eJ.length - 1] : e.value >= eJ[0]), (0, D.jsxs)(l.Fragment, {
+                                children: [(0, D.jsx)(e4, (0, o.Z)({
                                     "data-index": t
-                                }, tp, !(0, c.Z)(e8) && {
+                                }, tf, !(0, c.Z)(e4) && {
                                     markActive: r
                                 }, {
-                                    style: (0, a.Z)({}, o, tp.style),
-                                    className: (0, l.Z)(tp.className, r && e1.markActive)
-                                })), null != e.label ? (0, D.jsx)(e3, (0, a.Z)({
+                                    style: (0, o.Z)({}, a, tf.style),
+                                    className: (0, i.Z)(tf.className, r && e0.markActive)
+                                })), null != e.label ? (0, D.jsx)(e3, (0, o.Z)({
                                     "aria-hidden": !0,
                                     "data-index": t
-                                }, ty, !(0, c.Z)(e3) && {
+                                }, tp, !(0, c.Z)(e3) && {
                                     markLabelActive: r
                                 }, {
-                                    style: (0, a.Z)({}, o, ty.style),
-                                    className: (0, l.Z)(e1.markLabel, ty.className, r && e1.markLabelActive),
+                                    style: (0, o.Z)({}, a, tp.style),
+                                    className: (0, i.Z)(e0.markLabel, tp.className, r && e0.markLabelActive),
                                     children: e.label
                                 })) : null]
                             }, t)
                         }), eJ.map((e, t) => {
                             let r = (e - eT) * 100 / (eA - eT),
                                 n = eU[eW].offset(r),
-                                o = "off" === eZ ? q : e2;
-                            return (0, D.jsx)(o, (0, a.Z)({}, !(0, c.Z)(o) && {
+                                a = "off" === eZ ? q : e6;
+                            return (0, D.jsx)(a, (0, o.Z)({}, !(0, c.Z)(a) && {
                                 valueLabelFormat: ez,
                                 valueLabelDisplay: eZ,
-                                value: "function" == typeof ez ? ez(eC(e), t) : ez,
+                                value: "function" == typeof ez ? ez(eR(e), t) : ez,
                                 index: t,
                                 open: eF === t || eB === t || "on" === eZ,
-                                disabled: eO
+                                disabled: eS
                             }, td, {
-                                children: (0, D.jsx)(e6, (0, a.Z)({
+                                children: (0, D.jsx)(e2, (0, o.Z)({
                                     "data-index": t
-                                }, tf, {
-                                    className: (0, l.Z)(e1.thumb, tf.className, eB === t && e1.active, eX === t && e1.focusVisible),
-                                    style: (0, a.Z)({}, n, e0(t), tf.style),
-                                    children: (0, D.jsx)(e7, (0, a.Z)({
+                                }, tc, {
+                                    className: (0, i.Z)(e0.thumb, tc.className, eB === t && e0.active, eX === t && e0.focusVisible),
+                                    style: (0, o.Z)({}, n, {
+                                        pointerEvents: ek && eB !== t ? "none" : void 0
+                                    }, tc.style),
+                                    children: (0, D.jsx)(e8, (0, o.Z)({
                                         "data-index": t,
-                                        "aria-label": eS ? eS(t) : ep,
-                                        "aria-valuenow": eC(e),
+                                        "aria-label": eO ? eO(t) : ep,
+                                        "aria-valuenow": eR(e),
                                         "aria-labelledby": eh,
-                                        "aria-valuetext": e_ ? e_(eC(e), t) : ey,
+                                        "aria-valuetext": ex ? ex(eR(e), t) : ey,
                                         value: eJ[t]
-                                    }, th))
+                                    }, ty))
                                 }))
                             }), t)
                         })]
                     }))
                 });
             var G = J
         },
@@ -1025,56 +1023,56 @@
             var t = function(e) {
                     var t;
                     return !!e && "object" == typeof e && "[object RegExp]" !== (t = Object.prototype.toString.call(e)) && "[object Date]" !== t && e.$$typeof !== r
                 },
                 r = "function" == typeof Symbol && Symbol.for ? Symbol.for("react.element") : 60103;
 
             function n(e, t) {
-                return !1 !== t.clone && t.isMergeableObject(e) ? l(Array.isArray(e) ? [] : {}, e, t) : e
+                return !1 !== t.clone && t.isMergeableObject(e) ? i(Array.isArray(e) ? [] : {}, e, t) : e
             }
 
-            function o(e, t, r) {
+            function a(e, t, r) {
                 return e.concat(t).map(function(e) {
                     return n(e, r)
                 })
             }
 
-            function a(e) {
+            function o(e) {
                 return Object.keys(e).concat(Object.getOwnPropertySymbols ? Object.getOwnPropertySymbols(e).filter(function(t) {
                     return e.propertyIsEnumerable(t)
                 }) : [])
             }
 
-            function i(e, t) {
+            function l(e, t) {
                 try {
                     return t in e
                 } catch (e) {
                     return !1
                 }
             }
 
-            function l(e, r, u) {
-                (u = u || {}).arrayMerge = u.arrayMerge || o, u.isMergeableObject = u.isMergeableObject || t, u.cloneUnlessOtherwiseSpecified = n;
-                var s, c, f = Array.isArray(r);
-                return f !== Array.isArray(e) ? n(r, u) : f ? u.arrayMerge(e, r, u) : (c = {}, (s = u).isMergeableObject(e) && a(e).forEach(function(t) {
+            function i(e, r, u) {
+                (u = u || {}).arrayMerge = u.arrayMerge || a, u.isMergeableObject = u.isMergeableObject || t, u.cloneUnlessOtherwiseSpecified = n;
+                var s, c, d = Array.isArray(r);
+                return d !== Array.isArray(e) ? n(r, u) : d ? u.arrayMerge(e, r, u) : (c = {}, (s = u).isMergeableObject(e) && o(e).forEach(function(t) {
                     c[t] = n(e[t], s)
-                }), a(r).forEach(function(t) {
-                    (!i(e, t) || Object.hasOwnProperty.call(e, t) && Object.propertyIsEnumerable.call(e, t)) && (i(e, t) && s.isMergeableObject(r[t]) ? c[t] = (function(e, t) {
-                        if (!t.customMerge) return l;
+                }), o(r).forEach(function(t) {
+                    (!l(e, t) || Object.hasOwnProperty.call(e, t) && Object.propertyIsEnumerable.call(e, t)) && (l(e, t) && s.isMergeableObject(r[t]) ? c[t] = (function(e, t) {
+                        if (!t.customMerge) return i;
                         var r = t.customMerge(e);
-                        return "function" == typeof r ? r : l
+                        return "function" == typeof r ? r : i
                     })(t, s)(e[t], r[t], s) : c[t] = n(r[t], s))
                 }), c)
             }
-            l.all = function(e, t) {
+            i.all = function(e, t) {
                 if (!Array.isArray(e)) throw Error("first argument should be an array");
                 return e.reduce(function(e, r) {
-                    return l(e, r, t)
+                    return i(e, r, t)
                 }, {})
-            }, e.exports = l
+            }, e.exports = i
         },
         9090: function(e) {
             function t(e, t) {
                 e.onload = function() {
                     this.onerror = this.onload = null, t(null, e)
                 }, e.onerror = function() {
                     this.onerror = this.onload = null, t(Error("Failed to load " + this.src), e)
@@ -1082,316 +1080,96 @@
             }
 
             function r(e, t) {
                 e.onreadystatechange = function() {
                     ("complete" == this.readyState || "loaded" == this.readyState) && (this.onreadystatechange = null, t(null, e))
                 }
             }
-            e.exports = function(e, n, o) {
-                var a = document.head || document.getElementsByTagName("head")[0],
-                    i = document.createElement("script");
-                "function" == typeof n && (o = n, n = {}), n = n || {}, o = o || function() {}, i.type = n.type || "text/javascript", i.charset = n.charset || "utf8", i.async = !("async" in n) || !!n.async, i.src = e, n.attrs && function(e, t) {
+            e.exports = function(e, n, a) {
+                var o = document.head || document.getElementsByTagName("head")[0],
+                    l = document.createElement("script");
+                "function" == typeof n && (a = n, n = {}), n = n || {}, a = a || function() {}, l.type = n.type || "text/javascript", l.charset = n.charset || "utf8", l.async = !("async" in n) || !!n.async, l.src = e, n.attrs && function(e, t) {
                     for (var r in t) e.setAttribute(r, t[r])
-                }(i, n.attrs), n.text && (i.text = "" + n.text), ("onload" in i ? t : r)(i, o), i.onload || t(i, o), a.appendChild(i)
-            }
-        },
-        8668: function(e, t, r) {
-            var n = r(3369),
-                o = r(619),
-                a = r(2385);
-
-            function i(e) {
-                var t = -1,
-                    r = null == e ? 0 : e.length;
-                for (this.__data__ = new n; ++t < r;) this.add(e[t])
-            }
-            i.prototype.add = i.prototype.push = o, i.prototype.has = a, e.exports = i
-        },
-        2908: function(e) {
-            e.exports = function(e, t) {
-                for (var r = -1, n = null == e ? 0 : e.length; ++r < n;)
-                    if (t(e[r], r, e)) return !0;
-                return !1
-            }
-        },
-        939: function(e, t, r) {
-            var n = r(2492),
-                o = r(7005);
-            e.exports = function e(t, r, a, i, l) {
-                return t === r || (null != t && null != r && (o(t) || o(r)) ? n(t, r, a, i, e, l) : t != t && r != r)
-            }
-        },
-        2492: function(e, t, r) {
-            var n = r(6384),
-                o = r(7114),
-                a = r(8351),
-                i = r(6096),
-                l = r(4160),
-                u = r(1469),
-                s = r(4144),
-                c = r(6719),
-                f = "[object Arguments]",
-                d = "[object Array]",
-                p = "[object Object]",
-                y = Object.prototype.hasOwnProperty;
-            e.exports = function(e, t, r, h, v, m) {
-                var b = u(e),
-                    g = u(t),
-                    P = b ? d : l(e),
-                    w = g ? d : l(t);
-                P = P == f ? p : P, w = w == f ? p : w;
-                var k = P == p,
-                    O = w == p,
-                    S = P == w;
-                if (S && s(e)) {
-                    if (!s(t)) return !1;
-                    b = !0, k = !1
-                }
-                if (S && !k) return m || (m = new n), b || c(e) ? o(e, t, r, h, v, m) : a(e, t, P, r, h, v, m);
-                if (!(1 & r)) {
-                    var _ = k && y.call(e, "__wrapped__"),
-                        x = O && y.call(t, "__wrapped__");
-                    if (_ || x) {
-                        var A = _ ? e.value() : e,
-                            T = x ? t.value() : t;
-                        return m || (m = new n), v(A, T, r, h, m)
-                    }
-                }
-                return !!S && (m || (m = new n), i(e, t, r, h, v, m))
-            }
-        },
-        4757: function(e) {
-            e.exports = function(e, t) {
-                return e.has(t)
-            }
-        },
-        7114: function(e, t, r) {
-            var n = r(8668),
-                o = r(2908),
-                a = r(4757);
-            e.exports = function(e, t, r, i, l, u) {
-                var s = 1 & r,
-                    c = e.length,
-                    f = t.length;
-                if (c != f && !(s && f > c)) return !1;
-                var d = u.get(e),
-                    p = u.get(t);
-                if (d && p) return d == t && p == e;
-                var y = -1,
-                    h = !0,
-                    v = 2 & r ? new n : void 0;
-                for (u.set(e, t), u.set(t, e); ++y < c;) {
-                    var m = e[y],
-                        b = t[y];
-                    if (i) var g = s ? i(b, m, y, t, e, u) : i(m, b, y, e, t, u);
-                    if (void 0 !== g) {
-                        if (g) continue;
-                        h = !1;
-                        break
-                    }
-                    if (v) {
-                        if (!o(t, function(e, t) {
-                                if (!a(v, t) && (m === e || l(m, e, r, i, u))) return v.push(t)
-                            })) {
-                            h = !1;
-                            break
-                        }
-                    } else if (!(m === b || l(m, b, r, i, u))) {
-                        h = !1;
-                        break
-                    }
-                }
-                return u.delete(e), u.delete(t), h
-            }
-        },
-        8351: function(e, t, r) {
-            var n = r(2705),
-                o = r(1149),
-                a = r(7813),
-                i = r(7114),
-                l = r(8776),
-                u = r(1814),
-                s = n ? n.prototype : void 0,
-                c = s ? s.valueOf : void 0;
-            e.exports = function(e, t, r, n, s, f, d) {
-                switch (r) {
-                    case "[object DataView]":
-                        if (e.byteLength != t.byteLength || e.byteOffset != t.byteOffset) break;
-                        e = e.buffer, t = t.buffer;
-                    case "[object ArrayBuffer]":
-                        if (e.byteLength != t.byteLength || !f(new o(e), new o(t))) break;
-                        return !0;
-                    case "[object Boolean]":
-                    case "[object Date]":
-                    case "[object Number]":
-                        return a(+e, +t);
-                    case "[object Error]":
-                        return e.name == t.name && e.message == t.message;
-                    case "[object RegExp]":
-                    case "[object String]":
-                        return e == t + "";
-                    case "[object Map]":
-                        var p = l;
-                    case "[object Set]":
-                        var y = 1 & n;
-                        if (p || (p = u), e.size != t.size && !y) break;
-                        var h = d.get(e);
-                        if (h) return h == t;
-                        n |= 2, d.set(e, t);
-                        var v = i(p(e), p(t), n, s, f, d);
-                        return d.delete(e), v;
-                    case "[object Symbol]":
-                        if (c) return c.call(e) == c.call(t)
-                }
-                return !1
-            }
-        },
-        6096: function(e, t, r) {
-            var n = r(8234),
-                o = Object.prototype.hasOwnProperty;
-            e.exports = function(e, t, r, a, i, l) {
-                var u = 1 & r,
-                    s = n(e),
-                    c = s.length;
-                if (c != n(t).length && !u) return !1;
-                for (var f = c; f--;) {
-                    var d = s[f];
-                    if (!(u ? d in t : o.call(t, d))) return !1
-                }
-                var p = l.get(e),
-                    y = l.get(t);
-                if (p && y) return p == t && y == e;
-                var h = !0;
-                l.set(e, t), l.set(t, e);
-                for (var v = u; ++f < c;) {
-                    var m = e[d = s[f]],
-                        b = t[d];
-                    if (a) var g = u ? a(b, m, d, t, e, l) : a(m, b, d, e, t, l);
-                    if (!(void 0 === g ? m === b || i(m, b, r, a, l) : g)) {
-                        h = !1;
-                        break
-                    }
-                    v || (v = "constructor" == d)
-                }
-                if (h && !v) {
-                    var P = e.constructor,
-                        w = t.constructor;
-                    P != w && "constructor" in e && "constructor" in t && !("function" == typeof P && P instanceof P && "function" == typeof w && w instanceof w) && (h = !1)
-                }
-                return l.delete(e), l.delete(t), h
-            }
-        },
-        8776: function(e) {
-            e.exports = function(e) {
-                var t = -1,
-                    r = Array(e.size);
-                return e.forEach(function(e, n) {
-                    r[++t] = [n, e]
-                }), r
-            }
-        },
-        619: function(e) {
-            e.exports = function(e) {
-                return this.__data__.set(e, "__lodash_hash_undefined__"), this
-            }
-        },
-        2385: function(e) {
-            e.exports = function(e) {
-                return this.__data__.has(e)
-            }
-        },
-        1814: function(e) {
-            e.exports = function(e) {
-                var t = -1,
-                    r = Array(e.size);
-                return e.forEach(function(e) {
-                    r[++t] = e
-                }), r
-            }
-        },
-        8446: function(e, t, r) {
-            var n = r(939);
-            e.exports = function(e, t) {
-                return n(e, t)
+                }(l, n.attrs), n.text && (l.text = "" + n.text), ("onload" in l ? t : r)(l, a), l.onload || t(l, a), o.appendChild(l)
             }
         },
         845: function(e, t, r) {
             "use strict";
             r.r(t);
             var n = Number.isNaN || function(e) {
                 return "number" == typeof e && e != e
             };
 
-            function o(e, t) {
+            function a(e, t) {
                 if (e.length !== t.length) return !1;
-                for (var r, o, a = 0; a < e.length; a++)
-                    if (!((r = e[a]) === (o = t[a]) || n(r) && n(o))) return !1;
+                for (var r, a, o = 0; o < e.length; o++)
+                    if (!((r = e[o]) === (a = t[o]) || n(r) && n(a))) return !1;
                 return !0
             }
             t.default = function(e, t) {
-                void 0 === t && (t = o);
-                var r, n, a = [],
-                    i = !1;
+                void 0 === t && (t = a);
+                var r, n, o = [],
+                    l = !1;
                 return function() {
-                    for (var o = [], l = 0; l < arguments.length; l++) o[l] = arguments[l];
-                    return i && r === this && t(o, a) || (n = e.apply(this, o), i = !0, r = this, a = o), n
+                    for (var a = [], i = 0; i < arguments.length; i++) a[i] = arguments[i];
+                    return l && r === this && t(a, o) || (n = e.apply(this, a), l = !0, r = this, o = a), n
                 }
             }
         },
         9590: function(e) {
             var t = "undefined" != typeof Element,
                 r = "function" == typeof Map,
                 n = "function" == typeof Set,
-                o = "function" == typeof ArrayBuffer && !!ArrayBuffer.isView;
-            e.exports = function(e, a) {
+                a = "function" == typeof ArrayBuffer && !!ArrayBuffer.isView;
+            e.exports = function(e, o) {
                 try {
-                    return function e(a, i) {
-                        if (a === i) return !0;
-                        if (a && i && "object" == typeof a && "object" == typeof i) {
-                            var l, u, s, c;
-                            if (a.constructor !== i.constructor) return !1;
-                            if (Array.isArray(a)) {
-                                if ((l = a.length) != i.length) return !1;
-                                for (u = l; 0 != u--;)
-                                    if (!e(a[u], i[u])) return !1;
+                    return function e(o, l) {
+                        if (o === l) return !0;
+                        if (o && l && "object" == typeof o && "object" == typeof l) {
+                            var i, u, s, c;
+                            if (o.constructor !== l.constructor) return !1;
+                            if (Array.isArray(o)) {
+                                if ((i = o.length) != l.length) return !1;
+                                for (u = i; 0 != u--;)
+                                    if (!e(o[u], l[u])) return !1;
                                 return !0
                             }
-                            if (r && a instanceof Map && i instanceof Map) {
-                                if (a.size !== i.size) return !1;
-                                for (c = a.entries(); !(u = c.next()).done;)
-                                    if (!i.has(u.value[0])) return !1;
-                                for (c = a.entries(); !(u = c.next()).done;)
-                                    if (!e(u.value[1], i.get(u.value[0]))) return !1;
+                            if (r && o instanceof Map && l instanceof Map) {
+                                if (o.size !== l.size) return !1;
+                                for (c = o.entries(); !(u = c.next()).done;)
+                                    if (!l.has(u.value[0])) return !1;
+                                for (c = o.entries(); !(u = c.next()).done;)
+                                    if (!e(u.value[1], l.get(u.value[0]))) return !1;
                                 return !0
                             }
-                            if (n && a instanceof Set && i instanceof Set) {
-                                if (a.size !== i.size) return !1;
-                                for (c = a.entries(); !(u = c.next()).done;)
-                                    if (!i.has(u.value[0])) return !1;
+                            if (n && o instanceof Set && l instanceof Set) {
+                                if (o.size !== l.size) return !1;
+                                for (c = o.entries(); !(u = c.next()).done;)
+                                    if (!l.has(u.value[0])) return !1;
                                 return !0
                             }
-                            if (o && ArrayBuffer.isView(a) && ArrayBuffer.isView(i)) {
-                                if ((l = a.length) != i.length) return !1;
-                                for (u = l; 0 != u--;)
-                                    if (a[u] !== i[u]) return !1;
+                            if (a && ArrayBuffer.isView(o) && ArrayBuffer.isView(l)) {
+                                if ((i = o.length) != l.length) return !1;
+                                for (u = i; 0 != u--;)
+                                    if (o[u] !== l[u]) return !1;
                                 return !0
                             }
-                            if (a.constructor === RegExp) return a.source === i.source && a.flags === i.flags;
-                            if (a.valueOf !== Object.prototype.valueOf) return a.valueOf() === i.valueOf();
-                            if (a.toString !== Object.prototype.toString) return a.toString() === i.toString();
-                            if ((l = (s = Object.keys(a)).length) !== Object.keys(i).length) return !1;
-                            for (u = l; 0 != u--;)
-                                if (!Object.prototype.hasOwnProperty.call(i, s[u])) return !1;
-                            if (t && a instanceof Element) return !1;
-                            for (u = l; 0 != u--;)
-                                if (("_owner" !== s[u] && "__v" !== s[u] && "__o" !== s[u] || !a.$$typeof) && !e(a[s[u]], i[s[u]])) return !1;
+                            if (o.constructor === RegExp) return o.source === l.source && o.flags === l.flags;
+                            if (o.valueOf !== Object.prototype.valueOf) return o.valueOf() === l.valueOf();
+                            if (o.toString !== Object.prototype.toString) return o.toString() === l.toString();
+                            if ((i = (s = Object.keys(o)).length) !== Object.keys(l).length) return !1;
+                            for (u = i; 0 != u--;)
+                                if (!Object.prototype.hasOwnProperty.call(l, s[u])) return !1;
+                            if (t && o instanceof Element) return !1;
+                            for (u = i; 0 != u--;)
+                                if (("_owner" !== s[u] && "__v" !== s[u] && "__o" !== s[u] || !o.$$typeof) && !e(o[s[u]], l[s[u]])) return !1;
                             return !0
                         }
-                        return a != a && i != i
-                    }(e, a)
+                        return o != o && l != l
+                    }(e, o)
                 } catch (e) {
                     if ((e.message || "").match(/stack|recursion/i)) return console.warn("react-fast-compare cannot handle circular refs"), !1;
                     throw e
                 }
             }
         },
         9605: function(e, t, r) {
@@ -1403,33 +1181,33 @@
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                 })(e)
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.default = void 0;
-            var o, a = function(e) {
+            var a, o = function(e) {
                     if (e && e.__esModule) return e;
                     if (null === e || "object" !== n(e) && "function" != typeof e) return {
                         default: e
                     };
                     var t = s();
                     if (t && t.has(e)) return t.get(e);
                     var r = {},
-                        o = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (var a in e)
-                        if (Object.prototype.hasOwnProperty.call(e, a)) {
-                            var i = o ? Object.getOwnPropertyDescriptor(e, a) : null;
-                            i && (i.get || i.set) ? Object.defineProperty(r, a, i) : r[a] = e[a]
+                        a = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (var o in e)
+                        if (Object.prototype.hasOwnProperty.call(e, o)) {
+                            var l = a ? Object.getOwnPropertyDescriptor(e, o) : null;
+                            l && (l.get || l.set) ? Object.defineProperty(r, o, l) : r[o] = e[o]
                         } return r.default = e, t && t.set(e, r), r
                 }(r(7294)),
-                i = (o = r(9590)) && o.__esModule ? o : {
-                    default: o
+                l = (a = r(9590)) && a.__esModule ? a : {
+                    default: a
                 },
-                l = r(9448),
+                i = r(9448),
                 u = r(6281);
 
             function s() {
                 if ("function" != typeof WeakMap) return null;
                 var e = new WeakMap;
                 return s = function() {
                     return e
@@ -1442,23 +1220,23 @@
                         var r = arguments[t];
                         for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                     }
                     return e
                 }).apply(this, arguments)
             }
 
-            function f(e, t) {
+            function d(e, t) {
                 for (var r = 0; r < t.length; r++) {
                     var n = t[r];
                     n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
                 }
             }
 
-            function d(e, t) {
-                return (d = Object.setPrototypeOf || function(e, t) {
+            function f(e, t) {
+                return (f = Object.setPrototypeOf || function(e, t) {
                     return e.__proto__ = t, e
                 })(e, t)
             }
 
             function p(e) {
                 if (void 0 === e) throw ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return e
@@ -1474,95 +1252,95 @@
                 return t in e ? Object.defineProperty(e, t, {
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
-            var v = function(e) {
+            var m = function(e) {
                 ! function(e, t) {
                     if ("function" != typeof t && null !== t) throw TypeError("Super expression must either be null or a function");
                     e.prototype = Object.create(t && t.prototype, {
                         constructor: {
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
-                    }), t && d(e, t)
+                    }), t && f(e, t)
                 }(s, e);
-                var t, r, o, l = (t = function() {
+                var t, r, a, i = (t = function() {
                     if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                     if ("function" == typeof Proxy) return !0;
                     try {
                         return Date.prototype.toString.call(Reflect.construct(Date, [], function() {})), !0
                     } catch (e) {
                         return !1
                     }
                 }(), function() {
-                    var e, r, o = y(s);
+                    var e, r, a = y(s);
                     if (t) {
-                        var a = y(this).constructor;
-                        r = Reflect.construct(o, arguments, a)
-                    } else r = o.apply(this, arguments);
+                        var o = y(this).constructor;
+                        r = Reflect.construct(a, arguments, o)
+                    } else r = a.apply(this, arguments);
                     return (e = r) && ("object" === n(e) || "function" == typeof e) ? e : p(this)
                 });
 
                 function s() {
                     var e;
                     ! function(e, t) {
                         if (!(e instanceof t)) throw TypeError("Cannot call a class as a function")
                     }(this, s);
                     for (var t = arguments.length, r = Array(t), n = 0; n < t; n++) r[n] = arguments[n];
-                    return h(p(e = l.call.apply(l, [this].concat(r))), "mounted", !1), h(p(e), "isReady", !1), h(p(e), "isPlaying", !1), h(p(e), "isLoading", !0), h(p(e), "loadOnReady", null), h(p(e), "startOnPlay", !0), h(p(e), "seekOnPlay", null), h(p(e), "onDurationCalled", !1), h(p(e), "handlePlayerMount", function(t) {
+                    return h(p(e = i.call.apply(i, [this].concat(r))), "mounted", !1), h(p(e), "isReady", !1), h(p(e), "isPlaying", !1), h(p(e), "isLoading", !0), h(p(e), "loadOnReady", null), h(p(e), "startOnPlay", !0), h(p(e), "seekOnPlay", null), h(p(e), "onDurationCalled", !1), h(p(e), "handlePlayerMount", function(t) {
                         if (e.player) {
                             e.progress();
                             return
                         }
                         e.player = t, e.player.load(e.props.url), e.progress()
                     }), h(p(e), "getInternalPlayer", function(t) {
                         return e.player ? e.player[t] : null
                     }), h(p(e), "progress", function() {
                         if (e.props.url && e.player && e.isReady) {
                             var t = e.getCurrentTime() || 0,
                                 r = e.getSecondsLoaded(),
                                 n = e.getDuration();
                             if (n) {
-                                var o = {
+                                var a = {
                                     playedSeconds: t,
                                     played: t / n
                                 };
-                                null !== r && (o.loadedSeconds = r, o.loaded = r / n), (o.playedSeconds !== e.prevPlayed || o.loadedSeconds !== e.prevLoaded) && e.props.onProgress(o), e.prevPlayed = o.playedSeconds, e.prevLoaded = o.loadedSeconds
+                                null !== r && (a.loadedSeconds = r, a.loaded = r / n), (a.playedSeconds !== e.prevPlayed || a.loadedSeconds !== e.prevLoaded) && e.props.onProgress(a), e.prevPlayed = a.playedSeconds, e.prevLoaded = a.loadedSeconds
                             }
                         }
                         e.progressTimeout = setTimeout(e.progress, e.props.progressFrequency || e.props.progressInterval)
                     }), h(p(e), "handleReady", function() {
                         if (e.mounted) {
                             e.isReady = !0, e.isLoading = !1;
                             var t = e.props,
                                 r = t.onReady,
                                 n = t.playing,
-                                o = t.volume,
-                                a = t.muted;
-                            r(), a || null === o || e.player.setVolume(o), e.loadOnReady ? (e.player.load(e.loadOnReady, !0), e.loadOnReady = null) : n && e.player.play(), e.handleDurationCheck()
+                                a = t.volume,
+                                o = t.muted;
+                            r(), o || null === a || e.player.setVolume(a), e.loadOnReady ? (e.player.load(e.loadOnReady, !0), e.loadOnReady = null) : n && e.player.play(), e.handleDurationCheck()
                         }
                     }), h(p(e), "handlePlay", function() {
                         e.isPlaying = !0, e.isLoading = !1;
                         var t = e.props,
                             r = t.onStart,
                             n = t.onPlay,
-                            o = t.playbackRate;
-                        e.startOnPlay && (e.player.setPlaybackRate && 1 !== o && e.player.setPlaybackRate(o), r(), e.startOnPlay = !1), n(), e.seekOnPlay && (e.seekTo(e.seekOnPlay), e.seekOnPlay = null), e.handleDurationCheck()
+                            a = t.playbackRate;
+                        e.startOnPlay && (e.player.setPlaybackRate && 1 !== a && e.player.setPlaybackRate(a), r(), e.startOnPlay = !1), n(), e.seekOnPlay && (e.seekTo(e.seekOnPlay), e.seekOnPlay = null), e.handleDurationCheck()
                     }), h(p(e), "handlePause", function(t) {
                         e.isPlaying = !1, e.isLoading || e.props.onPause(t)
                     }), h(p(e), "handleEnded", function() {
                         var t = e.props,
                             r = t.activePlayer,
                             n = t.loop,
-                            o = t.onEnded;
-                        r.loopOnEnded && n && e.seekTo(0), n || (e.isPlaying = !1, o())
+                            a = t.onEnded;
+                        r.loopOnEnded && n && e.seekTo(0), n || (e.isPlaying = !1, a())
                     }), h(p(e), "handleError", function() {
                         var t;
                         e.isLoading = !1, (t = e.props).onError.apply(t, arguments)
                     }), h(p(e), "handleDurationCheck", function() {
                         clearTimeout(e.durationCheckTimeout);
                         var t = e.getDuration();
                         t ? e.onDurationCalled || (e.props.onDuration(t), e.onDurationCalled = !0) : e.durationCheckTimeout = setTimeout(e.handleDurationCheck, 100)
@@ -1583,32 +1361,32 @@
                 }, {
                     key: "componentDidUpdate",
                     value: function(e) {
                         var t = this;
                         if (this.player) {
                             var r = this.props,
                                 n = r.url,
-                                o = r.playing,
-                                a = r.volume,
-                                l = r.muted,
+                                a = r.playing,
+                                o = r.volume,
+                                i = r.muted,
                                 s = r.playbackRate,
                                 c = r.pip,
-                                f = r.loop,
-                                d = r.activePlayer,
+                                d = r.loop,
+                                f = r.activePlayer,
                                 p = r.disableDeferredLoading;
-                            if (!(0, i.default)(e.url, n)) {
-                                if (this.isLoading && !d.forceLoad && !p && !(0, u.isMediaStream)(n)) {
+                            if (!(0, l.default)(e.url, n)) {
+                                if (this.isLoading && !f.forceLoad && !p && !(0, u.isMediaStream)(n)) {
                                     console.warn("ReactPlayer: the attempt to load ".concat(n, " is being deferred until the player has loaded")), this.loadOnReady = n;
                                     return
                                 }
                                 this.isLoading = !0, this.startOnPlay = !0, this.onDurationCalled = !1, this.player.load(n, this.isReady)
                             }
-                            e.playing || !o || this.isPlaying || this.player.play(), e.playing && !o && this.isPlaying && this.player.pause(), !e.pip && c && this.player.enablePIP && this.player.enablePIP(), e.pip && !c && this.player.disablePIP && this.player.disablePIP(), e.volume !== a && null !== a && this.player.setVolume(a), e.muted !== l && (l ? this.player.mute() : (this.player.unmute(), null !== a && setTimeout(function() {
-                                return t.player.setVolume(a)
-                            }))), e.playbackRate !== s && this.player.setPlaybackRate && this.player.setPlaybackRate(s), e.loop !== f && this.player.setLoop && this.player.setLoop(f)
+                            e.playing || !a || this.isPlaying || this.player.play(), e.playing && !a && this.isPlaying && this.player.pause(), !e.pip && c && this.player.enablePIP && this.player.enablePIP(), e.pip && !c && this.player.disablePIP && this.player.disablePIP(), e.volume !== o && null !== o && this.player.setVolume(o), e.muted !== i && (i ? this.player.mute() : (this.player.unmute(), null !== o && setTimeout(function() {
+                                return t.player.setVolume(o)
+                            }))), e.playbackRate !== s && this.player.setPlaybackRate && this.player.setPlaybackRate(s), e.loop !== d && this.player.setLoop && this.player.setLoop(d)
                         }
                     }
                 }, {
                     key: "getDuration",
                     value: function() {
                         return this.isReady ? this.player.getDuration() : null
                     }
@@ -1643,73 +1421,73 @@
                         }
                         this.player.seekTo(e)
                     }
                 }, {
                     key: "render",
                     value: function() {
                         var e = this.props.activePlayer;
-                        return e ? a.default.createElement(e, c({}, this.props, {
+                        return e ? o.default.createElement(e, c({}, this.props, {
                             onMount: this.handlePlayerMount,
                             onReady: this.handleReady,
                             onPlay: this.handlePlay,
                             onPause: this.handlePause,
                             onEnded: this.handleEnded,
                             onLoaded: this.handleLoaded,
                             onError: this.handleError
                         })) : null
                     }
-                }], f(s.prototype, r), o && f(s, o), s
-            }(a.Component);
-            t.default = v, h(v, "displayName", "Player"), h(v, "propTypes", l.propTypes), h(v, "defaultProps", l.defaultProps)
+                }], d(s.prototype, r), a && d(s, a), s
+            }(o.Component);
+            t.default = m, h(m, "displayName", "Player"), h(m, "propTypes", i.propTypes), h(m, "defaultProps", i.defaultProps)
         },
-        8800: function(e, t, r) {
+        1276: function(e, t, r) {
             "use strict";
 
             function n(e) {
                 return (n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                 })(e)
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.createReactPlayer = void 0;
-            var o = function(e) {
+            var a = function(e) {
                     if (e && e.__esModule) return e;
                     if (null === e || "object" !== n(e) && "function" != typeof e) return {
                         default: e
                     };
-                    var t = d();
+                    var t = f();
                     if (t && t.has(e)) return t.get(e);
                     var r = {},
-                        o = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (var a in e)
-                        if (Object.prototype.hasOwnProperty.call(e, a)) {
-                            var i = o ? Object.getOwnPropertyDescriptor(e, a) : null;
-                            i && (i.get || i.set) ? Object.defineProperty(r, a, i) : r[a] = e[a]
+                        a = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (var o in e)
+                        if (Object.prototype.hasOwnProperty.call(e, o)) {
+                            var l = a ? Object.getOwnPropertyDescriptor(e, o) : null;
+                            l && (l.get || l.set) ? Object.defineProperty(r, o, l) : r[o] = e[o]
                         } return r.default = e, t && t.set(e, r), r
                 }(r(7294)),
-                a = f(r(9996)),
-                i = f(r(845)),
-                l = f(r(9590)),
+                o = d(r(9996)),
+                l = d(r(845)),
+                i = d(r(9590)),
                 u = r(9448),
                 s = r(6281),
-                c = f(r(9605));
+                c = d(r(9605));
 
-            function f(e) {
+            function d(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
 
-            function d() {
+            function f() {
                 if ("function" != typeof WeakMap) return null;
                 var e = new WeakMap;
-                return d = function() {
+                return f = function() {
                     return e
                 }, e
             }
 
             function p(e, t) {
                 var r = Object.keys(e);
                 if (Object.getOwnPropertySymbols) {
@@ -1739,32 +1517,32 @@
                         var r = arguments[t];
                         for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                     }
                     return e
                 }).apply(this, arguments)
             }
 
-            function v(e) {
+            function m(e) {
                 return function(e) {
-                    if (Array.isArray(e)) return m(e)
+                    if (Array.isArray(e)) return v(e)
                 }(e) || function(e) {
                     if ("undefined" != typeof Symbol && Symbol.iterator in Object(e)) return Array.from(e)
                 }(e) || function(e, t) {
                     if (e) {
-                        if ("string" == typeof e) return m(e, t);
+                        if ("string" == typeof e) return v(e, t);
                         var r = Object.prototype.toString.call(e).slice(8, -1);
                         if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                        if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return m(e, t)
+                        if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return v(e, t)
                     }
                 }(e) || function() {
                     throw TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }
 
-            function m(e, t) {
+            function v(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
 
             function b(e, t) {
                 for (var r = 0; r < t.length; r++) {
@@ -1794,61 +1572,61 @@
                 return t in e ? Object.defineProperty(e, t, {
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
-            var O = (0, o.lazy)(function() {
+            var S = (0, a.lazy)(function() {
                     return r.e(664).then(r.bind(r, 7284))
                 }),
-                S = "undefined" != typeof window && window.document,
-                _ = void 0 !== r.g && r.g.window && r.g.window.document,
-                x = Object.keys(u.propTypes),
-                A = S || _ ? o.Suspense : function() {
+                O = "undefined" != typeof window && window.document,
+                x = void 0 !== r.g && r.g.window && r.g.window.document,
+                _ = Object.keys(u.propTypes),
+                A = O || x ? a.Suspense : function() {
                     return null
                 },
                 T = [];
             t.createReactPlayer = function(e, t) {
-                var r, f;
-                return f = r = function(r) {
+                var r, d;
+                return d = r = function(r) {
                     (function(e, t) {
                         if ("function" != typeof t && null !== t) throw TypeError("Super expression must either be null or a function");
                         e.prototype = Object.create(t && t.prototype, {
                             constructor: {
                                 value: e,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), t && g(e, t)
-                    })(S, r);
-                    var f, d, p, m = (f = function() {
+                    })(O, r);
+                    var d, f, p, v = (d = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Date.prototype.toString.call(Reflect.construct(Date, [], function() {})), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t, r = w(S);
-                        if (f) {
-                            var o = w(this).constructor;
-                            t = Reflect.construct(r, arguments, o)
+                        var e, t, r = w(O);
+                        if (d) {
+                            var a = w(this).constructor;
+                            t = Reflect.construct(r, arguments, a)
                         } else t = r.apply(this, arguments);
                         return (e = t) && ("object" === n(e) || "function" == typeof e) ? e : P(this)
                     });
 
-                    function S() {
+                    function O() {
                         var r;
                         (function(e, t) {
                             if (!(e instanceof t)) throw TypeError("Cannot call a class as a function")
-                        })(this, S);
-                        for (var n = arguments.length, l = Array(n), f = 0; f < n; f++) l[f] = arguments[f];
-                        return k(P(r = m.call.apply(m, [this].concat(l))), "state", {
+                        })(this, O);
+                        for (var n = arguments.length, i = Array(n), d = 0; d < n; d++) i[d] = arguments[d];
+                        return k(P(r = v.call.apply(v, [this].concat(i))), "state", {
                             showPreview: !!r.props.light
                         }), k(P(r), "references", {
                             wrapper: function(e) {
                                 r.wrapper = e
                             },
                             player: function(e) {
                                 r.player = e
@@ -1871,43 +1649,43 @@
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "player";
                             return r.player ? r.player.getInternalPlayer(e) : null
                         }), k(P(r), "seekTo", function(e, t) {
                             if (!r.player) return null;
                             r.player.seekTo(e, t)
                         }), k(P(r), "handleReady", function() {
                             r.props.onReady(P(r))
-                        }), k(P(r), "getActivePlayer", (0, i.default)(function(r) {
-                            for (var n = 0, o = [].concat(T, v(e)); n < o.length; n++) {
-                                var a = o[n];
-                                if (a.canPlay(r)) return a
+                        }), k(P(r), "getActivePlayer", (0, l.default)(function(r) {
+                            for (var n = 0, a = [].concat(T, m(e)); n < a.length; n++) {
+                                var o = a[n];
+                                if (o.canPlay(r)) return o
                             }
                             return t || null
-                        })), k(P(r), "getConfig", (0, i.default)(function(e, t) {
+                        })), k(P(r), "getConfig", (0, l.default)(function(e, t) {
                             var n = r.props.config;
-                            return a.default.all([u.defaultProps.config, u.defaultProps.config[t] || {}, n, n[t] || {}])
-                        })), k(P(r), "getAttributes", (0, i.default)(function(e) {
-                            return (0, s.omit)(r.props, x)
+                            return o.default.all([u.defaultProps.config, u.defaultProps.config[t] || {}, n, n[t] || {}])
+                        })), k(P(r), "getAttributes", (0, l.default)(function(e) {
+                            return (0, s.omit)(r.props, _)
                         })), k(P(r), "renderActivePlayer", function(e) {
                             if (!e) return null;
                             var t = r.getActivePlayer(e);
                             if (!t) return null;
                             var n = r.getConfig(e, t.key);
-                            return o.default.createElement(c.default, h({}, r.props, {
+                            return a.default.createElement(c.default, h({}, r.props, {
                                 key: t.key,
                                 ref: r.references.player,
                                 config: n,
                                 activePlayer: t.lazyPlayer || t,
                                 onReady: r.handleReady
                             }))
                         }), r
                     }
-                    return d = [{
+                    return f = [{
                         key: "shouldComponentUpdate",
                         value: function(e, t) {
-                            return !(0, l.default)(this.props, e) || !(0, l.default)(this.state, t)
+                            return !(0, i.default)(this.props, e) || !(0, i.default)(this.state, t)
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e) {
                             var t = this.props.light;
                             !e.light && t && this.setState({
                                 showPreview: !0
@@ -1918,173 +1696,173 @@
                     }, {
                         key: "renderPreview",
                         value: function(e) {
                             if (!e) return null;
                             var t = this.props,
                                 r = t.light,
                                 n = t.playIcon,
-                                a = t.previewTabIndex,
-                                i = t.oEmbedUrl;
-                            return o.default.createElement(O, {
+                                o = t.previewTabIndex,
+                                l = t.oEmbedUrl;
+                            return a.default.createElement(S, {
                                 url: e,
                                 light: r,
                                 playIcon: n,
-                                previewTabIndex: a,
-                                oEmbedUrl: i,
+                                previewTabIndex: o,
+                                oEmbedUrl: l,
                                 onClick: this.handleClickPreview
                             })
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this.props,
                                 t = e.url,
                                 r = e.style,
                                 n = e.width,
-                                a = e.height,
-                                i = e.fallback,
-                                l = e.wrapper,
+                                o = e.height,
+                                l = e.fallback,
+                                i = e.wrapper,
                                 u = this.state.showPreview,
                                 s = this.getAttributes(t),
-                                c = "string" == typeof l ? this.references.wrapper : void 0;
-                            return o.default.createElement(l, h({
+                                c = "string" == typeof i ? this.references.wrapper : void 0;
+                            return a.default.createElement(i, h({
                                 ref: c,
                                 style: y(y({}, r), {}, {
                                     width: n,
-                                    height: a
+                                    height: o
                                 })
-                            }, s), o.default.createElement(A, {
-                                fallback: i
+                            }, s), a.default.createElement(A, {
+                                fallback: l
                             }, u ? this.renderPreview(t) : this.renderActivePlayer(t)))
                         }
-                    }], b(S.prototype, d), p && b(S, p), S
-                }(o.Component), k(r, "displayName", "ReactPlayer"), k(r, "propTypes", u.propTypes), k(r, "defaultProps", u.defaultProps), k(r, "addCustomPlayer", function(e) {
+                    }], b(O.prototype, f), p && b(O, p), O
+                }(a.Component), k(r, "displayName", "ReactPlayer"), k(r, "propTypes", u.propTypes), k(r, "defaultProps", u.defaultProps), k(r, "addCustomPlayer", function(e) {
                     T.push(e)
                 }), k(r, "removeCustomPlayers", function() {
                     T.length = 0
                 }), k(r, "canPlay", function(t) {
-                    for (var r = 0, n = [].concat(T, v(e)); r < n.length; r++)
+                    for (var r = 0, n = [].concat(T, m(e)); r < n.length; r++)
                         if (n[r].canPlay(t)) return !0;
                     return !1
                 }), k(r, "canEnablePIP", function(t) {
-                    for (var r = 0, n = [].concat(T, v(e)); r < n.length; r++) {
-                        var o = n[r];
-                        if (o.canEnablePIP && o.canEnablePIP(t)) return !0
+                    for (var r = 0, n = [].concat(T, m(e)); r < n.length; r++) {
+                        var a = n[r];
+                        if (a.canEnablePIP && a.canEnablePIP(t)) return !0
                     }
                     return !1
-                }), f
+                }), d
             }
         },
         6310: function(e, t, r) {
             "use strict";
             t.Z = void 0;
-            var n, o = (n = r(9760)) && n.__esModule ? n : {
+            var n, a = (n = r(9760)) && n.__esModule ? n : {
                     default: n
                 },
-                a = r(8800),
-                i = o.default[o.default.length - 1],
-                l = (0, a.createReactPlayer)(o.default, i);
-            t.Z = l
+                o = r(1276),
+                l = a.default[a.default.length - 1],
+                i = (0, o.createReactPlayer)(a.default, l);
+            t.Z = i
         },
         9790: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.canPlay = t.FLV_EXTENSIONS = t.DASH_EXTENSIONS = t.HLS_EXTENSIONS = t.VIDEO_EXTENSIONS = t.AUDIO_EXTENSIONS = t.MATCH_URL_KALTURA = t.MATCH_URL_VIDYARD = t.MATCH_URL_MIXCLOUD = t.MATCH_URL_DAILYMOTION = t.MATCH_URL_TWITCH_CHANNEL = t.MATCH_URL_TWITCH_VIDEO = t.MATCH_URL_WISTIA = t.MATCH_URL_STREAMABLE = t.MATCH_URL_FACEBOOK_WATCH = t.MATCH_URL_FACEBOOK = t.MATCH_URL_VIMEO = t.MATCH_URL_SOUNDCLOUD = t.MATCH_URL_YOUTUBE = void 0;
             var n = r(6281);
 
-            function o(e, t) {
+            function a(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
-            var a = /(?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:embed\/|v\/|watch\/|watch\?v=|watch\?.+&v=|shorts\/|live\/))((\w|-){11})|youtube\.com\/playlist\?list=|youtube\.com\/user\//;
-            t.MATCH_URL_YOUTUBE = a;
-            var i = /(?:soundcloud\.com|snd\.sc)\/[^.]+$/;
-            t.MATCH_URL_SOUNDCLOUD = i;
-            var l = /vimeo\.com\/(?!progressive_redirect).+/;
-            t.MATCH_URL_VIMEO = l;
+            var o = /(?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:embed\/|v\/|watch\/|watch\?v=|watch\?.+&v=|shorts\/|live\/))((\w|-){11})|youtube\.com\/playlist\?list=|youtube\.com\/user\//;
+            t.MATCH_URL_YOUTUBE = o;
+            var l = /(?:soundcloud\.com|snd\.sc)\/[^.]+$/;
+            t.MATCH_URL_SOUNDCLOUD = l;
+            var i = /vimeo\.com\/(?!progressive_redirect).+/;
+            t.MATCH_URL_VIMEO = i;
             var u = /^https?:\/\/(www\.)?facebook\.com.*\/(video(s)?|watch|story)(\.php?|\/).+$/;
             t.MATCH_URL_FACEBOOK = u;
             var s = /^https?:\/\/fb\.watch\/.+$/;
             t.MATCH_URL_FACEBOOK_WATCH = s;
             var c = /streamable\.com\/([a-z0-9]+)$/;
             t.MATCH_URL_STREAMABLE = c;
-            var f = /(?:wistia\.(?:com|net)|wi\.st)\/(?:medias|embed)\/(?:iframe\/)?(.*)$/;
-            t.MATCH_URL_WISTIA = f;
-            var d = /(?:www\.|go\.)?twitch\.tv\/videos\/(\d+)($|\?)/;
-            t.MATCH_URL_TWITCH_VIDEO = d;
+            var d = /(?:wistia\.(?:com|net)|wi\.st)\/(?:medias|embed)\/(?:iframe\/)?(.*)$/;
+            t.MATCH_URL_WISTIA = d;
+            var f = /(?:www\.|go\.)?twitch\.tv\/videos\/(\d+)($|\?)/;
+            t.MATCH_URL_TWITCH_VIDEO = f;
             var p = /(?:www\.|go\.)?twitch\.tv\/([a-zA-Z0-9_]+)($|\?)/;
             t.MATCH_URL_TWITCH_CHANNEL = p;
             var y = /^(?:(?:https?):)?(?:\/\/)?(?:www\.)?(?:(?:dailymotion\.com(?:\/embed)?\/video)|dai\.ly)\/([a-zA-Z0-9]+)(?:_[\w_-]+)?(?:[\w.#_-]+)?/;
             t.MATCH_URL_DAILYMOTION = y;
             var h = /mixcloud\.com\/([^/]+\/[^/]+)/;
             t.MATCH_URL_MIXCLOUD = h;
-            var v = /vidyard.com\/(?:watch\/)?([a-zA-Z0-9-_]+)/;
-            t.MATCH_URL_VIDYARD = v;
-            var m = /^https?:\/\/[a-zA-Z]+\.kaltura.(com|org)\/p\/([0-9]+)\/sp\/([0-9]+)00\/embedIframeJs\/uiconf_id\/([0-9]+)\/partner_id\/([0-9]+)(.*)entry_id.([a-zA-Z0-9-_].*)$/;
-            t.MATCH_URL_KALTURA = m;
+            var m = /vidyard.com\/(?:watch\/)?([a-zA-Z0-9-_]+)/;
+            t.MATCH_URL_VIDYARD = m;
+            var v = /^https?:\/\/[a-zA-Z]+\.kaltura.(com|org)\/p\/([0-9]+)\/sp\/([0-9]+)00\/embedIframeJs\/uiconf_id\/([0-9]+)\/partner_id\/([0-9]+)(.*)entry_id.([a-zA-Z0-9-_].*)$/;
+            t.MATCH_URL_KALTURA = v;
             var b = /\.(m4a|m4b|mp4a|mpga|mp2|mp2a|mp3|m2a|m3a|wav|weba|aac|oga|spx)($|\?)/i;
             t.AUDIO_EXTENSIONS = b;
             var g = /\.(mp4|og[gv]|webm|mov|m4v)(#t=[,\d+]+)?($|\?)/i;
             t.VIDEO_EXTENSIONS = g;
             var P = /\.(m3u8)($|\?)/i;
             t.HLS_EXTENSIONS = P;
             var w = /\.(mpd)($|\?)/i;
             t.DASH_EXTENSIONS = w;
             var k = /\.(flv)($|\?)/i;
             t.FLV_EXTENSIONS = k, t.canPlay = {
                 youtube: function(e) {
                     return e instanceof Array ? e.every(function(e) {
-                        return a.test(e)
-                    }) : a.test(e)
+                        return o.test(e)
+                    }) : o.test(e)
                 },
                 soundcloud: function(e) {
-                    return i.test(e) && !b.test(e)
+                    return l.test(e) && !b.test(e)
                 },
                 vimeo: function(e) {
-                    return l.test(e) && !g.test(e) && !P.test(e)
+                    return i.test(e) && !g.test(e) && !P.test(e)
                 },
                 facebook: function(e) {
                     return u.test(e) || s.test(e)
                 },
                 streamable: function(e) {
                     return c.test(e)
                 },
                 wistia: function(e) {
-                    return f.test(e)
+                    return d.test(e)
                 },
                 twitch: function(e) {
-                    return d.test(e) || p.test(e)
+                    return f.test(e) || p.test(e)
                 },
                 dailymotion: function(e) {
                     return y.test(e)
                 },
                 mixcloud: function(e) {
                     return h.test(e)
                 },
                 vidyard: function(e) {
-                    return v.test(e)
+                    return m.test(e)
                 },
                 kaltura: function(e) {
-                    return m.test(e)
+                    return v.test(e)
                 },
                 file: function e(t) {
                     if (t instanceof Array) {
-                        var r, a = function(e, t) {
+                        var r, o = function(e, t) {
                             if ("undefined" == typeof Symbol || null == e[Symbol.iterator]) {
-                                if (Array.isArray(e) || (a = function(e, t) {
+                                if (Array.isArray(e) || (o = function(e, t) {
                                         if (e) {
-                                            if ("string" == typeof e) return o(e, t);
+                                            if ("string" == typeof e) return a(e, t);
                                             var r = Object.prototype.toString.call(e).slice(8, -1);
                                             if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return o(e, t)
+                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return a(e, t)
                                         }
                                     }(e))) {
-                                    a && (e = a);
+                                    o && (e = o);
                                     var r = 0,
                                         n = function() {};
                                     return {
                                         s: n,
                                         n: function() {
                                             return r >= e.length ? {
                                                 done: !0
@@ -2097,257 +1875,257 @@
                                             throw e
                                         },
                                         f: n
                                     }
                                 }
                                 throw TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                             }
-                            var a, i, l = !0,
+                            var o, l, i = !0,
                                 u = !1;
                             return {
                                 s: function() {
-                                    a = e[Symbol.iterator]()
+                                    o = e[Symbol.iterator]()
                                 },
                                 n: function() {
-                                    var e = a.next();
-                                    return l = e.done, e
+                                    var e = o.next();
+                                    return i = e.done, e
                                 },
                                 e: function(e) {
-                                    u = !0, i = e
+                                    u = !0, l = e
                                 },
                                 f: function() {
                                     try {
-                                        l || null == a.return || a.return()
+                                        i || null == o.return || o.return()
                                     } finally {
-                                        if (u) throw i
+                                        if (u) throw l
                                     }
                                 }
                             }
                         }(t);
                         try {
-                            for (a.s(); !(r = a.n()).done;) {
-                                var i = r.value;
-                                if ("string" == typeof i && e(i) || e(i.src)) return !0
+                            for (o.s(); !(r = o.n()).done;) {
+                                var l = r.value;
+                                if ("string" == typeof l && e(l) || e(l.src)) return !0
                             }
                         } catch (e) {
-                            a.e(e)
+                            o.e(e)
                         } finally {
-                            a.f()
+                            o.f()
                         }
                         return !1
                     }
                     return !!((0, n.isMediaStream)(t) || (0, n.isBlobUrl)(t)) || b.test(t) || g.test(t) || P.test(t) || w.test(t) || k.test(t)
                 }
             }
         },
         9760: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.default = void 0;
             var n = r(7294),
-                o = r(6281),
-                a = r(9790),
-                i = [{
+                a = r(6281),
+                o = r(9790),
+                l = [{
                     key: "youtube",
                     name: "YouTube",
-                    canPlay: a.canPlay.youtube,
+                    canPlay: o.canPlay.youtube,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(439).then(r.bind(r, 5034))
                     })
                 }, {
                     key: "soundcloud",
                     name: "SoundCloud",
-                    canPlay: a.canPlay.soundcloud,
+                    canPlay: o.canPlay.soundcloud,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(125).then(r.bind(r, 6655))
                     })
                 }, {
                     key: "vimeo",
                     name: "Vimeo",
-                    canPlay: a.canPlay.vimeo,
+                    canPlay: o.canPlay.vimeo,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(743).then(r.bind(r, 6746))
                     })
                 }, {
                     key: "facebook",
                     name: "Facebook",
-                    canPlay: a.canPlay.facebook,
+                    canPlay: o.canPlay.facebook,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(121).then(r.bind(r, 6429))
                     })
                 }, {
                     key: "streamable",
                     name: "Streamable",
-                    canPlay: a.canPlay.streamable,
+                    canPlay: o.canPlay.streamable,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(546).then(r.bind(r, 6479))
                     })
                 }, {
                     key: "wistia",
                     name: "Wistia",
-                    canPlay: a.canPlay.wistia,
+                    canPlay: o.canPlay.wistia,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(55).then(r.bind(r, 3134))
                     })
                 }, {
                     key: "twitch",
                     name: "Twitch",
-                    canPlay: a.canPlay.twitch,
+                    canPlay: o.canPlay.twitch,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(216).then(r.bind(r, 9743))
                     })
                 }, {
                     key: "dailymotion",
                     name: "DailyMotion",
-                    canPlay: a.canPlay.dailymotion,
+                    canPlay: o.canPlay.dailymotion,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(596).then(r.bind(r, 5134))
                     })
                 }, {
                     key: "mixcloud",
                     name: "Mixcloud",
-                    canPlay: a.canPlay.mixcloud,
+                    canPlay: o.canPlay.mixcloud,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(667).then(r.bind(r, 9734))
                     })
                 }, {
                     key: "vidyard",
                     name: "Vidyard",
-                    canPlay: a.canPlay.vidyard,
+                    canPlay: o.canPlay.vidyard,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(965).then(r.bind(r, 7287))
                     })
                 }, {
                     key: "kaltura",
                     name: "Kaltura",
-                    canPlay: a.canPlay.kaltura,
+                    canPlay: o.canPlay.kaltura,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(261).then(r.bind(r, 9289))
                     })
                 }, {
                     key: "file",
                     name: "FilePlayer",
-                    canPlay: a.canPlay.file,
+                    canPlay: o.canPlay.file,
                     canEnablePIP: function(e) {
-                        return a.canPlay.file(e) && (document.pictureInPictureEnabled || (0, o.supportsWebKitPresentationMode)()) && !a.AUDIO_EXTENSIONS.test(e)
+                        return o.canPlay.file(e) && (document.pictureInPictureEnabled || (0, a.supportsWebKitPresentationMode)()) && !o.AUDIO_EXTENSIONS.test(e)
                     },
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(11).then(r.bind(r, 3364))
                     })
                 }];
-            t.default = i
+            t.default = l
         },
         9448: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.defaultProps = t.propTypes = void 0;
-            var n, o = (n = r(5697)) && n.__esModule ? n : {
+            var n, a = (n = r(5697)) && n.__esModule ? n : {
                     default: n
                 },
-                a = o.default.string,
-                i = o.default.bool,
-                l = o.default.number,
-                u = o.default.array,
-                s = o.default.oneOfType,
-                c = o.default.shape,
-                f = o.default.object,
-                d = o.default.func,
-                p = o.default.node,
+                o = a.default.string,
+                l = a.default.bool,
+                i = a.default.number,
+                u = a.default.array,
+                s = a.default.oneOfType,
+                c = a.default.shape,
+                d = a.default.object,
+                f = a.default.func,
+                p = a.default.node,
                 y = {
-                    url: s([a, u, f]),
-                    playing: i,
-                    loop: i,
-                    controls: i,
-                    volume: l,
-                    muted: i,
-                    playbackRate: l,
-                    width: s([a, l]),
-                    height: s([a, l]),
-                    style: f,
-                    progressInterval: l,
-                    playsinline: i,
-                    pip: i,
-                    stopOnUnmount: i,
-                    light: s([i, a, f]),
+                    url: s([o, u, d]),
+                    playing: l,
+                    loop: l,
+                    controls: l,
+                    volume: i,
+                    muted: l,
+                    playbackRate: i,
+                    width: s([o, i]),
+                    height: s([o, i]),
+                    style: d,
+                    progressInterval: i,
+                    playsinline: l,
+                    pip: l,
+                    stopOnUnmount: l,
+                    light: s([l, o, d]),
                     playIcon: p,
-                    previewTabIndex: l,
+                    previewTabIndex: i,
                     fallback: p,
-                    oEmbedUrl: a,
-                    wrapper: s([a, d, c({
-                        render: d.isRequired
+                    oEmbedUrl: o,
+                    wrapper: s([o, f, c({
+                        render: f.isRequired
                     })]),
                     config: c({
                         soundcloud: c({
-                            options: f
+                            options: d
                         }),
                         youtube: c({
-                            playerVars: f,
-                            embedOptions: f,
-                            onUnstarted: d
+                            playerVars: d,
+                            embedOptions: d,
+                            onUnstarted: f
                         }),
                         facebook: c({
-                            appId: a,
-                            version: a,
-                            playerId: a,
-                            attributes: f
+                            appId: o,
+                            version: o,
+                            playerId: o,
+                            attributes: d
                         }),
                         dailymotion: c({
-                            params: f
+                            params: d
                         }),
                         vimeo: c({
-                            playerOptions: f,
-                            title: a
+                            playerOptions: d,
+                            title: o
                         }),
                         file: c({
-                            attributes: f,
+                            attributes: d,
                             tracks: u,
-                            forceVideo: i,
-                            forceAudio: i,
-                            forceHLS: i,
-                            forceSafariHLS: i,
-                            forceDASH: i,
-                            forceFLV: i,
-                            hlsOptions: f,
-                            hlsVersion: a,
-                            dashVersion: a,
-                            flvVersion: a
+                            forceVideo: l,
+                            forceAudio: l,
+                            forceHLS: l,
+                            forceSafariHLS: l,
+                            forceDASH: l,
+                            forceFLV: l,
+                            hlsOptions: d,
+                            hlsVersion: o,
+                            dashVersion: o,
+                            flvVersion: o
                         }),
                         wistia: c({
-                            options: f,
-                            playerId: a,
+                            options: d,
+                            playerId: o,
                             customControls: u
                         }),
                         mixcloud: c({
-                            options: f
+                            options: d
                         }),
                         twitch: c({
-                            options: f,
-                            playerId: a
+                            options: d,
+                            playerId: o
                         }),
                         vidyard: c({
-                            options: f
+                            options: d
                         })
                     }),
-                    onReady: d,
-                    onStart: d,
-                    onPlay: d,
-                    onPause: d,
-                    onBuffer: d,
-                    onBufferEnd: d,
-                    onEnded: d,
-                    onError: d,
-                    onDuration: d,
-                    onSeek: d,
-                    onPlaybackRateChange: d,
-                    onProgress: d,
-                    onClickPreview: d,
-                    onEnablePIP: d,
-                    onDisablePIP: d
+                    onReady: f,
+                    onStart: f,
+                    onPlay: f,
+                    onPause: f,
+                    onBuffer: f,
+                    onBufferEnd: f,
+                    onEnded: f,
+                    onError: f,
+                    onDuration: f,
+                    onSeek: f,
+                    onPlaybackRateChange: f,
+                    onProgress: f,
+                    onClickPreview: f,
+                    onEnablePIP: f,
+                    onDisablePIP: f
                 };
             t.propTypes = y;
             var h = function() {};
             t.defaultProps = {
                 playing: !1,
                 loop: !1,
                 controls: !1,
@@ -2459,152 +2237,152 @@
             }
         },
         6281: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.parseStartTime = function(e) {
-                return f(e, l)
+                return d(e, i)
             }, t.parseEndTime = function(e) {
-                return f(e, u)
+                return d(e, u)
             }, t.randomString = function() {
                 return Math.random().toString(36).substr(2, 5)
             }, t.queryString = function(e) {
                 return Object.keys(e).map(function(t) {
                     return "".concat(t, "=").concat(e[t])
                 }).join("&")
             }, t.getSDK = function(e, t) {
                 var r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null,
-                    o = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : function() {
+                    a = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : function() {
                         return !0
                     },
-                    a = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : n.default,
-                    i = d(t);
-                return i && o(i) ? Promise.resolve(i) : new Promise(function(n, o) {
+                    o = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : n.default,
+                    l = f(t);
+                return l && a(l) ? Promise.resolve(l) : new Promise(function(n, a) {
                     if (p[e]) {
                         p[e].push({
                             resolve: n,
-                            reject: o
+                            reject: a
                         });
                         return
                     }
                     p[e] = [{
                         resolve: n,
-                        reject: o
+                        reject: a
                     }];
-                    var i = function(t) {
+                    var l = function(t) {
                         p[e].forEach(function(e) {
                             return e.resolve(t)
                         })
                     };
                     if (r) {
-                        var l = window[r];
+                        var i = window[r];
                         window[r] = function() {
-                            l && l(), i(d(t))
+                            i && i(), l(f(t))
                         }
                     }
-                    a(e, function(n) {
+                    o(e, function(n) {
                         n ? (p[e].forEach(function(e) {
                             return e.reject(n)
-                        }), p[e] = null) : r || i(d(t))
+                        }), p[e] = null) : r || l(f(t))
                     })
                 })
             }, t.getConfig = function(e, t) {
-                return (0, o.default)(t.config, e.config)
+                return (0, a.default)(t.config, e.config)
             }, t.omit = function(e) {
-                for (var t, r = arguments.length, n = Array(r > 1 ? r - 1 : 0), o = 1; o < r; o++) n[o - 1] = arguments[o];
-                for (var a = (t = []).concat.apply(t, n), i = {}, l = Object.keys(e), u = 0; u < l.length; u++) {
-                    var s = l[u]; - 1 === a.indexOf(s) && (i[s] = e[s])
+                for (var t, r = arguments.length, n = Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) n[a - 1] = arguments[a];
+                for (var o = (t = []).concat.apply(t, n), l = {}, i = Object.keys(e), u = 0; u < i.length; u++) {
+                    var s = i[u]; - 1 === o.indexOf(s) && (l[s] = e[s])
                 }
-                return i
+                return l
             }, t.callPlayer = function(e) {
                 var t;
                 if (!this.player || !this.player[e]) {
                     var r = "ReactPlayer: ".concat(this.constructor.displayName, " player could not call %c").concat(e, "%c – ");
                     return this.player ? this.player[e] || (r += "The method was not available") : r += "The player was not available", console.warn(r, "font-weight: bold", ""), null
                 }
-                for (var n = arguments.length, o = Array(n > 1 ? n - 1 : 0), a = 1; a < n; a++) o[a - 1] = arguments[a];
-                return (t = this.player)[e].apply(t, o)
+                for (var n = arguments.length, a = Array(n > 1 ? n - 1 : 0), o = 1; o < n; o++) a[o - 1] = arguments[o];
+                return (t = this.player)[e].apply(t, a)
             }, t.isMediaStream = function(e) {
                 return "undefined" != typeof window && void 0 !== window.MediaStream && e instanceof window.MediaStream
             }, t.isBlobUrl = function(e) {
                 return /^blob:/.test(e)
             }, t.supportsWebKitPresentationMode = function() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : document.createElement("video"),
                     t = !1 === /iPhone|iPod/.test(navigator.userAgent);
                 return e.webkitSupportsPresentationMode && "function" == typeof e.webkitSetPresentationMode && t
             };
-            var n = a(r(9090)),
-                o = a(r(9996));
+            var n = o(r(9090)),
+                a = o(r(9996));
 
-            function a(e) {
+            function o(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
 
-            function i(e, t) {
+            function l(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
-            var l = /[?&#](?:start|t)=([0-9hms]+)/,
+            var i = /[?&#](?:start|t)=([0-9hms]+)/,
                 u = /[?&#]end=([0-9hms]+)/,
                 s = /(\d+)(h|m|s)/g,
                 c = /^\d+$/;
 
-            function f(e, t) {
+            function d(e, t) {
                 if (!(e instanceof Array)) {
                     var r = e.match(t);
                     if (r) {
                         var n = r[1];
                         if (n.match(s)) return function(e) {
                             for (var t = 0, r = s.exec(e); null !== r;) {
-                                var n, o = function(e) {
+                                var n, a = function(e) {
                                         if (Array.isArray(e)) return e
                                     }(n = r) || function(e, t) {
                                         if ("undefined" != typeof Symbol && Symbol.iterator in Object(e)) {
                                             var r = [],
                                                 n = !0,
-                                                o = !1,
-                                                a = void 0;
+                                                a = !1,
+                                                o = void 0;
                                             try {
-                                                for (var i, l = e[Symbol.iterator](); !(n = (i = l.next()).done) && (r.push(i.value), !t || r.length !== t); n = !0);
+                                                for (var l, i = e[Symbol.iterator](); !(n = (l = i.next()).done) && (r.push(l.value), !t || r.length !== t); n = !0);
                                             } catch (e) {
-                                                o = !0, a = e
+                                                a = !0, o = e
                                             } finally {
                                                 try {
-                                                    n || null == l.return || l.return()
+                                                    n || null == i.return || i.return()
                                                 } finally {
-                                                    if (o) throw a
+                                                    if (a) throw o
                                                 }
                                             }
                                             return r
                                         }
                                     }(n, 3) || function(e, t) {
                                         if (e) {
-                                            if ("string" == typeof e) return i(e, t);
+                                            if ("string" == typeof e) return l(e, t);
                                             var r = Object.prototype.toString.call(e).slice(8, -1);
                                             if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return i(e, t)
+                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return l(e, t)
                                         }
                                     }(n, 3) || function() {
                                         throw TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                     }(),
-                                    a = o[1],
-                                    l = o[2];
-                                "h" === l && (t += 3600 * parseInt(a, 10)), "m" === l && (t += 60 * parseInt(a, 10)), "s" === l && (t += parseInt(a, 10)), r = s.exec(e)
+                                    o = a[1],
+                                    i = a[2];
+                                "h" === i && (t += 3600 * parseInt(o, 10)), "m" === i && (t += 60 * parseInt(o, 10)), "s" === i && (t += parseInt(o, 10)), r = s.exec(e)
                             }
                             return t
                         }(n);
                         if (c.test(n)) return parseInt(n)
                     }
                 }
             }
 
-            function d(e) {
+            function f(e) {
                 return window[e] ? window[e] : window.exports && window.exports[e] ? window.exports[e] : window.module && window.module.exports && window.module.exports[e] ? window.module.exports[e] : null
             }
             var p = {}
         }
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/699-e1dda1328195ce40.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,10 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [699], {
-        8385: function(e, t, r) {
-            var n = r(7294),
-                o = r(3935),
-                i = r(3703),
-                l = r(3546),
-                a = r(7960),
-                s = r(5893);
-            let d = n.forwardRef(function(e, t) {
-                let {
-                    children: r,
-                    container: d,
-                    disablePortal: u = !1
-                } = e, [c, p] = n.useState(null), f = (0, i.Z)(n.isValidElement(r) ? r.ref : null, t);
-                return ((0, l.Z)(() => {
-                    !u && p(("function" == typeof d ? d() : d) || document.body)
-                }, [d, u]), (0, l.Z)(() => {
-                    if (c && !u) return (0, a.Z)(t, c), () => {
-                        (0, a.Z)(t, null)
-                    }
-                }, [t, c, u]), u) ? n.isValidElement(r) ? n.cloneElement(r, {
-                    ref: f
-                }) : (0, s.jsx)(n.Fragment, {
-                    children: r
-                }) : (0, s.jsx)(n.Fragment, {
-                    children: c ? o.createPortal(r, c) : c
-                })
-            });
-            t.Z = d
-        },
-        1873: function(e, t, r) {
-            r.d(t, {
-                T: function() {
-                    return i
-                }
-            });
-            var n = r(7294);
-            r(5893);
-            let o = n.createContext({
-                disableDefaultClasses: !1
-            });
-
-            function i(e) {
-                let {
-                    disableDefaultClasses: t
-                } = n.useContext(o);
-                return r => t ? "" : e(r)
-            }
-        },
         4808: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return g
                 }
             });
             var n = r(3366),
@@ -366,15 +318,15 @@
 
             function a(e) {
                 return (0, i.Z)("MuiInput", e)
             }
             let s = (0, n.Z)({}, l.Z, (0, o.Z)("MuiInput", ["root", "underline", "input"]));
             t.Z = s
         },
-        3970: function(e, t, r) {
+        3032: function(e, t, r) {
             r.d(t, {
                 rA: function() {
                     return j
                 },
                 Ej: function() {
                     return z
                 },
@@ -501,21 +453,20 @@
                     }, x)), (0, m.jsx)("textarea", {
                         "aria-hidden": !0,
                         className: e.className,
                         readOnly: !0,
                         ref: S,
                         tabIndex: -1,
                         style: (0, o.Z)({}, b.shadow, s, {
-                            paddingTop: 0,
-                            paddingBottom: 0
+                            padding: 0
                         })
                     })]
                 })
             });
-            var x = r(8442),
+            var x = r(3247),
                 y = r(5704),
                 R = r(7167),
                 w = r(4423),
                 S = r(948),
                 P = r(1657),
                 k = r(8216),
                 C = r(1705),
@@ -986,15 +937,15 @@
             var g = Z
         },
         9773: function(e, t, r) {
             var n = r(7294);
             let o = n.createContext({});
             t.Z = o
         },
-        2980: function(e, t, r) {
+        9219: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return W
                 }
             });
             var n = r(3366),
                 o = r(7462),
@@ -1006,15 +957,15 @@
 
             function u(...e) {
                 return e.reduce((e, t) => null == t ? e : function(...r) {
                     e.apply(this, r), t.apply(this, r)
                 }, () => {})
             }
             var c = r(4780),
-                p = r(8385),
+                p = r(8173),
                 f = r(4161),
                 m = r(5806);
 
             function h(e, t) {
                 t ? e.setAttribute("aria-hidden", "true") : e.removeAttribute("aria-hidden")
             }
 
@@ -1146,16 +1097,16 @@
                 },
                 w = r(1588),
                 S = r(4867);
 
             function P(e) {
                 return (0, S.Z)("MuiModal", e)
             }(0, w.Z)("MuiModal", ["root", "hidden", "backdrop"]);
-            var k = r(6504),
-                C = r(1873);
+            var k = r(3249),
+                C = r(3905);
             let E = ["children", "closeAfterTransition", "container", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "manager", "onBackdropClick", "onClose", "onKeyDown", "open", "onTransitionEnter", "onTransitionExited", "slotProps", "slots"],
                 M = e => {
                     let {
                         open: t,
                         exited: r
                     } = e;
                     return (0, c.Z)({
@@ -1360,16 +1311,16 @@
                                 isEnabled: J,
                                 open: O,
                                 children: i.cloneElement(c, en)
                             })]
                         }))
                     }) : null
                 });
-            var T = r(1276),
-                N = r(8442),
+            var T = r(7488),
+                N = r(3247),
                 O = r(948),
                 A = r(1657),
                 z = r(4808);
             let j = ["BackdropComponent", "BackdropProps", "classes", "className", "closeAfterTransition", "children", "container", "component", "components", "componentsProps", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "onBackdropClick", "onClose", "open", "slotProps", "slots", "theme"],
                 L = (0, O.ZP)("div", {
                     name: "MuiModal",
                     slot: "Root",
@@ -1549,15 +1500,15 @@
                         easing: t.transitions.easing.easeOut,
                         delay: 50
                     })
                 })));
             var f = r(4423),
                 m = r(5704),
                 h = r(4656),
-                v = r(3970),
+                v = r(3032),
                 b = r(1657);
             let Z = ["components", "fullWidth", "inputComponent", "label", "multiline", "notched", "slots", "type"],
                 g = e => {
                     let {
                         classes: t
                     } = e, r = (0, a.Z)({
                         root: ["root"],
@@ -1697,15 +1648,15 @@
                         } = c,
                         M = (0, o.Z)(c, Z),
                         I = g(c),
                         F = (0, f.Z)(),
                         T = (0, m.Z)({
                             props: c,
                             muiFormControl: F,
-                            states: ["color", "disabled", "error", "focused", "hiddenLabel", "size", "required"]
+                            states: ["required"]
                         }),
                         N = (0, i.Z)({}, c, {
                             color: T.color || "primary",
                             disabled: T.disabled,
                             error: T.error,
                             focused: T.focused,
                             formControl: F,
@@ -1772,15 +1723,15 @@
                 a = r(7294),
                 s = r(6010),
                 d = r(4780),
                 u = r(2996),
                 c = r(948),
                 p = r(1657),
                 f = r(9766),
-                m = r(3970),
+                m = r(3032),
                 h = r(7021),
                 v = r(5893);
             let b = ["disableUnderline", "components", "componentsProps", "fullWidth", "inputComponent", "multiline", "slotProps", "slots", "type"],
                 Z = e => {
                     let {
                         classes: t,
                         disableUnderline: r
@@ -2541,16 +2492,16 @@
                         p && p(e)
                     },
                     tabIndex: n ? 0 : -1
                 }, m, {
                     children: x
                 }))
             });
-            var ec = r(6504),
-                ep = r(8442),
+            var ec = r(3249),
+                ep = r(3247),
                 ef = r(7144),
                 em = r(5340),
                 eh = r(8662),
                 ev = r(2734),
                 eb = r(577);
             let eZ = ["addEndListener", "appear", "children", "easing", "in", "onEnter", "onEntered", "onEntering", "onExit", "onExited", "onExiting", "style", "timeout", "TransitionComponent"];
 
@@ -2657,15 +2608,15 @@
                                 visibility: "exited" !== e || d ? void 0 : "hidden"
                             }, ex[e], b, o.props.style),
                             ref: P
                         }, t))
                     }))
                 });
             eR.muiSupportAuto = !0;
-            var ew = r(2980),
+            var ew = r(9219),
                 eS = r(629);
 
             function eP(e) {
                 return (0, N.Z)("MuiPopover", e)
             }(0, T.Z)("MuiPopover", ["root", "paper"]);
             let ek = ["onEntering"],
                 eC = ["action", "anchorEl", "anchorOrigin", "anchorPosition", "anchorReference", "children", "className", "container", "elevation", "marginThreshold", "open", "PaperProps", "slots", "slotProps", "transformOrigin", "TransitionComponent", "transitionDuration", "TransitionProps"],
@@ -3707,14 +3658,62 @@
             r(7294);
             var n = r(8169),
                 o = r(5893);
             t.Z = (0, n.Z)((0, o.jsx)("path", {
                 d: "M7 10l5 5 5-5z"
             }), "ArrowDropDown")
         },
+        8173: function(e, t, r) {
+            var n = r(7294),
+                o = r(3935),
+                i = r(3703),
+                l = r(3546),
+                a = r(7960),
+                s = r(5893);
+            let d = n.forwardRef(function(e, t) {
+                let {
+                    children: r,
+                    container: d,
+                    disablePortal: u = !1
+                } = e, [c, p] = n.useState(null), f = (0, i.Z)(n.isValidElement(r) ? r.ref : null, t);
+                return ((0, l.Z)(() => {
+                    !u && p(("function" == typeof d ? d() : d) || document.body)
+                }, [d, u]), (0, l.Z)(() => {
+                    if (c && !u) return (0, a.Z)(t, c), () => {
+                        (0, a.Z)(t, null)
+                    }
+                }, [t, c, u]), u) ? n.isValidElement(r) ? n.cloneElement(r, {
+                    ref: f
+                }) : (0, s.jsx)(n.Fragment, {
+                    children: r
+                }) : (0, s.jsx)(n.Fragment, {
+                    children: c ? o.createPortal(r, c) : c
+                })
+            });
+            t.Z = d
+        },
+        3905: function(e, t, r) {
+            r.d(t, {
+                T: function() {
+                    return i
+                }
+            });
+            var n = r(7294);
+            r(5893);
+            let o = n.createContext({
+                disableDefaultClasses: !1
+            });
+
+            function i(e) {
+                let {
+                    disableDefaultClasses: t
+                } = n.useContext(o);
+                return r => t ? "" : e(r)
+            }
+        },
         1579: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return o
                 }
             });
             var n = r(7294),
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/713-307f96321a681e2c.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [713], {
-        9713: function(e, t, o) {
+    [913], {
+        3913: function(e, t, o) {
             o.d(t, {
                 Z: function() {
                     return tI
                 }
             });
             var r, n, a, i, l, s, c, p = o(3366),
                 u = o(7462),
@@ -1042,23 +1042,23 @@
                             return e()
                         }), i = []
                     }
                     return c.setOptions(o).then(function(e) {
                         !s && o.onFirstUpdate && o.onFirstUpdate(e)
                     }), c
                 }),
-                eR = o(8385),
+                eR = o(8173),
                 eL = o(4867),
                 eA = o(1588);
 
             function eD(e) {
                 return (0, eL.Z)("MuiPopper", e)
             }(0, eA.Z)("MuiPopper", ["root"]);
-            var eE = o(6504),
-                eM = o(1873),
+            var eE = o(3249),
+                eM = o(3905),
                 eT = o(5893);
             let ej = ["anchorEl", "children", "direction", "disablePortal", "modifiers", "open", "placement", "popperOptions", "popperRef", "slotProps", "slots", "TransitionProps", "ownerState"],
                 eN = ["anchorEl", "children", "container", "direction", "disablePortal", "keepMounted", "modifiers", "open", "placement", "popperOptions", "popperRef", "style", "transition", "slotProps", "slots"];
 
             function ez(e) {
                 return "function" == typeof e ? e() : e
             }
@@ -2701,15 +2701,15 @@
                             });
                             return eX((0, u.Z)({}, o, {
                                 className: eK.option
                             }), e, {
                                 selected: o["aria-selected"],
                                 index: t,
                                 inputValue: eE
-                            }, eq)
+                            })
                         },
                         eJ = null != (o = eg.clearIndicator) ? o : D.clearIndicator,
                         eQ = null != (r = eg.paper) ? r : D.paper,
                         e0 = null != (n = eg.popper) ? n : D.popper,
                         e1 = null != (a = eg.popupIndicator) ? a : D.popupIndicator;
                     return (0, eT.jsxs)(d.Fragment, {
                         children: [(0, eT.jsx)(tv, (0, u.Z)({
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/731-adbd7bf9e28fe493.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,110 +1,9 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [731], {
-        8442: function(e, t, l) {
-            "use strict";
-
-            function r(e) {
-                return "string" == typeof e
-            }
-            l.d(t, {
-                Z: function() {
-                    return r
-                }
-            })
-        },
-        1276: function(e, t, l) {
-            "use strict";
-
-            function r(e, t, l) {
-                return "function" == typeof e ? e(t, l) : e
-            }
-            l.d(t, {
-                Z: function() {
-                    return r
-                }
-            })
-        },
-        6504: function(e, t, l) {
-            "use strict";
-            l.d(t, {
-                Z: function() {
-                    return d
-                }
-            });
-            var r = l(7462),
-                o = l(3366),
-                n = l(3703),
-                i = l(8442),
-                a = l(6010);
-
-            function s(e) {
-                if (void 0 === e) return {};
-                let t = {};
-                return Object.keys(e).filter(t => !(t.match(/^on[A-Z]/) && "function" == typeof e[t])).forEach(l => {
-                    t[l] = e[l]
-                }), t
-            }
-            var c = l(1276);
-            let u = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
-
-            function d(e) {
-                var t, l;
-                let {
-                    elementType: d,
-                    externalSlotProps: f,
-                    ownerState: p,
-                    skipResolvingSlotProps: h = !1
-                } = e, b = (0, o.Z)(e, u), m = h ? {} : (0, c.Z)(f, p), {
-                    props: v,
-                    internalRef: y
-                } = function(e) {
-                    let {
-                        getSlotProps: t,
-                        additionalProps: l,
-                        externalSlotProps: o,
-                        externalForwardedProps: n,
-                        className: i
-                    } = e;
-                    if (!t) {
-                        let e = (0, a.Z)(null == n ? void 0 : n.className, null == o ? void 0 : o.className, i, null == l ? void 0 : l.className),
-                            t = (0, r.Z)({}, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
-                            s = (0, r.Z)({}, l, n, o);
-                        return e.length > 0 && (s.className = e), Object.keys(t).length > 0 && (s.style = t), {
-                            props: s,
-                            internalRef: void 0
-                        }
-                    }
-                    let c = function(e, t = []) {
-                            if (void 0 === e) return {};
-                            let l = {};
-                            return Object.keys(e).filter(l => l.match(/^on[A-Z]/) && "function" == typeof e[l] && !t.includes(l)).forEach(t => {
-                                l[t] = e[t]
-                            }), l
-                        }((0, r.Z)({}, n, o)),
-                        u = s(o),
-                        d = s(n),
-                        f = t(c),
-                        p = (0, a.Z)(null == f ? void 0 : f.className, null == l ? void 0 : l.className, i, null == n ? void 0 : n.className, null == o ? void 0 : o.className),
-                        h = (0, r.Z)({}, null == f ? void 0 : f.style, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
-                        b = (0, r.Z)({}, f, l, d, u);
-                    return p.length > 0 && (b.className = p), Object.keys(h).length > 0 && (b.style = h), {
-                        props: b,
-                        internalRef: f.ref
-                    }
-                }((0, r.Z)({}, b, {
-                    externalSlotProps: m
-                })), Z = (0, n.Z)(y, null == m ? void 0 : m.ref, null == (t = e.additionalProps) ? void 0 : t.ref), g = (l = (0, r.Z)({}, v, {
-                    ref: Z
-                }), void 0 === d || (0, i.Z)(d) ? l : (0, r.Z)({}, l, {
-                    ownerState: (0, r.Z)({}, l.ownerState, p)
-                }));
-                return g
-            }
-        },
         4267: function(e, t, l) {
             "use strict";
             l.d(t, {
                 Z: function() {
                     return y
                 }
             });
@@ -351,15 +250,15 @@
             });
             var o = l(3366),
                 n = l(7462),
                 i = l(7294);
             l(9864);
             var a = l(6010),
                 s = l(4780),
-                c = l(6504),
+                c = l(3249),
                 u = l(948),
                 d = l(1657),
                 f = l(2734),
                 p = l(7144);
 
             function h() {
                 if (r) return r;
@@ -418,15 +317,15 @@
                         orientation: l,
                         disabled: r
                     } = e;
                     return (0, s.Z)({
                         root: ["root", l, r && "disabled"]
                     }, E, t)
                 },
-                k = (0, u.ZP)(_.Z, {
+                N = (0, u.ZP)(_.Z, {
                     name: "MuiTabScrollButton",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.root, l.orientation && t[l.orientation]]
@@ -443,15 +342,15 @@
                 }, "vertical" === e.orientation && {
                     width: "100%",
                     height: 40,
                     "& svg": {
                         transform: `rotate(${e.isRtl?-90:90}deg)`
                     }
                 })),
-                N = i.forwardRef(function(e, t) {
+                k = i.forwardRef(function(e, t) {
                     var l, r;
                     let i = (0, d.Z)({
                             props: e,
                             name: "MuiTabScrollButton"
                         }),
                         {
                             className: s,
@@ -480,15 +379,15 @@
                             elementType: w,
                             externalSlotProps: p.endScrollButtonIcon,
                             additionalProps: {
                                 fontSize: "small"
                             },
                             ownerState: y
                         });
-                    return (0, Z.jsx)(k, (0, n.Z)({
+                    return (0, Z.jsx)(N, (0, n.Z)({
                         component: "div",
                         className: (0, a.Z)(g.root, s),
                         ref: t,
                         role: null,
                         ownerState: y,
                         tabIndex: null
                     }, b, {
@@ -691,18 +590,18 @@
                             children: w,
                             className: S,
                             component: C = "div",
                             allowScrollButtonsMobile: _ = !1,
                             indicatorColor: B = "primary",
                             onChange: P,
                             orientation: E = "horizontal",
-                            ScrollButtonComponent: M = N,
+                            ScrollButtonComponent: M = k,
                             scrollButtons: R = "auto",
                             selectionFollowsFocus: T,
-                            slots: k = {},
+                            slots: N = {},
                             slotProps: W = {},
                             TabIndicatorProps: I = {},
                             TabScrollButtonProps: q = {},
                             textColor: K = "primary",
                             value: U,
                             variant: J = "standard",
                             visibleScrollbar: Q = !1
@@ -730,20 +629,20 @@
                             scrollableX: et && !el,
                             scrollableY: et && el,
                             centered: x && !et,
                             scrollButtonsHideMobile: !_
                         }),
                         ec = H(es),
                         eu = (0, c.Z)({
-                            elementType: k.StartScrollButtonIcon,
+                            elementType: N.StartScrollButtonIcon,
                             externalSlotProps: W.startScrollButtonIcon,
                             ownerState: es
                         }),
                         ed = (0, c.Z)({
-                            elementType: k.EndScrollButtonIcon,
+                            elementType: N.EndScrollButtonIcon,
                             externalSlotProps: W.endScrollButtonIcon,
                             ownerState: es
                         }),
                         [ef, ep] = i.useState(!1),
                         [eh, eb] = i.useState(G),
                         [em, ev] = i.useState({
                             start: !1,
@@ -881,15 +780,15 @@
                                     let r = t[er] + (l[en] - t[en]);
                                     e_(r, {
                                         animation: e
                                     })
                                 }
                             }
                         }),
-                        ek = (0, j.Z)(() => {
+                        eN = (0, j.Z)(() => {
                             if (et && !1 !== R) {
                                 let e, t;
                                 let {
                                     scrollTop: l,
                                     scrollHeight: o,
                                     clientHeight: n,
                                     scrollWidth: i,
@@ -904,38 +803,38 @@
                                     end: t
                                 })
                             }
                         });
                     i.useEffect(() => {
                         let e;
                         let t = (0, p.Z)(() => {
-                                ex.current && (eC(), ek())
+                                ex.current && (eC(), eN())
                             }),
                             l = (0, y.Z)(ex.current);
                         return l.addEventListener("resize", t), "undefined" != typeof ResizeObserver && (e = new ResizeObserver(t), Array.from(ew.current.children).forEach(t => {
                             e.observe(t)
                         })), () => {
                             t.clear(), l.removeEventListener("resize", t), e && e.disconnect()
                         }
-                    }, [eC, ek]);
-                    let eN = i.useMemo(() => (0, p.Z)(() => {
-                        ek()
-                    }), [ek]);
+                    }, [eC, eN]);
+                    let ek = i.useMemo(() => (0, p.Z)(() => {
+                        eN()
+                    }), [eN]);
                     i.useEffect(() => () => {
-                        eN.clear()
-                    }, [eN]), i.useEffect(() => {
+                        ek.clear()
+                    }, [ek]), i.useEffect(() => {
                         ep(!0)
                     }, []), i.useEffect(() => {
-                        eC(), ek()
+                        eC(), eN()
                     }), i.useEffect(() => {
                         eT(G !== eh)
                     }, [eT, eh]), i.useImperativeHandle(g, () => ({
                         updateIndicator: eC,
-                        updateScrollButtons: ek
-                    }), [eC, ek]);
+                        updateScrollButtons: eN
+                    }), [eC, eN]);
                     let ej = (0, Z.jsx)(V, (0, n.Z)({}, I, {
                             className: (0, a.Z)(ec.indicator, I.className),
                             ownerState: es,
                             style: (0, n.Z)({}, eh, I.style)
                         })),
                         eW = 0,
                         eI = i.Children.map(w, e => {
@@ -961,28 +860,28 @@
                                 onChange: eR,
                                 className: (0, a.Z)(ec.scrollableX, ec.hideScrollbar)
                             }) : null;
                             let t = em.start || em.end,
                                 l = et && ("auto" === R && t || !0 === R);
                             return e.scrollButtonStart = l ? (0, Z.jsx)(M, (0, n.Z)({
                                 slots: {
-                                    StartScrollButtonIcon: k.StartScrollButtonIcon
+                                    StartScrollButtonIcon: N.StartScrollButtonIcon
                                 },
                                 slotProps: {
                                     startScrollButtonIcon: eu
                                 },
                                 orientation: E,
                                 direction: s ? "right" : "left",
                                 onClick: eE,
                                 disabled: !em.start
                             }, q, {
                                 className: (0, a.Z)(ec.scrollButtons, q.className)
                             })) : null, e.scrollButtonEnd = l ? (0, Z.jsx)(M, (0, n.Z)({
                                 slots: {
-                                    EndScrollButtonIcon: k.EndScrollButtonIcon
+                                    EndScrollButtonIcon: N.EndScrollButtonIcon
                                 },
                                 slotProps: {
                                     endScrollButtonIcon: ed
                                 },
                                 orientation: E,
                                 direction: s ? "left" : "right",
                                 onClick: eM,
@@ -1001,15 +900,15 @@
                             className: ec.scroller,
                             ownerState: es,
                             style: {
                                 overflow: ey.overflow,
                                 [el ? `margin${s?"Left":"Right"}` : "marginBottom"]: Q ? void 0 : -ey.scrollbarWidth
                             },
                             ref: ex,
-                            onScroll: eN,
+                            onScroll: ek,
                             children: [(0, Z.jsx)(X, {
                                 "aria-label": u,
                                 "aria-labelledby": v,
                                 "aria-orientation": "vertical" === E ? "vertical" : null,
                                 className: ec.flexContainer,
                                 ownerState: es,
                                 onKeyDown: e => {
@@ -1038,14 +937,114 @@
                                 children: eI
                             }), ef && ej]
                         }), eL.scrollButtonEnd]
                     }))
                 });
             var K = q
         },
+        3247: function(e, t, l) {
+            "use strict";
+
+            function r(e) {
+                return "string" == typeof e
+            }
+            l.d(t, {
+                Z: function() {
+                    return r
+                }
+            })
+        },
+        7488: function(e, t, l) {
+            "use strict";
+
+            function r(e, t) {
+                return "function" == typeof e ? e(t) : e
+            }
+            l.d(t, {
+                Z: function() {
+                    return r
+                }
+            })
+        },
+        3249: function(e, t, l) {
+            "use strict";
+            l.d(t, {
+                Z: function() {
+                    return d
+                }
+            });
+            var r = l(7462),
+                o = l(3366),
+                n = l(3703),
+                i = l(3247),
+                a = l(6010);
+
+            function s(e) {
+                if (void 0 === e) return {};
+                let t = {};
+                return Object.keys(e).filter(t => !(t.match(/^on[A-Z]/) && "function" == typeof e[t])).forEach(l => {
+                    t[l] = e[l]
+                }), t
+            }
+            var c = l(7488);
+            let u = ["elementType", "externalSlotProps", "ownerState"];
+
+            function d(e) {
+                var t, l;
+                let {
+                    elementType: d,
+                    externalSlotProps: f,
+                    ownerState: p
+                } = e, h = (0, o.Z)(e, u), b = (0, c.Z)(f, p), {
+                    props: m,
+                    internalRef: v
+                } = function(e) {
+                    let {
+                        getSlotProps: t,
+                        additionalProps: l,
+                        externalSlotProps: o,
+                        externalForwardedProps: n,
+                        className: i
+                    } = e;
+                    if (!t) {
+                        let e = (0, a.Z)(null == n ? void 0 : n.className, null == o ? void 0 : o.className, i, null == l ? void 0 : l.className),
+                            t = (0, r.Z)({}, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
+                            s = (0, r.Z)({}, l, n, o);
+                        return e.length > 0 && (s.className = e), Object.keys(t).length > 0 && (s.style = t), {
+                            props: s,
+                            internalRef: void 0
+                        }
+                    }
+                    let c = function(e, t = []) {
+                            if (void 0 === e) return {};
+                            let l = {};
+                            return Object.keys(e).filter(l => l.match(/^on[A-Z]/) && "function" == typeof e[l] && !t.includes(l)).forEach(t => {
+                                l[t] = e[t]
+                            }), l
+                        }((0, r.Z)({}, n, o)),
+                        u = s(o),
+                        d = s(n),
+                        f = t(c),
+                        p = (0, a.Z)(null == f ? void 0 : f.className, null == l ? void 0 : l.className, i, null == n ? void 0 : n.className, null == o ? void 0 : o.className),
+                        h = (0, r.Z)({}, null == f ? void 0 : f.style, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
+                        b = (0, r.Z)({}, f, l, d, u);
+                    return p.length > 0 && (b.className = p), Object.keys(h).length > 0 && (b.style = h), {
+                        props: b,
+                        internalRef: f.ref
+                    }
+                }((0, r.Z)({}, h, {
+                    externalSlotProps: b
+                })), y = (0, n.Z)(v, null == b ? void 0 : b.ref, null == (t = e.additionalProps) ? void 0 : t.ref), Z = (l = (0, r.Z)({}, m, {
+                    ref: y
+                }), void 0 === d || (0, i.Z)(d) ? l : (0, r.Z)({}, l, {
+                    ownerState: (0, r.Z)({}, l.ownerState, p)
+                }));
+                return Z
+            }
+        },
         2690: function(e, t, l) {
             "use strict";
 
             function r(e) {
                 return e && e.ownerDocument || document
             }
             l.d(t, {
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/767-13c0b6c8b2e638dd.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
                 n = r(6010),
                 l = r(4780),
                 s = r(2996),
                 d = r(8216),
-                c = r(2980),
+                c = r(9219),
                 p = r(6628),
                 u = r(629),
                 m = r(1657),
                 Z = r(948),
                 v = r(1588),
                 f = r(4867);
 
@@ -484,15 +484,15 @@
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
                 n = r(6010),
                 l = r(4780),
-                s = r(8442),
+                s = r(3247),
                 d = r(1796),
                 c = r(948),
                 p = r(1657),
                 u = r(2022),
                 m = r(1579),
                 Z = r(8974),
                 v = r(1705),
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/839-49c1e145187c690b.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,108 +1,10 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [839], {
-        8442: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return i
-                }
-            });
-
-            function i(t) {
-                return "string" == typeof t
-            }
-        },
-        1276: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return i
-                }
-            });
-
-            function i(t, n, e) {
-                return "function" == typeof t ? t(n, e) : t
-            }
-        },
-        6504: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return d
-                }
-            });
-            var i = e(7462),
-                o = e(3366),
-                r = e(3703),
-                s = e(8442),
-                a = e(6010);
-
-            function u(t) {
-                if (void 0 === t) return {};
-                let n = {};
-                return Object.keys(t).filter(n => !(n.match(/^on[A-Z]/) && "function" == typeof t[n])).forEach(e => {
-                    n[e] = t[e]
-                }), n
-            }
-            var l = e(1276);
-            let c = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
-
-            function d(t) {
-                var n, e;
-                let {
-                    elementType: d,
-                    externalSlotProps: p,
-                    ownerState: f,
-                    skipResolvingSlotProps: h = !1
-                } = t, E = (0, o.Z)(t, c), x = h ? {} : (0, l.Z)(p, f), {
-                    props: m,
-                    internalRef: v
-                } = function(t) {
-                    let {
-                        getSlotProps: n,
-                        additionalProps: e,
-                        externalSlotProps: o,
-                        externalForwardedProps: r,
-                        className: s
-                    } = t;
-                    if (!n) {
-                        let t = (0, a.Z)(null == r ? void 0 : r.className, null == o ? void 0 : o.className, s, null == e ? void 0 : e.className),
-                            n = (0, i.Z)({}, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
-                            u = (0, i.Z)({}, e, r, o);
-                        return t.length > 0 && (u.className = t), Object.keys(n).length > 0 && (u.style = n), {
-                            props: u,
-                            internalRef: void 0
-                        }
-                    }
-                    let l = function(t, n = []) {
-                            if (void 0 === t) return {};
-                            let e = {};
-                            return Object.keys(t).filter(e => e.match(/^on[A-Z]/) && "function" == typeof t[e] && !n.includes(e)).forEach(n => {
-                                e[n] = t[n]
-                            }), e
-                        }((0, i.Z)({}, r, o)),
-                        c = u(o),
-                        d = u(r),
-                        p = n(l),
-                        f = (0, a.Z)(null == p ? void 0 : p.className, null == e ? void 0 : e.className, s, null == r ? void 0 : r.className, null == o ? void 0 : o.className),
-                        h = (0, i.Z)({}, null == p ? void 0 : p.style, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
-                        E = (0, i.Z)({}, p, e, d, c);
-                    return f.length > 0 && (E.className = f), Object.keys(h).length > 0 && (E.style = h), {
-                        props: E,
-                        internalRef: p.ref
-                    }
-                }((0, i.Z)({}, E, {
-                    externalSlotProps: x
-                })), y = (0, r.Z)(v, null == x ? void 0 : x.ref, null == (n = t.additionalProps) ? void 0 : n.ref), Z = (e = (0, i.Z)({}, m, {
-                    ref: y
-                }), void 0 === d || (0, s.Z)(d) ? e : (0, i.Z)({}, e, {
-                    ownerState: (0, i.Z)({}, e.ownerState, f)
-                }));
-                return Z
-            }
-        },
+    [418], {
         6628: function(t, n, e) {
             var i = e(7462),
                 o = e(3366),
                 r = e(7294),
                 s = e(8662),
                 a = e(2734),
                 u = e(577),
@@ -144,16 +46,16 @@
                         D = (0, l.Z)(R, x.ref, n),
                         w = t => n => {
                             if (t) {
                                 let e = R.current;
                                 void 0 === n ? t(e) : t(e, n)
                             }
                         },
-                        P = w(b),
-                        M = w((t, n) => {
+                        M = w(b),
+                        P = w((t, n) => {
                             (0, u.n)(t);
                             let i = (0, u.C)({
                                 style: C,
                                 timeout: N,
                                 easing: m
                             }, {
                                 mode: "enter"
@@ -173,17 +75,17 @@
                             t.style.webkitTransition = e.transitions.create("opacity", n), t.style.transition = e.transitions.create("opacity", n), g && g(t)
                         }),
                         U = w(S);
                     return (0, c.jsx)(T, (0, i.Z)({
                         appear: E,
                         in: v,
                         nodeRef: R,
-                        onEnter: M,
+                        onEnter: P,
                         onEntered: L,
-                        onEntering: P,
+                        onEntering: M,
                         onExit: I,
                         onExited: U,
                         onExiting: j,
                         addEndListener: t => {
                             h && h(R.current, t)
                         },
                         timeout: N
@@ -195,14 +97,111 @@
                             }, p[t], C, x.props.style),
                             ref: D
                         }, n))
                     }))
                 });
             n.Z = f
         },
+        3247: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return i
+                }
+            });
+
+            function i(t) {
+                return "string" == typeof t
+            }
+        },
+        7488: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return i
+                }
+            });
+
+            function i(t, n) {
+                return "function" == typeof t ? t(n) : t
+            }
+        },
+        3249: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return d
+                }
+            });
+            var i = e(7462),
+                o = e(3366),
+                r = e(3703),
+                s = e(3247),
+                a = e(6010);
+
+            function u(t) {
+                if (void 0 === t) return {};
+                let n = {};
+                return Object.keys(t).filter(n => !(n.match(/^on[A-Z]/) && "function" == typeof t[n])).forEach(e => {
+                    n[e] = t[e]
+                }), n
+            }
+            var l = e(7488);
+            let c = ["elementType", "externalSlotProps", "ownerState"];
+
+            function d(t) {
+                var n, e;
+                let {
+                    elementType: d,
+                    externalSlotProps: p,
+                    ownerState: f
+                } = t, h = (0, o.Z)(t, c), E = (0, l.Z)(p, f), {
+                    props: x,
+                    internalRef: m
+                } = function(t) {
+                    let {
+                        getSlotProps: n,
+                        additionalProps: e,
+                        externalSlotProps: o,
+                        externalForwardedProps: r,
+                        className: s
+                    } = t;
+                    if (!n) {
+                        let t = (0, a.Z)(null == r ? void 0 : r.className, null == o ? void 0 : o.className, s, null == e ? void 0 : e.className),
+                            n = (0, i.Z)({}, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
+                            u = (0, i.Z)({}, e, r, o);
+                        return t.length > 0 && (u.className = t), Object.keys(n).length > 0 && (u.style = n), {
+                            props: u,
+                            internalRef: void 0
+                        }
+                    }
+                    let l = function(t, n = []) {
+                            if (void 0 === t) return {};
+                            let e = {};
+                            return Object.keys(t).filter(e => e.match(/^on[A-Z]/) && "function" == typeof t[e] && !n.includes(e)).forEach(n => {
+                                e[n] = t[n]
+                            }), e
+                        }((0, i.Z)({}, r, o)),
+                        c = u(o),
+                        d = u(r),
+                        p = n(l),
+                        f = (0, a.Z)(null == p ? void 0 : p.className, null == e ? void 0 : e.className, s, null == r ? void 0 : r.className, null == o ? void 0 : o.className),
+                        h = (0, i.Z)({}, null == p ? void 0 : p.style, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
+                        E = (0, i.Z)({}, p, e, d, c);
+                    return f.length > 0 && (E.className = f), Object.keys(h).length > 0 && (E.style = h), {
+                        props: E,
+                        internalRef: p.ref
+                    }
+                }((0, i.Z)({}, h, {
+                    externalSlotProps: E
+                })), v = (0, r.Z)(m, null == E ? void 0 : E.ref, null == (n = t.additionalProps) ? void 0 : n.ref), y = (e = (0, i.Z)({}, x, {
+                    ref: v
+                }), void 0 === d || (0, s.Z)(d) ? e : (0, i.Z)({}, e, {
+                    ownerState: (0, i.Z)({}, e.ownerState, f)
+                }));
+                return y
+            }
+        },
         577: function(t, n, e) {
             e.d(n, {
                 C: function() {
                     return o
                 },
                 n: function() {
                     return i
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/main-bfbd70c9b9a5a25b.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -232,15 +232,15 @@
                     router: function() {
                         return n
                     },
                     emitter: function() {
                         return V
                     },
                     initialize: function() {
-                        return K
+                        return J
                     },
                     hydrate: function() {
                         return ec
                     }
                 });
             let g = r(8754);
             r(37);
@@ -250,48 +250,48 @@
                 v = g._(r(6595)),
                 P = r(9955),
                 w = r(3105),
                 S = r(3162),
                 j = r(3908),
                 O = r(7905),
                 E = r(9064),
-                R = r(3232),
-                x = g._(r(9623)),
+                x = r(3232),
+                R = g._(r(9623)),
                 C = g._(r(9030)),
                 M = g._(r(5108)),
                 A = r(2827),
                 L = r(6885),
-                I = r(676),
-                T = r(3341),
+                T = r(676),
+                I = r(3341),
                 N = r(9577),
                 k = r(2140),
                 D = r(4224),
                 B = r(9486),
                 H = r(8463),
                 U = g._(r(4225)),
                 F = e => t => e(t) + "",
-                W = r.u;
-            r.u = F(W);
-            let q = r.k;
-            r.k = F(q);
+                q = r.u;
+            r.u = F(q);
+            let W = r.k;
+            r.k = F(W);
             let z = r.miniCssF;
             r.miniCssF = F(z);
-            let G = "13.4.9",
+            let G = "13.4.7",
                 V = (0, v.default)(),
                 X = e => [].slice.call(e),
-                $ = !1;
+                Y = !1;
             self.__next_require__ = r;
-            class Y extends y.default.Component {
+            class $ extends y.default.Component {
                 componentDidCatch(e, t) {
                     this.props.fn(e, t)
                 }
                 componentDidMount() {
-                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, S.isDynamicRoute)(n.pathname) || location.search || $) || a.props && a.props.__N_SSG && (location.search || $)) && n.replace(n.pathname + "?" + String((0, j.assign)((0, j.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
+                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, S.isDynamicRoute)(n.pathname) || location.search || Y) || a.props && a.props.__N_SSG && (location.search || Y)) && n.replace(n.pathname + "?" + String((0, j.assign)((0, j.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
                         _h: 1,
-                        shallow: !a.isFallback && !$
+                        shallow: !a.isFallback && !Y
                     }).catch(e => {
                         if (!e.cancelled) throw e
                     })
                 }
                 componentDidUpdate() {
                     this.scrollToHash()
                 }
@@ -303,15 +303,15 @@
                     let t = document.getElementById(e);
                     t && setTimeout(() => t.scrollIntoView(), 0)
                 }
                 render() {
                     return this.props.children
                 }
             }
-            async function K(e) {
+            async function J(e) {
                 void 0 === e && (e = {}), a = JSON.parse(document.getElementById("__NEXT_DATA__").textContent), window.__NEXT_DATA__ = a, p = a.defaultLocale;
                 let t = a.assetPrefix || "";
                 if (r.p = "" + t + "/_next/", (0, O.setConfig)({
                         serverRuntimeConfig: {},
                         publicRuntimeConfig: a.runtimeConfig || {}
                     }), o = (0, E.getURL)(), (0, k.hasBasePath)(o) && (o = (0, N.removeBasePath)(o)), a.scriptLoader) {
                     let {
@@ -320,45 +320,45 @@
                     e(a.scriptLoader)
                 }
                 i = new C.default(a.buildId, t);
                 let s = e => {
                     let [t, r] = e;
                     return i.routeLoader.onEntrypoint(t, r)
                 };
-                return window.__NEXT_P && window.__NEXT_P.map(e => setTimeout(() => s(e), 0)), window.__NEXT_P = [], window.__NEXT_P.push = s, (u = (0, x.default)()).getIsSsr = () => n.isSsr, l = document.getElementById("__next"), {
+                return window.__NEXT_P && window.__NEXT_P.map(e => setTimeout(() => s(e), 0)), window.__NEXT_P = [], window.__NEXT_P.push = s, (u = (0, R.default)()).getIsSsr = () => n.isSsr, l = document.getElementById("__next"), {
                     assetPrefix: t
                 }
             }
 
-            function J(e, t) {
+            function K(e, t) {
                 return y.default.createElement(e, t)
             }
 
             function Q(e) {
                 var t;
                 let {
                     children: r
-                } = e, a = y.default.useMemo(() => (0, B.adaptForAppRouterInstance)(n), []);
-                return y.default.createElement(Y, {
+                } = e;
+                return y.default.createElement($, {
                     fn: e => ee({
                         App: f,
                         err: e
                     }).catch(e => console.error("Error rendering page: ", e))
                 }, y.default.createElement(D.AppRouterContext.Provider, {
-                    value: a
+                    value: (0, B.adaptForAppRouterInstance)(n)
                 }, y.default.createElement(H.SearchParamsContext.Provider, {
                     value: (0, B.adaptForSearchParams)(n)
                 }, y.default.createElement(B.PathnameContextProviderAdapter, {
                     router: n,
                     isAutoExport: null != (t = self.__NEXT_DATA__.autoExport) && t
                 }, y.default.createElement(P.RouterContext.Provider, {
                     value: (0, L.makePublicRouterInstance)(n)
                 }, y.default.createElement(b.HeadManagerContext.Provider, {
                     value: u
-                }, y.default.createElement(T.ImageConfigContext.Provider, {
+                }, y.default.createElement(I.ImageConfigContext.Provider, {
                     value: {
                         deviceSizes: [640, 750, 828, 1080, 1200, 1920, 2048, 3840],
                         imageSizes: [16, 32, 48, 64, 96, 128, 256, 384],
                         path: "/_next/image",
                         loader: "default",
                         dangerouslyAllowSVG: !1,
                         unoptimized: !1
@@ -368,15 +368,15 @@
             let Z = e => t => {
                 let r = {
                     ...t,
                     Component: h,
                     err: a.err,
                     router: n
                 };
-                return y.default.createElement(Q, null, J(e, r))
+                return y.default.createElement(Q, null, K(e, r))
             };
 
             function ee(e) {
                 let {
                     App: t,
                     err: l
                 } = e;
@@ -522,15 +522,15 @@
                                 y: r
                             } = e.scroll;
                             (0, w.handleSmoothScroll)(() => {
                                 window.scrollTo(t, r)
                             })
                         }
                     }
-                }), y.default.createElement(Q, null, J(r, f), y.default.createElement(R.Portal, {
+                }), y.default.createElement(Q, null, K(r, f), y.default.createElement(x.Portal, {
                     type: "next-route-announcer"
                 }, y.default.createElement(A.RouteAnnouncer, null))));
                 return ! function(e, t) {
                     E.ST && performance.mark("beforeRender");
                     let r = t(en ? eo : ei);
                     if (er) {
                         let e = y.default.startTransition;
@@ -548,15 +548,15 @@
                 if (e.err) {
                     await ee(e);
                     return
                 }
                 try {
                     await eu(e)
                 } catch (r) {
-                    let t = (0, I.getProperError)(r);
+                    let t = (0, T.getProperError)(r);
                     if (t.cancelled) throw t;
                     await ee({
                         ...e,
                         err: t
                     })
                 }
             }
@@ -591,15 +591,15 @@
                         };
                         c && (d.attribution = c), r.reportWebVitals(d)
                     });
                     let n = await i.routeLoader.whenEntrypoint(a.page);
                     if ("error" in n) throw n.error;
                     h = n.component
                 } catch (e) {
-                    t = (0, I.getProperError)(e)
+                    t = (0, T.getProperError)(e)
                 }
                 window.__NEXT_PRELOADREADY && await window.__NEXT_PRELOADREADY(a.dynamicIds), n = (0, L.createRouter)(a.page, a.query, o, {
                     initialProps: a.props,
                     pageLoader: i,
                     App: f,
                     Component: h,
                     wrapApp: Z,
@@ -610,15 +610,15 @@
                         scroll: r
                     })),
                     locale: a.locale,
                     locales: a.locales,
                     defaultLocale: p,
                     domainLocales: a.domainLocales,
                     isPreview: a.isPreview
-                }), $ = await n._initialMatchesMiddlewarePromise;
+                }), Y = await n._initialMatchesMiddlewarePromise;
                 let r = {
                     App: f,
                     initial: !0,
                     Component: h,
                     props: a.props,
                     err: t
                 };
@@ -2019,29 +2019,14 @@
                 a = r(8106);
 
             function o(e) {
                 let t = (0, a.normalizePathSep)(e);
                 return t.startsWith("/index/") && !(0, n.isDynamicRoute)(t) ? t.slice(6) : "/index" !== t ? t : "/"
             }
         },
-        7302: function(e, t) {
-            "use strict";
-
-            function r(e) {
-                return e.startsWith("/") ? e : "/" + e
-            }
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), Object.defineProperty(t, "ensureLeadingSlash", {
-                enumerable: !0,
-                get: function() {
-                    return r
-                }
-            })
-        },
         8106: function(e, t) {
             "use strict";
 
             function r(e) {
                 return e.replace(/\\/g, "/")
             }
             Object.defineProperty(t, "__esModule", {
@@ -2162,15 +2147,15 @@
                     default: function() {
                         return V
                     },
                     matchesMiddleware: function() {
                         return N
                     },
                     createKey: function() {
-                        return q
+                        return W
                     }
                 });
             let n = r(8754),
                 a = r(1757),
                 o = r(7734),
                 i = r(5564),
                 l = r(5442),
@@ -2191,23 +2176,23 @@
                 v = r(2080),
                 P = r(9577),
                 w = r(4266),
                 S = r(2140),
                 j = r(9423),
                 O = r(6373),
                 E = r(9473),
-                R = r(6385),
-                x = r(3353),
+                x = r(6385),
+                R = r(3353),
                 C = r(293),
                 M = r(5821),
                 A = r(4532),
                 L = r(5036),
-                I = r(3105);
+                T = r(3105);
 
-            function T() {
+            function I() {
                 return Object.assign(Error("Route Cancelled"), {
                     cancelled: !0
                 })
             }
             async function N(e) {
                 let t = await Promise.resolve(e.router.pageLoader.getMiddleware());
                 if (!t) return !1;
@@ -2350,15 +2335,15 @@
                 try {
                     return JSON.parse(e)
                 } catch (e) {
                     return null
                 }
             }
 
-            function W(e) {
+            function q(e) {
                 var t;
                 let {
                     dataHref: r,
                     inflightCache: n,
                     isPrefetch: a,
                     hasMiddleware: o,
                     isServerRender: l,
@@ -2424,15 +2409,15 @@
                     throw f || delete n[d], ("Failed to fetch" === e.message || "NetworkError when attempting to fetch resource." === e.message || "Load failed" === e.message) && (0, i.markAssetError)(e), e
                 });
                 return f && s ? h({}).then(e => (n[d] = Promise.resolve(e), e)) : void 0 !== n[d] ? n[d] : n[d] = h(c ? {
                     method: "HEAD"
                 } : {})
             }
 
-            function q() {
+            function W() {
                 return Math.random().toString(36).slice(2, 10)
             }
 
             function z(e) {
                 let {
                     url: t,
                     router: r
@@ -2506,53 +2491,53 @@
                                     }
                                 }
                             }
                     }
                     return !1
                 }
                 async change(e, t, r, n, a) {
-                    var s, c, f, j, O, E, C, A, I;
+                    var s, c, f, j, O, E, C, A, T;
                     let k, H;
-                    if (!(0, x.isLocalURL)(t)) return z({
+                    if (!(0, R.isLocalURL)(t)) return z({
                         url: t,
                         router: this
                     }), !1;
                     let F = 1 === n._h;
                     F || n.shallow || await this._bfl(r, void 0, n.locale);
-                    let W = F || n._shouldResolveHref || (0, _.parsePath)(t).pathname === (0, _.parsePath)(r).pathname,
-                        q = {
+                    let q = F || n._shouldResolveHref || (0, _.parsePath)(t).pathname === (0, _.parsePath)(r).pathname,
+                        W = {
                             ...this.state
                         },
                         G = !0 !== this.isReady;
                     this.isReady = !0;
                     let X = this.isSsr;
                     if (F || (this.isSsr = !1), F && this.clc) return !1;
-                    let $ = q.locale;
+                    let Y = W.locale;
                     d.ST && performance.mark("routeChange");
                     let {
-                        shallow: Y = !1,
-                        scroll: K = !0
-                    } = n, J = {
-                        shallow: Y
+                        shallow: $ = !1,
+                        scroll: J = !0
+                    } = n, K = {
+                        shallow: $
                     };
-                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", T(), this._inFlightRoute, J), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
-                    let Q = (0, v.removeLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, q.locale);
+                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", I(), this._inFlightRoute, K), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
+                    let Q = (0, v.removeLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, W.locale);
                     this._inFlightRoute = r;
-                    let Z = $ !== q.locale;
+                    let Z = Y !== W.locale;
                     if (!F && this.onlyAHashChange(Q) && !Z) {
-                        q.asPath = Q, V.events.emit("hashChangeStart", r, J), this.changeState(e, t, r, {
+                        W.asPath = Q, V.events.emit("hashChangeStart", r, K), this.changeState(e, t, r, {
                             ...n,
                             scroll: !1
-                        }), K && this.scrollToHash(Q);
+                        }), J && this.scrollToHash(Q);
                         try {
-                            await this.set(q, this.components[q.route], null)
+                            await this.set(W, this.components[W.route], null)
                         } catch (e) {
-                            throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, J), e
+                            throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, K), e
                         }
-                        return V.events.emit("hashChangeComplete", r, J), !0
+                        return V.events.emit("hashChangeComplete", r, K), !0
                     }
                     let ee = (0, p.parseRelativeUrl)(t),
                         {
                             pathname: et,
                             query: er
                         } = ee;
                     if (null == (s = this.components[et]) ? void 0 : s.__appRouter) return z({
@@ -2573,22 +2558,22 @@
                     let en = r;
                     et = et ? (0, o.removeTrailingSlash)((0, P.removeBasePath)(et)) : et;
                     let ea = (0, o.removeTrailingSlash)(et),
                         eo = r.startsWith("/") && (0, p.parseRelativeUrl)(r).pathname,
                         ei = !!(eo && ea !== eo && (!(0, h.isDynamicRoute)(ea) || !(0, m.getRouteMatcher)((0, g.getRouteRegex)(ea))(eo))),
                         el = !n.shallow && await N({
                             asPath: r,
-                            locale: q.locale,
+                            locale: W.locale,
                             router: this
                         });
-                    if (F && el && (W = !1), W && "/_error" !== et && (n._shouldResolveHref = !0, ee.pathname = B(et, k), ee.pathname === et || (et = ee.pathname, ee.pathname = (0, w.addBasePath)(et), el || (t = (0, y.formatWithValidation)(ee)))), !(0, x.isLocalURL)(r)) return z({
+                    if (F && el && (q = !1), q && "/_error" !== et && (n._shouldResolveHref = !0, ee.pathname = B(et, k), ee.pathname === et || (et = ee.pathname, ee.pathname = (0, w.addBasePath)(et), el || (t = (0, y.formatWithValidation)(ee)))), !(0, R.isLocalURL)(r)) return z({
                         url: r,
                         router: this
                     }), !1;
-                    en = (0, v.removeLocale)((0, P.removeBasePath)(en), q.locale), ea = (0, o.removeTrailingSlash)(et);
+                    en = (0, v.removeLocale)((0, P.removeBasePath)(en), W.locale), ea = (0, o.removeTrailingSlash)(et);
                     let eu = !1;
                     if ((0, h.isDynamicRoute)(ea)) {
                         let e = (0, p.parseRelativeUrl)(en),
                             n = e.pathname,
                             a = (0, g.getRouteRegex)(ea);
                         eu = (0, m.getRouteMatcher)(a)(n);
                         let o = ea === n,
@@ -2598,38 +2583,38 @@
                             query: (0, M.omit)(er, i.params)
                         })) : Object.assign(er, eu);
                         else {
                             let e = Object.keys(a.groups).filter(e => !er[e] && !a.groups[e].optional);
                             if (e.length > 0 && !el) throw Error((o ? "The provided `href` (" + t + ") value is missing query values (" + e.join(", ") + ") to be interpolated properly. " : "The provided `as` value (" + n + ") is incompatible with the `href` value (" + ea + "). ") + "Read more: https://nextjs.org/docs/messages/" + (o ? "href-interpolation-failed" : "incompatible-href-as"))
                         }
                     }
-                    F || V.events.emit("routeChangeStart", r, J);
+                    F || V.events.emit("routeChangeStart", r, K);
                     let es = "/404" === this.pathname || "/_error" === this.pathname;
                     try {
                         let o = await this.getRouteInfo({
                             route: ea,
                             pathname: et,
                             query: er,
                             as: r,
                             resolvedAs: en,
-                            routeProps: J,
-                            locale: q.locale,
-                            isPreview: q.isPreview,
+                            routeProps: K,
+                            locale: W.locale,
+                            isPreview: W.isPreview,
                             hasMiddleware: el,
                             unstable_skipClientCache: n.unstable_skipClientCache,
                             isQueryUpdating: F && !this.isFallback,
                             isMiddlewareRewrite: ei
                         });
-                        if (F || n.shallow || await this._bfl(r, "resolvedAs" in o ? o.resolvedAs : void 0, q.locale), "route" in o && el) {
-                            ea = et = o.route || ea, J.shallow || (er = Object.assign({}, o.query || {}, er));
+                        if (F || n.shallow || await this._bfl(r, "resolvedAs" in o ? o.resolvedAs : void 0, W.locale), "route" in o && el) {
+                            ea = et = o.route || ea, K.shallow || (er = Object.assign({}, o.query || {}, er));
                             let e = (0, S.hasBasePath)(ee.pathname) ? (0, P.removeBasePath)(ee.pathname) : ee.pathname;
                             if (eu && et !== e && Object.keys(eu).forEach(e => {
                                     eu && er[e] === eu[e] && delete er[e]
                                 }), (0, h.isDynamicRoute)(et)) {
-                                let e = !J.shallow && o.resolvedAs ? o.resolvedAs : (0, w.addBasePath)((0, b.addLocale)(new URL(r, location.href).pathname, q.locale), !0),
+                                let e = !K.shallow && o.resolvedAs ? o.resolvedAs : (0, w.addBasePath)((0, b.addLocale)(new URL(r, location.href).pathname, W.locale), !0),
                                     t = e;
                                 (0, S.hasBasePath)(t) && (t = (0, P.removeBasePath)(t));
                                 let n = (0, g.getRouteRegex)(et),
                                     a = (0, m.getRouteMatcher)(n)(new URL(t, location.href).pathname);
                                 a && Object.assign(er, a)
                             }
                         }
@@ -2661,15 +2646,15 @@
                                     return this.change(e, a, o, n)
                                 }
                                 return z({
                                     url: t,
                                     router: this
                                 }), new Promise(() => {})
                             }
-                            if (q.isPreview = !!o.props.__N_PREVIEW, o.props.notFound === U) {
+                            if (W.isPreview = !!o.props.__N_PREVIEW, o.props.notFound === U) {
                                 let e;
                                 try {
                                     await this.fetchComponent("/404"), e = "/404"
                                 } catch (t) {
                                     e = "/_error"
                                 }
                                 if (o = await this.getRouteInfo({
@@ -2677,29 +2662,29 @@
                                         pathname: e,
                                         query: er,
                                         as: r,
                                         resolvedAs: en,
                                         routeProps: {
                                             shallow: !1
                                         },
-                                        locale: q.locale,
-                                        isPreview: q.isPreview,
+                                        locale: W.locale,
+                                        isPreview: W.isPreview,
                                         isNotFound: !0
                                     }), "type" in o) throw Error("Unexpected middleware effect on /404")
                             }
                         }
                         F && "/_error" === this.pathname && (null == (c = self.__NEXT_DATA__.props) ? void 0 : null == (f = c.pageProps) ? void 0 : f.statusCode) === 500 && (null == (j = o.props) ? void 0 : j.pageProps) && (o.props.pageProps.statusCode = 500);
-                        let s = n.shallow && q.route === (null != (O = o.route) ? O : ea),
+                        let s = n.shallow && W.route === (null != (O = o.route) ? O : ea),
                             d = null != (E = n.scroll) ? E : !F && !s,
                             y = null != a ? a : d ? {
                                 x: 0,
                                 y: 0
                             } : null,
                             _ = {
-                                ...q,
+                                ...W,
                                 route: ea,
                                 pathname: et,
                                 query: er,
                                 asPath: Q,
                                 isFallback: !1
                             };
                         if (F && es) {
@@ -2708,59 +2693,59 @@
                                     pathname: this.pathname,
                                     query: er,
                                     as: r,
                                     resolvedAs: en,
                                     routeProps: {
                                         shallow: !1
                                     },
-                                    locale: q.locale,
-                                    isPreview: q.isPreview,
+                                    locale: W.locale,
+                                    isPreview: W.isPreview,
                                     isQueryUpdating: F && !this.isFallback
                                 }), "type" in o) throw Error("Unexpected middleware effect on " + this.pathname);
-                            "/_error" === this.pathname && (null == (C = self.__NEXT_DATA__.props) ? void 0 : null == (A = C.pageProps) ? void 0 : A.statusCode) === 500 && (null == (I = o.props) ? void 0 : I.pageProps) && (o.props.pageProps.statusCode = 500);
+                            "/_error" === this.pathname && (null == (C = self.__NEXT_DATA__.props) ? void 0 : null == (A = C.pageProps) ? void 0 : A.statusCode) === 500 && (null == (T = o.props) ? void 0 : T.pageProps) && (o.props.pageProps.statusCode = 500);
                             try {
                                 await this.set(_, o, y)
                             } catch (e) {
-                                throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, J), e
+                                throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, K), e
                             }
                             return !0
                         }
-                        V.events.emit("beforeHistoryChange", r, J), this.changeState(e, t, r, n);
-                        let v = F && !y && !G && !Z && (0, R.compareRouterStates)(_, this.state);
+                        V.events.emit("beforeHistoryChange", r, K), this.changeState(e, t, r, n);
+                        let v = F && !y && !G && !Z && (0, x.compareRouterStates)(_, this.state);
                         if (!v) {
                             try {
                                 await this.set(_, o, y)
                             } catch (e) {
                                 if (e.cancelled) o.error = o.error || e;
                                 else throw e
                             }
-                            if (o.error) throw F || V.events.emit("routeChangeError", o.error, Q, J), o.error;
-                            F || V.events.emit("routeChangeComplete", r, J), d && /#.+$/.test(r) && this.scrollToHash(r)
+                            if (o.error) throw F || V.events.emit("routeChangeError", o.error, Q, K), o.error;
+                            F || V.events.emit("routeChangeComplete", r, K), d && /#.+$/.test(r) && this.scrollToHash(r)
                         }
                         return !0
                     } catch (e) {
                         if ((0, u.default)(e) && e.cancelled) return !1;
                         throw e
                     }
                 }
                 changeState(e, t, r, n) {
                     void 0 === n && (n = {}), ("pushState" !== e || (0, d.getURL)() !== r) && (this._shallow = n.shallow, window.history[e]({
                         url: t,
                         as: r,
                         options: n,
                         __N: !0,
-                        key: this._key = "pushState" !== e ? this._key : q()
+                        key: this._key = "pushState" !== e ? this._key : W()
                     }, "", r))
                 }
                 async handleRouteInfoError(e, t, r, n, a, o) {
                     if (console.error(e), e.cancelled) throw e;
                     if ((0, i.isAssetError)(e) || o) throw V.events.emit("routeChangeError", e, n, a), z({
                         url: n,
                         router: this
-                    }), T();
+                    }), I();
                     try {
                         let n;
                         let {
                             page: a,
                             styleSheets: o
                         } = await this.fetchComponent("/_error"), i = {
                             props: n,
@@ -2825,15 +2810,15 @@
                                 inflightCache: p ? this.sbc : this.sdc,
                                 persistCache: !d,
                                 isPrefetch: !1,
                                 unstable_skipClientCache: h,
                                 isBackground: p
                             },
                             E = p && !m ? null : await H({
-                                fetchData: () => W(O),
+                                fetchData: () => q(O),
                                 asPath: g ? "/404" : i,
                                 locale: s,
                                 router: this
                             }).catch(e => {
                                 if (p) return null;
                                 throw e
                             });
@@ -2851,71 +2836,71 @@
                                 route: _
                             }
                         }
                         if ((0, j.isAPIRoute)(_)) return z({
                             url: a,
                             router: this
                         }), new Promise(() => {});
-                        let R = u || await this.fetchComponent(_).then(e => ({
+                        let x = u || await this.fetchComponent(_).then(e => ({
                                 Component: e.page,
                                 styleSheets: e.styleSheets,
                                 __N_SSG: e.mod.__N_SSG,
                                 __N_SSP: e.mod.__N_SSP
                             })),
-                            x = null == E ? void 0 : null == (S = E.response) ? void 0 : S.headers.get("x-middleware-skip"),
-                            C = R.__N_SSG || R.__N_SSP;
-                        x && (null == E ? void 0 : E.dataHref) && delete this.sdc[E.dataHref];
+                            R = null == E ? void 0 : null == (S = E.response) ? void 0 : S.headers.get("x-middleware-skip"),
+                            C = x.__N_SSG || x.__N_SSP;
+                        R && (null == E ? void 0 : E.dataHref) && delete this.sdc[E.dataHref];
                         let {
                             props: M,
                             cacheKey: A
                         } = await this._getData(async () => {
                             if (C) {
-                                if ((null == E ? void 0 : E.json) && !x) return {
+                                if ((null == E ? void 0 : E.json) && !R) return {
                                     cacheKey: E.cacheKey,
                                     props: E.json
                                 };
                                 let e = (null == E ? void 0 : E.dataHref) ? E.dataHref : this.pageLoader.getDataHref({
                                         href: (0, y.formatWithValidation)({
                                             pathname: r,
                                             query: n
                                         }),
                                         asPath: i,
                                         locale: s
                                     }),
-                                    t = await W({
+                                    t = await q({
                                         dataHref: e,
                                         isServerRender: this.isSsr,
                                         parseJSON: !0,
-                                        inflightCache: x ? {} : this.sdc,
+                                        inflightCache: R ? {} : this.sdc,
                                         persistCache: !d,
                                         isPrefetch: !1,
                                         unstable_skipClientCache: h
                                     });
                                 return {
                                     cacheKey: t.cacheKey,
                                     props: t.json || {}
                                 }
                             }
                             return {
                                 headers: {},
-                                props: await this.getInitialProps(R.Component, {
+                                props: await this.getInitialProps(x.Component, {
                                     pathname: r,
                                     query: n,
                                     asPath: a,
                                     locale: s,
                                     locales: this.locales,
                                     defaultLocale: this.defaultLocale
                                 })
                             }
                         });
-                        return R.__N_SSP && O.dataHref && A && delete this.sdc[A], this.isPreview || !R.__N_SSG || p || W(Object.assign({}, O, {
+                        return x.__N_SSP && O.dataHref && A && delete this.sdc[A], this.isPreview || !x.__N_SSG || p || q(Object.assign({}, O, {
                             isBackground: !0,
                             persistCache: !1,
                             inflightCache: this.sbc
-                        })).catch(() => {}), M.pageProps = Object.assign({}, M.pageProps), R.props = M, R.route = _, R.query = n, R.resolvedAs = i, this.components[_] = R, R
+                        })).catch(() => {}), M.pageProps = Object.assign({}, M.pageProps), x.props = M, x.route = _, x.query = n, x.resolvedAs = i, this.components[_] = x, x
                     } catch (e) {
                         return this.handleRouteInfoError((0, u.getProperError)(e), r, n, a, l)
                     }
                 }
                 set(e, t, r) {
                     return this.state = e, this.sub(t, this.components["/_app"].Component, r)
                 }
@@ -2926,25 +2911,25 @@
                     if (!this.asPath) return !1;
                     let [t, r] = this.asPath.split("#"), [n, a] = e.split("#");
                     return !!a && t === n && r === a || t === n && r !== a
                 }
                 scrollToHash(e) {
                     let [, t = ""] = e.split("#");
                     if ("" === t || "top" === t) {
-                        (0, I.handleSmoothScroll)(() => window.scrollTo(0, 0));
+                        (0, T.handleSmoothScroll)(() => window.scrollTo(0, 0));
                         return
                     }
                     let r = decodeURIComponent(t),
                         n = document.getElementById(r);
                     if (n) {
-                        (0, I.handleSmoothScroll)(() => n.scrollIntoView());
+                        (0, T.handleSmoothScroll)(() => n.scrollIntoView());
                         return
                     }
                     let a = document.getElementsByName(r)[0];
-                    a && (0, I.handleSmoothScroll)(() => a.scrollIntoView())
+                    a && (0, T.handleSmoothScroll)(() => a.scrollIntoView())
                 }
                 urlIsNew(e) {
                     return this.asPath !== e
                 }
                 async prefetch(e, t, r) {
                     if (void 0 === t && (t = e), void 0 === r && (r = {}), (0, C.isBot)(window.navigator.userAgent)) return;
                     let n = (0, p.parseRelativeUrl)(e),
@@ -2960,15 +2945,15 @@
                         d = await N({
                             asPath: t,
                             locale: f,
                             router: this
                         });
                     n.pathname = B(n.pathname, s), (0, h.isDynamicRoute)(n.pathname) && (i = n.pathname, n.pathname = i, Object.assign(l, (0, m.getRouteMatcher)((0, g.getRouteRegex)(n.pathname))((0, _.parsePath)(t).pathname) || {}), d || (e = (0, y.formatWithValidation)(n)));
                     let b = await H({
-                        fetchData: () => W({
+                        fetchData: () => q({
                             dataHref: this.pageLoader.getDataHref({
                                 href: (0, y.formatWithValidation)({
                                     pathname: u,
                                     query: l
                                 }),
                                 skipInterpolation: !0,
                                 asPath: c,
@@ -2988,15 +2973,15 @@
                     if ((null == b ? void 0 : b.effect.type) === "rewrite" && (n.pathname = b.effect.resolvedHref, i = b.effect.resolvedHref, l = {
                             ...l,
                             ...b.effect.parsedAs.query
                         }, c = b.effect.parsedAs.pathname, e = (0, y.formatWithValidation)(n)), (null == b ? void 0 : b.effect.type) === "redirect-external") return;
                     let v = (0, o.removeTrailingSlash)(i);
                     await this._bfl(t, c, r.locale, !0) && (this.components[a] = {
                         __appRouter: !0
-                    }), await Promise.all([this.pageLoader._isSsg(v).then(t => !!t && W({
+                    }), await Promise.all([this.pageLoader._isSsg(v).then(t => !!t && q({
                         dataHref: (null == b ? void 0 : b.json) ? null == b ? void 0 : b.dataHref : this.pageLoader.getDataHref({
                             href: e,
                             asPath: c,
                             locale: f
                         }),
                         isServerRender: !1,
                         parseJSON: !0,
@@ -3028,15 +3013,15 @@
                             let e = Error("Loading initial props cancelled");
                             throw e.cancelled = !0, e
                         }
                         return e
                     })
                 }
                 _getFlightData(e) {
-                    return W({
+                    return q({
                         dataHref: e,
                         isServerRender: !0,
                         parseJSON: !1,
                         inflightCache: this.sdc,
                         persistCache: !1,
                         isPrefetch: !1
                     }).then(e => {
@@ -3091,15 +3076,15 @@
                     isFallback: m,
                     locale: g,
                     locales: _,
                     defaultLocale: b,
                     domainLocales: v,
                     isPreview: P
                 }) {
-                    this.sdc = {}, this.sbc = {}, this.isFirstPopStateEvent = !0, this._key = q(), this.onPopState = e => {
+                    this.sdc = {}, this.sbc = {}, this.isFirstPopStateEvent = !0, this._key = W(), this.onPopState = e => {
                         let t;
                         let {
                             isFirstPopStateEvent: r
                         } = this;
                         this.isFirstPopStateEvent = !1;
                         let n = e.state;
                         if (!n) {
@@ -3251,42 +3236,14 @@
                     pathname: r,
                     query: a,
                     hash: o
                 } = (0, n.parsePath)(e);
                 return "" + r + t + a + o
             }
         },
-        6097: function(e, t, r) {
-            "use strict";
-            Object.defineProperty(t, "__esModule", {
-                    value: !0
-                }),
-                function(e, t) {
-                    for (var r in t) Object.defineProperty(e, r, {
-                        enumerable: !0,
-                        get: t[r]
-                    })
-                }(t, {
-                    normalizeAppPath: function() {
-                        return a
-                    },
-                    normalizeRscPath: function() {
-                        return o
-                    }
-                });
-            let n = r(7302);
-
-            function a(e) {
-                return (0, n.ensureLeadingSlash)(e.split("/").reduce((e, t, r, n) => !t || "(" === t[0] && t.endsWith(")") || "@" === t[0] || ("page" === t || "route" === t) && r === n.length - 1 ? e : e + "/" + t, ""))
-            }
-
-            function o(e, t) {
-                return t ? e.replace(/\.rsc($|\?)/, "$1") : e
-            }
-        },
         6385: function(e, t) {
             "use strict";
 
             function r(e, t) {
                 let r = Object.keys(e);
                 if (r.length !== Object.keys(t).length) return !1;
                 for (let n = r.length; n--;) {
@@ -3753,16 +3710,17 @@
                 s = r(3162),
                 c = r(5036);
 
             function f(e, t, r) {
                 let f;
                 let d = "string" == typeof t ? t : (0, a.formatWithValidation)(t),
                     h = d.match(/^[a-zA-Z]{1,}:\/\//),
-                    p = h ? d.slice(h[0].length) : d;
-                if ((p.split("?")[0] || "").match(/(\/\/|\\)/)) {
+                    p = h ? d.slice(h[0].length) : d,
+                    m = p.split("?");
+                if ((m[0] || "").match(/(\/\/|\\)/)) {
                     console.error("Invalid href '" + d + "' passed to next/router in page: '" + e.pathname + "'. Repeated forward-slashes (//) or backslashes \\ are not valid in the href.");
                     let t = (0, i.normalizeRepeatedSlashes)(p);
                     d = (h ? h[0] : "") + t
                 }
                 if (!(0, u.isLocalURL)(d)) return r ? [d] : d;
                 try {
                     f = new URL(d.startsWith("#") ? e.asPath : e.pathname, "http://n")
@@ -3839,66 +3797,52 @@
                         get: t[r]
                     })
                 }(t, {
                     getRouteRegex: function() {
                         return u
                     },
                     getNamedRouteRegex: function() {
-                        return f
+                        return c
                     },
                     getNamedMiddlewareRegex: function() {
-                        return d
+                        return f
                     }
                 });
-            let n = r(2407),
-                a = r(5987),
-                o = r(7734);
+            let n = r(5987),
+                a = r(7734),
+                o = "nxtP";
 
             function i(e) {
                 let t = e.startsWith("[") && e.endsWith("]");
                 t && (e = e.slice(1, -1));
                 let r = e.startsWith("...");
                 return r && (e = e.slice(3)), {
                     key: e,
                     repeat: r,
                     optional: t
                 }
             }
 
             function l(e) {
-                let t = (0, o.removeTrailingSlash)(e).slice(1).split("/"),
+                let t = (0, a.removeTrailingSlash)(e).slice(1).split("/"),
                     r = {},
-                    l = 1;
+                    o = 1;
                 return {
                     parameterizedRoute: t.map(e => {
-                        let t = n.INTERCEPTION_ROUTE_MARKERS.find(t => e.startsWith(t)),
-                            o = e.match(/\[((?:\[.*\])|.+)\]/);
-                        if (t && o) {
+                        if (!(e.startsWith("[") && e.endsWith("]"))) return "/" + (0, n.escapeStringRegexp)(e); {
                             let {
-                                key: e,
+                                key: t,
                                 optional: n,
-                                repeat: u
-                            } = i(o[1]);
-                            return r[e] = {
-                                pos: l++,
-                                repeat: u,
-                                optional: n
-                            }, "/" + (0, a.escapeStringRegexp)(t) + "([^/]+?)"
-                        }
-                        if (!o) return "/" + (0, a.escapeStringRegexp)(e); {
-                            let {
-                                key: e,
-                                repeat: t,
-                                optional: n
-                            } = i(o[1]);
-                            return r[e] = {
-                                pos: l++,
-                                repeat: t,
+                                repeat: a
+                            } = i(e.slice(1, -1));
+                            return r[t] = {
+                                pos: o++,
+                                repeat: a,
                                 optional: n
-                            }, t ? n ? "(?:/(.+?))?" : "/(.+?)" : "/([^/]+?)"
+                            }, a ? n ? "(?:/(.+?))?" : "/(.+?)" : "/([^/]+?)"
                         }
                     }).join(""),
                     groups: r
                 }
             }
 
             function u(e) {
@@ -3908,78 +3852,61 @@
                 } = l(e);
                 return {
                     re: RegExp("^" + t + "(?:/)?$"),
                     groups: r
                 }
             }
 
-            function s(e) {
-                let t, r, {
-                        segment: n,
-                        routeKeys: a,
-                        keyPrefix: o
-                    } = e,
-                    l = (t = 97, r = 1, () => {
+            function s(e, t) {
+                let r, l;
+                let u = (0, a.removeTrailingSlash)(e).slice(1).split("/"),
+                    s = (r = 97, l = 1, () => {
                         let e = "";
-                        for (let n = 0; n < r; n++) e += String.fromCharCode(t), ++t > 122 && (r++, t = 97);
+                        for (let t = 0; t < l; t++) e += String.fromCharCode(r), ++r > 122 && (l++, r = 97);
                         return e
                     }),
-                    {
-                        key: u,
-                        optional: s,
-                        repeat: c
-                    } = i(n),
-                    f = u.replace(/\W/g, "");
-                o && (f = "" + o + f);
-                let d = !1;
-                return (0 === f.length || f.length > 30) && (d = !0), isNaN(parseInt(f.slice(0, 1))) || (d = !0), d && (f = l()), o ? a[f] = "" + o + u : a[f] = "" + u, c ? s ? "(?:/(?<" + f + ">.+?))?" : "/(?<" + f + ">.+?)" : "/(?<" + f + ">[^/]+?)"
-            }
-
-            function c(e, t) {
-                let r = (0, o.removeTrailingSlash)(e).slice(1).split("/"),
-                    i = {};
+                    c = {};
                 return {
-                    namedParameterizedRoute: r.map(e => {
-                        let r = n.INTERCEPTION_ROUTE_MARKERS.some(t => e.startsWith(t)),
-                            o = e.match(/\[((?:\[.*\])|.+)\]/);
-                        return r && o ? s({
-                            segment: o[1],
-                            routeKeys: i,
-                            keyPrefix: t ? "nxtI" : void 0
-                        }) : o ? s({
-                            segment: o[1],
-                            routeKeys: i,
-                            keyPrefix: t ? "nxtP" : void 0
-                        }) : "/" + (0, a.escapeStringRegexp)(e)
+                    namedParameterizedRoute: u.map(e => {
+                        if (!(e.startsWith("[") && e.endsWith("]"))) return "/" + (0, n.escapeStringRegexp)(e); {
+                            let {
+                                key: r,
+                                optional: n,
+                                repeat: a
+                            } = i(e.slice(1, -1)), l = r.replace(/\W/g, "");
+                            t && (l = "" + o + l);
+                            let u = !1;
+                            return (0 === l.length || l.length > 30) && (u = !0), isNaN(parseInt(l.slice(0, 1))) || (u = !0), u && (l = s()), t ? c[l] = "" + o + r : c[l] = "" + r, a ? n ? "(?:/(?<" + l + ">.+?))?" : "/(?<" + l + ">.+?)" : "/(?<" + l + ">[^/]+?)"
+                        }
                     }).join(""),
-                    routeKeys: i
+                    routeKeys: c
                 }
             }
 
-            function f(e, t) {
-                let r = c(e, t);
+            function c(e, t) {
+                let r = s(e, t);
                 return {
                     ...u(e),
                     namedRegex: "^" + r.namedParameterizedRoute + "(?:/)?$",
                     routeKeys: r.routeKeys
                 }
             }
 
-            function d(e, t) {
+            function f(e, t) {
                 let {
                     parameterizedRoute: r
                 } = l(e), {
                     catchAll: n = !0
                 } = t;
                 if ("/" === r) return {
                     namedRegex: "^/" + (n ? ".*" : "") + "$"
                 };
                 let {
                     namedParameterizedRoute: a
-                } = c(e, !1);
+                } = s(e, !1);
                 return {
                     namedRegex: "^" + a + (n ? "(?:(/.*)?)" : "") + "$"
                 }
             }
         },
         9163: function(e, t) {
             "use strict";
@@ -4176,17 +4103,14 @@
                         return g
                     },
                     MissingStaticPage: function() {
                         return y
                     },
                     MiddlewareNotFoundError: function() {
                         return _
-                    },
-                    stringifyError: function() {
-                        return b
                     }
                 });
             let r = ["CLS", "FCP", "FID", "INP", "LCP", "TTFB"];
 
             function n(e) {
                 let t, r = !1;
                 return function() {
@@ -4254,36 +4178,29 @@
                 }
             }
             class _ extends Error {
                 constructor() {
                     super(), this.code = "ENOENT", this.message = "Cannot find the middleware module"
                 }
             }
-
-            function b(e) {
-                return JSON.stringify({
-                    message: e.message,
-                    stack: e.stack
-                })
-            }
         },
         4210: function(e, t) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), Object.defineProperty(t, "warnOnce", {
                 enumerable: !0,
                 get: function() {
                     return r
                 }
             });
             let r = e => {}
         },
         8018: function(e) {
-            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, S, j, O, E, R, x, C, M, A, L, I, T, N, k, D, B, H, U, F, W, q, z, G, V;
+            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, S, j, O, E, x, R, C, M, A, L, T, I, N, k, D, B, H, U, F, q, W, z, G, V;
             (t = {}).d = function(e, r) {
                 for (var n in r) t.o(r, n) && !t.o(e, n) && Object.defineProperty(e, n, {
                     enumerable: !0,
                     get: r[n]
                 })
             }, t.o = function(e, t) {
                 return Object.prototype.hasOwnProperty.call(e, t)
@@ -4300,15 +4217,15 @@
                 getFCP: function() {
                     return v
                 },
                 getFID: function() {
                     return M
                 },
                 getINP: function() {
-                    return W
+                    return q
                 },
                 getLCP: function() {
                     return z
                 },
                 getTTFB: function() {
                     return V
                 },
@@ -4318,15 +4235,15 @@
                 onFCP: function() {
                     return v
                 },
                 onFID: function() {
                     return M
                 },
                 onINP: function() {
-                    return W
+                    return q
                 },
                 onLCP: function() {
                     return z
                 },
                 onTTFB: function() {
                     return V
                 }
@@ -4436,43 +4353,43 @@
                 }), s(function() {
                     i = 0, w = -1, n = m(a, o = d("CLS", 0), r, t.reportAllChanges)
                 }))
             }, j = {
                 passive: !0,
                 capture: !0
             }, O = new Date, E = function(e, t) {
-                n || (n = t, a = e, o = new Date, C(removeEventListener), R())
-            }, R = function() {
+                n || (n = t, a = e, o = new Date, C(removeEventListener), x())
+            }, x = function() {
                 if (a >= 0 && a < o - O) {
                     var e = {
                         entryType: "first-input",
                         name: n.type,
                         target: n.target,
                         cancelable: n.cancelable,
                         startTime: n.timeStamp,
                         processingStart: n.timeStamp + a
                     };
                     i.forEach(function(t) {
                         t(e)
                     }), i = []
                 }
-            }, x = function(e) {
+            }, R = function(e) {
                 if (e.cancelable) {
                     var t, r, n, a = (e.timeStamp > 1e12 ? new Date : performance.now()) - e.timeStamp;
                     "pointerdown" == e.type ? (t = function() {
                         E(a, e), n()
                     }, r = function() {
                         n()
                     }, n = function() {
                         removeEventListener("pointerup", t, j), removeEventListener("pointercancel", r, j)
                     }, addEventListener("pointerup", t, j), addEventListener("pointercancel", r, j)) : E(a, e)
                 }
             }, C = function(e) {
                 ["mousedown", "keydown", "touchstart", "pointerdown"].forEach(function(t) {
-                    return e(t, x, j)
+                    return e(t, R, j)
                 })
             }, M = function(e, t) {
                 t = t || {};
                 var r, o = [100, 300],
                     l = b(),
                     u = d("FID"),
                     c = function(e) {
@@ -4481,24 +4398,24 @@
                     f = function(e) {
                         e.forEach(c)
                     },
                     g = h("first-input", f);
                 r = m(e, u, o, t.reportAllChanges), g && p(function() {
                     f(g.takeRecords()), g.disconnect()
                 }, !0), g && s(function() {
-                    r = m(e, u = d("FID"), o, t.reportAllChanges), i = [], a = -1, n = null, C(addEventListener), i.push(c), R()
+                    r = m(e, u = d("FID"), o, t.reportAllChanges), i = [], a = -1, n = null, C(addEventListener), i.push(c), x()
                 })
-            }, A = 0, L = 1 / 0, I = 0, T = function(e) {
+            }, A = 0, L = 1 / 0, T = 0, I = function(e) {
                 e.forEach(function(e) {
-                    e.interactionId && (L = Math.min(L, e.interactionId), A = (I = Math.max(I, e.interactionId)) ? (I - L) / 7 + 1 : 0)
+                    e.interactionId && (L = Math.min(L, e.interactionId), A = (T = Math.max(T, e.interactionId)) ? (T - L) / 7 + 1 : 0)
                 })
             }, N = function() {
                 return l ? A : performance.interactionCount || 0
             }, k = function() {
-                "interactionCount" in performance || l || (l = h("event", T, {
+                "interactionCount" in performance || l || (l = h("event", I, {
                     type: "event",
                     buffered: !0,
                     durationThreshold: 0
                 }))
             }, D = 0, B = function() {
                 return N() - D
             }, H = [], U = {}, F = function(e) {
@@ -4516,15 +4433,15 @@
                     }
                     H.sort(function(e, t) {
                         return t.latency - e.latency
                     }), H.splice(10).forEach(function(e) {
                         delete U[e.id]
                     })
                 }
-            }, W = function(e, t) {
+            }, q = function(e, t) {
                 t = t || {};
                 var r = [200, 500];
                 k();
                 var n, a = d("INP"),
                     o = function(e) {
                         e.forEach(function(e) {
                             e.interactionId && F(e), "first-input" !== e.entryType || H.some(function(t) {
@@ -4543,15 +4460,15 @@
                     type: "first-input",
                     buffered: !0
                 }), p(function() {
                     o(i.takeRecords()), a.value < 0 && B() > 0 && (a.value = 0, a.entries = []), n(!0)
                 }), s(function() {
                     H = [], D = N(), n = m(e, a = d("INP"), r, t.reportAllChanges)
                 }))
-            }, q = {}, z = function(e, t) {
+            }, W = {}, z = function(e, t) {
                 t = t || {};
                 var r, n = [2500, 4e3],
                     a = b(),
                     o = d("LCP"),
                     i = function(e) {
                         var t = e[e.length - 1];
                         if (t) {
@@ -4559,25 +4476,25 @@
                             n < a.firstHiddenTime && (o.value = n, o.entries = [t], r())
                         }
                     },
                     l = h("largest-contentful-paint", i);
                 if (l) {
                     r = m(e, o, n, t.reportAllChanges);
                     var u = function() {
-                        q[o.id] || (i(l.takeRecords()), l.disconnect(), q[o.id] = !0, r(!0))
+                        W[o.id] || (i(l.takeRecords()), l.disconnect(), W[o.id] = !0, r(!0))
                     };
                     ["keydown", "click"].forEach(function(e) {
                         addEventListener(e, u, {
                             once: !0,
                             capture: !0
                         })
                     }), p(u, !0), s(function(a) {
                         r = m(e, o = d("LCP"), n, t.reportAllChanges), requestAnimationFrame(function() {
                             requestAnimationFrame(function() {
-                                o.value = performance.now() - a.timeStamp, q[o.id] = !0, r(!0)
+                                o.value = performance.now() - a.timeStamp, W[o.id] = !0, r(!0)
                             })
                         })
                     })
                 }
             }, G = function e(t) {
                 document.prerendering ? addEventListener("prerenderingchange", function() {
                     return e(t)
@@ -4639,74 +4556,14 @@
                 return "object" == typeof e && null !== e && "name" in e && "message" in e
             }
 
             function o(e) {
                 return a(e) ? e : Error((0, n.isPlainObject)(e) ? JSON.stringify(e) : e + "")
             }
         },
-        2407: function(e, t, r) {
-            "use strict";
-            Object.defineProperty(t, "__esModule", {
-                    value: !0
-                }),
-                function(e, t) {
-                    for (var r in t) Object.defineProperty(e, r, {
-                        enumerable: !0,
-                        get: t[r]
-                    })
-                }(t, {
-                    INTERCEPTION_ROUTE_MARKERS: function() {
-                        return a
-                    },
-                    isInterceptionRouteAppPath: function() {
-                        return o
-                    },
-                    extractInterceptionRouteInformation: function() {
-                        return i
-                    }
-                });
-            let n = r(6097),
-                a = ["(..)(..)", "(.)", "(..)", "(...)"];
-
-            function o(e) {
-                return void 0 !== e.split("/").find(e => a.find(t => e.startsWith(t)))
-            }
-
-            function i(e) {
-                let t, r, o;
-                for (let n of e.split("/"))
-                    if (r = a.find(e => n.startsWith(e))) {
-                        [t, o] = e.split(r, 2);
-                        break
-                    } if (!t || !r || !o) throw Error(`Invalid interception route: ${e}. Must be in the format /<intercepting route>/(..|...|..)(..)/<intercepted route>`);
-                switch (t = (0, n.normalizeAppPath)(t), r) {
-                    case "(.)":
-                        o = "/" === t ? `/${o}` : t + "/" + o;
-                        break;
-                    case "(..)":
-                        if ("/" === t) throw Error(`Invalid interception route: ${e}. Cannot use (..) marker at the root level, use (.) instead.`);
-                        o = t.split("/").slice(0, -1).concat(o).join("/");
-                        break;
-                    case "(...)":
-                        o = "/" + o;
-                        break;
-                    case "(..)(..)":
-                        let i = t.split("/");
-                        if (i.length <= 2) throw Error(`Invalid interception route: ${e}. Cannot use (..)(..) marker at the root level or one level up.`);
-                        o = i.slice(0, -2).concat(o).join("/");
-                        break;
-                    default:
-                        throw Error("Invariant: unexpected marker")
-                }
-                return {
-                    interceptingRoute: t,
-                    interceptedRoute: o
-                }
-            }
-        },
         2431: function() {},
         8754: function(e, t, r) {
             "use strict";
 
             function n(e) {
                 return e && e.__esModule ? e : {
                     default: e
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2831,15 +2831,18 @@
                         theme: r
                     } = e, n = p(), a = i.useMemo(() => {
                         let e = null === n ? r : function(e, t) {
                             if ("function" == typeof t) {
                                 let r = t(e);
                                 return r
                             }
-                            return (0, l.Z)({}, e, t)
+                            return {
+                                ...e,
+                                ...t
+                            }
                         }(n, r);
                         return null != e && (e[m] = null !== n), e
                     }, [r, n]);
                     return (0, o.jsx)(f.Provider, {
                         value: a,
                         children: t
                     })
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-6924375f59017114.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -164,15 +164,15 @@
                 r = n(7294),
                 a = n(1163),
                 s = n(2734),
                 o = n(5582),
                 l = n(6886),
                 c = n(8456),
                 d = n(5861),
-                u = n(9713),
+                u = n(3913),
                 p = n(699),
                 h = n(3321),
                 x = n(6154),
                 m = n(8103),
                 y = function() {
                     let e = (0, a.useRouter)().query,
                         [t, n] = (0, r.useState)(),
@@ -283,12 +283,12 @@
                         noHeader: !0,
                         children: (0, i.jsx)(y, {})
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 134, 839, 498, 699, 154, 713, 774, 888, 179], function() {
+        e.O(0, [702, 134, 418, 498, 699, 154, 913, 774, 888, 179], function() {
             return e(e.s = 1328)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-0fcd948dd1ceee0b.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -436,12 +436,12 @@
                         noHeader: !0,
                         children: (0, n.jsx)(P, {})
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 134, 839, 498, 699, 154, 767, 774, 888, 179], function() {
+        e.O(0, [702, 134, 418, 498, 699, 154, 767, 774, 888, 179], function() {
             return e(e.s = 8573)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/data-bf9ec2c59e015b44.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -224,51 +224,50 @@
                 }
             }
         },
         6351: function(e, t, s) {
             "use strict";
             s.r(t), s.d(t, {
                 default: function() {
-                    return E
+                    return P
                 }
             });
             var n = s(5893),
                 i = s(7294),
                 o = s(5582),
                 a = s(1163),
                 r = s(2734),
                 c = s(6886),
                 l = s(1703),
                 d = s(44),
                 h = s(8456),
-                u = s(361),
-                p = s.n(u),
-                y = s(6018),
-                m = s(5152),
-                g = s.n(m),
-                w = s(4267),
-                b = s(5861);
-            let k = g()(() => s.e(171).then(s.t.bind(s, 5171, 23)), {
+                u = s(6486),
+                p = s(6018),
+                y = s(5152),
+                m = s.n(y),
+                g = s(4267),
+                w = s(5861);
+            let b = m()(() => s.e(171).then(s.t.bind(s, 5171, 23)), {
                 loadableGenerated: {
                     webpack: () => [5171]
                 },
                 ssr: !1
             });
-            var x = function(e) {
+            var k = function(e) {
                 let {
                     name: t,
                     data: s
                 } = e;
-                return (0, n.jsxs)(w.Z, {
-                    children: [(0, n.jsx)(b.Z, {
+                return (0, n.jsxs)(g.Z, {
+                    children: [(0, n.jsx)(w.Z, {
                         gutterBottom: !0,
                         variant: "h4",
                         component: "h3",
                         children: t
-                    }), s ? (0, n.jsx)(k, {
+                    }), s ? (0, n.jsx)(b, {
                         src: s,
                         displayDataTypes: !1,
                         displayObjectSize: !0,
                         enableClipboard: !0,
                         iconStyle: "triangle",
                         name: null,
                         collapseStringsAfterLength: 140,
@@ -281,121 +280,121 @@
                         container: !0,
                         direction: "row",
                         justifyContent: "center",
                         children: (0, n.jsx)(h.Z, {})
                     })]
                 })
             };
-            let f = ["battery", "cpu", "disk", "display", "gpu", "media", "memory", "network", "sensors", "system"],
-                S = {
+            let x = ["battery", "cpu", "disk", "display", "gpu", "media", "memory", "network", "sensors", "system"],
+                f = {
                     battery: "Battery",
                     cpu: "CPU",
                     disk: "Disk",
                     display: "Display",
                     gpu: "GPU",
                     media: "Media",
                     memory: "Memory",
                     network: "Network",
                     sensors: "Sensors",
                     system: "System"
                 },
-                j = {
+                S = {
                     battery: {},
                     cpu: {},
                     disk: {},
                     media: {},
                     memory: {},
                     network: {},
                     sensors: {},
                     system: {}
                 };
-            var v = function() {
-                    let [e, t] = (0, i.useState)(j), [s, o] = (0, i.useState)(!1), [u, m] = (0, i.useState)(0), g = (0, a.useRouter)().query, w = (0, i.useCallback)(e => {
+            var j = function() {
+                    let [e, t] = (0, i.useState)(S), [s, o] = (0, i.useState)(!1), [y, m] = (0, i.useState)(0), g = (0, a.useRouter)().query, w = (0, i.useCallback)(e => {
                         console.log("Event:", e), "DATA_UPDATE" === e.type && (console.log("Data update:", e.module, e.data), t(t => {
-                            let s = p()(t);
+                            let s = (0, u.cloneDeep)(t);
                             return "string" == typeof e.module && (s[e.module] = e.data), s
                         }))
                     }, []), b = (0, i.useCallback)((e, t) => {
                         console.log("Setup WebSocketConnection");
-                        let s = new y.C(e, t, async () => {
-                            s.getData(f), s.registerDataListener(f)
+                        let s = new p.C(e, t, async () => {
+                            s.getData(x), s.registerDataListener(x)
                         });
                         s.onEvent = w
                     }, [w]);
                     (0, i.useEffect)(() => {
                         !s && g && g.apiKey && (o(!0), b(Number(g.apiPort) || 9170, String(g.apiKey)))
                     }, [s, b, g]);
-                    let k = (0, r.Z)();
+                    let j = (0, r.Z)();
                     return (0, n.jsx)(n.Fragment, {
                         children: (0, n.jsx)(c.ZP, {
                             container: !0,
                             direction: "column",
                             spacing: 2,
                             alignItems: "stretch",
                             sx: {
-                                padding: k.spacing(2)
+                                padding: j.spacing(2)
                             },
                             children: (0, n.jsxs)(c.ZP, {
                                 container: !0,
                                 direction: "row",
                                 item: !0,
                                 xs: !0,
                                 children: [(0, n.jsx)(c.ZP, {
                                     item: !0,
                                     children: (0, n.jsx)(l.Z, {
                                         orientation: "vertical",
                                         variant: "scrollable",
-                                        value: u,
+                                        value: y,
                                         onChange: (e, t) => {
                                             m(t)
                                         },
-                                        children: f.map((e, t) => (0, n.jsx)(d.Z, {
-                                            label: S[e],
+                                        children: x.map((e, t) => (0, n.jsx)(d.Z, {
+                                            label: f[e],
                                             id: "scrollable-auto-tab-".concat(t),
                                             "aria-controls": "scrollable-auto-tabpanel-".concat(t)
                                         }, t))
                                     })
                                 }), (0, n.jsx)(c.ZP, {
                                     item: !0,
                                     xs: !0,
-                                    children: f.map((t, s) => (0, n.jsx)(i.Fragment, {
-                                        children: u === s ? (0, n.jsx)(n.Fragment, {
-                                            children: e[t] ? (0, n.jsx)(x, {
+                                    children: x.map((t, s) => (0, n.jsx)(i.Fragment, {
+                                        children: y === s ? (0, n.jsx)(n.Fragment, {
+                                            children: e[t] ? (0, n.jsx)(k, {
                                                 data: e[t],
-                                                name: S[t]
+                                                name: f[t]
                                             }) : (0, n.jsx)(c.ZP, {
                                                 container: !0,
                                                 direction: "row",
                                                 justifyContent: "center",
                                                 sx: {
-                                                    margin: k.spacing(8, 0, 14)
+                                                    margin: j.spacing(8, 0, 14)
                                                 },
                                                 children: (0, n.jsx)(h.Z, {})
                                             })
                                         }) : ""
                                     }, s))
                                 })]
                             })
                         })
                     })
                 },
-                P = s(8980),
-                E = function() {
-                    return (0, n.jsx)(P.Z, {
+                v = s(8980),
+                P = function() {
+                    return (0, n.jsx)(v.Z, {
                         title: "Data",
                         url: "https://system-bridge.timmo.dev",
                         description: "Frontend for System Bridge",
                         children: (0, n.jsx)(o.Z, {
                             component: "article",
                             maxWidth: "xl",
-                            children: (0, n.jsx)(v, {})
+                            children: (0, n.jsx)(j, {})
                         })
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 134, 498, 361, 731, 774, 888, 179], function() {
+        e.O(0, [702, 662, 134, 498, 731, 774, 888, 179], function() {
             return e(e.s = 8792)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/notification-b76a6b7af2e3a0c9.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [723], {
-        8973: function(e, t, n) {
+        4239: function(e, t, n) {
             (window.__NEXT_P = window.__NEXT_P || []).push(["/app/notification", function() {
                 return n(154)
             }])
         },
         8980: function(e, t, n) {
             "use strict";
             n.d(t, {
@@ -230,15 +230,15 @@
                                 r[e] = i
                             }
                         }), n = (0, d.Z)(n, (0, x.k9)({
                             theme: t
                         }, a, (t, n) => e.useFlexGap ? {
                             gap: (0, y.NA)(i, t)
                         } : {
-                            "& > :not(style) ~ :not(style)": {
+                            "& > :not(style) + :not(style)": {
                                 margin: 0,
                                 [`margin${k(n?r[n]:e.direction)}`]: (0, y.NA)(i, t)
                             }
                         }))
                     }
                     return (0, x.dt)(t.breakpoints, n)
                 };
@@ -508,11 +508,11 @@
                         })
                     })
                 }
         }
     },
     function(e) {
         e.O(0, [702, 134, 154, 774, 888, 179], function() {
-            return e(e.s = 8973)
+            return e(e.s = 4239)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-377fb73a175a7afa.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -26,12 +26,12 @@
                         })
                     })
                 })
             }
         }
     },
     function(e) {
-        e.O(0, [702, 885, 134, 839, 361, 514, 142, 774, 888, 179], function() {
+        e.O(0, [702, 662, 885, 134, 418, 633, 142, 774, 888, 179], function() {
             return e(e.s = 2134)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-dd8ee3c5bcd7fd5a.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -26,12 +26,12 @@
                         })
                     })
                 })
             }
         }
     },
     function(e) {
-        e.O(0, [702, 885, 134, 839, 361, 514, 142, 774, 888, 179], function() {
+        e.O(0, [702, 662, 885, 134, 418, 633, 142, 774, 888, 179], function() {
             return e(e.s = 3049)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/app/settings-734d9ba521512578.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -277,15 +277,15 @@
                 f = i(9953),
                 v = i(3395),
                 k = i(9653),
                 b = i(4054),
                 Z = i(7709),
                 w = i(7109),
                 S = i(3946),
-                P = i(9713),
+                P = i(3913),
                 C = i(699),
                 E = i(8849),
                 I = i(8995),
                 N = i(8396),
                 _ = i(657),
                 A = i(7645),
                 O = i(8951),
@@ -788,12 +788,12 @@
                             children: (0, s.jsx)(H, {})
                         })
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 662, 134, 839, 498, 699, 713, 767, 826, 774, 888, 179], function() {
+        e.O(0, [702, 662, 134, 418, 498, 699, 913, 767, 826, 774, 888, 179], function() {
             return e(e.s = 4768)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/bridges/openon.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/openon.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/839-49c1e145187c690b.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-e1dda1328195ce40.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/713-307f96321a681e2c.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-6924375f59017114.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/913-948b3bc7b49750f4.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/bridges/setup.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/setup.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/839-49c1e145187c690b.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-e1dda1328195ce40.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/767-13c0b6c8b2e638dd.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-0fcd948dd1ceee0b.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/767-b6df483a2f96f15d.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/data.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/data.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/731-adbd7bf9e28fe493.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-bf9ec2c59e015b44.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/731-eb947eaba8f94f26.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/notification.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/notification.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-b76a6b7af2e3a0c9.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/player/audio.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/audio.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/839-49c1e145187c690b.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-a199f049b736895b.js" defer=""></script><script src="/_next/static/chunks/142-e96944db890d0712.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-377fb73a175a7afa.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/633-a2b446f38d34df6a.js" defer=""></script><script src="/_next/static/chunks/142-b511304dc754f6ca.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/player/video.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/video.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/839-49c1e145187c690b.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-a199f049b736895b.js" defer=""></script><script src="/_next/static/chunks/142-e96944db890d0712.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-dd8ee3c5bcd7fd5a.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/633-a2b446f38d34df6a.js" defer=""></script><script src="/_next/static/chunks/142-b511304dc754f6ca.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/app/settings.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/settings.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-809b6f0b05884bf7.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/839-49c1e145187c690b.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-e1dda1328195ce40.js" defer=""></script><script src="/_next/static/chunks/713-307f96321a681e2c.js" defer=""></script><script src="/_next/static/chunks/767-13c0b6c8b2e638dd.js" defer=""></script><script src="/_next/static/chunks/826-e44464776abed9eb.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-734d9ba521512578.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/913-948b3bc7b49750f4.js" defer=""></script><script src="/_next/static/chunks/767-b6df483a2f96f15d.js" defer=""></script><script src="/_next/static/chunks/826-e44464776abed9eb.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/favicon.svg` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/favicon.svg`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend/out/index.html` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-bfbd70c9b9a5a25b.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js" defer=""></script><script src="/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"MLmAr5WUt_Z2jZX98r6Z_","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0/systembridgefrontend.egg-info/SOURCES.txt` & `systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 systembridgefrontend.egg-info/PKG-INFO
 systembridgefrontend.egg-info/SOURCES.txt
 systembridgefrontend.egg-info/dependency_links.txt
 systembridgefrontend.egg-info/top_level.txt
 systembridgefrontend/out/404.html
 systembridgefrontend/out/favicon.svg
 systembridgefrontend/out/index.html
-systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_buildManifest.js
-systembridgefrontend/out/_next/static/MLmAr5WUt_Z2jZX98r6Z_/_ssgManifest.js
+systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js
+systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js
 systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js
-systembridgefrontend/out/_next/static/chunks/142-e96944db890d0712.js
+systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js
 systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js
 systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js
-systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
-systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
+systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js
+systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js
 systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js
-systembridgefrontend/out/_next/static/chunks/514-a199f049b736895b.js
-systembridgefrontend/out/_next/static/chunks/699-e1dda1328195ce40.js
-systembridgefrontend/out/_next/static/chunks/713-307f96321a681e2c.js
-systembridgefrontend/out/_next/static/chunks/731-adbd7bf9e28fe493.js
+systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js
+systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js
+systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js
 systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js
-systembridgefrontend/out/_next/static/chunks/767-13c0b6c8b2e638dd.js
+systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js
 systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js
-systembridgefrontend/out/_next/static/chunks/839-49c1e145187c690b.js
+systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js
 systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
 systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js
-systembridgefrontend/out/_next/static/chunks/main-bfbd70c9b9a5a25b.js
+systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js
 systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
@@ -40,24 +39,24 @@
 systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
 systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js
-systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
+systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js
 systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
-systembridgefrontend/out/_next/static/chunks/pages/app/data-bf9ec2c59e015b44.js
-systembridgefrontend/out/_next/static/chunks/pages/app/notification-b76a6b7af2e3a0c9.js
-systembridgefrontend/out/_next/static/chunks/pages/app/settings-734d9ba521512578.js
-systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-6924375f59017114.js
-systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-0fcd948dd1ceee0b.js
-systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-377fb73a175a7afa.js
-systembridgefrontend/out/_next/static/chunks/pages/app/player/video-dd8ee3c5bcd7fd5a.js
+systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js
+systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js
+systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js
+systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js
+systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js
+systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js
+systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js
 systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
```

