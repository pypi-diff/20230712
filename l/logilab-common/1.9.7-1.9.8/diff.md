# Comparing `tmp/logilab-common-1.9.7.tar.gz` & `tmp/logilab-common-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logilab-common-1.9.7.tar", last modified: Tue Jun  7 14:22:58 2022, max compression
+gzip compressed data, was "logilab-common-1.9.8.tar", last modified: Wed Jan  4 22:32:54 2023, max compression
```

## Comparing `logilab-common-1.9.7.tar` & `logilab-common-1.9.8.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.951329 logilab-common-1.9.7/
--rw-rw-rw-   0 root         (0) root         (0)    17987 2022-06-07 14:22:37.000000 logilab-common-1.9.7/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2022-06-07 14:22:37.000000 logilab-common-1.9.7/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)    46847 2022-06-07 14:22:37.000000 logilab-common-1.9.7/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-06-07 14:22:37.000000 logilab-common-1.9.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2805 2022-06-07 14:22:58.951329 logilab-common-1.9.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2268 2022-06-07 14:22:37.000000 logilab-common-1.9.7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1992 2022-06-07 14:22:37.000000 logilab-common-1.9.7/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-06-07 14:22:37.000000 logilab-common-1.9.7/announce.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.891328 logilab-common-1.9.7/bin/
--rwxrwxrwx   0 root         (0) root         (0)      138 2022-06-07 14:22:37.000000 logilab-common-1.9.7/bin/logilab-pytest
--rw-rw-rw-   0 root         (0) root         (0)      351 2022-06-07 14:22:37.000000 logilab-common-1.9.7/bin/logilab-pytest.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.895328 logilab-common-1.9.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     5621 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4144 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/logilab-pytest.1
--rw-rw-rw-   0 root         (0) root         (0)     6086 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/logilab.common.rst
--rw-rw-rw-   0 root         (0) root         (0)     1019 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/logilab.common.ureports.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/logilab.rst
--rw-rw-rw-   0 root         (0) root         (0)      755 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-07 14:22:37.000000 logilab-common-1.9.7/docs/requirements-doc.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.895328 logilab-common-1.9.7/logilab/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.911328 logilab-common-1.9.7/logilab/common/
--rw-rw-rw-   0 root         (0) root         (0)     5559 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3787 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     8655 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/changelog.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/clcommands.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/compat.py
--rw-rw-rw-   0 root         (0) root         (0)    46872 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/daemon.py
--rw-rw-rw-   0 root         (0) root         (0)    12080 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/date.py
--rw-rw-rw-   0 root         (0) root         (0)     7146 2022-06-07 14:22:37.000000 logilab-common-1.9.7/logilab/common/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     9795 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    27229 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)    12982 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2644 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     6692 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/logging_ext.py
--rw-rw-rw-   0 root         (0) root         (0)    27108 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/modutils.py
--rw-rw-rw-   0 root         (0) root         (0)    16325 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/optik_ext.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/optparser.py
--rw-rw-rw-   0 root         (0) root         (0)     9111 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/proc.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    53429 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/pytest.py
--rw-rw-rw-   0 root         (0) root         (0)    47142 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12888 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/shellutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/sphinx_ext.py
--rw-rw-rw-   0 root         (0) root         (0)     4367 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/sphinxutils.py
--rw-rw-rw-   0 root         (0) root         (0)    33629 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/table.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/tasksqueue.py
--rw-rw-rw-   0 root         (0) root         (0)    25286 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/testlib.py
--rw-rw-rw-   0 root         (0) root         (0)    18518 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/textutils.py
--rw-rw-rw-   0 root         (0) root         (0)    11668 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/tree.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/types.py
--rw-rw-rw-   0 root         (0) root         (0)     6644 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/umessage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.911328 logilab-common-1.9.7/logilab/common/ureports/
--rw-rw-rw-   0 root         (0) root         (0)     8042 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/ureports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/ureports/docbook_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     5165 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/ureports/html_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     6785 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/ureports/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     5597 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/ureports/text_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/urllib2ext.py
--rw-rw-rw-   0 root         (0) root         (0)     7227 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/vcgutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3824 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/visitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2022-06-07 14:22:38.000000 logilab-common-1.9.7/logilab/common/xmlutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.915328 logilab-common-1.9.7/logilab_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2805 2022-06-07 14:22:57.000000 logilab-common-1.9.7/logilab_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4097 2022-06-07 14:22:58.000000 logilab-common-1.9.7/logilab_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-07 14:22:57.000000 logilab-common-1.9.7/logilab_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-06-07 14:22:58.000000 logilab-common-1.9.7/logilab_common.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-06-07 14:22:58.000000 logilab-common-1.9.7/logilab_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-06-07 14:22:58.000000 logilab-common-1.9.7/logilab_common.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      254 2022-06-07 14:22:38.000000 logilab-common-1.9.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-07 14:22:38.000000 logilab-common-1.9.7/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-06-07 14:22:58.951329 logilab-common-1.9.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2307 2022-06-07 14:22:38.000000 logilab-common-1.9.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.923328 logilab-common-1.9.7/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.931329 logilab-common-1.9.7/test/data/
--rw-rw-rw-   0 root         (0) root         (0)     3834 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)     1222 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/MyPyPa-0.1.0-py2.5.egg
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/MyPyPa-0.1.0.zip
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1880 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.931329 logilab-common-1.9.7/test/data/content_differ_dir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/content_differ_dir/NOTHING
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/content_differ_dir/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.931329 logilab-common-1.9.7/test/data/content_differ_dir/subdir/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/content_differ_dir/subdir/coin
--rw-rw-rw-   0 root         (0) root         (0)     3159 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/content_differ_dir/subdir/toto.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/deprecation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.931329 logilab-common-1.9.7/test/data/file_differ_dir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/file_differ_dir/NOTHING
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/file_differ_dir/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.931329 logilab-common-1.9.7/test/data/file_differ_dir/subdir/
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/file_differ_dir/subdir/toto.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.935329 logilab-common-1.9.7/test/data/file_differ_dir/subdirtwo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/file_differ_dir/subdirtwo/Hello
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.939329 logilab-common-1.9.7/test/data/find_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/foo.txt
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/module.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/module2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/newlines.txt
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/noendingnewline.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/nonregr.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/normal_file.txt
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/spam.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.939329 logilab-common-1.9.7/test/data/find_test/sub/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/sub/doc.txt
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/sub/momo.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/test.ini
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/test1.msg
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/test2.msg
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/find_test/write_protected_file.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/foo.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.939329 logilab-common-1.9.7/test/data/lmfp/
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/lmfp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/lmfp/foo.py
--rw-rw-rw-   0 root         (0) root         (0)     1402 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/module.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/module2.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/newlines.txt
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/noendingnewline.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/nonregr.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/normal_file.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.939329 logilab-common-1.9.7/test/data/reference_dir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/reference_dir/NOTHING
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/reference_dir/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.939329 logilab-common-1.9.7/test/data/reference_dir/subdir/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/reference_dir/subdir/coin
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/reference_dir/subdir/toto.txt
--rw-rw-rw-   0 root         (0) root         (0)      600 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/regobjects.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/regobjects2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.947329 logilab-common-1.9.7/test/data/same_dir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/same_dir/NOTHING
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/same_dir/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.947329 logilab-common-1.9.7/test/data/same_dir/subdir/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/same_dir/subdir/coin
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/same_dir/subdir/toto.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/spam.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.947329 logilab-common-1.9.7/test/data/sub/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/sub/doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/sub/momo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.951329 logilab-common-1.9.7/test/data/subdir_differ_dir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/subdir_differ_dir/NOTHING
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/subdir_differ_dir/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-07 14:22:58.951329 logilab-common-1.9.7/test/data/subdir_differ_dir/subdir/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/subdir_differ_dir/subdir/coin
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/subdir_differ_dir/subdir/toto.txt
--rw-rw-rw-   0 root         (0) root         (0)      178 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/test.ini
--rw-rw-rw-   0 root         (0) root         (0)      928 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/test1.msg
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/test2.msg
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/data/write_protected_file.txt
--rw-rw-rw-   0 root         (0) root         (0)     5453 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_changelog.py
--rw-rw-rw-   0 root         (0) root         (0)    16051 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     8603 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_date.py
--rw-rw-rw-   0 root         (0) root         (0)     7053 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    40204 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_interface.py
--rw-rw-rw-   0 root         (0) root         (0)    11963 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_modutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     9846 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_shellutils.py
--rw-rw-rw-   0 root         (0) root         (0)    17907 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2692 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_taskqueue.py
--rw-rw-rw-   0 root         (0) root         (0)    30142 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)    11874 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_textutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9465 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_tree.py
--rw-rw-rw-   0 root         (0) root         (0)     3355 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_umessage.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_ureports_html.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_ureports_text.py
--rw-rw-rw-   0 root         (0) root         (0)     2744 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/test_xmlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3517 2022-06-07 14:22:38.000000 logilab-common-1.9.7/test/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2022-06-07 14:22:38.000000 logilab-common-1.9.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.126615 logilab-common-1.9.8/
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2023-01-04 22:32:31.000000 logilab-common-1.9.8/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2023-01-04 22:32:31.000000 logilab-common-1.9.8/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)    46847 2023-01-04 22:32:31.000000 logilab-common-1.9.8/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-01-04 22:32:31.000000 logilab-common-1.9.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-01-04 22:32:54.126615 logilab-common-1.9.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2023-01-04 22:32:31.000000 logilab-common-1.9.8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2023-01-04 22:32:31.000000 logilab-common-1.9.8/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-01-04 22:32:31.000000 logilab-common-1.9.8/announce.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.070614 logilab-common-1.9.8/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      138 2023-01-04 22:32:31.000000 logilab-common-1.9.8/bin/logilab-pytest
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-01-04 22:32:31.000000 logilab-common-1.9.8/bin/logilab-pytest.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.074614 logilab-common-1.9.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5621 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/logilab-pytest.1
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/logilab.common.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/logilab.common.ureports.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/logilab.rst
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-01-04 22:32:31.000000 logilab-common-1.9.8/docs/requirements-doc.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.074614 logilab-common-1.9.8/logilab/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.094615 logilab-common-1.9.8/logilab/common/
+-rw-rw-rw-   0 root         (0) root         (0)     5559 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3787 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     8655 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/changelog.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/clcommands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)    46872 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)    12080 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/date.py
+-rw-rw-rw-   0 root         (0) root         (0)     7146 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     9795 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)    27435 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12982 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2644 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     6692 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/logging_ext.py
+-rw-rw-rw-   0 root         (0) root         (0)    27108 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/modutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16325 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/optik_ext.py
+-rw-rw-rw-   0 root         (0) root         (0)     3330 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/optparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9111 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    53429 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)    47142 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12888 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/shellutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/sphinx_ext.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/sphinxutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    33628 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/tasksqueue.py
+-rw-rw-rw-   0 root         (0) root         (0)    25284 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    18518 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/textutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11668 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/umessage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.094615 logilab-common-1.9.8/logilab/common/ureports/
+-rw-rw-rw-   0 root         (0) root         (0)     8043 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/ureports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5727 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/ureports/docbook_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5165 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/ureports/html_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6784 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/ureports/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5597 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/ureports/text_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/urllib2ext.py
+-rw-rw-rw-   0 root         (0) root         (0)     7227 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/vcgutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/visitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2023-01-04 22:32:31.000000 logilab-common-1.9.8/logilab/common/xmlutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.098615 logilab-common-1.9.8/logilab_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-01-04 22:32:53.000000 logilab-common-1.9.8/logilab_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-01-04 22:32:54.000000 logilab-common-1.9.8/logilab_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 22:32:53.000000 logilab-common-1.9.8/logilab_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-01-04 22:32:53.000000 logilab-common-1.9.8/logilab_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-01-04 22:32:53.000000 logilab-common-1.9.8/logilab_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-01-04 22:32:53.000000 logilab-common-1.9.8/logilab_common.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-01-04 22:32:31.000000 logilab-common-1.9.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-01-04 22:32:31.000000 logilab-common-1.9.8/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-01-04 22:32:54.126615 logilab-common-1.9.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2023-01-04 22:32:31.000000 logilab-common-1.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.106615 logilab-common-1.9.8/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/MyPyPa-0.1.0-py2.5.egg
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/MyPyPa-0.1.0.zip
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/content_differ_dir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/content_differ_dir/NOTHING
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/content_differ_dir/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/content_differ_dir/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/content_differ_dir/subdir/coin
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/content_differ_dir/subdir/toto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/deprecation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/file_differ_dir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/file_differ_dir/NOTHING
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/file_differ_dir/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/file_differ_dir/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/file_differ_dir/subdir/toto.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.114615 logilab-common-1.9.8/test/data/file_differ_dir/subdirtwo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/file_differ_dir/subdirtwo/Hello
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.118615 logilab-common-1.9.8/test/data/find_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/foo.txt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/module.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/module2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/newlines.txt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/noendingnewline.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/nonregr.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/normal_file.txt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/spam.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.118615 logilab-common-1.9.8/test/data/find_test/sub/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/sub/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/sub/momo.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/test.ini
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/test1.msg
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/test2.msg
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/find_test/write_protected_file.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/foo.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.118615 logilab-common-1.9.8/test/data/lmfp/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/lmfp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/lmfp/foo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/module2.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/newlines.txt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/noendingnewline.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/nonregr.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/normal_file.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/reference_dir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/reference_dir/NOTHING
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/reference_dir/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/reference_dir/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/reference_dir/subdir/coin
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/reference_dir/subdir/toto.txt
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/regobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/regobjects2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/same_dir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/same_dir/NOTHING
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/same_dir/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/same_dir/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/same_dir/subdir/coin
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/same_dir/subdir/toto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/spam.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/sub/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/sub/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/sub/momo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.122615 logilab-common-1.9.8/test/data/subdir_differ_dir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/subdir_differ_dir/NOTHING
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/subdir_differ_dir/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 22:32:54.126615 logilab-common-1.9.8/test/data/subdir_differ_dir/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/subdir_differ_dir/subdir/coin
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/subdir_differ_dir/subdir/toto.txt
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/test.ini
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/test1.msg
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/test2.msg
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/data/write_protected_file.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5453 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_changelog.py
+-rw-rw-rw-   0 root         (0) root         (0)    16051 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     8603 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     7053 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)    40203 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6002 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11963 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_modutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     9846 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_shellutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    17907 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_taskqueue.py
+-rw-rw-rw-   0 root         (0) root         (0)    30142 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    11874 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_textutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9465 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     3355 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_umessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_ureports_html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_ureports_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     2744 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/test_xmlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2023-01-04 22:32:31.000000 logilab-common-1.9.8/test/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-01-04 22:32:31.000000 logilab-common-1.9.8/tox.ini
```

### Comparing `logilab-common-1.9.7/COPYING` & `logilab-common-1.9.8/COPYING`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/COPYING.LESSER` & `logilab-common-1.9.8/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/ChangeLog` & `logilab-common-1.9.8/ChangeLog`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/MANIFEST.in` & `logilab-common-1.9.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/PKG-INFO` & `logilab-common-1.9.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logilab-common
-Version: 1.9.7
+Version: 1.9.8
 Summary: collection of low-level Python packages and modules used by Logilab projects
 Home-page: http://www.logilab.org/project/logilab-common
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
```

### Comparing `logilab-common-1.9.7/README.rst` & `logilab-common-1.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/__pkginfo__.py` & `logilab-common-1.9.8/__pkginfo__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,23 +17,22 @@
 # along with logilab-common.  If not, see <http://www.gnu.org/licenses/>.
 
 """logilab.common packaging information"""
 
 __docformat__ = "restructuredtext en"
 
 import os
