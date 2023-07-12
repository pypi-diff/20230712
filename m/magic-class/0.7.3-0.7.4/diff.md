# Comparing `tmp/magic_class-0.7.3.tar.gz` & `tmp/magic_class-0.7.4.tar.gz`

## Comparing `magic_class-0.7.3.tar` & `magic_class-0.7.4.tar`

### file list

```diff
@@ -1,137 +1,141 @@
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_app.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_register_types.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/command_palette.py
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/core.py
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/help.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/plot_api.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/signature.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/undo.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/__init__.py
--rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_base.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_dock_widget.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_function_gui.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_gui_modes.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_icon.py
--rw-r--r--   0        0        0    23956 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_macro.py
--rw-r--r--   0        0        0    12944 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_macro_utils.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_message_box.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_napari_type.py
--rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/class_gui.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/keybinding.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/menu_gui.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/mgui_ext.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/runner.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/toolbar.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/_doc.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/_shared_utils.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/__init__.py
--rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/progress.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/resource.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/__init__.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/_magicgui.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/types.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/utils.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/viewer.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/widgets.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/tests/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/tests/test_viewer.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/tests/test_viewer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/_const.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/components.py
--rw-r--r--   0        0        0    24189 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/graph_items.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/mouse_event.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/plot_api.py
--rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/_qt.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/widgets.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/_base.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/camera.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layer2d.py
--rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layer3d.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layerlist.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/plot_api.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/widgets2d.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/widgets3d.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/tests/__init__.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/tests/test_vispy2d.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/__init__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/components.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/const.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/volume.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/widgets.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_define.py
--rw-r--r--   0        0        0    29154 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_fields.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_group.py
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_property.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/__init__.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_dispatch.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_partial.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_wraps.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/logging/__init__.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/logging/core.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/stylesheets/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_bound.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_choices.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_const.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_expr.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_optional.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_path.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_union.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/__init__.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_click.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_functions.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_recent.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qt.py
--rw-r--r--   0        0        0    32376 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qthreading.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qtsignal.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/__init__.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_html.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_mpl_canvas.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_union.py
--rw-r--r--   0        0        0    25634 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/codeedit.py
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/color.py
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/colormap.py
--rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/containers.py
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/eval.py
--rw-r--r--   0        0        0    20883 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/logger.py
--rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/misc.py
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/plot.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/separator.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/toggle_switch.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/utils.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/__init__.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/dict.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/list.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/object.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/tests/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/tests/test_eval.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_abstractapi.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_confirm.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_misc.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_preview.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/core.pyi
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/__init__.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/_function_gui_test.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/_gui_test.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.3/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.3/LICENSE
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.3/README.md
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 magic_class-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 magic_class-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_app.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_exceptions.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_register_types.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/command_palette.py
+-rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/core.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/help.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/plot_api.py
+-rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/signature.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/undo.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/__init__.py
+-rw-r--r--   0        0        0    48991 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_base.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_dock_widget.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_function_gui.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_gui_modes.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_icon.py
+-rw-r--r--   0        0        0    29832 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_macro.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_macro_utils.py
+-rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_message_box.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/_napari_type.py
+-rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/class_gui.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/keybinding.py
+-rw-r--r--   0        0        0    11223 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/menu_gui.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/mgui_ext.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/runner.py
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/toolbar.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/_gui/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/_doc.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/_shared_utils.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/dask/__init__.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/dask/progress.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/dask/resource.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/_magicgui.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/types.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/utils.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/viewer.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/napari/widgets.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pandas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pandas/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pandas/tests/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pandas/tests/test_viewer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/polars/__init__.py
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/polars/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/polars/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/polars/tests/test_viewer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/_const.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/components.py
+-rw-r--r--   0        0        0    24189 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/graph_items.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/mouse_event.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/plot_api.py
+-rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/tests/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/qtconsole/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/qtconsole/_qt.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/qtconsole/widgets.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/_base.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/camera.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/layer2d.py
+-rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/layer3d.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/layerlist.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/plot_api.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/widgets2d.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/widgets3d.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vispy/tests/test_vispy2d.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vtk/__init__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vtk/components.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vtk/const.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vtk/volume.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/ext/vtk/widgets.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/fields/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/fields/_define.py
+-rw-r--r--   0        0        0    29154 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/fields/_fields.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/fields/_group.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/fields/_property.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/functools/__init__.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/functools/_dispatch.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/functools/_partial.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/functools/_wraps.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/logging/__init__.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/logging/core.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/stylesheets/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_bound.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_choices.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_const.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_expr.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_optional.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_path.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/types/_union.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/__init__.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/_click.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/_functions.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/_recent.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/qt.py
+-rw-r--r--   0        0        0    33157 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/qthreading.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/utils/qtsignal.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/_const.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/_html.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/_mpl_canvas.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/_union.py
+-rw-r--r--   0        0        0    37238 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/codeedit.py
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/color.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/colormap.py
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/containers.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/eval.py
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/line_runner.py
+-rw-r--r--   0        0        0    20883 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/logger.py
+-rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/misc.py
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/plot.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/separator.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/toggle_switch.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/utils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/pywidgets/__init__.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/pywidgets/dict.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/pywidgets/list.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/pywidgets/object.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/pywidgets/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/tests/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/widgets/tests/test_eval.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/wrappers/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/wrappers/_abstractapi.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/wrappers/_confirm.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/wrappers/_misc.py
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/wrappers/_preview.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/core.pyi
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/testing/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/testing/_error_test.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/testing/_function_gui_test.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 magic_class-0.7.4/magicclass/testing/_gui_test.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.4/README.md
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 magic_class-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 magic_class-0.7.4/PKG-INFO
```

### Comparing `magic_class-0.7.3/magicclass/__init__.py` & `magic_class-0.7.4/magicclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 
 from .core import (
     magicclass,
     magicmenu,
     magiccontext,
     magictoolbar,
     Parameters,
```

### Comparing `magic_class-0.7.3/magicclass/_app.py` & `magic_class-0.7.4/magicclass/_app.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_register_types.py` & `magic_class-0.7.4/magicclass/_register_types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/command_palette.py` & `magic_class-0.7.4/magicclass/command_palette.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Iterable
 from typing_extensions import Literal
 from qt_command_palette import get_palette
 from magicclass._gui import BaseGui
+from magicclass._gui.class_gui import ClassGuiBase
 from magicclass._gui.mgui_ext import Clickable, is_clickable
 
 if TYPE_CHECKING:
     from qt_command_palette._api import CommandPalette
 
 _PALETTES: dict[int, CommandPalette] = {}
 
@@ -51,28 +52,28 @@
         if _id in processed:
             continue
         _qualname = type(parent).__qualname__
         palette.register(
             _define_command(wdt.changed.emit),
             title=_qualname,
             desc=wdt.text,
-            when=_define_when(wdt),
+            when=_define_when(wdt, parent),
         )
         processed.add(_id)
     palette.sort(rule=lambda cmd: str(cmd.title.count(".")) + cmd.title + cmd.desc)
     _PALETTES[_id] = palette
     palette.install(gui.native)
     return palette.show_widget(gui.native)
 
 
 def _define_command(fn: Callable) -> Callable:
     return lambda: fn()
 
 
-def _define_when(wdt: Clickable) -> Callable[[], bool]:
+def _define_when(wdt: Clickable, parent: BaseGui) -> Callable[[], bool]:
     return lambda: wdt.enabled
 
 
 def _iter_executable(gui: BaseGui) -> Iterable[tuple[BaseGui, Clickable]]:
     for child in gui.__magicclass_children__:
         yield from _iter_executable(child)
     for wdt in gui:
```

### Comparing `magic_class-0.7.3/magicclass/core.py` & `magic_class-0.7.4/magicclass/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from functools import wraps as functools_wraps
 import inspect
 from types import ModuleType
+import warnings
 from weakref import WeakValueDictionary
 from typing import Any, TYPE_CHECKING, Callable
 from macrokit import Symbol, Expr
 
 from magicclass._gui.class_gui import (
     ClassGuiBase,
     ClassGui,
@@ -558,15 +559,15 @@
         else:
             raise TypeError(
                 "The first argument of `get_function_gui() must be a method if "
                 "the method name is not given."
             )
     else:
         func = getattr(ui, name)
-    widget = ui[name]
+    widget: Clickable = ui[name]
 
     if not hasattr(widget, "mgui"):
         raise TypeError(f"Widget {widget} does not have FunctionGui inside it.")
 
     if widget.mgui is not None:
         return widget.mgui
 
@@ -585,14 +586,19 @@
     ----------
     ui : MagicTemplate
         Target magic-class widget.
     index : int, default is -1
         Which execution will be repeated. Any object that support list slicing can be used.
         By default the last operation will be repeated.
     """
+    warnings.warn(
+        "repeat() is deprecated and will be removed soon. Use `ui.macro.repeat_method()` "
+        "to specify call options in more detail.",
+        DeprecationWarning,
+    )
     line = ui.macro[index]
     try:
         line.eval({"ui": ui})
     except Exception as e:
         msg = e.args[0]
         msg = f"Caused by >>> {line}. {msg}"
         raise e
```

### Comparing `magic_class-0.7.3/magicclass/help.py` & `magic_class-0.7.4/magicclass/help.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/plot_api.py` & `magic_class-0.7.4/magicclass/plot_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 >>> plt.show()
 
 """
 
 from __future__ import annotations
 
 from functools import wraps
+from matplotlib.axes import Axes
 import matplotlib.pyplot as plt
+from matplotlib.figure import Figure as mpl_Figure
 from magicclass.widgets import Figure
 
-CURRENT_WIDGET: Figure = None
+CURRENT_WIDGET: Figure | None = None
 
 
 @wraps(plt.figure)
 def figure(*args, **kwargs):
     global CURRENT_WIDGET
     CURRENT_WIDGET = Figure()
     return CURRENT_WIDGET.figure
@@ -56,21 +58,21 @@
         subplot_kw=subplot_kw,
         gridspec_kw=gridspec_kw,
     )
     return fig, axs
 
 
 @wraps(plt.gcf)
-def gcf():
+def gcf() -> mpl_Figure:
     """Get current figure."""
     return CURRENT_WIDGET.figure
 
 
 @wraps(plt.gca)
-def gca():
+def gca() -> Axes:
     """Get current axis."""
     return CURRENT_WIDGET.axes[-1]
 
 
 def gcw() -> Figure:
     """Get current widget."""
     global CURRENT_WIDGET
```

### Comparing `magic_class-0.7.3/magicclass/signature.py` & `magic_class-0.7.4/magicclass/signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,17 +211,22 @@
             return_annotation=return_annotation,
             gui_options=cls.get_gui_options(self),
             caller_options=self.caller_options,
             additional_options=self.additional_options,
         )
 
 
+def is_annotated(annotation: Any) -> bool:
+    """Check if a type hint is an Annotated type."""
+    return isinstance(annotation, _AnnotatedAlias)
+
+
 def split_annotated_type(annotation: _AnnotatedAlias) -> tuple[Any, dict]:
     """Split an Annotated type into its base type and options dict."""
