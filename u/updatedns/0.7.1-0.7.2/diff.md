# Comparing `tmp/updatedns-0.7.1.tar.gz` & `tmp/updatedns-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "updatedns-0.7.1.tar", last modified: Wed Mar  1 19:56:18 2023, max compression
+gzip compressed data, was "updatedns-0.7.2.tar", last modified: Wed Jul 12 18:13:56 2023, max compression
```

## Comparing `updatedns-0.7.1.tar` & `updatedns-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-01 19:56:18.330225 updatedns-0.7.1/
--rw-r--r--   0 matt       (501) staff       (20)       44 2023-03-01 18:38:48.000000 updatedns-0.7.1/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)     1129 2023-03-01 19:56:18.330040 updatedns-0.7.1/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      845 2023-03-01 18:30:38.000000 updatedns-0.7.1/README.md
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-03-01 19:56:18.330257 updatedns-0.7.1/setup.cfg
--rwxr-xr-x   0 matt       (501) staff       (20)      931 2023-03-01 19:55:32.000000 updatedns-0.7.1/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-01 19:56:18.328936 updatedns-0.7.1/updatedns/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-03-01 18:37:12.000000 updatedns-0.7.1/updatedns/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      201 2023-03-01 18:36:39.000000 updatedns-0.7.1/updatedns/updatedns-exit-hook
--rwxr-xr-x   0 matt       (501) staff       (20)     8536 2023-03-01 19:53:03.000000 updatedns-0.7.1/updatedns/updatedns.py
--rw-r--r--   0 matt       (501) staff       (20)      121 2023-03-01 18:37:37.000000 updatedns-0.7.1/updatedns/updatedns.service
--rw-r--r--   0 matt       (501) staff       (20)      159 2023-03-01 19:56:15.000000 updatedns-0.7.1/updatedns/version.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-01 19:56:18.329850 updatedns-0.7.1/updatedns.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     1129 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      386 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       55 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/entry_points.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-03-01 19:40:20.000000 updatedns-0.7.1/updatedns.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       16 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       10 2023-03-01 19:56:18.000000 updatedns-0.7.1/updatedns.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-12 18:13:56.747764 updatedns-0.7.2/
+-rw-r--r--   0 matt      (1000) matt      (1000)       43 2023-07-12 18:01:53.000000 updatedns-0.7.2/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1142 2023-07-12 18:13:56.747764 updatedns-0.7.2/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      798 2023-03-01 20:06:10.000000 updatedns-0.7.2/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-07-12 18:13:56.747764 updatedns-0.7.2/setup.cfg
+-rwxr-xr-x   0 matt      (1000) matt      (1000)      985 2023-07-12 18:13:54.000000 updatedns-0.7.2/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-12 18:13:56.747764 updatedns-0.7.2/updatedns/
+-rw-r--r--   0 matt      (1000) matt      (1000)        0 2023-03-01 18:37:12.000000 updatedns-0.7.2/updatedns/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      201 2023-03-01 18:36:39.000000 updatedns-0.7.2/updatedns/updatedns-exit-hook
+-rwxr-xr-x   0 matt      (1000) matt      (1000)     8662 2023-03-02 01:39:54.000000 updatedns-0.7.2/updatedns/updatedns.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      121 2023-03-01 18:37:37.000000 updatedns-0.7.2/updatedns/updatedns.service
+-rw-r--r--   0 matt      (1000) matt      (1000)      159 2023-03-03 13:06:28.000000 updatedns-0.7.2/updatedns/version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-12 18:13:56.747764 updatedns-0.7.2/updatedns.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1142 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      386 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       56 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2023-03-01 19:40:20.000000 updatedns-0.7.2/updatedns.egg-info/not-zip-safe
+-rw-r--r--   0 matt      (1000) matt      (1000)       16 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2023-07-12 18:13:56.000000 updatedns-0.7.2/updatedns.egg-info/top_level.txt
```

### Comparing `updatedns-0.7.1/PKG-INFO` & `updatedns-0.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: updatedns
-Version: 0.7.1
+Version: 0.7.2
 Summary: Command-Line Cloud DNS utility
 Home-page: https://shaw.cx/updatedns
 Author: Matthew Shaw
 Author-email: mshaw.cx@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
 
 UpdateDNS
 =========
 
 Edit updatedns.ini to specify the API key for each provider hosting your DNS.
 Add a FQDN entry specifying which interface to monitor and update.
 
@@ -31,23 +33,21 @@
 	[yep.example.com]
 	interface = eth0
 
 	[yep.test.io]
 	interface = eth0
 
 
-Providers as of libcloud-2.8.0
+Providers as of libcloud-3.7.0
 ------------------------------
 * auroradns
 * buddyns
 * cloudflare
 * digital_ocean
 * dnsimple
-* dnspod
-* dummy
 * durabledns
 * gandi
 * gandi_live
 * godaddy
 * google
 * hostvirtual
 * linode
@@ -55,16 +55,16 @@
 * luadns
 * nfsn
 * nsone
 * onapp
 * pointdns
 * powerdns
 * rackspace
-* rackspace_uk
-* rackspace_us
 * rcodezero
 * route53
 * softlayer
 * vultr
 * worldwidedns
 * zerigo
 * zonomi
+
+
```

### Comparing `updatedns-0.7.1/README.md` & `updatedns-0.7.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,21 @@
 	[yep.example.com]
 	interface = eth0
 
 	[yep.test.io]
 	interface = eth0
 
 
-Providers as of libcloud-2.8.0
+Providers as of libcloud-3.7.0
 ------------------------------
 * auroradns
 * buddyns
 * cloudflare
 * digital_ocean
 * dnsimple