-import sys
 from os.path import join
 
 distname = "logilab-common"
 modname = "common"
 subpackage_of = "logilab"
 subpackage_master = True
 
-numversion = (1, 9, 7)
+numversion = (1, 9, 8)
 version = ".".join([str(num) for num in numversion])
 
 license = "LGPL"  # 2.1 or later
 description = "collection of low-level Python packages and modules" " used by Logilab projects"
 web = "http://www.logilab.org/project/%s" % distname
 mailinglist = "mailto://python-projects@lists.logilab.org"
 author = "Logilab"
@@ -43,25 +42,23 @@
 scripts = [join("bin", "logilab-pytest")]
 include_dirs = [join("test", "data")]
 
 __depends__ = {
     "setuptools": None,
     "mypy-extensions": None,
     "typing_extensions": None,
+    "importlib_metadata": ">=6,<7",
 }
 tests_require = [
     "pytz",
     "egenix-mx-base",
 ]
 
 if os.name == "nt":
     __depends__["colorama"] = None
 
-if sys.version_info < (3, 8):
-    __depends__["importlib_metadata"] = None
-
 classifiers = [
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
```

### Comparing `logilab-common-1.9.7/docs/Makefile` & `logilab-common-1.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/conf.py` & `logilab-common-1.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/index.rst` & `logilab-common-1.9.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/logilab-pytest.1` & `logilab-common-1.9.8/docs/logilab-pytest.1`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/logilab.common.rst` & `logilab-common-1.9.8/docs/logilab.common.rst`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/logilab.common.ureports.rst` & `logilab-common-1.9.8/docs/logilab.common.ureports.rst`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/docs/make.bat` & `logilab-common-1.9.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/__init__.py` & `logilab-common-1.9.8/logilab/common/__init__.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/cache.py` & `logilab-common-1.9.8/logilab/common/cache.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/changelog.py` & `logilab-common-1.9.8/logilab/common/changelog.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/clcommands.py` & `logilab-common-1.9.8/logilab/common/clcommands.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/compat.py` & `logilab-common-1.9.8/logilab/common/compat.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/configuration.py` & `logilab-common-1.9.8/logilab/common/configuration.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/daemon.py` & `logilab-common-1.9.8/logilab/common/daemon.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/date.py` & `logilab-common-1.9.8/logilab/common/date.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/debugger.py` & `logilab-common-1.9.8/logilab/common/debugger.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/decorators.py` & `logilab-common-1.9.8/logilab/common/decorators.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/deprecation.py` & `logilab-common-1.9.8/logilab/common/deprecation.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
     import importlib_metadata
 
 
+class FakeDistribution(importlib_metadata.Distribution):
+    "see https://github.com/python/importlib_metadata/blob/main/CHANGES.rst#v600"
+
+    def locate_file(self):
+        pass
+
+    def read_text(self):
+        pass
+
+
 def _unstack_all_deprecation_decorators(function):
     """
     This is another super edge magic case which is needed because we uses
     lazy_wraps because of logilab.common.modutils.LazyObject and because
     __name__ has special behavior and doesn't work like a normal attribute and
     that __getattribute__ of lazy_wraps is bypassed.
 
@@ -168,15 +178,15 @@
     global _cached_path_to_package
 
     if _cached_path_to_package is None:
         _cached_path_to_package = {}
         # mypy fails to understand the result of .discover(): Cannot
         # instantiate abstract class 'Distribution' with abstract attributes
         # 'locate_file' and 'read_text'
-        for distribution in importlib_metadata.Distribution().discover():  # type: ignore
+        for distribution in FakeDistribution().discover():  # type: ignore
             # sometime distribution has a "name" attribute, sometime not
             if distribution.files and hasattr(distribution, "name"):
                 for file in distribution.files:
                     _cached_path_to_package[str(distribution.locate_file(file))] = distribution.name
                 continue
 
             if distribution.files and "name" in distribution.metadata:
```

### Comparing `logilab-common-1.9.7/logilab/common/fileutils.py` & `logilab-common-1.9.8/logilab/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/graph.py` & `logilab-common-1.9.8/logilab/common/graph.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/interface.py` & `logilab-common-1.9.8/logilab/common/interface.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/logging_ext.py` & `logilab-common-1.9.8/logilab/common/logging_ext.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/modutils.py` & `logilab-common-1.9.8/logilab/common/modutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/optik_ext.py` & `logilab-common-1.9.8/logilab/common/optik_ext.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/optparser.py` & `logilab-common-1.9.8/logilab/common/optparser.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/proc.py` & `logilab-common-1.9.8/logilab/common/proc.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/pytest.py` & `logilab-common-1.9.8/logilab/common/pytest.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/registry.py` & `logilab-common-1.9.8/logilab/common/registry.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/shellutils.py` & `logilab-common-1.9.8/logilab/common/shellutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/sphinx_ext.py` & `logilab-common-1.9.8/logilab/common/sphinx_ext.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/sphinxutils.py` & `logilab-common-1.9.8/logilab/common/sphinxutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/table.py` & `logilab-common-1.9.8/logilab/common/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,14 @@
         return "\n".join(lines)
 
 
 class TableStyle:
     """Defines a table's style"""
 
     def __init__(self, table: Table) -> None:
-
         self._table = table
         self.size = dict([(col_name, "1*") for col_name in table.col_names])
         # __row_column__ is a special key to define the first column which
         # actually has no name (<=> left most column <=> row names column)
         self.size["__row_column__"] = "1*"
         self.alignment = dict([(col_name, "right") for col_name in table.col_names])
         self.alignment["__row_column__"] = "right"
```

### Comparing `logilab-common-1.9.7/logilab/common/tasksqueue.py` & `logilab-common-1.9.8/logilab/common/tasksqueue.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/testlib.py` & `logilab-common-1.9.8/logilab/common/testlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
         return proxy
 
     else:
 
         @wraps(callable)
         def proxy(*args: Any, **kargs: Any) -> Any:
-
             old_tmpdir = tempfile.gettempdir()
             new_tmpdir = tempfile.mkdtemp(prefix="temp-lgc-")
             tempfile.tempdir = new_tmpdir
             try:
                 return callable(*args, **kargs)
             finally:
                 try:
@@ -130,15 +129,14 @@
 
 
 def in_tempdir(callable):
     """A decorator moving the enclosed function inside the tempfile.tempfdir"""
 
     @wraps(callable)
     def proxy(*args, **kargs):
-
         old_cwd = os.getcwd()
         os.chdir(tempfile.tempdir)
         try:
             return callable(*args, **kargs)
         finally:
             os.chdir(old_cwd)
```

### Comparing `logilab-common-1.9.7/logilab/common/textutils.py` & `logilab-common-1.9.8/logilab/common/textutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/tree.py` & `logilab-common-1.9.8/logilab/common/tree.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/types.py` & `logilab-common-1.9.8/logilab/common/types.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/umessage.py` & `logilab-common-1.9.8/logilab/common/umessage.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/ureports/__init__.py` & `logilab-common-1.9.8/logilab/common/ureports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 
     def compute_content(self, layout: VNode) -> Generator[str, Any, None]:
         """trick to compute the formatting of children layout before actually
         writing it
 
         return an iterator on strings (one for each child element)
         """
+
         # use cells !
         def write(data: str) -> None:
             try:
                 stream.write(data)
             except UnicodeEncodeError:
                 # mypy: Argument 1 to "write" of "TextIOWrapper" has incompatible type "bytes";
                 # mypy: expected "str"
```

### Comparing `logilab-common-1.9.7/logilab/common/ureports/docbook_writer.py` & `logilab-common-1.9.8/logilab/common/ureports/docbook_writer.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/ureports/html_writer.py` & `logilab-common-1.9.8/logilab/common/ureports/html_writer.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/ureports/nodes.py` & `logilab-common-1.9.8/logilab/common/ureports/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         children: Union[
             TypingList["Text"],
             Tuple[Union["Paragraph", str], Union[TypingList, str]],
             Tuple[str, ...],
         ] = (),
         **kwargs: Any,
     ) -> None:
-
         super(BaseLayout, self).__init__(**kwargs)
 
         for child in children:
             if isinstance(child, BaseComponent):
                 self.append(child)
             else:
                 # mypy: Argument 1 to "add_text" of "BaseLayout" has incompatible type
```

### Comparing `logilab-common-1.9.7/logilab/common/ureports/text_writer.py` & `logilab-common-1.9.8/logilab/common/ureports/text_writer.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/urllib2ext.py` & `logilab-common-1.9.8/logilab/common/urllib2ext.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/vcgutils.py` & `logilab-common-1.9.8/logilab/common/vcgutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/visitor.py` & `logilab-common-1.9.8/logilab/common/visitor.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab/common/xmlutils.py` & `logilab-common-1.9.8/logilab/common/xmlutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/logilab_common.egg-info/PKG-INFO` & `logilab-common-1.9.8/logilab_common.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logilab-common
-Version: 1.9.7
+Version: 1.9.8
 Summary: collection of low-level Python packages and modules used by Logilab projects
 Home-page: http://www.logilab.org/project/logilab-common
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
```

### Comparing `logilab-common-1.9.7/logilab_common.egg-info/SOURCES.txt` & `logilab-common-1.9.8/logilab_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/setup.py` & `logilab-common-1.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/ChangeLog` & `logilab-common-1.9.8/test/data/ChangeLog`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/MyPyPa-0.1.0-py2.5.egg` & `logilab-common-1.9.8/test/data/MyPyPa-0.1.0-py2.5.egg`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/__pkginfo__.py` & `logilab-common-1.9.8/test/data/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/content_differ_dir/subdir/toto.txt` & `logilab-common-1.9.8/test/data/content_differ_dir/subdir/toto.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/file_differ_dir/subdir/toto.txt` & `logilab-common-1.9.8/test/data/file_differ_dir/subdir/toto.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/module.py` & `logilab-common-1.9.8/test/data/module.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/module2.py` & `logilab-common-1.9.8/test/data/module2.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/reference_dir/subdir/toto.txt` & `logilab-common-1.9.8/test/data/reference_dir/subdir/toto.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/regobjects.py` & `logilab-common-1.9.8/test/data/regobjects.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/same_dir/subdir/toto.txt` & `logilab-common-1.9.8/test/data/same_dir/subdir/toto.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/subdir_differ_dir/subdir/toto.txt` & `logilab-common-1.9.8/test/data/subdir_differ_dir/subdir/toto.txt`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/test1.msg` & `logilab-common-1.9.8/test/data/test1.msg`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/data/test2.msg` & `logilab-common-1.9.8/test/data/test2.msg`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_cache.py` & `logilab-common-1.9.8/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_changelog.py` & `logilab-common-1.9.8/test/test_changelog.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_configuration.py` & `logilab-common-1.9.8/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_date.py` & `logilab-common-1.9.8/test/test_date.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_decorators.py` & `logilab-common-1.9.8/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_deprecation.py` & `logilab-common-1.9.8/test/test_deprecation.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from logilab.common import deprecation
 
 
 CURRENT_FILE = os.path.abspath(__file__)
 
 
 class RawInputTC(TestCase):
-
     # XXX with 2.6 we could test warnings
     # http://docs.python.org/library/warnings.html#testing-warnings
     # instead we just make sure it does not crash
 
     def mock_warn(self, *args, **kwargs):
         self.messages.append(str(args[0]))
```

