# Comparing `tmp/gemini_self_protector-0.1.1.tar.gz` & `tmp/gemini_self_protector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_self_protector-0.1.1.tar", max compression
+gzip compressed data, was "gemini_self_protector-0.1.2.tar", max compression
```

## Comparing `gemini_self_protector-0.1.1.tar` & `gemini_self_protector-0.1.2.tar`

### file list

```diff
@@ -1,131 +1,133 @@
--rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.1/LICENSE
--rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.1/README.md
--rw-r--r--   0        0        0      473 2023-06-24 06:45:00.301040 gemini_self_protector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.1/src/gemini_self_protector/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.1/src/gemini_self_protector/_audit.py
--rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.1/src/gemini_self_protector/_cli.py
--rw-r--r--   0        0        0    11523 2023-06-24 06:36:42.962571 gemini_self_protector-0.1.1/src/gemini_self_protector/_config.py
--rw-r--r--   0        0        0    20405 2023-06-24 06:36:22.865320 gemini_self_protector-0.1.1/src/gemini_self_protector/_gemini.py
--rw-r--r--   0        0        0    31306 2023-06-24 06:35:49.887327 gemini_self_protector-0.1.1/src/gemini_self_protector/_gui.py
--rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.1/src/gemini_self_protector/_logger.py
--rw-r--r--   0        0        0     3240 2023-06-24 06:35:37.294824 gemini_self_protector-0.1.1/src/gemini_self_protector/_model.py
--rw-r--r--   0        0        0    14692 2023-06-24 06:35:20.927744 gemini_self_protector-0.1.1/src/gemini_self_protector/_protect.py
--rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.1/src/gemini_self_protector/_template.py
--rw-r--r--   0        0        0    17196 2023-06-24 06:34:52.531115 gemini_self_protector-0.1.1/src/gemini_self_protector/_utils.py
--rw-r--r--   0        0        0     6391 2023-06-24 06:34:27.727893 gemini_self_protector-0.1.1/src/gemini_self_protector/gemini_self_protector.py
--rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/dark.css
--rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/install.css
--rw-r--r--   0        0        0   311857 2023-06-24 06:37:46.977525 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/style.css
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
--rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
--rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
--rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
--rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
--rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
--rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
--rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
--rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
--rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
--rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/chrome.png
--rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/firefox.png
--rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/ie.png
--rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/opera.png
--rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/safari.png
--rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/favicon.ico
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/gemini-7.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo-dark.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo-thumb.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo.png
--rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
--rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
--rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
--rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
--rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
--rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
--rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
--rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
--rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
--rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
--rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
--rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
--rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
--rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
--rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/profile.jpg
--rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/user-1.png
--rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/user-2.png
--rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/box.png
--rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
--rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
--rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
--rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
--rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
--rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
--rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
--rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/dark-mode.js
--rw-r--r--   0        0        0     9948 2023-06-19 17:02:55.247014 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/install.js
--rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
--rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
--rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pcoded.min.js
--rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
--rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
--rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
--rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
--rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
--rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
--rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
--rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
--rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
--rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
--rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
--rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
--rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
--rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
--rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
--rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
--rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
--rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
--rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
--rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
--rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
--rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
--rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
--rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
--rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/scss/dark.scss
--rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/accounts/login.html
--rw-r--r--   0        0        0    11196 2023-06-22 17:50:33.882578 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/acl.html
--rw-r--r--   0        0        0    19310 2023-06-24 06:37:19.450233 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/config.html
--rw-r--r--   0        0        0     7827 2023-06-19 17:02:55.285356 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/dependency.html
--rw-r--r--   0        0        0    27512 2023-06-26 15:14:17.209691 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/index.html
--rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-403.html
--rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-404.html
--rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-500.html
--rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-blank.html
--rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/profile.html
--rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/navigation.html
--rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/scripts.html
--rw-r--r--   0        0        0     4505 2023-06-21 15:00:19.355909 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/sidebar.html
--rw-r--r--   0        0        0    15450 2023-06-19 17:02:55.293138 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/install.html
--rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
--rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/layouts/base.html
--rw-r--r--   0        0        0     1770 2023-06-19 17:02:55.294701 gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/license.html
--rw-r--r--   0        0        0     7416 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.2/README.md
+-rw-r--r--   0        0        0      489 2023-07-12 15:08:56.794162 gemini_self_protector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.2/src/gemini_self_protector/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.2/src/gemini_self_protector/_audit.py
+-rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.2/src/gemini_self_protector/_cli.py
+-rw-r--r--   0        0        0    13840 2023-07-04 17:18:00.743973 gemini_self_protector-0.1.2/src/gemini_self_protector/_config.py
+-rw-r--r--   0        0        0    20786 2023-07-12 14:31:35.889747 gemini_self_protector-0.1.2/src/gemini_self_protector/_gemini.py
+-rw-r--r--   0        0        0    35678 2023-07-12 14:30:47.625077 gemini_self_protector-0.1.2/src/gemini_self_protector/_gui.py
+-rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.2/src/gemini_self_protector/_logger.py
+-rw-r--r--   0        0        0     3508 2023-07-12 14:32:01.923270 gemini_self_protector-0.1.2/src/gemini_self_protector/_model.py
+-rw-r--r--   0        0        0    14724 2023-07-03 17:28:57.174109 gemini_self_protector-0.1.2/src/gemini_self_protector/_protect.py
+-rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.2/src/gemini_self_protector/_template.py
+-rw-r--r--   0        0        0    16392 2023-07-12 14:57:22.958818 gemini_self_protector-0.1.2/src/gemini_self_protector/_utils.py
+-rw-r--r--   0        0        0     6391 2023-07-03 17:31:00.908120 gemini_self_protector-0.1.2/src/gemini_self_protector/gemini_self_protector.py
+-rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/dark.css
+-rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/install.css
+-rw-r--r--   0        0        0   311910 2023-07-04 17:15:39.423308 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/style.css
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
+-rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
+-rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
+-rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
+-rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
+-rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
+-rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
+-rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
+-rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
+-rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
+-rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/chrome.png
+-rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/firefox.png
+-rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/ie.png
+-rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/opera.png
+-rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/safari.png
+-rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/favicon.ico
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/gemini-7.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-dark.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-thumb.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo.png
+-rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
+-rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
+-rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
+-rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
+-rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
+-rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
+-rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
+-rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
+-rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
+-rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
+-rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
+-rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
+-rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
+-rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
+-rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/profile.jpg
+-rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-1.png
+-rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-2.png
+-rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/box.png
+-rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
+-rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
+-rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
+-rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
+-rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
+-rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
+-rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
+-rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/dark-mode.js
+-rw-r--r--   0        0        0    10781 2023-07-12 14:30:13.012279 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/install.js
+-rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
+-rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
+-rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pcoded.min.js
+-rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
+-rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
+-rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
+-rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
+-rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
+-rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
+-rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
+-rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
+-rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
+-rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
+-rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
+-rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
+-rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
+-rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
+-rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
+-rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
+-rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
+-rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
+-rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
+-rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
+-rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
+-rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
+-rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
+-rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
+-rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/scss/dark.scss
+-rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/accounts/login.html
+-rw-r--r--   0        0        0    11196 2023-07-04 17:16:01.979812 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/acl.html
+-rw-r--r--   0        0        0    23017 2023-07-12 14:42:39.685655 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/config.html
+-rw-r--r--   0        0        0     7827 2023-07-04 17:16:19.165269 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/dependency.html
+-rw-r--r--   0        0        0     4563 2023-07-04 17:16:27.724233 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/endpoint.html
+-rw-r--r--   0        0        0     5184 2023-07-05 11:53:27.086067 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/feedback.html
+-rw-r--r--   0        0        0    32266 2023-07-04 17:17:24.326002 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/index.html
+-rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-403.html
+-rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-404.html
+-rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-500.html
+-rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-blank.html
+-rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/profile.html
+-rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/navigation.html
+-rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/scripts.html
+-rw-r--r--   0        0        0     5310 2023-07-12 14:31:09.510236 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/sidebar.html
+-rw-r--r--   0        0        0    15819 2023-07-12 14:30:33.367878 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/install.html
+-rw-r--r--   0        0        0     1683 2023-07-12 14:31:24.110465 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/key.html
+-rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
+-rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base.html
+-rw-r--r--   0        0        0     7452 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.2/PKG-INFO
```

### Comparing `gemini_self_protector-0.1.1/LICENSE` & `gemini_self_protector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/README.md` & `gemini_self_protector-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/__init__.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_audit.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_audit.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_cli.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_cli.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_config.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
-import yaml
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from ._logger import logger
 import json
