# Comparing `tmp/netbox_software-0.1.7.tar.gz` & `tmp/netbox_software-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.1.7.tar", max compression
+gzip compressed data, was "netbox_software-0.2.0.tar", max compression
```

## Comparing `netbox_software-0.1.7.tar` & `netbox_software-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.7/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.7/README.md
--rw-r--r--   0        0        0      636 2023-06-23 08:10:05.968201 netbox_software-0.1.7/netbox_software/__init__.py
--rw-r--r--   0        0        0      616 2023-06-19 13:55:08.848877 netbox_software-0.1.7/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     3459 2023-06-20 10:54:23.034743 netbox_software-0.1.7/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.7/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.7/netbox_software/api/views.py
--rw-r--r--   0        0        0     1705 2023-06-20 11:07:06.570213 netbox_software-0.1.7/netbox_software/filtersets.py
--rw-r--r--   0        0        0     3975 2023-06-20 10:07:37.384282 netbox_software-0.1.7/netbox_software/forms.py
--rw-r--r--   0        0        0     5261 2023-06-20 10:12:28.772709 netbox_software-0.1.7/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     5779 2023-06-22 13:29:04.297691 netbox_software-0.1.7/netbox_software/models.py
--rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/navigation.py
--rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.7/netbox_software/search.py
--rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.7/netbox_software/tables.py
--rw-r--r--   0        0        0     2663 2023-06-23 07:46:52.094449 netbox_software-0.1.7/netbox_software/template_content.py
--rw-r--r--   0        0        0     1455 2023-06-21 06:29:50.919881 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0      693 2023-06-20 10:19:13.746862 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2384 2023-06-23 07:56:09.499077 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.1.7/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1725 2023-06-22 12:45:05.033649 netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     1352 2023-06-21 06:17:56.368583 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware.html
--rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
--rw-r--r--   0        0        0     2639 2023-06-23 07:56:09.487077 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
--rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.7/netbox_software/urls.py
--rw-r--r--   0        0        0     4296 2023-06-20 14:19:58.292417 netbox_software-0.1.7/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-06-23 08:10:05.972201 netbox_software-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-12 08:59:31.636782 netbox_software-0.2.0/README.md
+-rw-r--r--   0        0        0      640 2023-07-12 08:57:46.799132 netbox_software-0.2.0/netbox_software/__init__.py
+-rw-r--r--   0        0        0      432 2023-07-12 08:33:18.432206 netbox_software-0.2.0/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.0/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     3423 2023-07-12 08:39:44.218151 netbox_software-0.2.0/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      317 2023-07-12 08:47:07.805077 netbox_software-0.2.0/netbox_software/api/urls.py
+-rw-r--r--   0        0        0      803 2023-07-12 08:39:44.214151 netbox_software-0.2.0/netbox_software/api/views.py
+-rw-r--r--   0        0        0     2944 2023-07-12 08:49:48.671608 netbox_software-0.2.0/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     4266 2023-07-12 08:33:18.392206 netbox_software-0.2.0/netbox_software/forms.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.0/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     6323 2023-07-12 08:39:44.202150 netbox_software-0.2.0/netbox_software/models.py
+-rw-r--r--   0        0        0     2327 2023-07-12 08:57:46.807132 netbox_software-0.2.0/netbox_software/navigation.py
+-rw-r--r--   0        0        0      799 2023-07-12 08:33:18.436206 netbox_software-0.2.0/netbox_software/search.py
+-rw-r--r--   0        0        0     3286 2023-07-12 08:33:18.444206 netbox_software-0.2.0/netbox_software/tables.py
+-rw-r--r--   0        0        0     3755 2023-07-12 08:33:18.428206 netbox_software-0.2.0/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1606 2023-07-12 07:09:12.516168 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2194 2023-07-11 16:51:09.747148 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2384 2023-06-23 07:56:09.499077 netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.0/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1725 2023-06-22 12:45:05.033649 netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     1519 2023-07-11 14:01:34.581904 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware.html
+-rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
+-rw-r--r--   0        0        0     2639 2023-06-23 07:56:09.487077 netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
+-rw-r--r--   0        0        0     2079 2023-07-12 08:47:07.813077 netbox_software-0.2.0/netbox_software/urls.py
+-rw-r--r--   0        0        0     3139 2023-07-12 08:33:18.388206 netbox_software-0.2.0/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-07-12 08:57:46.807132 netbox_software-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.0/PKG-INFO
```

### Comparing `netbox_software-0.1.7/LICENSE` & `netbox_software-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.7/README.md` & `netbox_software-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       |      0.5.0     |
+|     3.2+       | 0.2.0          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