-    if not isinstance(annotation, _AnnotatedAlias):
+    if not is_annotated(annotation):
         raise TypeError("Type hint must be an 'Annotated' type.")
 
     typ, *meta = get_args(annotation)
     all_meta = {}
     for m in meta:
         if not isinstance(m, dict):
             raise TypeError(
```

### Comparing `magic_class-0.7.3/magicclass/undo.py` & `magic_class-0.7.4/magicclass/undo.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/_base.py` & `magic_class-0.7.4/magicclass/_gui/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 import functools
 from typing import (
     Any,
+    Union,
     Callable,
     TYPE_CHECKING,
     Iterable,
     Iterator,
     TypeVar,
     overload,
     MutableSequence,
 )
 from types import MethodType
 from abc import ABCMeta
 from typing_extensions import _AnnotatedAlias
 import inspect
 import warnings
-from qtpy.QtWidgets import QWidget, QDockWidget
+from qtpy import QtWidgets as QtW
 
 from psygnal import Signal
 from magicgui.signature import MagicParameter
 from magicgui.widgets import (
     FunctionGui,
     FileEdit,
     EmptyWidget,
@@ -85,14 +86,17 @@
 
 defaults = {
     "popup_mode": PopUpMode.popup,
     "error_mode": ErrorMode.msgbox,
     "close_on_run": True,
     "macro-max-history": 100000,
     "macro-highlight": False,
+    "macro-attribute-check": True,
+    "macro-signature-check": True,
+    "macro-name-check": True,
     "undo-max-history": 100,
 }
 
 _RESERVED = frozenset(
     {
         "__magicclass_parent__",
         "__magicclass_children__",
@@ -123,14 +127,15 @@
         "visible",
         "widget_type",
         "width",
         "wraps",
         "_unwrap_method",
         "_search_parent_magicclass",
         "_iter_child_magicclasses",
+        "_initialized",
     }
 )
 
 
 def check_override(cls: type):
     """
     Some of the methods should not be overriden because they are essential for magic
@@ -160,29 +165,30 @@
 _F = TypeVar("_F", bound=Callable)
 
 
 class _MagicTemplateMeta(ABCMeta):
     """This metaclass enables type checking of nested magicclasses."""
 
     @overload
-    def __get__(self: type[_T], obj: MagicTemplate, objtype=None) -> _T:
+    def __get__(self: type[_T], obj: Any, objtype=None) -> _T:
         ...
 
     @overload
     def __get__(self: type[_T], obj: None, objtype=None) -> type[_T]:
         ...
 
     def __get__(self, obj, objtype=None):
         return self
 
 
 _W = TypeVar("_W", bound=Widget)
+_Comp = TypeVar("_Comp", Widget, AbstractAction)
 
 
-class MagicTemplate(MutableSequence[Widget], metaclass=_MagicTemplateMeta):
+class MagicTemplate(MutableSequence[_Comp], metaclass=_MagicTemplateMeta):
     __doc__ = ""
     __magicclass_parent__: None | MagicTemplate
     __magicclass_children__: list[MagicTemplate]
     _close_on_run: bool
     _component_class: type[Action | PushButtonPlus]
     _error_mode: ErrorMode
     _list: list[Action | Widget]
@@ -201,61 +207,70 @@
     labels: bool
     margins: tuple[int, int, int, int]
     max_height: int
     max_width: int
     min_height: int
     min_width: int
     name: str
-    native: QWidget
+    native: QtW.QWidget
     options: dict
     param_kind: inspect._ParameterKind
     parent: Widget | None
     parent_changed: Signal
     tooltip: str
     visible: bool
     widget_type: str
     width: int
 
     __init_subclass__ = check_override
 
-    def show(self, run: bool = True) -> None:
-        raise NotImplementedError()
-
-    def hide(self) -> None:
-        raise NotImplementedError()
-
-    def close(self) -> None:
-        raise NotImplementedError()
-
     @overload
-    def __getitem__(self, key: int | str) -> Widget:
+    def __getitem__(self, key: int | str) -> _Comp:
         ...
 
     @overload
-    def __getitem__(self, key: slice) -> Self[Widget]:
+    def __getitem__(self, key: slice) -> list[_Comp]:
         ...
 
     def __getitem__(self, key):
         raise NotImplementedError()
 
-    if TYPE_CHECKING:
+    def __setitem__(self, key: int, value: Any):
+        raise NotImplementedError()
 
-        def __iter__(self) -> Iterator[Widget]:
-            raise NotImplementedError()
+    def __delitem__(self, key: int) -> None:
+        raise NotImplementedError()
+
+    def __len__(self) -> int:
+        raise NotImplementedError()
+
+    def __dir__(self) -> list[str]:
+        return super().__dir__()
+
+    if TYPE_CHECKING:
 
         def index(self, value: Any, start: int, stop: int) -> int:
             raise NotImplementedError()
 
-        def remove(self, value: Widget | str):
+        def remove(self, value: _Comp | str):
             raise NotImplementedError()
 
-    def _fast_insert(self, key: int, widget: Widget | Callable) -> None:
+    def show(self, run: bool = True) -> None:
+        raise NotImplementedError()
+
+    def hide(self) -> None:
         raise NotImplementedError()
 
-    def insert(self, key: int, widget: Widget | Callable) -> None:
+    def close(self) -> None:
+        raise NotImplementedError()
+
+    def _fast_insert(self, key: int, widget: _Comp | Callable) -> None:
+        raise NotImplementedError()
+
+    def insert(self, key: int, widget: _Comp | Callable) -> None:
         self._fast_insert(key, widget)
         self._unify_label_widths()
 
     def render(self) -> np.ndarray:
         raise NotImplementedError()
 
     def _unify_label_widths(self):
@@ -272,28 +287,28 @@
         else:
             return self.__magicclass_parent__.macro
 
     @property
     def parent_viewer(self) -> napari.Viewer | None:
         """Return napari.Viewer if magic class is a dock widget of a viewer."""
         parent_self = self._search_parent_magicclass()
-        if not isinstance(parent_self.native.parent(), QDockWidget):
+        if not isinstance(parent_self.native.parent(), QtW.QDockWidget):
             return None
         return _find_viewer_ancestor(parent_self.native)
 
     @property
-    def parent_dock_widget(self) -> QDockWidget | None:
+    def parent_dock_widget(self) -> QtW.QDockWidget | None:
         """
         Return dock widget object if magic class is a dock widget of a main
         window widget, such as a napari Viewer.
         """
         parent_self = self._search_parent_magicclass()
         try:
             dock = parent_self.native.parent()
-            if not isinstance(dock, QDockWidget):
+            if not isinstance(dock, QtW.QDockWidget):
                 dock = None
         except AttributeError:
             dock = None
 
         return dock
 
     def find_ancestor(self, ancestor: type[_T], cache: bool = False) -> _T:
@@ -769,15 +784,15 @@
                         start_path=str(fdialog.value),
                         filter=fdialog.filter,
                     ):
                         fdialog.value = result
                     else:
                         return None
 
-                self._popup_mode.activate_magicgui(mgui)
+                self._popup_mode.activate_magicgui(mgui, self)
                 return None
 
         widget.changed.connect(run_function)
 
         # If design is given, load the options.
         widget.from_options(func)
 
@@ -808,23 +823,19 @@
         from magicclass.core import get_function_gui
 
         fgui = get_function_gui(self, fname)
         fgui(*args, **kwargs)
         return None
 
 
-class BaseGui(MagicTemplate[_W]):
+class BaseGui(MagicTemplate[_Comp]):
     def __init__(
         self, close_on_run=True, popup_mode=PopUpMode.popup, error_mode=ErrorMode.msgbox
     ):
-        self._macro_instance = GuiMacro(
-            max_lines=defaults["macro-max-history"],
-            max_undo=defaults["undo-max-history"],
-            ui=self,
-        )
+        self._macro_instance = GuiMacro(self, options=defaults)
         self.__magicclass_parent__: BaseGui | None = None
         self.__magicclass_children__: list[MagicTemplate] = []
         self._close_on_run = close_on_run
         self._popup_mode = popup_mode or PopUpMode.popup
         self._error_mode = error_mode or ErrorMode.msgbox
         self._my_symbol = Symbol.var("ui")
         self._icon = None
@@ -843,20 +854,21 @@
             self.native.setIcon(qicon)
         else:
             self.native.setWindowIcon(qicon)
         if hasattr(self.native, "setIconSize"):
             self.native.setIconSize(self.native.size())
 
 
-class ContainerLikeGui(BaseGui[Action], mguiLike):
+class ContainerLikeGui(BaseGui[Union[Action, Widget]], mguiLike):
     # This class enables similar API between magicgui widgets and additional widgets
     # in magicclass such as menu and toolbar.
     _component_class = Action
     changed = Signal(object)
     _list: list[AbstractAction | ContainerLikeGui]
+    native: QtW.QMenu | QtW.QToolBar
 
     def reset_choices(self, *_: Any):
         """Reset child Categorical widgets"""
         all_widgets: set[Widget] = set()
 
         for item in self._list:
             widget = getattr(item, "_inner_widget", item)
@@ -895,28 +907,37 @@
                 out = obj
                 break
         if out is None:
             raise KeyError(key)
         return out
 
     def __setitem__(self, key, value):
-        raise NotImplementedError()
+        raise AttributeError("Can't set item to widgets. Use append or insert instead.")
 
     def __delitem__(self, key: int | str) -> None:
+        if isinstance(key, str):
+            key = self.index(key)
         self.native.removeAction(self[key].native)
+        del self._list[key]
 
     def __iter__(self) -> Iterator[ContainerLikeGui | AbstractAction]:
         return iter(self._list)
 
     def __len__(self) -> int:
         return len(self._list)
 
     def append(self, obj: Callable | ContainerLikeGui | AbstractAction) -> None:
         return self.insert(len(self._list), obj)
 
+    def index(self, value: Any, start: int = 0, stop: int = 9223372036854775807) -> int:
+        """Return index of a specific widget instance (or widget name)."""
+        if isinstance(value, str):
+            value = self[value]
+        return super().index(value, start, stop)
+
     def _unify_label_widths(self):
         _hide_labels = (
             _LabeledWidgetAction,
             ButtonWidget,
             FreeWidget,
             Label,
             FunctionGui,
@@ -945,15 +966,15 @@
             ) from None
         import qtpy
 
         img = self.native.grab().toImage()
         bits = img.constBits()
         h, w, c = img.height(), img.width(), 4
         if qtpy.API_NAME == "PySide2":
-            arr = np.array(bits).reshape(h, w, c)
+            arr = np.asarray(bits).reshape(h, w, c)
         else:
             bits.setsize(h * w * c)
             arr = np.frombuffer(bits, np.uint8).reshape(h, w, c)
 
         return arr[:, :, [2, 1, 0, 3]]
 
     def _repr_png_(self):
@@ -970,14 +991,32 @@
             return None
 
         with BytesIO() as file_obj:
             imsave(file_obj, self.render(), format="png")
             file_obj.seek(0)
             return file_obj.read()
 
+    def close(self):
+        """Close the widget."""
+        return self.native.close()
+
+    def hide(self):
+        """Hide the widget."""
+        return self.native.hide()
+
+    def show(self, run=True):
+        """Show the widget."""
+        return self.native.show()
+
+    def __iter__(self) -> Iterator[ContainerLikeGui | AbstractAction]:
+        return iter(self._list)
+
+    def __len__(self) -> int:
+        return len(self._list)
+
 
 def _get_widget_name(widget: Widget):
     # To escape reference
     return widget.name
 
 
 def _create_gui_method(self: BaseGui, obj: MethodType):
@@ -1109,15 +1148,15 @@
         raise MagicGuiBuildError(msg)
 
     return _connect_functiongui_event(mgui, opt)
 
 
 def _connect_functiongui_event(
     mgui: FunctionGuiPlus, opt: dict[str, Any]
-) -> FunctionGui:
+) -> FunctionGuiPlus:
     _on_calling = opt.get("on_calling", [])
     for cb in _on_calling:
         mgui.calling.connect(cb)
 
     _on_called = opt.get("on_called", [])
     for cb in _on_called:
         mgui.called.connect(lambda: cb(mgui))
@@ -1151,14 +1190,42 @@
         if child_instance.__class__.__name__ == child_clsname:
             break
     else:
         raise ValueError(f"{widget_or_name} not found.")
     return child_instance
 
 
+def convert_function(obj: Callable, default: str | None = None, is_method: bool = True):
+    """Convert function for macro recording."""
+    _record_policy = get_additional_option(obj, "record", default)
+    if _record_policy is None:
+        new_attr = inject_recorder(obj, is_method)
+    elif _record_policy == "false":
+        if is_method:
+            new_attr = obj
+        else:
+            sig = get_signature(obj)
+
+            @functools.wraps(obj)
+            def _func(self, *args, **kwargs):
+                return obj(*args, **kwargs)
+
+            _self = inspect.Parameter("self", inspect.Parameter.POSITIONAL_OR_KEYWORD)
+            _func.__signature__ = sig.replace(
+                parameters=[_self] + list(sig.parameters.values()),
+                return_annotation=sig.return_annotation,
+            )
+            new_attr = _func
+    elif _record_policy == "all-false":
+        new_attr = inject_silencer(obj, is_method)
+    else:
+        raise ValueError(f"Invalid record policy: {_record_policy}")
+    return new_attr
+
+
 def convert_attributes(
     cls: type[_T], hide: tuple[type, ...], record: bool = True
 ) -> dict[str, Any]:
     """
     Convert class attributes into macro recordable ones.
 
     Returned dictionary can be directly used for the third argument of
@@ -1195,23 +1262,15 @@
             _isfunc = callable(obj)
             if isinstance(obj, _MagicTemplateMeta):
                 new_attr = copy_class(obj, cls, name=name)
             elif name.startswith("_") or isinstance(obj, _pass) or not _isfunc:
                 # private method, non-action-like object, not-callable object are passed.
                 new_attr = obj
             elif _isfunc:
-                _record_policy = get_additional_option(obj, "record", default)
-                if _record_policy is None:
-                    new_attr = inject_recorder(obj)
-                elif _record_policy == "false":
-                    new_attr = obj
-                elif _record_policy == "all-false":
-                    new_attr = inject_silencer(obj)
-                else:
-                    raise ValueError(f"Invalid record policy: {_record_policy}")
+                new_attr = convert_function(obj, default)
             else:
                 new_attr = obj
 
             _dict[name] = new_attr
     # replace the macro object with the dummy one.
     if not record:
         _dict["macro"] = macro
@@ -1316,15 +1375,15 @@
     method: MethodType,
     self: BaseGui,
     opt: ConfirmDict,
 ):
     """Implement confirmation callback to a method."""
     sig = inspect.signature(method)
 
-    @wraps(method)
+    @functools.wraps(method)
     def _method(*args, **kwargs):
         if self[method.__name__].running:
             arguments = sig.bind(*args, **kwargs)
             arguments.apply_defaults()
             all_args = arguments.arguments
             all_args.update(self=self)
             need_confirmation = False
@@ -1363,15 +1422,15 @@
 def _empty_func(name: str) -> Callable[[Any], None]:
     """Create a named function that does nothing."""
     f = lambda x: None
     f.__name__ = name
     return f
 
 
-def _find_viewer_ancestor(widget: QWidget) -> napari.Viewer | None:
+def _find_viewer_ancestor(widget: QtW.QWidget) -> napari.Viewer | None:
     """Return the closest parent napari Viewer."""
     parent = widget.parent()
     while parent:
         if hasattr(parent, "_qt_viewer"):  # QMainWindow
             return parent._qt_viewer.viewer
 
         parent = parent.parent()
```

### Comparing `magic_class-0.7.3/magicclass/_gui/_dock_widget.py` & `magic_class-0.7.4/magicclass/_gui/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/_function_gui.py` & `magic_class-0.7.4/magicclass/_gui/_function_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/_gui_modes.py` & `magic_class-0.7.4/magicclass/_gui/_gui_modes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
-from types import TracebackType
 
+from types import TracebackType
+from contextlib import contextmanager
 from typing import Callable
 from enum import Enum
 import functools
-from magicgui.widgets import FunctionGui, Widget
+from magicgui.widgets import Widget
 from .mgui_ext import FunctionGuiPlus
+from magicclass._exceptions import Canceled
 
 
 class PopUpMode(Enum):
     """Define how to popup FunctionGui."""
 
     popup = "popup"
     first = "first"
@@ -25,39 +27,39 @@
         return self not in {
             PopUpMode.popup,
             PopUpMode.dock,
             PopUpMode.parentsub,
             PopUpMode.dialog,
         }
 
-    def activate_magicgui(self, mgui: FunctionGuiPlus):
+    def activate_magicgui(self, mgui: FunctionGuiPlus, parent: Widget):
         if self not in (
             PopUpMode.dock,
             PopUpMode.dialog,
             PopUpMode.parentsub,
         ):
             mgui.show()
         elif self is PopUpMode.dock:
             mgui.parent.show()  # show dock widget
         elif self is PopUpMode.parentsub:
             mgui.native.parent().setVisible(True)
         else:
-            mgui.exec_as_dialog(parent=self)
+            mgui.exec_as_dialog(parent=parent)
         try:
             mgui[0].native.setFocus()
         except Exception:
             pass
 
-    def connect_close_callback(self, mgui: FunctionGui):
+    def connect_close_callback(self, mgui: FunctionGuiPlus):
         if self not in {PopUpMode.dock, PopUpMode.parentsub, PopUpMode.dialog}:
-            mgui.called.connect(mgui.hide)
+            mgui.calling.connect(mgui.hide)
         elif self in {PopUpMode.dock, PopUpMode.parentsub}:
             # If FunctioGui is docked or in a subwindow, we should close
             # the parent QDockWidget/QMdiSubwindow.
-            mgui.called.connect(lambda: mgui.parent.hide())
+            mgui.calling.connect(lambda: mgui.parent.hide())
 
 
 def _msgbox_raising(e: Exception, parent: Widget):
     from ._message_box import QtErrorMessageBox
 
     return QtErrorMessageBox.raise_(e, parent=parent.native)
 
@@ -72,46 +74,68 @@
 
 def _napari_notification_raising(e: Exception, parent: Widget):
     from napari.utils.notifications import show_error
 
     return show_error(str(e))
 
 
+def _debug_raising(e: Exception, parent: Widget):
+    from magicclass.testing import GuiErrorMonitor
+
+    monitor = GuiErrorMonitor.get_instance(parent)
+    with monitor.catch():
+        raise e
+
+
 class ErrorMode(Enum):
+    """Mode to handle error raised in magicclass during manual operations."""
+
     msgbox = "msgbox"
     stderr = "stderr"
     stdout = "stdout"
     napari = "napari"
+    debug = "debug"
 
     def get_handler(self):
         """Get error handler."""
         return ErrorModeHandlers[self]
 
     def wrap_handler(self, func: Callable, parent):
         """Wrap function with the error handler."""
         handler = self.get_handler()
 
         @functools.wraps(func)
         def wrapped_func(*args, **kwargs):
             try:
                 out = func(*args, **kwargs)
+            except Canceled as e:
+                out = e  # Do not raise "Canceled" message box
             except Exception as e:
                 e.__traceback__ = _cleanup_tb(e.__traceback__)
                 handler(e, parent=parent)
                 out = e
             return out
 
         return wrapped_func
 
+    @contextmanager
+    def raise_with_handler(self, parent):
+        """Raise error with the error handler in this context."""
+        try:
+            yield
+        except Exception as e:
+            self.get_handler()(e, parent=parent)
+
 
 ErrorModeHandlers = {
     ErrorMode.msgbox: _msgbox_raising,
     ErrorMode.stderr: _stderr_raising,
     ErrorMode.stdout: _stdout_raising,
     ErrorMode.napari: _napari_notification_raising,
+    ErrorMode.debug: _debug_raising,
 }
 
 
 def _cleanup_tb(tb: TracebackType):
     """Remove useless info from a traceback object."""
     current_tb = tb
     while current_tb is not None:
```

### Comparing `magic_class-0.7.3/magicclass/_gui/_icon.py` & `magic_class-0.7.4/magicclass/_gui/_icon.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/_macro.py` & `magic_class-0.7.4/magicclass/_gui/_macro.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+from contextlib import contextmanager
 from pathlib import Path
 
 from typing import TYPE_CHECKING, Any, Callable, Iterable, overload
 import warnings
+from datetime import datetime
 from qtpy import QtWidgets as QtW, QtCore
-from macrokit import Symbol, Expr, Head, BaseMacro, parse
+from macrokit import Symbol, Expr, Head, BaseMacro, parse, symbol
+from macrokit.utils import check_call_args, check_attributes
 from magicgui.widgets import FileEdit, LineEdit, EmptyWidget, PushButton
 from magicclass.utils.qthreading import thread_worker
 
 from magicclass.widgets import CodeEdit, TabbedContainer, ScrollableContainer, Dialog
 from magicclass.utils import move_to_screen_center
 from magicclass.undo import ImplementsUndo, RedoAction, UndoCallback
 from magicclass._gui.runner import CommandRunnerMenu
@@ -19,38 +22,47 @@
 
 
 class MacroEdit(TabbedContainer):
     """A text edit embeded with a custom menu bar."""
 
     window_count = 0
 
-    def __init__(self, **kwargs):
+    def __init__(self, is_main: bool = True, **kwargs):
         super().__init__(labels=False, **kwargs)
         self.native: QtW.QWidget
         self.__magicclass_parent__: BaseGui | None = None
         self.native.setWindowTitle("Macro")
         self.native_tab_widget.setTabBarAutoHide(True)
-        self._native_macro = None
-        self._recorded_macro = None
-        self._set_menubar()
+        self._native_macro: CodeEdit | None = None
+        self._recorded_macro: CodeEdit | None = None
+        self._set_menubar(is_main=is_main)
+        self._attribute_check = True
+        self._signature_check = True
+        self._name_check = True
+        self._syntax_highlight = True
 
-    def _add_code_edit(self, name: str = "macro", native: bool = False) -> CodeEdit:
+    def _add_code_edit(self, name: str = "script", native: bool = False) -> CodeEdit:
         """Add a new code edit widget as a new tab."""
-        from magicclass._gui._base import defaults
 
         textedit = CodeEdit(name=name)
         if native:
             if self._native_macro is not None:
                 raise ValueError("Native macro already exists.")
             textedit.read_only = True
             self._native_macro = textedit
 
         self.append(textedit)
-        if defaults["macro-highlight"]:
-            textedit.syntax_highlight()
+        if self._syntax_highlight:
+            qtextedit: QtW.QTextEdit = textedit.native
+            # get background color
+            bg = qtextedit.palette().color(qtextedit.backgroundRole())
+            if sum(bg.getRgb()[:3]) > 255 * 3 / 2:
+                textedit.syntax_highlight(theme="default")
+            else:
+                textedit.syntax_highlight(theme="native")
         textedit.__magicclass_parent__ = self.__magicclass_parent__
         textedit.executing.connect(self._on_executing)
         return textedit
 
     def _on_executing(self, desc: str):
         if desc == "exec-line":
             self._execute_selected()
@@ -139,49 +151,57 @@
         """Execute macro."""
         self._execute(parse(self.textedit.value))
 
     def _create_native_duplicate(self, e=None):
         new = self.new_tab("script")
         new.value = self.native_macro.value
 
-    def new_tab(self, name: str | None = None) -> CodeEdit:
+    def new_tab(self, name: str | None = None, text: str | None = None) -> CodeEdit:
         if name is None:
             name = "script"
         # find unique name
         suffix = 0
         tab_name = name
         existing_names = {tab.name for tab in self}
         while tab_name in existing_names:
             tab_name = f"{name}-{suffix}"
             suffix += 1
         new = self._add_code_edit(tab_name)
         self.current_index = len(self) - 1
+        if text is not None:
+            new.value = text
         return new
 
-    def new_window(self, name: str = None) -> MacroEdit:
+    def new_window(
+        self, name: str | None = None, tabname: str | None = None
+    ) -> MacroEdit:
         """
         Create a new window with same parent magic class widget.
 
         Parameters
         ----------
         name : str, optional
             Widget name. This name will be the title.
+        tabname : str, optional
+            Tab name. If not given, the tab name will be "script".
 
         Returns
         -------
         MacroEdit
             New MacroEdit widget.
         """
         if name is None:
             name = f"Macro-{self.__class__.window_count}"
             self.__class__.window_count += 1
-        new = self.__class__(name=name)
+        new = self.__class__(name=name, is_main=False)
         new.__magicclass_parent__ = self.__magicclass_parent__
         new.native.setParent(self.native.parent(), new.native.windowFlags())
-        new._add_code_edit()
+        if tabname is None:
+            tabname = "script"
+        new._add_code_edit(name=tabname)
         new.show()
         geometry = self.native.geometry()
         geometry.moveTopLeft(geometry.topLeft() + QtCore.QPoint(20, 20))
         new.native.setGeometry(geometry)
         return new
 
     def duplicate(self, name: str = None):
@@ -224,39 +244,54 @@
     def _zoom_in(self, e=None):
         self.textedit.zoom_in()
 
     def _zoom_out(self, e=None):
         self.textedit.zoom_out()
 
     def show(self):
+        was_visible = self.visible
         if self.parent is None:
             ui = self.__magicclass_parent__
             self.native.setParent(ui.native, self.native.windowFlags())
         super().show()
-        move_to_screen_center(self.native)
+        if not was_visible:
+            move_to_screen_center(self.native)
         self.textedit.native.setFocus()
 
     def _execute(self, code: Expr):
         """Run macro."""
         parent = self._search_parent_magicclass()
-        try:
+        ns = {Symbol.var("ui"): parent}
+        with parent._error_mode.raise_with_handler(self):
+            if self._attribute_check:
+                strs = [f"- {exc}" for exc in check_attributes(code, ns)]
+                if strs:
+                    raise AttributeError("Attribute check failed.\n" + "\n".join(strs))
+
+            if self._signature_check:
+                strs = [f"- {exc}" for exc in check_call_args(code, ns)]
+                if strs:
+                    raise AttributeError("Signature check failed.\n" + "\n".join(strs))
+
+            if self._name_check:
+                # TODO
+                pass
+
             if str(code) == "":
                 raise ValueError("No code selected")
-            ns = {Symbol.var("ui"): parent}
             if (viewer := parent.parent_viewer) is not None:
                 ns.setdefault(Symbol.var("viewer"), viewer)
             code.eval(ns)
-        except Exception as e:
-            parent._error_mode.get_handler()(e, self)
 
     def _execute_selected(self, e=None):
         """Run selected line of macro."""
         self._execute(self.get_selected_expr())
 
     def execute_lines(self, indices: int | slice | Iterable[int]):
+        """Execute given lines"""
         all_text: str = self.textedit.value
         lines = all_text.split("\n")
         if isinstance(indices, int):
             input_text = lines[indices]
         elif isinstance(indices, slice):
             input_text = "\n".join(lines[indices])
         else:
@@ -302,15 +337,15 @@
         if self[index] is self.native_macro:
             self.new_tab("record")
         self._recorded_macro = self.textedit
 
     def _finish_recording(self):
         self._recorded_macro = None
 
-    def _set_menubar(self):
+    def _set_menubar(self, is_main: bool):
         self._menubar = QtW.QMenuBar(self.native)
         self.native.layout().setMenuBar(self._menubar)
 
         # fmt: off
         _file_menu = QtW.QMenu("File", self.native)
         _file_menu.setToolTipsVisible(True)
         self._menubar.addMenu(_file_menu)
@@ -322,15 +357,15 @@
         _file_menu.addSeparator()
         _file_menu.addAction(_action("Close", self._close, tooltip="Close this macro editor", parent=_file_menu))
 
         _tab_menu = QtW.QMenu("Tab", self.native)
         _tab_menu.setToolTipsVisible(True)
         self._menubar.addMenu(_tab_menu)
         _tab_menu.addAction(_action("New tab", self._new_tab, "Ctrl+T", tooltip="Open a new empty tab", parent=_tab_menu))
-        _tab_menu.addAction(_action("Duplicate tab", self._duplicate_tab, "Ctrl+D", tooltip="Duplicate current tab as a new tab", parent=_tab_menu))
+        _tab_menu.addAction(_action("Duplicate tab", self._duplicate_tab, "Ctrl+Shift+D", tooltip="Duplicate current tab as a new tab", parent=_tab_menu))
         _tab_menu.addAction(_action("Current macro in new tab", self._create_native_duplicate, tooltip="Duplicate current GUI macro in a new tab", parent=_tab_menu))
         _tab_menu.addAction(_action("Delete tab", self._delete_tab, "Ctrl+W", tooltip="Delete current tab", parent=_tab_menu))
         _tab_menu.addSeparator()
         _tab_menu.addAction(_action("Zoom in", self._zoom_in, "Ctrl+Shift+.", tooltip="Zoom in the text", parent=_tab_menu))
         _tab_menu.addAction(_action("Zoom out", self._zoom_out, "Ctrl+Shift+,", tooltip="Zoom out the text", parent=_tab_menu))
 
 
@@ -338,21 +373,22 @@
         _macro_menu = QtW.QMenu("Macro", self.native)
         _macro_menu.setToolTipsVisible(True)
         self._menubar.addMenu(_macro_menu)
 
         _macro_menu.addAction(_action("Execute", self.execute, "Ctrl+F5", tooltip="Execute the entire script of the current tab", parent=_macro_menu))
         _macro_menu.addAction(_action("Execute selected lines", self._execute_selected, "Ctrl+Shift+F5", tooltip="Execute the selected lines of the current tab", parent=_macro_menu))
         _macro_menu.addSeparator()
-        _action_start = _action("Start recording", self._start_recording, tooltip="Open a new tab and start recording GUI operations in it", parent=_macro_menu)
-        _macro_menu.addAction(_action_start)
-        _action_finish = _action("Finish recording", self._finish_recording, tooltip="Finish the recording task started by 'Start recording' menu", parent=_macro_menu)
-        _macro_menu.addAction(_action_finish)
-        _action_finish.setEnabled(False)
-        _action_start.triggered.connect(lambda: _action_finish.setEnabled(True))
-        _action_finish.triggered.connect(lambda: _action_finish.setEnabled(False))
+        if is_main:
+            _action_start = _action("Start recording", self._start_recording, tooltip="Open a new tab and start recording GUI operations in it", parent=_macro_menu)
+            _macro_menu.addAction(_action_start)
+            _action_finish = _action("Finish recording", self._finish_recording, tooltip="Finish the recording task started by 'Start recording' menu", parent=_macro_menu)
+            _macro_menu.addAction(_action_finish)
+            _action_finish.setEnabled(False)
+            _action_start.triggered.connect(lambda: _action_finish.setEnabled(True))
+            _action_finish.triggered.connect(lambda: _action_finish.setEnabled(False))
 
         self._command_menu = CommandRunnerMenu(
             "Command",
             parent=self.native,
             magicclass_parent=self._search_parent_magicclass(),
         )
         self._command_menu.native.setToolTipsVisible(True)
@@ -376,34 +412,116 @@
     if shortcut:
         action.setShortcut(shortcut)
     if tooltip:
         action.setToolTip(tooltip)
     return action
 
 
+class PropertyGroup:
+    def __init__(self, parent: GuiMacro | None = None):
+        self._instances: dict[int, PropertyGroup] = {}
+        self._parent = parent
+        self._max_lines = 10000
+        self._max_undo = 100
+
+    def __get__(self, instance: GuiMacro, owner) -> PropertyGroup:
+        if instance is None:
+            return self
+        return self._instances.setdefault(id(instance), self.__class__(parent=instance))
+
+    @property
+    def macro(self) -> GuiMacro:
+        if self._parent is None:
+            raise RuntimeError("This property group is not bound to any macro.")
+        return self._parent
+
+    @property
+    def max_lines(self) -> int:
+        return self._max_lines
+
+    @max_lines.setter
+    def max_lines(self, value: int):
+        if value < 0:
+            raise ValueError("max_lines must be >= 0")
+        if value < len(self.macro):
+            raise ValueError("max_lines must be larger than current number of lines")
+        self._max_lines = value
+
+    @property
+    def max_undo(self) -> int:
+        return self._max_undo
+
+    @max_undo.setter
+    def max_undo(self, value: int):
+        if value < 0:
+            raise ValueError("max_undo must be >= 0")
+        if value < len(self.macro._stack_undo):
+            raise ValueError(
+                "max_undo must be larger than current number of undo steps"
+            )
+        self._max_undo = value
+
+    @property
+    def syntax_highlight(self) -> bool:
+        return self.macro.widget._syntax_highlight
+
+    @syntax_highlight.setter
+    def syntax_highlight(self, value: bool):
+        self.macro.widget._syntax_highlight = bool(value)
+
+    @property
+    def attribute_check(self) -> bool:
+        return self.macro.widget._attribute_check
+
+    @attribute_check.setter
+    def attribute_check(self, value: bool):
+        self.macro.widget._attribute_check = bool(value)
+
+    @property
+    def signature_check(self) -> bool:
+        return self.macro.widget._signature_check
+
+    @signature_check.setter
+    def signature_check(self, value: bool):
+        self.macro.widget._signature_check = bool(value)
+
+    @property
+    def name_check(self) -> bool:
+        return self.macro.widget._name_check
+
+    @name_check.setter
+    def name_check(self, value: bool):
+        self.macro.widget._name_check = bool(value)
+
+
 class GuiMacro(BaseMacro):
     """Macro object with GUI-specific functions."""
 
-    def __init__(self, ui: BaseGui = None, max_lines: int = 10000, max_undo: int = 100):
-        from datetime import datetime
+    options = PropertyGroup()
 
+    def __init__(self, ui: BaseGui = None, options: dict[str, Any] = {}):
+        self._blocking_sources = []
         super().__init__()
-        self._max_lines = max_lines
-        self._max_undo = max_undo
         self.on_appended.append(self._on_macro_added)
         self.on_popped.append(self._on_macro_popped)
 
         self._widget = MacroEdit(name="Macro")
         self._widget.__magicclass_parent__ = ui
         self._widget._add_code_edit(native=True)
         now = datetime.now()
         self.append(Expr(Head.comment, [now.strftime("%Y/%m/%d %H:%M:%S")]))
 
         self._stack_undo: list[ImplementsUndo] = []
         self._stack_redo: list[tuple[Expr, ImplementsUndo]] = []
+        self.options.max_lines = options.get("macro-max-history", 10000)
+        self.options.max_undo = options.get("undo-max-history", 100)
+        self.options.syntax_highlight = options.get("macro-highlight", False)
+        self.options.attribute_check = options.get("macro-attribute-check", True)
+        self.options.signature_check = options.get("macro-signature-check", True)
+        self.options.name_check = options.get("macro-name-check", True)
 
     @property
     def widget(self) -> MacroEdit:
         """Returns the macro editor."""
         return self._widget
 
     @property
@@ -412,29 +530,36 @@
         return self.widget.__magicclass_parent__
 
     def clear_undo_stack(self) -> None:
         """Clear all the history of undo/redo."""
         self._stack_undo.clear()
         self._stack_redo.clear()
 
-    def append_with_undo(self, expr: Expr, undo: UndoCallback) -> None:
+    def append_with_undo(
+        self,
+        expr: Expr,
+        undo: UndoCallback,
+        redo: Callable[[], Any] | None = None,
+    ) -> None:
         """Append an expression with its undo action."""
         if not isinstance(undo, UndoCallback):
             if callable(undo):
                 undo = UndoCallback(undo)
             else:
                 raise TypeError(f"undo must be callable, not {type(undo)}")
+        if redo is not None:
+            undo = undo.with_redo(redo)
         self.append(expr)
         self._append_undo(undo)
         return None
 
     def _append_undo(self, undo: ImplementsUndo) -> None:
         self._stack_undo.append(undo)
         self._stack_redo.clear()
-        if len(self._stack_undo) > self._max_undo:
+        if len(self._stack_undo) > self.options.max_undo:
             self._stack_undo.pop(0)
         return None
 
     def _pop_undo(self) -> ImplementsUndo:
         return self._stack_undo.pop()
 
     @property
@@ -510,14 +635,39 @@
         ...
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             return BaseMacro(self._args)[key]
         return super().__getitem__(key)
 
+    @contextmanager
+    def blocked(self, source: Any | None = None):
+        """Block macro recording in this context."""
+        self._blocking_sources.append(source)
+        try:
+            yield
+        finally:
+            try:
+                # `source` should be considered in the future
+                self._blocking_sources.pop()
+            except IndexError:
+                pass
+
+    @property
+    def active(self) -> bool:
+        """Macro is active if it is not blocked."""
+        return len(self._blocking_sources) == 0
+
+    @active.setter
+    def active(self, value: bool):
+        if value:
+            self._blocking_sources.clear()
+        else:
+            raise NotImplementedError("Cannot set active=False")
+
     def subset(self, indices: Iterable[int]) -> BaseMacro:
         """Generate a subset of macro."""
         args = [self._args[i] for i in indices]
         return BaseMacro(args)
 
     def get_command(self, key: int) -> Callable[[], Any]:
         """Get the command function at the give index."""
@@ -580,47 +730,57 @@
         assert _ui == ui._my_symbol
         ins = ui
         for attr in _attributes:
             ins = getattr(ins, attr.name)
 
         wdt: Clickable = ins[_last.name]
         if wdt.mgui is None:
-            raise ValueError(f"Method {_object} is not called yet.")
+            # If macro is added by users, the internal magicgui will not be tagged
+            # to the button. Create one here.
+            from ._base import _build_mgui, _create_gui_method
+
+            func = _create_gui_method(ui, getattr(ins, _last.name))
+            wdt.mgui = _build_mgui(wdt, func, ui)
+
         if check_nargs and not same_args:
             n_widget_args = sum(
                 not isinstance(w, EmptyWidget)
                 for w in wdt.mgui
                 if not isinstance(w, PushButton)
             )
             if n_widget_args == 0:
                 raise ValueError(f"Method {_object} does not have any arguments.")
 
         if not blocking:
             if same_args:
+                _args, _kwargs = self[index].eval_call_args({symbol(ui): ui})
+                _input = wdt.mgui.__signature__.bind_partial(_args, _kwargs).arguments
+                with wdt.mgui.changed.blocked():
+                    wdt.mgui.update(**_input)
                 wdt.mgui.call_button.changed()  # click the call button
             else:
                 wdt.changed()  # click the button to open magicgui
         else:
             if same_args:
-                wdt.mgui()  # call the method
+                self[index].eval({symbol(ui): ui})  # call the method
             else:
                 if isinstance(wdt.mgui._function, thread_worker):
                     raise ValueError(
                         "same_args=False is not supported for blocking=True."
                     )
                 wdt.changed()  # save as blocking=False for non-thread worker
         return None
 
     def _on_macro_added(self, expr=None):
         line = str(self.args[-1])
         if wdt := self.widget.native_macro:
             wdt.append(line)
         if wdt := self.widget.recorded_macro:
             wdt.append(line)
-        if len(self) > self._max_lines:
+        if len(self) > self.options.max_lines:
             del self[0]
 
     def _on_macro_popped(self, expr=None):
         self._erase_last()
 
     def _erase_last(self):
         if wdt := self.widget.native_macro:
```

### Comparing `magic_class-0.7.3/magicclass/_gui/_macro_utils.py` & `magic_class-0.7.4/magicclass/_gui/_macro_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,16 +230,15 @@
     else:
         _auto_call = False
 
     if sig.return_annotation is inspect.Parameter.empty:
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
-            kwargs = dict(bound.arguments.items())
-            expr = Expr.parse_method(bgui, func, (), kwargs)
+            expr = Expr.parse_method(bgui, func, *_format_arguments(bound))
             if _auto_call:
                 # Auto-call will cause many redundant macros. To avoid this, only the last
                 # input will be recorded in magic-class.
                 last_expr = bgui.macro[-1]
                 if (
                     last_expr.head == Head.call
                     and last_expr.args[0].head == Head.getattr
@@ -259,16 +258,16 @@
             return None
 
     else:
         _cname_ = "_call_with_return_callback"
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
-            kwargs = dict(bound.arguments.items())
-            expr = Expr.parse_method(bgui, _cname_, (func.__name__,), kwargs)
+            _args, _kwargs = _format_arguments(bound)
+            expr = Expr.parse_method(bgui, _cname_, (func.__name__,) + _args, _kwargs)
             if _auto_call:
                 # Auto-call will cause many redundant macros. To avoid this, only the last
                 # input will be recorded in magic-class.
                 last_expr = bgui.macro[-1]
                 if (
                     last_expr.head == Head.call
                     and last_expr.args[0].head == Head.getattr
@@ -297,16 +296,15 @@
         _auto_call = False
 
     if sig.return_annotation is inspect.Parameter.empty:
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
             bound.apply_defaults()
-            kwargs = bound.arguments
-            expr = Expr.parse_method(bgui, base_func, (), kwargs)
+            expr = Expr.parse_method(bgui, base_func, *_format_arguments(bound))
             if _auto_call:
                 # Auto-call will cause many redundant macros. To avoid this, only the last
                 # input will be recorded in magic-class.
                 last_expr = bgui.macro[-1]
                 if (
                     last_expr.head == Head.call
                     and last_expr.args[0].head == Head.getattr
@@ -328,15 +326,18 @@
     else:
         _cname_ = "_call_with_return_callback"
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
             bound.apply_defaults()
             kwargs = bound.arguments
-            expr = Expr.parse_method(bgui, _cname_, (base_func.__name__,), kwargs)
+            _args, _kwargs = _format_arguments(bound)
+            expr = Expr.parse_method(
+                bgui, _cname_, (base_func.__name__,) * _args, _kwargs
+            )
             if _auto_call:
                 # Auto-call will cause many redundant macros. To avoid this, only the last
                 # input will be recorded in magic-class.
                 last_expr = bgui.macro[-1]
                 if (
                     last_expr.head == Head.call
                     and last_expr.args[0].head == Head.getattr
@@ -355,7 +356,20 @@
 
 def _is_recordable(func: Callable):
     if hasattr(func, _IS_RECORDABLE):
         return getattr(func, _IS_RECORDABLE)
     if hasattr(func, "__func__"):
         return _is_recordable(func.__func__)
     return False
+
+
+def _format_arguments(bound: inspect.BoundArguments):
+    """Use keyword argument as much as possible"""
+    args = []
+    kwargs = {}
+    bound.apply_defaults()
+    for name, param in bound.signature.parameters.items():
+        if param.kind is inspect.Parameter.POSITIONAL_ONLY:
+            args.append(bound.arguments[name])
+        else:
+            kwargs[name] = bound.arguments[name]
+    return tuple(args), kwargs
```

### Comparing `magic_class-0.7.3/magicclass/_gui/_message_box.py` & `magic_class-0.7.4/magicclass/_gui/_message_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from __future__ import annotations
-import sys
 import re
 from typing import Callable, Generator
 from qtpy.QtWidgets import QMessageBox, QTextEdit, QDialog, QVBoxLayout
-
-if sys.platform == "win32":
-    _FONT = "Consolas"
-else:
-    _FONT = "Menlo"
+from magicclass.widgets._const import FONT
 
 
 class QtTracebackDialog(QDialog):
     """A dialog box that shows Python traceback."""
 
     def __init__(self, parent):
         super().__init__(parent)
         self.setWindowTitle("Traceback")
         layout = QVBoxLayout()
         self.setLayout(layout)
 
         # prepare text edit
         self._text = QTextEdit(self)
         self._text.setReadOnly(True)
-        self._text.setFontFamily(_FONT)
+        self._text.setFontFamily(FONT)
         self._text.setLineWrapMode(QTextEdit.LineWrapMode.NoWrap)
         layout.addWidget(self._text)
 
         self.resize(600, 400)
 
     def setText(self, text: str):
         """Always set text as a HTML text."""
@@ -135,15 +130,15 @@
                     vbtb.text(*info)
                     .replace(" ", "&nbsp;")
                     .replace("<", "&lt;")
                     .replace(">", "&gt;")
                 )
                 html = "".join(ansi2html(ansi_string)).replace("\n", "<br>")
                 html = (
-                    f"<span style='font-family: monaco,{_FONT},monospace;'>"
+                    f"<span style='font-family: monaco,{FONT},monospace;'>"
                     + html
                     + "</span>"
                 )
                 tb_text = html
             else:
                 tb_text = vbtb.text(*info)
 
@@ -215,15 +210,15 @@
                     "function calls leading up to the error, "
                     "in the order they occurred.</p>",
                     "<br>",
                 )
                 # remove hardcoded fonts
                 html = html.replace("\n", "<br>")
                 html = (
-                    f"<span style='font-family: monaco,{_FONT},monospace;'>"
+                    f"<span style='font-family: monaco,{FONT},monospace;'>"
                     + html
                     + "</span>"
                 )
                 tb_text = html
             else:
                 # if we don't need HTML, just use traceback
                 tb_text = "".join(traceback.format_exception(*info))
```

### Comparing `magic_class-0.7.3/magicclass/_gui/_napari_type.py` & `magic_class-0.7.4/magicclass/_gui/_napari_type.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/class_gui.py` & `magic_class-0.7.4/magicclass/_gui/class_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from typing import Any, Callable, Sequence, TypeVar
 import warnings
 from psygnal import Signal
 from qtpy.QtWidgets import QMenuBar, QWidget, QMainWindow, QBoxLayout, QDockWidget
 from qtpy.QtCore import Qt
+from magicgui.application import use_app
 from magicgui.widgets import (
     Container,
     MainWindow,
     Label,
     FunctionGui,
     Image,
     Table,
@@ -27,14 +28,15 @@
 from .mgui_ext import PushButtonPlus
 from .toolbar import ToolBarGui, QtTabToolBar
 from .menu_gui import MenuGui, ContextMenuGui
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
+    convert_function,
 )
 from .utils import format_error, connect_magicclasses
 from ._macro_utils import value_widget_callback, nested_function_gui_callback
 from magicclass.widgets import (
     ButtonContainer,
     GroupBoxContainer,
     FrameContainer,
@@ -296,38 +298,23 @@
             # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 widget = obj
             else:
-                from ._base import inject_recorder
-
-                obj = inject_recorder(obj, is_method=False).__get__(self)
+                obj = convert_function(obj, is_method=False).__get__(self)
                 widget = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             widget = obj
 
-        # _hide_labels should not contain Container because some ValueWidget like widgets
-        # are Containers.
-        _hide_labels = (
-            _LabeledWidget,
-            ButtonWidget,
-            ClassGuiBase,
-            FreeWidget,
-            Label,
-            Image,
-            Table,
-            FunctionGui,
-        )
-
         if isinstance(widget, (ValueWidget, ContainerWidget)):
             widget.changed.connect(lambda: self.changed.emit(self))
 
         if hasattr(widget, _MCLS_PAREMT) or hasattr(widget.__class__, _MCLS_PAREMT):
             widget.__magicclass_parent__ = self
             if isinstance(widget, ClassGuiBase):
                 if self._remove_child_margins:
@@ -340,29 +327,143 @@
                     self.__magicclass_children__.append(widget)
                     widget._my_symbol = Symbol(widget.name)
 
         _widget = widget
 
         if self.labels:
             # no labels for button widgets (push buttons, checkboxes, have their own)
-            if not isinstance(widget, _hide_labels) and not remove_label:
+            if not isinstance(widget, _HIDE_LABELS) and not remove_label:
                 _widget = _LabeledWidget(widget)
                 widget.label_changed.connect(self._unify_label_widths)
 
         if key < 0:
             key += len(self)
         self._list.insert(key, widget)
         self._widget._mgui_insert_widget(key, _widget)
 
         # NOTE: Function GUI is invisible by some reason...
         # See https://github.com/hanjinliu/magic-class/issues/53
         if isinstance(widget, FunctionGui):
             widget.visible = True
         return None
 
+    def insert(self, key: int, widget: Widget) -> None:
+        """Insert widget at the give position."""
+        self._fast_insert(key, widget)
+        self._unify_label_widths()
+        return None
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        if not isinstance(getattr(self.__class__, name, None), MagicField):
+            Container.__setattr__(self, name, value)
+        else:
+            object.__setattr__(self, name, value)
+
+    def reset_choices(self, *_: Any):
+        """Reset child Categorical widgets"""
+        all_widgets: set[Widget] = set()
+
+        for item in self._list:
+            widget = getattr(item, "_inner_widget", item)
+            all_widgets.add(widget)
+        for widget in self.__magicclass_children__:
+            all_widgets.add(widget)
+
+        for w in all_widgets:
+            if hasattr(w, "reset_choices"):
+                w.reset_choices()
+        return None
+
+    def show(self, run: bool = True) -> None:
+        """
+        Show GUI. If any of the parent GUI is a dock widget in napari, then this
+        will also show up as a dock widget (floating if in popup mode).
+
+        Parameters
+        ----------
+        run : bool, default is True
+            *Unlike magicgui, this parameter should always be True* unless you want
+            to close the window immediately. If true, application gets executed if
+            needed.
+        """
+        mcls_parent = self.__magicclass_parent__
+        if mcls_parent is not None and self.parent is None:
+            # If child magic class is closed before, we have to set parent again.
+            self.native.setParent(mcls_parent.native, self.native.windowFlags())
+
+        viewer = self.parent_viewer
+        if viewer is not None and self.parent is not None:
+            name = self.parent.objectName()
+            if name in viewer.window._dock_widgets and isinstance(
+                self.parent, QDockWidget
+            ):
+                viewer.window._dock_widgets[name].show()
+            else:
+                _floating = self._popup_mode == PopUpMode.popup
+                _area = "left" if _floating else "right"
+                dock = viewer.window.add_dock_widget(
+                    self,
+                    name=self.name.replace("_", " ").strip(),
+                    area=_area,
+                    allowed_areas=["left", "right"],
+                )
+                dock.setFloating(_floating)
+        else:
+            Container.show(self, run=False)
+            if mcls_parent is not None:
+                topleft = mcls_parent.native.geometry().topLeft()
+                topleft.setX(topleft.x() + 20)
+                topleft.setY(topleft.y() + 20)
+                self.native.move(topleft)
+            self.native.activateWindow()
+            if run:
+                run_app()
+        return None
+
+    def close(self):
+        """Close GUI. if this widget is a dock widget, then also close it."""
+
+        current_self = self._search_parent_magicclass()
+
+        viewer = current_self.parent_viewer
+        if viewer is not None:
+            try:
+                viewer.window.remove_dock_widget(self.parent)
+            except Exception:
+                pass
+
+        Container.close(self)
+
+        return None
+
+    def _unify_label_widths(self):
+        if not self._initialized:
+            return
+
+        need_labels = [w for w in self._list if not isinstance(w, _HIDE_LABELS)]
+        if self.layout == "vertical" and self.labels and need_labels:
+            measure = use_app().get_obj("get_text_width")
+            widest_label = max(measure(w.label) for w in need_labels)
+            for w in self:
+                labeled_widget = w._labeled_widget()
+                if labeled_widget:
+                    labeled_widget.label_width = widest_label
+
+
+_HIDE_LABELS = (
+    _LabeledWidget,
+    ButtonWidget,
+    ClassGuiBase,
+    FreeWidget,
+    Label,
+    Image,
+    Table,
+    FunctionGui,
+)
+
 
 def find_window_ancestor(widget: Widget) -> SubWindowsClassGui:
     """
     Try to find a window ancestor of the given widget.
 
     This function is used only for subwindows.
     """
@@ -421,111 +522,15 @@
 
             self._menubar = None
             self._toolbar = None
 
             self.native.setObjectName(self.name)
             self.native.setWindowTitle(self.name)
 
-        # ui["x"] will not return widget if x is a MagicValueField.
-        # To ensure __getitem__ returns a Widget, this method should be overriden.
-        def __getitem__(self: ClassGuiBase, key):
-            """Get item by integer, str, or slice."""
-            if isinstance(key, str):
-                for widget in self._list:
-                    if key == widget.name:
-                        return widget
-            return container.__getattr__(self, key)
-
-        def __setattr__(self, name: str, value: Any) -> None:
-            if not isinstance(getattr(self.__class__, name, None), MagicField):
-                container.__setattr__(self, name, value)
-            else:
-                object.__setattr__(self, name, value)
-
-        def insert(self: ClassGuiBase, key: int, widget: Widget) -> None:
-            self._fast_insert(key, widget)
-            self._unify_label_widths()
-            return None
-
-        def reset_choices(self: ClassGuiBase, *_: Any):
-            """Reset child Categorical widgets"""
-            all_widgets: set[Widget] = set()
-
-            for item in self._list:
-                widget = getattr(item, "_inner_widget", item)
-                all_widgets.add(widget)
-            for widget in self.__magicclass_children__:
-                all_widgets.add(widget)
-
-            for w in all_widgets:
-                if hasattr(w, "reset_choices"):
-                    w.reset_choices()
-            return None
-
-        def show(self: ClassGuiBase, run: bool = True) -> None:
-            """
-            Show GUI. If any of the parent GUI is a dock widget in napari, then this
-            will also show up as a dock widget (floating if in popup mode).
-
-            Parameters
-            ----------
-            run : bool, default is True
-                *Unlike magicgui, this parameter should always be True* unless you want
-                to close the window immediately. If true, application gets executed if
-                needed.
-            """
-            mcls_parent = self.__magicclass_parent__
-            if mcls_parent is not None and self.parent is None:
-                # If child magic class is closed before, we have to set parent again.
-                self.native.setParent(mcls_parent.native, self.native.windowFlags())
-
-            viewer = self.parent_viewer
-            if viewer is not None and self.parent is not None:
-                name = self.parent.objectName()
-                if name in viewer.window._dock_widgets and isinstance(
-                    self.parent, QDockWidget
-                ):
-                    viewer.window._dock_widgets[name].show()
-                else:
-                    _floating = self._popup_mode == PopUpMode.popup
-                    _area = "left" if _floating else "right"
-                    dock = viewer.window.add_dock_widget(
-                        self,
-                        name=self.name.replace("_", " ").strip(),
-                        area=_area,
-                        allowed_areas=["left", "right"],
-                    )
-                    dock.setFloating(_floating)
-            else:
-                container.show(self, run=False)
-                if mcls_parent is not None:
-                    topleft = mcls_parent.native.geometry().topLeft()
-                    topleft.setX(topleft.x() + 20)
-                    topleft.setY(topleft.y() + 20)
-                    self.native.move(topleft)
-                self.native.activateWindow()
-                if run:
-                    run_app()
-            return None
-
-        def close(self: ClassGuiBase):
-            """Close GUI. if this widget is a dock widget, then also close it."""
-
-            current_self = self._search_parent_magicclass()
-
-            viewer = current_self.parent_viewer
-            if viewer is not None:
-                try:
-                    viewer.window.remove_dock_widget(self.parent)
-                except Exception:
-                    pass
-
-            container.close(self)
-
-            return None
+        close = ClassGuiBase.close
 
         if issubclass(container, MainWindow):
             # Similar to napari's viewer.window.add_dock_widget.
             # See napari/_qt/widgets/qt_viewer_dock_widget.py
             from magicclass.wrappers import nogui
 
             # This function will be detected as non-reserved method so that magicclass will
@@ -588,15 +593,15 @@
                         break
                 else:
                     raise RuntimeError("Dock widget not found.")
 
                 self.native.removeDockWidget(dock)
                 self.__magicclass_children__.pop(i_dock)
 
-            def close(self: ClassGuiBase):
+            def close(self: MainWindowClassGui):
                 """Close GUI."""
                 self.native.close()
                 return None
 
             @property
             def status(self: MainWindowClassGui) -> str:
                 """Get status tip."""
@@ -609,92 +614,56 @@
                 self.native.statusBar().showMessage(text, 5000)
 
             cls.add_dock_widget = add_dock_widget
             cls.remove_dock_widget = remove_dock_widget
             cls.status = status
 
         cls.__init__ = __init__
-        cls.__setattr__ = __setattr__
-        cls.insert = insert
-        cls.show = show
-        cls.reset_choices = reset_choices
+        cls.__delitem__ = container.__delitem__
+        cls.__iter__ = container.__iter__
+        cls.__len__ = container.__len__
+        cls.__dir__ = ClassGuiBase.__dir__
+        cls._unify_label_widths = ClassGuiBase._unify_label_widths
+        cls.__setattr__ = ClassGuiBase.__setattr__
+        cls.insert = ClassGuiBase.insert
+        cls.show = ClassGuiBase.show
+        cls.reset_choices = ClassGuiBase.reset_choices
         cls.close = close
         cls._container_widget = container
         cls._remove_child_margins = no_margin
         return cls
 
     return wrapper
 
 
+# fmt: off
 @make_gui(Container)
-class ClassGui:
-    pass
-
-
+class ClassGui: pass
 @make_gui(SplitterContainer)
-class SplitClassGui:
-    pass
-
-
+class SplitClassGui: pass
 @make_gui(ScrollableContainer)
-class ScrollableClassGui:
-    pass
-
-
+class ScrollableClassGui: pass
 @make_gui(DraggableContainer)
-class DraggableClassGui:
-    pass
-
-
+class DraggableClassGui: pass
 @make_gui(CollapsibleContainer)
-class CollapsibleClassGui:
-    pass
-
-
+class CollapsibleClassGui: pass
 @make_gui(HCollapsibleContainer)
-class HCollapsibleClassGui:
-    pass
-
-
+class HCollapsibleClassGui: pass
 @make_gui(ButtonContainer)
-class ButtonClassGui:
-    pass
-
-
+class ButtonClassGui: pass
 @make_gui(ToolBoxContainer, no_margin=False)
-class ToolBoxClassGui:
-    pass
-
-
+class ToolBoxClassGui: pass
 @make_gui(TabbedContainer, no_margin=False)
-class TabbedClassGui:
-    pass
-
-
+class TabbedClassGui: pass
 @make_gui(StackedContainer, no_margin=False)
-class StackedClassGui:
-    pass
-
-
+class StackedClassGui: pass
 @make_gui(ListContainer, no_margin=False)
-class ListClassGui:
-    pass
-
-
+class ListClassGui: pass
 @make_gui(SubWindowsContainer, no_margin=False)
-class SubWindowsClassGui:
-    pass
-
-
+class SubWindowsClassGui: pass
 @make_gui(GroupBoxContainer, no_margin=False)
-class GroupBoxClassGui:
-    pass
-
-
+class GroupBoxClassGui: pass
 @make_gui(FrameContainer, no_margin=False)
-class FrameClassGui:
-    pass
-
-
+class FrameClassGui: pass
 @make_gui(MainWindow)
-class MainWindowClassGui:
-    pass
+class MainWindowClassGui: pass
+# fmt: on
```

### Comparing `magic_class-0.7.3/magicclass/_gui/keybinding.py` & `magic_class-0.7.4/magicclass/_gui/keybinding.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/menu_gui.py` & `magic_class-0.7.4/magicclass/_gui/menu_gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from .mgui_ext import AbstractAction, WidgetAction, _LabeledWidgetAction
 from .keybinding import register_shortcut
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
     ContainerLikeGui,
+    convert_function,
 )
 from .utils import format_error, connect_magicclasses
-from ._macro_utils import nested_function_gui_callback, inject_recorder
+from ._macro_utils import nested_function_gui_callback
 
 from magicclass.signature import get_additional_option
 from magicclass.fields import MagicField
 from magicclass.widgets import Separator, FreeWidget
 from magicclass.utils import iter_members, Tooltips
 
 
@@ -164,34 +165,37 @@
 
         self._unify_label_widths()
         return None
 
     def _fast_insert(
         self,
         key: int,
-        obj: Callable | MenuGuiBase | AbstractAction,
+        obj: Callable | MenuGuiBase | AbstractAction | Widget,
         remove_label: bool = False,
     ) -> None:
         if isinstance(obj, Callable):
             # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 _obj = obj
             else:
-                obj = inject_recorder(obj, is_method=False).__get__(self)
+                obj = convert_function(obj, is_method=False).__get__(self)
                 _obj = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             _obj = obj
 
+        if isinstance(_obj, Widget):
+            _obj = WidgetAction(_obj)
+
         if isinstance(_obj, (self._component_class, MenuGuiBase)):
             insert_action_like(self.native, key, _obj.native)
             self._list.insert(key, _obj)
 
         elif isinstance(_obj, WidgetAction):
             from .toolbar import ToolBarGui
```

### Comparing `magic_class-0.7.3/magicclass/_gui/mgui_ext.py` & `magic_class-0.7.4/magicclass/_gui/mgui_ext.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/runner.py` & `magic_class-0.7.4/magicclass/_gui/runner.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/_gui/toolbar.py` & `magic_class-0.7.4/magicclass/_gui/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from .mgui_ext import AbstractAction, _LabeledWidgetAction, WidgetAction, ToolButtonPlus
 from .keybinding import register_shortcut
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
     ContainerLikeGui,
+    convert_function,
 )
 from .utils import format_error, connect_magicclasses
 from .menu_gui import ContextMenuGui, MenuGui, MenuGuiBase, insert_action_like
-from ._macro_utils import inject_recorder, nested_function_gui_callback
+from ._macro_utils import nested_function_gui_callback
 
 from magicclass.signature import get_additional_option
 from magicclass.fields import MagicField
 from magicclass.widgets import FreeWidget, Separator
 from magicclass.utils import iter_members, Tooltips
 
 if TYPE_CHECKING:
@@ -242,15 +243,15 @@
             # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 _obj = obj
             else:
-                obj = inject_recorder(obj, is_method=False).__get__(self)
+                obj = convert_function(obj, is_method=False).__get__(self)
                 _obj = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             _obj = obj
```

### Comparing `magic_class-0.7.3/magicclass/_gui/utils.py` & `magic_class-0.7.4/magicclass/_gui/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 from typing import Any, TYPE_CHECKING, Callable, TypeVar
 from types import FunctionType
 
-from magicgui import __version__ as _magicgui_version
 from magicgui.widgets import FunctionGui, Widget
 from magicgui.types import Undefined
 from magicgui.type_map import get_widget_class
 from magicgui.signature import magic_signature, MagicParameter
 
 from macrokit import Symbol
 from magicclass.signature import split_annotated_type
```

### Comparing `magic_class-0.7.3/magicclass/ext/_doc.py` & `magic_class-0.7.4/magicclass/ext/_doc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/dask/progress.py` & `magic_class-0.7.4/magicclass/ext/dask/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from functools import wraps
 import inspect
 from typing import Any, Callable, TYPE_CHECKING
 from dask.diagnostics import Callback as DaskCallback
 from psygnal import Signal
 from superqt.utils import FunctionWorker, GeneratorWorker, create_worker
 
@@ -26,15 +27,18 @@
     def __init__(
         self,
         max: int = 100,
         minimum: float = 0.5,
         dt: float = 0.1,
     ):
         self._minimum = minimum
+        self._worker: FunctionWorker | GeneratorWorker | None = None
         self._dt = dt
+        self._state = None
+        self._running = False
         self._frac = 0.0
         self._n_computation = 0
         super().__init__(max=max)
         self._computed_signal = QtSignal()
         self._computed_signal.connect(self._on_computed)
         self._new_cycle_signal = QtSignal()
```

### Comparing `magic_class-0.7.3/magicclass/ext/dask/resource.py` & `magic_class-0.7.4/magicclass/ext/dask/resource.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/napari/_magicgui.py` & `magic_class-0.7.4/magicclass/ext/napari/_magicgui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/napari/types.py` & `magic_class-0.7.4/magicclass/ext/napari/types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/napari/utils.py` & `magic_class-0.7.4/magicclass/ext/napari/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/napari/viewer.py` & `magic_class-0.7.4/magicclass/ext/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/napari/widgets.py` & `magic_class-0.7.4/magicclass/ext/napari/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pandas/_viewer.py` & `magic_class-0.7.4/magicclass/ext/pandas/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pandas/tests/test_viewer.py` & `magic_class-0.7.4/magicclass/ext/pandas/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/polars/_viewer.py` & `magic_class-0.7.4/magicclass/ext/polars/_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         rstart = start.row()
         rstop = stop.row() + 1
         cstart = start.column()
         cstop = stop.column() + 1
         df = self.model().df
         columns = df.columns[cstart:cstop]
         df_sub = df.select(columns)[rstart:rstop]
-        text = df_sub.write_csv(sep="\t")
+        text = df_sub.write_csv(separator="\t")
         clipboard = QtGui.QGuiApplication.clipboard()
         clipboard.setText(text)
 
     if TYPE_CHECKING:  # pragma: no cover
 
         def model(self) -> QDataFrameModel:
             ...
```

### Comparing `magic_class-0.7.3/magicclass/ext/polars/tests/test_viewer.py` & `magic_class-0.7.4/magicclass/ext/polars/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/__init__.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/components.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/graph_items.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/graph_items.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/mouse_event.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/mouse_event.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/plot_api.py` & `magic_class-0.7.4/magicclass/ext/vispy/plot_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
-
-from typing import overload, TYPE_CHECKING, Sequence
+from typing import overload, TYPE_CHECKING
 import numpy as np
-from .widgets import QtPlotCanvas, QtMultiPlotCanvas, QtImageCanvas
+from .widgets2d import VispyPlotCanvas, VispyMultiPlotCanvas, VispyImageCanvas
 
 if TYPE_CHECKING:
-    from .widgets import HasViewBox, _MultiPlot
+    from .widgets2d import Has2DViewBox, MultiPlot
 
-CURRENT_MULTI_CANVAS: _MultiPlot | None = None
-CURRENT_CANVAS: HasViewBox | None = None
+CURRENT_MULTI_CANVAS: MultiPlot | None = None
+CURRENT_CANVAS: Has2DViewBox | None = None
 
 
-def gca() -> QtPlotCanvas:
+def gca() -> VispyPlotCanvas:
     global CURRENT_CANVAS
     if CURRENT_CANVAS is None:
-        CURRENT_CANVAS = QtPlotCanvas()
+        CURRENT_CANVAS = VispyPlotCanvas()
     return CURRENT_CANVAS
 
 
 def _set_current_canvas(canvas):
     global CURRENT_CANVAS
     CURRENT_CANVAS = canvas
     return canvas
@@ -32,19 +31,16 @@
 
 def gcf():
     if CURRENT_MULTI_CANVAS is None:
         return gca()
     return CURRENT_MULTI_CANVAS
 
 
-gcw = gcf
-
-
 def figure():
-    _set_current_canvas(QtPlotCanvas())
+    _set_current_canvas(VispyPlotCanvas())
     return CURRENT_CANVAS
 
 
 @overload
 def subplot(pos: int):
     ...
 
@@ -58,15 +54,15 @@
     if len(args) == 1 and args[0] >= 111:
         if args[0] >= 1000:
             raise ValueError(f"Too large: {args[0]}")
         args = (args[0] // 100, args[0] // 10 % 10, args[0] % 10)
 
     row, col, idx = args
     if CURRENT_MULTI_CANVAS is None:
-        _set_current_multi_canvas(QtMultiPlotCanvas(row, col))
+        _set_current_multi_canvas(VispyMultiPlotCanvas(row, col))
     else:
         if not CURRENT_MULTI_CANVAS.shape == (row, col):
             raise ValueError("Shape of subplots does not match")
     return _set_current_canvas(CURRENT_MULTI_CANVAS[idx - 1])
 
 
 def plot(
@@ -76,15 +72,15 @@
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     lw: float = 1,
     ls: str = "-",
     symbol=None,
-) -> QtPlotCanvas:
+) -> VispyPlotCanvas:
     return gca().add_curve(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
@@ -100,63 +96,55 @@
     y=None,
     face_color=None,
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     symbol=None,
-) -> QtPlotCanvas:
+) -> VispyPlotCanvas:
     return gca().add_scatter(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
         name=name,
         symbol=symbol,
     )
 
 
 def hist(
-    data: Sequence[float],
-    bins: int | Sequence | str = 10,
-    range=None,
-    density: bool = False,
+    data,
+    bins: int = 10,
     face_color=None,
     edge_color=None,
-    color=None,
+    color="white",
     name: str | None = None,
-    lw: float = 1,
-    ls: str = "-",
-) -> QtPlotCanvas:
+) -> VispyPlotCanvas:
     return gca().add_hist(
         data,
         bins=bins,
-        range=range,
-        density=density,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         name=name,
-        lw=lw,
-        ls=ls,
     )
 
 
 def show():
     if CURRENT_MULTI_CANVAS is not None:
         CURRENT_MULTI_CANVAS.show()
     else:
         gca().show()
 
 
 def imshow(image, cmap=None, vmin=None, vmax=None):
     image = np.asarray(image)
