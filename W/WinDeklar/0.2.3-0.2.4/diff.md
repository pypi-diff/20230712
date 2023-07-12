# Comparing `tmp/windeklar-0.2.3.tar.gz` & `tmp/windeklar-0.2.4.tar.gz`

## Comparing `windeklar-0.2.3.tar` & `windeklar-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.3/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.3/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/__init__.py
--rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    45855 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.3/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.3/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.4/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.4/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/__init__.py
+-rwxr-xr-x   0        0        0    16073 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.4/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.4/PKG-INFO
```

### Comparing `windeklar-0.2.3/.github/workflows/python-publish.yml` & `windeklar-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/QTAux.py` & `windeklar-0.2.4/src/WinDeklar/QTAux.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,24 +393,22 @@
 class Label(ScreenControl):
     """
     Read only text (also known as Label)
     """
     def __init__(self, name, title, bound, action, layout, tooltip=None, align_left=True):
 
         # Widget must be created before calling super
-        self.text = QtWidgets.QLabel(title)
+        self.label_title = title
+        self.text        = QtWidgets.QLabel(title)
+        self.text.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         if align_left:
             self.text.setAlignment(QtCore.Qt.AlignLeft)
         bound.set_control_value_if_not_present(name, title)
         super(Label, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
-    def title(self):
-        # returns '' to avoid creating another Label
-        return ''
-
     def get_widget(self):
         return True, self.text
 
     def refresh(self):
         # print('current value:%s' % self.current_value())
         self.text.setText('%s' % self.current_value())
```

### Comparing `windeklar-0.2.3/src/WinDeklar/WindowForm.py` & `windeklar-0.2.4/src/WinDeklar/WindowForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,15 +1152,15 @@
         qt_control = def_button(c_name, e_name, provider, layout, action, control, tooltip=tooltip)
     elif c_type == 'Constant':
         result = False
         qt_control = def_constant(c_name, e_name, provider, layout, action)
     elif c_type == 'Check':
         result = True
         qt_control = QTAux.CheckButton(c_name, e_name, provider, action, layout, tooltip=tooltip)
-    elif c_type == 'Text':
+    elif c_type in ['Text', 'Label']:
         result = True
         qt_control = QTAux.Label(c_name, e_name, provider, action, layout)
     elif c_type == 'EditText':
         result = True
         qt_control = QTAux.EditText(c_name, e_name, provider, action, layout, tooltip=tooltip)
     elif c_type == 'EditNumber':
         result = True
```

### Comparing `windeklar-0.2.3/src/WinDeklar/graph_aux.py` & `windeklar-0.2.4/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/points_box.py` & `windeklar-0.2.4/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/record.py` & `windeklar-0.2.4/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/signal_aux.py` & `windeklar-0.2.4/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/test_animation.py` & `windeklar-0.2.4/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.4/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/view_animation.py` & `windeklar-0.2.4/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/view_animation.yaml` & `windeklar-0.2.4/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/view_example.py` & `windeklar-0.2.4/src/WinDeklar/view_example.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/view_example.yaml` & `windeklar-0.2.4/src/WinDeklar/view_example.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,19 @@
                       - control:
                           name:    line_width
                           title:   Line Width
                           type:    EditNumberSpin
                           parms:   {step: 1.0, maximum: 10}
                           value:   1.0
                       - control:
+                          name:    just_text
+                          title:   ''  # null to avoid present it on the form
+                          type:    Text
+                          value:   Text
+                      - control:
                           name:    redraw
                           title:   Draw again
                           type:    Button
                           action:  redraw   # method to call
 
                 - item:
                     name:    figures
```

### Comparing `windeklar-0.2.3/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.4/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.4/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/LICENSE` & `windeklar-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/README.md` & `windeklar-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.3/pyproject.toml` & `windeklar-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2.3/PKG-INFO` & `windeklar-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2.3
+Version: 0.2.4
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