### Comparing `netbox_software-0.1.7/netbox_software/__init__.py` & `netbox_software-0.2.0/netbox_software/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.1.7'
+    version = '0.2.0'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
-        "enable_virtual-machine_software": True,
+        # "enable_virtual-machine_software": True,
         "device_software_location": "left",
-        "virtual-machine_software_location": "left",
+        # "virtual-machine_software_location": "left",
     }
 
 
 config = NetboxSoftware
```

### Comparing `netbox_software-0.1.7/netbox_software/models.py` & `netbox_software-0.2.0/netbox_software/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.models import ContentType
+from django.db.models import Q
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.urls import reverse
 
 from netbox.models import NetBoxModel
 from utilities.choices import ChoiceSet
 
@@ -28,24 +31,21 @@
         devices = []
         dev_softs = DeviceSoftware.objects.filter(vendor=self)
         for soft in dev_softs:
             devices.append(soft.device.name)
         return DeviceSoftware.objects.filter(vendor=self)
 
     def get_software_count(self):
-        return DeviceSoftware.objects.filter(vendor=self).count() + VirtualMachineSoftware.objects.filter(vendor=self).count()
+        return DeviceSoftware.objects.filter(vendor=self).count()
 
     def get_software(self):
         soft_list = []
         dev_softs = DeviceSoftware.objects.filter(vendor=self)
         for soft in dev_softs:
             soft_list.append(soft)
-        vm_softs = VirtualMachineSoftware.objects.filter(vendor=self)
-        for soft in vm_softs:
-            soft_list.append(soft)
         return soft_list
 
 
 class SoftwareType(NetBoxModel):
     name = models.CharField(verbose_name="название", max_length=100, help_text='Укажите тип ПО')
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
@@ -63,26 +63,43 @@
     def get_devices_count(self):
         return DeviceSoftware.objects.filter(software_type=self).count()
 
     def get_devices(self):
         return DeviceSoftware.objects.filter(software_type=self)
 
 
+SOFTWARE_ASSIGNMENT_MODELS = Q(
+    Q(app_label='dcim', model='device') |
+    Q(app_label='virtualization', model='virtualmachine')
+)
+
+
 class DeviceSoftware(NetBoxModel):
     name = models.CharField(
         verbose_name="название",
         max_length=100,
         help_text='Укажите имя, которое будет отображаться для этого ПО.'
     )
 
