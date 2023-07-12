# Comparing `tmp/landingai-0.1.4.tar.gz` & `tmp/landingai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.1.4.tar", max compression
+gzip compressed data, was "landingai-0.1.5.tar", max compression
```

## Comparing `landingai-0.1.4.tar` & `landingai-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-07-07 18:46:35.903424 landingai-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     6741 2023-07-07 18:46:35.903424 landingai-0.1.4/README.md
--rw-r--r--   0        0        0      354 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/data_management/client.py
--rw-r--r--   0        0        0    19873 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9418 2023-07-07 18:46:35.931424 landingai-0.1.4/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     6843 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/io.py
--rw-r--r--   0        0        0      221 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0     5287 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     5912 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/postprocess.py
--rw-r--r--   0        0        0    25157 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4374 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1685 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/utils.py
--rw-r--r--   0        0        0    23703 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/vision_pipeline.py
--rw-r--r--   0        0        0    13403 2023-07-07 18:46:35.943424 landingai-0.1.4/landingai/visualize.py
--rw-r--r--   0        0        0     2487 2023-07-07 18:46:36.627427 landingai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-12 18:41:46.000441 landingai-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     6741 2023-07-12 18:41:46.000441 landingai-0.1.5/README.md
+-rw-r--r--   0        0        0      354 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/client.py
+-rw-r--r--   0        0        0    19873 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9418 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-12 18:41:46.036442 landingai-0.1.5/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     6843 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/io.py
+-rw-r--r--   0        0        0      221 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5287 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     5912 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/postprocess.py
+-rw-r--r--   0        0        0    25559 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4374 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     2657 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/telemetry.py
+-rw-r--r--   0        0        0     1685 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/utils.py
+-rw-r--r--   0        0        0    23703 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/vision_pipeline.py
+-rw-r--r--   0        0        0    13403 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-12 18:41:46.736454 landingai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.5/PKG-INFO
```

### Comparing `landingai-0.1.4/LICENSE.md` & `landingai-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/README.md` & `landingai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/common.py` & `landingai-0.1.5/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/data_management/client.py` & `landingai-0.1.5/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/data_management/media.py` & `landingai-0.1.5/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/data_management/metadata.py` & `landingai-0.1.5/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/data_management/utils.py` & `landingai-0.1.5/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/exceptions.py` & `landingai-0.1.5/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.1.5/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/io.py` & `landingai-0.1.5/landingai/io.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/pipeline/image_source.py` & `landingai-0.1.5/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/postprocess.py` & `landingai-0.1.5/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/predict.py` & `landingai-0.1.5/landingai/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Module for making predictions on LandingLens models."""
 
 import json
 import logging
-
-# from importlib.metadata import version
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
 import numpy as np
 import PIL.Image
 import requests
 from requests import Session
 from requests.adapters import HTTPAdapter
@@ -18,14 +16,15 @@
     ClassificationPrediction,
     ObjectDetectionPrediction,
     OcrPrediction,
     Prediction,
     SegmentationPrediction,
 )
 from landingai.exceptions import HttpResponse
+from landingai.telemetry import get_runtime_environment_info, is_running_in_pytest
 from landingai.utils import load_api_credential, serialize_image
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Predictor:
     """A class that calls your inference endpoint on the LandingLens platform."""
@@ -84,19 +83,15 @@
         """
         buffer_bytes = serialize_image(image)
         files = [("file", ("image.png", buffer_bytes, "image/png"))]
         payload = {
             "endpoint_id": self._endpoint_id,
             "device_type": "pylib",
         }
-        # Add library version if available
-        # try:
-        #     payload["device_version"] = version("landingai")
-        # except Exception:
-        #     pass
+        _add_defualt_query_params(payload)
         return _do_inference(
             self._session, Predictor._url, files, payload, _CloudExtractor
         )
 
 
 class OcrPredictor(Predictor):
     """A class that calls your OCR inference endpoint on the LandingLens platform."""
