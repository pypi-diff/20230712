# Comparing `tmp/imephu-0.2.1.tar.gz` & `tmp/imephu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.2.1.tar", max compression
+gzip compressed data, was "imephu-0.3.0.tar", max compression
```

## Comparing `imephu-0.2.1.tar` & `imephu-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.2.1/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.2.1/README.md
--rw-r--r--   0        0        0      991 2023-07-10 14:47:42.724245 imephu-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      185 2023-07-10 14:47:42.735179 imephu-0.2.1/src/imephu/__init__.py
--rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.2.1/src/imephu/annotation/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.2.1/src/imephu/annotation/general/__init__.py
--rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.2.1/src/imephu/annotation/general/arrow.py
--rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.2.1/src/imephu/annotation/general/circle.py
--rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.2.1/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.2.1/src/imephu/annotation/general/empty.py
--rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.2.1/src/imephu/annotation/general/group.py
--rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.2.1/src/imephu/annotation/general/line_path.py
--rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.2.1/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.2.1/src/imephu/annotation/general/text.py
--rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.2.1/src/imephu/annotation/motion.py
--rw-r--r--   0        0        0    12039 2023-07-10 14:47:42.739506 imephu-0.2.1/src/imephu/cli.py
--rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.2.1/src/imephu/finder_chart.py
--rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.2.1/src/imephu/geometry.py
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.2.1/src/imephu/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.2.1/src/imephu/salt/annotation/__init__.py
--rw-r--r--   0        0        0    12257 2023-07-10 14:47:42.740967 imephu-0.2.1/src/imephu/salt/annotation/nir.py
--rw-r--r--   0        0        0     3859 2023-07-10 14:47:42.741179 imephu-0.2.1/src/imephu/salt/annotation/rss.py
--rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.2.1/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.2.1/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0        0        0    14802 2023-07-10 14:47:42.741868 imephu-0.2.1/src/imephu/salt/finder_chart.py
--rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.2.1/src/imephu/salt/utils.py
--rw-r--r--   0        0        0    10458 2023-07-10 14:47:42.742329 imephu-0.2.1/src/imephu/schema.json
--rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.2.1/src/imephu/service/horizons.py
--rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.2.1/src/imephu/service/survey.py
--rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.2.1/src/imephu/utils.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.3.0/README.md
+-rw-r--r--   0        0        0      991 2023-07-12 17:32:34.545589 imephu-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.3.0/src/imephu/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.3.0/src/imephu/annotation/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.3.0/src/imephu/annotation/general/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.3.0/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.3.0/src/imephu/annotation/general/circle.py
+-rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.3.0/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.3.0/src/imephu/annotation/general/empty.py
+-rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.3.0/src/imephu/annotation/general/group.py
+-rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.3.0/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.3.0/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.3.0/src/imephu/annotation/general/text.py
+-rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.3.0/src/imephu/annotation/motion.py
+-rw-r--r--   0        0        0    12102 2023-07-12 17:32:34.547123 imephu-0.3.0/src/imephu/cli.py
+-rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.3.0/src/imephu/finder_chart.py
+-rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.3.0/src/imephu/geometry.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.3.0/src/imephu/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.3.0/src/imephu/salt/annotation/__init__.py
+-rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.3.0/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0        0        0     3859 2023-07-10 14:47:42.741179 imephu-0.3.0/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.3.0/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.3.0/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0        0        0    15176 2023-07-12 17:32:34.548326 imephu-0.3.0/src/imephu/salt/finder_chart.py
+-rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.3.0/src/imephu/salt/utils.py
+-rw-r--r--   0        0        0    10440 2023-07-12 17:32:34.548999 imephu-0.3.0/src/imephu/schema.json
+-rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.3.0/src/imephu/service/horizons.py
+-rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.3.0/src/imephu/service/survey.py
+-rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.3.0/src/imephu/utils.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.3.0/PKG-INFO
```

### Comparing `imephu-0.2.1/LICENSE` & `imephu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/README.md` & `imephu-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/pyproject.toml` & `imephu-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imephu"
-version = "0.2.1"
+version = "0.3.0"
 description = "Generate finder charts for astronomical observations."
 authors = ["Southern African Large Telescope"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `imephu-0.2.1/src/imephu/annotation/__init__.py` & `imephu-0.3.0/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/__init__.py` & `imephu-0.3.0/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/arrow.py` & `imephu-0.3.0/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/circle.py` & `imephu-0.3.0/src/imephu/annotation/general/circle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/crosshairs.py` & `imephu-0.3.0/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/empty.py` & `imephu-0.3.0/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/group.py` & `imephu-0.3.0/src/imephu/annotation/general/group.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/line_path.py` & `imephu-0.3.0/src/imephu/annotation/general/line_path.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/rectangle.py` & `imephu-0.3.0/src/imephu/annotation/general/rectangle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/general/text.py` & `imephu-0.3.0/src/imephu/annotation/general/text.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/annotation/motion.py` & `imephu-0.3.0/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/cli.py` & `imephu-0.3.0/src/imephu/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -323,21 +323,24 @@
 ) -> FinderChart:
     return sfc.hrs_finder_chart(fits=fits, general=general)
 
 
 def _create_nir_finder_chart(
     fits: Union[BinaryIO, Path], general: GeneralProperties, nir: Dict[str, Any]
 ) -> FinderChart:
-    science_bundle_center = SkyCoord(
-        ra=nir["science-bundle"]["ra"], dec=nir["science-bundle"]["dec"]
-    )
+    if "reference-star" in nir:
+        reference_star = SkyCoord(
+            ra=nir["reference-star"]["ra"], dec=nir["reference-star"]["dec"]
+        )
+    else:
+        reference_star = None
     bundle_separation = Angle(nir["bundle-separation"])
     return sfc.nir_finder_chart(
         fits=fits,
         general=general,
-        science_bundle_center=science_bundle_center,
+        reference_star=reference_star,
         bundle_separation=bundle_separation,
     )
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `imephu-0.2.1/src/imephu/finder_chart.py` & `imephu-0.3.0/src/imephu/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/geometry.py` & `imephu-0.3.0/src/imephu/geometry.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/salt/annotation/nir.py` & `imephu-0.3.0/src/imephu/salt/annotation/nir.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 )
 from imephu.geometry import translate
 
 _OUTLINE_COLOR = "red"
 
 
 def bundles_annotation(
+    finder_chart_center: SkyCoord,
     science_bundle_center: SkyCoord,
     bundle_separation: Angle,
     position_angle: Angle,
     wcs: WCS,
     include_fibers: bool = False,
 ) -> GroupAnnotation:
     """Return the annotation for NIR fiber bundles.
 
     The annotation contains the outline of the science fiber bundle (with its center
     marked by crosshairs) and the outlines of the sky fiber bundles.
 
     Parameters
     ----------
+    finder_chart_center: `~astropy.coordinates.SkyCoord`
+        The finder chart center, as a position on the sky, in right ascension and
+        declination.
     science_bundle_center: `~astropy.coordinates.SkyCoord`
         The center position of the sky fiber bundle, as a position on the sky, in
         right ascension and declination.
     bundle_separation: ~astropy.coordinates.Angle`
         The separation between the science fiber bundle and the sky fiber bundles, as an
         angle on the sky. The separation is measured between the center of the science
         bundle and the midpoint of the line between the centers of the sky bundles.
@@ -50,32 +54,36 @@
     d_horizontal = 1.63 * u.arcsec
     d_vertical = 1.42 * u.arcsec
     bundle_separaration_arcsec = bundle_separation.to_value(u.arcsec)
     science_bundle = _science_bundle(
         r=r,
         d_horizontal=d_horizontal,
         d_vertical=d_vertical,
-        center=science_bundle_center,
+        center=finder_chart_center,
         wcs=wcs,
         include_fibers=include_fibers,
-    )
+    ).rotate(finder_chart_center, 90 * u.deg + position_angle)
     sky_bundle = (
         _sky_bundle(
             r=r,
             d_horizontal=d_horizontal,
             d_vertical=d_vertical,
-            center=science_bundle_center,
+            center=finder_chart_center,
             wcs=wcs,
             include_fibers=include_fibers,
         )
-        .rotate(science_bundle_center, 90 * u.deg)
-        .translate((0, bundle_separaration_arcsec) * u.arcsec)
+        .rotate(finder_chart_center, 90 * u.deg)
+        .translate((bundle_separaration_arcsec, 0) * u.arcsec)
+        .rotate(finder_chart_center, position_angle)
     )
     annotation = GroupAnnotation([sky_bundle, science_bundle])
-    return annotation.rotate(science_bundle_center, position_angle)
+
+    target_offsets = finder_chart_center.spherical_offsets_to(science_bundle_center)
+
+    return annotation.translate(target_offsets)
 
 
 def _science_bundle(
     r: Angle,
     d_horizontal: Angle,
     d_vertical: Angle,
     center: SkyCoord,
```

### Comparing `imephu-0.2.1/src/imephu/salt/annotation/rss.py` & `imephu-0.3.0/src/imephu/salt/annotation/rss.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/salt/annotation/salticam.py` & `imephu-0.3.0/src/imephu/salt/annotation/salticam.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/salt/annotation/telescope.py` & `imephu-0.3.0/src/imephu/salt/annotation/telescope.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/salt/finder_chart.py` & `imephu-0.3.0/src/imephu/salt/finder_chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,40 +230,43 @@
     finder_chart.add_annotation(annotation)
     return finder_chart
 
 
 def nir_finder_chart(
     fits: Union[str, BinaryIO, os.PathLike[Any]],
     general: GeneralProperties,
-    science_bundle_center: SkyCoord,
+    reference_star: Optional[SkyCoord],
     bundle_separation: Angle,
 ) -> FinderChart:
     """Return the finder chart for an NIR observation.
 