-    device = models.ForeignKey(
-        verbose_name="устройство",
-        to='dcim.Device',
-        on_delete=models.CASCADE,
-        related_name='software'
+    assigned_object_type = models.ForeignKey(
+        to=ContentType,
+        limit_choices_to=SOFTWARE_ASSIGNMENT_MODELS,
+        on_delete=models.PROTECT,
+        related_name='+',
+        blank=True,
+        null=True
+    )
+
+    assigned_object_id = models.PositiveBigIntegerField(
+        blank=True,
+        null=True
+    )
+    assigned_object = GenericForeignKey(
+        ct_field='assigned_object_type',
+        fk_field='assigned_object_id'
     )
 
     software_type = models.ForeignKey(
         to=SoftwareType,
         verbose_name="тип ПО",
         on_delete=models.CASCADE,
         related_name='device_software'
@@ -110,76 +127,79 @@
         ordering = ('name',)
         verbose_name_plural = "ПО устройств"
         verbose_name = "ПО устройства"
 
     def __str__(self):
         return self.name
 
+    def to_objectchange(self, action):
+        objectchange = super().to_objectchange(action)
+        objectchange.related_object = self.assigned_object
+        return objectchange
+
     def get_absolute_url(self):
         return reverse('plugins:netbox_software:devicesoftware', args=[self.pk])
 
     def get_devices(self):
-        return DeviceSoftware.objects.filter(vendor=self.vendor).count() + \
-            VirtualMachineSoftware.objects.filter(vendor=self.vendor).count()
+        return DeviceSoftware.objects.filter(vendor=self.vendor).count()
 
     def get_software(self):
-        return list(DeviceSoftware.objects.filter(vendor=self.vendor)) + list(
-            VirtualMachineSoftware.objects.filter(vendor=self.vendor))
+        return list(DeviceSoftware.objects.filter(vendor=self.vendor))
 
 
-class VirtualMachineSoftware(NetBoxModel):
-    name = models.CharField(
-        verbose_name="название",
-        max_length=100,
-        help_text='Укажите имя, которое будет отображаться для этого ПО.'
-    )
-
-    virtual_machine = models.ForeignKey(
-        verbose_name="виртуальая машина",
-        to='virtualization.VirtualMachine',
-        on_delete=models.CASCADE,
-        related_name='software'
-    )
-
-    software_type = models.ForeignKey(
-        to=SoftwareType,
-        verbose_name="тип ПО",
-        on_delete=models.CASCADE,
-        related_name='vm_software'
-    )
-
-    vendor = models.ForeignKey(
-        to=Vendor,
-        verbose_name="Разработчик",
-        on_delete=models.CASCADE,
-        related_name='vm_software'
-    )
-
-    version = models.CharField(
-        verbose_name="версия",
-        max_length=50,
-        blank=True
-    )
-
-    comments = models.TextField(
-        verbose_name="комментарий",
-        blank=True
-    )
-
-    class Meta:
-        ordering = ('name',)
-        verbose_name_plural = "ПО виртуальных машин"
-        verbose_name = "ПО виртуальной машины"
-
-    def __str__(self):
-        return self.name
-
-    def get_absolute_url(self):
-        return reverse('plugins:netbox_software:virtualmachinesoftware', args=[self.pk])
-
-    def get_software_count(self):
-        return DeviceSoftware.objects.filter(name=self.name).count() + \
-            VirtualMachineSoftware.objects.filter(name=self.name).count()
-
-    def get_software(self):
-        return list(DeviceSoftware.objects.filter(vendor=self.vendor)) + list(
-            VirtualMachineSoftware.objects.filter(vendor=self.vendor))
+# class VirtualMachineSoftware(NetBoxModel):
+#     name = models.CharField(
+#         verbose_name="название",
+#         max_length=100,
+#         help_text='Укажите имя, которое будет отображаться для этого ПО.'
+#     )
+#
+#     virtual_machine = models.ForeignKey(
+#         verbose_name="виртуальая машина",
+#         to='virtualization.VirtualMachine',
+#         on_delete=models.CASCADE,
+#         related_name='software'
+#     )
+#
+#     software_type = models.ForeignKey(
+#         to=SoftwareType,
+#         verbose_name="тип ПО",
+#         on_delete=models.CASCADE,
+#         related_name='vm_software'
+#     )
+#
+#     vendor = models.ForeignKey(
+#         to=Vendor,
+#         verbose_name="Разработчик",
+#         on_delete=models.CASCADE,
+#         related_name='vm_software'
+#     )
+#
+#     version = models.CharField(
+#         verbose_name="версия",
+#         max_length=50,
+#         blank=True
+#     )
+#
+#     comments = models.TextField(
+#         verbose_name="комментарий",
+#         blank=True
+#     )
+#
+#     class Meta:
+#         ordering = ('name',)
+#         verbose_name_plural = "ПО виртуальных машин"
+#         verbose_name = "ПО виртуальной машины"
+#
+#     def __str__(self):
+#         return self.name
+#
+#     def get_absolute_url(self):
+#         return reverse('plugins:netbox_software:virtualmachinesoftware', args=[self.pk])
+#
+#     def get_software_count(self):
+#         return DeviceSoftware.objects.filter(name=self.name, version=self.version).count() + \
+#             VirtualMachineSoftware.objects.filter(name=self.name, version=self.version).count()
+#
+#     def get_software(self):
+#         return list(DeviceSoftware.objects.filter(vendor=self.vendor)) + list(
+#             VirtualMachineSoftware.objects.filter(vendor=self.vendor))
```

### Comparing `netbox_software-0.1.7/netbox_software/navigation.py` & `netbox_software-0.2.0/netbox_software/navigation.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,28 +33,28 @@
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
 
     # Add a menu item for Device software if enabled
-    if plugin_settings.get('enable_virtual-machine_software'):
-        menuitem.append(
-            PluginMenuItem(
-                link='plugins:netbox_software:virtualmachinesoftware_list',
-                link_text='ПО ВМ',
-                buttons=[PluginMenuButton(
-                    link='plugins:netbox_software:virtualmachinesoftware_add',
-                    title='Создать',
-                    icon_class='mdi mdi-plus-thick',
-                    color=ButtonColorChoices.GREEN
-                )],
-                permissions=['dcim.view_device']
-            )
-        )
+    # if plugin_settings.get('enable_virtual-machine_software'):
+    #     menuitem.append(
+    #         PluginMenuItem(
+    #             link='plugins:netbox_software:virtualmachinesoftware_list',
+    #             link_text='ПО ВМ',
+    #             buttons=[PluginMenuButton(
+    #                 link='plugins:netbox_software:virtualmachinesoftware_add',
+    #                 title='Создать',
+    #                 icon_class='mdi mdi-plus-thick',
+    #                 color=ButtonColorChoices.GREEN
+    #             )],
+    #             permissions=['dcim.view_device']
+    #         )
+    #     )
     # If we are using NB 3.4.0+ display the new top level navigation option
     if settings.VERSION >= '3.4.0':
         menu = MyPluginMenu(
             name='SoftPl',
             label='Установленное ПО',
             groups=(
                 ('Программы', menuitem),
```

### Comparing `netbox_software-0.1.7/netbox_software/search.py` & `netbox_software-0.2.0/netbox_software/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.search import SearchIndex
-from .models import DeviceSoftware, VirtualMachineSoftware, Vendor, SoftwareType
+from .models import DeviceSoftware, Vendor, SoftwareType
 from django.conf import settings
 
 # If we run NB 3.4+ register search indexes 
 if settings.VERSION >= '3.4.0':
     class VendorIndex(SearchIndex):
         model = Vendor
         fields = (
@@ -22,16 +22,9 @@
         model = DeviceSoftware
         fields = (
             ("name", 100),
             ("version", 500),
             ("comments", 5000),
         )
 
-    class VirtualMachineSoftwareIndex(SearchIndex):
-        model = VirtualMachineSoftware
-        fields = (
-            ("name", 100),
-            ("version", 500),
-            ("comments", 5000),
-        )
     # Register indexes
-    indexes = [DeviceSoftwareIndex, VirtualMachineSoftwareIndex]
+    indexes = [VendorIndex, SoftwareTypeIndex, DeviceSoftwareIndex]
```

### Comparing `netbox_software-0.1.7/netbox_software/tables.py` & `netbox_software-0.2.0/netbox_software/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import django_tables2 as tables
 
 from netbox.tables import NetBoxTable, columns
-from .models import DeviceSoftware, VirtualMachineSoftware, Vendor, SoftwareType
+from tenancy.tables import TenantColumn
+from .models import DeviceSoftware, Vendor, SoftwareType
 
 SOFTWARE_TYPE_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:softwaretype' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
@@ -17,22 +18,18 @@
 
 DEVICE_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
-VIRTUAL_MACHINE_SOFTWARE_LINK = """
-{% if record %}
-    <a href="{% url 'plugins:netbox_software:virtualmachinesoftware' pk=record.pk %}">
-    {% firstof record.name record.name %}</a>
-{% endif %}
+SOFTWARE_ASSIGN_LINK = """
+<a href="{% url ''plugins:netbox_software:devicesoftware' pk=record.pk %}?{% if request.GET.device_soft %}device={{ request.GET.device_soft }}{% elif request.GET.vm_soft %}vm_soft={{ request.GET.vm_soft }}{% endif %}&return_url={{ request.GET.return_url }}">{{ record }}</a>
 """
 
-
 class VendorTable(NetBoxTable):
     name = tables.TemplateColumn(template_code=VENDOR_SOFTWARE_LINK)
 
     class Meta(NetBoxTable.Meta):
         model = Vendor
         fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
         default_columns = ('name',)
@@ -54,40 +51,55 @@
     )
     vendor = tables.Column(
         linkify=True
     )
     device = tables.Column(
         linkify=True
     )
+    assigned_object = tables.Column(
+        linkify=True,
+        orderable=False,
+        verbose_name='Устройство'
+    )
 
     tags = columns.TagColumn(
         url_name='dcim:sitegroup_list'
     )
 
     class Meta(NetBoxTable.Meta):
         model = DeviceSoftware
-        fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'version', 'device', 'comments', 'actions',
+        fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'version', 'comments', 'actions',
                   'created', 'last_updated', 'tags')
-        default_columns = ('name', 'software_type', 'device', 'tags')
+        default_columns = ('name', 'software_type', 'assigned_object', 'vendor', 'tags')
 
 
-class VirtualMachineSoftwareTable(NetBoxTable):
-    name = tables.TemplateColumn(template_code=VIRTUAL_MACHINE_SOFTWARE_LINK)
-    software_type = tables.Column(
-        linkify=True
+class DeviceSoftwareAssignTable(NetBoxTable):
+    address = tables.TemplateColumn(
+        template_code=SOFTWARE_ASSIGN_LINK,
+        verbose_name='ПО'
     )
-    vendor = tables.Column(
-        linkify=True
-    )
-    virtual_machine = tables.Column(
-        linkify=True
+    status = columns.ChoiceFieldColumn()
+    assigned_object = tables.Column(
+        orderable=False
     )
 
-    tags = columns.TagColumn(
-        url_name='dcim:sitegroup_list'
+    class Meta(NetBoxTable.Meta):
+        model = DeviceSoftware
+        fields = ('name', 'software_type', 'vendor', 'version', 'assigned_object', 'description')
+        exclude = ('id', )
+        orderable = False
+
+
+class AssignedDeviceSoftwareTable(NetBoxTable):
+    """
+    List DeviceSoftware assigned to an object.
+    """
+    name = tables.Column(
+        linkify=True,
+        verbose_name='ПО'
     )
 
     class Meta(NetBoxTable.Meta):
-        model = VirtualMachineSoftware
-        fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'version', 'virtual_machine', 'comments', 'actions',
-                  'created', 'last_updated', 'tags')
-        default_columns = ('name', 'software_type', 'virtual_machine', 'tags')
+        model = DeviceSoftware
+        fields = ('name', 'software_type', 'vendor', 'version', 'assigned_object', 'description')
+        exclude = ('id', )
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netbox_software-0.1.7/netbox_software/template_content.py` & `netbox_software-0.2.0/netbox_software/template_content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,78 @@
 from extras.plugins import PluginTemplateExtension
 from django.conf import settings
-from .models import DeviceSoftware, VirtualMachineSoftware
+from .models import DeviceSoftware
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_software', {})
 
 
 class DeviceSoftwareList(PluginTemplateExtension):
     model = 'dcim.device'
     def left_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
-                'device_software': DeviceSoftware.objects.filter(device=self.context['object'])[:20],
-                'soft_count': DeviceSoftware.objects.filter(device=self.context['object']).count(),
+                'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'])[:20],
+                'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object']).count(),
             })
         else:
             return ""
 
     def right_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'right':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
-                'device_software': DeviceSoftware.objects.filter(device=self.context['object'])[:20],
-                'soft_count': DeviceSoftware.objects.filter(device=self.context['object']).count(),
+                'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'])[:20],
+                'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object']).count(),
             })
         else:
             return ""
 
 
-class VirtualMachineSoftwareList(PluginTemplateExtension):
-    model = 'virtualization.virtualmachine'
-
-    def left_page(self):
-        if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'left':
-
-            return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
-                'virtual_machine_software': VirtualMachineSoftware.objects.filter(
-                    virtual_machine=self.context['object']
-                )[:20],
-                'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
-            })
-        else:
-            return ""
-
-    def right_page(self):
-        if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'right':
-
-            return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
-                'virtual_machine_software': VirtualMachineSoftware.objects.filter(
-                    virtual_machine=self.context['object']
-                )[:20],
-                'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
-            })
-        else:
-            return ""
+# class VirtualMachineSoftwareList(PluginTemplateExtension):
+#     model = 'virtualization.virtualmachine'
+#
+#     def left_page(self):
+#         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
+#
+#             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+#                 'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'])[:20],
+#                 'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object']).count(),
+#             })
+#         else:
+#             return ""
+#
+#     def right_page(self):
+#         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'right':
+#
+#             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+#                 'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'])[:20],
+#                 'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object']).count(),
+#             })
+#         else:
+#             return ""
+#     def left_page(self):
+#         if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'left':
+#
+#             return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
+#                 'virtual_machine_software': VirtualMachineSoftware.objects.filter(
+#                     virtual_machine=self.context['object']
+#                 )[:20],
+#                 'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
+#             })
+#         else:
+#             return ""
+#
+#     def right_page(self):
+#         if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'right':
+#
+#             return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
+#                 'virtual_machine_software': VirtualMachineSoftware.objects.filter(
+#                     virtual_machine=self.context['object']
+#                 )[:20],
+#                 'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
+#             })
+#         else:
+#             return ""
 
 
-template_extensions = [DeviceSoftwareList, VirtualMachineSoftwareList]
+template_extensions = [DeviceSoftwareList]
```

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">ПО устройства</h5>
+        <h5 class="card-header">ПО виртуальных машин</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Название ПО</th>
               <td>{{ object.name|placeholder }}</td>
             </tr>
             <tr>
-              <th scope="row">Устройство</th>
-              <td><a href="{% url 'dcim:device' pk=object.device.pk %}">{{ object.device }}</a></td>
+              <th scope="row">Виртуальная машина</th>
+              <td><a href="{% url 'virtualization:virtualmachine' pk=object.virtual_machine.pk %}">{{ object.virtual_machine }}</a></td>
             </tr>
             <tr>
               <th scope="row">Тип ПО</th>
               <td>{{ object.software_type }}</td>
             </tr>
             <tr>
               <th scope="row">Установлено</th>
               <td> на {{ object.get_software_count }} хостах</td>
             </tr>
             <tr>
               <th scope="row">Разработчик</th>
-              <td>{{ object.vendor }}</tr>
+              <td>{{ object.vendor|placeholder }}</tr>
             <tr>
               <th scope="row">Версия</th>
-              <td>{{ object.version|placeholder }}</tr>
+              <td>{{ object.version }}</tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
-** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
-ÐÐ°Ð·Ð²Ð°Ð�{{ object.name|placeholder }}
-Ð£ÑÑÑÐ¾Ð�{{_object.device_}}
-Ð¢Ð¸Ð¿ ÐÐ  {{ object.software_type }}
-Ð£ÑÑÐ°Ð½Ð�Ð½Ð° {{ object.get_software_count }} ÑÐ¾ÑÑÐ°Ñ
-Ð Ð°Ð·ÑÐ°Ð�{{ object.vendor }}º
-ÐÐµÑÑÐ¸Ñ�{{ object.version|placeholder }}
+** ÐÐ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½ÑÑ Ð¼Ð°ÑÐ¸Ð½ **
+ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ðµ Ð�{{ object.name|placeholder }}
+ÐÐ¸ÑÑÑÐ°Ð»ÑÐ½{{_object.virtual_machine_}}�Ð°
+Ð¢Ð¸Ð¿ ÐÐ               {{ object.software_type }}
+Ð£ÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð° {{ object.get_software_count }}
+                                    ÑÐ¾ÑÑÐ°Ñ
+Ð Ð°Ð·ÑÐ°Ð±Ð¾ÑÑ{{ object.vendor|placeholder }}
+ÐÐµÑÑÐ¸Ñ            {{ object.version }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/software_edit.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-/p  {% extends 'generic/object_edit.html' %}
+{% extends 'generic/object_edit.html' %}
 {% load static %}
 {% load form_helpers %}
 {% load helpers %}
 
 {% block form %}
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
         {% render_field form.vendor %}
         {% render_field form.version %}
-        {% render_field form.device %}
 
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
             {% render_field form.comments %}
         </div>
```

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
         {% render_field form.vendor %}
         {% render_field form.version %}
-
+        {% render_field form.virtual_machine %}
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
             {% render_field form.comments %}
         </div>
```

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html` & `netbox_software-0.2.0/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.7/netbox_software/urls.py` & `netbox_software-0.2.0/netbox_software/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,22 +30,8 @@
     path('device-software/<int:pk>/', views.DeviceSoftwareView.as_view(), name='devicesoftware'),
     path('device-software/<int:pk>/edit/', views.DeviceSoftwareEditView.as_view(), name='devicesoftware_edit'),
     path('device-software/<int:pk>/delete/', views.DeviceSoftwareDeleteView.as_view(), name='devicesoftware_delete'),
     path('device-software/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='devicesoftware_changelog', kwargs={
         'model': models.DeviceSoftware
     }),
 
-    # VirtualMachineSoftware
-    path('virtual-machine-software/', views.VirtualMachineSoftwareListView.as_view(),
-         name='virtualmachinesoftware_list'),
-    path('virtual-machine-software/add/', views.VirtualMachineSoftwareEditView.as_view(),
-         name='virtualmachinesoftware_add'),
-    path('virtual-machine-software/<int:pk>/', views.VirtualMachineSoftwareView.as_view(),
-         name='virtualmachinesoftware'),
-    path('virtual-machine-software/<int:pk>/edit/', views.VirtualMachineSoftwareEditView.as_view(),
-         name='virtualmachinesoftware_edit'),
-    path('virtual-machine-software/<int:pk>/delete/', views.VirtualMachineSoftwareDeleteView.as_view(),
-         name='virtualmachinesoftware_delete'),
-    path('virtual-machine-software/<int:pk>/changelog/', ObjectChangeLogView.as_view(),
-         name='virtualmachinesoftware_changelog', kwargs={'model': models.VirtualMachineSoftware}),
-
 )
```

### Comparing `netbox_software-0.1.7/netbox_software/views.py` & `netbox_software-0.2.0/netbox_software/views.py`

 * *Files 27% similar despite different names*

```diff
@@ -78,34 +78,7 @@
 
     template_name = 'netbox_software/devicesoftware_edit.html'
 
 
 class DeviceSoftwareDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.DeviceSoftware.objects.all()
-
-
-### VirtualMachineSoftware
-class VirtualMachineSoftwareView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = ('dcim.view_site', 'dcim.view_device')
-    queryset = models.VirtualMachineSoftware.objects.all()
-
-
-class VirtualMachineSoftwareListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = ('dcim.view_site', 'dcim.view_device')
-    queryset = models.VirtualMachineSoftware.objects.all()
-    table = tables.VirtualMachineSoftwareTable
-    filterset = filtersets.VirtualMachineSoftwareFilterSet
-    filterset_form = forms.VirtualMachineSoftwareFilterForm
-
-
-class VirtualMachineSoftwareEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = ('dcim.view_site', 'dcim.view_device')
-    queryset = models.VirtualMachineSoftware.objects.all()
-    form = forms.VirtualMachineSoftwareForm
-
-    template_name = 'netbox_software/virtualmachinesoftware_edit.html'
-
-
-class VirtualMachineSoftwareDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = ('dcim.view_site', 'dcim.view_device')
-    queryset = models.VirtualMachineSoftware.objects.all()
```

### Comparing `netbox_software-0.1.7/PKG-INFO` & `netbox_software-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.1.7
+Version: 0.2.0
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
-|     3.2+       |      0.5.0     |
+|     3.2+       | 0.2.0          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

