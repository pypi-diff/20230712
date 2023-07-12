# Comparing `tmp/azure-maps-render-1.0.0b1.zip` & `tmp/azure-maps-render-1.0.0b2.zip`

## zipinfo {}

```diff
@@ -1,83 +1,84 @@
-Zip file size: 112753 bytes, number of entries: 81
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/samples/
--rw-rw-r--  2.0 unx    12188 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/README.md
--rw-rw-r--  2.0 unx       82 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     2985 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx    13116 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx      177 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     3229 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/tests/test_render_client.py
--rw-rw-r--  2.0 unx      625 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/tests/render_preparer.py
--rw-rw-r--  2.0 unx     1258 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/tests/conftest.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/
--rw-rw-r--  2.0 unx       65 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/
--rw-rw-r--  2.0 unx       65 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/models/
--rw-rw-r--  2.0 unx      515 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_version.py
--rw-rw-r--  2.0 unx      698 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/__init__.py
--rw-rw-r--  2.0 unx    21060 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_render_client.py
--rw-rw-r--  2.0 unx     1873 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_base_client.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/
--rw-rw-r--  2.0 unx     4196 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/_client.py
--rw-rw-r--  2.0 unx     3637 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/_configuration.py
--rw-rw-r--  2.0 unx      831 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/__init__.py
--rw-rw-r--  2.0 unx    77450 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/_serialization.py
--rw-rw-r--  2.0 unx      843 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/_patch.py
--rw-rw-r--  2.0 unx    68951 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_operations.py
--rw-rw-r--  2.0 unx      788 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/
--rw-rw-r--  2.0 unx     4269 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_client.py
--rw-rw-r--  2.0 unx     3635 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      831 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx    55655 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      788 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     9833 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_enums.py
--rw-rw-r--  2.0 unx     1694 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/__init__.py
--rw-rw-r--  2.0 unx    15633 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_models.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_patch.py
--rw-rw-r--  2.0 unx    21819 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/aio/_render_client_async.py
--rw-rw-r--  2.0 unx      550 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/aio/__init__.py
--rw-rw-r--  2.0 unx     1895 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/aio/_base_client_async.py
--rw-rw-r--  2.0 unx      699 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/models/__init__.py
--rw-rw-r--  2.0 unx    10089 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/azure/maps/render/models/_models.py
--rw-rw-r--  2.0 unx     2597 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       63 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    13116 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-13 22:48 azure-maps-render-1.0.0b1/azure_maps_render.egg-info/not-zip-safe
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-13 22:48 azure-maps-render-1.0.0b1/samples/async_samples/
--rw-rw-r--  2.0 unx     4743 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/README.md
--rw-rw-r--  2.0 unx     1598 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_tile.py
--rw-rw-r--  2.0 unx     1681 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_map_tile.py
--rw-rw-r--  2.0 unx     1287 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_map_tileset.py
--rw-rw-r--  2.0 unx     1531 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_world.py
--rw-rw-r--  2.0 unx     1522 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_map_attribution.py
--rw-rw-r--  2.0 unx     1707 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_copyright_from_bounding_box.py
--rw-rw-r--  2.0 unx     1345 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_copyright_caption.py
--rw-rw-r--  2.0 unx     2502 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_authentication.py
--rw-rw-r--  2.0 unx     1787 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/sample_get_map_static_image.py
--rw-rw-r--  2.0 unx     1716 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_tile_async.py
--rw-rw-r--  2.0 unx     1464 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_caption_async.py
--rw-rw-r--  2.0 unx     1491 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_static_image_async.py
--rw-rw-r--  2.0 unx     1848 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_from_bounding_box_async.py
--rw-rw-r--  2.0 unx     1666 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_world_async.py
--rw-rw-r--  2.0 unx     2869 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_authentication_async.py
--rw-rw-r--  2.0 unx     1676 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_attribution_async.py
--rw-rw-r--  2.0 unx     1568 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tile_async.py
--rw-rw-r--  2.0 unx     1399 b- defN 22-Oct-13 22:47 azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tileset_async.py
-81 files, 396640 bytes uncompressed, 96607 bytes compressed:  75.6%
+Zip file size: 112955 bytes, number of entries: 82
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/samples/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/MANIFEST.in
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/setup.cfg
+-rw-rw-r--  2.0 unx     2967 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/setup.py
+-rw-rw-r--  2.0 unx    13171 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx      187 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/pyproject.toml
+-rw-rw-r--  2.0 unx    12188 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/README.md
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       63 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    13171 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     2612 b- defN 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure_maps_render.egg-info/SOURCES.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/_generated/
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/py.typed
+-rw-rw-r--  2.0 unx      515 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_version.py
+-rw-rw-r--  2.0 unx      698 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/__init__.py
+-rw-rw-r--  2.0 unx    21060 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_render_client.py
+-rw-rw-r--  2.0 unx     1873 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_base_client.py
+-rw-rw-r--  2.0 unx     1895 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/aio/_base_client_async.py
+-rw-rw-r--  2.0 unx    21819 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/aio/_render_client_async.py
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/aio/__init__.py
+-rw-rw-r--  2.0 unx    10089 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/models/_models.py
+-rw-rw-r--  2.0 unx      699 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/__init__.py
+-rw-rw-r--  2.0 unx     3585 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/_configuration.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     4171 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/_client.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3627 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     4307 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx    55733 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      773 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    69044 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_operations.py
+-rw-rw-r--  2.0 unx      773 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx    15759 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_models.py
+-rw-rw-r--  2.0 unx     1679 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx     7665 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/tests/conftest.py
+-rw-rw-r--  2.0 unx     3221 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/tests/test_render_client.py
+-rw-rw-r--  2.0 unx      625 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/tests/render_preparer.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-12 02:35 azure-maps-render-1.0.0b2/samples/async_samples/
+-rw-rw-r--  2.0 unx     1531 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_world.py
+-rw-rw-r--  2.0 unx     1681 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_map_tile.py
+-rw-rw-r--  2.0 unx     1522 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_map_attribution.py
+-rw-rw-r--  2.0 unx     1287 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_map_tileset.py
+-rw-rw-r--  2.0 unx     1707 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_copyright_from_bounding_box.py
+-rw-rw-r--  2.0 unx     1598 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_tile.py
+-rw-rw-r--  2.0 unx     1787 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_map_static_image.py
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_authentication.py
+-rw-rw-r--  2.0 unx     4743 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/README.md
+-rw-rw-r--  2.0 unx     1345 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/sample_get_copyright_caption.py
+-rw-rw-r--  2.0 unx     1491 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_static_image_async.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_attribution_async.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_from_bounding_box_async.py
+-rw-rw-r--  2.0 unx     1666 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_world_async.py
+-rw-rw-r--  2.0 unx     2869 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--  2.0 unx     1399 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tileset_async.py
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_tile_async.py
+-rw-rw-r--  2.0 unx     1464 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_caption_async.py
+-rw-rw-r--  2.0 unx     1568 b- defN 23-Jul-12 02:34 azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tile_async.py
+82 files, 396483 bytes uncompressed, 96653 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,244 +1,247 @@
-Filename: azure-maps-render-1.0.0b1/
+Filename: azure-maps-render-1.0.0b2/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/tests/
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/
+Filename: azure-maps-render-1.0.0b2/azure/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/
+Filename: azure-maps-render-1.0.0b2/tests/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/
+Filename: azure-maps-render-1.0.0b2/samples/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/README.md
+Filename: azure-maps-render-1.0.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/CHANGELOG.md
+Filename: azure-maps-render-1.0.0b2/setup.cfg
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/setup.py
+Filename: azure-maps-render-1.0.0b2/setup.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/setup.cfg
+Filename: azure-maps-render-1.0.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/PKG-INFO
+Filename: azure-maps-render-1.0.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/MANIFEST.in
+Filename: azure-maps-render-1.0.0b2/pyproject.toml
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/tests/test_render_client.py
+Filename: azure-maps-render-1.0.0b2/README.md
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/tests/render_preparer.py
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/tests/conftest.py
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/requires.txt
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure_maps_render.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/
+Filename: azure-maps-render-1.0.0b2/azure/maps/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/aio/
+Filename: azure-maps-render-1.0.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/models/
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_version.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/aio/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_render_client.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/models/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_base_client.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/py.typed
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/py.typed
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_version.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_render_client.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/_client.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_base_client.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/_configuration.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/aio/_base_client_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/aio/_render_client_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/_serialization.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/aio/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/_vendor.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/models/_models.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/_patch.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/models/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_operations.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_patch.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_client.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/_configuration.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_configuration.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/_serialization.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/_client.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_patch.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/_vendor.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_operations.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/_patch.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_patch.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_enums.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_models.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_patch.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/aio/_render_client_async.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/aio/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/aio/_base_client_async.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/models/__init__.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure/maps/render/models/_models.py
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/SOURCES.txt
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_models.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/requires.txt
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/dependency_links.txt
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_enums.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/top_level.txt
+Filename: azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/PKG-INFO
+Filename: azure-maps-render-1.0.0b2/tests/conftest.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/azure_maps_render.egg-info/not-zip-safe
+Filename: azure-maps-render-1.0.0b2/tests/test_render_client.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/
+Filename: azure-maps-render-1.0.0b2/tests/render_preparer.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/README.md
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_tile.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_world.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_map_tile.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_map_tile.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_map_tileset.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_map_attribution.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_world.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_map_tileset.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_map_attribution.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_copyright_from_bounding_box.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_copyright_from_bounding_box.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_tile.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_copyright_caption.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_map_static_image.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_authentication.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_authentication.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/sample_get_map_static_image.py
+Filename: azure-maps-render-1.0.0b2/samples/README.md
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_tile_async.py
+Filename: azure-maps-render-1.0.0b2/samples/sample_get_copyright_caption.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_caption_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_static_image_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_static_image_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_attribution_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_from_bounding_box_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_from_bounding_box_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_world_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_world_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_authentication_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_authentication_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_attribution_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tileset_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tile_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_tile_async.py
 Comment: 
 
-Filename: azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tileset_async.py
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_caption_async.py
+Comment: 
+
+Filename: azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tile_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-maps-render-1.0.0b1/README.md` & `azure-maps-render-1.0.0b2/README.md`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/setup.py` & `azure-maps-render-1.0.0b2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,27 +61,27 @@
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/maps/azure-maps-render',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.maps',
     ]),