-* dnspod
-* dummy
 * durabledns
 * gandi
 * gandi_live
 * godaddy
 * google
 * hostvirtual
 * linode
@@ -44,16 +42,14 @@
 * luadns
 * nfsn
 * nsone
 * onapp
 * pointdns
 * powerdns
 * rackspace
-* rackspace_uk
-* rackspace_us
 * rcodezero
 * route53
 * softlayer
 * vultr
 * worldwidedns
 * zerigo
 * zonomi
```

### Comparing `updatedns-0.7.1/setup.py` & `updatedns-0.7.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     author               = __author__,
     author_email         = __email__,
     version              = __version__,
     license              = __license__,
     url                  = 'https://shaw.cx/updatedns',
     description          = 'Command-Line Cloud DNS utility',
     long_description     = open('README.md').read(),
+    long_description_content_type = 'text/markdown', 
     packages             = setuptools.find_packages(),
     include_package_data = True,
     zip_safe             = False,
     install_requires = [
         'apache-libcloud',
         ],
     entry_points = {
```

### Comparing `updatedns-0.7.1/updatedns/updatedns.py` & `updatedns-0.7.2/updatedns/updatedns.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
             for zone in zones:
                 zone_domain = zone.domain
                 if zone_domain.endswith('.'):
                     zone_domain = zone_domain[:-1]
 
                 if zone_domain not in self.domains:
-                    self._log('Skipping', zone_domain)
+                    self._log(f'Skipping {zone_domain}')
                     continue
 
                 self.domains[zone_domain].append(zone)
 
                 for record in driver.list_records(zone):
                     if record.type != 'A':
                         continue
@@ -206,44 +206,46 @@
     def _find_driver(self, fqdn):
         for zone_domain in self.domains:
             if not fqdn.endswith(zone_domain):
                 continue
             driver,zone = self.domains[zone_domain]
             name = fqdn[:-(len(zone_domain)+1)]
             return driver,zone,name
-
         raise ValueError('Unknown domain:', fqdn)
 
     def create(self, fqdn, addr):
         driver,zone,name = self._find_driver(fqdn)
 
         if fqdn in self.records:
             record = self.records[fqdn]
             if addr != record.data:
                 self.records[fqdn] = driver.update_record(record, data=addr)
-                self._log('Updated:', fqdn, '=', addr)
+                self._log(f'Updated: {fqdn} = {addr}')
                 return True
             else:
-                self._log('No change:', fqdn, '=', addr)
+                self._log(f'No change: {fqdn} = {addr}')
         else:
-            self.records[fqdn] = driver.create_record(name, zone, RecordType.A, addr)
-            self._log('Created:', fqdn, '=', addr)
-            return True
+            try:
+                self.records[fqdn] = driver.create_record(name, zone, RecordType.A, addr)
+                self._log(f'Created: {fqdn} = {addr}')
+                return True
+            except Exception as e:
+                print(f'[!] Error: {e}', file=sys.stderr)
 
     def delete(self, fqdns):
         for fqdn in fqdns:
             if fqdn not in self.records:
-                self._log('Unknown host:', fqdn)
+                self._log(f'Unknown host: {fqdn}')
                 continue
 
             driver,zone,name = self._find_driver(fqdn)
 
             driver.delete_record(self.records[fqdn])
             del self.records[fqdn]
-            self._log('Deleted:', fqdn)
+            self._log(f'Deleted: {fqdn}')
 
     def monitor(self):
         def get_local_address(ifname):
             SIOCGIFADDR = 0x8915
             skt = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             ifname = ifname[:15].encode('ascii')
             ifname = struct.pack('256s', ifname)
@@ -251,15 +253,15 @@
             return socket.inet_ntoa(data[20:24])
 
         while True:
             for interface,fqdns in self.interfaces.items():
                 try:
                     local_address = get_local_address(interface)
                 except Exception as e:
-                    self._log('Could not get address for interface', interface, ':', e)
+                    self._log(f'Could not get address for interface {interface}: {e}')
                     continue
                 for fqdn in fqdns:
                     modified = self.create(fqdn,local_address)
                     if modified:
                         self._log(f'Updated: {fqdn} = {local_address}')
             time.sleep(60.0)
```

### Comparing `updatedns-0.7.1/updatedns.egg-info/PKG-INFO` & `updatedns-0.7.2/updatedns.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: updatedns
-Version: 0.7.1
+Version: 0.7.2
 Summary: Command-Line Cloud DNS utility
 Home-page: https://shaw.cx/updatedns
 Author: Matthew Shaw
 Author-email: mshaw.cx@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
 
 UpdateDNS
 =========
 
 Edit updatedns.ini to specify the API key for each provider hosting your DNS.
 Add a FQDN entry specifying which interface to monitor and update.
 
@@ -31,23 +33,21 @@
 	[yep.example.com]
 	interface = eth0
 
 	[yep.test.io]
 	interface = eth0
 
 
-Providers as of libcloud-2.8.0
+Providers as of libcloud-3.7.0
 ------------------------------
 * auroradns
 * buddyns
 * cloudflare
 * digital_ocean
 * dnsimple
-* dnspod
-* dummy
 * durabledns
 * gandi
 * gandi_live
 * godaddy
 * google
 * hostvirtual
 * linode
@@ -55,16 +55,16 @@
 * luadns
 * nfsn
 * nsone
 * onapp
 * pointdns
 * powerdns
 * rackspace
-* rackspace_uk
-* rackspace_us
 * rcodezero
 * route53
 * softlayer
 * vultr
 * worldwidedns
 * zerigo
 * zonomi
+
+
```

