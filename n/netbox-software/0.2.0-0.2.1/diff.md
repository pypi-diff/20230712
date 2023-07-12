# Comparing `tmp/netbox_software-0.2.0.tar.gz` & `tmp/netbox_software-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.2.0.tar", max compression
+gzip compressed data, was "netbox_software-0.2.1.tar", max compression
```

## Comparing `netbox_software-0.2.0.tar` & `netbox_software-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.0/LICENSE
--rw-r--r--   0        0        0     3420 2023-07-12 08:59:31.636782 netbox_software-0.2.0/README.md
--rw-r--r--   0        0        0      640 2023-07-12 08:57:46.799132 netbox_software-0.2.0/netbox_software/__init__.py
--rw-r--r--   0        0        0      432 2023-07-12 08:33:18.432206 netbox_software-0.2.0/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.0/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     3423 2023-07-12 08:39:44.218151 netbox_software-0.2.0/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      317 2023-07-12 08:47:07.805077 netbox_software-0.2.0/netbox_software/api/urls.py
--rw-r--r--   0        0        0      803 2023-07-12 08:39:44.214151 netbox_software-0.2.0/netbox_software/api/views.py
--rw-r--r--   0        0        0     2944 2023-07-12 08:49:48.671608 netbox_software-0.2.0/netbox_software/filtersets.py
--rw-r--r--   0        0        0     4266 2023-07-12 08:33:18.392206 netbox_software-0.2.0/netbox_software/forms.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.0/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     6323 2023-07-12 08:39:44.202150 netbox_software-0.2.0/netbox_software/models.py
--rw-r--r--   0        0        0     2327 2023-07-12 08:57:46.807132 netbox_software-0.2.0/netbox_software/navigation.py
--rw-r--r--   0        0        0      799 2023-07-12 08:33:18.436206 netbox_software-0.2.0/netbox_software/search.py
--rw-r--r--   0        0        0     3286 2023-07-12 08:33:18.444206 netbox_software-0.2.0/netbox_software/tables.py
--rw-r--r--   0        0        0     3755 2023-07-12 08:33:18.428206 netbox_software-0.2.0/netbox_software/template_content.py
--rw-r--r--   0        0        0     1606 2023-07-12 07:09:12.516168 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0     2194 2023-07-11 16:51:09.747148 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2384 2023-06-23 07:56:09.499077 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.0/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1725 2023-06-22 12:45:05.033649 netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     1519 2023-07-11 14:01:34.581904 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware.html
--rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
--rw-r--r--   0        0        0     2639 2023-06-23 07:56:09.487077 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
--rw-r--r--   0        0        0     2079 2023-07-12 08:47:07.813077 netbox_software-0.2.0/netbox_software/urls.py
--rw-r--r--   0        0        0     3139 2023-07-12 08:33:18.388206 netbox_software-0.2.0/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-07-12 08:57:46.807132 netbox_software-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-12 13:04:05.122871 netbox_software-0.2.1/README.md
+-rw-r--r--   0        0        0      640 2023-07-12 13:04:05.106870 netbox_software-0.2.1/netbox_software/__init__.py
+-rw-r--r--   0        0        0      432 2023-07-12 08:33:18.432206 netbox_software-0.2.1/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.1/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     3279 2023-07-12 09:55:40.939239 netbox_software-0.2.1/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      317 2023-07-12 08:47:07.805077 netbox_software-0.2.1/netbox_software/api/urls.py
+-rw-r--r--   0        0        0      797 2023-07-12 09:21:02.309618 netbox_software-0.2.1/netbox_software/api/views.py
+-rw-r--r--   0        0        0     3000 2023-07-12 12:42:24.681855 netbox_software-0.2.1/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     4341 2023-07-12 09:26:23.994787 netbox_software-0.2.1/netbox_software/forms.py
+-rw-r--r--   0        0        0     4000 2023-07-12 09:30:42.438940 netbox_software-0.2.1/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.1/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     6449 2023-07-12 09:43:09.423061 netbox_software-0.2.1/netbox_software/models.py
+-rw-r--r--   0        0        0     2616 2023-07-12 09:55:40.931239 netbox_software-0.2.1/netbox_software/navigation.py
+-rw-r--r--   0        0        0      799 2023-07-12 08:33:18.436206 netbox_software-0.2.1/netbox_software/search.py
+-rw-r--r--   0        0        0     3283 2023-07-12 09:28:27.960779 netbox_software-0.2.1/netbox_software/tables.py
+-rw-r--r--   0        0        0     5647 2023-07-12 12:45:38.932973 netbox_software-0.2.1/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1606 2023-07-12 07:09:12.516168 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2194 2023-07-11 16:51:09.747148 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2387 2023-07-12 12:46:24.945718 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.1/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1685 2023-07-12 09:48:10.295965 netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     2079 2023-07-12 08:47:07.813077 netbox_software-0.2.1/netbox_software/urls.py
+-rw-r--r--   0        0        0     3139 2023-07-12 08:33:18.388206 netbox_software-0.2.1/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-07-12 13:04:05.114870 netbox_software-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.1/PKG-INFO
```

### Comparing `netbox_software-0.2.0/LICENSE` & `netbox_software-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/README.md` & `netbox_software-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.0          |
+|     3.2+       | 0.2.1          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