@@ -117,15 +112,15 @@
             The minimum confidence threshold of the prediction to keep, by default 0.5
         api_key
             The API Key of your LandingLens organization.
             If not provided, it will try to load from the environment variable
             LANDINGAI_API_KEY or from the .env file.
         """
         self._threshold = threshold
-        self._api_crendential = load_api_credential(api_key)
+        self._api_credential = load_api_credential(api_key)
         headers = self._build_default_headers(self._api_credential)
         self._session = _create_session(Predictor._url, self._num_retry, headers)
 
     def predict(
         self, image: Union[np.ndarray, PIL.Image.Image], **kwargs: Any
     ) -> List[Prediction]:
         """Run OCR on the input image and return the prediction result.
@@ -163,14 +158,15 @@
             )
         data = {}
         rois: List[List[Tuple[int, int]]] = kwargs.get("regions_of_interest", [])
         if rois:
             data["rois"] = serialize_rois(rois, mode)
 
         payload: Dict[str, Any] = {"device_type": "pylib"}
+        _add_defualt_query_params(payload)
         preds = _do_inference(
             self._session,
             OcrPredictor._url,
             files,
             payload,
             _OcrExtractor,
             data=data,
@@ -702,7 +698,17 @@
             f"Failed to connect to the model server. Please double check the model server url ({endpoint_url}) is correct.\nException detail: {e}"
         )
     response = HttpResponse.from_response(resp)
     _LOGGER.debug("Response: %s", response)
     response.raise_for_status()
     json_dict = response.json()
     return extractor_class.extract_prediction(json_dict)
+
+
+def _add_defualt_query_params(payload: Dict[str, Any]) -> None:
+    """Add default query params to the payload for tracking and analystics purppose."""
+    env_info = get_runtime_environment_info()
+    payload["runtime"] = env_info["runtime"]
+    if is_running_in_pytest():
+        # Don't add extra query params if pytest is running, otherwise it will fail some unit tests
+        return
+    payload["lib_version"] = env_info["lib_version"]
```

### Comparing `landingai-0.1.4/landingai/st_utils.py` & `landingai-0.1.5/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/storage/snowflake.py` & `landingai-0.1.5/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/transform.py` & `landingai-0.1.5/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/utils.py` & `landingai-0.1.5/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/vision_pipeline.py` & `landingai-0.1.5/landingai/vision_pipeline.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/landingai/visualize.py` & `landingai-0.1.5/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.4/pyproject.toml` & `landingai-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.1.4"
+version = "0.1.5"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
 "repository" = "https://github.com/landing-ai/landingai-python"
 "documentation" = "https://landing-ai.github.io/landingai-python/landingai.html"
 
 [tool.poetry.dependencies]  # main dependency group
 python = ">=3.8,<4.0"
 
-opencv-python = ">=4.5,<5.0"
+opencv-python = ">=4.5,<5.0"  # about 87MB (exclude transitive dependencies)
 numpy = ">=1.21.0,<2.0.0"
 pillow = "9.*" # Version 10.0.0 had a issue on FreeTypeFont that will be fixed on the next release 
 pydantic = { version = "1.*", extras = ["dotenv"] } # Version 2 has breaking changes (in particular to seetings)
 requests = "2.*"
-snowflake-connector-python = "3.0.*"
+snowflake-connector-python = "3.0.*"  # about 51MB (exclude transitive dependencies)
 bbox-visualizer = "^0.1.0"
 segmentation-mask-overlay = "^0.3.4"
 imageio = { version = "2.*", extras = ["ffmpeg"] }
 aiohttp = { version = ">=3.7.3,<4.0.0", extras = ["speedups"] }
 aiofiles = ">=0.7.0,<1.0.0"
 tqdm = ">=4.64.0,<5.0.0"
 
@@ -43,14 +43,15 @@
 types-requests = "^2.31.0.0"
 types-pillow = "^9.5.0.4"
 data-science-types = "^0.2.23"
 testbook = "^0.4.2"
 types-aiofiles = "^23.1.0.4"
 types-tqdm = "^4.65.0.1"
 aioresponses = "^0.7.4"
+setuptools = "^68.0.0"
 
 
 [tool.poetry.group.examples.dependencies]
 jupyterlab = "4.*"
 
 [tool.pytest.ini_options]
 log_cli = true
```

### Comparing `landingai-0.1.4/PKG-INFO` & `landingai-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