+    If coordinates for a reference star are passed, they define the center of the finder
+    chart, and the sky bundle is centered on the target coordinates.
+
     Parameters
     ----------
     fits: `str`, `path-like` or `binary file-like`
         FITS file to display.
-    science_bundle_center: `~astropy.coordinates.SkyCoord`
-        The center position of the sky fiber bundle, as a position on the sky, in
-        right ascension and declination.
+    reference_star: `~astropy.coordinates.SkyCoord`, optional
+        The position of the reference star, as a position on the sky, in right ascension
+        and declination. This is taken to be the center of the finder chart.
     bundle_separation: ~astropy.coordinates.Angle`
         The separation between the science fiber bundle and the sky fiber bundles, as an
         angle on the sky. The separation is measured between the center of the science
         bundle and the midpoint of the line between the centers of the sky bundles.
 
     Returns
     -------
     `~imephu.finder_chart.FinderChart`
         The finder chart for an NIR observation.
     """
     finder_chart = FinderChart(fits)
     annotation = _nir_observation_annotation(
         general=general,
-        science_bundle_center=science_bundle_center,
+        reference_star=reference_star,
         bundle_separation=bundle_separation,
         wcs=finder_chart.wcs,
     )
     finder_chart.add_annotation(annotation)
     return finder_chart
 
 
@@ -394,20 +397,24 @@
     general: GeneralProperties, wcs: WCS
 ) -> GroupAnnotation:
     return _imaging_annotation(general=general, is_slot_mode=False, wcs=wcs)
 
 
 def _nir_observation_annotation(
     general: GeneralProperties,
-    science_bundle_center: SkyCoord,
+    reference_star: Optional[SkyCoord],
     bundle_separation: Angle,
     wcs: WCS,
 ) -> GroupAnnotation:
+    science_bundle_center = general.target.position
+    if reference_star:
+        general.target.position = reference_star
     observation_annotation = _base_annotations(general, wcs)
     bundles_annotation = nir.bundles_annotation(
+        finder_chart_center=general.target.position,
         science_bundle_center=science_bundle_center,
         bundle_separation=bundle_separation,
         position_angle=general.position_angle,
         wcs=wcs,
     )
     observation_annotation.add_item(bundles_annotation)
     return observation_annotation
```