### Comparing `netbox_software-0.2.0/netbox_software/__init__.py` & `netbox_software-0.2.1/netbox_software/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.2.0'
+    version = '0.2.1'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
```

### Comparing `netbox_software-0.2.0/netbox_software/api/serializers.py` & `netbox_software-0.2.1/netbox_software/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from django.contrib.contenttypes.models import ContentType
 
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
 from netbox.api.fields import ChoiceField, ContentTypeField, SerializedPKRelatedField
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from utilities.api import get_serializer_for_model
 from ..models import DeviceSoftware, SoftwareType, Vendor, SOFTWARE_ASSIGNMENT_MODELS
-from dcim.api.nested_serializers import NestedDeviceSerializer
-from virtualization.api.nested_serializers import NestedVirtualMachineSerializer
 
 
 # Vendor Serializer
 class VendorSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_software-api:vendor-detail')
 
     class Meta:
```

### Comparing `netbox_software-0.2.0/netbox_software/api/views.py` & `netbox_software-0.2.1/netbox_software/api/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import models, filtersets
-from .serializers import DeviceSoftwareSerializer, SoftwareTypeSerializer, \
-    VendorSerializer
+from .serializers import DeviceSoftwareSerializer, SoftwareTypeSerializer, VendorSerializer
 
 
 class VendorViewSet(NetBoxModelViewSet):
     queryset = models.Vendor.objects.all()
     serializer_class = VendorSerializer
     filterset_class = filtersets.VendorFilterSet
```

### Comparing `netbox_software-0.2.0/netbox_software/filtersets.py` & `netbox_software-0.2.1/netbox_software/filtersets.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,30 +35,30 @@
             Q(name__icontains=value) |
             Q(comments__icontains=value)
         )
 
 
 class DeviceSoftwareFilterSet(NetBoxModelFilterSet):
     device = MultiValueCharFilter(
-        method='device',
+        method='filter_device',
         field_name='name',
         label=_('Device (name)'),
     )
     device_id = MultiValueNumberFilter(
-        method='device',
+        method='filter_device',
         field_name='pk',
         label=_('Device (ID)'),
     )
     virtual_machine = MultiValueCharFilter(
-        method='virtualmachine',
+        method='filter_virtual_machine',
         field_name='name',
         label=_('Virtual machine (name)'),
     )
     virtual_machine_id = MultiValueNumberFilter(
-        method='virtualmachine',
+        method='filter_virtual_machine',
         field_name='pk',
         label=_('Virtual machine (ID)'),
     )
 
     class Meta:
         model = DeviceSoftware
         fields = ('id', 'name', 'software_type', 'vendor')
@@ -67,29 +67,31 @@
         if not value.strip():
             return queryset
         return queryset.filter(
             Q(name__icontains=value) |
             Q(version__icontains=value)
         )
 