+    include_package_data=True,
     install_requires=[
         'msrest>=0.6.21',
         'azure-common~=1.1',
         'azure-mgmt-core>=1.3.0,<2.0.0',
     ]
 )
```

## Comparing `azure-maps-render-1.0.0b1/PKG-INFO` & `azure-maps-render-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: azure-maps-render
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Microsoft Azure Maps Render Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/maps/azure-maps-render
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
@@ -291,12 +290,19 @@
 [create_new_application_registration]: https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/applicationsListBlade/quickStartType/AspNetWebAppQuickstartPage/sourceType/docs
 [manage_aad_auth_page]: https://docs.microsoft.com/azure/azure-maps/how-to-manage-authentication
 [how_to_manage_authentication]: https://docs.microsoft.com/azure/azure-maps/how-to-manage-authentication#view-authentication-details
 
 
 # Release History
 
+## 1.0.0b2 (2023-07-13)
+
+### Other Changes
+
+- Deprecate Elevation tile enum
+- Remove python 3.6 support
+
 ## 1.0.0b1 (2022-10-13)
 
 ### Features Added
 
 - Initial release
```

## Comparing `azure-maps-render-1.0.0b1/tests/test_render_client.py` & `azure-maps-render-1.0.0b2/tests/test_render_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
         import types
         assert isinstance(result, types.GeneratorType)
 
     @MapsRenderPreparer()
     @recorded_by_proxy
     def test_get_map_tileset(self):
         result = self.client.get_map_tileset(tileset_id=TilesetID.MICROSOFT_BASE)
-        assert result.name == "microsoft.base"
-        assert "TomTom" in result.map_attribution
+        assert result.name == "microsoft.base" or result.name == "microsoft.core.vector"
         assert len(result.tiles_endpoints) > 0
 
     @MapsRenderPreparer()
     @recorded_by_proxy
     def test_get_map_attribution(self):
         result = self.client.get_map_attribution(
             tileset_id=TilesetID.MICROSOFT_BASE,
```

## Comparing `azure-maps-render-1.0.0b1/tests/render_preparer.py` & `azure-maps-render-1.0.0b2/tests/render_preparer.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/tests/conftest.py` & `azure-maps-render-1.0.0b2/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_version.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-VERSION = "1.0.0b1"
+VERSION = "1.0.0b2"
 API_VERSION = "2022-08-01"
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_render_client.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_render_client.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_base_client.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_base_client.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/_client.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from copy import deepcopy
 from typing import Any, Optional, TYPE_CHECKING
 
 from azure.core import PipelineClient
 from azure.core.rest import HttpRequest, HttpResponse
 
-from . import models
+from . import models as _models
 from ._configuration import MapsRenderClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import RenderOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
@@ -46,17 +46,17 @@
         credential: "TokenCredential",
         client_id: Optional[str] = None,
         *,
         endpoint: str = "https://atlas.microsoft.com",
         **kwargs: Any
     ) -> None:
         self._config = MapsRenderClientConfiguration(credential=credential, client_id=client_id, **kwargs)
-        self._client = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.render = RenderOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
@@ -76,19 +76,16 @@
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         self._client.close()
 