-    canvas = QtImageCanvas()
+    canvas = VispyImageCanvas()
     _set_current_canvas(canvas)
     canvas.image = image
 
     if cmap is not None:
         canvas.cmap = cmap
 
     if vmin is not None or vmax is not None:
```

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/widgets.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/test_qtgraph.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/tests/test_qtgraph.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/qtconsole/__init__.py` & `magic_class-0.7.4/magicclass/ext/qtconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/qtconsole/_qt.py` & `magic_class-0.7.4/magicclass/ext/qtconsole/_qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/qtconsole/widgets.py` & `magic_class-0.7.4/magicclass/ext/qtconsole/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/_base.py` & `magic_class-0.7.4/magicclass/ext/vispy/_base.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/camera.py` & `magic_class-0.7.4/magicclass/ext/vispy/camera.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/layer2d.py` & `magic_class-0.7.4/magicclass/ext/vispy/layer2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/layer3d.py` & `magic_class-0.7.4/magicclass/ext/vispy/layer3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/layerlist.py` & `magic_class-0.7.4/magicclass/ext/vispy/layerlist.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/plot_api.py` & `magic_class-0.7.4/magicclass/ext/pyqtgraph/plot_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 from __future__ import annotations
-from typing import overload, TYPE_CHECKING
+
+from typing import overload, TYPE_CHECKING, Sequence
 import numpy as np
-from .widgets2d import VispyPlotCanvas, VispyMultiPlotCanvas, VispyImageCanvas
+from .widgets import QtPlotCanvas, QtMultiPlotCanvas, QtImageCanvas
 
 if TYPE_CHECKING:
-    from .widgets2d import Has2DViewBox, MultiPlot
+    from .widgets import HasViewBox, _MultiPlot
 
-CURRENT_MULTI_CANVAS: MultiPlot | None = None
-CURRENT_CANVAS: Has2DViewBox | None = None
+CURRENT_MULTI_CANVAS: _MultiPlot | None = None
+CURRENT_CANVAS: HasViewBox | None = None
 
 
-def gca() -> VispyPlotCanvas:
+def gca() -> QtPlotCanvas:
     global CURRENT_CANVAS
     if CURRENT_CANVAS is None:
-        CURRENT_CANVAS = VispyPlotCanvas()
+        CURRENT_CANVAS = QtPlotCanvas()
     return CURRENT_CANVAS
 
 
-def _set_current_canvas(canvas):
+def _set_current_canvas(canvas: HasViewBox) -> HasViewBox:
     global CURRENT_CANVAS
     CURRENT_CANVAS = canvas
     return canvas
 
 
 def _set_current_multi_canvas(multi):
     global CURRENT_MULTI_CANVAS
     CURRENT_MULTI_CANVAS = multi
     return multi
 
 
-def gcf():
+def gcf() -> _MultiPlot | QtPlotCanvas:
     if CURRENT_MULTI_CANVAS is None:
         return gca()
     return CURRENT_MULTI_CANVAS
 
 
-def figure():
-    _set_current_canvas(VispyPlotCanvas())
+gcw = gcf
+
+
+def figure() -> QtPlotCanvas:
+    _set_current_canvas(QtPlotCanvas())
     return CURRENT_CANVAS
 
 
 @overload
-def subplot(pos: int):
+def subplot(pos: int) -> HasViewBox:
     ...
 
 
 @overload
-def subplot(row: int, col: int, idx: int):
+def subplot(row: int, col: int, idx: int) -> HasViewBox:
     ...
 
 
 def subplot(*args):
     if len(args) == 1 and args[0] >= 111:
         if args[0] >= 1000:
             raise ValueError(f"Too large: {args[0]}")
         args = (args[0] // 100, args[0] // 10 % 10, args[0] % 10)
 
     row, col, idx = args
     if CURRENT_MULTI_CANVAS is None:
-        _set_current_multi_canvas(VispyMultiPlotCanvas(row, col))
+        _set_current_multi_canvas(QtMultiPlotCanvas(row, col))
     else:
         if not CURRENT_MULTI_CANVAS.shape == (row, col):
             raise ValueError("Shape of subplots does not match")
     return _set_current_canvas(CURRENT_MULTI_CANVAS[idx - 1])
 
 
 def plot(
@@ -72,15 +76,15 @@
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     lw: float = 1,
     ls: str = "-",
     symbol=None,
-) -> VispyPlotCanvas:
+) -> QtPlotCanvas:
     return gca().add_curve(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
@@ -96,55 +100,63 @@
     y=None,
     face_color=None,
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     symbol=None,
-) -> VispyPlotCanvas:
+) -> QtPlotCanvas:
     return gca().add_scatter(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
         name=name,
         symbol=symbol,
     )
 
 
 def hist(
-    data,
-    bins: int = 10,
+    data: Sequence[float],
+    bins: int | Sequence | str = 10,
+    range=None,
+    density: bool = False,
     face_color=None,
     edge_color=None,
-    color="white",
+    color=None,
     name: str | None = None,
-) -> VispyPlotCanvas:
+    lw: float = 1,
+    ls: str = "-",
+) -> QtPlotCanvas:
     return gca().add_hist(
         data,
         bins=bins,
+        range=range,
+        density=density,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         name=name,
+        lw=lw,
+        ls=ls,
     )
 
 
-def show():
+def show() -> None:
     if CURRENT_MULTI_CANVAS is not None:
         CURRENT_MULTI_CANVAS.show()
     else:
         gca().show()
 
 
 def imshow(image, cmap=None, vmin=None, vmax=None):
     image = np.asarray(image)
-    canvas = VispyImageCanvas()
+    canvas = QtImageCanvas()
     _set_current_canvas(canvas)
     canvas.image = image
 
     if cmap is not None:
         canvas.cmap = cmap
 
     if vmin is not None or vmax is not None:
```

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/widgets2d.py` & `magic_class-0.7.4/magicclass/ext/vispy/widgets2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/widgets3d.py` & `magic_class-0.7.4/magicclass/ext/vispy/widgets3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vispy/tests/test_vispy2d.py` & `magic_class-0.7.4/magicclass/ext/vispy/tests/test_vispy2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vtk/components.py` & `magic_class-0.7.4/magicclass/ext/vtk/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vtk/const.py` & `magic_class-0.7.4/magicclass/ext/vtk/const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vtk/volume.py` & `magic_class-0.7.4/magicclass/ext/vtk/volume.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/ext/vtk/widgets.py` & `magic_class-0.7.4/magicclass/ext/vtk/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/fields/_define.py` & `magic_class-0.7.4/magicclass/fields/_define.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/fields/_fields.py` & `magic_class-0.7.4/magicclass/fields/_fields.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/fields/_group.py` & `magic_class-0.7.4/magicclass/fields/_group.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/fields/_property.py` & `magic_class-0.7.4/magicclass/fields/_property.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/functools/_dispatch.py` & `magic_class-0.7.4/magicclass/functools/_dispatch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/functools/_partial.py` & `magic_class-0.7.4/magicclass/functools/_partial.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/functools/_wraps.py` & `magic_class-0.7.4/magicclass/functools/_wraps.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/logging/core.py` & `magic_class-0.7.4/magicclass/logging/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/stylesheets/__init__.py` & `magic_class-0.7.4/magicclass/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/__init__.py` & `magic_class-0.7.4/magicclass/types/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/_bound.py` & `magic_class-0.7.4/magicclass/types/_bound.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/_choices.py` & `magic_class-0.7.4/magicclass/types/_choices.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/_const.py` & `magic_class-0.7.4/magicclass/types/_const.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "below",
     "dock",
     "dialog",
     "parentlast",
 ]
 
 
