# Comparing `tmp/ebook-converter-noimage-4.12.1.tar.gz` & `tmp/ebook-converter-noimage-4.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebook-converter-noimage-4.12.1.tar", last modified: Wed Jul  5 15:05:41 2023, max compression
+gzip compressed data, was "ebook-converter-noimage-4.12.2.tar", last modified: Wed Jul 12 13:38:58 2023, max compression
```

## Comparing `ebook-converter-noimage-4.12.1.tar` & `ebook-converter-noimage-4.12.2.tar`

### file list

```diff
@@ -1,437 +1,437 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35151 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1226 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.330633 ebook-converter-noimage-4.12.1/ebook_converter/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2404 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2409 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/constants_old.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3912 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/ordered_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23830 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22273 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/select.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/tests.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/customize/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23498 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/customize/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39468 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/customize/builtins.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11939 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/customize/conversion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26449 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/customize/profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16013 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/customize/ui.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31220 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/default_tweaks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18267 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/fb2.xsl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7410 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/html.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   867091 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/iso_639-3.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/data/jacket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2824 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/jacket/stylesheet.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2419 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/jacket/template.xhtml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8121 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/lrf.xsl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42450 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/mime.types
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      214 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/new_nav.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17686 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/data/rtf.xsl
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/devices/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/devices/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29738 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/devices/interface.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/BeautifulSoup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8287 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5672 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/chardet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/compression/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/compression/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2790 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/compression/palmdoc.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.334633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15729 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.338633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      789 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/azw4_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/chm_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13345 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/comic_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/djvu_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1569 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/docx_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/docx_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/epub_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23301 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/epub_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7660 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/fb2_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7221 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/fb2_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11891 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/html_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10081 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/html_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4690 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/htmlz_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5514 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/htmlz_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2704 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lit_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lit_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lrf_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7617 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lrf_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2218 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/mobi_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14894 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/mobi_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/odt_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5043 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/oeb_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1129 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdb_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdb_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3080 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdf_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13044 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdf_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pml_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2949 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pml_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rb_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1270 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rb_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7437 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/recipe_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12454 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rtf_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1106 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rtf_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5227 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/snb_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12644 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/snb_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1135 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/tcr_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1712 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/tcr_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14920 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/txt_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7520 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/txt_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57255 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plumber.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28309 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/preprocess.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45890 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/covers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.338633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17177 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/block_styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9784 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/char_styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8016 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/cleanup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10040 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/container.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1164 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10139 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15547 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/fonts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/footnotes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12223 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8890 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5896 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/names.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14708 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/numbering.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20976 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25702 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/tables.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/theme.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36454 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/to_html.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4762 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/toc.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.338633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12846 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/container.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/fonts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27364 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/from_html.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10063 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6545 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/links.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6000 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/lists.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33237 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13874 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/tables.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1528 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.338633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/epub/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1481 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/epub/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.338633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/fb2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1210 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/fb2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24865 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/fb2/fb2ml.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8683 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/to_zip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46447 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html_entities.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/htmlz/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/htmlz/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16174 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/htmlz/oeb2html.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4410 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1542 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/fonts.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/color_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    89477 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/convert_from.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13908 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14304 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6864 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/lrfparser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27521 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/meta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42302 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/objects.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2059 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/elements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24013 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1466 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrfopt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80184 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7819 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/tags.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12090 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6564 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/archive.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5259 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32896 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/formatter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1841 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/json_codec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15062 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/fb2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14860 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/html.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/meta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/odt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70653 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/opf2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40629 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/opf3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/pdf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7732 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/rtf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11244 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/toc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/txt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24387 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/xmp.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/huffcdic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9871 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/langcodes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/mobiml.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/containers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14148 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/headers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9639 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15263 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/markup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42555 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/mobi6.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25484 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/mobi8.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3290 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/ncx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3626 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/tweak.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19662 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.342633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30330 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/indexer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17788 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6266 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/resources.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/serializer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1161 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/cleanup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7291 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/exth.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/odt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/odt/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13093 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/odt/input.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72526 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/normalize_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13253 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/parse_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    65763 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/container.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16500 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1711 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/opf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4436 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/parsing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9024 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/pretty.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15402 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/replace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19073 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/split.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33402 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/toc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7870 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29995 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32898 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/stylizer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5152 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/cover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/data_url.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/filenames.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29063 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/flatcss.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/guide.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4362 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/htmltoc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2697 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/jacket.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4017 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/manglecase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8584 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/metadata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6433 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/page_margin.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9123 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/rasterize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3411 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/rescale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19536 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/split.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14974 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/structure.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11263 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/subset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2637 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/trimmanifest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2705 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/writer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2863 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8849 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader132.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5475 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader202.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/formatreader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/haodoo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/haodoo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/haodoo/reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2801 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/header.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/palmdoc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/palmdoc/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2288 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/palmdoc/reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/pdf/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/pdf/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/pdf/reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/plucker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/plucker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27494 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/plucker/reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ztxt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ztxt/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3074 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ztxt/reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.346633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5949 2023-07-05 09:23:28.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/pdftohtml.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.350633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/render/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/render/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6357 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/render/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.350633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1166 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf/input.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.350633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23172 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/ParseRtf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8911 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/add_brackets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3357 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/body_styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8129 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/border_parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   705801 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/char_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2429 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/check_brackets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/check_encoding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9538 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/colors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3469 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/combine_borders.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10525 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/convert_to_tags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6372 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/default_encoding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8354 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/delete_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34875 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/field_strings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15252 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fields_large.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fields_small.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8971 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fonts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11089 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/footnote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2080 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/get_char_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10921 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/group_borders.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8815 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/group_styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10622 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/header.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8278 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/headings_to_sections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22384 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/hex_2_utf8.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11696 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16638 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/inline.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/line_endings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7757 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/list_numbers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18231 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/list_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/make_lists.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5159 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/old_rtf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4096 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8345 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/override_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29733 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/paragraph_def.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10351 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/paragraphs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7236 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/pict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23025 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/preamble_div.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/preamble_rest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42075 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/process_tokens.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19958 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/sections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27721 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/styles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20969 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3535 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/table_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/tokenize.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38659 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/functions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7790 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/unsmarten.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10479 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/markdownml.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/newlines.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11412 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19237 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/textileml.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/txtml.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1709 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406462 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/jacodepoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1334 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/jadecoder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406295 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/krcodepoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/krdecoder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   187198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/unicodepoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3978 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/unidecoder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406313 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/vncodepoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/vndecoder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   405777 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/zhcodepoints.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/library/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2515 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/library/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30056 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/library/field_metadata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-05 10:51:45.000000 ebook-converter-noimage-4.12.1/ebook_converter/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/polyglot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7424 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/ptempfile.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/spell/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1802 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/spell/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.354633 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12224 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/color3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29516 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/css21.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9126 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/decoding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7592 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/fonts3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/media3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/page3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4442 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/parsing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1052 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8336 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/color3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14313 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/css21.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3426 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/decoding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/fonts3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2909 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/media3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3770 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/page3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8808 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/tokenizing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13441 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/token_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7736 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tokenizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/tinycss/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/cleantext.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9618 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22068 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/config_base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      408 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/directory.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      721 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/encoding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3344 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/entities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13132 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/filenames.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4115 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/metadata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12951 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/scanner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1649 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11349 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/dict_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7734 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10242 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cmap.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7676 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6039 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/container.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      209 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3344 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/glyf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5802 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/gsub.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6671 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/head.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/kern.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3155 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/loca.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1575 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/maxp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12103 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/subset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17110 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14659 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/formatter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68191 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/formatter_functions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1355 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/html2text.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9060 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/icu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25367 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/img.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6097 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/imghdr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1409 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/iso8601.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3696 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/localization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10556 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/localunzip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/mreplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/resources.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3521 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1800 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/shared_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1928 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/short_uuid.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33107 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/smartypants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6712 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/speedups.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7489 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/terminal.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/titlecase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/wordcount.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/xml_parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    64817 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.1/ebook_converter/utils/zipfile.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 15:05:41.358633 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1226 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16333 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-05 15:05:41.000000 ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1062 2023-07-05 15:05:41.362633 ebook-converter-noimage-4.12.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-07-05 15:03:15.000000 ebook-converter-noimage-4.12.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35151 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1207 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.150485 ebook-converter-noimage-4.12.2/ebook_converter/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2404 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2409 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/constants_old.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.150485 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/errors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3912 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/ordered_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23830 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22273 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/select.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.154485 ebook-converter-noimage-4.12.2/ebook_converter/customize/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23498 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/customize/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39468 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/customize/builtins.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11939 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/customize/conversion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26449 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/customize/profiles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16013 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/customize/ui.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31220 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/default_tweaks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18267 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/fb2.xsl
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7410 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/html.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   867091 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/iso_639-3.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/data/jacket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2824 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/jacket/stylesheet.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2419 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/jacket/template.xhtml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8121 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/lrf.xsl
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42450 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/mime.types
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      214 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/new_nav.html
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17686 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/data/rtf.xsl
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/devices/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/devices/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29738 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/devices/interface.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/BeautifulSoup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8287 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5672 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/chardet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/compression/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/compression/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2790 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/compression/palmdoc.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.162485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15729 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.166485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      789 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/azw4_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/chm_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13345 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/comic_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/djvu_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1569 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/docx_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/docx_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/epub_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23301 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/epub_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7660 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/fb2_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7221 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/fb2_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11891 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/html_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10081 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/html_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4690 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/htmlz_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5514 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/htmlz_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2704 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lit_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lit_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lrf_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7617 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lrf_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2218 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/mobi_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14894 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/mobi_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/odt_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5043 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/oeb_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1129 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdb_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdb_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3080 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdf_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13044 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdf_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pml_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2949 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pml_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rb_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1270 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rb_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7437 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/recipe_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12454 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rtf_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1106 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rtf_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5227 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/snb_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12644 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/snb_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1135 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/tcr_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1712 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/tcr_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14920 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/txt_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7520 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/txt_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57255 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plumber.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28309 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/preprocess.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45890 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/covers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.170485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17177 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/block_styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9784 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/char_styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8016 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/cleanup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10040 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/container.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1164 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/dump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10139 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15547 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/fonts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/footnotes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12223 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8890 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5896 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/names.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14708 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/numbering.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20976 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25702 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/tables.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/theme.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36454 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/to_html.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4762 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/toc.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12846 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/container.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/fonts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27364 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/from_html.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10063 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6545 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/links.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6000 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/lists.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33237 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13874 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/tables.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1528 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/epub/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1481 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/epub/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/fb2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1210 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/fb2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24865 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/fb2/fb2ml.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8683 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/to_zip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46447 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html_entities.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/htmlz/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/htmlz/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16174 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/htmlz/oeb2html.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4410 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1542 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/fonts.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/color_map.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    89477 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/convert_from.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13908 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14304 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6864 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/lrfparser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27521 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/meta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42302 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/objects.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.174485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2059 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/elements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24013 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1466 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrfopt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80184 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7819 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/tags.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12090 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6564 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/archive.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5259 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32896 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/formatter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1841 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/json_codec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15062 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/fb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14860 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/html.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/meta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/odt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70653 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/opf2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40629 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/opf3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/pdf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7732 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/rtf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11244 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/toc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/txt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24387 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/xmp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/huffcdic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9871 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/langcodes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/mobiml.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/containers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14148 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/headers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9639 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15263 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/markup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42555 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/mobi6.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25484 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/mobi8.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3290 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/ncx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3626 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/tweak.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19662 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30330 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/indexer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17788 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6266 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/resources.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/serializer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1161 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/cleanup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7291 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/exth.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.178485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/odt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/odt/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13093 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/odt/input.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.182485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72526 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21170 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/normalize_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13253 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/parse_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.182485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    65763 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/container.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16500 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/errors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1711 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/opf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4436 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/parsing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9024 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/pretty.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15402 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/replace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19073 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/split.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33402 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/toc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7870 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29995 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32898 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/stylizer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.182485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5152 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/cover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/data_url.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/filenames.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29488 2023-07-12 13:37:24.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/flatcss.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/guide.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4362 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/htmltoc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2697 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/jacket.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4017 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/manglecase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8584 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/metadata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6433 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/page_margin.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9123 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/rasterize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3411 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/rescale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19536 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/split.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14974 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/structure.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11263 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/subset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2637 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/trimmanifest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2705 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/writer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.182485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2863 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8849 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader132.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5475 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader202.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/formatreader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/haodoo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/haodoo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/haodoo/reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2801 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/header.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/palmdoc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/palmdoc/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2288 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/palmdoc/reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/pdf/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/pdf/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/pdf/reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/plucker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/plucker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27494 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/plucker/reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ztxt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ztxt/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3074 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ztxt/reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5949 2023-07-05 09:23:28.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/pdftohtml.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/render/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/render/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6357 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/render/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.186485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1166 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf/input.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.190485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23172 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/ParseRtf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8911 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/add_brackets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3357 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/body_styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8129 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/border_parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   705801 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/char_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2429 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/check_brackets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/check_encoding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9538 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/colors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3469 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/combine_borders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10525 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/convert_to_tags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6372 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/default_encoding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8354 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/delete_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34875 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/field_strings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15252 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fields_large.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fields_small.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8971 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fonts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11089 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/footnote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2080 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/get_char_map.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10921 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/group_borders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8815 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/group_styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10622 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/header.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8278 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/headings_to_sections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22384 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/hex_2_utf8.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11696 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16638 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/inline.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/line_endings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7757 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/list_numbers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18231 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/list_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/make_lists.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5159 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/old_rtf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4096 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8345 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/override_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29733 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/paragraph_def.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10351 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/paragraphs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7236 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/pict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23025 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/preamble_div.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/preamble_rest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42075 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/process_tokens.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19958 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/sections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27721 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/styles.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20969 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3535 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/table_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/tokenize.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.190485 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38659 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/functions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7790 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/unsmarten.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.194486 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10479 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/markdownml.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/newlines.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11412 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19237 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/textileml.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/txtml.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.194486 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1709 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406462 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/jacodepoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1334 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/jadecoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406295 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/krcodepoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/krdecoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   187198 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/unicodepoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3978 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/unidecoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   406313 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/vncodepoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/vndecoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   405777 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/zhcodepoints.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.194486 ebook-converter-noimage-4.12.2/ebook_converter/library/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2515 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/library/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30056 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/library/field_metadata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-05 10:51:45.000000 ebook-converter-noimage-4.12.2/ebook_converter/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/polyglot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7424 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/ptempfile.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.194486 ebook-converter-noimage-4.12.2/ebook_converter/spell/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1802 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/spell/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.198485 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12224 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/color3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29516 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/css21.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9126 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/decoding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7592 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/fonts3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/media3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/page3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4442 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/parsing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.198485 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1052 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8336 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/color3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14313 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/css21.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3426 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/decoding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3022 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/fonts3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2909 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/media3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3770 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/page3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8808 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/tokenizing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13441 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/token_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7736 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tokenizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/tinycss/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/ebook_converter/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/cleantext.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9618 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22068 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/config_base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      408 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/directory.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      721 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/encoding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3344 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/entities.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13132 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/filenames.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4115 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/metadata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12951 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/scanner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1649 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11406 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11349 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/dict_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7734 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10242 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cmap.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7676 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6039 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/container.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      209 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/errors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3344 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/glyf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5802 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/gsub.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6671 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/head.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/kern.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3155 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/loca.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1575 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/maxp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12103 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/subset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17110 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14659 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/formatter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68191 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/formatter_functions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1355 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/html2text.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9060 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/icu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25367 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/img.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6097 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/imghdr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1409 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/iso8601.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3696 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10556 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/localunzip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/mreplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/resources.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3521 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1800 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/shared_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1928 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/short_uuid.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33107 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/smartypants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6712 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/speedups.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7489 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/terminal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/titlecase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/wordcount.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/xml_parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    64817 2023-07-05 08:58:17.000000 ebook-converter-noimage-4.12.2/ebook_converter/utils/zipfile.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 13:38:58.202486 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1207 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16333 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-07-12 13:38:58.000000 ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-07-12 13:38:58.206486 ebook-converter-noimage-4.12.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-07-05 15:03:15.000000 ebook-converter-noimage-4.12.2/setup.py
```

### Comparing `ebook-converter-noimage-4.12.1/LICENSE` & `ebook-converter-noimage-4.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/PKG-INFO` & `ebook-converter-noimage-4.12.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ebook-converter-noimage
-Version: 4.12.1
+Version: 4.12.2
 Summary: Convert ebook between different formats
 Home-page: https://github.com/gryf/ebook-converter
 Author: gryf
 Author-email: gryf73@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +20,7 @@
 License-File: LICENSE
 
  # ebook-converter
 This is a published wheel for the 3-year-unmaintained [ebook-converter](https://github.com/gryf/ebook-converter) project, developed by gryf.
 
 I (152334H) am merely publishing this wheel to PyPI so that I can use it in my own projects. It has a very slight modification: a hardcoded statement to ignore all images in all files. I was not responsible for 99.99% of the code present in the package.
     
-
```

### Comparing `ebook-converter-noimage-4.12.1/README.rst` & `ebook-converter-noimage-4.12.2/README.rst`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/constants.py` & `ebook-converter-noimage-4.12.2/ebook_converter/constants.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/constants_old.py` & `ebook-converter-noimage-4.12.2/ebook_converter/constants_old.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/ordered_set.py` & `ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/ordered_set.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/parser.py` & `ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/parser.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/select.py` & `ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/select.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/css_selectors/tests.py` & `ebook-converter-noimage-4.12.2/ebook_converter/css_selectors/tests.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/customize/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/customize/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/customize/builtins.py` & `ebook-converter-noimage-4.12.2/ebook_converter/customize/builtins.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/customize/conversion.py` & `ebook-converter-noimage-4.12.2/ebook_converter/customize/conversion.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/customize/profiles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/customize/profiles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/customize/ui.py` & `ebook-converter-noimage-4.12.2/ebook_converter/customize/ui.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/default_tweaks.py` & `ebook-converter-noimage-4.12.2/ebook_converter/data/default_tweaks.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/fb2.xsl` & `ebook-converter-noimage-4.12.2/ebook_converter/data/fb2.xsl`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/html.css` & `ebook-converter-noimage-4.12.2/ebook_converter/data/html.css`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/iso_639-3.json` & `ebook-converter-noimage-4.12.2/ebook_converter/data/iso_639-3.json`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/jacket/stylesheet.css` & `ebook-converter-noimage-4.12.2/ebook_converter/data/jacket/stylesheet.css`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/jacket/template.xhtml` & `ebook-converter-noimage-4.12.2/ebook_converter/data/jacket/template.xhtml`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/lrf.xsl` & `ebook-converter-noimage-4.12.2/ebook_converter/data/lrf.xsl`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/mime.types` & `ebook-converter-noimage-4.12.2/ebook_converter/data/mime.types`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/data/rtf.xsl` & `ebook-converter-noimage-4.12.2/ebook_converter/data/rtf.xsl`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/devices/interface.py` & `ebook-converter-noimage-4.12.2/ebook_converter/devices/interface.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/BeautifulSoup.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/BeautifulSoup.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/chardet.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/chardet.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/compression/palmdoc.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/compression/palmdoc.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/cli.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/azw4_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/azw4_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/chm_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/chm_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/comic_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/comic_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/djvu_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/djvu_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/docx_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/docx_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/docx_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/docx_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/epub_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/epub_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/epub_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/epub_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/fb2_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/fb2_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/fb2_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/fb2_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/html_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/html_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/html_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/html_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/htmlz_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/htmlz_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/htmlz_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/htmlz_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lit_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lit_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lit_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lit_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lrf_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lrf_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/lrf_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/lrf_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/mobi_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/mobi_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/mobi_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/mobi_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/odt_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/odt_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/oeb_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/oeb_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdb_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdb_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdb_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdb_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdf_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdf_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pdf_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pdf_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pml_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pml_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/pml_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/pml_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rb_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rb_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rb_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rb_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/recipe_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/recipe_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rtf_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rtf_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/rtf_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/rtf_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/snb_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/snb_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/snb_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/snb_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/tcr_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/tcr_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/tcr_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/tcr_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/txt_input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/txt_input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plugins/txt_output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plugins/txt_output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/plumber.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/plumber.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/preprocess.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/preprocess.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/conversion/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/covers.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/covers.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/block_styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/block_styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/char_styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/char_styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/cleanup.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/cleanup.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/container.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/container.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/dump.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/dump.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/fields.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/fields.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/fonts.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/fonts.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/footnotes.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/footnotes.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/images.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/images.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/index.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/index.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/names.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/names.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/numbering.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/numbering.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/settings.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/settings.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/tables.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/tables.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/theme.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/theme.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/to_html.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/to_html.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/toc.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/toc.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/container.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/container.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/fonts.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/fonts.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/from_html.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/from_html.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/images.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/images.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/links.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/links.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/lists.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/lists.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/tables.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/tables.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/docx/writer/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/docx/writer/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/epub/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/epub/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/fb2/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/fb2/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/fb2/fb2ml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/fb2/fb2ml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html/to_zip.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html/to_zip.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/html_entities.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/html_entities.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/htmlz/oeb2html.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/htmlz/oeb2html.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/fonts.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/fonts.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/color_map.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/color_map.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/convert_from.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/convert_from.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/html/table.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/html/table.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/lrfparser.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/lrfparser.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/meta.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/meta.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/objects.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/objects.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/elements.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/elements.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrfopt.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrfopt.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/pylrs/pylrs.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/pylrs/pylrs.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/lrf/tags.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/lrf/tags.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/archive.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/archive.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/base.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/base.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/formatter.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/formatter.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/book/json_codec.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/book/json_codec.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/fb2.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/fb2.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/html.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/html.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/meta.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/meta.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/odt.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/odt.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/opf2.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/opf2.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/opf3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/opf3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/pdf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/pdf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/rtf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/rtf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/toc.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/toc.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/txt.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/txt.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/metadata/xmp.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/metadata/xmp.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/huffcdic.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/huffcdic.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/langcodes.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/langcodes.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/mobiml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/mobiml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/containers.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/containers.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/headers.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/headers.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/index.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/index.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/markup.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/markup.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/mobi6.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/mobi6.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/mobi8.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/mobi8.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/reader/ncx.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/reader/ncx.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/tweak.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/tweak.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/indexer.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/indexer.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/main.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/main.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/resources.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/resources.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer2/serializer.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer2/serializer.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/cleanup.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/cleanup.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/mobi/writer8/exth.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/mobi/writer8/exth.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/odt/input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/odt/input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/base.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/base.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/normalize_css.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/normalize_css.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/parse_utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/parse_utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/container.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/container.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/css.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/css.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/opf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/opf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/parsing.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/parsing.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/pretty.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/pretty.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/replace.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/replace.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/split.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/split.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/toc.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/toc.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/polish/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/polish/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/stylizer.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/stylizer.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/cover.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/cover.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/data_url.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/data_url.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/filenames.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/filenames.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/flatcss.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/flatcss.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from ebook_converter.ebooks.oeb.stylizer import Stylizer
 from ebook_converter.utils.filenames import ascii_filename, ascii_text
 
 
 COLLAPSE = re.compile(r'[ \t\r\n\v]+')
 STRIPNUM = re.compile(r'[-0-9]+$')
 
-
+def find_direct_child_tag(html, t: str):
+    return html.xpath(f'./*[local-name()="{t}"]')[0]
 def asfloat(value, default):
     if not isinstance(value, numbers.Number):
         value = default
     return float(value)
 
 
 class KeyMapper(object):
@@ -271,15 +272,16 @@
 
     def stylize_spine(self):
         self.stylizers = {}
         profile = self.context.source
         css = ''
         for item in self.items:
             html = item.data
-            body = html.find(base.tag('xhtml', 'body'))
+            #body = html.find(base.tag('xhtml', 'body'))
+            body = find_direct_child_tag(html,'body')
             if 'style' in html.attrib:
                 b = body.attrib.get('style', '')
                 body.set('style',  html.get('style') + ';' + b)
                 del html.attrib['style']
             bs = body.get('style', '').split(';')
             bs.append('margin-top: 0pt')
             bs.append('margin-bottom: 0pt')
@@ -312,15 +314,16 @@
                 sizes[csize] += len(COLLAPSE.sub(' ', child.tail))
 
     def baseline_spine(self):
         sizes = collections.defaultdict(float)
         for item in self.items:
             html = item.data
             stylizer = self.stylizers[item]
-            body = html.find(base.tag('xhtml', 'body'))
+            # body = html.find(base.tag('xhtml', 'body'))
+            body = find_direct_child_tag(html, 'body')
             fsize = self.context.source.fbase
             self.baseline_node(body, stylizer, sizes, fsize)
         try:
             sbase = max(list(sizes.items()), key=operator.itemgetter(1))[0]
         except:
             sbase = 12.0
         self.oeb.logger.info("Source base font size is %0.05fpt", sbase)
@@ -371,14 +374,15 @@
                     # which text-align does not. And the ever trustworthy Word
                     # uses this construct in its HTML output. See
                     # https://bugs.launchpad.net/bugs/1569583
                     if tag == 'table':
                         if 'margin-left' not in cssdict and 'margin-right' not in cssdict:
                             cssdict['margin-left'] = cssdict['margin-right'] = 'auto'
                     else:
+                        # TODO possibly fix
                         for table in node.iterchildren(base.tag('xhtml', "table")):
                             ts = stylizer.style(table)
                             if ts.get('margin-left') is None and ts.get('margin-right') is None:
                                 ts.set('margin-left', 'auto')
                                 ts.set('margin-right', 'auto')
             else:
                 val = node.attrib['align']
@@ -570,15 +574,16 @@
             del node.attrib['style']
         if recurse:
             for child in node:
                 self.flatten_node(child, stylizer, names, styles, pseudo_styles, psize, item_id)
 
     def flatten_head(self, item, href, global_href):
         html = item.data
-        head = html.find(base.tag('xhtml', 'head'))
+        #head = html.find(base.tag('xhtml', 'head'))
+        head = find_direct_child_tag(html, 'head')
 
         def safe_lower(x):
             try:
                 x = x.lower()
             except Exception:
                 pass
             return x
@@ -658,15 +663,16 @@
         for item in self.items:
             html = item.data
             stylizer = self.stylizers[item]
             if self.specializer is not None:
                 self.specializer(item, stylizer)
             fsize = self.context.dest.fbase
             self.flatten_node(html, stylizer, names, styles, pseudo_styles, fsize, item.id, recurse=False)
-            self.flatten_node(html.find(base.tag('xhtml', 'body')), stylizer, names, styles, pseudo_styles, fsize, item.id)
+            #self.flatten_node(html.find(base.tag('xhtml', 'body')), stylizer, names, styles, pseudo_styles, fsize, item.id)
+            self.flatten_node(find_direct_child_tag(html, 'body'), stylizer, names, styles, pseudo_styles, fsize, item.id)
         items = sorted(((key, val) for (val, key) in styles.items()))
         # :hover must come after link and :active must come after :hover
         psels = sorted(pseudo_styles, key=lambda x :
                 {'hover':1, 'active':2}.get(x, 0))
         for psel in psels:
             styles = pseudo_styles[psel]
             if not styles:
```

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/guide.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/guide.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/htmltoc.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/htmltoc.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/jacket.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/jacket.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/manglecase.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/manglecase.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/metadata.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/metadata.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/page_margin.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/page_margin.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/rasterize.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/rasterize.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/rescale.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/rescale.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/split.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/split.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/structure.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/structure.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/subset.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/subset.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/transforms/trimmanifest.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/transforms/trimmanifest.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/oeb/writer.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/oeb/writer.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader132.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader132.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ereader/reader202.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ereader/reader202.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/haodoo/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/haodoo/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/header.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/header.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/palmdoc/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/palmdoc/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/pdf/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/pdf/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/plucker/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/plucker/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdb/ztxt/reader.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdb/ztxt/reader.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/pdftohtml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/pdftohtml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/pdf/render/common.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/pdf/render/common.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf/input.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf/input.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/ParseRtf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/ParseRtf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/add_brackets.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/add_brackets.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/body_styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/body_styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/border_parse.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/border_parse.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/char_set.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/char_set.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/check_brackets.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/check_brackets.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/check_encoding.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/check_encoding.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/colors.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/colors.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/combine_borders.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/combine_borders.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/convert_to_tags.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/convert_to_tags.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/copy.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/copy.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/default_encoding.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/default_encoding.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/delete_info.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/delete_info.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/field_strings.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/field_strings.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fields_large.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fields_large.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fields_small.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fields_small.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/fonts.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/fonts.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/footnote.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/footnote.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/get_char_map.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/get_char_map.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/group_borders.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/group_borders.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/group_styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/group_styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/header.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/header.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/headings_to_sections.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/headings_to_sections.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/hex_2_utf8.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/hex_2_utf8.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/info.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/info.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/inline.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/inline.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/line_endings.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/line_endings.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/list_numbers.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/list_numbers.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/list_table.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/list_table.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/make_lists.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/make_lists.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/old_rtf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/old_rtf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/output.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/output.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/override_table.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/override_table.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/paragraph_def.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/paragraph_def.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/paragraphs.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/paragraphs.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/pict.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/pict.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/preamble_div.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/preamble_div.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/preamble_rest.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/preamble_rest.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/process_tokens.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/process_tokens.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/sections.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/sections.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/styles.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/styles.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/table.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/table.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/table_info.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/table_info.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/rtf2xml/tokenize.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/rtf2xml/tokenize.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/functions.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/functions.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/textile/unsmarten.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/textile/unsmarten.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/markdownml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/markdownml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/newlines.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/newlines.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/processor.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/processor.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/textileml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/textileml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/txt/txtml.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/txt/txtml.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/jacodepoints.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/jacodepoints.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/jadecoder.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/jadecoder.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/krcodepoints.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/krcodepoints.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/krdecoder.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/krdecoder.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/unicodepoints.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/unicodepoints.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/unidecoder.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/unidecoder.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/vncodepoints.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/vncodepoints.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/vndecoder.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/vndecoder.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ebooks/unihandecode/zhcodepoints.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ebooks/unihandecode/zhcodepoints.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/library/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/library/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/library/field_metadata.py` & `ebook-converter-noimage-4.12.2/ebook_converter/library/field_metadata.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/logging.py` & `ebook-converter-noimage-4.12.2/ebook_converter/logging.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/main.py` & `ebook-converter-noimage-4.12.2/ebook_converter/main.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/polyglot.py` & `ebook-converter-noimage-4.12.2/ebook_converter/polyglot.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/ptempfile.py` & `ebook-converter-noimage-4.12.2/ebook_converter/ptempfile.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/spell/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/spell/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/color3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/color3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/css21.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/css21.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/decoding.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/decoding.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/fonts3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/fonts3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/media3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/media3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/page3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/page3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/parsing.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/parsing.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/color3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/color3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/css21.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/css21.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/decoding.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/decoding.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/fonts3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/fonts3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/main.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/main.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/media3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/media3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/page3.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/page3.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tests/tokenizing.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tests/tokenizing.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/token_data.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/token_data.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/tinycss/tokenizer.py` & `ebook-converter-noimage-4.12.2/ebook_converter/tinycss/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/cleantext.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/cleantext.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/config.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/config.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/config_base.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/config_base.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/date.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/date.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/encoding.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/entities.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/entities.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/filenames.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/filenames.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/metadata.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/metadata.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/scanner.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/scanner.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/__init__.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/__init__.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/constants.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/constants.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/dict_data.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/dict_data.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cff/table.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cff/table.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/cmap.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/cmap.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/common.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/common.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/container.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/container.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/glyf.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/glyf.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/gsub.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/gsub.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/head.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/head.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/kern.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/kern.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/loca.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/loca.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/maxp.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/maxp.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/sfnt/subset.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/sfnt/subset.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/fonts/utils.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/fonts/utils.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/formatter.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/formatter_functions.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/formatter_functions.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/html2text.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/html2text.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/icu.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/icu.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/img.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/img.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/imghdr.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/imghdr.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/iso8601.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/localization.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/localization.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/localunzip.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/localunzip.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/mreplace.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/mreplace.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/resources.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/resources.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/serialize.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/shared_file.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/shared_file.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/short_uuid.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/short_uuid.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/smartypants.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/smartypants.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/speedups.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/speedups.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/terminal.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/titlecase.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/titlecase.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/wordcount.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/wordcount.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/xml_parse.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/xml_parse.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter/utils/zipfile.py` & `ebook-converter-noimage-4.12.2/ebook_converter/utils/zipfile.py`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/PKG-INFO` & `ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ebook-converter-noimage
-Version: 4.12.1
+Version: 4.12.2
 Summary: Convert ebook between different formats
 Home-page: https://github.com/gryf/ebook-converter
 Author: gryf
 Author-email: gryf73@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +20,7 @@
 License-File: LICENSE
 
  # ebook-converter
 This is a published wheel for the 3-year-unmaintained [ebook-converter](https://github.com/gryf/ebook-converter) project, developed by gryf.
 
 I (152334H) am merely publishing this wheel to PyPI so that I can use it in my own projects. It has a very slight modification: a hardcoded statement to ignore all images in all files. I was not responsible for 99.99% of the code present in the package.
     
-
```

### Comparing `ebook-converter-noimage-4.12.1/ebook_converter_noimage.egg-info/SOURCES.txt` & `ebook-converter-noimage-4.12.2/ebook_converter_noimage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebook-converter-noimage-4.12.1/setup.cfg` & `ebook-converter-noimage-4.12.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ebook-converter-noimage
-version = 4.12.1
+version = 4.12.2
 summary = Convert ebook between different formats
 description-file = 
 	README.rst
 author = gryf
 author-email = gryf73@gmail.com
 license = GPL3
 license_file = LICENSE
@@ -21,26 +21,26 @@
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	filelock
-	python-dateutil
+	beautifulsoup4>=4.9.3
+	css-parser>=1.0.6
+	filelock>=3.0.12
+	html2text>=2020.1.16
+	html5-parser==0.4.9
 	lxml
-	css-parser
-	beautifulsoup4
-	tinycss
-	pillow
-	msgpack
-	html5-parser
-	odfpy
-	setuptools
-	html2text
+	msgpack>=1.0.0
+	odfpy>=1.4.1
+	pillow>=8.0.1
+	python-dateutil>=2.8.1
+	setuptools>=50.3.2
+	tinycss>=0.4
 
 [options.entry_points]
 console_scripts = 
 	ebook-converter=ebook_converter.main:main
 
 [options.package_data]
 * = *.types *.css, *.html, *.xsl
```

### Comparing `ebook-converter-noimage-4.12.1/setup.py` & `ebook-converter-noimage-4.12.2/setup.py`

 * *Files identical despite different names*