+import csv
 from ipaddress import ip_address
 from datetime import datetime
-from ._model import Base, tb_User, tb_Config, tb_Summary, tb_RequestLog, tb_AccessControlList, tb_Dependency
+from ._model import Base, tb_User, tb_Config, tb_Summary, tb_RequestLog, tb_AccessControlList, tb_Dependency, tb_Feedback
 
 class _Config(object):
 
     def __init__(self, working_directory):
 
         database_file = working_directory+'/gemini.db'
         try:
@@ -178,14 +178,27 @@
                 event_id=event_id).first()
             session.close()
             return req_record
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Config.get_tb_config', e))
 
+    def update_record_request_log(_event_id) -> None:
+        try:
+            session = _Config.get_session()
+            request_log_record = session.query(tb_RequestLog).filter_by(
+                event_id=_event_id).first()
+            if request_log_record:
+                request_log_record.review = True
+                session.commit()
+                session.close()
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Config.update_record_request_log', e))
+
     def get_tb_acl() -> None:
         try:
             session = _Config.get_session()
             acl = _Config.get_model_instance_all(session, tb_AccessControlList)
             return acl
         except Exception as e:
             logger.error(
@@ -275,7 +288,48 @@
             )
             session.add(new_record)
             session.commit()
             session.close()
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Config.store_tb_dependency', e))
+
+    def get_tb_feedback() -> None:
+        try:
+            session = _Config.get_session()
+            feedback = _Config.get_model_instance_all(session, tb_Feedback)
+            return feedback
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong, please check your error message.\n Message - {0}".format('_Config.get_tb_dependency', e))
+
+    def store_tb_feedback(_sentence, _label):
+        try:
+            session = _Config.get_session()
+            new_record = tb_Feedback(
+                sentence=_sentence,
+                label=_label,
+            )
+            session.add(new_record)
+            session.commit()
+            session.close()
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Config.store_gemini_feedback', e))
+
+    def export_tb_feedback() -> str:
+        try:
+            session = _Config.get_session()
+            feedback = _Config.get_model_instance_all(session, tb_Feedback)
+
+            gemini_working_directory = _Config.get_tb_config().working_directory
+            csv_file_path = gemini_working_directory+"/feedback.csv"
+
+            with open(csv_file_path, mode='w', newline='') as file:
+                writer = csv.writer(file)
+                writer.writerow(['Sentence', 'Label'])  # Write header
+                for row in feedback:
+                    writer.writerow([row.sentence, row.label])
+
+            return csv_file_path
+        except Exception as e:
+            logger.error("[x_x] Something went wrong, please check your error message.\n Message - {0}".format('_Config.export_tb_feedback', e))
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_gemini.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_gemini.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 from ._protect import _Protect
 from ._audit import _Audit
 from datetime import datetime, timezone
 
 
 class _Gemini(object):
 
-    def init_gemini_database(working_directory):
+    def init_gemini_database(_working_directory):
         try:
-            _Config(working_directory)
+            _Config(_working_directory)
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.update_gemini_config', e))
 
     def get_gemini_config() -> None:
         try:
             _gemini_return = _Config.get_tb_config()
             return _gemini_return
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_config', e))
 
-    def update_gemini_config(update_content):
+    def update_gemini_config(_update_content):
         try:
-            _Config.update_tb_config(update_content)
+            _Config.update_tb_config(_update_content)
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.update_gemini_config', e))
 
     def get_gemini_user() -> None:
         try:
             _gemini_return = _Config.get_tb_user()
@@ -69,30 +69,36 @@
         try:
             _gemini_return = _Config.get_tb_request_log()
             return _gemini_return
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_summary', e))
 
-    def get_gemini_detail_request_log(event_id) -> None:
+    def get_gemini_detail_request_log(_event_id) -> None:
         try:
-            _gemini_return = _Config.get_tb_request_log_first(event_id)
+            _gemini_return = _Config.get_tb_request_log_first(_event_id)
             return _gemini_return
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_detail_request_log', e))
 
-
     def store_gemini_request_log(ipaddress, url, request, response, attack_type, predict, event_id, latitude, longitude):
         try:
             _Config.store_tb_request_log(ipaddress, url, request, response, attack_type, predict, event_id, latitude, longitude)
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.store_gemini_request_log', e))
 
+    def update_gemini_request_log(_event_id):
+        try:
+            _Config.update_record_request_log(_event_id)
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.update_gemini_request_log', e))
+
     def get_gemini_acl():
         try:
             _gemini_return = _Config.get_tb_acl()
             return _gemini_return
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_acl', e))
@@ -122,41 +128,45 @@
         try:
             _gemini_return = _Config.get_tb_dependency()
             return _gemini_return
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_audit_dependency', e))
 
-    def validator_license_key(license_key):
-        """
-        It takes a license key as an argument and validates it
+    def get_gemini_feedback() -> None:
+        try:
+            _gemini_return = _Config.get_tb_feedback()
+            return _gemini_return
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.get_gemini_feedback', e))
 
-        :param license_key: The license key you received from the license server
-        """
+    def store_gemini_feedback(_sentence, _label):
         try:
-            _gemini_return = _Validator.validate_license_key(license_key)
+            _Config.store_tb_feedback(_sentence, _label)
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.store_gemini_feedback', e))
+
+    def export_gemini_feedback() -> str:
+        try:
+            _gemini_return = _Config.export_tb_feedback()
             return _gemini_return
         except Exception as e:
             logger.error(
-                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.validator_license_key', e))
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.export_gemini_feedback', e))
 
-    def is_valid_license_key() -> None:
-        """
-        This function attempts to validate a license key and logs an error message if an exception
-        occurs.
-        :return: the output of the `_Validator.is_valid_license_key()` method, which is not specified in
-        the code provided. The return type is also not specified, but it is assumed to be a boolean
-        value since the method name suggests that it is checking if a license key is valid or not.
-        """
+
+    def validator_key_auth(_key):
         try:
-            _gemini_return = _Validator.is_valid_license_key()
+            _gemini_return = _Validator.validate_key_auth(_key)
             return _gemini_return
         except Exception as e:
             logger.error(
-                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.is_valid_license_key', e))
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.validator_key_auth', e))
 
     def validator_protect_mode(protect_mode) -> None:
         """
         The function takes a string as an argument, and checks if the string is in a list of strings. If
         it is, it returns the string. If it isn't, it returns None
 
         :param protect_mode: This is the mode of the protector
@@ -438,20 +448,20 @@
     def health_check_predict_server() -> None:
         try:
             return _Utils.predict_server_health()
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.check_predict_server', e))
 
-    def validator_predict_server(server) -> None:
+    def validator_predict_server(_server, _key) -> None:
         try:
-            return _Validator.validate_predict_server(server)
+            return _Validator.validate_predict_server(_server, _key)
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.validator_predict_server', e))
 
     def __load_mini_anti_dos__() -> None:
         try:
             return _Protect.__handle_mini_anti_dos__()
         except Exception as e:
             logger.error(
-                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.__load_mini_anti_dos__', e))
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Gemini.__load_mini_anti_dos__', e))
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_gui.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-from flask import Flask, Blueprint, request, make_response, render_template, session, redirect, url_for, flash, stream_with_context, jsonify
+from flask import Flask, Blueprint, request, make_response, render_template, session, redirect, url_for, flash, stream_with_context, jsonify, send_file
 from ._logger import logger
 from ._gemini import _Gemini
-from flask_sqlalchemy import SQLAlchemy
-from argon2 import PasswordHasher, exceptions as argon2_exceptions
+from passlib.hash import argon2
 from datetime import datetime, timezone
 import ipaddress
 import re
 import os
 import json
 import ast
 from math import floor
 
 class _Gemini_GUI(object):
 
     def __init__(self, flask_app: Flask) -> None:
         logger.info(
             "[+] Running gemini-self protector - GUI Mode")
-        
+
         # @flask_app.before_request
         # def count_request_to_service():
         #     _Gemini.calulate_total_access()
 
         # Create a blueprint for the nested Flask service
         nested_service = Blueprint(
             'nested_service', __name__, template_folder="templates", static_folder='static')
 
         if flask_app.secret_key is None:
             flask_app.secret_key = _Gemini.get_gemini_config().secret_key
-
+        
+        if flask_app.config.get('MAX_CONTENT_LENGTH') is None:
+            flask_app.config.update(
+                MAX_CONTENT_LENGTH= _Gemini.get_gemini_config().max_content_length
+            )
+        
         if flask_app.template_folder and flask_app.static_folder:
             if _Gemini.get_gemini_config().app_path is None:
                 _Gemini.init_gemini_app_path()
 
             _Gemini.init_gemini_dashboard(
                 flask_app.template_folder, flask_app.static_folder)
 
             gemini_app_path = _Gemini.get_gemini_config().app_path
             logger.info(
                 "[+] Access Your Gemini Dashboard as Path: http://host:port/{0}".format(gemini_app_path))
-
+            
             @nested_service.app_template_filter('gemini_datetime_format')
             def datetime_format(value, format='%d %B %H:%M'):
                 if isinstance(value, str):
                     value = datetime.strptime(value, '%Y-%m-%d %H:%M:%S')
                 return value.strftime(format)
 
             @nested_service.app_template_filter('gemini_round_number')
@@ -78,42 +82,42 @@
                         if request.method == 'POST':
                             protect_mode = request.form['radio-mode']
                             sensitive_value = request.form['sensitive-value']
                             app_path = request.form['gemini-app-path']
                             password = request.form['pwd']
                             confirm_password = request.form['cpwd']
                             notification_channel = request.form['radio-channel']
-                            license_key = request.form['license-key']
+                            predict_server_key_auth = request.form['key-auth-server-value']
                             predict_server = request.form['predit-server-value']
                             telegram_token = ''
                             telegram_chat_id = ''
                             notification_webhook = ''
                             if notification_channel == 'disable':
                                 notification_channel = 'disable'
                             elif notification_channel == 'telegram':
                                 telegram_token = request.form['telegram-token']
                                 telegram_chat_id = request.form['telegram-chat-id']
                             else:
                                 notification_webhook = request.form['channel-webhook']
 
-                            if _Gemini.validator_protect_mode(protect_mode) and _Gemini.validator_sensitive_value(sensitive_value) and _Gemini.validator_app_path(app_path) and _Gemini.validator_dashboard_password(password, confirm_password) and _Gemini.validator_notification_channel(notification_channel) and _Gemini.validator_license_key(license_key) and _Gemini.validator_predict_server(predict_server):
-                                ph = PasswordHasher()
+                            if _Gemini.validator_protect_mode(protect_mode) and _Gemini.validator_sensitive_value(sensitive_value) and _Gemini.validator_app_path(app_path) and _Gemini.validator_dashboard_password(password, confirm_password) and _Gemini.validator_notification_channel(notification_channel) and _Gemini.validator_predict_server(predict_server, predict_server_key_auth):
                                 _Gemini.update_gemini_config({
                                     "isinstall": True,
                                     "global_protect_mode": protect_mode,
                                     "sensitive_value": int(sensitive_value),
                                     "app_path": app_path,
                                     "notification_channel": notification_channel,
                                     "telegram_token": telegram_token,
                                     "telegram_chat_id": telegram_chat_id,
                                     "notification_webhook": notification_webhook,
-                                    "predict_server": predict_server
+                                    "predict_server": predict_server,
+                                    "predict_server_key_auth" : predict_server_key_auth
                                 })
                                 _Gemini.update_gemini_user({
-                                    "password": ph.hash(password),
+                                    "password": argon2.hash(password),
                                 })
                                 logger.info(
                                     "[+] Install gemini-self-protector successful.!")
                                 flash('Instal gemini-self-protector successful. Login and explore now', 'login')
                                 return redirect(url_for('nested_service.gemini_login'))
                         else:
                             sensitive_value = _Gemini.get_gemini_config().sensitive_value
@@ -133,21 +137,20 @@
 
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
                     
                     if request.method == 'POST':
                         key = request.form['key']
-                        if _Gemini.validator_license_key(key):
-                            flash('License key update successful', 'key_update_success')
+                        if _Gemini.validator_key_auth(key):
+                            flash('Predict server key auth update successful', 'key_update_success')
                             return redirect(url_for('nested_service.gemini_dashboard'))
                         else:
-                            return render_template('gemini-protector-gui/license.html', msg="Invalid license key")
-
-                    return render_template('gemini-protector-gui/license.html')
+                            return render_template('gemini-protector-gui/key.html', msg="Invalid predict server key auth")
+                    return render_template('gemini-protector-gui/key.html')
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_update_key', e))
 
             @nested_service.route('/login', methods=['GET', 'POST'])
             def gemini_login():
                 try:
@@ -162,71 +165,56 @@
                     if request.method == 'POST':
                         username = request.form['username']
                         password = request.form['password']
 
                         app_username = _Gemini.get_gemini_user().username
                         app_password = _Gemini.get_gemini_user().password
 
-                        ph = PasswordHasher()
-                        try:
-                            ph.verify(app_password, password)
-                        except argon2_exceptions.VerifyMismatchError:
-                            return render_template('gemini-protector-gui/accounts/login.html', msg="Incorrect Username / Password")
-
-                        if username == app_username:
+                        password_check = argon2.verify(password, app_password)
+                        
+                        if username == app_username and password_check:
                             session['gemini_logged_in'] = True
-
-                            if not _Gemini.is_valid_license_key():
-                                flash('Please update license key!', 'required')
-                                return redirect(url_for('nested_service.gemini_update_key'))
-   
                             flash('Welcome back {}!'.format(app_username), 'login')
                             return redirect(url_for('nested_service.gemini_dashboard'))
-
+                        else:
+                            return render_template('gemini-protector-gui/accounts/login.html', msg="Incorrect Username / Password")
                     return render_template('gemini-protector-gui/accounts/login.html')
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_login', e))
 
             @nested_service.route('/profile')
             def gemini_profile():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
                     
                     if request.method == 'POST':
                         password = request.form['pwd']
                         confirm_password = request.form['cpwd']
 
                         if not _Gemini.validator_dashboard_password(password, confirm_password):
                             return render_template('gemini-protector-gui/home/profile.html', msg="Invalid password")
 
-                        ph = PasswordHasher()
                         _Gemini.update_gemini_config({
-                            "gemini_app_password": ph.hash(password),
+                            "gemini_app_password": argon2.hash(password),
                         })
                         logger.info("[+] Update password successful.")
                         return redirect(url_for('nested_service.gemini_login'))
 
                     app_username = _Gemini.get_gemini_user().username
                     return render_template('gemini-protector-gui/home/profile.html', _username=app_username)
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_profile', e))
 
             @nested_service.route('/dashboard')
             def gemini_dashboard():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-                    
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
                     
                     gemini_summary = _Gemini.get_gemini_summary()
                     gemini_config = _Gemini.get_gemini_config()
                     gemini_user = _Gemini.get_gemini_user()
@@ -278,17 +266,14 @@
                                         )
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_dashboard', e))
 
             @nested_service.route('/configurate', methods=['GET', 'POST'])
             def gemini_configurate():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
 
                     if request.method == 'POST':
                         predict_server = request.form['predict_server']
                         protect_mode = request.form['protect_mode']
@@ -345,17 +330,14 @@
                                             )
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_configurate', e))
 
             @nested_service.route('/access-control-list', methods=['GET', 'POST'])
             def gemini_access_control_list():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
 
                     if request.method == 'POST':
                         ip_address = request.form['ip_address']
                         access_type = request.form['access_type']
@@ -403,17 +385,14 @@
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_access_control_list', e))
 
             @nested_service.route('/remove-acl', methods=['POST'])
             def gemini_remove_acl():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
 
                     ip_address = request.form['ip_address']
 
                     try:
@@ -428,17 +407,14 @@
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_remove_acl', e))
 
             @nested_service.route('/dependency-vulnerability', methods=['GET', 'POST'])
             def gemini_dependency_audit():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
 
                     if request.method == 'POST':
                         file_path = request.form['dependency_path']
                         filename = os.path.basename(file_path)
                         if filename == 'requirements.txt':
@@ -474,25 +450,24 @@
 
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_dependency_audit', e))
 
             @nested_service.route('/event', methods=['POST'])
             def gemini_get_event():
                 try:
-                    if not _Gemini.is_valid_license_key():
-                        return redirect(url_for('nested_service.gemini_update_key'))
-
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
 
                     event_id = request.json['event_id']
 
                     record = _Gemini.get_gemini_detail_request_log(event_id)
                     if record:
+                        if record.predict is None:
+                            _Gemini.update_gemini_request_log(record.event_id)
                         return jsonify({
                             "status": True,
                             "time": record.time,
                             "ip_address": record.ipaddress,
                             "event_id": record.event_id,
                             "url": record.url,
                             "user_agent": record.useragent,
@@ -511,28 +486,132 @@
                         return jsonify({
                             "status": False,
                             "message": "Event ID does not exist"
                         })
                 except Exception as e:
                     logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_get_event', e))
 
+            @nested_service.route('/event-feedback', methods=['POST'])
+            def gemini_event_feedback():
+                try:
+                    if not session.get('gemini_logged_in'):
+                        return redirect(url_for('nested_service.gemini_login'))
+                    
+                    event_id = request.json['event_id']
+                    feedback_value = request.json['feedback_value']
+
+                    record = _Gemini.get_gemini_detail_request_log(event_id)
+                    if record:
+                        sentence = "{}{}".format(record.request, record.req_body)
+                        _Gemini.store_gemini_feedback(sentence, int(feedback_value))
+                        _Gemini.update_gemini_request_log(record.event_id)
+                        return jsonify({
+                            "status": True,
+                            "message": "Update feedback successful"
+                        })
+                    else:
+                        return jsonify({
+                            "status": False,
+                            "message": "Update feedback failed"
+                        })
+                except Exception as e:
+                    logger.error(
+                        "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_event_feedback', e))
+            
+            @nested_service.route('/endpoint', methods=['GET'])
+            def gemini_endpoint():
+                try:
+                    if not session.get('gemini_logged_in'):
+                        return redirect(url_for('nested_service.gemini_login'))
+                    
+                    app_path = _Gemini.get_gemini_config().app_path
+                    links = []
+                    for rule in flask_app.url_map.iter_rules():
+                        options = {}
+                        for arg in rule.arguments:
+                            options[arg] = "[{0}]".format(arg)
+
+                        methods = ','.join(rule.methods)
+                        url = url_for(rule.endpoint, _external=True, **options)
+                        if app_path not in url:
+                            link = {
+                                'endpoint': rule.endpoint,
+                                'method': methods,
+                                'url': url,
+                            }
+                            links.append(link)
+
+                    _sorted_links = sorted(links, key=lambda x: x['endpoint'])
+                    page = int(request.args.get('page', 1))
+                    per_page = 5
+
+                    total_records = len(_sorted_links)
+                    total_pages = (total_records + per_page - 1) // per_page
+
+                    start_index = (page - 1) * per_page
+                    end_index = start_index + per_page
+                    limited_links = _sorted_links[start_index:end_index]
+                    return render_template('gemini-protector-gui/home/endpoint.html', 
+                                            _sorted_links=limited_links,
+                                            _current_page=page,
+                                            _total_pages=total_pages
+                                           )
+                except Exception as e:
+                    logger.error(
+                        "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_endpoint', e))
+
+            @nested_service.route('/feedback', methods=['GET'])
+            def gemini_feedback():
+                try:
+                    if not session.get('gemini_logged_in'):
+                        return redirect(url_for('nested_service.gemini_login'))
+                    
+                    feedback = _Gemini.get_gemini_feedback()
+
+                    _sorted_links = sorted(feedback, key=lambda x: x.created_at)
+                    page = int(request.args.get('page', 1))
+                    per_page = 5
+
+                    total_records = len(_sorted_links)
+                    total_pages = (total_records + per_page - 1) // per_page
+
+                    start_index = (page - 1) * per_page
+                    end_index = start_index + per_page
+                    limited_links = _sorted_links[start_index:end_index]
+                    return render_template('gemini-protector-gui/home/feedback.html', 
+                                            _sorted_links=limited_links,
+                                            _current_page=page,
+                                            _total_pages=total_pages
+                                           )
+                except Exception as e:
+                    logger.error(
+                        "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_endpoint', e))
+
+            @nested_service.route('/export-feedback')
+            def gemini_export_feedback():
+                try:
+                    if not session.get('gemini_logged_in'):
+                        return redirect(url_for('nested_service.gemini_login'))
+                    
+                    csv_file = _Gemini.export_gemini_feedback()
+                    return send_file(csv_file, as_attachment=True) 
+                except Exception as e:
+                    logger.error(
+                        "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_export_feedback', e))
+
             @nested_service.route('/logout')
             def gemini_logout():
                 try:
                     app_username = _Gemini.get_gemini_user().username
                     session['gemini_logged_in'] = False
                     flash('Goodbye {}!'.format(app_username), 'logout')
                     return redirect(url_for('nested_service.gemini_login'))
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_logout', e))
-
-            @nested_service.route('/chart')
-            def gemini_chart():
-                return render_template('gemini-protector-gui/home/chart-morris.html')
             
             @nested_service.errorhandler(403)
             def access_forbidden(error):
                 return render_template('gemini-protector-gui/home/page-403.html'), 403
 
             @nested_service.errorhandler(404)
             def not_found_error(error):
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_logger.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_logger.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_model.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,17 +14,16 @@
     password = Column(String)
 
 
 class tb_Config(Base):
     __tablename__ = 'configs'
 
     id = Column(Integer, primary_key=True)
-    license_key = Column(String)
+    predict_server_key_auth = Column(String)
     isinstall = Column(Integer)
-    access_token = Column(String)
     app_path = Column(String)
     database_path = Column(String)
     cors = Column(JSON)
     predict_server = Column(String)
     global_protect_mode = Column(String)
     http_method_allow = Column(String)
     max_content_length = Column(Integer)
@@ -77,14 +76,15 @@
     latitude = Column(Float)
     longitude = Column(Float)
     status = Column(String)
     review = Column(String)
     created_at = Column(DateTime, default=func.now())
     updated_at = Column(DateTime, default=func.now(), onupdate=func.now())
 
+
 class tb_AccessControlList(Base):
     __tablename__ = 'acls'
 
     id = Column(Integer, primary_key=True)
     ipaddress = Column(String, unique=True)
     is_allowed = Column(Integer)
     desciption = Column(String)
@@ -98,7 +98,17 @@
     id = Column(Integer, primary_key=True)
     package = Column(String)
     version = Column(String)
     cve_id = Column(String)
     severity = Column(String)
     created_at = Column(DateTime, default=func.now())
     updated_at = Column(DateTime, default=func.now(), onupdate=func.now())
+
+
+class tb_Feedback(Base):
+    __tablename__ = 'feedbacks'
+
+    id = Column(Integer, primary_key=True)
+    sentence = Column(String)
+    label = Column(String)
+    created_at = Column(DateTime, default=func.now())
+    updated_at = Column(DateTime, default=func.now(), onupdate=func.now())
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_protect.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_protect.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
             cors = _Config.get_tb_config().cors
             cors_origin = cors['origin']
             cors_method = cors['methods']
             cors_credential = cors['credentials']
             cors_header = cors['headers']
             http_method_list = ast.literal_eval(http_method_allow)
 
+            response.add_etag()
             response.headers['Server'] = server_name
             response.headers['X-Gemini-Self-Protector'] = global_protect_mode
             response.headers['Referrer-Policy'] = 'no-referrer-when-downgrade'
             response.headers['X-Content-Type-Options'] = 'nosniff'
             response.headers['X-XSS-Protection'] = '1; mode=block'
             response.headers['X-Frame-Options'] = 'SAMEORIGIN'
             response.headers['Strict-Transport-Security'] = 'max-age=31536000; includeSubDomains; preload'
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_template.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_template.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/_utils.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,27 +100,30 @@
 
         :param payload: The payload is the data that you want to send to the API. In this case, it's the
         data that you want to predict
         :return: The accuracy of the prediction.
         """
         try:
             predict_server = _Config.get_tb_config().predict_server
-            headers = {"Content-Type": "application/json"}
-            predict = requests.post(f'{predict_server}/predict', json={"data": payload}, headers=headers)
+            predict_server_key_auth = _Config.get_tb_config().predict_server_key_auth
+            headers = {"Content-Type": "application/json",
+                       "Authorization": predict_server_key_auth}
+            predict = requests.post(
+                f'{predict_server}/predict', json={"data": payload}, headers=headers)
             if (predict):
                 response = predict.json()
-                accuracy = response.get('accuracy')
+                accuracy = response.get('accuracy', 0)
                 return accuracy
             else:
                 logger.warning(
                     "[!] Cannot connect to predict server. Gemini-self protector cannot predit this request.")
                 return 0
         except requests.exceptions.RequestException as e:
             logger.warning(
-                    "[!] Cannot connect to predict server. Gemini-self protector cannot predit this request.")
+                "[!] Cannot connect to predict server. Gemini-self protector cannot predit this request.")
             return 0
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Utils.web_vuln_detect_predict', e))
 
     def flask_client_ip() -> None:
         """
@@ -199,59 +202,35 @@
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.predict_server_health', e))
 
 
 class _Validator(object):
 
-    def validate_license_key(license_key) -> None:
-        """
-        If the license key is valid, then update the config file with the license key and the access
-        token
-
-        :param license_key: The license key that you received from the API
-        :return: True or False
-        """
+    def validate_key_auth(_key) -> None:
         try:
-            if license_key:
-                if license_key == '988907ce-9803-11ed-a8fc-0242ac120002':
-                    # call api and return access_token
-                    access_token = jwt.encode(
-                        {"license": license_key}, "secret", algorithm="HS256")
-
+            if _key:
+                predict_server = _Config.get_tb_config().predict_server
+                headers = {"Content-Type": "application/json",
+                           "Authorization": _key}
+                response = requests.post(
+                    f'{predict_server}/predict', json={"data": "healthcheck"}, headers=headers)
+                data = response.json()
+                if response.status_code == 200 and 'accuracy' in data:
                     _Config.update_tb_config({
-                        'license_key': license_key,
-                        'access_token': access_token
+                        'predict_server_key_auth': _key,
                     })
                     return True
                 else:
-                    logger.error("[x_x] Invalid License Key")
                     return False
             else:
-                logger.error("[x_x] Invalid License Key")
                 return False
         except Exception as e:
             logger.error(
-                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.validate_license_key', e))
-
-    def is_valid_license_key() -> None:
-        """
-        The function checks if a given license key is valid and returns a boolean value.
-        :return: a boolean value (True or False) depending on whether the current_key matches the
-        specified license key or not.
-        """
-        try:
-            current_key = _Config.get_tb_config().license_key
-            if current_key == '988907ce-9803-11ed-a8fc-0242ac120002':
-                return True
-            else:
-                return False
-        except Exception as e:
-            logger.error(
-                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.is_valid_license_key', e))
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.validate_key_auth', e))
 
     def validate_protect_mode(protect_mode) -> None:
         """
         It checks if the protect_mode is in the array arr_mode. If it is, it returns True. If it isn't,
         it returns False
 
         :param protect_mode: This is the mode that you want to run the script in
@@ -387,24 +366,23 @@
                         return False
                     else:
                         return True
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.validate_trust_domain', e))
 
-    def validate_predict_server(server) -> None:
+    def validate_predict_server(_server, _key) -> None:
         try:
-            if re.match(r'https?://\S+', server):
-                headers = {"Content-Type": "application/json"}
+            if re.match(r'https?://\S+', _server):
+                headers = {"Content-Type": "application/json",
+                           "Authorization": _key}
                 response = requests.post(
-                    f'{server}/predict', json={"data": "healthcheck"}, headers=headers)
-                if response.status_code == 200:
-                    _Config.update_tb_config({
-                        'predict_server': server,
-                    })
+                    f'{_server}/predict', json={"data": "healthcheck"}, headers=headers)
+                data = response.json()
+                if response.status_code == 200 and 'accuracy' in data:
                     return True
                 else:
                     return False
             else:
                 return False
         except Exception as e:
             logger.error(
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/gemini_self_protector.py` & `gemini_self_protector-0.1.2/src/gemini_self_protector/gemini_self_protector.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/dark.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/dark.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/install.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/install.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/css/style.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -9028,14 +9028,18 @@
   border-left: 1px solid #eaeaea;
 }
 
 .table-columned>tbody>tr>th {
   border: 0;
 }
 