-ErrorModeStr = Literal["msgbox", "stderr", "stdout"]
+ErrorModeStr = Literal["msgbox", "stderr", "stdout", "napari", "debug"]
 
 Color = Union[Iterable[float], str]
 Colormap = Dict[float, Color]
 
 MGUI_SIMPLE_TYPES = (
     Union[
         int,
```

### Comparing `magic_class-0.7.3/magicclass/types/_expr.py` & `magic_class-0.7.4/magicclass/types/_expr.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/_optional.py` & `magic_class-0.7.4/magicclass/types/_optional.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/types/_path.py` & `magic_class-0.7.4/magicclass/types/_path.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
-from abc import ABCMeta
 
+import sys
+from abc import ABCMeta
 import pathlib
 from typing import TYPE_CHECKING, Any, Sequence
 from typing_extensions import Annotated
 
 
 if TYPE_CHECKING:
     from typing_extensions import Self
@@ -23,15 +24,19 @@
 
     def __subclasscheck__(cls, subclass: type) -> bool:
         return issubclass(subclass, pathlib.Path)
 
 
 class _AnnotatedMultiPathAlias(ABCMeta):
     def __getitem__(cls, filter: str) -> Self:
-        return Annotated[list[Path], {"mode": "rm", "filter": filter}]
+        if sys.version_info >= (3, 9):
+            return Annotated[list[pathlib.Path], {"mode": "rm", "filter": filter}]
+        return Annotated[
+            Any, {"mode": "rm", "filter": filter, "widget_type": "FileEdit"}
+        ]
 
 
 class _Path(pathlib.Path, metaclass=_AnnotatedPathAlias):
     _file_edit_mode = "r"
 
 
 class _SavePath(_Path):
```

### Comparing `magic_class-0.7.3/magicclass/types/_union.py` & `magic_class-0.7.4/magicclass/types/_union.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/__init__.py` & `magic_class-0.7.4/magicclass/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/_click.py` & `magic_class-0.7.4/magicclass/utils/_click.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/_functions.py` & `magic_class-0.7.4/magicclass/utils/_functions.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/_recent.py` & `magic_class-0.7.4/magicclass/utils/_recent.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/qt.py` & `magic_class-0.7.4/magicclass/utils/qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/utils/qthreading.py` & `magic_class-0.7.4/magicclass/utils/qthreading.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     overload,
     TypeVar,
     Generic,
     Protocol,
     runtime_checkable,
 )
 from typing_extensions import TypedDict, ParamSpec
+import warnings
 
 from superqt.utils import create_worker, GeneratorWorker, FunctionWorker
 from qtpy.QtCore import Qt, QThread, QCoreApplication
 from magicgui.widgets import ProgressBar, Container, Widget, PushButton, Label
 from magicgui.application import use_app
 
 from .qt import move_to_screen_center
@@ -194,15 +195,17 @@
         self._pbar.close()
 
 
 class Timer:
     """A timer class with intuitive API."""
 
     def __init__(self):
-        self.reset()
+        self._t0 = default_timer()
+        self._t_total = 0.0
+        self._running = False
 
     def __repr__(self) -> str:
         """Return string in format hh:mm:ss"""
         return self.format_time()
 
     @property
     def sec(self) -> float:
@@ -226,18 +229,15 @@
             now = default_timer()
             self._t_total += now - self._t0
             self._t0 = now
         return self._t_total
 
     def reset(self):
         """Reset timer."""
-        self._t0 = default_timer()
-        self._t_total = 0.0
-        self._running = False
-        return None
+        return self.__init__()
 
     def format_time(self, fmt: str = "{hour:0>2}:{min:0>2}:{sec:0>2}") -> str:
         """Format current time."""
         min_all, sec = divmod(self.sec, 60)
         hour, min = divmod(min_all, 60)
         return fmt.format(hour=int(hour), min=int(min), sec=int(sec))
 
@@ -270,14 +270,17 @@
         cnt.margins = (0, 0, 0, 0)
         self.footer = cnt
         self.pbar.min_width = 240
         self._timer = Timer()
         self._time_signal = QtSignal()
         self._time_signal.connect(self._on_timer_updated)
 
+        self._running = False
+        self._thread_timer: threading.Thread | None = None
+
         super().__init__(widgets=[self.progress_label, self.pbar, cnt], labels=False)
 
     def _on_timer_updated(self, _=None):
         with suppress(RuntimeError):
             if self._timer.sec < 3600:
                 self.time_label.value = self._timer.format_time("{min:0>2}:{sec:0>2}")
             else:
@@ -543,20 +546,29 @@
                     "'napari', or a proper type object."
                 )
         cls._DEFAULT_PROGRESS_BAR = pbar_cls
         return pbar_cls
 
     @staticmethod
     def to_callback(callback: Callable, *args, **kwargs) -> Callback:
-        """Convert a callback to a callback object."""
-        cb = Callback(callback)
+        warnings.warn(
+            "Defining callback with to_callback is deprecated because its "
+            "behavior is confusing. Use thread_worker.callback instead.",
+            DeprecationWarning,
+        )
+        cb = _CallbackDeprecated(callback)
         if args or kwargs:
             cb = cb(*args, **kwargs)
         return cb
 
+    @staticmethod
+    def callback(callback: Callable) -> Callback:
+        """Convert a callback function to a callback object."""
+        return Callback(callback)
+
     @property
     def is_generator(self) -> bool:
         """True if bound function is a generator function."""
         return inspect.isgeneratorfunction(self._func)
 
     @property
     def __is_recordable__(self) -> bool:
@@ -701,27 +713,27 @@
             if _is_non_blocking:
 
                 @worker.errored.connect
                 def _on_error(err: Exception):
                     # NOTE: Exceptions are raised in other thread so context manager
                     # cannot catch them. Macro has to be reactived here.
                     gui._error_mode.get_handler()(err, parent=gui)
-                    gui.macro.active = True
                     if not self._ignore_errors:
                         raise err  # reraise
 
                 worker.start()
             else:
                 # If function is called from script, some events must get processed by
                 # the application while keep script stopping at each line of code.
                 self._run_blocked(gui, worker, pbar)
 
             return None
 
         _create_worker.__self__ = gui