### Comparing `imephu-0.2.1/src/imephu/salt/utils.py` & `imephu-0.3.0/src/imephu/salt/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/schema.json` & `imephu-0.3.0/src/imephu/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992404513888888%*

 * *Differences: {"'$defs'": "{'nir': {'properties': {'reference-star': OrderedDict([('type', 'object'), "*

 * *            "('properties', OrderedDict([('dec', OrderedDict([('type', 'string'), ('description', "*

 * *            "'Declination of the reference star, in a format understood by AstroPy'), ('examples', "*

 * *            "['-24d 5m 16s', '-15.967d'])])), ('ra', OrderedDict([('type', 'string'), "*

 * *            "('description', 'Right ascension of the reference star, in a format understood by "*

 * *            "AstroPy'), ('examples', […]*

```diff
@@ -46,27 +46,27 @@
                     "description": "The separation between the science and sky bundle as an angle, in a format understood by AstroPy",
                     "examples": [
                         "52arcsec",
                         "74.4arcsec"
                     ],
                     "type": "string"
                 },
-                "science-bundle": {
+                "reference-star": {
                     "additionalProperties": false,
                     "properties": {
                         "dec": {
-                            "description": "Declination of the sky bundle, in a format understood by AstroPy",
+                            "description": "Declination of the reference star, in a format understood by AstroPy",
                             "examples": [
                                 "-24d 5m 16s",
                                 "-15.967d"
                             ],
                             "type": "string"
                         },
                         "ra": {
-                            "description": "Right ascension of the sky bundle, in a format understood by AstroPy",
+                            "description": "Right ascension of the reference star, in a format understood by AstroPy",
                             "examples": [
                                 "23h 17m 22s",
                                 "134.9823d"
                             ],
                             "type": "string"
                         }
                     },
@@ -74,16 +74,15 @@
                         "dec",
                         "ra"
                     ],
                     "type": "object"
                 }
             },
             "required": [
-                "bundle-separation",
-                "science-bundle"
+                "bundle-separation"
             ],
             "type": "object"
         },
         "non-sidereal-target": {
             "additionalProperties": false,
             "description": "Non-sidereal target",
             "properties": {
```

### Comparing `imephu-0.2.1/src/imephu/service/horizons.py` & `imephu-0.3.0/src/imephu/service/horizons.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/service/survey.py` & `imephu-0.3.0/src/imephu/service/survey.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/src/imephu/utils.py` & `imephu-0.3.0/src/imephu/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.2.1/PKG-INFO` & `imephu-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generate finder charts for astronomical observations.
 License: MIT
 Author: Southern African Large Telescope
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