-    # def filter_device(self, queryset, name, value):
-    #     devices = Device.objects.filter(**{'{}__in'.format(name): value})
-    #     if not devices.exists():
-    #         return queryset.none()
-    #     devices_ids = []
-    #     for device in devices:
-    #         devices_ids.extend(device.values_list('id', flat=True))
-    #     return queryset.filter(
-    #         devices__in=devices_ids
-    #     )
-    #
-    # def filter_virtual_machine(self, queryset, name, value):
-    #     virtual_machines = VirtualMachine.objects.filter(**{'{}__in'.format(name): value})
-    #     if not virtual_machines.exists():
-    #         return queryset.none()
-    #     vm_ids = []
-    #     for vm in virtual_machines:
-    #         vm_ids.extend(vm.values_list('id', flat=True))
-    #     return queryset.filter(
-    #         virtualmachine__in=vm_ids
-    #     )
+    def filter_device(self, queryset, name, value):
+        devices = Device.objects.filter(**{'{}__in'.format(name): value})
+        if not devices.exists():
+            return queryset.none()
+        devices_ids = []
+        for device in devices:
+            devices_ids.append(device.id)
+        return queryset.filter(
+            assigned_object_id__in=devices_ids,
+            assigned_object_type__model='device'
+        )
+
+    def filter_virtual_machine(self, queryset, name, value):
+        virtual_machines = VirtualMachine.objects.filter(**{'{}__in'.format(name): value})
+        if not virtual_machines.exists():
+            return queryset.none()
+        vm_ids = []
+        for vm in virtual_machines:
+            vm_ids.append(vm.id)
+        return queryset.filter(
+            assigned_object_id__in=vm_ids,
+            assigned_object_type__model='virtualmachine'
+        )
```

### Comparing `netbox_software-0.2.0/netbox_software/forms.py` & `netbox_software-0.2.1/netbox_software/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from .models import DeviceSoftware, SoftwareType, Vendor
 
 from django.conf import settings
 from packaging import version
 
 NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
 if NETBOX_CURRENT_VERSION >= version.parse("3.5"):
-    from utilities.forms.fields import TagFilterField, CommentField, DynamicModelChoiceField
+    from utilities.forms.fields import TagFilterField, CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField
 else:
-    from utilities.forms import TagFilterField, CommentField, DynamicModelChoiceField
+    from utilities.forms import TagFilterField, CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField
 
 
 # Vendor Form & Filter Form
 class VendorForm(NetBoxModelForm):
     comments = CommentField()
 
     class Meta:
@@ -117,21 +117,21 @@
     )
 
     name = forms.CharField(
         label='Название',
         required=False
     )
 