+        _create_worker.__thread_worker__ = self
         return _create_worker
 
     def _run_blocked(
         self,
         gui: BaseGui,
         worker: FunctionWorker | GeneratorWorker,
         pbar: ProgressBar | None,
@@ -974,31 +986,41 @@
     """True if the current thread is the main thread."""
     return QThread.currentThread() is QCoreApplication.instance().thread()
 
 
 class Callback:
     """Callback object that can be recognized by thread_worker."""
 
-    def __init__(self, f: Callable[[], Any]):
+    def __init__(self, f: Callable[..., Any]):
         if not callable(f):
             raise TypeError(f"{f} is not callable.")
         self._func = f
+        wraps(f)(self)
 
     @staticmethod
     def catch(out, gui: BaseGui, tw: thread_worker, args, kwargs, record=True):
         if isinstance(out, Callback):
             with gui.macro.blocked():
                 out = out._func()
         if record and gui.macro.active and tw._recorder is not None:
             tw._recorder(gui, out, *args, **kwargs)
 
     def __call__(self, *args, **kwargs) -> Callback:
+        return self._func(*args, **kwargs)
+
+    def with_args(self, *args, **kwargs):
         """Return a partial callback."""
         return self.__class__(partial(self._func, *args, **kwargs))
 
     def __get__(self, obj, type=None) -> Callback:
         if obj is None:
             return self
-        return self(obj)
+        return self.with_args(obj)
+
+
+class _CallbackDeprecated(Callback):
+    def __call__(self, *args, **kwargs) -> Callback:
+        """Return a partial callback."""
+        return self.__class__(partial(self._func, *args, **kwargs))
 
 
 to_callback = thread_worker.to_callback  # function version
```

### Comparing `magic_class-0.7.3/magicclass/widgets/__init__.py` & `magic_class-0.7.4/magicclass/widgets/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from .plot import Figure, SeabornFigure
 from .separator import Separator
 from .utils import FreeWidget
 from .logger import Logger
 from .codeedit import CodeEdit
 from .toggle_switch import ToggleSwitch
 from .eval import EvalLineEdit
+from .line_runner import OneLineRunner
 from ._union import UnionWidget
 
 __all__ = [
     "ButtonContainer",
     "CodeEdit",
     "ColorEdit",
     "ColormapEdit",
@@ -55,14 +56,15 @@
     "GroupBoxContainer",
     "HCollapsibleContainer",
     "HistoryFileEdit",
     "HistoryLineEdit",
     "ListContainer",
     "ListWidget",
     "Logger",
+    "OneLineRunner",
     "OptionalWidget",
     "SeabornFigure",
     "Separator",
     "ScrollableContainer",
     "SubWindowsContainer",
     "SplitterContainer",
     "SpreadSheet",
```

### Comparing `magic_class-0.7.3/magicclass/widgets/_html.py` & `magic_class-0.7.4/magicclass/widgets/_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 class HtmlExporter:
     """A stateful HTML exporter for a Q(Plain)TextEdit.
 
     This class is designed for convenient user interaction.
     """
 
-    def __init__(self, control):
+    def __init__(self, control: QtW.QPlainTextEdit | QtW.QTextEdit):
         """Creates an HtmlExporter for the given Q(Plain)TextEdit."""
         assert isinstance(control, (QtW.QPlainTextEdit, QtW.QTextEdit))
         self.control = control
         self.filename = None
 
     def export(self):
         """Displays a dialog for exporting HTML generated by Qt's rich text
```

### Comparing `magic_class-0.7.3/magicclass/widgets/_mpl_canvas.py` & `magic_class-0.7.4/magicclass/widgets/_mpl_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         in which cursor exists will be resized.
         """
         ax = self.last_axis
         if not self._interactive or not ax:
             return
         delta = event.angleDelta().y() / 120
         event = self.get_mouse_event(event)
-        factor = 0.75 ** delta
+        factor = 0.75**delta
 
         _zoom_x_wheel(ax, factor)
         _zoom_y_wheel(ax, factor)
         self.figure.canvas.draw()
         return None
 
     def mousePressEvent(self, event):
@@ -125,40 +125,62 @@
 
     def _make_context_menu(self):
         """Make a QMenu object with default actions."""
         menu = QtW.QMenu(self)
         menu.addAction("Copy ...", self._copy_canvas)
         menu.addAction("Save As...", self._save_canvas_dialog)
         menu.addSeparator()
+        menu.addAction("Reset Zoom", self._reset_zoom)
+        menu.addAction("Toggle legend", self._toggle_legend)
         return menu
 
     def _save_canvas_dialog(self, format="PNG"):
         """Open a file dialog and save the current canvas state."""
         dialog = QtW.QFileDialog(self, "Save Image")
-        dialog.setAcceptMode(QtW.QFileDialog.AcceptSave)
+        dialog.setAcceptMode(QtW.QFileDialog.AcceptMode.AcceptSave)
         dialog.setDefaultSuffix(format.lower())
         dialog.setNameFilter(f"{format} file (*.{format.lower()})")
         if dialog.exec_():
             filename = dialog.selectedFiles()[0]
             self._save_canvas(filename)
 
+    def _reset_zoom(self):
+        """Reset zoom to initial state."""
+        ax = self.last_axis
+        if not ax:
+            return
+        ax.autoscale(axis="both")
+        self.figure.canvas.draw()
+
+    def _toggle_legend(self):
+        """Toggle legend."""
+        ax = self.last_axis
+        if not ax:
+            return
+        if getattr(ax, "legend_", None) is None:
+            ax.legend()
+        else:
+            visible = not ax.legend_.get_visible()
+            ax.legend_.set_visible(visible)
+        self.figure.canvas.draw()
+
     def _save_canvas(self, path: str):
         """Save current canvas state at the specified path."""
         self.figure.savefig(path)
 
     def _asarray(self) -> np.ndarray:
         """Convert current canvas state into RGBA numpy array."""
         return np.asarray(self.renderer.buffer_rgba(), dtype=np.uint8)
 
     def _copy_canvas(self):
         """Copy current canvas state into clipboard."""
         arr = self._asarray()
         clipboard = QtW.QApplication.clipboard()
         h, w, _ = arr.shape
-        image = QtGui.QImage(arr, w, h, QtGui.QImage.Format_RGBA8888)
+        image = QtGui.QImage(arr, w, h, QtGui.QImage.Format.Format_RGBA8888)
         clipboard.setImage(image)
 
 
 def _translate_x(ax: Axes, xstart: float, xstop: float):
     xscale = ax.get_xscale()
     x0, x1 = ax.get_xlim()
     if xscale == "linear":
```

### Comparing `magic_class-0.7.3/magicclass/widgets/_union.py` & `magic_class-0.7.4/magicclass/widgets/_union.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/codeedit.py` & `magic_class-0.7.4/magicclass/widgets/codeedit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 from contextlib import contextmanager
-import sys
+import inspect
 from typing import Any, Iterator, NamedTuple, TYPE_CHECKING
 import weakref
 from qtpy import QtWidgets as QtW, QtGui, QtCore
 from qtpy.QtCore import Qt, Signal as pyqtSignal
 
 from psygnal import Signal
 from magicgui.backends._qtpy.widgets import TextEdit as QBaseTextEdit, QBaseStringWidget
 from magicgui.widgets import TextEdit, EmptyWidget, FileEdit
 from magicgui.application import use_app
 from magicgui.widgets.bases import ValueWidget
 from magicgui.types import Undefined
 
 from macrokit import parse, Symbol, Expr, Head
 from magicclass._gui.utils import show_dialog_from_mgui
-from magicclass.utils import show_messagebox
+from magicclass.signature import split_annotated_type, is_annotated
+from magicclass.widgets._const import FONT
 
 if TYPE_CHECKING:
     from magicclass import MagicTemplate
 
+_TAB = " " * 4
+_PAIRS = {"(": ")", "[": "]", "{": "}"}
+
 
 class QLineNumberArea(QtW.QWidget):
     def __init__(self, editor: QCodeEditor):
         super().__init__(editor)
         self.editor = editor
         self.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self.customContextMenuRequested.connect(self.editor._show_context_menu)
@@ -58,26 +62,28 @@
             cursor.movePosition(
                 QtGui.QTextCursor.MoveOperation.EndOfLine,
                 QtGui.QTextCursor.MoveMode.KeepAnchor,
             )
             self.editor.setTextCursor(cursor)
 
 
+class Mod:
+    No = Qt.KeyboardModifier.NoModifier
+    Ctrl = Qt.KeyboardModifier.ControlModifier
+    Shift = Qt.KeyboardModifier.ShiftModifier
+    Alt = Qt.KeyboardModifier.AltModifier
+
+
 class QCodeEditor(QtW.QPlainTextEdit):
     executionRequested = pyqtSignal(object)
 
     def __init__(self, parent: QtW.QWidget | None = None):
         super().__init__(parent)
-        if sys.platform == "win32":
-            _font = "Consolas"
-        elif sys.platform == "darwin":
-            _font = "Menlo"
-        else:
-            _font = "Monospace"
-        font = QtGui.QFont(_font, self.font().pointSize())
+        self.setStyleSheet("QToolTip { font-family: FONT; }".replace("FONT", FONT))
+        font = QtGui.QFont(FONT, self.font().pointSize())
         font.setStyleHint(QtGui.QFont.StyleHint.Monospace)
         font.setFixedPitch(True)
         self.setFont(font)
 
         self._line_number_area = QLineNumberArea(self)
 
         self.blockCountChanged.connect(self._update_line_number_area_width)
@@ -86,24 +92,25 @@
         self._update_line_number_area_width()
 
         self.setTabSize(4)
         self.setWordWrapMode(QtGui.QTextOption.WrapMode.NoWrap)
         self.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self.customContextMenuRequested.connect(self._show_context_menu)
         self._magicclass_parent_ref: weakref.ReferenceType[MagicTemplate] = None
+        self._highlight = None
 
-    def tabSize(self):
+    def tabSize(self) -> int:
         metrics = self.fontMetrics()
         return self.tabStopWidth() // metrics.width(" ")
 
-    def setTabSize(self, size: int):
+    def setTabSize(self, size: int) -> None:
         metrics = self.fontMetrics()
         self.setTabStopWidth(size * metrics.width(" "))
 
-    def lineNumberAreaWidth(self):
+    def lineNumberAreaWidth(self) -> int:
         count = max(1, self.blockCount())
         digits = len(str(count))
         space = 8 + self.fontMetrics().width("9") * digits
         return space
 
     def _update_line_number_area_width(self):
         self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
@@ -126,62 +133,38 @@
         self._line_number_area.setGeometry(
             QtCore.QRect(cr.left(), cr.top(), self.lineNumberAreaWidth(), cr.height())
         )
 
     def event(self, ev: QtCore.QEvent):
         try:
             if ev.type() == QtCore.QEvent.Type.ToolTip:
-                ev = QtGui.QHelpEvent(ev)
-                line = self._analyze_line(self.viewport().mapFromGlobal(ev.globalPos()))
-                QtW.QToolTip.showText(ev.globalPos(), str(line), self)
+                return self._show_tooltip(ev)
             elif ev.type() == QtCore.QEvent.Type.KeyPress:
                 ev = QtGui.QKeyEvent(ev)
-                if (
-                    ev.key() == Qt.Key.Key_Tab
-                    and ev.modifiers() & Qt.KeyboardModifier.NoModifier
-                ):
-                    if self.textCursor().hasSelection():
-                        for cursor in self.iter_selected_lines():
-                            self.add_at_the_start("\t", cursor)
-                    else:
-                        self.textCursor().insertText("\t")
-                    return True
-                if (
-                    ev.key() == Qt.Key.Key_Tab
-                    and ev.modifiers() & Qt.KeyboardModifier.ShiftModifier
-                ) or ev.key() == Qt.Key.Key_Backtab:
-                    # unindent
-                    for cursor in self.iter_selected_lines():
-                        self.remove_at_the_start("\t", cursor)
-                    return True
+                _key = ev.key()
+                _mod = ev.modifiers()
+                if _key == Qt.Key.Key_Tab and _mod == Mod.No:
+                    return self._tab_event()
+                elif _key == Qt.Key.Key_Tab and _mod & Mod.Shift:
+                    return self._back_tab_event()
+                elif _key == Qt.Key.Key_Backtab:
+                    return self._back_tab_event()
                 # comment out selected lines
-                elif (
-                    ev.key() == Qt.Key.Key_Slash
-                    and ev.modifiers() & Qt.KeyboardModifier.ControlModifier
-                ):
-                    for cursor in self.iter_selected_lines():
-                        line = cursor.block().text()
-                        if line.startswith("#"):
-                            if line.startswith("# "):
-                                self.remove_at_the_start("# ", cursor)
-                            else:
-                                self.remove_at_the_start("#", cursor)
-                        else:
-                            self.add_at_the_start("# ", cursor)
-                    return True
+                elif _key == Qt.Key.Key_Slash and _mod & Mod.Ctrl:
+                    return self._ctrl_slash_event()
                 # move selected lines up or down
                 elif (
-                    ev.key() in (Qt.Key.Key_Up, Qt.Key.Key_Down)
-                    and ev.modifiers() & Qt.KeyboardModifier.AltModifier
+                    _key in (Qt.Key.Key_Up, Qt.Key.Key_Down)
+                    and _mod & Qt.KeyboardModifier.AltModifier
                 ):
                     cursor = self.textCursor()
                     cursor0 = self.textCursor()
                     start = cursor.selectionStart()
                     end = cursor.selectionEnd()
-                    if ev.key() == Qt.Key.Key_Up and min(start, end) > 0:
+                    if _key == Qt.Key.Key_Up and min(start, end) > 0:
                         cursor0.setPosition(start)
                         cursor0.movePosition(
                             QtGui.QTextCursor.MoveOperation.PreviousBlock
                         )
                         cursor0.movePosition(
                             QtGui.QTextCursor.MoveOperation.StartOfLine
                         )
@@ -204,15 +187,15 @@
                             txt = txt.rstrip("\u2029")
                         cursor0.movePosition(
                             QtGui.QTextCursor.MoveOperation.NextCharacter
                         )
                         cursor0.insertText(txt)
                         self.setTextCursor(cursor)
                     elif (
-                        ev.key() == Qt.Key.Key_Down
+                        _key == Qt.Key.Key_Down
                         and max(start, end) < self.document().characterCount() - 1
                     ):
                         cursor0.setPosition(end)
                         cursor0.movePosition(QtGui.QTextCursor.MoveOperation.EndOfLine)
                         cursor0.movePosition(
                             QtGui.QTextCursor.MoveOperation.NextCharacter,
                             QtGui.QTextCursor.MoveMode.KeepAnchor,
@@ -234,14 +217,59 @@
                             txt = txt.lstrip("\u2029")
                         cursor0.movePosition(
                             QtGui.QTextCursor.MoveOperation.PreviousCharacter
                         )
                         cursor0.insertText(txt)
                         self.setTextCursor(cursor)
                     return True
+                elif _key in (Qt.Key.Key_Enter, Qt.Key.Key_Return):
+                    # get current line, check if it has tabs at the beginning
+                    # if yes, insert the same number of tabs at the next line
+                    self._new_line_event()
+                    return True
+                elif _key == Qt.Key.Key_Backspace and _mod == Mod.No:
+                    # delete 4 spaces
+                    _cursor = self.textCursor()
+                    _cursor.movePosition(
+                        QtGui.QTextCursor.MoveOperation.StartOfLine,
+                        QtGui.QTextCursor.MoveMode.KeepAnchor,
+                    )
+                    line = _cursor.selectedText()
+                    if line.endswith("    "):
+                        for _ in range(4):
+                            self.textCursor().deletePreviousChar()
+                        return True
+                elif _key == Qt.Key.Key_D and _mod & Mod.Ctrl:
+                    return self._select_word_event()
+                elif _key == Qt.Key.Key_L and _mod & Mod.Ctrl:
+                    return self._select_line_event()
+                elif _key == Qt.Key.Key_Home and _mod == Mod.No:
+                    return self._home_event()
+                elif _key in (
+                    Qt.Key.Key_ParenLeft,
+                    Qt.Key.Key_BracketLeft,
+                    Qt.Key.Key_BraceLeft,
+                ):
+                    _char = QtGui.QKeySequence(_key).toString()
+                    return self._put_selection_in(_char, _PAIRS[_char])
+                elif _key in (
+                    Qt.Key.Key_ParenRight,
+                    Qt.Key.Key_BracketRight,
+                    Qt.Key.Key_BraceRight,
+                ):
+                    _char = QtGui.QKeySequence(_key).toString()
+                    return self._key_no_duplicate(_char)
+                elif _key in (
+                    Qt.Key.Key_QuoteDbl,
+                    Qt.Key.Key_Apostrophe,
+                    Qt.Key.Key_QuoteLeft,
+                ):
+                    _char = QtGui.QKeySequence(_key).toString()
+                    return self._quote_selection(_char)
+
         except Exception:
             pass
         return super().event(ev)
 
     def _magicclass_parent(self):
         if self._magicclass_parent_ref is None:
             return None
@@ -250,22 +278,17 @@
     def _search_parent_magicclass(self) -> MagicTemplate | None:
         if self._magicclass_parent_ref is None:
             return None
         if obj := self._magicclass_parent_ref():
             return obj._search_parent_magicclass()
         return None
 
-    def _analyze_line(self, pos: QtCore.QPoint):
-        """Analyze the line under position."""
-        info = self.wordAt(pos)
-        if info is None:
-            return ""
-        return f"{info.expr} (type: {type(info.obj).__name__})"
-
     def wordAt(self, pos: QtCore.QPoint) -> WordInfo | None:
+        if not self.isVisible():
+            return None
         cursor = self.cursorForPosition(pos)
         cursor.select(QtGui.QTextCursor.SelectionType.WordUnderCursor)
         block = cursor.block()
         line = block.text().strip()
         clicked_pos = cursor.position() - block.position()
         try:
             return eval_under_cursor(
@@ -276,31 +299,35 @@
             # raise e
             return None
 
     def _open_magicgui(self, pos: QtCore.QPoint):
         from magicclass._gui.mgui_ext import is_clickable
 
         info = self.wordAt(pos)
-        if info and is_clickable(info.obj):
-            mgui = info.obj.mgui
+        if info and is_clickable(info.widget):
+            mgui = info.widget.mgui
+            mcls = self._search_parent_magicclass()
             if mgui is None:
-                return show_messagebox("error", "Error", "No magicgui found", self)
+                # macro is not added from GUI. Create one.
+                from magicclass._gui._base import _build_mgui, _create_gui_method
+
+                func = _create_gui_method(mcls, info.obj)
+                mgui = _build_mgui(info.widget, func, mcls)
+                info.widget.mgui = mgui
+
             nwidgets = sum(not isinstance(wdt, EmptyWidget) for wdt in mgui)
             if nwidgets > 1:
                 if isinstance(mgui[0], FileEdit):
                     show_dialog_from_mgui(mgui)
                 else:
-                    mgui.show()
+                    info.widget.changed()
             else:
-                show_messagebox(
-                    "error",
-                    "Error",
-                    f"No parameter can be chosen in {info.obj.name!r}.",
-                    self,
-                )
+                with mcls._error_mode.raise_with_handler(mcls):
+                    raise TypeError(f"No parameter can be chosen in {info.widget!r}.")
+
         return
 
     def _show_context_menu(self, pos: QtCore.QPoint):
         menu = QtW.QMenu(self.viewport())
         cursor = self.textCursor()
         new_pos = self.cursorForPosition(pos).position()
         if not cursor.selectionStart() <= new_pos <= cursor.selectionEnd():
@@ -500,49 +527,327 @@
         """Return the text."""
         return self.toPlainText().replace("\u2029", "\n")
 
     def setText(self, text: str):
         """Set the text."""
         self.setPlainText(text.replace("\n", "\u2029"))
 
+    def _text_of_current_line(self):
+        _cursor = self.textCursor()
+        _cursor.movePosition(QtGui.QTextCursor.MoveOperation.StartOfLine)
+        _cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.EndOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        return _cursor.selectedText()
+
+    def _text_of_line_before_cursor(self):
+        _cursor = self.textCursor()
+        _cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.StartOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        return _cursor.selectedText()
+
+    def _show_tooltip(self, ev: QtGui.QHelpEvent):
+        pos = self.viewport().mapFromGlobal(ev.globalPos())
+        info = self.wordAt(pos)
+        if info is None:
+            return False
+        try:
+            tooltip = info.get_method_tooltip()
+        except Exception:
+            tooltip = info.get_simple_tooltip()
+        QtW.QToolTip.showText(ev.globalPos(), tooltip, self)
+        return True
+
+    def _tab_event(self):
+        if self.textCursor().hasSelection():
+            for cursor in self.iter_selected_lines():
+                self.add_at_the_start(_TAB, cursor)
+        else:
+            self.textCursor().insertText(_TAB)
+        return True
+
+    def _back_tab_event(self):
+        # unindent
+        for cursor in self.iter_selected_lines():
+            self.remove_at_the_start(_TAB, cursor)
+        return True
+
+    def _ctrl_slash_event(self):
+        for cursor in self.iter_selected_lines():
+            line = cursor.block().text()
+            if line.startswith("#"):
+                if line.startswith("# "):
+                    self.remove_at_the_start("# ", cursor)
+                else:
+                    self.remove_at_the_start("#", cursor)
+            else:
+                self.add_at_the_start("# ", cursor)
+        return True
+
+    def _select_word_event(self):
+        cursor = self.textCursor()
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.NextWord)
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.PreviousWord,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        self.setTextCursor(cursor)
+        return True
+
+    def _select_line_event(self):
+        cursor = self.textCursor()
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.StartOfLine)
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.EndOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.NextCharacter,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        self.setTextCursor(cursor)
+        return True
+
+    def _new_line_event(self):
+        line = self._text_of_line_before_cursor()
+        cursor = self.textCursor()
+        line_rstripped = line.rstrip()
+        indent = _get_indents(line)
+        if line_rstripped == "":
+            cursor.insertText("\n" + indent)
+            self.setTextCursor(cursor)
+            return
+
+        ndel = len(line) - len(line_rstripped)
+        last_char = line_rstripped[-1]
+        if last_char in "([{:":
+            for _ in range(ndel):
+                cursor.deletePreviousChar()
+            cursor.insertText("\n" + indent + _TAB)
+            self.setTextCursor(cursor)
+            cursor = self.textCursor()
+            if _close := {"(": ")", "{": "}", "[": "]"}.get(last_char):
+                cursor.movePosition(
+                    QtGui.QTextCursor.MoveOperation.EndOfLine,
+                    QtGui.QTextCursor.MoveMode.KeepAnchor,
+                )
+                if (idx := cursor.selectedText().find(_close)) >= 0:
+                    cursor.clearSelection()
+                    for _ in range(idx):
+                        cursor.movePosition(
+                            QtGui.QTextCursor.MoveOperation.NextCharacter,
+                        )
+                    cursor.movePosition(QtGui.QTextCursor.MoveOperation.Left)
+                    cursor.insertText("\n" + indent)
+                    cursor.movePosition(QtGui.QTextCursor.MoveOperation.Up)
+                    cursor.movePosition(QtGui.QTextCursor.MoveOperation.StartOfLine)
+                    cursor.movePosition(QtGui.QTextCursor.MoveOperation.NextWord)
+                cursor.clearSelection()
+            self.setTextCursor(cursor)
+        else:
+            cursor.insertText("\n" + indent)
+            self.setTextCursor(cursor)
+
+        line_lstripped = line.lstrip()
+        if (
+            line_lstripped.startswith("return ")
+            or line_lstripped.startswith("raise ")
+            or line_lstripped in ("return", "raise", "break", "continue", "pass")
+        ):
+            if line.startswith(_TAB):
+                for _ in range(4):
+                    cursor.deletePreviousChar()
+        self.setTextCursor(cursor)
+
+    def _home_event(self):
+        # fn + left
+        cursor = self.textCursor()
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.StartOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        text = cursor.selectedText()
+        if all(c == " " for c in text):
+            cursor.clearSelection()
+        else:
+            text_lstrip = text.lstrip()
+            nmove = len(text) - len(text_lstrip)
+            cursor.clearSelection()
+            for _ in range(nmove):
+                cursor.movePosition(QtGui.QTextCursor.MoveOperation.Right)
+
+        self.setTextCursor(cursor)
+        return True
+
+    def _put_selection_in(self, left: str, right: str) -> bool:
+        cursor = self.textCursor()
+        start = cursor.selectionStart()
+        end = cursor.selectionEnd()
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.EndOfLine)
+        pos_line_end = cursor.position()
+        cursor.setPosition(end)
+        if start != end or pos_line_end == end:
+            cursor.insertText(right)
+        cursor.setPosition(start)
+        cursor.insertText(left)
+        cursor.setPosition(start + 1)
+        cursor.setPosition(end + 1, QtGui.QTextCursor.MoveMode.KeepAnchor)
+        self.setTextCursor(cursor)
+        return True
+
+    def _quote_selection(self, quot: str) -> bool:
+        cursor = self.textCursor()
+        start = cursor.selectionStart()
+        end = cursor.selectionEnd()
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.EndOfLine)
+        pos_line_end = cursor.position()
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.StartOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        line = cursor.selectedText()
+        nquot = line.count(quot)
+        cursor.clearSelection()
+        cursor.setPosition(end)
+        if nquot % 2 == 0:
+            if start != end or pos_line_end == end:
+                cursor.insertText(quot)
+        cursor.setPosition(start)
+        cursor.insertText(quot)
+        cursor.setPosition(start + 1)
+        cursor.setPosition(end + 1, QtGui.QTextCursor.MoveMode.KeepAnchor)
+        self.setTextCursor(cursor)
+        return True
+
+    def _key_no_duplicate(self, char: str) -> bool:
+        cursor = self.textCursor()
+        pos = cursor.position()
+        cursor.movePosition(
+            QtGui.QTextCursor.MoveOperation.EndOfLine,
+            QtGui.QTextCursor.MoveMode.KeepAnchor,
+        )
+        line = cursor.selectedText()
+        if line.startswith(char):
+            cursor.setPosition(pos + 1)
+        else:
+            cursor.setPosition(pos)
+            cursor.insertText(char)
+        self.setTextCursor(cursor)
+        return True
+
+
+def _get_indents(text: str) -> int:
+    chars = []
+    for c in text:
+        if c == " ":
+            chars.append(" ")
+        elif c == "\t":
+            chars.append(_TAB)
+        else:
+            break
+    return "".join(chars)
+
 
 class WordInfo(NamedTuple):