+.unread {
+  background-color: rgb(246, 229, 222);
+}
+
 /**====== Foo-table css end ======**/
 /**====== Data Tables css end ======**/
 /**  =====================
       Authentication css start
 ==========================  **/
 .auth-wrapper {
   position: relative;
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/chrome.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/chrome.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/firefox.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/firefox.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/ie.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/ie.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/opera.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/opera.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/browser/safari.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/safari.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/favicon.ico` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/gemini-7.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/gemini-7.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo-dark.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-dark.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo-thumb.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-thumb.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/logo.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img1.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img2.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/slider/img3.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/profile.jpg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/profile.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/user-1.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/user/user-2.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/box.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/box.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/images/widget/emoticon.png` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/emoticon.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/dark-mode.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/dark-mode.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/install.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/install.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -181,36 +181,52 @@
             jQuery(this).siblings('.wizard-form-error').slideUp("3000");
         }
     });
 
     $("#predict-server").click(function(event) {
         $("#loading-spinner").show();
         // Get the input value
-        var inputValue = $("#predictServerValue").val();
-
+        var serverValue = $("#predictServerValue").val();
+        var keyAuthValue = $("#keyAuthServerValue").val();
         // Make the POST request
         $.ajax({
-            url: inputValue + '/predict',
+            url: serverValue + '/predict',
             type: "POST",
+            headers: {
+                "Authorization": keyAuthValue
+            },
             contentType: "application/json",
             data: JSON.stringify({
                 data: "healthcheck"
             }),
             success: function(response) {
                 // Handle the success response
-                Toastify({
-                    text: "Connected to this predict server",
-                    duration: 3000,
-                    gravity: "top", // `top` or `bottom`
-                    position: "right", // `left`, `center` or `right`
-                    stopOnFocus: true, // Prevents dismissing of toast on hover
-                    style: {
-                        background: "linear-gradient(to right, #00b09b, #96c93d)",
-                    },
-                }).showToast();
+                if (response.accuracy) {
+                    Toastify({
+                        text: "Connected to this predict server",
+                        duration: 3000,
+                        gravity: "top", // `top` or `bottom`
+                        position: "right", // `left`, `center` or `right`
+                        stopOnFocus: true, // Prevents dismissing of toast on hover
+                        style: {
+                            background: "linear-gradient(to right, #00b09b, #96c93d)",
+                        },
+                    }).showToast();
+                } else {
+                    Toastify({
+                        text: "Cannot connect to this predict server",
+                        duration: 3000,
+                        gravity: "top", // `top` or `bottom`
+                        position: "right", // `left`, `center` or `right`
+                        stopOnFocus: true, // Prevents dismissing of toast on hover
+                        style: {
+                            background: "linear-gradient(to right, rgb(255, 95, 109), rgb(255, 195, 113))",
+                        },
+                    }).showToast();
+                }
             },
             error: function(error) {
                 // Handle the error response
                 Toastify({
                     text: "Cannot connect to this predict server",
                     duration: 3000,
                     gravity: "top", // `top` or `bottom`
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pages/google-maps.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/google-maps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/pcoded.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pcoded.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/js/vendor-all.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/vendor-all.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/assets/scss/dark.scss` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/scss/dark.scss`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/accounts/login.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/acl.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/acl.html`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
 <script>
     const removeButtons = document.querySelectorAll('.remove-acl-btn');
     removeButtons.forEach(button => {
         button.addEventListener('click', () => {
             const ip = button.getAttribute('data-ip');
-            fetch('{{url_for('nested_service.gemini_remove_acl')}}', {
+            fetch("{{url_for('nested_service.gemini_remove_acl')}}", {
                 method: 'POST',
                 headers: {
                     'Content-Type': 'application/x-www-form-urlencoded'
                 },
                 body: `ip_address=${ip}`
             })
                 .then(response => {
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/config.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/config.html`

 * *Files 18% similar despite different names*

```diff
@@ -90,17 +90,30 @@
                                                         for="protect-mode-off">Off</label>
                                                 </div>
                                             </div>
                                             <!-- [ Protect Mode ] stop -->
                                             <!-- [ Predict Server ] start -->
                                             <div class="form-group">
                                                 <label>Predict Server</label>
-                                                <input type="text" class="form-control" placeholder="http://127.0.0.1"
-                                                    value="{{_predict_server}}" name="predict_server">
+                                                <div class="input-group mb-3">
+                                                    <input id="predictServerValue" type="text" class="form-control"
+                                                        placeholder="http://127.0.0.1" value="{{_predict_server}}"
+                                                        name="predict_server">
+                                                    <div class="input-group-append">
+                                                        <button class="btn btn-primary" id="predict-server-check"
+                                                            type="button">Check
+                                                            <div id="loading-spinner"
+                                                                style="display: none; float: right;">
+                                                                <i class="fa fa-spinner fa-spin"></i>
+                                                            </div>
+                                                        </button>
+                                                    </div>
+                                                </div>
                                             </div>
+
                                             <!-- [ Predict Server ] stop -->
                                             <!-- [ Sensitive Value ] start -->
                                             <div class="form-group">
                                                 <label>Sensitive Value</label>
                                                 <input type="text" class="form-control" placeholder="50"
                                                     value="{{_sensitive_value}}" name="sensitive_value">
                                             </div>
@@ -259,8 +272,65 @@
             background: "linear-gradient(to right, rgb(255, 95, 109), rgb(255, 195, 113))",
         },
     }).showToast();
 </script>
 {% endif %}
 {% endfor %}
 {% endwith %}
+<script>
+    $(document).ready(function () {
+        $("#predict-server-check").click(function (event) {
+            $("#loading-spinner").show();
+            var inputValue = $("#predictServerValue").val();
+            $.ajax({
+                url: inputValue + '/predict',
+                type: "POST",
+                contentType: "application/json",
+                data: JSON.stringify({ data: "healthcheck" }),
+                success: function (response) {
+                    if (response.message) {
+                        // Handle the success response
+                        Toastify({
+                            text: "Connected to this predict server",
+                            duration: 3000,
+                            gravity: "top", // `top` or `bottom`
+                            position: "right", // `left`, `center` or `right`
+                            stopOnFocus: true, // Prevents dismissing of toast on hover
+                            style: {
+                                background: "linear-gradient(to right, #00b09b, #96c93d)",
+                            },
+                        }).showToast();
+                    } else {
+                        Toastify({
+                            text: "Cannot connect to this predict server",
+                            duration: 3000,
+                            gravity: "top", // `top` or `bottom`
+                            position: "right", // `left`, `center` or `right`
+                            stopOnFocus: true, // Prevents dismissing of toast on hover
+                            style: {
+                                background: "linear-gradient(to right, rgb(255, 95, 109), rgb(255, 195, 113))",
+                            },
+                        }).showToast();
+                    }
+                },
+                error: function (error) {
+                    // Handle the error response
+                    Toastify({
+                        text: "Cannot connect to this predict server",
+                        duration: 3000,
+                        gravity: "top", // `top` or `bottom`
+                        position: "right", // `left`, `center` or `right`
+                        stopOnFocus: true, // Prevents dismissing of toast on hover
+                        style: {
+                            background: "linear-gradient(to right, rgb(255, 95, 109), rgb(255, 195, 113))",
+                        },
+                    }).showToast();
+                },
+                complete: function () {
+                    // Hide the loading spinner when the request is complete
+                    $("#loading-spinner").hide();
+                }
+            });
+        });
+    });
+</script>
 {% endblock javascripts %}
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/dependency.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/dependency.html`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
 <script>
     const removeButtons = document.querySelectorAll('.remove-acl-btn');
     removeButtons.forEach(button => {
         button.addEventListener('click', () => {
             const ip = button.getAttribute('data-ip');
-            fetch('{{url_for('nested_service.gemini_remove_acl')}}', {
+            fetch("{{url_for('nested_service.gemini_remove_acl')}}", {
                 method: 'POST',
                 headers: {
                     'Content-Type': 'application/x-www-form-urlencoded'
                 },
                 body: `ip_address=${ip}`
             })
                 .then(response => {
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-403.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-403.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-404.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-404.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-500.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-500.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/page-blank.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-blank.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/home/profile.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/profile.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/navigation.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/scripts.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/includes/sidebar.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/sidebar.html`

 * *Files 8% similar despite different names*

```diff
@@ -18,39 +18,52 @@
                     <label>Navigation</label>
                 </li>
                 <li data-username="Dashboard Page" class="nav-item {% if 'dashboard' in segment %} active {% endif %}">
                     <a href="{{url_for('nested_service.gemini_dashboard')}}" class="nav-link "><span
                             class="pcoded-micon"><i class="feather icon-home"></i></span><span
                             class="pcoded-mtext">Dashboard</span></a>
                 </li>
-                <li data-username="Configurate Page"
-                    class="nav-item {% if 'configurate' in segment %} active {% endif %}">
-                    <a href="{{ url_for('nested_service.gemini_configurate') }}" class="nav-link">
-                        <span class="pcoded-micon"><i class="feather icon-settings"></i></span>
-                        <span class="pcoded-mtext">Configurate</span></a>
+
+                <li data-username="Endpoint Page" class="nav-item {% if 'endpoint' in segment %} active {% endif %}">
+                    <a href="{{ url_for('nested_service.gemini_endpoint') }}" class="nav-link">
+                        <span class="pcoded-micon"><i class="feather icon-target"></i></span>
+                        <span class="pcoded-mtext">Endpoint</span></a>
                 </li>
 
                 <li data-username="ACL Page"
                     class="nav-item {% if 'access-control-list' in segment %} active {% endif %}">
                     <a href="{{ url_for('nested_service.gemini_access_control_list') }}" class="nav-link">
                         <span class="pcoded-micon"><i class="feather icon-cloud-off"></i></span>
                         <span class="pcoded-mtext">Access Control List</span></a>
                 </li>
 
-                <li data-username="ACL Page"
+                <li data-username="Dependency Page"
                     class="nav-item {% if 'dependency-vulnerability' in segment %} active {% endif %}">
                     <a href="{{ url_for('nested_service.gemini_dependency_audit') }}" class="nav-link">
                         <span class="pcoded-micon"><i class="feather icon-check-square"></i></span>
                         <span class="pcoded-mtext">Dependency Check</span></a>
                 </li>
 
-                <li data-username="ACL Page" class="nav-item {% if 'update-key' in segment %} active {% endif %}">
+                <li data-username="Configurate Page"
+                    class="nav-item {% if 'configurate' in segment %} active {% endif %}">
+                    <a href="{{ url_for('nested_service.gemini_configurate') }}" class="nav-link">
+                        <span class="pcoded-micon"><i class="feather icon-settings"></i></span>
+                        <span class="pcoded-mtext">Configurate</span></a>
+                </li>
+
+                <li data-username="Configurate Page" class="nav-item {% if 'feedback' in segment %} active {% endif %}">
+                    <a href="{{ url_for('nested_service.gemini_feedback') }}" class="nav-link">
+                        <span class="pcoded-micon"><i class="feather icon-star"></i></span>
+                        <span class="pcoded-mtext">Feedback</span></a>
+                </li>
+
+                <li data-username="Key Page" class="nav-item {% if 'update-key' in segment %} active {% endif %}">
                     <a href="{{ url_for('nested_service.gemini_update_key') }}" class="nav-link">
                         <span class="pcoded-micon"><i class="feather icon-heart"></i></span>
-                        <span class="pcoded-mtext">License Key</span></a>
+                        <span class="pcoded-mtext">Key</span></a>
                 </li>
 
                 <li data-username="Disabled Menu" class="nav-item">
                     <a href="{{ url_for('nested_service.gemini_logout') }}" class="nav-link">
                         <span class="pcoded-micon"><i class="feather icon-power"></i></span><span
                             class="pcoded-mtext">Logout</span>
                     </a>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 
 [Generic_placeholder_image]
 Gemini
 
     * Navigation
     * Dashboard
-    *  Configurate
+    *  Endpoint
     *  Access_Control_List
     *  Dependency_Check
-    *  License_Key
+    *  Configurate
+    *  Feedback
+    *  Key
     * Logout
     * More Resources
     *    Issue
     *    Support
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/install.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/install.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                                             <form id="install" method="POST"
                                                 action="{{url_for('nested_service.gemini_install')}}">
                                                 <div class="form-wizard-header">
                                                     <ul class="list-unstyled form-wizard-steps clearfix">
                                                         <li class="active"><span>1</span></li>
                                                         <li><span>2</span></li>
                                                         <li><span>3</span></li>
-                                                        <li><span>4</span></li>
+                                                        <!-- <li><span>4</span></li> -->
                                                     </ul>
                                                 </div>
                                                 <fieldset class="wizard-fieldset show">
                                                     <h5>Protect Mode</h5>
                                                     <div class="form-group">
                                                         <div class="wizard-form-radio">
                                                             <input name="radio-mode" id="radio1" type="radio"
@@ -56,18 +56,24 @@
                                                             name="sensitive-value" value="{{_sensitive_value}}"
                                                             required>
                                                         <!-- <label for="fname" class="wizard-form-text-label">Value</label> -->
                                                         <div class="wizard-form-error"></div>
                                                     </div>
                                                     <h5>Predict Server</h5>
                                                     <div class="form-group">
-                                                        <input type="text" min="0" max="100"
-                                                            class="form-control wizard-required" id="predictServerValue"
-                                                            name="predit-server-value" required>
-                                                        <a id="predict-server" href="#">Check</a>
+                                                        <input type="text" class="form-control wizard-required"
+                                                            id="predictServerValue" name="predit-server-value" required>
+                                                        <div class="wizard-form-error"></div>
+                                                    </div>
+                                                    <h5>Predict Server Key Auth</h5>
+                                                    <div class="form-group">
+                                                        <input type="text" class="form-control wizard-required"
+                                                            id="keyAuthServerValue" name="key-auth-server-value"
+                                                            required>
+                                                        <a id="predict-server" href="#">Check Connection</a>
                                                         <div id="loading-spinner" style="display: none; float: right;">
                                                             <i class="fa fa-spinner fa-spin"></i>
                                                         </div>
                                                         <div class="wizard-form-error"></div>
                                                     </div>
                                                     <div class="form-group clearfix">
                                                         <a href="javascript:;"
@@ -151,38 +157,36 @@
                                                     <div class="form-group" id="webhook-form">
                                                         <input type="text" class="form-control" id="channel_webhook"
                                                             name="channel-webhook">
                                                         <label for="channel_webhook"
                                                             class="wizard-form-text-label">Webhook</label>
                                                         <div class="wizard-form-error"></div>
                                                     </div>
-                                                    <div class="form-group clearfix">
+                                                    <!-- <div class="form-group clearfix">
                                                         <a href="javascript:;"
                                                             class="form-wizard-previous-btn float-left">Previous</a>
                                                         <a href="javascript:;"
                                                             class="form-wizard-next-btn float-right">Next</a>
+                                                    </div> -->
+                                                    <div class="form-group clearfix">
+                                                        <a href="javascript:;"
+                                                            class="form-wizard-previous-btn float-left">Previous</a>
+                                                        <a href="javascript:;" class="form-wizard-submit float-right"
+                                                            onclick="document.getElementById('install').submit();">Install</a>
                                                     </div>
                                                 </fieldset>
-                                                <fieldset class="wizard-fieldset">
+                                                <!-- <fieldset class="wizard-fieldset">
                                                     <h5>License</h5>
                                                     <div class="form-group">
                                                         <input type="text" class="form-control wizard-required"
                                                             id="license_key" name="license-key"
                                                             value="988907ce-9803-11ed-a8fc-0242ac120002">
-                                                        <!-- <label for="license_key" class="wizard-form-text-label">License
-                                                            Key</label> -->
                                                         <div class="wizard-form-error"></div>
                                                     </div>
-                                                    <div class="form-group clearfix">
-                                                        <a href="javascript:;"
-                                                            class="form-wizard-previous-btn float-left">Previous</a>
-                                                        <a href="javascript:;" class="form-wizard-submit float-right"
-                                                            onclick="document.getElementById('install').submit();">Install</a>
-                                                    </div>
-                                                </fieldset>
+                                                </fieldset> -->
                                             </form>
                                         </div>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </div>
```

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/layouts/base.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.1/src/gemini_self_protector/resource/templates/license.html` & `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/key.html`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             <span class="r"></span>
         </div>
         <div class="card">
             <div class="card-body text-center">
                 <a href="{{ url_for('nested_service.gemini_dashboard') }}" class="nav-link">
                     <span class="pcoded-micon"><i class="feather icon-arrow-left"></i></span>
                 </a>
-                <h3 class="mb-4">License Key</h3>
+                <h3 class="mb-4">Predict Server Key Auth</h3>
 
                 <span class="mb-2 text-muted">
                     {% if msg %}
                     <span class="text-danger">{{ msg | safe }}</span>
                     {% else %}
                     Update your key
                     {% endif %}
@@ -38,16 +38,15 @@
                         <input class="form-control" placeholder="License key" type="text" name="key" required>
                     </div>
 
                     <button type="submit" name="key" class="btn btn-primary shadow-2 mb-4">Update</button>
 
                 </form>
 
-                <p class="mb-0 text-muted">Need a key? <a
-                        href="https://github.com/noobpk/gemini-self-protector">gemini-self-protector</a></p>
+                <p class="mb-0 text-muted">Thank you for using.</p>
 
             </div>
         </div>
     </div>
 </div>
 
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "gemini-protector-gui/layouts/base-fullscreen.html" %} {% block
 title %} License Update {% endblock %} {% block content %}
 
-**** License Key ****
+**** Predict Server Key Auth ****
  {% if msg %} {{ msg | safe }} {% else %} Update your key {% endif %}
 
 [key                 ]
 Update
-Need a key? gemini-self-protector
+Thank you for using.
 {% endblock content %} {% block javascripts %}{% endblock javascripts %}
```

### Comparing `gemini_self_protector-0.1.1/PKG-INFO` & `gemini_self_protector-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gemini-self-protector
-Version: 0.1.1
+Version: 0.1.2
 Summary: Runtime Application Self-Protection
 License: MIT
 Author: lethanhphuc
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: flask-sqlalchemy (>=3.0.3,<4.0.0)
+Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # gemini_self_protector
 
 Gemini - The Runtime Application Self Protection (RASP) Solution Combined With Deep Learning
 
 ## Installation
```