### Comparing `logilab-common-1.9.7/test/test_fileutils.py` & `logilab-common-1.9.8/test/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_graph.py` & `logilab-common-1.9.8/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_interface.py` & `logilab-common-1.9.8/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_modutils.py` & `logilab-common-1.9.8/test/test_modutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_pytest.py` & `logilab-common-1.9.8/test/test_pytest.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_registry.py` & `logilab-common-1.9.8/test/test_registry.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_shellutils.py` & `logilab-common-1.9.8/test/test_shellutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_table.py` & `logilab-common-1.9.8/test/test_table.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_taskqueue.py` & `logilab-common-1.9.8/test/test_taskqueue.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_testlib.py` & `logilab-common-1.9.8/test/test_testlib.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_textutils.py` & `logilab-common-1.9.8/test/test_textutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_tree.py` & `logilab-common-1.9.8/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_umessage.py` & `logilab-common-1.9.8/test/test_umessage.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_ureports_html.py` & `logilab-common-1.9.8/test/test_ureports_html.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_ureports_text.py` & `logilab-common-1.9.8/test/test_ureports_text.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/test_xmlutils.py` & `logilab-common-1.9.8/test/test_xmlutils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/test/utils.py` & `logilab-common-1.9.8/test/utils.py`

 * *Files identical despite different names*

### Comparing `logilab-common-1.9.7/tox.ini` & `logilab-common-1.9.8/tox.ini`

 * *Files identical despite different names*