-    obj: Any
-    expr: Expr
-    word: str
+    """Info of a word in the code."""
+
+    widget: Any  # hovered widget (if available)
+    expr: Expr  # hovered expression
+    word: str  # hovered word
+    obj: Any = None
+
+    def get_simple_tooltip(self) -> str:
+        return f"{self.expr} (widget: {annot_to_str(type(self.widget))})"
+
+    def get_method_tooltip(self) -> str:
+        sig = inspect.signature(self.obj)
+        doc = getattr(self.obj, "__doc__", None)
+        if doc is None:
+            doc = "<No Docstring>"
+        param_strs: list[str] = []
+        for name, param in sig.parameters.items():
+            if param.annotation is param.empty:
+                repr_ = name
+            else:
+                repr_ = f"{name}: {annot_to_str(param.annotation)}"
+            if param.default is not param.empty:
+                repr_ += f" = {safe_repr(param.default)}"
+            param_strs.append(repr_)
+        if sig.return_annotation is not sig.empty:
+            ret_annot = f" -> {annot_to_str(sig.return_annotation)}"
+        else:
+            ret_annot = ""
+        if len(param_strs) == 0:
+            all_args_str = ""
+        else:
+            all_args_str = "\n  " + ",\n  ".join(param_strs) + "\n"
+        return (
+            f"{self.expr} (widget: {annot_to_str(type(self.widget))})\n"
+            f"def {self.expr.args[-1]}({all_args_str}){ret_annot}\n"
+            f"{doc}"
+        )
+
+
+def annot_to_str(annot: Any) -> str:
+    if isinstance(annot, type):
+        return annot.__name__
+    if is_annotated(annot):
+        return annot_to_str(split_annotated_type(annot)[0])
+    s = str(annot)
+    if s.startswith("typing."):
+        return s[7:]
+    return s
+
+
+def safe_repr(obj: Any) -> str:
+    try:
+        out = repr(obj)
+    except Exception:
+        return "???"
+    if len(out) > 36:
+        return out[:36] + " ..."
+    return out
 
 
 def eval_under_cursor(
-    line: str, clicked_pos: int, parent: MagicTemplate
+    line: str, clicked_pos: int, parent: MagicTemplate | None = None
 ) -> WordInfo | None:
+    if parent is None:
+        return None
     expr = parse(line)
     pos_start = 0
     pos_stop = len(line)
     if not isinstance(expr, Expr):
         # got a Symbol
-        obj = expr.eval({expr: parent})
+        obj = widget = expr.eval({expr: parent})
         words = expr
 
     elif expr.head is Head.call:
-        first = expr.args[0]
+        first = expr.args[0]  # e.g. ui, ui.method. ui.subclass.method
         while isinstance(first, Expr) and first.head is Head.getattr:
             next_first, _ = first.args
             _length = len(str(next_first))
             if _length < clicked_pos - 1:
                 pos_start = _length
                 break
             first = next_first
+        if len(str(first)) < clicked_pos:
+            return None
 
         if isinstance(first, Expr):
             left, right = first.args
             words = first
             expr = Expr(Head.getitem, [left, str(right)])
-            obj = expr.eval({Symbol.var("ui"): parent})
+            widget = expr.eval({Symbol.var("ui"): parent})
+            obj = first.eval({Symbol.var("ui"): parent})
         else:
-            obj = first.eval({first: parent})
+            obj = widget = first.eval({first: parent})
             words = first
 
     elif expr.head is Head.assign:
         first = expr.args[0]
         if not isinstance(first, Expr) or not str(first.args[0]).startswith("ui"):
             return None
         while isinstance(first, Expr) and first.head is Head.getattr:
@@ -553,24 +858,26 @@
                 break
             first = next_first
 
         if isinstance(first, Expr):
             left, right = first.args
             left_obj = left.eval({Symbol.var("ui"): parent})
             if hasattr(left_obj, "__getitem__"):
-                obj = left_obj[str(right)]
+                widget = left_obj[str(right)]
+                obj = first.eval({Symbol.var("ui"): parent})
             else:
-                obj = getattr(left_obj, str(right))
+                obj = widget = getattr(left_obj, str(right))
             words = first
         else:
-            obj = first.eval({first: parent})
+            obj = widget = first.eval({first: parent})
             words = first
     else:
         return None
-    return WordInfo(obj, words, str(words).split(".")[-1])
+    info = WordInfo(widget, words, str(words).split(".")[-1], obj)
+    return info
 
 
 # ##############################################################################
 # ##############################################################################
 
 
 class QBaseCodeEdit(QBaseTextEdit):
@@ -602,50 +909,50 @@
         )
         self._qcode_edit().executionRequested.connect(self.executing.emit)
 
     def _qcode_edit(self) -> QCodeEditor:
         return self._widget._qwidget
 
     @property
-    def tab_size(self):
+    def tab_size(self) -> int:
         return self._qcode_edit().tabSize()
 
     @tab_size.setter
-    def tab_size(self, size: int):
+    def tab_size(self, size: int) -> None:
         return self._qcode_edit().setTabSize(size)
 
-    def erase_last(self):
+    def erase_last(self) -> None:
         """Erase the last line."""
         self._qcode_edit().eraseLast()
 
-    def erase_first(self):
+    def erase_first(self) -> None:
         """Erase the first line."""
         self._qcode_edit().eraseFirst()
 
-    def append(self, text: str):
+    def append(self, text: str) -> None:
         """Append text to the end of the document."""
         self._qcode_edit().appendPlainText(text)
 
     @property
     def selected(self) -> str:
         """Return selected string."""
         return self._qcode_edit().selectedText()
 
     def syntax_highlight(self, lang: str = "python", theme: str = "default"):
         """Highlight syntax."""
         self._qcode_edit().syntaxHighlight(lang, theme)
 
     @property
-    def __magicclass_parent__(self):
+    def __magicclass_parent__(self) -> MagicTemplate | None:
         return self._qcode_edit()._magicclass_parent()
 
     @__magicclass_parent__.setter
-    def __magicclass_parent__(self, val):
+    def __magicclass_parent__(self, val) -> None:
         self._qcode_edit()._magicclass_parent_ref = weakref.ref(val)
 
-    def zoom_in(self):
+    def zoom_in(self) -> None:
         """Zoom in."""
         self._qcode_edit().zoomIn()
 
-    def zoom_out(self):
+    def zoom_out(self) -> None:
         """Zoom out."""
         self._qcode_edit().zoomOut()
```

### Comparing `magic_class-0.7.3/magicclass/widgets/color.py` & `magic_class-0.7.4/magicclass/widgets/color.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/colormap.py` & `magic_class-0.7.4/magicclass/widgets/colormap.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/containers.py` & `magic_class-0.7.4/magicclass/widgets/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, TypeVar, Callable
+from typing import Any, Callable, TypeVar
 import warnings
 from qtpy import QtWidgets as QtW, QtCore
 from qtpy.QtCore import Qt, QEvent, QSize
 
 from magicgui.application import use_app
 from magicgui.widgets import Widget
 from magicgui.widgets._concrete import _LabeledWidget
```

### Comparing `magic_class-0.7.3/magicclass/widgets/eval.py` & `magic_class-0.7.4/magicclass/widgets/eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-import sys
 from types import MappingProxyType
 from typing import Any, Mapping
 from collections import Counter
 
 from macrokit import parse, Head, Expr
 from qtpy import QtWidgets as QtW, QtCore, QtGui
 from qtpy.QtCore import Qt
 
 from magicgui.backends._qtpy.widgets import QBaseStringWidget
 from magicgui.widgets.bases import ValueWidget
+from magicclass.widgets._const import FONT
 
 
 def _get_last_group(text: str) -> str | None:
     if text.endswith(" "):
         # look for the global namespace
         return ""
 
@@ -97,21 +97,15 @@
 
 
 class QEvalLineEdit(QtW.QLineEdit):
     def __init__(self, parent=None):
         super().__init__(parent)
         self.textChanged.connect(self._on_text_changed)
         self._namespace: Mapping[str, Any] = {}
-        if sys.platform == "win32":
-            _font = "Consolas"
-        elif sys.platform == "darwin":
-            _font = "Menlo"
-        else:
-            _font = "Monospace"
-        self.setFont(QtGui.QFont(_font))
+        self.setFont(QtGui.QFont(FONT))
         self._current_completion_state: tuple[str, list[str]] = None
         self._list_widget = None
         self._auto_suggest = True
 
     def namespace(self) -> dict[str, Any]:
         return self._namespace
```

### Comparing `magic_class-0.7.3/magicclass/widgets/logger.py` & `magic_class-0.7.4/magicclass/widgets/logger.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/misc.py` & `magic_class-0.7.4/magicclass/widgets/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
+
 from pathlib import Path
-import sys
+import os
 from typing import (
     Iterable,
     MutableSequence,
     Any,
     TypeVar,
 )
 from typing_extensions import _AnnotatedAlias, get_args
@@ -25,24 +26,18 @@
 from magicgui.widgets.bases import ValueWidget, RangedWidget
 from magicgui.backends._qtpy.widgets import (
     QBaseStringWidget,
     LineEdit as BaseLineEdit,
 )
 from .utils import FreeWidget, merge_super_sigs
 from magicclass.signature import split_annotated_type
+from magicclass.widgets._const import FONT
 
 _W = TypeVar("_W", bound=ValueWidget)
 
-if sys.platform == "win32":
-    _FONT = "Consolas"
-elif sys.platform == "darwin":
-    _FONT = "Menlo"
-else:
-    _FONT = "Monospace"
-
 
 @merge_super_sigs
 class OptionalWidget(Container):
     """
     A container that can represent optional argument.
 
     Parameters
@@ -172,15 +167,15 @@
     """A text edit with console-like setting."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from qtpy.QtGui import QFont, QTextOption
 
         self.native: QtW.QTextEdit
-        font = QFont(_FONT)
+        font = QFont(FONT)
         font.setStyleHint(QFont.StyleHint.Monospace)
         font.setFixedPitch(True)
         self.native.setFont(font)
         self.native.setWordWrapMode(QTextOption.WrapMode.NoWrap)
 
         # set tab width
         self.tab_size = 4
@@ -293,15 +288,15 @@
 
 class _QtSpreadSheet(QtW.QTabWidget):
     def __init__(self):
         super().__init__()
         self.setMovable(True)
         self._n_table = 0
         self.tabBar().tabBarDoubleClicked.connect(self.editTabBarLabel)
-        self.tabBar().setContextMenuPolicy(Qt.CustomContextMenu)
+        self.tabBar().setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
         self.tabBar().customContextMenuRequested.connect(self.showContextMenu)
         self._line_edit = None
 
     def addTable(self, table):
         self.addTab(table, f"Sheet {self._n_table}")
         self._n_table += 1
 
@@ -420,17 +415,20 @@
         self._read_only = v
 
 
 class _QEditableComboBox(QtW.QComboBox):
     def __init__(self, parent: QtW.QWidget | None = None) -> None:
         super().__init__(parent)
         self.setEditable(True)
-        self.setSizePolicy(
-            QtW.QSizePolicy.Policy.Expanding, QtW.QSizePolicy.Policy.Fixed
-        )
+        self.setSizePolicy(QtW.QSizePolicy.Policy.Ignored, QtW.QSizePolicy.Policy.Fixed)
+
+    def showPopup(self):
+        """Do not abbreviate the text."""
+        self.view().setMinimumWidth(self.view().sizeHintForColumn(0))
+        return super().showPopup()
 
     def keyPressEvent(self, event: QtGui.QKeyEvent):
         if event.key() in (Qt.Key.Key_Down, Qt.Key.Key_Up):
             self.showPopup()
         super().keyPressEvent(event)
 
     def wheelEvent(self, e: QtGui.QWheelEvent) -> None:
@@ -514,29 +512,43 @@
         kwargs["layout"] = "horizontal"
         Container.__init__(self, **kwargs)
         self.margins = (0, 0, 0, 0)
         self._show_file_dialog = use_app().get_obj("show_file_dialog")
         self.choose_btn.changed.disconnect()
         self.line_edit.changed.disconnect()
         self.choose_btn.changed.connect(self._on_choose_clicked)
+        self.choose_btn.max_width = 60
         self.line_edit.changed.connect(lambda: self.changed.emit(self.value))
         self._append_history_of_current()
 
     def _append_history_of_current(self):
         val = self.value
         if isinstance(val, (str, Path)):
             val = str(val)
             if val != ".":
                 self.line_edit.append_history(val)
         elif isinstance(val, tuple):
             self.line_edit.append_history("; ".join(map(str, val)))
 
     def _on_choose_clicked(self):
-        super()._on_choose_clicked()
-        self._append_history_of_current()
+        _p = self.value
+        if _p:
+            start_path: Path = _p[0] if isinstance(_p, tuple) else _p
+            _start_path: str | None = os.fspath(start_path.expanduser().absolute())
+        else:
+            _start_path = None
+        result = self._show_file_dialog(
+            self.mode,
+            caption=self._btn_text,
+            start_path=_start_path,
+            filter=self.filter,
+        )
+        if result:
+            self.value = result
+            self._append_history_of_current()
 
     def append_history(self, path: str | Path):
         """Append new history to the line edit""" ""
         return self.line_edit.append_history(path)
 
     def pop_history(self, i: int):
         """Pop history at index `i`"""
```

### Comparing `magic_class-0.7.3/magicclass/widgets/plot.py` & `magic_class-0.7.4/magicclass/widgets/plot.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/separator.py` & `magic_class-0.7.4/magicclass/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/toggle_switch.py` & `magic_class-0.7.4/magicclass/widgets/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/utils.py` & `magic_class-0.7.4/magicclass/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/pywidgets/__init__.py` & `magic_class-0.7.4/magicclass/widgets/pywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/pywidgets/dict.py` & `magic_class-0.7.4/magicclass/widgets/pywidgets/dict.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/pywidgets/list.py` & `magic_class-0.7.4/magicclass/widgets/pywidgets/list.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/pywidgets/object.py` & `magic_class-0.7.4/magicclass/widgets/pywidgets/object.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/pywidgets/tree.py` & `magic_class-0.7.4/magicclass/widgets/pywidgets/tree.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/widgets/tests/test_eval.py` & `magic_class-0.7.4/magicclass/widgets/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/wrappers/__init__.py` & `magic_class-0.7.4/magicclass/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/wrappers/_abstractapi.py` & `magic_class-0.7.4/magicclass/wrappers/_abstractapi.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/wrappers/_confirm.py` & `magic_class-0.7.4/magicclass/wrappers/_confirm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 from typing import Callable, TYPE_CHECKING, TypeVar, overload
 
 from macrokit import Mock, Expr
 from magicclass.utils import show_messagebox
 from magicclass.signature import upgrade_signature
+from magicclass._exceptions import Canceled
 
 if TYPE_CHECKING:
     from magicclass._gui import BaseGui
 
 _F = TypeVar("_F", bound=Callable)
 
 
-class Canceled(RuntimeError):
-    """Raised when a function is canceled"""
-
-
 @overload
 def confirm(
     *,
     text: str | None,
     condition: Callable[..., bool] | str | Mock | Expr | None,
     callback: Callable[[str, BaseGui], None] | None = None,
 ) -> Callable[[_F], _F]:
@@ -32,21 +29,15 @@
     text: str | None,
     condition: Callable[..., bool] | str | Mock | Expr | None,
     callback: Callable[[str, BaseGui], None] | None = None,
 ) -> _F:
     ...
 
 
-def confirm(
-    f: _F | None = None,
-    *,
-    text: str | None = None,
-    condition: Callable[[BaseGui], bool] | str | Mock | Expr | None = None,
-    callback: Callable[[str, BaseGui], None] | None = None,
-):
+def confirm(f=None, *, text=None, condition=None, callback=None):
     """
     Confirm if it is OK to run function in GUI.
 
     Useful when the function will irreversibly delete or update something in GUI.
     Confirmation will be executed only when function is called in GUI.
 
     Parameters
```

### Comparing `magic_class-0.7.3/magicclass/wrappers/_misc.py` & `magic_class-0.7.4/magicclass/wrappers/_misc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/wrappers/_preview.py` & `magic_class-0.7.4/magicclass/wrappers/_preview.py`

 * *Files 19% similar despite different names*

```diff
@@ -163,13 +163,36 @@
                 prev_ns = qualnames[-2]
                 while ins.__class__.__name__ != prev_ns:
                     if ins.__magicclass_parent__ is None:
                         break
                     ins = ins.__magicclass_parent__
                 args = (ins,) + args[1:]
 
-        with ins.macro.blocked():
-            # filter input arguments
+            with ins.macro.blocked(), ins._error_mode.raise_with_handler(ins):
+                # filter input arguments
+                try:
+                    out = f(*_filter(args))
+                except Exception as e:
+                    raise PreviewError(e, f) from e
+        else:
             out = f(*_filter(args))
         return out
 
     return _func
+
+
+class PreviewError(Exception):
+    """Error raised during preview."""
+
+    def __init__(self, exc: Exception, target_func: Callable):
+        super().__init__(str(exc))
+        self._target_qualname: str = getattr(
+            target_func, "__qualname__", repr(target_func)
+        )
+        self._original_type = type(exc)
+
+    def __str__(self):
+        return (
+            f"{self.__class__.__name__}: Error calling preview function of "
+            f"`{self._target_qualname}`...\n{self._original_type.__name__}: "
+            f"{super().__str__()}"
+        )
```

### Comparing `magic_class-0.7.3/magicclass/core.pyi` & `magic_class-0.7.4/magicclass/core.pyi`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/testing/_function_gui_test.py` & `magic_class-0.7.4/magicclass/testing/_function_gui_test.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/magicclass/testing/_gui_test.py` & `magic_class-0.7.4/magicclass/testing/_gui_test.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/.gitignore` & `magic_class-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/LICENSE` & `magic_class-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/README.md` & `magic_class-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.3/pyproject.toml` & `magic_class-0.7.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 [project]
 name = "magic-class"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 description = "Generate multifunctional GUIs from classes"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 authors = [
     { name = "Hanjin Liu", email = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp" },
 ]
 dependencies = [
-    "macro-kit>=0.4.0",
+    "macro-kit>=0.4.6",
     "magicgui>=0.7.0",
     "qtpy>=1.10.0",
     "superqt>=0.4.0",
 ]
 
 [project.optional-dependencies]
 pyqt5 = ["pyqt5>=5.12.0"]
```

### Comparing `magic_class-0.7.3/PKG-INFO` & `magic_class-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-class
-Version: 0.7.3
+Version: 0.7.4
 Summary: Generate multifunctional GUIs from classes
 Project-URL: Download, https://github.com/hanjinliu/magic-class
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
@@ -34,19 +34,20 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Requires-Dist: macro-kit>=0.4.0
+Requires-Python: >=3.8
+Requires-Dist: macro-kit>=0.4.6
 Requires-Dist: magicgui>=0.7.0
 Requires-Dist: qtpy>=1.10.0
 Requires-Dist: superqt>=0.4.0
 Provides-Extra: pyqt5
 Requires-Dist: pyqt5>=5.12.0; extra == 'pyqt5'
 Provides-Extra: pyqt6
 Requires-Dist: pyqt6; extra == 'pyqt6'
```