-    def __enter__(self):
-        # type: () -> MapsRenderClient
+    def __enter__(self) -> "MapsRenderClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/_configuration.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,30 +34,27 @@
     :keyword api_version: Api Version. Default value is "2022-08-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", client_id: Optional[str] = None, **kwargs: Any) -> None:
         super(MapsRenderClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-08-01")  # type: str
+        api_version: str = kwargs.pop("api_version", "2022-08-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.credential = credential
         self.client_id = client_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://atlas.microsoft.com/.default"])
         kwargs.setdefault("sdk_moniker", "maps-render/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
         self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import MapsRenderClient
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["MapsRenderClient"]
+__all__ = [
+    "MapsRenderClient",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/_serialization.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,56 +21,71 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
+# pyright: reportUnnecessaryTypeIgnoreComment=false
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
-    from urllib.parse import quote  # type: ignore
+    from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
-import isodate
-
-from typing import Dict, Any, cast, TYPE_CHECKING
+import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-if TYPE_CHECKING:
-    from typing import Optional, Union, AnyStr, IO, Mapping
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
 
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
 
     @classmethod
-    def deserialize_from_text(cls, data, content_type=None):
-        # type: (Optional[Union[AnyStr, IO]], Optional[str]) -> Any
+    def deserialize_from_text(cls, data: Optional[Union[AnyStr, IO]], content_type: Optional[str] = None) -> Any:
         """Decode data according to content-type.
 
         Accept a stream of data as well, but will be load at once in memory for now.
 
         If no content-type, will return the string version (not bytes, not stream)
 
         :param data: Input, could be bytes or stream (will be decoded with UTF8) or text
@@ -128,16 +143,15 @@
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
                 raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
-    def deserialize_from_http_generics(cls, body_bytes, headers):
-        # type: (Optional[Union[AnyStr, IO]], Mapping) -> Any
+    def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
         specific implementation.
         Headers will tested for "content-type"
         """
         # Try to use content-type from headers if available
@@ -156,16 +170,16 @@
         return None
 
 
 try:
     basestring  # type: ignore
     unicode_str = unicode  # type: ignore
 except NameError:
-    basestring = str  # type: ignore
-    unicode_str = str  # type: ignore
+    basestring = str
+    unicode_str = str
 
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
@@ -184,15 +198,15 @@
 
     def dst(self, dt):
         """No daylight saving for UTC."""
         return datetime.timedelta(hours=1)
 
 
 try:
-    from datetime import timezone as _FixedOffset
+    from datetime import timezone as _FixedOffset  # type: ignore
 except ImportError:  # Python 2.7
 
     class _FixedOffset(datetime.tzinfo):  # type: ignore
         """Fixed offset in minutes east from UTC.
         Copy/pasted from Python doc
         :param datetime.timedelta offset: offset in timedelta format
         """
@@ -215,15 +229,15 @@
         def __getinitargs__(self):
             return (self.__offset,)
 
 
 try:
     from datetime import timezone
 
-    TZ_UTC = timezone.utc  # type: ignore
+    TZ_UTC = timezone.utc
 except ImportError:
     TZ_UTC = UTC()  # type: ignore
 
 _FLATTEN = re.compile(r"(?<!\\)\.")
 
 
 def attribute_transformer(key, attr_desc, value):
@@ -272,79 +286,84 @@
 
 
 class Model(object):
     """Mixin for all client request body/response body models to support
     serialization and deserialization.
     """
 
-    _subtype_map = {}  # type: Dict[str, Dict[str, Any]]
-    _attribute_map = {}  # type: Dict[str, Dict[str, Any]]
-    _validation = {}  # type: Dict[str, Dict[str, Any]]
+    _subtype_map: Dict[str, Dict[str, Any]] = {}
+    _attribute_map: Dict[str, Dict[str, Any]] = {}
+    _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
-            cls._xml_map
+            cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
     def _create_xml_node(cls):
         """Create XML node."""
         try:
-            xml_map = cls._xml_map
+            xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -383,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -449,15 +473,15 @@
             if subtype_value:
                 # Try to match base class. Can be class name only
                 # (bug to fix in Autorest to support x-ms-discriminator-name)
                 if cls.__name__ == subtype_value:
                     return cls
                 flatten_mapping_type = cls._flatten_subtype(subtype_key, objects)
                 try:
-                    return objects[flatten_mapping_type[subtype_value]]
+                    return objects[flatten_mapping_type[subtype_value]]  # type: ignore
                 except KeyError:
                     _LOGGER.warning(
                         "Subtype value %s has no mapping, use base class %s.",
                         subtype_value,
                         cls.__name__,
                     )
                     break
@@ -517,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -533,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -601,47 +625,46 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
-                            serialized.set(xml_name, new_attr)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                            serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
-                            serialized.text = new_attr
+                            serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
-                            serialized.extend(new_attr)
+                            serialized.extend(new_attr)  # type: ignore
                         elif isinstance(new_attr, ET.Element):
                             # If the down XML has no XML/Name, we MUST replace the tag with the local tag. But keeping the namespaces.
                             if "name" not in getattr(orig_attr, "_xml_map", {}):
                                 splitted_tag = new_attr.tag.split("}")
                                 if len(splitted_tag) == 2:  # Namespace
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
-                            serialized.append(new_attr)
+                            serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
-                            serialized.append(local_node)
+                            serialized.append(local_node)  # type: ignore
                     else:  # JSON
-                        for k in reversed(keys):
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                        for k in reversed(keys):  # type: ignore
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
-                        for k in keys:
+                        for k in keys:  # type: ignore
                             if k not in _serialized:
-                                _serialized.update(_new_attr)
-                            _new_attr = _new_attr[k]
+                                _serialized.update(_new_attr)  # type: ignore
+                            _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
                 except ValueError:
                     continue
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
@@ -655,31 +678,31 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
         if internal_data_type and not isinstance(internal_data_type, Enum):
             try:
                 deserializer = Deserializer(self.dependencies)
                 # Since it's on serialization, it's almost sure that format is not JSON REST
                 # We're not able to deal with additional properties for now.
                 deserializer.additional_properties_detection = False
                 if is_xml_model_serialization:
-                    deserializer.key_extractors = [
+                    deserializer.key_extractors = [  # type: ignore
                         attribute_key_case_insensitive_extractor,
                     ]
                 else:
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
@@ -776,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -839,15 +864,15 @@
         """
         try:  # If I received an enum, return its value
             return data.value
         except AttributeError:
             pass
 
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 # Don't change it, JSON and XML ElementTree are totally able
                 # to serialize correctly u'' strings
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
@@ -997,18 +1022,18 @@
     @staticmethod
     def serialize_enum(attr, enum_obj=None):
         try:
             result = attr.value
         except AttributeError:
             result = attr
         try:
-            enum_obj(result)
+            enum_obj(result)  # type: ignore
             return result
         except ValueError:
-            for enum_value in enum_obj:
+            for enum_value in enum_obj:  # type: ignore
                 if enum_value.value.lower() == str(attr).lower():
                     return enum_value.value
             error = "{!r} is not valid value for enum {!r}"
             raise SerializationError(error.format(attr, enum_obj))
 
     @staticmethod
     def serialize_bytearray(attr, **kwargs):
@@ -1160,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1241,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1265,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1331,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1351,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1412,15 +1438,15 @@
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
-            attributes = response._attribute_map
+            attributes = response._attribute_map  # type: ignore
             d_attrs = {}
             for attr, attr_desc in attributes.items():
                 # Check empty string. If it's not empty, someone has a real "additionalProperties"...
                 if attr == "additional_properties" and attr_desc["key"] == "":
                     continue
                 raw_value = None
                 # Enhance attr_desc with some dynamic data
@@ -1440,15 +1466,15 @@
                             _LOGGER.warning(msg, found_value, key_extractor, attr)
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
-            msg = "Unable to deserialize to object: " + class_name
+            msg = "Unable to deserialize to object: " + class_name  # type: ignore
             raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
@@ -1470,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
@@ -1539,15 +1565,15 @@
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
         if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
-            return RawDeserializer.deserialize_from_text(raw_data, content_type)
+            return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
         :param d_attrs: The deserialized response attributes.
@@ -1561,15 +1587,15 @@
                 response_obj = response(**kwargs)
                 for attr in readonly:
                     setattr(response_obj, attr, attrs.get(attr))
                 if additional_properties:
                     response_obj.additional_properties = additional_properties
                 return response_obj
             except TypeError as err:
-                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)
+                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)  # type: ignore
                 raise DeserializationError(msg + str(err))
         else:
             try:
                 for attr, value in attrs.items():
                     setattr(response, attr, value)
                 return response
             except Exception as exp:
@@ -1743,15 +1769,15 @@
         # We might be here because we have an enum modeled as string,
         # and we try to deserialize a partial dict with enum inside
         if isinstance(data, Enum):
             return data
 
         # Consider this is real string
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
 
     @staticmethod
@@ -1794,58 +1820,58 @@
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return bytearray(b64decode(attr))
+        return bytearray(b64decode(attr))  # type: ignore
 
     @staticmethod
     def deserialize_base64(attr):
         """Deserialize base64 encoded string into string.
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        padding = "=" * (3 - (len(attr) + 3) % 4)
-        attr = attr + padding
+        padding = "=" * (3 - (len(attr) + 3) % 4)  # type: ignore
+        attr = attr + padding  # type: ignore
         encoded = attr.replace("-", "+").replace("_", "/")
         return b64decode(encoded)
 
     @staticmethod
     def deserialize_decimal(attr):
         """Deserialize string into Decimal object.
 
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
         :raises: ValueError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return _long_type(attr)
+        return _long_type(attr)  # type: ignore
 
     @staticmethod
     def deserialize_duration(attr):
         """Deserialize ISO-8601 formatted string into TimeDelta object.
 
         :param str attr: response string to be deserialized.
         :rtype: TimeDelta
@@ -1867,45 +1893,45 @@
 
         :param str attr: response string to be deserialized.
         :rtype: Date
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
         return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         return isodate.parse_time(attr)
 
     @staticmethod
     def deserialize_rfc(attr):
         """Deserialize RFC-1123 formatted string into Datetime object.
 
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            parsed_date = email.utils.parsedate_tz(attr)
+            parsed_date = email.utils.parsedate_tz(attr)  # type: ignore
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
@@ -1920,15 +1946,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            attr = attr.upper()
+            attr = attr.upper()  # type: ignore
             match = Deserializer.valid_date.match(attr)
             if not match:
                 raise ValueError("Invalid datetime string: " + attr)
 
             check_decimal = attr.split(".")
             if len(check_decimal) > 1:
                 decimal_str = ""
@@ -1956,15 +1982,15 @@
         This is represented as seconds.
 
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
-            attr = int(attr.text)
+            attr = int(attr.text)  # type: ignore
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/_patch.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_operations.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_render_get_map_tile_request(
     *,
-    tileset_id: Union[str, "_models.TilesetID"],
+    tileset_id: Union[str, _models.TilesetID],
     z: int,
     x: int,
     y: int,
     time_stamp: Optional[datetime.datetime] = None,
-    tile_size: Optional[Union[str, "_models.MapTileSize"]] = None,
+    tile_size: Optional[Union[str, _models.MapTileSize]] = None,
     language: Optional[str] = None,
-    localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+    localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop(
         "Accept", "application/json, image/jpeg, image/png, image/pbf, application/vnd.mapbox-vector-tile"
     )
 
     # Construct URL
     _url = "/map/tile"
 
@@ -78,20 +78,20 @@
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_map_tileset_request(
-    *, tileset_id: Union[str, "_models.TilesetID"], client_id: Optional[str] = None, **kwargs: Any
+    *, tileset_id: Union[str, _models.TilesetID], client_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/tileset"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -103,24 +103,24 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_map_attribution_request(
     *,
-    tileset_id: Union[str, "_models.TilesetID"],
+    tileset_id: Union[str, _models.TilesetID],
     zoom: int,
     bounds: List[float],
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/attribution"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -138,15 +138,15 @@
 
 def build_render_get_map_state_tile_request(
     *, z: int, x: int, y: int, stateset_id: str, client_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/vnd.mapbox-vector-tile, application/json")
 
     # Construct URL
     _url = "/map/statetile"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -160,73 +160,73 @@
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_copyright_caption_request(
-    format: Union[str, "_models.ResponseFormat"] = "json", *, client_id: Optional[str] = None, **kwargs: Any
+    format: Union[str, _models.ResponseFormat] = "json", *, client_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/copyright/caption/{format}"
     path_format_arguments = {
         "format": _SERIALIZER.url("format", format, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if client_id is not None:
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_map_static_image_request(
-    format: Union[str, "_models.RasterTileFormat"] = "png",
+    format: Union[str, _models.RasterTileFormat] = "png",
     *,
-    layer: Optional[Union[str, "_models.StaticMapLayer"]] = None,
-    style: Optional[Union[str, "_models.MapImageStyle"]] = None,
+    layer: Optional[Union[str, _models.StaticMapLayer]] = None,
+    style: Optional[Union[str, _models.MapImageStyle]] = None,
     zoom: Optional[int] = None,
     center: Optional[List[float]] = None,
     bounding_box_private: Optional[List[float]] = None,
     height: Optional[int] = None,
     width: Optional[int] = None,
     language: Optional[str] = None,
-    localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+    localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
     pins: Optional[List[str]] = None,
     path: Optional[List[str]] = None,
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop(
         "Accept", "application/json, image/jpeg, image/png, image/pbf, application/vnd.mapbox-vector-tile"
     )
 
     # Construct URL
     _url = "/map/static/{format}"
     path_format_arguments = {
         "format": _SERIALIZER.url("format", format, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if layer is not None:
         _params["layer"] = _SERIALIZER.query("layer", layer, "str")
     if style is not None:
         _params["style"] = _SERIALIZER.query("style", style, "str")
@@ -254,35 +254,35 @@
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_copyright_from_bounding_box_request(
-    format: Union[str, "_models.ResponseFormat"] = "json",
+    format: Union[str, _models.ResponseFormat] = "json",
     *,
     south_west: List[float],
     north_east: List[float],
-    include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+    include_text: Optional[Union[str, _models.IncludeText]] = None,
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/copyright/bounding/{format}"
     path_format_arguments = {
         "format": _SERIALIZER.url("format", format, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     _params["mincoordinates"] = _SERIALIZER.query("south_west", south_west, "[float]", div=",")
     _params["maxcoordinates"] = _SERIALIZER.query("north_east", north_east, "[float]", div=",")
     if include_text is not None:
         _params["text"] = _SERIALIZER.query("include_text", include_text, "str")
@@ -292,36 +292,36 @@
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_copyright_for_tile_request(
-    format: Union[str, "_models.ResponseFormat"] = "json",
+    format: Union[str, _models.ResponseFormat] = "json",
     *,
     z: int,
     x: int,
     y: int,
-    include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+    include_text: Optional[Union[str, _models.IncludeText]] = None,
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/copyright/tile/{format}"
     path_format_arguments = {
         "format": _SERIALIZER.url("format", format, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     _params["zoom"] = _SERIALIZER.query("z", z, "int")
     _params["x"] = _SERIALIZER.query("x", x, "int")
     _params["y"] = _SERIALIZER.query("y", y, "int")
     if include_text is not None:
@@ -332,33 +332,33 @@
         _headers["x-ms-client-id"] = _SERIALIZER.header("client_id", client_id, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_render_get_copyright_for_world_request(
-    format: Union[str, "_models.ResponseFormat"] = "json",
+    format: Union[str, _models.ResponseFormat] = "json",
     *,
-    include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+    include_text: Optional[Union[str, _models.IncludeText]] = None,
     client_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/map/copyright/world/{format}"
     path_format_arguments = {
         "format": _SERIALIZER.url("format", format, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if include_text is not None:
         _params["text"] = _SERIALIZER.query("include_text", include_text, "str")
 
     # Construct headers
@@ -388,22 +388,22 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def get_map_tile(
         self,
         *,
-        tileset_id: Union[str, "_models.TilesetID"],
+        tileset_id: Union[str, _models.TilesetID],
         z: int,
         x: int,
         y: int,
         time_stamp: Optional[datetime.datetime] = None,
-        tile_size: Optional[Union[str, "_models.MapTileSize"]] = None,
+        tile_size: Optional[Union[str, _models.MapTileSize]] = None,
         language: Optional[str] = None,
-        localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+        localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
         **kwargs: Any
     ) -> Iterator[bytes]:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Tiles API allows users to request map tiles in vector or raster formats typically
         to be integrated  into a map control or SDK. Some example tiles that can be requested are Azure
         Maps road tiles, real-time  Weather Radar tiles or the map tiles created using `Azure Maps
@@ -416,16 +416,16 @@
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :keyword z: Zoom level for the desired tile.
 
          Please see `Zoom Levels and Tile Grid
@@ -468,23 +468,24 @@
 
          Please refer to `Supported Languages
          <https://docs.microsoft.com/azure/azure-maps/supported-languages>`_ for details. Default value
          is None.
         :paramtype language: str
         :keyword localized_map_view: The View parameter (also called the "user region" parameter)
          allows you to show the correct maps for a certain country/region for geopolitically disputed
-         regions. Different countries have different views of such regions, and the View parameter
-         allows your application to comply with the view required by the country your application will
-         be serving. By default, the View parameter is set to “Unified” even if you haven’t defined it
-         in  the request. It is your responsibility to determine the location of your users, and then
-         set the View parameter correctly for that location. Alternatively, you have the option to set
-         ‘View=Auto’, which will return the map data based on the IP  address of the request. The View
-         parameter in Azure Maps must be used in compliance with applicable laws, including those
-         regarding mapping, of the country where maps, images and other data and third party content
-         that you are authorized to  access via Azure Maps is made available. Example: view=IN.
+         regions. Different countries/regions have different views of such regions, and the View
+         parameter allows your application to comply with the view required by the country/region your
+         application will be serving. By default, the View parameter is set to “Unified” even if you
+         haven’t defined it in  the request. It is your responsibility to determine the location of your
+         users, and then set the View parameter correctly for that location. Alternatively, you have the
+         option to set ‘View=Auto’, which will return the map data based on the IP  address of the
+         request. The View parameter in Azure Maps must be used in compliance with applicable laws,
+         including those  regarding mapping, of the country/region where maps, images and other data and
+         third party content that you are authorized to  access via Azure Maps is made available.
+         Example: view=IN.
 
          Please refer to `Supported Views <https://aka.ms/AzureMapsLocalizationViews>`_ for details and
          to see the available Views. Known values are: "AE", "AR", "BH", "IN", "IQ", "JO", "KW", "LB",
          "MA", "OM", "PK", "PS", "QA", "SA", "SY", "YE", "Auto", and "Unified". Default value is None.
         :paramtype localized_map_view: str or ~azure.maps.render.models.LocalizedMapView
         :return: Iterator of the response bytes
         :rtype: Iterator[bytes]
@@ -497,15 +498,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[Iterator[bytes]]
+        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_tile_request(
             tileset_id=tileset_id,
             z=z,
             x=x,
             y=y,
             time_stamp=time_stamp,
@@ -513,18 +514,19 @@
             language=language,
             localized_map_view=localized_map_view,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -532,36 +534,36 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace
-    def get_map_tileset(self, *, tileset_id: Union[str, "_models.TilesetID"], **kwargs: Any) -> _models.MapTileset:
+    def get_map_tileset(self, *, tileset_id: Union[str, _models.TilesetID], **kwargs: Any) -> _models.MapTileset:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Tileset API allows users to request metadata for a tileset.
 
         :keyword tileset_id: A tileset is a collection of raster or vector data broken up into a
          uniform grid of square tiles at preset  zoom levels. Every tileset has a **tilesetId** to use
          when making requests. The **tilesetId** for tilesets created using `Azure Maps Creator
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :return: MapTileset
         :rtype: ~azure.maps.render.models.MapTileset
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -573,27 +575,28 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MapTileset]
+        cls: ClsType[_models.MapTileset] = kwargs.pop("cls", None)
 
         request = build_render_get_map_tileset_request(
             tileset_id=tileset_id,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -604,15 +607,15 @@
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace
     def get_map_attribution(
-        self, *, tileset_id: Union[str, "_models.TilesetID"], zoom: int, bounds: List[float], **kwargs: Any
+        self, *, tileset_id: Union[str, _models.TilesetID], zoom: int, bounds: List[float], **kwargs: Any
     ) -> _models.MapAttribution:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Attribution API allows users to request map copyright attribution information for a
         section of a tileset.
 
         :keyword tileset_id: A tileset is a collection of raster or vector data broken up into a
@@ -621,16 +624,16 @@
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :keyword zoom: Zoom level for the desired map attribution. Required.
         :paramtype zoom: int
         :keyword bounds: The string that represents the rectangular area of a bounding box. The bounds
@@ -650,29 +653,30 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MapAttribution]
+        cls: ClsType[_models.MapAttribution] = kwargs.pop("cls", None)
 
         request = build_render_get_map_attribution_request(
             tileset_id=tileset_id,
             zoom=zoom,
             bounds=bounds,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -727,30 +731,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[Iterator[bytes]]
+        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_state_tile_request(
             z=z,
             x=x,
             y=y,
             stateset_id=stateset_id,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -758,21 +763,21 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get_copyright_caption(
-        self, format: Union[str, "_models.ResponseFormat"] = "json", **kwargs: Any
+        self, format: Union[str, _models.ResponseFormat] = "json", **kwargs: Any
     ) -> _models.CopyrightCaption:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile
         service. In addition to basic copyright for the whole map, API is serving
         specific groups of copyrights for some countries/regions.
 
@@ -793,27 +798,28 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CopyrightCaption]
+        cls: ClsType[_models.CopyrightCaption] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_caption_request(
             format=format,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -825,25 +831,25 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace
     def get_map_static_image(
         self,
-        format: Union[str, "_models.RasterTileFormat"] = "png",
+        format: Union[str, _models.RasterTileFormat] = "png",
         *,
-        layer: Optional[Union[str, "_models.StaticMapLayer"]] = None,
-        style: Optional[Union[str, "_models.MapImageStyle"]] = None,
+        layer: Optional[Union[str, _models.StaticMapLayer]] = None,
+        style: Optional[Union[str, _models.MapImageStyle]] = None,
         zoom: Optional[int] = None,
         center: Optional[List[float]] = None,
         bounding_box_private: Optional[List[float]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         language: Optional[str] = None,
-        localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+        localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
         pins: Optional[List[str]] = None,
         path: Optional[List[str]] = None,
         **kwargs: Any
     ) -> Iterator[bytes]:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The static image service renders a user-defined, rectangular image containing a map section
@@ -985,23 +991,24 @@
 
          Please refer to `Supported Languages
          <https://docs.microsoft.com/azure/azure-maps/supported-languages>`_ for details. Default value
          is None.
         :paramtype language: str
         :keyword localized_map_view: The View parameter (also called the "user region" parameter)
          allows you to show the correct maps for a certain country/region for geopolitically disputed
-         regions. Different countries have different views of such regions, and the View parameter
-         allows your application to comply with the view required by the country your application will
-         be serving. By default, the View parameter is set to “Unified” even if you haven’t defined it
-         in  the request. It is your responsibility to determine the location of your users, and then
-         set the View parameter correctly for that location. Alternatively, you have the option to set
-         ‘View=Auto’, which will return the map data based on the IP  address of the request. The View
-         parameter in Azure Maps must be used in compliance with applicable laws, including those
-         regarding mapping, of the country where maps, images and other data and third party content
-         that you are authorized to  access via Azure Maps is made available. Example: view=IN.
+         regions. Different countries/regions have different views of such regions, and the View
+         parameter allows your application to comply with the view required by the country/region your
+         application will be serving. By default, the View parameter is set to “Unified” even if you
+         haven’t defined it in  the request. It is your responsibility to determine the location of your
+         users, and then set the View parameter correctly for that location. Alternatively, you have the
+         option to set ‘View=Auto’, which will return the map data based on the IP  address of the
+         request. The View parameter in Azure Maps must be used in compliance with applicable laws,
+         including those  regarding mapping, of the country/region where maps, images and other data and
+         third party content that you are authorized to  access via Azure Maps is made available.
+         Example: view=IN.
 
          Please refer to `Supported Views <https://aka.ms/AzureMapsLocalizationViews>`_ for details and
          to see the available Views. Known values are: "AE", "AR", "BH", "IN", "IQ", "JO", "KW", "LB",
          "MA", "OM", "PK", "PS", "QA", "SA", "SY", "YE", "Auto", and "Unified". Default value is None.
         :paramtype localized_map_view: str or ~azure.maps.render.models.LocalizedMapView
         :keyword pins: Pushpin style and instances. Use this parameter to optionally add pushpins to
          the image.
@@ -1292,15 +1299,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[Iterator[bytes]]
+        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_static_image_request(
             format=format,
             layer=layer,
             style=style,
             zoom=zoom,
             center=center,
@@ -1312,18 +1319,19 @@
             pins=pins,
             path=path,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1331,26 +1339,26 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get_copyright_from_bounding_box(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
         south_west: List[float],
         north_east: List[float],
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Returns copyright information for a given bounding box. Bounding-box requests should specify
         the minimum and maximum longitude and latitude (EPSG-3857) coordinates.
 
@@ -1360,15 +1368,16 @@
         :keyword south_west: Minimum coordinates (south-west point) of bounding box in latitude
          longitude coordinate system. E.g. 52.41064,4.84228. Required.
         :paramtype south_west: list[float]
         :keyword north_east: Maximum coordinates (north-east point) of bounding box in latitude
          longitude coordinate system. E.g. 52.41064,4.84228. Required.
         :paramtype north_east: list[float]
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1377,30 +1386,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_from_bounding_box_request(
             format=format,
             south_west=south_west,
             north_east=north_east,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1412,20 +1422,20 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace
     def get_copyright_for_tile(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
         z: int,
         x: int,
         y: int,
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile  service. In addition
         to basic copyright for the whole map, API is serving  specific groups of copyrights for some
         countries/regions.
@@ -1453,15 +1463,16 @@
          2:code:`<sup>`zoom`</sup>` -1].
 
          Please see `Zoom Levels and Tile Grid
          <https://docs.microsoft.com/azure/location-based-services/zoom-levels-and-tile-grid>`_ for
          details. Required.
         :paramtype y: int
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1470,31 +1481,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_for_tile_request(
             format=format,
             z=z,
             x=x,
             y=y,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1506,32 +1518,33 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace
     def get_copyright_for_world(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile  service. In addition
         to basic copyright for the whole map, API is serving  specific groups of copyrights for some
         countries/regions.
         Returns the copyright information for the world. To obtain the default copyright information
         for the whole world, do not specify a tile or bounding box.
 
         :param format: Desired format of the response. Value can be either *json* or *xml*. Known
          values are: "json" and "xml". Default value is "json".
         :type format: str or ~azure.maps.render.models.ResponseFormat
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1540,28 +1553,29 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_for_world_request(
             format=format,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import RenderOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "RenderOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/operations/_patch.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_client.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from copy import deepcopy
 from typing import Any, Awaitable, Optional, TYPE_CHECKING
 
 from azure.core import AsyncPipelineClient
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
-from .. import models
+from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import MapsRenderClientConfiguration
 from .operations import RenderOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
@@ -46,17 +46,17 @@
         credential: "AsyncTokenCredential",
         client_id: Optional[str] = None,
         *,
         endpoint: str = "https://atlas.microsoft.com",
         **kwargs: Any
     ) -> None:
         self._config = MapsRenderClientConfiguration(credential=credential, client_id=client_id, **kwargs)
-        self._client = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.render = RenderOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
@@ -83,9 +83,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MapsRenderClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_configuration.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     :keyword api_version: Api Version. Default value is "2022-08-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", client_id: Optional[str] = None, **kwargs: Any) -> None:
         super(MapsRenderClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-08-01")  # type: str
+        api_version: str = kwargs.pop("api_version", "2022-08-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.credential = credential
         self.client_id = client_id
         self.api_version = api_version
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import MapsRenderClient
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["MapsRenderClient"]
+__all__ = [
+    "MapsRenderClient",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/_patch.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_operations.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/aio/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,22 +58,22 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def get_map_tile(
         self,
         *,
-        tileset_id: Union[str, "_models.TilesetID"],
+        tileset_id: Union[str, _models.TilesetID],
         z: int,
         x: int,
         y: int,
         time_stamp: Optional[datetime.datetime] = None,
-        tile_size: Optional[Union[str, "_models.MapTileSize"]] = None,
+        tile_size: Optional[Union[str, _models.MapTileSize]] = None,
         language: Optional[str] = None,
-        localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+        localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
         **kwargs: Any
     ) -> AsyncIterator[bytes]:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Tiles API allows users to request map tiles in vector or raster formats typically
         to be integrated  into a map control or SDK. Some example tiles that can be requested are Azure
         Maps road tiles, real-time  Weather Radar tiles or the map tiles created using `Azure Maps
@@ -86,16 +86,16 @@
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :keyword z: Zoom level for the desired tile.
 
          Please see `Zoom Levels and Tile Grid
@@ -138,23 +138,24 @@
 
          Please refer to `Supported Languages
          <https://docs.microsoft.com/azure/azure-maps/supported-languages>`_ for details. Default value
          is None.
         :paramtype language: str
         :keyword localized_map_view: The View parameter (also called the "user region" parameter)
          allows you to show the correct maps for a certain country/region for geopolitically disputed
-         regions. Different countries have different views of such regions, and the View parameter
-         allows your application to comply with the view required by the country your application will
-         be serving. By default, the View parameter is set to “Unified” even if you haven’t defined it
-         in  the request. It is your responsibility to determine the location of your users, and then
-         set the View parameter correctly for that location. Alternatively, you have the option to set
-         ‘View=Auto’, which will return the map data based on the IP  address of the request. The View
-         parameter in Azure Maps must be used in compliance with applicable laws, including those
-         regarding mapping, of the country where maps, images and other data and third party content
-         that you are authorized to  access via Azure Maps is made available. Example: view=IN.
+         regions. Different countries/regions have different views of such regions, and the View
+         parameter allows your application to comply with the view required by the country/region your
+         application will be serving. By default, the View parameter is set to “Unified” even if you
+         haven’t defined it in  the request. It is your responsibility to determine the location of your
+         users, and then set the View parameter correctly for that location. Alternatively, you have the
+         option to set ‘View=Auto’, which will return the map data based on the IP  address of the
+         request. The View parameter in Azure Maps must be used in compliance with applicable laws,
+         including those  regarding mapping, of the country/region where maps, images and other data and
+         third party content that you are authorized to  access via Azure Maps is made available.
+         Example: view=IN.
 
          Please refer to `Supported Views <https://aka.ms/AzureMapsLocalizationViews>`_ for details and
          to see the available Views. Known values are: "AE", "AR", "BH", "IN", "IQ", "JO", "KW", "LB",
          "MA", "OM", "PK", "PS", "QA", "SA", "SY", "YE", "Auto", and "Unified". Default value is None.
         :paramtype localized_map_view: str or ~azure.maps.render.models.LocalizedMapView
         :return: Async iterator of the response bytes
         :rtype: AsyncIterator[bytes]
@@ -167,15 +168,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[AsyncIterator[bytes]]
+        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_tile_request(
             tileset_id=tileset_id,
             z=z,
             x=x,
             y=y,
             time_stamp=time_stamp,
@@ -183,18 +184,19 @@
             language=language,
             localized_map_view=localized_map_view,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -202,38 +204,36 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace_async
-    async def get_map_tileset(
-        self, *, tileset_id: Union[str, "_models.TilesetID"], **kwargs: Any
-    ) -> _models.MapTileset:
+    async def get_map_tileset(self, *, tileset_id: Union[str, _models.TilesetID], **kwargs: Any) -> _models.MapTileset:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Tileset API allows users to request metadata for a tileset.
 
         :keyword tileset_id: A tileset is a collection of raster or vector data broken up into a
          uniform grid of square tiles at preset  zoom levels. Every tileset has a **tilesetId** to use
          when making requests. The **tilesetId** for tilesets created using `Azure Maps Creator
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :return: MapTileset
         :rtype: ~azure.maps.render.models.MapTileset
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -245,27 +245,28 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MapTileset]
+        cls: ClsType[_models.MapTileset] = kwargs.pop("cls", None)
 
         request = build_render_get_map_tileset_request(
             tileset_id=tileset_id,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -276,15 +277,15 @@
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace_async
     async def get_map_attribution(
-        self, *, tileset_id: Union[str, "_models.TilesetID"], zoom: int, bounds: List[float], **kwargs: Any
+        self, *, tileset_id: Union[str, _models.TilesetID], zoom: int, bounds: List[float], **kwargs: Any
     ) -> _models.MapAttribution:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The Get Map Attribution API allows users to request map copyright attribution information for a
         section of a tileset.
 
         :keyword tileset_id: A tileset is a collection of raster or vector data broken up into a
@@ -293,16 +294,16 @@
          <https://aka.ms/amcreator>`_ are generated through the  `Tileset Create API
          <https://docs.microsoft.com/en-us/rest/api/maps/tileset>`_. The ready-to-use tilesets supplied
          by Azure Maps are listed below. For example, microsoft.base. Known values are:
          "microsoft.base", "microsoft.base.labels", "microsoft.base.hybrid", "microsoft.terra.main",
          "microsoft.base.road", "microsoft.base.darkgrey", "microsoft.base.labels.road",
          "microsoft.base.labels.darkgrey", "microsoft.base.hybrid.road",
          "microsoft.base.hybrid.darkgrey", "microsoft.imagery", "microsoft.weather.radar.main",
-         "microsoft.weather.infrared.main", "microsoft.dem", "microsoft.dem.contours",
-         "microsoft.traffic.absolute", "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
+         "microsoft.weather.infrared.main", "microsoft.traffic.absolute",
+         "microsoft.traffic.absolute.main", "microsoft.traffic.relative",
          "microsoft.traffic.relative.main", "microsoft.traffic.relative.dark",
          "microsoft.traffic.delay", "microsoft.traffic.delay.main", "microsoft.traffic.reduced.main",
          and "microsoft.traffic.incident". Required.
         :paramtype tileset_id: str or ~azure.maps.render.models.TilesetID
         :keyword zoom: Zoom level for the desired map attribution. Required.
         :paramtype zoom: int
         :keyword bounds: The string that represents the rectangular area of a bounding box. The bounds
@@ -322,29 +323,30 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MapAttribution]
+        cls: ClsType[_models.MapAttribution] = kwargs.pop("cls", None)
 
         request = build_render_get_map_attribution_request(
             tileset_id=tileset_id,
             zoom=zoom,
             bounds=bounds,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -401,30 +403,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[AsyncIterator[bytes]]
+        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_state_tile_request(
             z=z,
             x=x,
             y=y,
             stateset_id=stateset_id,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -432,21 +435,21 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get_copyright_caption(
-        self, format: Union[str, "_models.ResponseFormat"] = "json", **kwargs: Any
+        self, format: Union[str, _models.ResponseFormat] = "json", **kwargs: Any
     ) -> _models.CopyrightCaption:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile
         service. In addition to basic copyright for the whole map, API is serving
         specific groups of copyrights for some countries/regions.
 
@@ -467,27 +470,28 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CopyrightCaption]
+        cls: ClsType[_models.CopyrightCaption] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_caption_request(
             format=format,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -499,25 +503,25 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace_async
     async def get_map_static_image(
         self,
-        format: Union[str, "_models.RasterTileFormat"] = "png",
+        format: Union[str, _models.RasterTileFormat] = "png",
         *,
-        layer: Optional[Union[str, "_models.StaticMapLayer"]] = None,
-        style: Optional[Union[str, "_models.MapImageStyle"]] = None,
+        layer: Optional[Union[str, _models.StaticMapLayer]] = None,
+        style: Optional[Union[str, _models.MapImageStyle]] = None,
         zoom: Optional[int] = None,
         center: Optional[List[float]] = None,
         bounding_box_private: Optional[List[float]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         language: Optional[str] = None,
-        localized_map_view: Optional[Union[str, "_models.LocalizedMapView"]] = None,
+        localized_map_view: Optional[Union[str, _models.LocalizedMapView]] = None,
         pins: Optional[List[str]] = None,
         path: Optional[List[str]] = None,
         **kwargs: Any
     ) -> AsyncIterator[bytes]:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         The static image service renders a user-defined, rectangular image containing a map section
@@ -659,23 +663,24 @@
 
          Please refer to `Supported Languages
          <https://docs.microsoft.com/azure/azure-maps/supported-languages>`_ for details. Default value
          is None.
         :paramtype language: str
         :keyword localized_map_view: The View parameter (also called the "user region" parameter)
          allows you to show the correct maps for a certain country/region for geopolitically disputed
-         regions. Different countries have different views of such regions, and the View parameter
-         allows your application to comply with the view required by the country your application will
-         be serving. By default, the View parameter is set to “Unified” even if you haven’t defined it
-         in  the request. It is your responsibility to determine the location of your users, and then
-         set the View parameter correctly for that location. Alternatively, you have the option to set
-         ‘View=Auto’, which will return the map data based on the IP  address of the request. The View
-         parameter in Azure Maps must be used in compliance with applicable laws, including those
-         regarding mapping, of the country where maps, images and other data and third party content
-         that you are authorized to  access via Azure Maps is made available. Example: view=IN.
+         regions. Different countries/regions have different views of such regions, and the View
+         parameter allows your application to comply with the view required by the country/region your
+         application will be serving. By default, the View parameter is set to “Unified” even if you
+         haven’t defined it in  the request. It is your responsibility to determine the location of your
+         users, and then set the View parameter correctly for that location. Alternatively, you have the
+         option to set ‘View=Auto’, which will return the map data based on the IP  address of the
+         request. The View parameter in Azure Maps must be used in compliance with applicable laws,
+         including those  regarding mapping, of the country/region where maps, images and other data and
+         third party content that you are authorized to  access via Azure Maps is made available.
+         Example: view=IN.
 
          Please refer to `Supported Views <https://aka.ms/AzureMapsLocalizationViews>`_ for details and
          to see the available Views. Known values are: "AE", "AR", "BH", "IN", "IQ", "JO", "KW", "LB",
          "MA", "OM", "PK", "PS", "QA", "SA", "SY", "YE", "Auto", and "Unified". Default value is None.
         :paramtype localized_map_view: str or ~azure.maps.render.models.LocalizedMapView
         :keyword pins: Pushpin style and instances. Use this parameter to optionally add pushpins to
          the image.
@@ -966,15 +971,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[AsyncIterator[bytes]]
+        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_render_get_map_static_image_request(
             format=format,
             layer=layer,
             style=style,
             zoom=zoom,
             center=center,
@@ -986,18 +991,19 @@
             pins=pins,
             path=path,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=True, **kwargs
+        _stream = True
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1005,26 +1011,26 @@
 
         response_headers = {}
         response_headers["Content-Type"] = self._deserialize("str", response.headers.get("Content-Type"))
 
         deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get_copyright_from_bounding_box(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
         south_west: List[float],
         north_east: List[float],
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Returns copyright information for a given bounding box. Bounding-box requests should specify
         the minimum and maximum longitude and latitude (EPSG-3857) coordinates.
 
@@ -1034,15 +1040,16 @@
         :keyword south_west: Minimum coordinates (south-west point) of bounding box in latitude
          longitude coordinate system. E.g. 52.41064,4.84228. Required.
         :paramtype south_west: list[float]
         :keyword north_east: Maximum coordinates (north-east point) of bounding box in latitude
          longitude coordinate system. E.g. 52.41064,4.84228. Required.
         :paramtype north_east: list[float]
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1051,30 +1058,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_from_bounding_box_request(
             format=format,
             south_west=south_west,
             north_east=north_east,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1086,20 +1094,20 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace_async
     async def get_copyright_for_tile(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
         z: int,
         x: int,
         y: int,
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile  service. In addition
         to basic copyright for the whole map, API is serving  specific groups of copyrights for some
         countries/regions.
@@ -1127,15 +1135,16 @@
          2:code:`<sup>`zoom`</sup>` -1].
 
          Please see `Zoom Levels and Tile Grid
          <https://docs.microsoft.com/azure/location-based-services/zoom-levels-and-tile-grid>`_ for
          details. Required.
         :paramtype y: int
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1144,31 +1153,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_for_tile_request(
             format=format,
             z=z,
             x=x,
             y=y,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1180,32 +1190,33 @@
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @distributed_trace_async
     async def get_copyright_for_world(
         self,
-        format: Union[str, "_models.ResponseFormat"] = "json",
+        format: Union[str, _models.ResponseFormat] = "json",
         *,
-        include_text: Optional[Union[str, "_models.IncludeText"]] = None,
+        include_text: Optional[Union[str, _models.IncludeText]] = None,
         **kwargs: Any
     ) -> _models.Copyright:
         """**Applies to:** see pricing `tiers <https://aka.ms/AzureMapsPricingTier>`_.
 
         Copyrights API is designed to serve copyright information for Render Tile  service. In addition
         to basic copyright for the whole map, API is serving  specific groups of copyrights for some
         countries/regions.
         Returns the copyright information for the world. To obtain the default copyright information
         for the whole world, do not specify a tile or bounding box.
 
         :param format: Desired format of the response. Value can be either *json* or *xml*. Known
          values are: "json" and "xml". Default value is "json".
         :type format: str or ~azure.maps.render.models.ResponseFormat
         :keyword include_text: Yes/no value to exclude textual data from response. Only images and
-         country names will be in response. Known values are: "yes" and "no". Default value is None.
+         country/region names will be in response. Known values are: "yes" and "no". Default value is
+         None.
         :paramtype include_text: str or ~azure.maps.render.models.IncludeText
         :return: Copyright
         :rtype: ~azure.maps.render.models.Copyright
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
@@ -1214,28 +1225,29 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Copyright]
+        cls: ClsType[_models.Copyright] = kwargs.pop("cls", None)
 
         request = build_render_get_copyright_for_world_request(
             format=format,
             include_text=include_text,
             client_id=self._config.client_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import RenderOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "RenderOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/aio/operations/_patch.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ._enums import MapImageStyle
 from ._enums import MapTileSize
 from ._enums import RasterTileFormat
 from ._enums import ResponseFormat
 from ._enums import StaticMapLayer
 from ._enums import TilesetID
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Copyright",
     "CopyrightCaption",
     "ErrorAdditionalInfo",
     "ErrorDetail",
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_models.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import List, Optional, TYPE_CHECKING
+from typing import Any, List, Optional, TYPE_CHECKING
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
@@ -37,15 +37,15 @@
 
     _attribute_map = {
         "format_version": {"key": "formatVersion", "type": "str"},
         "general_copyrights": {"key": "generalCopyrights", "type": "[str]"},
         "regions": {"key": "regions", "type": "[RegionCopyrights]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.format_version = None
         self.general_copyrights = None
         self.regions = None
 
 
@@ -66,15 +66,15 @@
     }
 
     _attribute_map = {
         "format_version": {"key": "formatVersion", "type": "str"},
         "copyrights_caption": {"key": "copyrightsCaption", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.format_version = None
         self.copyrights_caption = None
 
 
 class ErrorAdditionalInfo(_serialization.Model):
@@ -94,15 +94,15 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "info": {"key": "info", "type": "object"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.info = None
 
 
 class ErrorDetail(_serialization.Model):
@@ -134,36 +134,37 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDetail]"},
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
 class ErrorResponse(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.maps.render.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
-    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
         :paramtype error: ~azure.maps.render.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
@@ -175,15 +176,15 @@
     :vartype copyrights: list[str]
     """
 
     _attribute_map = {
         "copyrights": {"key": "copyrights", "type": "[str]"},
     }
 
-    def __init__(self, *, copyrights: Optional[List[str]] = None, **kwargs):
+    def __init__(self, *, copyrights: Optional[List[str]] = None, **kwargs: Any) -> None:
         """
         :keyword copyrights: A list of copyright strings.
         :paramtype copyrights: list[str]
         """
         super().__init__(**kwargs)
         self.copyrights = copyrights
 
@@ -277,16 +278,16 @@
         tiles: Optional[List[str]] = None,
         grids: Optional[List[str]] = None,
         data: Optional[List[str]] = None,
         min_zoom: Optional[int] = None,
         max_zoom: Optional[int] = None,
         bounds: Optional[List[float]] = None,
         center: Optional[List[float]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tilejson: Describes the version of the TileJSON spec that is implemented by this JSON
          object.
         :paramtype tilejson: str
         :keyword name: A name describing the tileset. The name can contain any legal character.
          Implementations SHOULD NOT interpret the name as HTML.
         :paramtype name: str
@@ -365,15 +366,15 @@
     }
 
     _attribute_map = {
         "copyrights": {"key": "copyrights", "type": "[str]"},
         "country": {"key": "country", "type": "RegionCopyrightsCountry"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.copyrights = None
         self.country = None
 
 
 class RegionCopyrightsCountry(_serialization.Model):
@@ -393,12 +394,12 @@
     }
 
     _attribute_map = {
         "iso3": {"key": "ISO3", "type": "str"},
         "label": {"key": "label", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.iso3 = None
         self.label = None
```

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/_generated/models/_patch.py` & `azure-maps-render-1.0.0b2/azure/maps/render/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/aio/_render_client_async.py` & `azure-maps-render-1.0.0b2/azure/maps/render/aio/_render_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/aio/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/aio/_base_client_async.py` & `azure-maps-render-1.0.0b2/azure/maps/render/aio/_base_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/models/__init__.py` & `azure-maps-render-1.0.0b2/azure/maps/render/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure/maps/render/models/_models.py` & `azure-maps-render-1.0.0b2/azure/maps/render/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/azure_maps_render.egg-info/SOURCES.txt` & `azure-maps-render-1.0.0b2/azure_maps_render.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGELOG.md
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/maps/__init__.py
 azure/maps/render/__init__.py
 azure/maps/render/_base_client.py
 azure/maps/render/_render_client.py
 azure/maps/render/_version.py
```

## Comparing `azure-maps-render-1.0.0b1/azure_maps_render.egg-info/PKG-INFO` & `azure-maps-render-1.0.0b2/azure_maps_render.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: azure-maps-render
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Microsoft Azure Maps Render Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/maps/azure-maps-render
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
@@ -291,12 +290,19 @@
 [create_new_application_registration]: https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/applicationsListBlade/quickStartType/AspNetWebAppQuickstartPage/sourceType/docs
 [manage_aad_auth_page]: https://docs.microsoft.com/azure/azure-maps/how-to-manage-authentication
 [how_to_manage_authentication]: https://docs.microsoft.com/azure/azure-maps/how-to-manage-authentication#view-authentication-details
 
 
 # Release History
 
+## 1.0.0b2 (2023-07-13)
+
+### Other Changes
+
+- Deprecate Elevation tile enum
+- Remove python 3.6 support
+
 ## 1.0.0b1 (2022-10-13)
 
 ### Features Added
 
 - Initial release
```

## Comparing `azure-maps-render-1.0.0b1/samples/README.md` & `azure-maps-render-1.0.0b2/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_tile.py` & `azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_tile.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_map_tile.py` & `azure-maps-render-1.0.0b2/samples/sample_get_map_tile.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_map_tileset.py` & `azure-maps-render-1.0.0b2/samples/sample_get_map_tileset.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_copyright_for_world.py` & `azure-maps-render-1.0.0b2/samples/sample_get_copyright_for_world.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_map_attribution.py` & `azure-maps-render-1.0.0b2/samples/sample_get_map_attribution.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_copyright_from_bounding_box.py` & `azure-maps-render-1.0.0b2/samples/sample_get_copyright_from_bounding_box.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_copyright_caption.py` & `azure-maps-render-1.0.0b2/samples/sample_get_copyright_caption.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_authentication.py` & `azure-maps-render-1.0.0b2/samples/sample_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/sample_get_map_static_image.py` & `azure-maps-render-1.0.0b2/samples/sample_get_map_static_image.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_tile_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_tile_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_caption_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_caption_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_static_image_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_static_image_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_from_bounding_box_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_from_bounding_box_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_copyright_for_world_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_copyright_for_world_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_authentication_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_attribution_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_attribution_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tile_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tile_async.py`

 * *Files identical despite different names*

## Comparing `azure-maps-render-1.0.0b1/samples/async_samples/sample_get_map_tileset_async.py` & `azure-maps-render-1.0.0b2/samples/async_samples/sample_get_map_tileset_async.py`

 * *Files identical despite different names*