-    device_id = forms.ModelMultipleChoiceField(
+    device_id = DynamicModelMultipleChoiceField(
         label='Устройство',
         queryset=Device.objects.all(),
         required=False
     )
 
-    virtual_machine_id = DynamicModelChoiceField(
+    virtual_machine_id = DynamicModelMultipleChoiceField(
         label='ВМ',
         queryset=VirtualMachine.objects.all(),
         required=False
     )
 
     software_type_id = forms.ModelMultipleChoiceField(
         label='Тип',
```

### Comparing `netbox_software-0.2.0/netbox_software/models.py` & `netbox_software-0.2.1/netbox_software/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 
     def get_devices(self):
         return DeviceSoftware.objects.filter(vendor=self.vendor).count()
 
     def get_software(self):
         return list(DeviceSoftware.objects.filter(vendor=self.vendor))
 
+    def get_software_count(self):
+        return DeviceSoftware.objects.filter(name=self.name, version=self.version).count()
+
 
 # class VirtualMachineSoftware(NetBoxModel):
 #     name = models.CharField(
 #         verbose_name="название",
 #         max_length=100,
 #         help_text='Укажите имя, которое будет отображаться для этого ПО.'
 #     )
```

### Comparing `netbox_software-0.2.0/netbox_software/navigation.py` & `netbox_software-0.2.1/netbox_software/navigation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from extras.plugins import PluginMenuItem, PluginMenu, PluginMenuButton
 from utilities.choices import ButtonColorChoices
 from django.conf import settings
-from django.utils.text import slugify
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_software', {})
 
 
 class MyPluginMenu(PluginMenu):
     def __init__(self, name, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -32,36 +31,48 @@
                     icon_class='mdi mdi-plus-thick',
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
 
-    # Add a menu item for Device software if enabled
-    # if plugin_settings.get('enable_virtual-machine_software'):
-    #     menuitem.append(
-    #         PluginMenuItem(
-    #             link='plugins:netbox_software:virtualmachinesoftware_list',
-    #             link_text='ПО ВМ',
-    #             buttons=[PluginMenuButton(
-    #                 link='plugins:netbox_software:virtualmachinesoftware_add',
-    #                 title='Создать',
-    #                 icon_class='mdi mdi-plus-thick',
-    #                 color=ButtonColorChoices.GREEN
-    #             )],
-    #             permissions=['dcim.view_device']
-    #         )
-    #     )
+        menuitem.append(
+            PluginMenuItem(
+                link='plugins:netbox_software:softwaretype_list',
+                link_text='Типы ПО',
+                buttons=[PluginMenuButton(
+                    link='plugins:netbox_software:softwaretype_add',
+                    title='Создать',
+                    icon_class='mdi mdi-plus-thick',
+                    color=ButtonColorChoices.GREEN
+                )],
+                permissions=['dcim.view_device']
+            )
+        )
+        menuitem.append(
+            PluginMenuItem(
+                link='plugins:netbox_software:vendor_list',
+                link_text='Вендоры',
+                buttons=[PluginMenuButton(
+                    link='plugins:netbox_software:vendor_add',
+                    title='Создать',
+                    icon_class='mdi mdi-plus-thick',
+                    color=ButtonColorChoices.GREEN
+                )],
+                permissions=['dcim.view_device']
+            )
+        )
+
     # If we are using NB 3.4.0+ display the new top level navigation option
     if settings.VERSION >= '3.4.0':
         menu = MyPluginMenu(
             name='SoftPl',
             label='Установленное ПО',
             groups=(
-                ('Программы', menuitem),
+                ('', menuitem),
             ),
             icon_class='mdi mdi-microsoft-xbox-controller-off'
         )
 
     else:
 
         # Fall back to pre 3.4 navigation option
```

### Comparing `netbox_software-0.2.0/netbox_software/search.py` & `netbox_software-0.2.1/netbox_software/search.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/tables.py` & `netbox_software-0.2.1/netbox_software/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         model = DeviceSoftware
         fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'version', 'comments', 'actions',
                   'created', 'last_updated', 'tags')
         default_columns = ('name', 'software_type', 'assigned_object', 'vendor', 'tags')
 
 
 class DeviceSoftwareAssignTable(NetBoxTable):
-    address = tables.TemplateColumn(
+    name = tables.TemplateColumn(
         template_code=SOFTWARE_ASSIGN_LINK,
         verbose_name='ПО'
     )
     status = columns.ChoiceFieldColumn()
     assigned_object = tables.Column(
         orderable=False
     )
```

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load helpers %}
 
 <div class="card">
 <h5 class="card-header">
     ПО устройства
     {% if device_software %}
-      <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device={{ object.pk }}">
+      <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device_id={{ object.pk }}">
         (всего: {{ soft_count }})</a>
     {% endif %}
 </h5>
 <div class="card-body">
 {% if device_software %}
     <table class="table table-hover">
         <tr>
```

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor.html`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,17 @@
             </tr>
             <tr>
               <th scope="row">Приложений:</th>
               <table>
                 {% if object.get_software %}
                   {% for soft in object.get_software %}
                     <tr>
-                      <th scope="row"><a href="{% url 'plugins:netbox_software:vendor' pk=soft.pk %}">{{ object.name }}</a></th>
-<!--                      <th scope="row">{{ soft.name }}</th>-->
+                      <th scope="row"><a href="{% url 'plugins:netbox_software:devicesoftware' pk=soft.pk %}">| {{ soft.name }}</a></th>
                       <td></td>
-                      <td> {{ soft.version }}</td>
+                      <td> | Версия: {{ soft.version }} |</td>
                     </tr>
                   {% endfor %}
                 {% else %}
                 <tr>
                   <th scope="row"></th>
                   <td>нет установленных приложений </td>
                   <td></td>
```

#### html2text {}

```diff
@@ -1,15 +1,12 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
 ** Ð Ð°Ð·ÑÐ°Ð±Ð¾ÑÑÐ¸Ðº **
 ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ð�{{ object.name|placeholder }}
 ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ�{{ object.get_software_count }}
 Ð²ÑÐµÐ³Ð¾
 ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ð¹:
-                                                                             {
-{{_object.name_}}                                                            {
-                                                                             soft.version
-                                                                             }}
+|_{{_soft.name_}}                                                            | ÐÐµÑÑÐ¸Ñ: {{ soft.version }} |
                                Ð½ÐµÑ ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð½ÑÑ
                                Ð¿ÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ð¹
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.2.0/netbox_software/urls.py` & `netbox_software-0.2.1/netbox_software/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/netbox_software/views.py` & `netbox_software-0.2.1/netbox_software/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.0/PKG-INFO` & `netbox_software-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,15 +27,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.0          |
+|     3.2+       | 0.2.1          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

