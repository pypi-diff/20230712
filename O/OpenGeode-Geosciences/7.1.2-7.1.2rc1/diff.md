# Comparing `tmp/OpenGeode_Geosciences-7.1.2-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-7.1.2rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 547033 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-12 00:48 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Jul-12 00:48 opengeode_geosciences/explicit.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Jul-12 00:48 opengeode_geosciences/implicit.py
--rw-rw-rw-  2.0 fat   573440 b- defN 23-Jul-12 00:51 opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll
--rw-rw-rw-  2.0 fat   482304 b- defN 23-Jul-12 00:51 opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll
--rw-rw-rw-  2.0 fat   387072 b- defN 23-Jul-12 00:51 opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   334336 b- defN 23-Jul-12 00:51 opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3232 b- defN 23-Jul-12 00:51 OpenGeode_Geosciences-7.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-12 00:51 OpenGeode_Geosciences-7.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jul-12 00:51 OpenGeode_Geosciences-7.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1136 b- defN 23-Jul-12 00:51 OpenGeode_Geosciences-7.1.2.dist-info/RECORD
-11 files, 1784319 bytes uncompressed, 545057 bytes compressed:  69.5%
+Zip file size: 547061 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-11 09:04 opengeode_geosciences/__init__.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-Jul-11 09:04 opengeode_geosciences/explicit.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-Jul-11 09:04 opengeode_geosciences/implicit.py
+-rw-rw-rw-  2.0 fat   573440 b- defN 23-Jul-11 09:06 opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll
+-rw-rw-rw-  2.0 fat   482304 b- defN 23-Jul-11 09:06 opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll
+-rw-rw-rw-  2.0 fat   387072 b- defN 23-Jul-11 09:06 opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   334336 b- defN 23-Jul-11 09:06 opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3238 b- defN 23-Jul-11 09:06 OpenGeode_Geosciences-7.1.2rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-11 09:06 OpenGeode_Geosciences-7.1.2rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jul-11 09:06 OpenGeode_Geosciences-7.1.2rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1148 b- defN 23-Jul-11 09:06 OpenGeode_Geosciences-7.1.2rc1.dist-info/RECORD
+11 files, 1784337 bytes uncompressed, 545061 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
 Comment: 
 
 Filename: opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.1.2.dist-info/METADATA
+Filename: OpenGeode_Geosciences-7.1.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.1.2.dist-info/WHEEL
+Filename: OpenGeode_Geosciences-7.1.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.1.2.dist-info/top_level.txt
+Filename: OpenGeode_Geosciences-7.1.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.1.2.dist-info/RECORD
+Filename: OpenGeode_Geosciences-7.1.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180045b5c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jul 12 00:49:32 2023
+Time/Date		Tue Jul 11 09:05:42 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000047000
 SizeOfInitializedData	0000000000044c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000045b5c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00090000
 SizeOfHeaders		00000400
-CheckSum		00090707
+CheckSum		00094c0d
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -210,52 +210,52 @@
 	6aa34	 5787  OSRGetCRSInfoListFromDatabase
 	6aaea	 1291  ?DestroyCT@OGRCoordinateTransformation@@SAXPEAV1@@Z
 
  0006765c	00067b88 00000000 00000000 0006c356 000483b0
 
 	DLL Name: OpenGeode_mesh.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	6c2dc	 1843  ?set_active_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@@Z
-	6c266	 1059  ?delete_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@@Z
-	6c1ac	 1795  ?register_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@$$QEAV?$shared_ptr@V?$CoordinateReferenceSystem@$01@geode@@@std@@@Z
-	6c13c	  895  ?coordinate_reference_system_exists@?$CoordinateReferenceSystemManager@$01@geode@@QEBA_NVstring_view@absl@@@Z
-	6c0c6	  785  ?active_coordinate_reference_system_name@?$CoordinateReferenceSystemManager@$01@geode@@QEBA?AVstring_view@absl@@XZ
-	6c044	  779  ?active_coordinate_reference_system@?$CoordinateReferenceSystemManager@$01@geode@@QEBAAEBV?$CoordinateReferenceSystem@$01@2@XZ
-	6bfb2	 1421  ?find_coordinate_reference_system@?$CoordinateReferenceSystemManager@$01@geode@@QEBAAEBV?$CoordinateReferenceSystem@$01@2@Vstring_view@absl@@@Z
-	6bf38	 1844  ?set_active_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@@Z
-	6bec2	 1060  ?delete_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@@Z
-	6be08	 1796  ?register_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@$$QEAV?$shared_ptr@V?$CoordinateReferenceSystem@$02@geode@@@std@@@Z
-	6bd98	  896  ?coordinate_reference_system_exists@?$CoordinateReferenceSystemManager@$02@geode@@QEBA_NVstring_view@absl@@@Z
-	6bd22	  786  ?active_coordinate_reference_system_name@?$CoordinateReferenceSystemManager@$02@geode@@QEBA?AVstring_view@absl@@XZ
-	6bca0	  780  ?active_coordinate_reference_system@?$CoordinateReferenceSystemManager@$02@geode@@QEBAAEBV?$CoordinateReferenceSystem@$02@2@XZ
-	6bc0e	 1422  ?find_coordinate_reference_system@?$CoordinateReferenceSystemManager@$02@geode@@QEBAAEBV?$CoordinateReferenceSystem@$02@2@Vstring_view@absl@@@Z
-	6bb6a	 1579  ?main_coordinate_reference_system_manager_builder@?$CoordinateReferenceSystemManagersBuilder@$02@geode@@QEAA?AV?$CoordinateReferenceSystemManagerBuilder@$02@2@XZ
-	6bac6	 1578  ?main_coordinate_reference_system_manager_builder@?$CoordinateReferenceSystemManagersBuilder@$01@geode@@QEAA?AV?$CoordinateReferenceSystemManagerBuilder@$01@2@XZ
-	6ba36	 1575  ?main_coordinate_reference_system_manager@?$CoordinateReferenceSystemManagers@$01@geode@@QEBAAEBV?$CoordinateReferenceSystemManager@$01@2@XZ
-	6abce	  211  ??0?$AttributeCoordinateReferenceSystem@$01@geode@@QEAA@AEAVAttributeManager@1@Vstring_view@absl@@@Z
-	6ac36	  482  ??1?$AttributeCoordinateReferenceSystem@$01@geode@@UEAA@XZ
-	6ac74	 1705  ?point@?$AttributeCoordinateReferenceSystem@$01@geode@@UEBAAEBV?$Point@$01@2@I@Z
-	6acc8	 1867  ?set_point@?$AttributeCoordinateReferenceSystem@$01@geode@@UEAAXIV?$Point@$01@2@@Z
-	6ad1e	 1655  ?nb_points@?$AttributeCoordinateReferenceSystem@$01@geode@@QEBAIXZ
-	6ad64	  209  ??0?$AttributeCoordinateReferenceSystem@$01@geode@@IEAA@XZ
-	6ada2	  214  ??0?$AttributeCoordinateReferenceSystem@$02@geode@@QEAA@AEAVAttributeManager@1@Vstring_view@absl@@@Z
-	6ae0a	  483  ??1?$AttributeCoordinateReferenceSystem@$02@geode@@UEAA@XZ
-	6ae48	 1706  ?point@?$AttributeCoordinateReferenceSystem@$02@geode@@UEBAAEBV?$Point@$02@2@I@Z
-	6ae9c	 1868  ?set_point@?$AttributeCoordinateReferenceSystem@$02@geode@@UEAAXIV?$Point@$02@2@@Z
-	6aef2	 1656  ?nb_points@?$AttributeCoordinateReferenceSystem@$02@geode@@QEBAIXZ
-	6af38	  212  ??0?$AttributeCoordinateReferenceSystem@$02@geode@@IEAA@XZ
-	6af76	   88  ??$serialize@V?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$02@geode@@IEAAXAEAV?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
-	6b19c	  145  ??$serialize@V?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$02@geode@@IEAAXAEAV?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
-	6b3f6	   87  ??$serialize@V?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$01@geode@@IEAAXAEAV?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
-	6b61c	  144  ??$serialize@V?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$01@geode@@IEAAXAEAV?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
-	6b876	  812  ?attribute_name@?$AttributeCoordinateReferenceSystem@$02@geode@@QEBA?AVstring_view@absl@@XZ
-	6b8d4	  811  ?attribute_name@?$AttributeCoordinateReferenceSystem@$01@geode@@QEBA?AVstring_view@absl@@XZ
-	6b932	 1673  ?nb_vertices@VertexSet@geode@@QEBAIXZ
-	6b95a	 2080  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
-	6b9a6	 1577  ?main_coordinate_reference_system_manager@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$CoordinateReferenceSystemManager@$02@2@XZ
+	6c2dc	 1837  ?set_active_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@@Z
+	6c266	 1057  ?delete_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@@Z
+	6c1ac	 1789  ?register_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$01@geode@@QEAAXVstring_view@absl@@$$QEAV?$shared_ptr@V?$CoordinateReferenceSystem@$01@geode@@@std@@@Z
+	6c13c	  893  ?coordinate_reference_system_exists@?$CoordinateReferenceSystemManager@$01@geode@@QEBA_NVstring_view@absl@@@Z
+	6c0c6	  783  ?active_coordinate_reference_system_name@?$CoordinateReferenceSystemManager@$01@geode@@QEBA?AVstring_view@absl@@XZ
+	6c044	  777  ?active_coordinate_reference_system@?$CoordinateReferenceSystemManager@$01@geode@@QEBAAEBV?$CoordinateReferenceSystem@$01@2@XZ
+	6bfb2	 1419  ?find_coordinate_reference_system@?$CoordinateReferenceSystemManager@$01@geode@@QEBAAEBV?$CoordinateReferenceSystem@$01@2@Vstring_view@absl@@@Z
+	6bf38	 1838  ?set_active_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@@Z
+	6bec2	 1058  ?delete_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@@Z
+	6be08	 1790  ?register_coordinate_reference_system@?$CoordinateReferenceSystemManagerBuilder@$02@geode@@QEAAXVstring_view@absl@@$$QEAV?$shared_ptr@V?$CoordinateReferenceSystem@$02@geode@@@std@@@Z
+	6bd98	  894  ?coordinate_reference_system_exists@?$CoordinateReferenceSystemManager@$02@geode@@QEBA_NVstring_view@absl@@@Z
+	6bd22	  784  ?active_coordinate_reference_system_name@?$CoordinateReferenceSystemManager@$02@geode@@QEBA?AVstring_view@absl@@XZ
+	6bca0	  778  ?active_coordinate_reference_system@?$CoordinateReferenceSystemManager@$02@geode@@QEBAAEBV?$CoordinateReferenceSystem@$02@2@XZ
+	6bc0e	 1420  ?find_coordinate_reference_system@?$CoordinateReferenceSystemManager@$02@geode@@QEBAAEBV?$CoordinateReferenceSystem@$02@2@Vstring_view@absl@@@Z
+	6bb6a	 1573  ?main_coordinate_reference_system_manager_builder@?$CoordinateReferenceSystemManagersBuilder@$02@geode@@QEAA?AV?$CoordinateReferenceSystemManagerBuilder@$02@2@XZ
+	6bac6	 1572  ?main_coordinate_reference_system_manager_builder@?$CoordinateReferenceSystemManagersBuilder@$01@geode@@QEAA?AV?$CoordinateReferenceSystemManagerBuilder@$01@2@XZ
+	6ba36	 1569  ?main_coordinate_reference_system_manager@?$CoordinateReferenceSystemManagers@$01@geode@@QEBAAEBV?$CoordinateReferenceSystemManager@$01@2@XZ
+	6abce	  209  ??0?$AttributeCoordinateReferenceSystem@$01@geode@@QEAA@AEAVAttributeManager@1@Vstring_view@absl@@@Z
+	6ac36	  480  ??1?$AttributeCoordinateReferenceSystem@$01@geode@@UEAA@XZ
+	6ac74	 1699  ?point@?$AttributeCoordinateReferenceSystem@$01@geode@@UEBAAEBV?$Point@$01@2@I@Z
+	6acc8	 1861  ?set_point@?$AttributeCoordinateReferenceSystem@$01@geode@@UEAAXIV?$Point@$01@2@@Z
+	6ad1e	 1649  ?nb_points@?$AttributeCoordinateReferenceSystem@$01@geode@@QEBAIXZ
+	6ad64	  207  ??0?$AttributeCoordinateReferenceSystem@$01@geode@@IEAA@XZ
+	6ada2	  212  ??0?$AttributeCoordinateReferenceSystem@$02@geode@@QEAA@AEAVAttributeManager@1@Vstring_view@absl@@@Z
+	6ae0a	  481  ??1?$AttributeCoordinateReferenceSystem@$02@geode@@UEAA@XZ
+	6ae48	 1700  ?point@?$AttributeCoordinateReferenceSystem@$02@geode@@UEBAAEBV?$Point@$02@2@I@Z
+	6ae9c	 1862  ?set_point@?$AttributeCoordinateReferenceSystem@$02@geode@@UEAAXIV?$Point@$02@2@@Z
+	6aef2	 1650  ?nb_points@?$AttributeCoordinateReferenceSystem@$02@geode@@QEBAIXZ
+	6af38	  210  ??0?$AttributeCoordinateReferenceSystem@$02@geode@@IEAA@XZ
+	6af76	   86  ??$serialize@V?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$02@geode@@IEAAXAEAV?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
+	6b19c	  143  ??$serialize@V?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$02@geode@@IEAAXAEAV?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
+	6b3f6	   85  ??$serialize@V?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$01@geode@@IEAAXAEAV?$Deserializer@V?$BasicInputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
+	6b61c	  142  ??$serialize@V?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@?$AttributeCoordinateReferenceSystem@$01@geode@@IEAAXAEAV?$Serializer@V?$BasicBufferedOutputStreamAdapter@DUDefaultConfig@bitsery@@U?$char_traits@D@std@@V?$array@D$0BAA@@4@@bitsery@@V?$tuple@V?$PolymorphicContext@UStandardRTTI@ext@bitsery@@@ext@bitsery@@VPointerLinkingContext@23@VInheritanceContext@23@@std@@@bitsery@@@Z
+	6b876	  810  ?attribute_name@?$AttributeCoordinateReferenceSystem@$02@geode@@QEBA?AVstring_view@absl@@XZ
+	6b8d4	  809  ?attribute_name@?$AttributeCoordinateReferenceSystem@$01@geode@@QEBA?AVstring_view@absl@@XZ
+	6b932	 1667  ?nb_vertices@VertexSet@geode@@QEBAIXZ
+	6b95a	 2074  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
+	6b9a6	 1571  ?main_coordinate_reference_system_manager@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$CoordinateReferenceSystemManager@$02@2@XZ
 
  00067670	00067a60 00000000 00000000 0006cc6e 00048288
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	6cc0a	  110  ?directory@ZipFile@geode@@QEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
 	6cbee	   60  ??1ZipFile@geode@@QEAA@XZ
@@ -15237,74 +15237,74 @@
 	  12360: 30 30 50 45 41 48 40 5a 00 00 cc 09 3f 4f 47 52
 	  12370: 43 72 65 61 74 65 43 6f 6f 72 64 69 6e 61 74 65
 	  12380: 54 72 61 6e 73 66 6f 72 6d 61 74 69 6f 6e 40 40
 	  12390: 59 41 50 45 41 56 4f 47 52 43 6f 6f 72 64 69 6e
 	  123a0: 61 74 65 54 72 61 6e 73 66 6f 72 6d 61 74 69 6f
 	  123b0: 6e 40 40 50 45 42 56 4f 47 52 53 70 61 74 69 61
 	  123c0: 6c 52 65 66 65 72 65 6e 63 65 40 40 30 40 5a 00
-	  123d0: 67 64 61 6c 2e 64 6c 6c 00 00 d3 00 3f 3f 30 3f
+	  123d0: 67 64 61 6c 2e 64 6c 6c 00 00 d1 00 3f 3f 30 3f
 	  123e0: 24 41 74 74 72 69 62 75 74 65 43 6f 6f 72 64 69
 	  123f0: 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73
 	  12400: 74 65 6d 40 24 30 31 40 67 65 6f 64 65 40 40 51
 	  12410: 45 41 41 40 41 45 41 56 41 74 74 72 69 62 75 74
 	  12420: 65 4d 61 6e 61 67 65 72 40 31 40 56 73 74 72 69
 	  12430: 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a
-	  12440: 00 00 e2 01 3f 3f 31 3f 24 41 74 74 72 69 62 75
+	  12440: 00 00 e0 01 3f 3f 31 3f 24 41 74 74 72 69 62 75
 	  12450: 74 65 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65
 	  12460: 72 65 6e 63 65 53 79 73 74 65 6d 40 24 30 31 40
 	  12470: 67 65 6f 64 65 40 40 55 45 41 41 40 58 5a 00 00
-	  12480: a9 06 3f 70 6f 69 6e 74 40 3f 24 41 74 74 72 69
+	  12480: a3 06 3f 70 6f 69 6e 74 40 3f 24 41 74 74 72 69
 	  12490: 62 75 74 65 43 6f 6f 72 64 69 6e 61 74 65 52 65
 	  124a0: 66 65 72 65 6e 63 65 53 79 73 74 65 6d 40 24 30
 	  124b0: 31 40 67 65 6f 64 65 40 40 55 45 42 41 41 45 42
 	  124c0: 56 3f 24 50 6f 69 6e 74 40 24 30 31 40 32 40 49
-	  124d0: 40 5a 00 00 4b 07 3f 73 65 74 5f 70 6f 69 6e 74
+	  124d0: 40 5a 00 00 45 07 3f 73 65 74 5f 70 6f 69 6e 74
 	  124e0: 40 3f 24 41 74 74 72 69 62 75 74 65 43 6f 6f 72
 	  124f0: 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53
 	  12500: 79 73 74 65 6d 40 24 30 31 40 67 65 6f 64 65 40
 	  12510: 40 55 45 41 41 58 49 56 3f 24 50 6f 69 6e 74 40
-	  12520: 24 30 31 40 32 40 40 5a 00 00 77 06 3f 6e 62 5f
+	  12520: 24 30 31 40 32 40 40 5a 00 00 71 06 3f 6e 62 5f
 	  12530: 70 6f 69 6e 74 73 40 3f 24 41 74 74 72 69 62 75
 	  12540: 74 65 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65
 	  12550: 72 65 6e 63 65 53 79 73 74 65 6d 40 24 30 31 40
 	  12560: 67 65 6f 64 65 40 40 51 45 42 41 49 58 5a 00 00
-	  12570: d1 00 3f 3f 30 3f 24 41 74 74 72 69 62 75 74 65
+	  12570: cf 00 3f 3f 30 3f 24 41 74 74 72 69 62 75 74 65
 	  12580: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  12590: 6e 63 65 53 79 73 74 65 6d 40 24 30 31 40 67 65
-	  125a0: 6f 64 65 40 40 49 45 41 41 40 58 5a 00 00 d6 00
+	  125a0: 6f 64 65 40 40 49 45 41 41 40 58 5a 00 00 d4 00
 	  125b0: 3f 3f 30 3f 24 41 74 74 72 69 62 75 74 65 43 6f
 	  125c0: 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63
 	  125d0: 65 53 79 73 74 65 6d 40 24 30 32 40 67 65 6f 64
 	  125e0: 65 40 40 51 45 41 41 40 41 45 41 56 41 74 74 72
 	  125f0: 69 62 75 74 65 4d 61 6e 61 67 65 72 40 31 40 56
 	  12600: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  12610: 40 40 40 5a 00 00 e3 01 3f 3f 31 3f 24 41 74 74
+	  12610: 40 40 40 5a 00 00 e1 01 3f 3f 31 3f 24 41 74 74
 	  12620: 72 69 62 75 74 65 43 6f 6f 72 64 69 6e 61 74 65
 	  12630: 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 40
 	  12640: 24 30 32 40 67 65 6f 64 65 40 40 55 45 41 41 40
-	  12650: 58 5a 00 00 aa 06 3f 70 6f 69 6e 74 40 3f 24 41
+	  12650: 58 5a 00 00 a4 06 3f 70 6f 69 6e 74 40 3f 24 41
 	  12660: 74 74 72 69 62 75 74 65 43 6f 6f 72 64 69 6e 61
 	  12670: 74 65 52 65 66 65 72 65 6e 63 65 53 79 73 74 65
 	  12680: 6d 40 24 30 32 40 67 65 6f 64 65 40 40 55 45 42
 	  12690: 41 41 45 42 56 3f 24 50 6f 69 6e 74 40 24 30 32
-	  126a0: 40 32 40 49 40 5a 00 00 4c 07 3f 73 65 74 5f 70
+	  126a0: 40 32 40 49 40 5a 00 00 46 07 3f 73 65 74 5f 70
 	  126b0: 6f 69 6e 74 40 3f 24 41 74 74 72 69 62 75 74 65
 	  126c0: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  126d0: 6e 63 65 53 79 73 74 65 6d 40 24 30 32 40 67 65
 	  126e0: 6f 64 65 40 40 55 45 41 41 58 49 56 3f 24 50 6f
-	  126f0: 69 6e 74 40 24 30 32 40 32 40 40 5a 00 00 78 06
+	  126f0: 69 6e 74 40 24 30 32 40 32 40 40 5a 00 00 72 06
 	  12700: 3f 6e 62 5f 70 6f 69 6e 74 73 40 3f 24 41 74 74
 	  12710: 72 69 62 75 74 65 43 6f 6f 72 64 69 6e 61 74 65
 	  12720: 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 40
 	  12730: 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 49
-	  12740: 58 5a 00 00 d4 00 3f 3f 30 3f 24 41 74 74 72 69
+	  12740: 58 5a 00 00 d2 00 3f 3f 30 3f 24 41 74 74 72 69
 	  12750: 62 75 74 65 43 6f 6f 72 64 69 6e 61 74 65 52 65
 	  12760: 66 65 72 65 6e 63 65 53 79 73 74 65 6d 40 24 30
 	  12770: 32 40 67 65 6f 64 65 40 40 49 45 41 41 40 58 5a
-	  12780: 00 00 58 00 3f 3f 24 73 65 72 69 61 6c 69 7a 65
+	  12780: 00 00 56 00 3f 3f 24 73 65 72 69 61 6c 69 7a 65
 	  12790: 40 56 3f 24 44 65 73 65 72 69 61 6c 69 7a 65 72
 	  127a0: 40 56 3f 24 42 61 73 69 63 49 6e 70 75 74 53 74
 	  127b0: 72 65 61 6d 41 64 61 70 74 65 72 40 44 55 44 65
 	  127c0: 66 61 75 6c 74 43 6f 6e 66 69 67 40 62 69 74 73
 	  127d0: 65 72 79 40 40 55 3f 24 63 68 61 72 5f 74 72 61
 	  127e0: 69 74 73 40 44 40 73 74 64 40 40 40 62 69 74 73
 	  127f0: 65 72 79 40 40 56 3f 24 74 75 70 6c 65 40 56 3f
@@ -15330,15 +15330,15 @@
 	  12930: 69 63 43 6f 6e 74 65 78 74 40 55 53 74 61 6e 64
 	  12940: 61 72 64 52 54 54 49 40 65 78 74 40 62 69 74 73
 	  12950: 65 72 79 40 40 40 65 78 74 40 62 69 74 73 65 72
 	  12960: 79 40 40 56 50 6f 69 6e 74 65 72 4c 69 6e 6b 69
 	  12970: 6e 67 43 6f 6e 74 65 78 74 40 32 33 40 56 49 6e
 	  12980: 68 65 72 69 74 61 6e 63 65 43 6f 6e 74 65 78 74
 	  12990: 40 32 33 40 40 73 74 64 40 40 40 62 69 74 73 65
-	  129a0: 72 79 40 40 40 5a 00 00 91 00 3f 3f 24 73 65 72
+	  129a0: 72 79 40 40 40 5a 00 00 8f 00 3f 3f 24 73 65 72
 	  129b0: 69 61 6c 69 7a 65 40 56 3f 24 53 65 72 69 61 6c
 	  129c0: 69 7a 65 72 40 56 3f 24 42 61 73 69 63 42 75 66
 	  129d0: 66 65 72 65 64 4f 75 74 70 75 74 53 74 72 65 61
 	  129e0: 6d 41 64 61 70 74 65 72 40 44 55 44 65 66 61 75
 	  129f0: 6c 74 43 6f 6e 66 69 67 40 62 69 74 73 65 72 79
 	  12a00: 40 40 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73
 	  12a10: 40 44 40 73 74 64 40 40 56 3f 24 61 72 72 61 79
@@ -15368,15 +15368,15 @@
 	  12b90: 65 78 74 40 55 53 74 61 6e 64 61 72 64 52 54 54
 	  12ba0: 49 40 65 78 74 40 62 69 74 73 65 72 79 40 40 40
 	  12bb0: 65 78 74 40 62 69 74 73 65 72 79 40 40 56 50 6f
 	  12bc0: 69 6e 74 65 72 4c 69 6e 6b 69 6e 67 43 6f 6e 74
 	  12bd0: 65 78 74 40 32 33 40 56 49 6e 68 65 72 69 74 61
 	  12be0: 6e 63 65 43 6f 6e 74 65 78 74 40 32 33 40 40 73
 	  12bf0: 74 64 40 40 40 62 69 74 73 65 72 79 40 40 40 5a
-	  12c00: 00 00 57 00 3f 3f 24 73 65 72 69 61 6c 69 7a 65
+	  12c00: 00 00 55 00 3f 3f 24 73 65 72 69 61 6c 69 7a 65
 	  12c10: 40 56 3f 24 44 65 73 65 72 69 61 6c 69 7a 65 72
 	  12c20: 40 56 3f 24 42 61 73 69 63 49 6e 70 75 74 53 74
 	  12c30: 72 65 61 6d 41 64 61 70 74 65 72 40 44 55 44 65
 	  12c40: 66 61 75 6c 74 43 6f 6e 66 69 67 40 62 69 74 73
 	  12c50: 65 72 79 40 40 55 3f 24 63 68 61 72 5f 74 72 61
 	  12c60: 69 74 73 40 44 40 73 74 64 40 40 40 62 69 74 73
 	  12c70: 65 72 79 40 40 56 3f 24 74 75 70 6c 65 40 56 3f
@@ -15402,15 +15402,15 @@
 	  12db0: 69 63 43 6f 6e 74 65 78 74 40 55 53 74 61 6e 64
 	  12dc0: 61 72 64 52 54 54 49 40 65 78 74 40 62 69 74 73
 	  12dd0: 65 72 79 40 40 40 65 78 74 40 62 69 74 73 65 72
 	  12de0: 79 40 40 56 50 6f 69 6e 74 65 72 4c 69 6e 6b 69
 	  12df0: 6e 67 43 6f 6e 74 65 78 74 40 32 33 40 56 49 6e
 	  12e00: 68 65 72 69 74 61 6e 63 65 43 6f 6e 74 65 78 74
 	  12e10: 40 32 33 40 40 73 74 64 40 40 40 62 69 74 73 65
-	  12e20: 72 79 40 40 40 5a 00 00 90 00 3f 3f 24 73 65 72
+	  12e20: 72 79 40 40 40 5a 00 00 8e 00 3f 3f 24 73 65 72
 	  12e30: 69 61 6c 69 7a 65 40 56 3f 24 53 65 72 69 61 6c
 	  12e40: 69 7a 65 72 40 56 3f 24 42 61 73 69 63 42 75 66
 	  12e50: 66 65 72 65 64 4f 75 74 70 75 74 53 74 72 65 61
 	  12e60: 6d 41 64 61 70 74 65 72 40 44 55 44 65 66 61 75
 	  12e70: 6c 74 43 6f 6e 66 69 67 40 62 69 74 73 65 72 79
 	  12e80: 40 40 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73
 	  12e90: 40 44 40 73 74 64 40 40 56 3f 24 61 72 72 61 79
@@ -15440,181 +15440,181 @@
 	  13010: 65 78 74 40 55 53 74 61 6e 64 61 72 64 52 54 54
 	  13020: 49 40 65 78 74 40 62 69 74 73 65 72 79 40 40 40
 	  13030: 65 78 74 40 62 69 74 73 65 72 79 40 40 56 50 6f
 	  13040: 69 6e 74 65 72 4c 69 6e 6b 69 6e 67 43 6f 6e 74
 	  13050: 65 78 74 40 32 33 40 56 49 6e 68 65 72 69 74 61
 	  13060: 6e 63 65 43 6f 6e 74 65 78 74 40 32 33 40 40 73
 	  13070: 74 64 40 40 40 62 69 74 73 65 72 79 40 40 40 5a
-	  13080: 00 00 2c 03 3f 61 74 74 72 69 62 75 74 65 5f 6e
+	  13080: 00 00 2a 03 3f 61 74 74 72 69 62 75 74 65 5f 6e
 	  13090: 61 6d 65 40 3f 24 41 74 74 72 69 62 75 74 65 43
 	  130a0: 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e
 	  130b0: 63 65 53 79 73 74 65 6d 40 24 30 32 40 67 65 6f
 	  130c0: 64 65 40 40 51 45 42 41 3f 41 56 73 74 72 69 6e
 	  130d0: 67 5f 76 69 65 77 40 61 62 73 6c 40 40 58 5a 00
-	  130e0: 2b 03 3f 61 74 74 72 69 62 75 74 65 5f 6e 61 6d
+	  130e0: 29 03 3f 61 74 74 72 69 62 75 74 65 5f 6e 61 6d
 	  130f0: 65 40 3f 24 41 74 74 72 69 62 75 74 65 43 6f 6f
 	  13100: 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65
 	  13110: 53 79 73 74 65 6d 40 24 30 31 40 67 65 6f 64 65
 	  13120: 40 40 51 45 42 41 3f 41 56 73 74 72 69 6e 67 5f
-	  13130: 76 69 65 77 40 61 62 73 6c 40 40 58 5a 00 89 06
+	  13130: 76 69 65 77 40 61 62 73 6c 40 40 58 5a 00 83 06
 	  13140: 3f 6e 62 5f 76 65 72 74 69 63 65 73 40 56 65 72
 	  13150: 74 65 78 53 65 74 40 67 65 6f 64 65 40 40 51 45
-	  13160: 42 41 49 58 5a 00 20 08 3f 76 65 72 74 65 78 5f
+	  13160: 42 41 49 58 5a 00 1a 08 3f 76 65 72 74 65 78 5f
 	  13170: 61 74 74 72 69 62 75 74 65 5f 6d 61 6e 61 67 65
 	  13180: 72 40 56 65 72 74 65 78 53 65 74 40 67 65 6f 64
 	  13190: 65 40 40 51 45 42 41 41 45 41 56 41 74 74 72 69
 	  131a0: 62 75 74 65 4d 61 6e 61 67 65 72 40 32 40 58 5a
-	  131b0: 00 00 29 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
+	  131b0: 00 00 23 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
 	  131c0: 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73
 	  131d0: 79 73 74 65 6d 5f 6d 61 6e 61 67 65 72 40 3f 24
 	  131e0: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  131f0: 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72
 	  13200: 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  13210: 41 41 45 42 56 3f 24 43 6f 6f 72 64 69 6e 61 74
 	  13220: 65 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d
 	  13230: 4d 61 6e 61 67 65 72 40 24 30 32 40 32 40 58 5a
-	  13240: 00 00 27 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
+	  13240: 00 00 21 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
 	  13250: 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73
 	  13260: 79 73 74 65 6d 5f 6d 61 6e 61 67 65 72 40 3f 24
 	  13270: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  13280: 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72
 	  13290: 73 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42
 	  132a0: 41 41 45 42 56 3f 24 43 6f 6f 72 64 69 6e 61 74
 	  132b0: 65 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d
 	  132c0: 4d 61 6e 61 67 65 72 40 24 30 31 40 32 40 58 5a
-	  132d0: 00 00 2a 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
+	  132d0: 00 00 24 06 3f 6d 61 69 6e 5f 63 6f 6f 72 64 69
 	  132e0: 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73
 	  132f0: 79 73 74 65 6d 5f 6d 61 6e 61 67 65 72 5f 62 75
 	  13300: 69 6c 64 65 72 40 3f 24 43 6f 6f 72 64 69 6e 61
 	  13310: 74 65 52 65 66 65 72 65 6e 63 65 53 79 73 74 65
 	  13320: 6d 4d 61 6e 61 67 65 72 73 42 75 69 6c 64 65 72
 	  13330: 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 41 41
 	  13340: 3f 41 56 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52
 	  13350: 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d 61
 	  13360: 6e 61 67 65 72 42 75 69 6c 64 65 72 40 24 30 31
-	  13370: 40 32 40 58 5a 00 2b 06 3f 6d 61 69 6e 5f 63 6f
+	  13370: 40 32 40 58 5a 00 25 06 3f 6d 61 69 6e 5f 63 6f
 	  13380: 6f 72 64 69 6e 61 74 65 5f 72 65 66 65 72 65 6e
 	  13390: 63 65 5f 73 79 73 74 65 6d 5f 6d 61 6e 61 67 65
 	  133a0: 72 5f 62 75 69 6c 64 65 72 40 3f 24 43 6f 6f 72
 	  133b0: 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53
 	  133c0: 79 73 74 65 6d 4d 61 6e 61 67 65 72 73 42 75 69
 	  133d0: 6c 64 65 72 40 24 30 32 40 67 65 6f 64 65 40 40
 	  133e0: 51 45 41 41 3f 41 56 3f 24 43 6f 6f 72 64 69 6e
 	  133f0: 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73 74
 	  13400: 65 6d 4d 61 6e 61 67 65 72 42 75 69 6c 64 65 72
-	  13410: 40 24 30 32 40 32 40 58 5a 00 8e 05 3f 66 69 6e
+	  13410: 40 24 30 32 40 32 40 58 5a 00 8c 05 3f 66 69 6e
 	  13420: 64 5f 63 6f 6f 72 64 69 6e 61 74 65 5f 72 65 66
 	  13430: 65 72 65 6e 63 65 5f 73 79 73 74 65 6d 40 3f 24
 	  13440: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  13450: 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72
 	  13460: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41
 	  13470: 41 45 42 56 3f 24 43 6f 6f 72 64 69 6e 61 74 65
 	  13480: 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 40
 	  13490: 24 30 32 40 32 40 56 73 74 72 69 6e 67 5f 76 69
-	  134a0: 65 77 40 61 62 73 6c 40 40 40 5a 00 0c 03 3f 61
+	  134a0: 65 77 40 61 62 73 6c 40 40 40 5a 00 0a 03 3f 61
 	  134b0: 63 74 69 76 65 5f 63 6f 6f 72 64 69 6e 61 74 65
 	  134c0: 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73 74 65
 	  134d0: 6d 40 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52 65
 	  134e0: 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d 61 6e
 	  134f0: 61 67 65 72 40 24 30 32 40 67 65 6f 64 65 40 40
 	  13500: 51 45 42 41 41 45 42 56 3f 24 43 6f 6f 72 64 69
 	  13510: 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73
-	  13520: 74 65 6d 40 24 30 32 40 32 40 58 5a 00 00 12 03
+	  13520: 74 65 6d 40 24 30 32 40 32 40 58 5a 00 00 10 03
 	  13530: 3f 61 63 74 69 76 65 5f 63 6f 6f 72 64 69 6e 61
 	  13540: 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73
 	  13550: 74 65 6d 5f 6e 61 6d 65 40 3f 24 43 6f 6f 72 64
 	  13560: 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79
 	  13570: 73 74 65 6d 4d 61 6e 61 67 65 72 40 24 30 32 40
 	  13580: 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56 73 74
 	  13590: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
-	  135a0: 58 5a 00 00 80 03 3f 63 6f 6f 72 64 69 6e 61 74
+	  135a0: 58 5a 00 00 7e 03 3f 63 6f 6f 72 64 69 6e 61 74
 	  135b0: 65 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73 74
 	  135c0: 65 6d 5f 65 78 69 73 74 73 40 3f 24 43 6f 6f 72
 	  135d0: 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53
 	  135e0: 79 73 74 65 6d 4d 61 6e 61 67 65 72 40 24 30 32
 	  135f0: 40 67 65 6f 64 65 40 40 51 45 42 41 5f 4e 56 73
 	  13600: 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40
-	  13610: 40 40 5a 00 04 07 3f 72 65 67 69 73 74 65 72 5f
+	  13610: 40 40 5a 00 fe 06 3f 72 65 67 69 73 74 65 72 5f
 	  13620: 63 6f 6f 72 64 69 6e 61 74 65 5f 72 65 66 65 72
 	  13630: 65 6e 63 65 5f 73 79 73 74 65 6d 40 3f 24 43 6f
 	  13640: 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63
 	  13650: 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72 42 75
 	  13660: 69 6c 64 65 72 40 24 30 32 40 67 65 6f 64 65 40
 	  13670: 40 51 45 41 41 58 56 73 74 72 69 6e 67 5f 76 69
 	  13680: 65 77 40 61 62 73 6c 40 40 24 24 51 45 41 56 3f
 	  13690: 24 73 68 61 72 65 64 5f 70 74 72 40 56 3f 24 43
 	  136a0: 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e
 	  136b0: 63 65 53 79 73 74 65 6d 40 24 30 32 40 67 65 6f
-	  136c0: 64 65 40 40 40 73 74 64 40 40 40 5a 00 00 24 04
+	  136c0: 64 65 40 40 40 73 74 64 40 40 40 5a 00 00 22 04
 	  136d0: 3f 64 65 6c 65 74 65 5f 63 6f 6f 72 64 69 6e 61
 	  136e0: 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73
 	  136f0: 74 65 6d 40 3f 24 43 6f 6f 72 64 69 6e 61 74 65
 	  13700: 52 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d
 	  13710: 61 6e 61 67 65 72 42 75 69 6c 64 65 72 40 24 30
 	  13720: 32 40 67 65 6f 64 65 40 40 51 45 41 41 58 56 73
 	  13730: 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40
-	  13740: 40 40 5a 00 34 07 3f 73 65 74 5f 61 63 74 69 76
+	  13740: 40 40 5a 00 2e 07 3f 73 65 74 5f 61 63 74 69 76
 	  13750: 65 5f 63 6f 6f 72 64 69 6e 61 74 65 5f 72 65 66
 	  13760: 65 72 65 6e 63 65 5f 73 79 73 74 65 6d 40 3f 24
 	  13770: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  13780: 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72
 	  13790: 42 75 69 6c 64 65 72 40 24 30 32 40 67 65 6f 64
 	  137a0: 65 40 40 51 45 41 41 58 56 73 74 72 69 6e 67 5f
-	  137b0: 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 8d 05
+	  137b0: 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 8b 05
 	  137c0: 3f 66 69 6e 64 5f 63 6f 6f 72 64 69 6e 61 74 65
 	  137d0: 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73 74 65
 	  137e0: 6d 40 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52 65
 	  137f0: 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d 61 6e
 	  13800: 61 67 65 72 40 24 30 31 40 67 65 6f 64 65 40 40
 	  13810: 51 45 42 41 41 45 42 56 3f 24 43 6f 6f 72 64 69
 	  13820: 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73
 	  13830: 74 65 6d 40 24 30 31 40 32 40 56 73 74 72 69 6e
 	  13840: 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00
-	  13850: 0b 03 3f 61 63 74 69 76 65 5f 63 6f 6f 72 64 69
+	  13850: 09 03 3f 61 63 74 69 76 65 5f 63 6f 6f 72 64 69
 	  13860: 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65 5f 73
 	  13870: 79 73 74 65 6d 40 3f 24 43 6f 6f 72 64 69 6e 61
 	  13880: 74 65 52 65 66 65 72 65 6e 63 65 53 79 73 74 65
 	  13890: 6d 4d 61 6e 61 67 65 72 40 24 30 31 40 67 65 6f
 	  138a0: 64 65 40 40 51 45 42 41 41 45 42 56 3f 24 43 6f
 	  138b0: 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63
 	  138c0: 65 53 79 73 74 65 6d 40 24 30 31 40 32 40 58 5a
-	  138d0: 00 00 11 03 3f 61 63 74 69 76 65 5f 63 6f 6f 72
+	  138d0: 00 00 0f 03 3f 61 63 74 69 76 65 5f 63 6f 6f 72
 	  138e0: 64 69 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65
 	  138f0: 5f 73 79 73 74 65 6d 5f 6e 61 6d 65 40 3f 24 43
 	  13900: 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e
 	  13910: 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72 40
 	  13920: 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 3f
 	  13930: 41 56 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62
-	  13940: 73 6c 40 40 58 5a 00 00 7f 03 3f 63 6f 6f 72 64
+	  13940: 73 6c 40 40 58 5a 00 00 7d 03 3f 63 6f 6f 72 64
 	  13950: 69 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65 5f
 	  13960: 73 79 73 74 65 6d 5f 65 78 69 73 74 73 40 3f 24
 	  13970: 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65
 	  13980: 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72
 	  13990: 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41
 	  139a0: 5f 4e 56 73 74 72 69 6e 67 5f 76 69 65 77 40 61
-	  139b0: 62 73 6c 40 40 40 5a 00 03 07 3f 72 65 67 69 73
+	  139b0: 62 73 6c 40 40 40 5a 00 fd 06 3f 72 65 67 69 73
 	  139c0: 74 65 72 5f 63 6f 6f 72 64 69 6e 61 74 65 5f 72
 	  139d0: 65 66 65 72 65 6e 63 65 5f 73 79 73 74 65 6d 40
 	  139e0: 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52 65 66 65
 	  139f0: 72 65 6e 63 65 53 79 73 74 65 6d 4d 61 6e 61 67
 	  13a00: 65 72 42 75 69 6c 64 65 72 40 24 30 31 40 67 65
 	  13a10: 6f 64 65 40 40 51 45 41 41 58 56 73 74 72 69 6e
 	  13a20: 67 5f 76 69 65 77 40 61 62 73 6c 40 40 24 24 51
 	  13a30: 45 41 56 3f 24 73 68 61 72 65 64 5f 70 74 72 40
 	  13a40: 56 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52 65 66
 	  13a50: 65 72 65 6e 63 65 53 79 73 74 65 6d 40 24 30 31
 	  13a60: 40 67 65 6f 64 65 40 40 40 73 74 64 40 40 40 5a
-	  13a70: 00 00 23 04 3f 64 65 6c 65 74 65 5f 63 6f 6f 72
+	  13a70: 00 00 21 04 3f 64 65 6c 65 74 65 5f 63 6f 6f 72
 	  13a80: 64 69 6e 61 74 65 5f 72 65 66 65 72 65 6e 63 65
 	  13a90: 5f 73 79 73 74 65 6d 40 3f 24 43 6f 6f 72 64 69
 	  13aa0: 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73
 	  13ab0: 74 65 6d 4d 61 6e 61 67 65 72 42 75 69 6c 64 65
 	  13ac0: 72 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 41
 	  13ad0: 41 58 56 73 74 72 69 6e 67 5f 76 69 65 77 40 61
-	  13ae0: 62 73 6c 40 40 40 5a 00 33 07 3f 73 65 74 5f 61
+	  13ae0: 62 73 6c 40 40 40 5a 00 2d 07 3f 73 65 74 5f 61
 	  13af0: 63 74 69 76 65 5f 63 6f 6f 72 64 69 6e 61 74 65
 	  13b00: 5f 72 65 66 65 72 65 6e 63 65 5f 73 79 73 74 65
 	  13b10: 6d 40 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52 65
 	  13b20: 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d 61 6e
 	  13b30: 61 67 65 72 42 75 69 6c 64 65 72 40 24 30 31 40
 	  13b40: 67 65 6f 64 65 40 40 51 45 41 41 58 56 73 74 72
 	  13b50: 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40
@@ -104342,15 +104342,17 @@
    18004ba66:	insb   (%dx),%es:(%rdi)
    18004ba67:	outsl  %ds:(%rsi),(%dx)
    18004ba68:	movsxd 0x74(%rcx),%esp
    18004ba6b:	imul   $0x8b000000,0x6e(%rdi),%ebp
    18004ba72:	or     %al,0x1(%rax)
    18004ba78:	movabs 0x180088b,%al
    18004ba81:	add    %al,(%rax)
-   18004ba83:	add    %bl,0x64ad(%rax,%rdi,8)
+   18004ba83:	add    %ah,0x1b(%rsi)
+   18004ba86:	lods   %ds:(%rsi),%eax
+   18004ba87:	add    %al,%fs:(%rax)
    18004ba8a:	add    %al,(%rax)
    18004ba8c:	or     $0x3c000000,%eax
    18004ba91:	add    (%rax),%eax
    18004ba93:	add    %bl,0x3d(%rax)
    18004ba96:	add    $0x5315800,%eax
    18004ba9b:	add    %al,(%rax)
    18004ba9d:	add    %al,(%rax)
@@ -155675,15 +155677,15 @@
    18006abbf:	rex xor %al,0x5a(%rax)
    18006abc3:	add    %ah,0x64(%rdi)
    18006abc6:	(bad)
    18006abc7:	insb   (%dx),%es:(%rdi)
    18006abc8:	cs fs insb (%dx),%es:(%rdi)
    18006abcb:	insb   (%dx),%es:(%rdi)
    18006abcc:	add    %al,(%rax)
-   18006abce:	roll   %cl,(%rax)
+   18006abce:	roll   (%rax)
    18006abd0:	(bad)
    18006abd1:	(bad)
    18006abd2:	xor    %bh,(%rdi)
    18006abd4:	and    $0x41,%al
    18006abd6:	je     0x18006ac4c
    18006abd8:	jb     0x18006ac43
    18006abda:	(bad)
@@ -155723,15 +155725,15 @@
    18006ac25:	addr32 pop %rdi
    18006ac27:	jbe    0x18006ac92
    18006ac29:	gs ja  0x18006ac6c
    18006ac2c:	(bad)
    18006ac2d:	(bad)
    18006ac32:	rex pop %rdx
    18006ac34:	add    %al,(%rax)
-   18006ac36:	loop   0x18006ac39
+   18006ac36:	loopne 0x18006ac39
    18006ac38:	(bad)
    18006ac39:	(bad)
    18006ac3a:	xor    %edi,(%rdi)
    18006ac3c:	and    $0x41,%al
    18006ac3e:	je     0x18006acb4
    18006ac40:	jb     0x18006acab
    18006ac42:	(bad)
@@ -155752,16 +155754,17 @@
    18006ac6a:	rex push %rbp
    18006ac6c:	rex.RB
    18006ac6d:	rex.B
    18006ac6e:	rex.B
    18006ac6f:	rex pop %rax
    18006ac71:	pop    %rdx
    18006ac72:	add    %al,(%rax)
-   18006ac74:	test   $0x6f703f06,%eax
-   18006ac79:	imul   $0x41243f40,0x74(%rsi),%ebp
+   18006ac74:	movabs %eax,0x40746e696f703f06
+   18006ac7d:	(bad)
+   18006ac7e:	and    $0x41,%al
    18006ac80:	je     0x18006acf6
    18006ac82:	jb     0x18006aced
    18006ac84:	(bad)
    18006ac89:	outsl  %ds:(%rsi),(%dx)
    18006ac8a:	outsl  %ds:(%rsi),(%dx)
    18006ac8b:	jb     0x18006acf1
    18006ac8d:	imul   $0x65526574,0x61(%rsi),%ebp
@@ -155785,15 +155788,15 @@
    18006acb5:	(bad)
    18006acb6:	and    $0x50,%al
    18006acb8:	outsl  %ds:(%rsi),(%dx)
    18006acb9:	imul   $0x31302440,0x74(%rsi),%ebp
    18006acc0:	rex xor 0x49(%rax),%al
    18006acc4:	rex pop %rdx
    18006acc6:	add    %al,(%rax)
-   18006acc8:	rex.WXB (bad)
+   18006acc8:	rex.RB (bad)
    18006acca:	(bad)
    18006accb:	jae    0x18006ad32
    18006accd:	je     0x18006ad2e
    18006accf:	jo     0x18006ad40
    18006acd1:	imul   $0x41243f40,0x74(%rsi),%ebp
    18006acd8:	je     0x18006ad4e
    18006acda:	jb     0x18006ad45
@@ -155820,15 +155823,15 @@
    18006ad0c:	(bad)
    18006ad0d:	and    $0x50,%al
    18006ad0f:	outsl  %ds:(%rsi),(%dx)
    18006ad10:	imul   $0x31302440,0x74(%rsi),%ebp
    18006ad17:	rex xor 0x40(%rax),%al
    18006ad1b:	pop    %rdx
    18006ad1c:	add    %al,(%rax)
-   18006ad1e:	ja     0x18006ad26
+   18006ad1e:	jno    0x18006ad26
    18006ad20:	(bad)
    18006ad21:	outsb  %ds:(%rsi),(%dx)
    18006ad22:	(bad)
    18006ad23:	pop    %rdi
    18006ad24:	jo     0x18006ad95
    18006ad26:	imul   $0x243f4073,0x74(%rsi),%ebp
    18006ad2d:	rex.B je 0x18006ada4
@@ -155851,16 +155854,16 @@
    18006ad5a:	rex push %rcx
    18006ad5c:	rex.RB
    18006ad5d:	rex.X
    18006ad5e:	rex.B
    18006ad5f:	rex.WB pop %r8
    18006ad61:	pop    %rdx
    18006ad62:	add    %al,(%rax)
-   18006ad64:	roll   (%rax)
-   18006ad66:	(bad)
+   18006ad64:	iret
+   18006ad65:	add    %bh,(%rdi)
    18006ad67:	(bad)
    18006ad68:	xor    %bh,(%rdi)
    18006ad6a:	and    $0x41,%al
    18006ad6c:	je     0x18006ade2
    18006ad6e:	jb     0x18006add9
    18006ad70:	(bad)
    18006ad75:	outsl  %ds:(%rsi),(%dx)
@@ -155929,15 +155932,15 @@
    18006adf9:	addr32 pop %rdi
    18006adfb:	jbe    0x18006ae66
    18006adfd:	gs ja  0x18006ae40
    18006ae00:	(bad)
    18006ae01:	(bad)
    18006ae06:	rex pop %rdx
    18006ae08:	add    %al,(%rax)
-   18006ae0a:	jrcxz  0x18006ae0d
+   18006ae0a:	loope  0x18006ae0d
    18006ae0c:	(bad)
    18006ae0d:	(bad)
    18006ae0e:	xor    %edi,(%rdi)
    18006ae10:	and    $0x41,%al
    18006ae12:	je     0x18006ae88
    18006ae14:	jb     0x18006ae7f
    18006ae16:	(bad)
@@ -155958,15 +155961,15 @@
    18006ae3e:	rex push %rbp
    18006ae40:	rex.RB
    18006ae41:	rex.B
    18006ae42:	rex.B
    18006ae43:	rex pop %rax
    18006ae45:	pop    %rdx
    18006ae46:	add    %al,(%rax)
-   18006ae48:	stos   %al,%es:(%rdi)
+   18006ae48:	movsb  %ds:(%rsi),%es:(%rdi)
    18006ae49:	(bad)
    18006ae4a:	(bad)
    18006ae4b:	jo     0x18006aebc
    18006ae4d:	imul   $0x41243f40,0x74(%rsi),%ebp
    18006ae54:	je     0x18006aeca
    18006ae56:	jb     0x18006aec1
    18006ae58:	(bad)
@@ -155994,15 +155997,15 @@
    18006ae89:	(bad)
    18006ae8a:	and    $0x50,%al
    18006ae8c:	outsl  %ds:(%rsi),(%dx)
    18006ae8d:	imul   $0x32302440,0x74(%rsi),%ebp
    18006ae94:	rex xor 0x49(%rax),%al
    18006ae98:	rex pop %rdx
    18006ae9a:	add    %al,(%rax)
-   18006ae9c:	rex.WR (bad)
+   18006ae9c:	rex.RX (bad)
    18006ae9e:	(bad)
    18006ae9f:	jae    0x18006af06
    18006aea1:	je     0x18006af02
    18006aea3:	jo     0x18006af14
    18006aea5:	imul   $0x41243f40,0x74(%rsi),%ebp
    18006aeac:	je     0x18006af22
    18006aeae:	jb     0x18006af19
@@ -156029,15 +156032,15 @@
    18006aee0:	(bad)
    18006aee1:	and    $0x50,%al
    18006aee3:	outsl  %ds:(%rsi),(%dx)
    18006aee4:	imul   $0x32302440,0x74(%rsi),%ebp
    18006aeeb:	rex xor 0x40(%rax),%al
    18006aeef:	pop    %rdx
    18006aef0:	add    %al,(%rax)
-   18006aef2:	js     0x18006aefa
+   18006aef2:	jb     0x18006aefa
    18006aef4:	(bad)
    18006aef5:	outsb  %ds:(%rsi),(%dx)
    18006aef6:	(bad)
    18006aef7:	pop    %rdi
    18006aef8:	jo     0x18006af69
    18006aefa:	imul   $0x243f4073,0x74(%rsi),%ebp
    18006af01:	rex.B je 0x18006af78
@@ -156060,16 +156063,16 @@
    18006af2e:	rex push %rcx
    18006af30:	rex.RB
    18006af31:	rex.X
    18006af32:	rex.B
    18006af33:	rex.WB pop %r8
    18006af35:	pop    %rdx
    18006af36:	add    %al,(%rax)
-   18006af38:	(bad)
-   18006af39:	add    %bh,(%rdi)
+   18006af38:	rolb   %cl,(%rax)
+   18006af3a:	(bad)
    18006af3b:	(bad)
    18006af3c:	xor    %bh,(%rdi)
    18006af3e:	and    $0x41,%al
    18006af40:	je     0x18006afb6
    18006af42:	jb     0x18006afad
    18006af44:	(bad)
    18006af49:	outsl  %ds:(%rsi),(%dx)
@@ -156090,15 +156093,15 @@
    18006af6d:	rex.WB
    18006af6e:	rex.RB
    18006af6f:	rex.B
    18006af70:	rex.B
    18006af71:	rex pop %rax
    18006af73:	pop    %rdx
    18006af74:	add    %al,(%rax)
-   18006af76:	pop    %rax
+   18006af76:	push   %rsi
    18006af77:	add    %bh,(%rdi)
    18006af79:	(bad)
    18006af7a:	and    $0x73,%al
    18006af7c:	gs jb  0x18006afe8
    18006af7f:	(bad)
    18006af80:	insb   (%dx),%es:(%rdi)
    18006af81:	imul   $0x243f5640,0x65(%rdx),%edi
@@ -156334,16 +156337,16 @@
    18006b188:	rex jae 0x18006b1ff
    18006b18b:	fs rex
    18006b18d:	rex
    18006b18e:	rex (bad)
    18006b190:	imul   $0x40407972,0x65(%rbx,%rsi,2),%esi
    18006b198:	rex pop %rdx
    18006b19a:	add    %al,(%rax)
-   18006b19c:	xchg   %eax,%ecx
-   18006b19d:	add    %bh,(%rdi)
+   18006b19c:	pop    (%rax)
+   18006b19e:	(bad)
    18006b19f:	(bad)
    18006b1a0:	and    $0x73,%al
    18006b1a2:	gs jb  0x18006b20e
    18006b1a5:	(bad)
    18006b1a6:	insb   (%dx),%es:(%rdi)
    18006b1a7:	imul   $0x243f5640,0x65(%rdx),%edi
    18006b1ae:	push   %rbx
@@ -156602,15 +156605,15 @@
    18006b3e2:	rex jae 0x18006b459
    18006b3e5:	fs rex
    18006b3e7:	rex
    18006b3e8:	rex (bad)
    18006b3ea:	imul   $0x40407972,0x65(%rbx,%rsi,2),%esi
    18006b3f2:	rex pop %rdx
    18006b3f4:	add    %al,(%rax)
-   18006b3f6:	push   %rdi
+   18006b3f6:	push   %rbp
    18006b3f7:	add    %bh,(%rdi)
    18006b3f9:	(bad)
    18006b3fa:	and    $0x73,%al
    18006b3fc:	gs jb  0x18006b468
    18006b3ff:	(bad)
    18006b400:	insb   (%dx),%es:(%rdi)
    18006b401:	imul   $0x243f5640,0x65(%rdx),%edi
@@ -156846,16 +156849,16 @@
    18006b608:	rex jae 0x18006b67f
    18006b60b:	fs rex
    18006b60d:	rex
    18006b60e:	rex (bad)
    18006b610:	imul   $0x40407972,0x65(%rbx,%rsi,2),%esi
    18006b618:	rex pop %rdx
    18006b61a:	add    %al,(%rax)
-   18006b61c:	nop
-   18006b61d:	add    %bh,(%rdi)
+   18006b61c:	mov    (%rax),%es
+   18006b61e:	(bad)
    18006b61f:	(bad)
    18006b620:	and    $0x73,%al
    18006b622:	gs jb  0x18006b68e
    18006b625:	(bad)
    18006b626:	insb   (%dx),%es:(%rdi)
    18006b627:	imul   $0x243f5640,0x65(%rdx),%edi
    18006b62e:	push   %rbx
@@ -157114,15 +157117,15 @@
    18006b862:	rex jae 0x18006b8d9
    18006b865:	fs rex
    18006b867:	rex
    18006b868:	rex (bad)
    18006b86a:	imul   $0x40407972,0x65(%rbx,%rsi,2),%esi
    18006b872:	rex pop %rdx
    18006b874:	add    %al,(%rax)
-   18006b876:	sub    $0x3,%al
+   18006b876:	sub    (%rbx),%al
    18006b878:	(bad)
    18006b879:	(bad)
    18006b87a:	je     0x18006b8f0
    18006b87c:	jb     0x18006b8e7
    18006b87e:	(bad)
    18006b883:	outsb  %ds:(%rsi),(%dx)
    18006b884:	(bad)
@@ -157157,15 +157160,15 @@
    18006b8c4:	addr32 pop %rdi
    18006b8c6:	jbe    0x18006b931
    18006b8c8:	gs ja  0x18006b90b
    18006b8cb:	(bad)
    18006b8cc:	(bad)
    18006b8d1:	pop    %rax
    18006b8d2:	pop    %rdx
-   18006b8d3:	add    %ch,(%rbx)
+   18006b8d3:	add    %ch,(%rcx)
    18006b8d5:	add    (%rdi),%edi
    18006b8d7:	(bad)
    18006b8d8:	je     0x18006b94e
    18006b8da:	jb     0x18006b945
    18006b8dc:	(bad)
    18006b8e1:	outsb  %ds:(%rsi),(%dx)
    18006b8e2:	(bad)
@@ -157200,15 +157203,15 @@
    18006b922:	addr32 pop %rdi
    18006b924:	jbe    0x18006b98f
    18006b926:	gs ja  0x18006b969
    18006b929:	(bad)
    18006b92a:	(bad)
    18006b92f:	pop    %rax
    18006b930:	pop    %rdx
-   18006b931:	add    %cl,0x626e3f06(%rcx)
+   18006b931:	add    %al,0x626e3f06(%rbx)
    18006b937:	pop    %rdi
    18006b938:	jbe    0x18006b99f
    18006b93a:	jb     0x18006b9b0
    18006b93c:	imul   $0x65564073,0x65(%rbx),%esp
    18006b943:	jb     0x18006b9b9
    18006b945:	gs js  0x18006b99b
    18006b948:	gs je  0x18006b98b
@@ -157216,15 +157219,15 @@
    18006b94e:	fs gs rex
    18006b951:	rex push %rcx
    18006b953:	rex.RB
    18006b954:	rex.X
    18006b955:	rex.B
    18006b956:	rex.WB pop %r8
    18006b958:	pop    %rdx
-   18006b959:	add    %ah,(%rax)
+   18006b959:	add    %bl,(%rdx)
    18006b95b:	or     %bh,(%rdi)
    18006b95d:	jbe    0x18006b9c4
    18006b95f:	jb     0x18006b9d5
    18006b961:	gs js  0x18006b9c3
    18006b964:	(bad)
    18006b965:	je     0x18006b9db
    18006b967:	jb     0x18006b9d2
@@ -157253,15 +157256,15 @@
    18006b999:	(bad)
    18006b99a:	outsb  %ds:(%rsi),(%dx)
    18006b99b:	(bad)
    18006b99c:	addr32 gs jb 0x18006b9e0
    18006b9a0:	xor    0x58(%rax),%al
    18006b9a3:	pop    %rdx
    18006b9a4:	add    %al,(%rax)
-   18006b9a6:	sub    %eax,(%rsi)
+   18006b9a6:	and    (%rsi),%eax
    18006b9a8:	(bad)
    18006b9a9:	insl   (%dx),%es:(%rdi)
    18006b9aa:	(bad)
    18006b9ab:	imul   $0x726f6f63,0x5f(%rsi),%ebp
    18006b9b2:	imul   $0x725f6574,%fs:0x61(%rsi),%ebp
    18006b9ba:	gs data16 gs jb 0x18006ba24
    18006b9bf:	outsb  %ds:(%rsi),(%dx)
@@ -157319,16 +157322,15 @@
    18006ba27:	(bad)
    18006ba28:	addr32 gs jb 0x18006ba6c
    18006ba2c:	and    $0x30,%al
    18006ba2e:	xor    0x32(%rax),%al
    18006ba31:	rex pop %rax
    18006ba33:	pop    %rdx
    18006ba34:	add    %al,(%rax)
-   18006ba36:	(bad)
-   18006ba37:	(bad)
+   18006ba36:	and    %eax,(%rsi)
    18006ba38:	(bad)
    18006ba39:	insl   (%dx),%es:(%rdi)
    18006ba3a:	(bad)
    18006ba3b:	imul   $0x726f6f63,0x5f(%rsi),%ebp
    18006ba42:	imul   $0x725f6574,%fs:0x61(%rsi),%ebp
    18006ba4a:	gs data16 gs jb 0x18006bab4
    18006ba4f:	outsb  %ds:(%rsi),(%dx)
@@ -157386,15 +157388,15 @@
    18006bab7:	(bad)
    18006bab8:	addr32 gs jb 0x18006bafc
    18006babc:	and    $0x30,%al
    18006babe:	xor    %eax,0x32(%rax)
    18006bac1:	rex pop %rax
    18006bac3:	pop    %rdx
    18006bac4:	add    %al,(%rax)
-   18006bac6:	sub    (%rsi),%al
+   18006bac6:	and    $0x6,%al
    18006bac8:	(bad)
    18006bac9:	insl   (%dx),%es:(%rdi)
    18006baca:	(bad)
    18006bacb:	imul   $0x726f6f63,0x5f(%rsi),%ebp
    18006bad2:	imul   $0x725f6574,%fs:0x61(%rsi),%ebp
    18006bada:	gs data16 gs jb 0x18006bb44
    18006badf:	outsb  %ds:(%rsi),(%dx)
@@ -157455,19 +157457,15 @@
    18006bb5a:	jne    0x18006bbc5
    18006bb5c:	insb   (%dx),%es:(%rdi)
    18006bb5d:	fs gs jb 0x18006bba1
    18006bb61:	and    $0x30,%al
    18006bb63:	xor    %eax,0x32(%rax)
    18006bb66:	rex pop %rax
    18006bb68:	pop    %rdx
-   18006bb69:	add    %ch,(%rbx)
-   18006bb6b:	(bad)
-   18006bb6c:	(bad)
-   18006bb6d:	insl   (%dx),%es:(%rdi)
-   18006bb6e:	(bad)
+   18006bb69:	add    %ah,0x616d3f06(%rip)        # 0x1e173fa75
    18006bb6f:	imul   $0x726f6f63,0x5f(%rsi),%ebp
    18006bb76:	imul   $0x725f6574,%fs:0x61(%rsi),%ebp
    18006bb7e:	gs data16 gs jb 0x18006bbe8
    18006bb83:	outsb  %ds:(%rsi),(%dx)
    18006bb84:	movsxd 0x5f(%rbp),%esp
    18006bb87:	jae    0x18006bc02
    18006bb89:	jae    0x18006bbff
@@ -157525,16 +157523,15 @@
    18006bbfe:	jne    0x18006bc69
    18006bc00:	insb   (%dx),%es:(%rdi)
    18006bc01:	fs gs jb 0x18006bc45
    18006bc05:	and    $0x30,%al
    18006bc07:	xor    0x32(%rax),%al
    18006bc0a:	rex pop %rax
    18006bc0c:	pop    %rdx
-   18006bc0d:	add    %cl,0x69663f05(%rsi)
-   18006bc13:	outsb  %ds:(%rsi),(%dx)
+   18006bc0d:	add    %cl,0x6e69663f(%rbp,%rax,1)
    18006bc14:	fs pop %rdi
    18006bc16:	movsxd 0x6f(%rdi),%ebp
    18006bc19:	jb     0x18006bc7f
    18006bc1b:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006bc22:	gs data16 gs jb 0x18006bc8c
    18006bc27:	outsb  %ds:(%rsi),(%dx)
    18006bc28:	movsxd 0x5f(%rbp),%esp
@@ -157588,16 +157585,16 @@
    18006bc8f:	outsb  %ds:(%rsi),(%dx)
    18006bc90:	addr32 pop %rdi
    18006bc92:	jbe    0x18006bcfd
    18006bc94:	gs ja  0x18006bcd7
    18006bc97:	(bad)
    18006bc98:	(bad)
    18006bc9d:	rex pop %rdx
-   18006bc9f:	add    %cl,(%rbx,%rax,1)
-   18006bca2:	(bad)
+   18006bc9f:	add    %cl,(%rdx)
+   18006bca1:	add    (%rdi),%edi
    18006bca3:	(bad)
    18006bca4:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006bca8:	gs pop %rdi
    18006bcaa:	movsxd 0x6f(%rdi),%ebp
    18006bcad:	jb     0x18006bd13
    18006bcaf:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006bcb6:	gs data16 gs jb 0x18006bd20
@@ -157646,15 +157643,15 @@
    18006bd14:	je     0x18006bd7b
    18006bd16:	insl   (%dx),%es:(%rdi)
    18006bd17:	rex and $0x30,%al
    18006bd1a:	xor    0x32(%rax),%al
    18006bd1d:	rex pop %rax
    18006bd1f:	pop    %rdx
    18006bd20:	add    %al,(%rax)
-   18006bd22:	adc    (%rbx),%al
+   18006bd22:	adc    %al,(%rbx)
    18006bd24:	(bad)
    18006bd25:	(bad)
    18006bd26:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006bd2a:	gs pop %rdi
    18006bd2c:	movsxd 0x6f(%rdi),%ebp
    18006bd2f:	jb     0x18006bd95
    18006bd31:	imul   $0x725f6574,0x61(%rsi),%ebp
@@ -157700,15 +157697,16 @@
    18006bd89:	jbe    0x18006bdf4
    18006bd8b:	gs ja  0x18006bdce
    18006bd8e:	(bad)
    18006bd8f:	(bad)
    18006bd94:	pop    %rax
    18006bd95:	pop    %rdx
    18006bd96:	add    %al,(%rax)
-   18006bd98:	addb   $0x3f,(%rbx)
+   18006bd98:	jle    0x18006bd9d
+   18006bd9a:	(bad)
    18006bd9b:	movsxd 0x6f(%rdi),%ebp
    18006bd9e:	jb     0x18006be04
    18006bda0:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006bda7:	gs data16 gs jb 0x18006be11
    18006bdac:	outsb  %ds:(%rsi),(%dx)
    18006bdad:	movsxd 0x5f(%rbp),%esp
    18006bdb0:	jae    0x18006be2b
@@ -157748,15 +157746,16 @@
    18006bdf7:	outsb  %ds:(%rsi),(%dx)
    18006bdf8:	addr32 pop %rdi
    18006bdfa:	jbe    0x18006be65
    18006bdfc:	gs ja  0x18006be3f
    18006bdff:	(bad)
    18006be00:	(bad)
    18006be05:	rex pop %rdx
-   18006be07:	add    %al,(%rdi,%rax,1)
+   18006be07:	add    %bh,%dh
+   18006be09:	(bad)
    18006be0a:	(bad)
    18006be0b:	jb     0x18006be72
    18006be0d:	imul   $0x635f7265,0x74(%ebx),%esi
    18006be15:	outsl  %ds:(%rsi),(%dx)
    18006be16:	outsl  %ds:(%rsi),(%dx)
    18006be17:	jb     0x18006be7d
    18006be19:	imul   $0x725f6574,0x61(%rsi),%ebp
@@ -157831,16 +157830,15 @@
    18006beb4:	fs gs rex
    18006beb7:	rex
    18006beb8:	rex jae 0x18006bf2f
    18006bebb:	fs rex
    18006bebd:	rex
    18006bebe:	rex pop %rdx
    18006bec0:	add    %al,(%rax)
-   18006bec2:	and    $0x4,%al
-   18006bec4:	(bad)
+   18006bec2:	and    (%rdi,%rdi,1),%al
    18006bec5:	fs gs insb (%dx),%es:(%rdi)
    18006bec8:	gs je  0x18006bf30
    18006becb:	pop    %rdi
    18006becc:	movsxd 0x6f(%rdi),%ebp
    18006becf:	jb     0x18006bf35
    18006bed1:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006bed8:	gs data16 gs jb 0x18006bf42
@@ -157882,15 +157880,16 @@
    18006bf27:	outsb  %ds:(%rsi),(%dx)
    18006bf28:	addr32 pop %rdi
    18006bf2a:	jbe    0x18006bf95
    18006bf2c:	gs ja  0x18006bf6f
    18006bf2f:	(bad)
    18006bf30:	(bad)
    18006bf35:	rex pop %rdx
-   18006bf37:	add    %dh,(%rdi,%rax,1)
+   18006bf37:	add    %ch,(%rsi)
+   18006bf39:	(bad)
    18006bf3a:	(bad)
    18006bf3b:	jae    0x18006bfa2
    18006bf3d:	je     0x18006bf9e
    18006bf3f:	(bad)
    18006bf40:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006bf44:	gs pop %rdi
    18006bf46:	movsxd 0x6f(%rdi),%ebp
@@ -157935,15 +157934,15 @@
    18006bfa1:	outsb  %ds:(%rsi),(%dx)
    18006bfa2:	addr32 pop %rdi
    18006bfa4:	jbe    0x18006c00f
    18006bfa6:	gs ja  0x18006bfe9
    18006bfa9:	(bad)
    18006bfaa:	(bad)
    18006bfaf:	rex pop %rdx
-   18006bfb1:	add    %cl,0x69663f05(%rbp)
+   18006bfb1:	add    %cl,0x69663f05(%rbx)
    18006bfb7:	outsb  %ds:(%rsi),(%dx)
    18006bfb8:	fs pop %rdi
    18006bfba:	movsxd 0x6f(%rdi),%ebp
    18006bfbd:	jb     0x18006c023
    18006bfbf:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006bfc6:	gs data16 gs jb 0x18006c030
    18006bfcb:	outsb  %ds:(%rsi),(%dx)
@@ -157998,15 +157997,15 @@
    18006c033:	outsb  %ds:(%rsi),(%dx)
    18006c034:	addr32 pop %rdi
    18006c036:	jbe    0x18006c0a1
    18006c038:	gs ja  0x18006c07b
    18006c03b:	(bad)
    18006c03c:	(bad)
    18006c041:	rex pop %rdx
-   18006c043:	add    %cl,(%rbx)
+   18006c043:	add    %cl,(%rcx)
    18006c045:	add    (%rdi),%edi
    18006c047:	(bad)
    18006c048:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006c04c:	gs pop %rdi
    18006c04e:	movsxd 0x6f(%rdi),%ebp
    18006c051:	jb     0x18006c0b7
    18006c053:	imul   $0x725f6574,0x61(%rsi),%ebp
@@ -158056,16 +158055,15 @@
    18006c0b8:	je     0x18006c11f
    18006c0ba:	insl   (%dx),%es:(%rdi)
    18006c0bb:	rex and $0x30,%al
    18006c0be:	xor    %eax,0x32(%rax)
    18006c0c1:	rex pop %rax
    18006c0c3:	pop    %rdx
    18006c0c4:	add    %al,(%rax)
-   18006c0c6:	adc    %eax,(%rbx)
-   18006c0c8:	(bad)
+   18006c0c6:	lsl    (%rdi),%edi
    18006c0c9:	(bad)
    18006c0ca:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006c0ce:	gs pop %rdi
    18006c0d0:	movsxd 0x6f(%rdi),%ebp
    18006c0d3:	jb     0x18006c139
    18006c0d5:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006c0dc:	gs data16 gs jb 0x18006c146
@@ -158110,15 +158108,15 @@
    18006c12d:	jbe    0x18006c198
    18006c12f:	gs ja  0x18006c172
    18006c132:	(bad)
    18006c133:	(bad)
    18006c138:	pop    %rax
    18006c139:	pop    %rdx
    18006c13a:	add    %al,(%rax)
-   18006c13c:	jg     0x18006c141
+   18006c13c:	jge    0x18006c141
    18006c13e:	(bad)
    18006c13f:	movsxd 0x6f(%rdi),%ebp
    18006c142:	jb     0x18006c1a8
    18006c144:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006c14b:	gs data16 gs jb 0x18006c1b5
    18006c150:	outsb  %ds:(%rsi),(%dx)
    18006c151:	movsxd 0x5f(%rbp),%esp
@@ -158159,15 +158157,15 @@
    18006c19b:	outsb  %ds:(%rsi),(%dx)
    18006c19c:	addr32 pop %rdi
    18006c19e:	jbe    0x18006c209
    18006c1a0:	gs ja  0x18006c1e3
    18006c1a3:	(bad)
    18006c1a4:	(bad)
    18006c1a9:	rex pop %rdx
-   18006c1ab:	add    %al,(%rbx)
+   18006c1ab:	add    %bh,%ch
    18006c1ad:	(bad)
    18006c1ae:	(bad)
    18006c1af:	jb     0x18006c216
    18006c1b1:	imul   $0x635f7265,0x74(%ebx),%esi
    18006c1b9:	outsl  %ds:(%rsi),(%dx)
    18006c1ba:	outsl  %ds:(%rsi),(%dx)
    18006c1bb:	jb     0x18006c221
@@ -158243,15 +158241,15 @@
    18006c258:	fs gs rex
    18006c25b:	rex
    18006c25c:	rex jae 0x18006c2d3
    18006c25f:	fs rex
    18006c261:	rex
    18006c262:	rex pop %rdx
    18006c264:	add    %al,(%rax)
-   18006c266:	and    (%rdi,%rdi,1),%eax
+   18006c266:	and    %eax,(%rdi,%rdi,1)
    18006c269:	fs gs insb (%dx),%es:(%rdi)
    18006c26c:	gs je  0x18006c2d4
    18006c26f:	pop    %rdi
    18006c270:	movsxd 0x6f(%rdi),%ebp
    18006c273:	jb     0x18006c2d9
    18006c275:	imul   $0x725f6574,0x61(%rsi),%ebp
    18006c27c:	gs data16 gs jb 0x18006c2e6
@@ -158293,18 +158291,15 @@
    18006c2cb:	outsb  %ds:(%rsi),(%dx)
    18006c2cc:	addr32 pop %rdi
    18006c2ce:	jbe    0x18006c339
    18006c2d0:	gs ja  0x18006c313
    18006c2d3:	(bad)
    18006c2d4:	(bad)
    18006c2d9:	rex pop %rdx
-   18006c2db:	add    %dh,(%rbx)
-   18006c2dd:	(bad)
-   18006c2de:	(bad)
-   18006c2df:	jae    0x18006c346
+   18006c2db:	add    %ch,0x65733f07(%rip)        # 0x1e57a01e8
    18006c2e1:	je     0x18006c342
    18006c2e3:	(bad)
    18006c2e4:	movsxd 0x76(%rcx,%rbp,2),%esi
    18006c2e8:	gs pop %rdi
    18006c2ea:	movsxd 0x6f(%rdi),%ebp
    18006c2ed:	jb     0x18006c353
    18006c2ef:	imul   $0x725f6574,0x61(%rsi),%ebp
```

## opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180046450
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jul 12 00:50:27 2023
+Time/Date		Tue Jul 11 09:06:27 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000048c00
 SizeOfInitializedData	000000000002cc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000046450
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0007a000
 SizeOfHeaders		00000400
-CheckSum		0007a6de
+CheckSum		0007eb4a
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -240,85 +240,85 @@
 	66950	  356  ??1BlockRange@?$Blocks@$02@geode@@QEAA@XZ
 	6691c	  161  ??0BlockRange@?$Blocks@$02@geode@@QEAA@AEBV012@@Z
 
  0006347c	00063f40 00000000 00000000 00068ca4 0004a920
 
 	DLL Name: OpenGeode_mesh.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	68bf0	  956  ?create@?$EdgedCurveBuilder@$01@geode@@SA?AV?$unique_ptr@V?$EdgedCurveBuilder@$01@geode@@U?$default_delete@V?$EdgedCurveBuilder@$01@geode@@@std@@@std@@AEAV?$EdgedCurve@$01@2@@Z
-	68b68	  849  ?clone@?$EdgedCurve@$01@geode@@QEBA?AV?$unique_ptr@V?$EdgedCurve@$01@geode@@U?$default_delete@V?$EdgedCurve@$01@geode@@@std@@@std@@XZ
-	68b00	 1735  ?polygon_vertices@?$SurfaceMesh@$01@geode@@QEBA?AV?$InlinedVector@I$02V?$allocator@I@std@@@absl@@I@Z
-	68ab8	 1733  ?polygon_vertex@?$SurfaceMesh@$01@geode@@QEBAIAEBUPolygonVertex@2@@Z
-	68a7e	 1659  ?nb_polygon_vertices@?$SurfaceMesh@$01@geode@@QEBAEI@Z
-	68a4e	 1661  ?nb_polygons@?$SurfaceMesh@$01@geode@@QEBAIXZ
-	689e8	 2066  ?value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEBA?AV?$Point@$00@2@AEBV?$Point@$01@2@I@Z
-	68994	 2067  ?value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEBAAEBV?$Point@$00@2@I@Z
-	6893e	 1912  ?set_value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAAXIV?$Point@$00@2@@Z
-	688c6	 1413  ?find@?$TriangulatedSurfacePointFunction@$01$00@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@@Z
-	6883e	 1011  ?create@?$TriangulatedSurfacePointFunction@$01$00@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@V?$Point@$00@2@@Z
-	68800	  583  ??1?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAA@XZ
-	687b8	  422  ??0?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAA@$$QEAV01@@Z
-	68798	  463  ??0PolygonEdge@geode@@QEAA@XZ
-	68752	 1341  ?edge_attribute_manager@Graph@geode@@QEBAAEAVAttributeManager@2@XZ
-	68716	 1369  ?edge_vertices@Graph@geode@@QEBA?AV?$array@I$01@std@@I@Z
-	686e0	 1365  ?edge_vertex@Graph@geode@@QEBAIAEBUEdgeVertex@2@@Z
-	68628	  997  ?create@?$SurfaceMeshBuilder@$02@geode@@SA?AV?$unique_ptr@V?$SurfaceMeshBuilder@$02@geode@@U?$default_delete@V?$SurfaceMeshBuilder@$02@geode@@@std@@@std@@AEAV?$SurfaceMesh@$02@2@@Z
-	68584	  864  ?clone@?$TriangulatedSurface@$02@geode@@QEBA?AV?$unique_ptr@V?$TriangulatedSurface@$02@geode@@U?$default_delete@V?$TriangulatedSurface@$02@geode@@@std@@@std@@XZ
-	68530	 1718  ?polygon_attribute_manager@?$SurfaceMesh@$02@geode@@QEBAAEAVAttributeManager@2@XZ
-	684e8	 1734  ?polygon_vertex@?$SurfaceMesh@$02@geode@@QEBAIAEBUPolygonVertex@2@@Z
-	684ae	 1660  ?nb_polygon_vertices@?$SurfaceMesh@$02@geode@@QEBAEI@Z
-	6847e	 1662  ?nb_polygons@?$SurfaceMesh@$02@geode@@QEBAIXZ
-	68432	 1777  ?polyhedron_vertex@?$SolidMesh@$02@geode@@QEBAIAEBUPolyhedronVertex@2@@Z
-	683f8	 1666  ?nb_polyhedron_vertices@?$SolidMesh@$02@geode@@QEBAEI@Z
-	68396	 2060  ?value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEBA?AV?$Point@$01@2@AEBV?$Point@$02@2@I@Z
-	68344	 2061  ?value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEBAAEBV?$Point@$01@2@I@Z
-	682f0	 1909  ?set_value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEAAXIV?$Point@$01@2@@Z
-	6827e	 1410  ?find@?$TetrahedralSolidPointFunction@$02$01@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@@Z
-	681fc	 1002  ?create@?$TetrahedralSolidPointFunction@$02$01@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@V?$Point@$01@2@@Z
-	681c0	  567  ??1?$TetrahedralSolidPointFunction@$02$01@geode@@QEAA@XZ
-	6817c	  386  ??0?$TetrahedralSolidPointFunction@$02$01@geode@@QEAA@$$QEAV01@@Z
-	68158	  468  ??0PolyhedronFacet@geode@@QEAA@XZ
-	680bc	 1998  ?type_name_static@?$TetrahedralSolid@$02@geode@@SA?AV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UMeshTypeTag@geode@@@2@XZ
-	68054	  691  ??R?$DistanceToTetrahedron@$02@geode@@QEBA?AV?$tuple@NV?$Point@$02@geode@@@std@@AEBV?$Point@$02@1@I@Z
-	68004	   22  ??$create_aabb_tree@$02@geode@@YA?AV?$AABBTree@$02@0@AEBV?$SolidMesh@$02@0@@Z
-	67fb4	 2064  ?value@?$TetrahedralSolidScalarFunction@$02@geode@@QEBANAEBV?$Point@$02@2@I@Z
-	67f76	 2065  ?value@?$TetrahedralSolidScalarFunction@$02@geode@@QEBANI@Z
-	67f32	 1911  ?set_value@?$TetrahedralSolidScalarFunction@$02@geode@@QEAAXIN@Z
-	67ec2	 1412  ?find@?$TetrahedralSolidScalarFunction@$02@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@@Z
-	67e50	 1004  ?create@?$TetrahedralSolidScalarFunction@$02@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@N@Z
-	67e16	  569  ??1?$TetrahedralSolidScalarFunction@$02@geode@@QEAA@XZ
-	67dd4	  392  ??0?$TetrahedralSolidScalarFunction@$02@geode@@QEAA@$$QEAV01@@Z
-	67cd0	  692  ??R?$DistanceToTriangle@$01@geode@@QEBA?AV?$tuple@NV?$Point@$01@geode@@@std@@AEBV?$Point@$01@1@I@Z
-	6727e	 1650  ?nb_edges@Graph@geode@@QEBAIXZ
-	672a0	 1377  ?edges_around_vertex@Graph@geode@@QEBAAEBV?$InlinedVector@UEdgeVertex@geode@@$01V?$allocator@UEdgeVertex@geode@@@std@@@absl@@I@Z
-	67324	 1020  ?create@GraphBuilder@geode@@SA?AV?$unique_ptr@VGraphBuilder@geode@@U?$default_delete@VGraphBuilder@geode@@@std@@@std@@AEAVGraph@2@@Z
-	673ac	 1067  ?delete_edges@GraphBuilder@geode@@QEAA?AV?$vector@IV?$allocator@I@std@@@std@@AEBV?$vector@_NV?$allocator@_N@std@@@4@@Z
-	67426	 1673  ?nb_vertices@VertexSet@geode@@QEBAIXZ
-	6744e	 2080  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
-	6749a	 1707  ?point@?$CoordinateReferenceSystemManagers@$01@geode@@QEBAAEBV?$Point@$01@2@I@Z
-	674ec	 1708  ?point@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$Point@$02@2@I@Z
-	6753e	 1663  ?nb_polyhedra@?$SolidMesh@$02@geode@@QEBAIXZ
-	6756e	 1780  ?polyhedron_vertices@?$SolidMesh@$02@geode@@QEBA?AV?$InlinedVector@I$03V?$allocator@I@std@@@absl@@I@Z
-	675d6	  863  ?clone@?$TriangulatedSurface@$01@geode@@QEBA?AV?$unique_ptr@V?$TriangulatedSurface@$01@geode@@U?$default_delete@V?$TriangulatedSurface@$01@geode@@@std@@@std@@XZ
-	6767a	 1871  ?set_point@?$CoordinateReferenceSystemManagersBuilder@$01@geode@@QEAAXIV?$Point@$01@2@@Z
-	676d6	 1009  ?create@?$TriangulatedSurfaceBuilder@$01@geode@@SA?AV?$unique_ptr@V?$TriangulatedSurfaceBuilder@$01@geode@@U?$default_delete@V?$TriangulatedSurfaceBuilder@$01@geode@@@std@@@std@@AEAV?$TriangulatedSurface@$01@2@@Z
-	677ae	   84  ??$save_triangulated_surface@$01@geode@@YAXAEBV?$TriangulatedSurface@$01@0@Vstring_view@absl@@@Z
-	67812	  862  ?clone@?$TetrahedralSolid@$02@geode@@QEBA?AV?$unique_ptr@V?$TetrahedralSolid@$02@geode@@U?$default_delete@V?$TetrahedralSolid@$02@geode@@@std@@@std@@XZ
-	678ac	 1872  ?set_point@?$CoordinateReferenceSystemManagersBuilder@$02@geode@@QEAAXIV?$Point@$02@2@@Z
-	67d36	 1999  ?type_name_static@?$TriangulatedSurface@$01@geode@@SA?AV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UMeshTypeTag@geode@@@2@XZ
-	67908	 1000  ?create@?$TetrahedralSolidBuilder@$02@geode@@SA?AV?$unique_ptr@V?$TetrahedralSolidBuilder@$02@geode@@U?$default_delete@V?$TetrahedralSolidBuilder@$02@geode@@@std@@@std@@AEAV?$TetrahedralSolid@$02@2@@Z
-	679d4	   83  ??$save_tetrahedral_solid@$02@geode@@YAXAEBV?$TetrahedralSolid@$02@0@Vstring_view@absl@@@Z
-	67a32	  437  ??0?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAA@$$QEAV01@@Z
-	67a78	  588  ??1?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAA@XZ
-	67ab4	 1016  ?create@?$TriangulatedSurfaceScalarFunction@$01@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@N@Z
-	67b2c	 1418  ?find@?$TriangulatedSurfaceScalarFunction@$01@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@@Z
-	67ba2	 1917  ?set_value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAAXIN@Z
-	67be8	 2077  ?value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEBANI@Z
-	67c2a	 2076  ?value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEBANAEBV?$Point@$01@2@I@Z
-	67c7e	   20  ??$create_aabb_tree@$01@geode@@YA?AV?$AABBTree@$01@0@AEBV?$SurfaceMesh@$01@0@@Z
+	68bf0	  954  ?create@?$EdgedCurveBuilder@$01@geode@@SA?AV?$unique_ptr@V?$EdgedCurveBuilder@$01@geode@@U?$default_delete@V?$EdgedCurveBuilder@$01@geode@@@std@@@std@@AEAV?$EdgedCurve@$01@2@@Z
+	68b68	  847  ?clone@?$EdgedCurve@$01@geode@@QEBA?AV?$unique_ptr@V?$EdgedCurve@$01@geode@@U?$default_delete@V?$EdgedCurve@$01@geode@@@std@@@std@@XZ
+	68b00	 1729  ?polygon_vertices@?$SurfaceMesh@$01@geode@@QEBA?AV?$InlinedVector@I$02V?$allocator@I@std@@@absl@@I@Z
+	68ab8	 1727  ?polygon_vertex@?$SurfaceMesh@$01@geode@@QEBAIAEBUPolygonVertex@2@@Z
+	68a7e	 1653  ?nb_polygon_vertices@?$SurfaceMesh@$01@geode@@QEBAEI@Z
+	68a4e	 1655  ?nb_polygons@?$SurfaceMesh@$01@geode@@QEBAIXZ
+	689e8	 2060  ?value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEBA?AV?$Point@$00@2@AEBV?$Point@$01@2@I@Z
+	68994	 2061  ?value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEBAAEBV?$Point@$00@2@I@Z
+	6893e	 1906  ?set_value@?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAAXIV?$Point@$00@2@@Z
+	688c6	 1411  ?find@?$TriangulatedSurfacePointFunction@$01$00@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@@Z
+	6883e	 1009  ?create@?$TriangulatedSurfacePointFunction@$01$00@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@V?$Point@$00@2@@Z
+	68800	  581  ??1?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAA@XZ
+	687b8	  420  ??0?$TriangulatedSurfacePointFunction@$01$00@geode@@QEAA@$$QEAV01@@Z
+	68798	  461  ??0PolygonEdge@geode@@QEAA@XZ
+	68752	 1339  ?edge_attribute_manager@Graph@geode@@QEBAAEAVAttributeManager@2@XZ
+	68716	 1367  ?edge_vertices@Graph@geode@@QEBA?AV?$array@I$01@std@@I@Z
+	686e0	 1363  ?edge_vertex@Graph@geode@@QEBAIAEBUEdgeVertex@2@@Z
+	68628	  995  ?create@?$SurfaceMeshBuilder@$02@geode@@SA?AV?$unique_ptr@V?$SurfaceMeshBuilder@$02@geode@@U?$default_delete@V?$SurfaceMeshBuilder@$02@geode@@@std@@@std@@AEAV?$SurfaceMesh@$02@2@@Z
+	68584	  862  ?clone@?$TriangulatedSurface@$02@geode@@QEBA?AV?$unique_ptr@V?$TriangulatedSurface@$02@geode@@U?$default_delete@V?$TriangulatedSurface@$02@geode@@@std@@@std@@XZ
+	68530	 1712  ?polygon_attribute_manager@?$SurfaceMesh@$02@geode@@QEBAAEAVAttributeManager@2@XZ
+	684e8	 1728  ?polygon_vertex@?$SurfaceMesh@$02@geode@@QEBAIAEBUPolygonVertex@2@@Z
+	684ae	 1654  ?nb_polygon_vertices@?$SurfaceMesh@$02@geode@@QEBAEI@Z
+	6847e	 1656  ?nb_polygons@?$SurfaceMesh@$02@geode@@QEBAIXZ
+	68432	 1771  ?polyhedron_vertex@?$SolidMesh@$02@geode@@QEBAIAEBUPolyhedronVertex@2@@Z
+	683f8	 1660  ?nb_polyhedron_vertices@?$SolidMesh@$02@geode@@QEBAEI@Z
+	68396	 2054  ?value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEBA?AV?$Point@$01@2@AEBV?$Point@$02@2@I@Z
+	68344	 2055  ?value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEBAAEBV?$Point@$01@2@I@Z
+	682f0	 1903  ?set_value@?$TetrahedralSolidPointFunction@$02$01@geode@@QEAAXIV?$Point@$01@2@@Z
+	6827e	 1408  ?find@?$TetrahedralSolidPointFunction@$02$01@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@@Z
+	681fc	 1000  ?create@?$TetrahedralSolidPointFunction@$02$01@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@V?$Point@$01@2@@Z
+	681c0	  565  ??1?$TetrahedralSolidPointFunction@$02$01@geode@@QEAA@XZ
+	6817c	  384  ??0?$TetrahedralSolidPointFunction@$02$01@geode@@QEAA@$$QEAV01@@Z
+	68158	  466  ??0PolyhedronFacet@geode@@QEAA@XZ
+	680bc	 1992  ?type_name_static@?$TetrahedralSolid@$02@geode@@SA?AV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UMeshTypeTag@geode@@@2@XZ
+	68054	  689  ??R?$DistanceToTetrahedron@$02@geode@@QEBA?AV?$tuple@NV?$Point@$02@geode@@@std@@AEBV?$Point@$02@1@I@Z
+	68004	   20  ??$create_aabb_tree@$02@geode@@YA?AV?$AABBTree@$02@0@AEBV?$SolidMesh@$02@0@@Z
+	67fb4	 2058  ?value@?$TetrahedralSolidScalarFunction@$02@geode@@QEBANAEBV?$Point@$02@2@I@Z
+	67f76	 2059  ?value@?$TetrahedralSolidScalarFunction@$02@geode@@QEBANI@Z
+	67f32	 1905  ?set_value@?$TetrahedralSolidScalarFunction@$02@geode@@QEAAXIN@Z
+	67ec2	 1410  ?find@?$TetrahedralSolidScalarFunction@$02@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@@Z
+	67e50	 1002  ?create@?$TetrahedralSolidScalarFunction@$02@geode@@SA?AV12@AEBV?$TetrahedralSolid@$02@2@Vstring_view@absl@@N@Z
+	67e16	  567  ??1?$TetrahedralSolidScalarFunction@$02@geode@@QEAA@XZ
+	67dd4	  390  ??0?$TetrahedralSolidScalarFunction@$02@geode@@QEAA@$$QEAV01@@Z
+	67cd0	  690  ??R?$DistanceToTriangle@$01@geode@@QEBA?AV?$tuple@NV?$Point@$01@geode@@@std@@AEBV?$Point@$01@1@I@Z
+	6727e	 1644  ?nb_edges@Graph@geode@@QEBAIXZ
+	672a0	 1375  ?edges_around_vertex@Graph@geode@@QEBAAEBV?$InlinedVector@UEdgeVertex@geode@@$01V?$allocator@UEdgeVertex@geode@@@std@@@absl@@I@Z
+	67324	 1018  ?create@GraphBuilder@geode@@SA?AV?$unique_ptr@VGraphBuilder@geode@@U?$default_delete@VGraphBuilder@geode@@@std@@@std@@AEAVGraph@2@@Z
+	673ac	 1065  ?delete_edges@GraphBuilder@geode@@QEAA?AV?$vector@IV?$allocator@I@std@@@std@@AEBV?$vector@_NV?$allocator@_N@std@@@4@@Z
+	67426	 1667  ?nb_vertices@VertexSet@geode@@QEBAIXZ
+	6744e	 2074  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
+	6749a	 1701  ?point@?$CoordinateReferenceSystemManagers@$01@geode@@QEBAAEBV?$Point@$01@2@I@Z
+	674ec	 1702  ?point@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$Point@$02@2@I@Z
+	6753e	 1657  ?nb_polyhedra@?$SolidMesh@$02@geode@@QEBAIXZ
+	6756e	 1774  ?polyhedron_vertices@?$SolidMesh@$02@geode@@QEBA?AV?$InlinedVector@I$03V?$allocator@I@std@@@absl@@I@Z
+	675d6	  861  ?clone@?$TriangulatedSurface@$01@geode@@QEBA?AV?$unique_ptr@V?$TriangulatedSurface@$01@geode@@U?$default_delete@V?$TriangulatedSurface@$01@geode@@@std@@@std@@XZ
+	6767a	 1865  ?set_point@?$CoordinateReferenceSystemManagersBuilder@$01@geode@@QEAAXIV?$Point@$01@2@@Z
+	676d6	 1007  ?create@?$TriangulatedSurfaceBuilder@$01@geode@@SA?AV?$unique_ptr@V?$TriangulatedSurfaceBuilder@$01@geode@@U?$default_delete@V?$TriangulatedSurfaceBuilder@$01@geode@@@std@@@std@@AEAV?$TriangulatedSurface@$01@2@@Z
+	677ae	   82  ??$save_triangulated_surface@$01@geode@@YAXAEBV?$TriangulatedSurface@$01@0@Vstring_view@absl@@@Z
+	67812	  860  ?clone@?$TetrahedralSolid@$02@geode@@QEBA?AV?$unique_ptr@V?$TetrahedralSolid@$02@geode@@U?$default_delete@V?$TetrahedralSolid@$02@geode@@@std@@@std@@XZ
+	678ac	 1866  ?set_point@?$CoordinateReferenceSystemManagersBuilder@$02@geode@@QEAAXIV?$Point@$02@2@@Z
+	67d36	 1993  ?type_name_static@?$TriangulatedSurface@$01@geode@@SA?AV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UMeshTypeTag@geode@@@2@XZ
+	67908	  998  ?create@?$TetrahedralSolidBuilder@$02@geode@@SA?AV?$unique_ptr@V?$TetrahedralSolidBuilder@$02@geode@@U?$default_delete@V?$TetrahedralSolidBuilder@$02@geode@@@std@@@std@@AEAV?$TetrahedralSolid@$02@2@@Z
+	679d4	   81  ??$save_tetrahedral_solid@$02@geode@@YAXAEBV?$TetrahedralSolid@$02@0@Vstring_view@absl@@@Z
+	67a32	  435  ??0?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAA@$$QEAV01@@Z
+	67a78	  586  ??1?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAA@XZ
+	67ab4	 1014  ?create@?$TriangulatedSurfaceScalarFunction@$01@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@N@Z
+	67b2c	 1416  ?find@?$TriangulatedSurfaceScalarFunction@$01@geode@@SA?AV12@AEBV?$TriangulatedSurface@$01@2@Vstring_view@absl@@@Z
+	67ba2	 1911  ?set_value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEAAXIN@Z
+	67be8	 2071  ?value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEBANI@Z
+	67c2a	 2070  ?value@?$TriangulatedSurfaceScalarFunction@$01@geode@@QEBANAEBV?$Point@$01@2@I@Z
+	67c7e	   18  ??$create_aabb_tree@$01@geode@@YA?AV?$AABBTree@$01@0@AEBV?$SurfaceMesh@$01@0@@Z
 
  00063490	00063d80 00000000 00000000 00069a72 0004a760
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	699f8	   41  ??$point_triangle_distance@$01@geode@@YA?AV?$tuple@NV?$Point@$01@geode@@@std@@AEBV?$Point@$01@0@AEBV?$Triangle@$01@0@@Z
 	68cb8	  323  ??0OwnerTetrahedron@geode@@QEAA@V?$Point@$02@1@000@Z
@@ -14586,422 +14586,422 @@
 	  c930: 65 73 40 3f 24 53 75 72 66 61 63 65 73 40 24 30
 	  c940: 32 40 67 65 6f 64 65 40 40 51 45 42 41 49 58 5a
 	  c950: 00 00 0a 04 3f 6e 62 5f 6d 6f 64 65 6c 5f 62 6f
 	  c960: 75 6e 64 61 72 69 65 73 40 3f 24 4d 6f 64 65 6c
 	  c970: 42 6f 75 6e 64 61 72 69 65 73 40 24 30 32 40 67
 	  c980: 65 6f 64 65 40 40 51 45 42 41 49 58 5a 00 4f 70
 	  c990: 65 6e 47 65 6f 64 65 5f 6d 6f 64 65 6c 2e 64 6c
-	  c9a0: 6c 00 72 06 3f 6e 62 5f 65 64 67 65 73 40 47 72
+	  c9a0: 6c 00 6c 06 3f 6e 62 5f 65 64 67 65 73 40 47 72
 	  c9b0: 61 70 68 40 67 65 6f 64 65 40 40 51 45 42 41 49
-	  c9c0: 58 5a 00 00 61 05 3f 65 64 67 65 73 5f 61 72 6f
+	  c9c0: 58 5a 00 00 5f 05 3f 65 64 67 65 73 5f 61 72 6f
 	  c9d0: 75 6e 64 5f 76 65 72 74 65 78 40 47 72 61 70 68
 	  c9e0: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
 	  c9f0: 3f 24 49 6e 6c 69 6e 65 64 56 65 63 74 6f 72 40
 	  ca00: 55 45 64 67 65 56 65 72 74 65 78 40 67 65 6f 64
 	  ca10: 65 40 40 24 30 31 56 3f 24 61 6c 6c 6f 63 61 74
 	  ca20: 6f 72 40 55 45 64 67 65 56 65 72 74 65 78 40 67
 	  ca30: 65 6f 64 65 40 40 40 73 74 64 40 40 40 61 62 73
-	  ca40: 6c 40 40 49 40 5a 00 00 fc 03 3f 63 72 65 61 74
+	  ca40: 6c 40 40 49 40 5a 00 00 fa 03 3f 63 72 65 61 74
 	  ca50: 65 40 47 72 61 70 68 42 75 69 6c 64 65 72 40 67
 	  ca60: 65 6f 64 65 40 40 53 41 3f 41 56 3f 24 75 6e 69
 	  ca70: 71 75 65 5f 70 74 72 40 56 47 72 61 70 68 42 75
 	  ca80: 69 6c 64 65 72 40 67 65 6f 64 65 40 40 55 3f 24
 	  ca90: 64 65 66 61 75 6c 74 5f 64 65 6c 65 74 65 40 56
 	  caa0: 47 72 61 70 68 42 75 69 6c 64 65 72 40 67 65 6f
 	  cab0: 64 65 40 40 40 73 74 64 40 40 40 73 74 64 40 40
 	  cac0: 41 45 41 56 47 72 61 70 68 40 32 40 40 5a 00 00
-	  cad0: 2b 04 3f 64 65 6c 65 74 65 5f 65 64 67 65 73 40
+	  cad0: 29 04 3f 64 65 6c 65 74 65 5f 65 64 67 65 73 40
 	  cae0: 47 72 61 70 68 42 75 69 6c 64 65 72 40 67 65 6f
 	  caf0: 64 65 40 40 51 45 41 41 3f 41 56 3f 24 76 65 63
 	  cb00: 74 6f 72 40 49 56 3f 24 61 6c 6c 6f 63 61 74 6f
 	  cb10: 72 40 49 40 73 74 64 40 40 40 73 74 64 40 40 41
 	  cb20: 45 42 56 3f 24 76 65 63 74 6f 72 40 5f 4e 56 3f
 	  cb30: 24 61 6c 6c 6f 63 61 74 6f 72 40 5f 4e 40 73 74
-	  cb40: 64 40 40 40 34 40 40 5a 00 00 89 06 3f 6e 62 5f
+	  cb40: 64 40 40 40 34 40 40 5a 00 00 83 06 3f 6e 62 5f
 	  cb50: 76 65 72 74 69 63 65 73 40 56 65 72 74 65 78 53
 	  cb60: 65 74 40 67 65 6f 64 65 40 40 51 45 42 41 49 58
-	  cb70: 5a 00 20 08 3f 76 65 72 74 65 78 5f 61 74 74 72
+	  cb70: 5a 00 1a 08 3f 76 65 72 74 65 78 5f 61 74 74 72
 	  cb80: 69 62 75 74 65 5f 6d 61 6e 61 67 65 72 40 56 65
 	  cb90: 72 74 65 78 53 65 74 40 67 65 6f 64 65 40 40 51
 	  cba0: 45 42 41 41 45 41 56 41 74 74 72 69 62 75 74 65
-	  cbb0: 4d 61 6e 61 67 65 72 40 32 40 58 5a 00 00 ab 06
+	  cbb0: 4d 61 6e 61 67 65 72 40 32 40 58 5a 00 00 a5 06
 	  cbc0: 3f 70 6f 69 6e 74 40 3f 24 43 6f 6f 72 64 69 6e
 	  cbd0: 61 74 65 52 65 66 65 72 65 6e 63 65 53 79 73 74
 	  cbe0: 65 6d 4d 61 6e 61 67 65 72 73 40 24 30 31 40 67
 	  cbf0: 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24
 	  cc00: 50 6f 69 6e 74 40 24 30 31 40 32 40 49 40 5a 00
-	  cc10: ac 06 3f 70 6f 69 6e 74 40 3f 24 43 6f 6f 72 64
+	  cc10: a6 06 3f 70 6f 69 6e 74 40 3f 24 43 6f 6f 72 64
 	  cc20: 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65 53 79
 	  cc30: 73 74 65 6d 4d 61 6e 61 67 65 72 73 40 24 30 32
 	  cc40: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
 	  cc50: 3f 24 50 6f 69 6e 74 40 24 30 32 40 32 40 49 40
-	  cc60: 5a 00 7f 06 3f 6e 62 5f 70 6f 6c 79 68 65 64 72
+	  cc60: 5a 00 79 06 3f 6e 62 5f 70 6f 6c 79 68 65 64 72
 	  cc70: 61 40 3f 24 53 6f 6c 69 64 4d 65 73 68 40 24 30
 	  cc80: 32 40 67 65 6f 64 65 40 40 51 45 42 41 49 58 5a
-	  cc90: 00 00 f4 06 3f 70 6f 6c 79 68 65 64 72 6f 6e 5f
+	  cc90: 00 00 ee 06 3f 70 6f 6c 79 68 65 64 72 6f 6e 5f
 	  cca0: 76 65 72 74 69 63 65 73 40 3f 24 53 6f 6c 69 64
 	  ccb0: 4d 65 73 68 40 24 30 32 40 67 65 6f 64 65 40 40
 	  ccc0: 51 45 42 41 3f 41 56 3f 24 49 6e 6c 69 6e 65 64
 	  ccd0: 56 65 63 74 6f 72 40 49 24 30 33 56 3f 24 61 6c
 	  cce0: 6c 6f 63 61 74 6f 72 40 49 40 73 74 64 40 40 40
-	  ccf0: 61 62 73 6c 40 40 49 40 5a 00 5f 03 3f 63 6c 6f
+	  ccf0: 61 62 73 6c 40 40 49 40 5a 00 5d 03 3f 63 6c 6f
 	  cd00: 6e 65 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65
 	  cd10: 64 53 75 72 66 61 63 65 40 24 30 31 40 67 65 6f
 	  cd20: 64 65 40 40 51 45 42 41 3f 41 56 3f 24 75 6e 69
 	  cd30: 71 75 65 5f 70 74 72 40 56 3f 24 54 72 69 61 6e
 	  cd40: 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 40 24
 	  cd50: 30 31 40 67 65 6f 64 65 40 40 55 3f 24 64 65 66
 	  cd60: 61 75 6c 74 5f 64 65 6c 65 74 65 40 56 3f 24 54
 	  cd70: 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61
 	  cd80: 63 65 40 24 30 31 40 67 65 6f 64 65 40 40 40 73
-	  cd90: 74 64 40 40 40 73 74 64 40 40 58 5a 00 00 4f 07
+	  cd90: 74 64 40 40 40 73 74 64 40 40 58 5a 00 00 49 07
 	  cda0: 3f 73 65 74 5f 70 6f 69 6e 74 40 3f 24 43 6f 6f
 	  cdb0: 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e 63 65
 	  cdc0: 53 79 73 74 65 6d 4d 61 6e 61 67 65 72 73 42 75
 	  cdd0: 69 6c 64 65 72 40 24 30 31 40 67 65 6f 64 65 40
 	  cde0: 40 51 45 41 41 58 49 56 3f 24 50 6f 69 6e 74 40
-	  cdf0: 24 30 31 40 32 40 40 5a 00 00 f1 03 3f 63 72 65
+	  cdf0: 24 30 31 40 32 40 40 5a 00 00 ef 03 3f 63 72 65
 	  ce00: 61 74 65 40 3f 24 54 72 69 61 6e 67 75 6c 61 74
 	  ce10: 65 64 53 75 72 66 61 63 65 42 75 69 6c 64 65 72
 	  ce20: 40 24 30 31 40 67 65 6f 64 65 40 40 53 41 3f 41
 	  ce30: 56 3f 24 75 6e 69 71 75 65 5f 70 74 72 40 56 3f
 	  ce40: 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72
 	  ce50: 66 61 63 65 42 75 69 6c 64 65 72 40 24 30 31 40
 	  ce60: 67 65 6f 64 65 40 40 55 3f 24 64 65 66 61 75 6c
 	  ce70: 74 5f 64 65 6c 65 74 65 40 56 3f 24 54 72 69 61
 	  ce80: 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 42
 	  ce90: 75 69 6c 64 65 72 40 24 30 31 40 67 65 6f 64 65
 	  cea0: 40 40 40 73 74 64 40 40 40 73 74 64 40 40 41 45
 	  ceb0: 41 56 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64
 	  cec0: 53 75 72 66 61 63 65 40 24 30 31 40 32 40 40 5a
-	  ced0: 00 00 54 00 3f 3f 24 73 61 76 65 5f 74 72 69 61
+	  ced0: 00 00 52 00 3f 3f 24 73 61 76 65 5f 74 72 69 61
 	  cee0: 6e 67 75 6c 61 74 65 64 5f 73 75 72 66 61 63 65
 	  cef0: 40 24 30 31 40 67 65 6f 64 65 40 40 59 41 58 41
 	  cf00: 45 42 56 3f 24 54 72 69 61 6e 67 75 6c 61 74 65
 	  cf10: 64 53 75 72 66 61 63 65 40 24 30 31 40 30 40 56
 	  cf20: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  cf30: 40 40 40 5a 00 00 5e 03 3f 63 6c 6f 6e 65 40 3f
+	  cf30: 40 40 40 5a 00 00 5c 03 3f 63 6c 6f 6e 65 40 3f
 	  cf40: 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69
 	  cf50: 64 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  cf60: 41 3f 41 56 3f 24 75 6e 69 71 75 65 5f 70 74 72
 	  cf70: 40 56 3f 24 54 65 74 72 61 68 65 64 72 61 6c 53
 	  cf80: 6f 6c 69 64 40 24 30 32 40 67 65 6f 64 65 40 40
 	  cf90: 55 3f 24 64 65 66 61 75 6c 74 5f 64 65 6c 65 74
 	  cfa0: 65 40 56 3f 24 54 65 74 72 61 68 65 64 72 61 6c
 	  cfb0: 53 6f 6c 69 64 40 24 30 32 40 67 65 6f 64 65 40
 	  cfc0: 40 40 73 74 64 40 40 40 73 74 64 40 40 58 5a 00
-	  cfd0: 50 07 3f 73 65 74 5f 70 6f 69 6e 74 40 3f 24 43
+	  cfd0: 4a 07 3f 73 65 74 5f 70 6f 69 6e 74 40 3f 24 43
 	  cfe0: 6f 6f 72 64 69 6e 61 74 65 52 65 66 65 72 65 6e
 	  cff0: 63 65 53 79 73 74 65 6d 4d 61 6e 61 67 65 72 73
 	  d000: 42 75 69 6c 64 65 72 40 24 30 32 40 67 65 6f 64
 	  d010: 65 40 40 51 45 41 41 58 49 56 3f 24 50 6f 69 6e
-	  d020: 74 40 24 30 32 40 32 40 40 5a 00 00 e8 03 3f 63
+	  d020: 74 40 24 30 32 40 32 40 40 5a 00 00 e6 03 3f 63
 	  d030: 72 65 61 74 65 40 3f 24 54 65 74 72 61 68 65 64
 	  d040: 72 61 6c 53 6f 6c 69 64 42 75 69 6c 64 65 72 40
 	  d050: 24 30 32 40 67 65 6f 64 65 40 40 53 41 3f 41 56
 	  d060: 3f 24 75 6e 69 71 75 65 5f 70 74 72 40 56 3f 24
 	  d070: 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69 64
 	  d080: 42 75 69 6c 64 65 72 40 24 30 32 40 67 65 6f 64
 	  d090: 65 40 40 55 3f 24 64 65 66 61 75 6c 74 5f 64 65
 	  d0a0: 6c 65 74 65 40 56 3f 24 54 65 74 72 61 68 65 64
 	  d0b0: 72 61 6c 53 6f 6c 69 64 42 75 69 6c 64 65 72 40
 	  d0c0: 24 30 32 40 67 65 6f 64 65 40 40 40 73 74 64 40
 	  d0d0: 40 40 73 74 64 40 40 41 45 41 56 3f 24 54 65 74
 	  d0e0: 72 61 68 65 64 72 61 6c 53 6f 6c 69 64 40 24 30
-	  d0f0: 32 40 32 40 40 5a 00 00 53 00 3f 3f 24 73 61 76
+	  d0f0: 32 40 32 40 40 5a 00 00 51 00 3f 3f 24 73 61 76
 	  d100: 65 5f 74 65 74 72 61 68 65 64 72 61 6c 5f 73 6f
 	  d110: 6c 69 64 40 24 30 32 40 67 65 6f 64 65 40 40 59
 	  d120: 41 58 41 45 42 56 3f 24 54 65 74 72 61 68 65 64
 	  d130: 72 61 6c 53 6f 6c 69 64 40 24 30 32 40 30 40 56
 	  d140: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  d150: 40 40 40 5a 00 00 b5 01 3f 3f 30 3f 24 54 72 69
+	  d150: 40 40 40 5a 00 00 b3 01 3f 3f 30 3f 24 54 72 69
 	  d160: 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63 65
 	  d170: 53 63 61 6c 61 72 46 75 6e 63 74 69 6f 6e 40 24
 	  d180: 30 31 40 67 65 6f 64 65 40 40 51 45 41 41 40 24
-	  d190: 24 51 45 41 56 30 31 40 40 5a 00 00 4c 02 3f 3f
+	  d190: 24 51 45 41 56 30 31 40 40 5a 00 00 4a 02 3f 3f
 	  d1a0: 31 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53
 	  d1b0: 75 72 66 61 63 65 53 63 61 6c 61 72 46 75 6e 63
 	  d1c0: 74 69 6f 6e 40 24 30 31 40 67 65 6f 64 65 40 40
-	  d1d0: 51 45 41 41 40 58 5a 00 f8 03 3f 63 72 65 61 74
+	  d1d0: 51 45 41 41 40 58 5a 00 f6 03 3f 63 72 65 61 74
 	  d1e0: 65 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64
 	  d1f0: 53 75 72 66 61 63 65 53 63 61 6c 61 72 46 75 6e
 	  d200: 63 74 69 6f 6e 40 24 30 31 40 67 65 6f 64 65 40
 	  d210: 40 53 41 3f 41 56 31 32 40 41 45 42 56 3f 24 54
 	  d220: 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61
 	  d230: 63 65 40 24 30 31 40 32 40 56 73 74 72 69 6e 67
 	  d240: 5f 76 69 65 77 40 61 62 73 6c 40 40 4e 40 5a 00
-	  d250: 8a 05 3f 66 69 6e 64 40 3f 24 54 72 69 61 6e 67
+	  d250: 88 05 3f 66 69 6e 64 40 3f 24 54 72 69 61 6e 67
 	  d260: 75 6c 61 74 65 64 53 75 72 66 61 63 65 53 63 61
 	  d270: 6c 61 72 46 75 6e 63 74 69 6f 6e 40 24 30 31 40
 	  d280: 67 65 6f 64 65 40 40 53 41 3f 41 56 31 32 40 41
 	  d290: 45 42 56 3f 24 54 72 69 61 6e 67 75 6c 61 74 65
 	  d2a0: 64 53 75 72 66 61 63 65 40 24 30 31 40 32 40 56
 	  d2b0: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  d2c0: 40 40 40 5a 00 00 7d 07 3f 73 65 74 5f 76 61 6c
+	  d2c0: 40 40 40 5a 00 00 77 07 3f 73 65 74 5f 76 61 6c
 	  d2d0: 75 65 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65
 	  d2e0: 64 53 75 72 66 61 63 65 53 63 61 6c 61 72 46 75
 	  d2f0: 6e 63 74 69 6f 6e 40 24 30 31 40 67 65 6f 64 65
-	  d300: 40 40 51 45 41 41 58 49 4e 40 5a 00 1d 08 3f 76
+	  d300: 40 40 51 45 41 41 58 49 4e 40 5a 00 17 08 3f 76
 	  d310: 61 6c 75 65 40 3f 24 54 72 69 61 6e 67 75 6c 61
 	  d320: 74 65 64 53 75 72 66 61 63 65 53 63 61 6c 61 72
 	  d330: 46 75 6e 63 74 69 6f 6e 40 24 30 31 40 67 65 6f
-	  d340: 64 65 40 40 51 45 42 41 4e 49 40 5a 00 00 1c 08
+	  d340: 64 65 40 40 51 45 42 41 4e 49 40 5a 00 00 16 08
 	  d350: 3f 76 61 6c 75 65 40 3f 24 54 72 69 61 6e 67 75
 	  d360: 6c 61 74 65 64 53 75 72 66 61 63 65 53 63 61 6c
 	  d370: 61 72 46 75 6e 63 74 69 6f 6e 40 24 30 31 40 67
 	  d380: 65 6f 64 65 40 40 51 45 42 41 4e 41 45 42 56 3f
 	  d390: 24 50 6f 69 6e 74 40 24 30 31 40 32 40 49 40 5a
-	  d3a0: 00 00 14 00 3f 3f 24 63 72 65 61 74 65 5f 61 61
+	  d3a0: 00 00 12 00 3f 3f 24 63 72 65 61 74 65 5f 61 61
 	  d3b0: 62 62 5f 74 72 65 65 40 24 30 31 40 67 65 6f 64
 	  d3c0: 65 40 40 59 41 3f 41 56 3f 24 41 41 42 42 54 72
 	  d3d0: 65 65 40 24 30 31 40 30 40 41 45 42 56 3f 24 53
 	  d3e0: 75 72 66 61 63 65 4d 65 73 68 40 24 30 31 40 30
-	  d3f0: 40 40 5a 00 b4 02 3f 3f 52 3f 24 44 69 73 74 61
+	  d3f0: 40 40 5a 00 b2 02 3f 3f 52 3f 24 44 69 73 74 61
 	  d400: 6e 63 65 54 6f 54 72 69 61 6e 67 6c 65 40 24 30
 	  d410: 31 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56
 	  d420: 3f 24 74 75 70 6c 65 40 4e 56 3f 24 50 6f 69 6e
 	  d430: 74 40 24 30 31 40 67 65 6f 64 65 40 40 40 73 74
 	  d440: 64 40 40 41 45 42 56 3f 24 50 6f 69 6e 74 40 24
-	  d450: 30 31 40 31 40 49 40 5a 00 00 cf 07 3f 74 79 70
+	  d450: 30 31 40 31 40 49 40 5a 00 00 c9 07 3f 74 79 70
 	  d460: 65 5f 6e 61 6d 65 5f 73 74 61 74 69 63 40 3f 24
 	  d470: 54 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66
 	  d480: 61 63 65 40 24 30 31 40 67 65 6f 64 65 40 40 53
 	  d490: 41 3f 41 56 3f 24 4e 61 6d 65 64 54 79 70 65 40
 	  d4a0: 56 3f 24 62 61 73 69 63 5f 73 74 72 69 6e 67 40
 	  d4b0: 44 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73 40
 	  d4c0: 44 40 73 74 64 40 40 56 3f 24 61 6c 6c 6f 63 61
 	  d4d0: 74 6f 72 40 44 40 32 40 40 73 74 64 40 40 55 4d
 	  d4e0: 65 73 68 54 79 70 65 54 61 67 40 67 65 6f 64 65
-	  d4f0: 40 40 40 32 40 58 5a 00 88 01 3f 3f 30 3f 24 54
+	  d4f0: 40 40 40 32 40 58 5a 00 86 01 3f 3f 30 3f 24 54
 	  d500: 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69 64 53
 	  d510: 63 61 6c 61 72 46 75 6e 63 74 69 6f 6e 40 24 30
 	  d520: 32 40 67 65 6f 64 65 40 40 51 45 41 41 40 24 24
-	  d530: 51 45 41 56 30 31 40 40 5a 00 39 02 3f 3f 31 3f
+	  d530: 51 45 41 56 30 31 40 40 5a 00 37 02 3f 3f 31 3f
 	  d540: 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69
 	  d550: 64 53 63 61 6c 61 72 46 75 6e 63 74 69 6f 6e 40
 	  d560: 24 30 32 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  d570: 58 5a 00 00 ec 03 3f 63 72 65 61 74 65 40 3f 24
+	  d570: 58 5a 00 00 ea 03 3f 63 72 65 61 74 65 40 3f 24
 	  d580: 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69 64
 	  d590: 53 63 61 6c 61 72 46 75 6e 63 74 69 6f 6e 40 24
 	  d5a0: 30 32 40 67 65 6f 64 65 40 40 53 41 3f 41 56 31
 	  d5b0: 32 40 41 45 42 56 3f 24 54 65 74 72 61 68 65 64
 	  d5c0: 72 61 6c 53 6f 6c 69 64 40 24 30 32 40 32 40 56
 	  d5d0: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  d5e0: 40 40 4e 40 5a 00 84 05 3f 66 69 6e 64 40 3f 24
+	  d5e0: 40 40 4e 40 5a 00 82 05 3f 66 69 6e 64 40 3f 24
 	  d5f0: 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c 69 64
 	  d600: 53 63 61 6c 61 72 46 75 6e 63 74 69 6f 6e 40 24
 	  d610: 30 32 40 67 65 6f 64 65 40 40 53 41 3f 41 56 31
 	  d620: 32 40 41 45 42 56 3f 24 54 65 74 72 61 68 65 64
 	  d630: 72 61 6c 53 6f 6c 69 64 40 24 30 32 40 32 40 56
 	  d640: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  d650: 40 40 40 5a 00 00 77 07 3f 73 65 74 5f 76 61 6c
+	  d650: 40 40 40 5a 00 00 71 07 3f 73 65 74 5f 76 61 6c
 	  d660: 75 65 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c
 	  d670: 53 6f 6c 69 64 53 63 61 6c 61 72 46 75 6e 63 74
 	  d680: 69 6f 6e 40 24 30 32 40 67 65 6f 64 65 40 40 51
-	  d690: 45 41 41 58 49 4e 40 5a 00 00 11 08 3f 76 61 6c
+	  d690: 45 41 41 58 49 4e 40 5a 00 00 0b 08 3f 76 61 6c
 	  d6a0: 75 65 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c
 	  d6b0: 53 6f 6c 69 64 53 63 61 6c 61 72 46 75 6e 63 74
 	  d6c0: 69 6f 6e 40 24 30 32 40 67 65 6f 64 65 40 40 51
-	  d6d0: 45 42 41 4e 49 40 5a 00 10 08 3f 76 61 6c 75 65
+	  d6d0: 45 42 41 4e 49 40 5a 00 0a 08 3f 76 61 6c 75 65
 	  d6e0: 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f
 	  d6f0: 6c 69 64 53 63 61 6c 61 72 46 75 6e 63 74 69 6f
 	  d700: 6e 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  d710: 41 4e 41 45 42 56 3f 24 50 6f 69 6e 74 40 24 30
-	  d720: 32 40 32 40 49 40 5a 00 16 00 3f 3f 24 63 72 65
+	  d720: 32 40 32 40 49 40 5a 00 14 00 3f 3f 24 63 72 65
 	  d730: 61 74 65 5f 61 61 62 62 5f 74 72 65 65 40 24 30
 	  d740: 32 40 67 65 6f 64 65 40 40 59 41 3f 41 56 3f 24
 	  d750: 41 41 42 42 54 72 65 65 40 24 30 32 40 30 40 41
 	  d760: 45 42 56 3f 24 53 6f 6c 69 64 4d 65 73 68 40 24
-	  d770: 30 32 40 30 40 40 5a 00 b3 02 3f 3f 52 3f 24 44
+	  d770: 30 32 40 30 40 40 5a 00 b1 02 3f 3f 52 3f 24 44
 	  d780: 69 73 74 61 6e 63 65 54 6f 54 65 74 72 61 68 65
 	  d790: 64 72 6f 6e 40 24 30 32 40 67 65 6f 64 65 40 40
 	  d7a0: 51 45 42 41 3f 41 56 3f 24 74 75 70 6c 65 40 4e
 	  d7b0: 56 3f 24 50 6f 69 6e 74 40 24 30 32 40 67 65 6f
 	  d7c0: 64 65 40 40 40 73 74 64 40 40 41 45 42 56 3f 24
 	  d7d0: 50 6f 69 6e 74 40 24 30 32 40 31 40 49 40 5a 00
-	  d7e0: ce 07 3f 74 79 70 65 5f 6e 61 6d 65 5f 73 74 61
+	  d7e0: c8 07 3f 74 79 70 65 5f 6e 61 6d 65 5f 73 74 61
 	  d7f0: 74 69 63 40 3f 24 54 65 74 72 61 68 65 64 72 61
 	  d800: 6c 53 6f 6c 69 64 40 24 30 32 40 67 65 6f 64 65
 	  d810: 40 40 53 41 3f 41 56 3f 24 4e 61 6d 65 64 54 79
 	  d820: 70 65 40 56 3f 24 62 61 73 69 63 5f 73 74 72 69
 	  d830: 6e 67 40 44 55 3f 24 63 68 61 72 5f 74 72 61 69
 	  d840: 74 73 40 44 40 73 74 64 40 40 56 3f 24 61 6c 6c
 	  d850: 6f 63 61 74 6f 72 40 44 40 32 40 40 73 74 64 40
 	  d860: 40 55 4d 65 73 68 54 79 70 65 54 61 67 40 67 65
-	  d870: 6f 64 65 40 40 40 32 40 58 5a 00 00 d4 01 3f 3f
+	  d870: 6f 64 65 40 40 40 32 40 58 5a 00 00 d2 01 3f 3f
 	  d880: 30 50 6f 6c 79 68 65 64 72 6f 6e 46 61 63 65 74
 	  d890: 40 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a 00
-	  d8a0: 82 01 3f 3f 30 3f 24 54 65 74 72 61 68 65 64 72
+	  d8a0: 80 01 3f 3f 30 3f 24 54 65 74 72 61 68 65 64 72
 	  d8b0: 61 6c 53 6f 6c 69 64 50 6f 69 6e 74 46 75 6e 63
 	  d8c0: 74 69 6f 6e 40 24 30 32 24 30 31 40 67 65 6f 64
 	  d8d0: 65 40 40 51 45 41 41 40 24 24 51 45 41 56 30 31
-	  d8e0: 40 40 5a 00 37 02 3f 3f 31 3f 24 54 65 74 72 61
+	  d8e0: 40 40 5a 00 35 02 3f 3f 31 3f 24 54 65 74 72 61
 	  d8f0: 68 65 64 72 61 6c 53 6f 6c 69 64 50 6f 69 6e 74
 	  d900: 46 75 6e 63 74 69 6f 6e 40 24 30 32 24 30 31 40
 	  d910: 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a 00 00
-	  d920: ea 03 3f 63 72 65 61 74 65 40 3f 24 54 65 74 72
+	  d920: e8 03 3f 63 72 65 61 74 65 40 3f 24 54 65 74 72
 	  d930: 61 68 65 64 72 61 6c 53 6f 6c 69 64 50 6f 69 6e
 	  d940: 74 46 75 6e 63 74 69 6f 6e 40 24 30 32 24 30 31
 	  d950: 40 67 65 6f 64 65 40 40 53 41 3f 41 56 31 32 40
 	  d960: 41 45 42 56 3f 24 54 65 74 72 61 68 65 64 72 61
 	  d970: 6c 53 6f 6c 69 64 40 24 30 32 40 32 40 56 73 74
 	  d980: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
 	  d990: 56 3f 24 50 6f 69 6e 74 40 24 30 31 40 32 40 40
-	  d9a0: 5a 00 82 05 3f 66 69 6e 64 40 3f 24 54 65 74 72
+	  d9a0: 5a 00 80 05 3f 66 69 6e 64 40 3f 24 54 65 74 72
 	  d9b0: 61 68 65 64 72 61 6c 53 6f 6c 69 64 50 6f 69 6e
 	  d9c0: 74 46 75 6e 63 74 69 6f 6e 40 24 30 32 24 30 31
 	  d9d0: 40 67 65 6f 64 65 40 40 53 41 3f 41 56 31 32 40
 	  d9e0: 41 45 42 56 3f 24 54 65 74 72 61 68 65 64 72 61
 	  d9f0: 6c 53 6f 6c 69 64 40 24 30 32 40 32 40 56 73 74
 	  da00: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
-	  da10: 40 5a 00 00 75 07 3f 73 65 74 5f 76 61 6c 75 65
+	  da10: 40 5a 00 00 6f 07 3f 73 65 74 5f 76 61 6c 75 65
 	  da20: 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f
 	  da30: 6c 69 64 50 6f 69 6e 74 46 75 6e 63 74 69 6f 6e
 	  da40: 40 24 30 32 24 30 31 40 67 65 6f 64 65 40 40 51
 	  da50: 45 41 41 58 49 56 3f 24 50 6f 69 6e 74 40 24 30
-	  da60: 31 40 32 40 40 5a 00 00 0d 08 3f 76 61 6c 75 65
+	  da60: 31 40 32 40 40 5a 00 00 07 08 3f 76 61 6c 75 65
 	  da70: 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f
 	  da80: 6c 69 64 50 6f 69 6e 74 46 75 6e 63 74 69 6f 6e
 	  da90: 40 24 30 32 24 30 31 40 67 65 6f 64 65 40 40 51
 	  daa0: 45 42 41 41 45 42 56 3f 24 50 6f 69 6e 74 40 24
-	  dab0: 30 31 40 32 40 49 40 5a 00 00 0c 08 3f 76 61 6c
+	  dab0: 30 31 40 32 40 49 40 5a 00 00 06 08 3f 76 61 6c
 	  dac0: 75 65 40 3f 24 54 65 74 72 61 68 65 64 72 61 6c
 	  dad0: 53 6f 6c 69 64 50 6f 69 6e 74 46 75 6e 63 74 69
 	  dae0: 6f 6e 40 24 30 32 24 30 31 40 67 65 6f 64 65 40
 	  daf0: 40 51 45 42 41 3f 41 56 3f 24 50 6f 69 6e 74 40
 	  db00: 24 30 31 40 32 40 41 45 42 56 3f 24 50 6f 69 6e
-	  db10: 74 40 24 30 32 40 32 40 49 40 5a 00 82 06 3f 6e
+	  db10: 74 40 24 30 32 40 32 40 49 40 5a 00 7c 06 3f 6e
 	  db20: 62 5f 70 6f 6c 79 68 65 64 72 6f 6e 5f 76 65 72
 	  db30: 74 69 63 65 73 40 3f 24 53 6f 6c 69 64 4d 65 73
 	  db40: 68 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
-	  db50: 41 45 49 40 5a 00 f1 06 3f 70 6f 6c 79 68 65 64
+	  db50: 41 45 49 40 5a 00 eb 06 3f 70 6f 6c 79 68 65 64
 	  db60: 72 6f 6e 5f 76 65 72 74 65 78 40 3f 24 53 6f 6c
 	  db70: 69 64 4d 65 73 68 40 24 30 32 40 67 65 6f 64 65
 	  db80: 40 40 51 45 42 41 49 41 45 42 55 50 6f 6c 79 68
 	  db90: 65 64 72 6f 6e 56 65 72 74 65 78 40 32 40 40 5a
-	  dba0: 00 00 7e 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 73
+	  dba0: 00 00 78 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 73
 	  dbb0: 40 3f 24 53 75 72 66 61 63 65 4d 65 73 68 40 24
 	  dbc0: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 49 58
-	  dbd0: 5a 00 7c 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 5f
+	  dbd0: 5a 00 76 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 5f
 	  dbe0: 76 65 72 74 69 63 65 73 40 3f 24 53 75 72 66 61
 	  dbf0: 63 65 4d 65 73 68 40 24 30 32 40 67 65 6f 64 65
-	  dc00: 40 40 51 45 42 41 45 49 40 5a 00 00 c6 06 3f 70
+	  dc00: 40 40 51 45 42 41 45 49 40 5a 00 00 c0 06 3f 70
 	  dc10: 6f 6c 79 67 6f 6e 5f 76 65 72 74 65 78 40 3f 24
 	  dc20: 53 75 72 66 61 63 65 4d 65 73 68 40 24 30 32 40
 	  dc30: 67 65 6f 64 65 40 40 51 45 42 41 49 41 45 42 55
 	  dc40: 50 6f 6c 79 67 6f 6e 56 65 72 74 65 78 40 32 40
-	  dc50: 40 5a 00 00 b6 06 3f 70 6f 6c 79 67 6f 6e 5f 61
+	  dc50: 40 5a 00 00 b0 06 3f 70 6f 6c 79 67 6f 6e 5f 61
 	  dc60: 74 74 72 69 62 75 74 65 5f 6d 61 6e 61 67 65 72
 	  dc70: 40 3f 24 53 75 72 66 61 63 65 4d 65 73 68 40 24
 	  dc80: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  dc90: 41 56 41 74 74 72 69 62 75 74 65 4d 61 6e 61 67
-	  dca0: 65 72 40 32 40 58 5a 00 60 03 3f 63 6c 6f 6e 65
+	  dca0: 65 72 40 32 40 58 5a 00 5e 03 3f 63 6c 6f 6e 65
 	  dcb0: 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53
 	  dcc0: 75 72 66 61 63 65 40 24 30 32 40 67 65 6f 64 65
 	  dcd0: 40 40 51 45 42 41 3f 41 56 3f 24 75 6e 69 71 75
 	  dce0: 65 5f 70 74 72 40 56 3f 24 54 72 69 61 6e 67 75
 	  dcf0: 6c 61 74 65 64 53 75 72 66 61 63 65 40 24 30 32
 	  dd00: 40 67 65 6f 64 65 40 40 55 3f 24 64 65 66 61 75
 	  dd10: 6c 74 5f 64 65 6c 65 74 65 40 56 3f 24 54 72 69
 	  dd20: 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63 65
 	  dd30: 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74 64
-	  dd40: 40 40 40 73 74 64 40 40 58 5a 00 00 e5 03 3f 63
+	  dd40: 40 40 40 73 74 64 40 40 58 5a 00 00 e3 03 3f 63
 	  dd50: 72 65 61 74 65 40 3f 24 53 75 72 66 61 63 65 4d
 	  dd60: 65 73 68 42 75 69 6c 64 65 72 40 24 30 32 40 67
 	  dd70: 65 6f 64 65 40 40 53 41 3f 41 56 3f 24 75 6e 69
 	  dd80: 71 75 65 5f 70 74 72 40 56 3f 24 53 75 72 66 61
 	  dd90: 63 65 4d 65 73 68 42 75 69 6c 64 65 72 40 24 30
 	  dda0: 32 40 67 65 6f 64 65 40 40 55 3f 24 64 65 66 61
 	  ddb0: 75 6c 74 5f 64 65 6c 65 74 65 40 56 3f 24 53 75
 	  ddc0: 72 66 61 63 65 4d 65 73 68 42 75 69 6c 64 65 72
 	  ddd0: 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74 64
 	  dde0: 40 40 40 73 74 64 40 40 41 45 41 56 3f 24 53 75
 	  ddf0: 72 66 61 63 65 4d 65 73 68 40 24 30 32 40 32 40
-	  de00: 40 5a 00 00 55 05 3f 65 64 67 65 5f 76 65 72 74
+	  de00: 40 5a 00 00 53 05 3f 65 64 67 65 5f 76 65 72 74
 	  de10: 65 78 40 47 72 61 70 68 40 67 65 6f 64 65 40 40
 	  de20: 51 45 42 41 49 41 45 42 55 45 64 67 65 56 65 72
-	  de30: 74 65 78 40 32 40 40 5a 00 00 59 05 3f 65 64 67
+	  de30: 74 65 78 40 32 40 40 5a 00 00 57 05 3f 65 64 67
 	  de40: 65 5f 76 65 72 74 69 63 65 73 40 47 72 61 70 68
 	  de50: 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56 3f
 	  de60: 24 61 72 72 61 79 40 49 24 30 31 40 73 74 64 40
-	  de70: 40 49 40 5a 00 00 3d 05 3f 65 64 67 65 5f 61 74
+	  de70: 40 49 40 5a 00 00 3b 05 3f 65 64 67 65 5f 61 74
 	  de80: 74 72 69 62 75 74 65 5f 6d 61 6e 61 67 65 72 40
 	  de90: 47 72 61 70 68 40 67 65 6f 64 65 40 40 51 45 42
 	  dea0: 41 41 45 41 56 41 74 74 72 69 62 75 74 65 4d 61
-	  deb0: 6e 61 67 65 72 40 32 40 58 5a 00 00 cf 01 3f 3f
+	  deb0: 6e 61 67 65 72 40 32 40 58 5a 00 00 cd 01 3f 3f
 	  dec0: 30 50 6f 6c 79 67 6f 6e 45 64 67 65 40 67 65 6f
-	  ded0: 64 65 40 40 51 45 41 41 40 58 5a 00 a6 01 3f 3f
+	  ded0: 64 65 40 40 51 45 41 41 40 58 5a 00 a4 01 3f 3f
 	  dee0: 30 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53
 	  def0: 75 72 66 61 63 65 50 6f 69 6e 74 46 75 6e 63 74
 	  df00: 69 6f 6e 40 24 30 31 24 30 30 40 67 65 6f 64 65
 	  df10: 40 40 51 45 41 41 40 24 24 51 45 41 56 30 31 40
-	  df20: 40 5a 00 00 47 02 3f 3f 31 3f 24 54 72 69 61 6e
+	  df20: 40 5a 00 00 45 02 3f 3f 31 3f 24 54 72 69 61 6e
 	  df30: 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 50 6f
 	  df40: 69 6e 74 46 75 6e 63 74 69 6f 6e 40 24 30 31 24
 	  df50: 30 30 40 67 65 6f 64 65 40 40 51 45 41 41 40 58
-	  df60: 5a 00 f3 03 3f 63 72 65 61 74 65 40 3f 24 54 72
+	  df60: 5a 00 f1 03 3f 63 72 65 61 74 65 40 3f 24 54 72
 	  df70: 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63
 	  df80: 65 50 6f 69 6e 74 46 75 6e 63 74 69 6f 6e 40 24
 	  df90: 30 31 24 30 30 40 67 65 6f 64 65 40 40 53 41 3f
 	  dfa0: 41 56 31 32 40 41 45 42 56 3f 24 54 72 69 61 6e
 	  dfb0: 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 40 24
 	  dfc0: 30 31 40 32 40 56 73 74 72 69 6e 67 5f 76 69 65
 	  dfd0: 77 40 61 62 73 6c 40 40 56 3f 24 50 6f 69 6e 74
-	  dfe0: 40 24 30 30 40 32 40 40 5a 00 85 05 3f 66 69 6e
+	  dfe0: 40 24 30 30 40 32 40 40 5a 00 83 05 3f 66 69 6e
 	  dff0: 64 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64
 	  e000: 53 75 72 66 61 63 65 50 6f 69 6e 74 46 75 6e 63
 	  e010: 74 69 6f 6e 40 24 30 31 24 30 30 40 67 65 6f 64
 	  e020: 65 40 40 53 41 3f 41 56 31 32 40 41 45 42 56 3f
 	  e030: 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72
 	  e040: 66 61 63 65 40 24 30 31 40 32 40 56 73 74 72 69
 	  e050: 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a
-	  e060: 00 00 78 07 3f 73 65 74 5f 76 61 6c 75 65 40 3f
+	  e060: 00 00 72 07 3f 73 65 74 5f 76 61 6c 75 65 40 3f
 	  e070: 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72
 	  e080: 66 61 63 65 50 6f 69 6e 74 46 75 6e 63 74 69 6f
 	  e090: 6e 40 24 30 31 24 30 30 40 67 65 6f 64 65 40 40
 	  e0a0: 51 45 41 41 58 49 56 3f 24 50 6f 69 6e 74 40 24
-	  e0b0: 30 30 40 32 40 40 5a 00 13 08 3f 76 61 6c 75 65
+	  e0b0: 30 30 40 32 40 40 5a 00 0d 08 3f 76 61 6c 75 65
 	  e0c0: 40 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53
 	  e0d0: 75 72 66 61 63 65 50 6f 69 6e 74 46 75 6e 63 74
 	  e0e0: 69 6f 6e 40 24 30 31 24 30 30 40 67 65 6f 64 65
 	  e0f0: 40 40 51 45 42 41 41 45 42 56 3f 24 50 6f 69 6e
-	  e100: 74 40 24 30 30 40 32 40 49 40 5a 00 12 08 3f 76
+	  e100: 74 40 24 30 30 40 32 40 49 40 5a 00 0c 08 3f 76
 	  e110: 61 6c 75 65 40 3f 24 54 72 69 61 6e 67 75 6c 61
 	  e120: 74 65 64 53 75 72 66 61 63 65 50 6f 69 6e 74 46
 	  e130: 75 6e 63 74 69 6f 6e 40 24 30 31 24 30 30 40 67
 	  e140: 65 6f 64 65 40 40 51 45 42 41 3f 41 56 3f 24 50
 	  e150: 6f 69 6e 74 40 24 30 30 40 32 40 41 45 42 56 3f
 	  e160: 24 50 6f 69 6e 74 40 24 30 31 40 32 40 49 40 5a
-	  e170: 00 00 7d 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 73
+	  e170: 00 00 77 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 73
 	  e180: 40 3f 24 53 75 72 66 61 63 65 4d 65 73 68 40 24
 	  e190: 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 49 58
-	  e1a0: 5a 00 7b 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 5f
+	  e1a0: 5a 00 75 06 3f 6e 62 5f 70 6f 6c 79 67 6f 6e 5f
 	  e1b0: 76 65 72 74 69 63 65 73 40 3f 24 53 75 72 66 61
 	  e1c0: 63 65 4d 65 73 68 40 24 30 31 40 67 65 6f 64 65
-	  e1d0: 40 40 51 45 42 41 45 49 40 5a 00 00 c5 06 3f 70
+	  e1d0: 40 40 51 45 42 41 45 49 40 5a 00 00 bf 06 3f 70
 	  e1e0: 6f 6c 79 67 6f 6e 5f 76 65 72 74 65 78 40 3f 24
 	  e1f0: 53 75 72 66 61 63 65 4d 65 73 68 40 24 30 31 40
 	  e200: 67 65 6f 64 65 40 40 51 45 42 41 49 41 45 42 55
 	  e210: 50 6f 6c 79 67 6f 6e 56 65 72 74 65 78 40 32 40
-	  e220: 40 5a 00 00 c7 06 3f 70 6f 6c 79 67 6f 6e 5f 76
+	  e220: 40 5a 00 00 c1 06 3f 70 6f 6c 79 67 6f 6e 5f 76
 	  e230: 65 72 74 69 63 65 73 40 3f 24 53 75 72 66 61 63
 	  e240: 65 4d 65 73 68 40 24 30 31 40 67 65 6f 64 65 40
 	  e250: 40 51 45 42 41 3f 41 56 3f 24 49 6e 6c 69 6e 65
 	  e260: 64 56 65 63 74 6f 72 40 49 24 30 32 56 3f 24 61
 	  e270: 6c 6c 6f 63 61 74 6f 72 40 49 40 73 74 64 40 40
-	  e280: 40 61 62 73 6c 40 40 49 40 5a 00 00 51 03 3f 63
+	  e280: 40 61 62 73 6c 40 40 49 40 5a 00 00 4f 03 3f 63
 	  e290: 6c 6f 6e 65 40 3f 24 45 64 67 65 64 43 75 72 76
 	  e2a0: 65 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42
 	  e2b0: 41 3f 41 56 3f 24 75 6e 69 71 75 65 5f 70 74 72
 	  e2c0: 40 56 3f 24 45 64 67 65 64 43 75 72 76 65 40 24
 	  e2d0: 30 31 40 67 65 6f 64 65 40 40 55 3f 24 64 65 66
 	  e2e0: 61 75 6c 74 5f 64 65 6c 65 74 65 40 56 3f 24 45
 	  e2f0: 64 67 65 64 43 75 72 76 65 40 24 30 31 40 67 65
 	  e300: 6f 64 65 40 40 40 73 74 64 40 40 40 73 74 64 40
-	  e310: 40 58 5a 00 bc 03 3f 63 72 65 61 74 65 40 3f 24
+	  e310: 40 58 5a 00 ba 03 3f 63 72 65 61 74 65 40 3f 24
 	  e320: 45 64 67 65 64 43 75 72 76 65 42 75 69 6c 64 65
 	  e330: 72 40 24 30 31 40 67 65 6f 64 65 40 40 53 41 3f
 	  e340: 41 56 3f 24 75 6e 69 71 75 65 5f 70 74 72 40 56
 	  e350: 3f 24 45 64 67 65 64 43 75 72 76 65 42 75 69 6c
 	  e360: 64 65 72 40 24 30 31 40 67 65 6f 64 65 40 40 55
 	  e370: 3f 24 64 65 66 61 75 6c 74 5f 64 65 6c 65 74 65
 	  e380: 40 56 3f 24 45 64 67 65 64 43 75 72 76 65 42 75
@@ -106326,19 +106326,17 @@
    18004df73:	addb   $0x0,(%rcx)
    18004df76:	add    %al,(%rax)
    18004df78:	subb   $0x7,(%rbx)
    18004df7b:	addb   $0x0,(%rcx)
    18004df7e:	add    %al,(%rax)
    18004df80:	add    %al,(%rax)
    18004df82:	add    %al,(%rax)
-   18004df84:	sar    %cl,%eax
-   18004df86:	lods   %ds:(%rsi),%eax
-   18004df87:	add    %al,%fs:(%rax)
-   18004df8a:	add    %al,(%rax)
-   18004df8c:	or     $0x3c000000,%eax
+   18004df84:	xchg   %eax,%ebx
+   18004df85:	sbb    0x64(%rbp),%ebp
+   18004df8b:	add    %cl,0x3c000000(%rip)        # 0x1bc04df91
    18004df91:	add    (%rax),%eax
    18004df93:	add    %ch,0x5(%rbp,%rdi,1)
    18004df97:	add    %ch,0x5(%rbp,%rbp,1)
    18004df9b:	add    %al,(%rax)
    18004df9d:	add    %al,(%rax)
    18004df9f:	add    %bh,(%rax)
    18004dfa1:	add    %eax,(%rax)
@@ -146830,16 +146828,15 @@
    18006726f:	outsl  %gs:(%rsi),(%dx)
    180067271:	fs gs pop %rdi
    180067274:	insl   (%dx),%es:(%rdi)
    180067275:	outsl  %ds:(%rsi),(%dx)
    180067276:	fs gs insb (%dx),%es:(%rdi)
    180067279:	cs fs insb (%dx),%es:(%rdi)
    18006727c:	insb   (%dx),%es:(%rdi)
-   18006727d:	add    %dh,0x6(%rdx)
-   180067280:	(bad)
+   18006727d:	add    %ch,0x3f(%rsi,%rax,1)
    180067281:	outsb  %ds:(%rsi),(%dx)
    180067282:	(bad)
    180067283:	pop    %rdi
    180067284:	gs fs addr32 gs jae 0x1800672ca
    18006728a:	rex.RXB jb 0x1800672ee
    18006728d:	jo     0x1800672f7
    18006728f:	rex
@@ -146848,15 +146845,15 @@
    180067296:	rex push %rcx
    180067298:	rex.RB
    180067299:	rex.X
    18006729a:	rex.B
    18006729b:	rex.WB pop %r8
    18006729d:	pop    %rdx
    18006729e:	add    %al,(%rax)
-   1800672a0:	(bad)
+   1800672a0:	pop    %rdi
    1800672a1:	add    $0x6764653f,%eax
    1800672a6:	gs jae 0x180067308
    1800672a9:	(bad)
    1800672aa:	jb     0x18006731b
    1800672ac:	jne    0x18006731c
    1800672ae:	fs pop %rdi
    1800672b0:	jbe    0x180067317
@@ -146909,15 +146906,15 @@
    180067315:	fs rex
    180067317:	rex
    180067318:	rex (bad)
    18006731a:	(bad)
    18006731f:	rex.WB
    180067320:	rex pop %rdx
    180067322:	add    %al,(%rax)
-   180067324:	cld
+   180067324:	cli
    180067325:	add    (%rdi),%edi
    180067327:	movsxd 0x65(%rdx),%esi
    18006732a:	(bad)
    18006732b:	je     0x180067392
    18006732d:	rex
    18006732e:	rex.RXB jb 0x180067392
    180067331:	jo     0x18006739b
@@ -146969,15 +146966,15 @@
    18006739d:	rex.RB
    18006739e:	push   %r14
    1800673a0:	rex.RXB jb 0x180067404
    1800673a3:	jo     0x18006740d
    1800673a5:	rex xor 0x40(%rax),%al
    1800673a9:	pop    %rdx
    1800673aa:	add    %al,(%rax)
-   1800673ac:	sub    (%rdi,%rdi,1),%eax
+   1800673ac:	sub    %eax,(%rdi,%rdi,1)
    1800673af:	fs gs insb (%dx),%es:(%rdi)
    1800673b2:	gs je  0x18006741a
    1800673b5:	pop    %rdi
    1800673b6:	gs fs addr32 gs jae 0x1800673fc
    1800673bc:	rex.RXB jb 0x180067420
    1800673bf:	jo     0x180067429
    1800673c1:	rex.X jne 0x18006742d
@@ -147030,16 +147027,15 @@
    180067418:	rex.WRX
    180067419:	rex jae 0x180067490
    18006741c:	fs rex
    18006741e:	rex
    18006741f:	rex xor $0x40,%al
    180067422:	rex pop %rdx
    180067424:	add    %al,(%rax)
-   180067426:	mov    %eax,(%rsi)
-   180067428:	(bad)
+   180067426:	addl   $0x3f,(%rsi)
    180067429:	outsb  %ds:(%rsi),(%dx)
    18006742a:	(bad)
    18006742b:	pop    %rdi
    18006742c:	jbe    0x180067493
    18006742e:	jb     0x1800674a4
    180067430:	imul   $0x65564073,0x65(%rbx),%esp
    180067437:	jb     0x1800674ad
@@ -147049,15 +147045,15 @@
    180067442:	fs gs rex
    180067445:	rex push %rcx
    180067447:	rex.RB
    180067448:	rex.X
    180067449:	rex.B
    18006744a:	rex.WB pop %r8
    18006744c:	pop    %rdx
-   18006744d:	add    %ah,(%rax)
+   18006744d:	add    %bl,(%rdx)
    18006744f:	or     %bh,(%rdi)
    180067451:	jbe    0x1800674b8
    180067453:	jb     0x1800674c9
    180067455:	gs js  0x1800674b7
    180067458:	(bad)
    180067459:	je     0x1800674cf
    18006745b:	jb     0x1800674c6
@@ -147086,15 +147082,15 @@
    18006748d:	(bad)
    18006748e:	outsb  %ds:(%rsi),(%dx)
    18006748f:	(bad)
    180067490:	addr32 gs jb 0x1800674d4
    180067494:	xor    0x58(%rax),%al
    180067497:	pop    %rdx
    180067498:	add    %al,(%rax)
-   18006749a:	stos   %eax,%es:(%rdi)
+   18006749a:	movsl  %ds:(%rsi),%es:(%rdi)
    18006749b:	(bad)
    18006749c:	(bad)
    18006749d:	jo     0x18006750e
    18006749f:	imul   $0x43243f40,0x74(%rsi),%ebp
    1800674a6:	outsl  %ds:(%rsi),(%dx)
    1800674a7:	outsl  %ds:(%rsi),(%dx)
    1800674a8:	jb     0x18006750e
@@ -147122,19 +147118,16 @@
    1800674d8:	rex.X push %rsi
    1800674da:	(bad)
    1800674db:	and    $0x50,%al
    1800674dd:	outsl  %ds:(%rsi),(%dx)
    1800674de:	imul   $0x31302440,0x74(%rsi),%ebp
    1800674e5:	rex xor 0x49(%rax),%al
    1800674e9:	rex pop %rdx
-   1800674eb:	add    %ch,0x696f703f(%rsi,%rax,1)
-   1800674f2:	outsb  %ds:(%rsi),(%dx)
-   1800674f3:	je     0x180067535
-   1800674f5:	(bad)
-   1800674f6:	and    $0x43,%al
+   1800674eb:	add    %ah,0x6f703f06(%rsi)
+   1800674f1:	imul   $0x43243f40,0x74(%rsi),%ebp
    1800674f8:	outsl  %ds:(%rsi),(%dx)
    1800674f9:	outsl  %ds:(%rsi),(%dx)
    1800674fa:	jb     0x180067560
    1800674fc:	imul   $0x65526574,0x61(%rsi),%ebp
    180067503:	data16 gs jb 0x18006756c
    180067507:	outsb  %ds:(%rsi),(%dx)
    180067508:	movsxd 0x53(%rbp),%esp
@@ -147158,15 +147151,15 @@
    18006752a:	rex.X push %rsi
    18006752c:	(bad)
    18006752d:	and    $0x50,%al
    18006752f:	outsl  %ds:(%rsi),(%dx)
    180067530:	imul   $0x32302440,0x74(%rsi),%ebp
    180067537:	rex xor 0x49(%rax),%al
    18006753b:	rex pop %rdx
-   18006753d:	add    %bh,0x6(%rdi)
+   18006753d:	add    %bh,0x6(%rcx)
    180067540:	(bad)
    180067541:	outsb  %ds:(%rsi),(%dx)
    180067542:	(bad)
    180067543:	pop    %rdi
    180067544:	jo     0x1800675b5
    180067546:	insb   (%dx),%es:(%rdi)
    180067547:	jns    0x1800675b1
@@ -147183,15 +147176,15 @@
    180067564:	rex push %rcx
    180067566:	rex.RB
    180067567:	rex.X
    180067568:	rex.B
    180067569:	rex.WB pop %r8
    18006756b:	pop    %rdx
    18006756c:	add    %al,(%rax)
-   18006756e:	hlt
+   18006756e:	out    %al,(%dx)
    18006756f:	(bad)
    180067570:	(bad)
    180067571:	jo     0x1800675e2
    180067573:	insb   (%dx),%es:(%rdi)
    180067574:	jns    0x1800675de
    180067576:	gs fs jb 0x1800675e9
    18006757a:	outsb  %ds:(%rsi),(%dx)
@@ -147232,15 +147225,15 @@
    1800675c5:	rex jae 0x18006763c
    1800675c8:	fs rex
    1800675ca:	rex
    1800675cb:	rex (bad)
    1800675cd:	(bad)
    1800675d2:	rex.WB
    1800675d3:	rex pop %rdx
-   1800675d5:	add    %bl,0x3(%rdi)
+   1800675d5:	add    %bl,0x3(%rbp)
    1800675d8:	(bad)
    1800675d9:	movsxd 0x6e(%rdi,%rbp,2),%ebp
    1800675dd:	gs rex (bad)
    1800675e0:	and    $0x54,%al
    1800675e2:	jb     0x18006764d
    1800675e4:	(bad)
    1800675e5:	outsb  %ds:(%rsi),(%dx)
@@ -147312,15 +147305,15 @@
    18006766d:	fs rex
    18006766f:	rex
    180067670:	rex jae 0x1800676e7
    180067673:	fs rex
    180067675:	rex pop %rax
    180067677:	pop    %rdx
    180067678:	add    %al,(%rax)
-   18006767a:	rex.WRXB (bad)
+   18006767a:	rex.WB (bad)
    18006767c:	(bad)
    18006767d:	jae    0x1800676e4
    18006767f:	je     0x1800676e0
    180067681:	jo     0x1800676f2
    180067683:	imul   $0x43243f40,0x74(%rsi),%ebp
    18006768a:	outsl  %ds:(%rsi),(%dx)
    18006768b:	outsl  %ds:(%rsi),(%dx)
@@ -147351,15 +147344,15 @@
    1800676c4:	(bad)
    1800676c5:	and    $0x50,%al
    1800676c7:	outsl  %ds:(%rsi),(%dx)
    1800676c8:	imul   $0x31302440,0x74(%rsi),%ebp
    1800676cf:	rex xor 0x40(%rax),%al
    1800676d3:	pop    %rdx
    1800676d4:	add    %al,(%rax)
-   1800676d6:	int1
+   1800676d6:	out    %eax,(%dx)
    1800676d7:	add    (%rdi),%edi
    1800676d9:	movsxd 0x65(%rdx),%esi
    1800676dc:	(bad)
    1800676dd:	je     0x180067744
    1800676df:	rex (bad)
    1800676e1:	and    $0x54,%al
    1800676e3:	jb     0x18006774e
@@ -147458,15 +147451,15 @@
    18006779f:	data16 (bad)
    1800677a1:	movsxd 0x40(%rbp),%esp
    1800677a4:	and    $0x30,%al
    1800677a6:	xor    %eax,0x32(%rax)
    1800677a9:	rex
    1800677aa:	rex pop %rdx
    1800677ac:	add    %al,(%rax)
-   1800677ae:	push   %rsp
+   1800677ae:	push   %rdx
    1800677af:	add    %bh,(%rdi)
    1800677b1:	(bad)
    1800677b2:	and    $0x73,%al
    1800677b4:	(bad)
    1800677b5:	jbe    0x18006781c
    1800677b7:	pop    %rdi
    1800677b8:	je     0x18006782c
@@ -147507,15 +147500,15 @@
    180067801:	addr32 pop %rdi
    180067803:	jbe    0x18006786e
    180067805:	gs ja  0x180067848
    180067808:	(bad)
    180067809:	(bad)
    18006780e:	rex pop %rdx
    180067810:	add    %al,(%rax)
-   180067812:	pop    %rsi
+   180067812:	pop    %rsp
    180067813:	add    (%rdi),%edi
    180067815:	movsxd 0x6e(%rdi,%rbp,2),%ebp
    180067819:	gs rex (bad)
    18006781c:	and    $0x54,%al
    18006781e:	gs je  0x180067893
    180067821:	(bad)
    180067822:	push   $0x61726465
@@ -147574,15 +147567,15 @@
    18006789d:	rex jae 0x180067914
    1800678a0:	fs rex
    1800678a2:	rex
    1800678a3:	rex jae 0x18006791a
    1800678a6:	fs rex
    1800678a8:	rex pop %rax
    1800678aa:	pop    %rdx
-   1800678ab:	add    %dl,0x7(%rax)
+   1800678ab:	add    %cl,0x7(%rdx)
    1800678ae:	(bad)
    1800678af:	jae    0x180067916
    1800678b1:	je     0x180067912
    1800678b3:	jo     0x180067924
    1800678b5:	imul   $0x43243f40,0x74(%rsi),%ebp
    1800678bc:	outsl  %ds:(%rsi),(%dx)
    1800678bd:	outsl  %ds:(%rsi),(%dx)
@@ -147613,16 +147606,18 @@
    1800678f6:	(bad)
    1800678f7:	and    $0x50,%al
    1800678f9:	outsl  %ds:(%rsi),(%dx)
    1800678fa:	imul   $0x32302440,0x74(%rsi),%ebp
    180067901:	rex xor 0x40(%rax),%al
    180067905:	pop    %rdx
    180067906:	add    %al,(%rax)
-   180067908:	call   0x1f269b810
-   18006790d:	gs (bad)
+   180067908:	out    %al,$0x3
+   18006790a:	(bad)
+   18006790b:	movsxd 0x65(%rdx),%esi
+   18006790e:	(bad)
    18006790f:	je     0x180067976
    180067911:	rex (bad)
    180067913:	and    $0x54,%al
    180067915:	gs je  0x18006798a
    180067918:	(bad)
    180067919:	push   $0x61726465
    18006791e:	insb   (%dx),%es:(%rdi)
@@ -147702,15 +147697,15 @@
    1800679c4:	push   %rbx
    1800679c5:	outsl  %ds:(%rsi),(%dx)
    1800679c6:	insb   (%dx),%es:(%rdi)
    1800679c7:	imul   $0x32403230,0x24(%rax,%rax,2),%esp
    1800679cf:	rex
    1800679d0:	rex pop %rdx
    1800679d2:	add    %al,(%rax)
-   1800679d4:	push   %rbx
+   1800679d4:	push   %rcx
    1800679d5:	add    %bh,(%rdi)
    1800679d7:	(bad)
    1800679d8:	and    $0x73,%al
    1800679da:	(bad)
    1800679db:	jbe    0x180067a42
    1800679dd:	pop    %rdi
    1800679de:	je     0x180067a45
@@ -147746,15 +147741,15 @@
    180067a21:	addr32 pop %rdi
    180067a23:	jbe    0x180067a8e
    180067a25:	gs ja  0x180067a68
    180067a28:	(bad)
    180067a29:	(bad)
    180067a2e:	rex pop %rdx
    180067a30:	add    %al,(%rax)
-   180067a32:	mov    $0x1,%ch
+   180067a32:	mov    $0x1,%bl
    180067a34:	(bad)
    180067a35:	(bad)
    180067a36:	xor    %bh,(%rdi)
    180067a38:	and    $0x54,%al
    180067a3a:	jb     0x180067aa5
    180067a3c:	(bad)
    180067a3d:	outsb  %ds:(%rsi),(%dx)
@@ -147783,15 +147778,15 @@
    180067a6d:	push   %rcx
    180067a6e:	rex.RB
    180067a6f:	push   %r14
    180067a71:	xor    %dh,(%rcx)
    180067a73:	rex
    180067a74:	rex pop %rdx
    180067a76:	add    %al,(%rax)
-   180067a78:	rex.WR add (%rdi),%r15b
+   180067a78:	rex.WX add (%rdi),%dil
    180067a7b:	(bad)
    180067a7c:	xor    %edi,(%rdi)
    180067a7e:	and    $0x54,%al
    180067a80:	jb     0x180067aeb
    180067a82:	(bad)
    180067a83:	outsb  %ds:(%rsi),(%dx)
    180067a84:	addr32 jne 0x180067af3
@@ -147813,15 +147808,15 @@
    180067aa8:	fs gs rex
    180067aab:	rex push %rcx
    180067aad:	rex.RB
    180067aae:	rex.B
    180067aaf:	rex.B
    180067ab0:	rex pop %rax
    180067ab2:	pop    %rdx
-   180067ab3:	add    %bh,%al
+   180067ab3:	add    %dh,%dh
    180067ab5:	add    (%rdi),%edi
    180067ab7:	movsxd 0x65(%rdx),%esi
    180067aba:	(bad)
    180067abb:	je     0x180067b22
    180067abd:	rex (bad)
    180067abf:	and    $0x54,%al
    180067ac1:	jb     0x180067b2c
@@ -147873,15 +147868,15 @@
    180067b1b:	addr32 pop %rdi
    180067b1d:	jbe    0x180067b88
    180067b1f:	gs ja  0x180067b62
    180067b22:	(bad)
    180067b23:	(bad)
    180067b28:	rex.WRX
    180067b29:	rex pop %rdx
-   180067b2b:	add    %cl,0x69663f05(%rdx)
+   180067b2b:	add    %cl,0x69663f05(%rax)
    180067b31:	outsb  %ds:(%rsi),(%dx)
    180067b32:	fs rex (bad)
    180067b35:	and    $0x54,%al
    180067b37:	jb     0x180067ba2
    180067b39:	(bad)
    180067b3a:	outsb  %ds:(%rsi),(%dx)
    180067b3b:	addr32 jne 0x180067baa
@@ -147930,15 +147925,15 @@
    180067b91:	addr32 pop %rdi
    180067b93:	jbe    0x180067bfe
    180067b95:	gs ja  0x180067bd8
    180067b98:	(bad)
    180067b99:	(bad)
    180067b9e:	rex pop %rdx
    180067ba0:	add    %al,(%rax)
-   180067ba2:	jge    0x180067bab
+   180067ba2:	ja     0x180067bab
    180067ba4:	(bad)
    180067ba5:	jae    0x180067c0c
    180067ba7:	je     0x180067c08
    180067ba9:	jbe    0x180067c0c
    180067bab:	insb   (%dx),%es:(%rdi)
    180067bac:	jne    0x180067c13
    180067bae:	rex (bad)
@@ -147966,15 +147961,17 @@
    180067bdd:	rex push %rcx
    180067bdf:	rex.RB
    180067be0:	rex.B
    180067be1:	pop    %r8
    180067be3:	rex.WB
    180067be4:	rex.WRX
    180067be5:	rex pop %rdx
-   180067be7:	add    %bl,0x61763f08(%rip)        # 0x1e17cbaf5
+   180067be7:	add    %dl,(%rdi)
+   180067be9:	or     %bh,(%rdi)
+   180067beb:	jbe    0x180067c4e
    180067bed:	insb   (%dx),%es:(%rdi)
    180067bee:	jne    0x180067c55
    180067bf0:	rex (bad)
    180067bf2:	and    $0x54,%al
    180067bf4:	jb     0x180067c5f
    180067bf6:	(bad)
    180067bf7:	outsb  %ds:(%rsi),(%dx)
@@ -147999,16 +147996,16 @@
    180067c21:	rex.RB
    180067c22:	rex.X
    180067c23:	rex.B
    180067c24:	rex.WRX
    180067c25:	rex.WB
    180067c26:	rex pop %rdx
    180067c28:	add    %al,(%rax)
-   180067c2a:	sbb    $0x8,%al
-   180067c2c:	(bad)
+   180067c2a:	(bad)
+   180067c2b:	or     %bh,(%rdi)
    180067c2d:	jbe    0x180067c90
    180067c2f:	insb   (%dx),%es:(%rdi)
    180067c30:	jne    0x180067c97
    180067c32:	rex (bad)
    180067c34:	and    $0x54,%al
    180067c36:	jb     0x180067ca1
    180067c38:	(bad)
@@ -148041,15 +148038,15 @@
    180067c6b:	(bad)
    180067c6c:	and    $0x50,%al
    180067c6e:	outsl  %ds:(%rsi),(%dx)
    180067c6f:	imul   $0x31302440,0x74(%rsi),%ebp
    180067c76:	rex xor 0x49(%rax),%al
    180067c7a:	rex pop %rdx
    180067c7c:	add    %al,(%rax)
-   180067c7e:	adc    $0x0,%al
+   180067c7e:	adc    (%rax),%al
    180067c80:	(bad)
    180067c81:	(bad)
    180067c82:	and    $0x63,%al
    180067c84:	jb     0x180067ceb
    180067c86:	(bad)
    180067c87:	je     0x180067cee
    180067c89:	pop    %rdi
@@ -148081,15 +148078,16 @@
    180067cbe:	data16 (bad)
    180067cc0:	movsxd 0x4d(%rbp),%esp
    180067cc3:	gs jae 0x180067d2e
    180067cc6:	rex and $0x30,%al
    180067cc9:	xor    %eax,0x30(%rax)
    180067ccc:	rex
    180067ccd:	rex pop %rdx
-   180067ccf:	add    %dh,0x3f523f3f(%rdx,%rax,1)
+   180067ccf:	add    %dh,0x523f3f02(%rdx)
+   180067cd5:	(bad)
    180067cd6:	and    $0x44,%al
    180067cd8:	imul   $0x65636e61,0x74(%rbx),%esi
    180067cdf:	push   %rsp
    180067ce0:	outsl  %ds:(%rsi),(%dx)
    180067ce1:	push   %rsp
    180067ce2:	jb     0x180067d4d
    180067ce4:	(bad)
@@ -148127,15 +148125,15 @@
    180067d23:	(bad)
    180067d24:	and    $0x50,%al
    180067d26:	outsl  %ds:(%rsi),(%dx)
    180067d27:	imul   $0x31302440,0x74(%rsi),%ebp
    180067d2e:	rex xor %eax,0x49(%rax)
    180067d32:	rex pop %rdx
    180067d34:	add    %al,(%rax)
-   180067d36:	iret
+   180067d36:	leave
    180067d37:	(bad)
    180067d38:	(bad)
    180067d39:	je     0x180067db4
    180067d3b:	jo     0x180067da2
    180067d3d:	pop    %rdi
    180067d3e:	outsb  %ds:(%rsi),(%dx)
    180067d3f:	(bad)
@@ -148204,15 +148202,15 @@
    180067dc4:	(bad)
    180067dc5:	addr32 rex
    180067dc7:	outsl  %gs:(%esi),(%dx)
    180067dca:	fs gs rex
    180067dcd:	rex
    180067dce:	rex xor 0x58(%rax),%al
    180067dd2:	pop    %rdx
-   180067dd3:	add    %cl,0x303f3f01(%rax)
+   180067dd3:	add    %al,0x303f3f01(%rsi)
    180067dd9:	(bad)
    180067dda:	and    $0x54,%al
    180067ddc:	gs je  0x180067e51
    180067ddf:	(bad)
    180067de0:	push   $0x61726465
    180067de5:	insb   (%dx),%es:(%rdi)
    180067de6:	push   %rbx
@@ -148233,15 +148231,15 @@
    180067e09:	rex and $0x24,%al
    180067e0c:	push   %rcx
    180067e0d:	rex.RB
    180067e0e:	push   %r14
    180067e10:	xor    %dh,(%rcx)
    180067e12:	rex
    180067e13:	rex pop %rdx
-   180067e15:	add    %bh,(%rcx)
+   180067e15:	add    %dh,(%rdi)
    180067e17:	add    (%rdi),%bh
    180067e19:	(bad)
    180067e1a:	xor    %edi,(%rdi)
    180067e1c:	and    $0x54,%al
    180067e1e:	gs je  0x180067e93
    180067e21:	(bad)
    180067e22:	push   $0x61726465
@@ -148260,15 +148258,15 @@
    180067e46:	rex push %rcx
    180067e48:	rex.RB
    180067e49:	rex.B
    180067e4a:	rex.B
    180067e4b:	rex pop %rax
    180067e4d:	pop    %rdx
    180067e4e:	add    %al,(%rax)
-   180067e50:	in     (%dx),%al
+   180067e50:	(bad)
    180067e51:	add    (%rdi),%edi
    180067e53:	movsxd 0x65(%rdx),%esi
    180067e56:	(bad)
    180067e57:	je     0x180067ebe
    180067e59:	rex (bad)
    180067e5b:	and    $0x54,%al
    180067e5d:	gs je  0x180067ed2
@@ -148311,15 +148309,16 @@
    180067eb1:	addr32 pop %rdi
    180067eb3:	jbe    0x180067f1e
    180067eb5:	gs ja  0x180067ef8
    180067eb8:	(bad)
    180067eb9:	(bad)
    180067ebe:	rex.WRX
    180067ebf:	rex pop %rdx
-   180067ec1:	add    %al,0x6e69663f(%rbp,%rax,1)
+   180067ec1:	add    %al,0x69663f05(%rdx)
+   180067ec7:	outsb  %ds:(%rsi),(%dx)
    180067ec8:	fs rex (bad)
    180067ecb:	and    $0x54,%al
    180067ecd:	gs je  0x180067f42
    180067ed0:	(bad)
    180067ed1:	push   $0x61726465
    180067ed6:	insb   (%dx),%es:(%rdi)
    180067ed7:	push   %rbx
@@ -148358,15 +148357,15 @@
    180067f21:	addr32 pop %rdi
    180067f23:	jbe    0x180067f8e
    180067f25:	gs ja  0x180067f68
    180067f28:	(bad)
    180067f29:	(bad)
    180067f2e:	rex pop %rdx
    180067f30:	add    %al,(%rax)
-   180067f32:	ja     0x180067f3b
+   180067f32:	jno    0x180067f3b
    180067f34:	(bad)
    180067f35:	jae    0x180067f9c
    180067f37:	je     0x180067f98
    180067f39:	jbe    0x180067f9c
    180067f3b:	insb   (%dx),%es:(%rdi)
    180067f3c:	jne    0x180067fa3
    180067f3e:	rex (bad)
@@ -148390,15 +148389,15 @@
    180067f6c:	rex.RB
    180067f6d:	rex.B
    180067f6e:	pop    %r8
    180067f70:	rex.WB
    180067f71:	rex.WRX
    180067f72:	rex pop %rdx
    180067f74:	add    %al,(%rax)
-   180067f76:	adc    %ecx,(%rax)
+   180067f76:	or     (%rax),%ecx
    180067f78:	(bad)
    180067f79:	jbe    0x180067fdc
    180067f7b:	insb   (%dx),%es:(%rdi)
    180067f7c:	jne    0x180067fe3
    180067f7e:	rex (bad)
    180067f80:	and    $0x54,%al
    180067f82:	gs je  0x180067ff7
@@ -148419,15 +148418,15 @@
    180067faa:	rex push %rcx
    180067fac:	rex.RB
    180067fad:	rex.X
    180067fae:	rex.B
    180067faf:	rex.WRX
    180067fb0:	rex.WB
    180067fb1:	rex pop %rdx
-   180067fb3:	add    %dl,(%rax)
+   180067fb3:	add    %cl,(%rdx)
    180067fb5:	or     %bh,(%rdi)
    180067fb7:	jbe    0x18006801a
    180067fb9:	insb   (%dx),%es:(%rdi)
    180067fba:	jne    0x180068021
    180067fbc:	rex (bad)
    180067fbe:	and    $0x54,%al
    180067fc0:	gs je  0x180068035
@@ -148455,16 +148454,16 @@
    180067ff0:	rex.X push %rsi
    180067ff2:	(bad)
    180067ff3:	and    $0x50,%al
    180067ff5:	outsl  %ds:(%rsi),(%dx)
    180067ff6:	imul   $0x32302440,0x74(%rsi),%ebp
    180067ffd:	rex xor 0x49(%rax),%al
    180068001:	rex pop %rdx
-   180068003:	add    %dl,(%rsi)
-   180068005:	add    %bh,(%rdi)
+   180068003:	add    %dl,(%rax,%rax,1)
+   180068006:	(bad)
    180068007:	(bad)
    180068008:	and    $0x63,%al
    18006800a:	jb     0x180068071
    18006800c:	(bad)
    18006800d:	je     0x180068074
    18006800f:	pop    %rdi
    180068010:	(bad)
@@ -148493,15 +148492,15 @@
    180068040:	and    $0x53,%al
    180068042:	outsl  %ds:(%rsi),(%dx)
    180068043:	insb   (%dx),%es:(%rdi)
    180068044:	imul   $0x24406873,0x65(%rbp,%rcx,2),%esp
    18006804c:	xor    %dh,(%rdx)
    18006804e:	rex xor %al,0x40(%rax)
    180068052:	pop    %rdx
-   180068053:	add    %dh,0x523f3f02(%rbx)
+   180068053:	add    %dh,0x523f3f02(%rcx)
    180068059:	(bad)
    18006805a:	and    $0x44,%al
    18006805c:	imul   $0x65636e61,0x74(%rbx),%esi
    180068063:	push   %rsp
    180068064:	outsl  %ds:(%rsi),(%dx)
    180068065:	push   %rsp
    180068066:	gs je  0x1800680db
@@ -148539,15 +148538,15 @@
    1800680a8:	rex.X push %rsi
    1800680aa:	(bad)
    1800680ab:	and    $0x50,%al
    1800680ad:	outsl  %ds:(%rsi),(%dx)
    1800680ae:	imul   $0x32302440,0x74(%rsi),%ebp
    1800680b5:	rex xor %eax,0x49(%rax)
    1800680b9:	rex pop %rdx
-   1800680bb:	add    %cl,%dh
+   1800680bb:	add    %cl,%al
    1800680bd:	(bad)
    1800680be:	(bad)
    1800680bf:	je     0x18006813a
    1800680c1:	jo     0x180068128
    1800680c3:	pop    %rdi
    1800680c4:	outsb  %ds:(%rsi),(%dx)
    1800680c5:	(bad)
@@ -148613,16 +148612,16 @@
    180068148:	addr32 rex
    18006814a:	outsl  %gs:(%esi),(%dx)
    18006814d:	fs gs rex
    180068150:	rex
    180068151:	rex xor 0x58(%rax),%al
    180068155:	pop    %rdx
    180068156:	add    %al,(%rax)
-   180068158:	(bad)
-   180068159:	add    %edi,(%rdi)
+   180068158:	rolb   %cl,(%rcx)
+   18006815a:	(bad)
    18006815b:	(bad)
    18006815c:	xor    %dl,0x6f(%rax)
    18006815f:	insb   (%dx),%es:(%rdi)
    180068160:	jns    0x1800681ca
    180068162:	gs fs jb 0x1800681d5
    180068166:	outsb  %ds:(%rsi),(%dx)
    180068167:	rex.RX (bad)
@@ -148632,15 +148631,15 @@
    180068170:	fs gs rex
    180068173:	rex push %rcx
    180068175:	rex.RB
    180068176:	rex.B
    180068177:	rex.B
    180068178:	rex pop %rax
    18006817a:	pop    %rdx
-   18006817b:	add    %al,0x303f3f01(%rdx)
+   18006817b:	add    %al,0x303f3f01(%rax)
    180068181:	(bad)
    180068182:	and    $0x54,%al
    180068184:	gs je  0x1800681f9
    180068187:	(bad)
    180068188:	push   $0x61726465
    18006818d:	insb   (%dx),%es:(%rdi)
    18006818e:	push   %rbx
@@ -148662,18 +148661,16 @@
    1800681b3:	rex and $0x24,%al
    1800681b6:	push   %rcx
    1800681b7:	rex.RB
    1800681b8:	push   %r14
    1800681ba:	xor    %dh,(%rcx)
    1800681bc:	rex
    1800681bd:	rex pop %rdx
-   1800681bf:	add    %dh,(%rdi)
-   1800681c1:	add    (%rdi),%bh
-   1800681c3:	(bad)
-   1800681c4:	xor    %edi,(%rdi)
+   1800681bf:	add    %dh,0x313f3f02(%rip)        # 0x1b145c0c7
+   1800681c5:	(bad)
    1800681c6:	and    $0x54,%al
    1800681c8:	gs je  0x18006823d
    1800681cb:	(bad)
    1800681cc:	push   $0x61726465
    1800681d1:	insb   (%dx),%es:(%rdi)
    1800681d2:	push   %rbx
    1800681d3:	outsl  %ds:(%rsi),(%dx)
@@ -148690,18 +148687,16 @@
    1800681f2:	rex push %rcx
    1800681f4:	rex.RB
    1800681f5:	rex.B
    1800681f6:	rex.B
    1800681f7:	rex pop %rax
    1800681f9:	pop    %rdx
    1800681fa:	add    %al,(%rax)
-   1800681fc:	(bad)
-   1800681fd:	add    (%rdi),%edi
-   1800681ff:	movsxd 0x65(%rdx),%esi
-   180068202:	(bad)
+   1800681fc:	call   0x1f269c104
+   180068201:	gs (bad)
    180068203:	je     0x18006826a
    180068205:	rex (bad)
    180068207:	and    $0x54,%al
    180068209:	gs je  0x18006827e
    18006820c:	(bad)
    18006820d:	push   $0x61726465
    180068212:	insb   (%dx),%es:(%rdi)
@@ -148747,15 +148742,15 @@
    18006826c:	push   %rsi
    18006826d:	(bad)
    18006826e:	and    $0x50,%al
    180068270:	outsl  %ds:(%rsi),(%dx)
    180068271:	imul   $0x31302440,0x74(%rsi),%ebp
    180068278:	rex xor 0x40(%rax),%al
    18006827c:	pop    %rdx
-   18006827d:	add    %al,0x69663f05(%rdx)
+   18006827d:	add    %al,0x69663f05(%rax)
    180068283:	outsb  %ds:(%rsi),(%dx)
    180068284:	fs rex (bad)
    180068287:	and    $0x54,%al
    180068289:	gs je  0x1800682fe
    18006828c:	(bad)
    18006828d:	push   $0x61726465
    180068292:	insb   (%dx),%es:(%rdi)
@@ -148796,15 +148791,16 @@
    1800682df:	addr32 pop %rdi
    1800682e1:	jbe    0x18006834c
    1800682e3:	gs ja  0x180068326
    1800682e6:	(bad)
    1800682e7:	(bad)
    1800682ec:	rex pop %rdx
    1800682ee:	add    %al,(%rax)
-   1800682f0:	jne    0x1800682f9
+   1800682f0:	outsl  %ds:(%rsi),(%dx)
+   1800682f1:	(bad)
    1800682f2:	(bad)
    1800682f3:	jae    0x18006835a
    1800682f5:	je     0x180068356
    1800682f7:	jbe    0x18006835a
    1800682f9:	insb   (%dx),%es:(%rdi)
    1800682fa:	jne    0x180068361
    1800682fc:	rex (bad)
@@ -148833,15 +148829,17 @@
    180068332:	(bad)
    180068333:	and    $0x50,%al
    180068335:	outsl  %ds:(%rsi),(%dx)
    180068336:	imul   $0x31302440,0x74(%rsi),%ebp
    18006833d:	rex xor 0x40(%rax),%al
    180068341:	pop    %rdx
    180068342:	add    %al,(%rax)
-   180068344:	or     $0x61763f08,%eax
+   180068344:	(bad)
+   180068345:	or     %bh,(%rdi)
+   180068347:	jbe    0x1800683aa
    180068349:	insb   (%dx),%es:(%rdi)
    18006834a:	jne    0x1800683b1
    18006834c:	rex (bad)
    18006834e:	and    $0x54,%al
    180068350:	gs je  0x1800683c5
    180068353:	(bad)
    180068354:	push   $0x61726465
@@ -148868,16 +148866,16 @@
    180068383:	(bad)
    180068384:	and    $0x50,%al
    180068386:	outsl  %ds:(%rsi),(%dx)
    180068387:	imul   $0x31302440,0x74(%rsi),%ebp
    18006838e:	rex xor 0x49(%rax),%al
    180068392:	rex pop %rdx
    180068394:	add    %al,(%rax)
-   180068396:	or     $0x8,%al
-   180068398:	(bad)
+   180068396:	(bad)
+   180068397:	or     %bh,(%rdi)
    180068399:	jbe    0x1800683fc
    18006839b:	insb   (%dx),%es:(%rdi)
    18006839c:	jne    0x180068403
    18006839e:	rex (bad)
    1800683a0:	and    $0x54,%al
    1800683a2:	gs je  0x180068417
    1800683a5:	(bad)
@@ -148909,15 +148907,17 @@
    1800683e4:	rex.X push %rsi
    1800683e6:	(bad)
    1800683e7:	and    $0x50,%al
    1800683e9:	outsl  %ds:(%rsi),(%dx)
    1800683ea:	imul   $0x32302440,0x74(%rsi),%ebp
    1800683f1:	rex xor 0x49(%rax),%al
    1800683f5:	rex pop %rdx
-   1800683f7:	add    %al,0x626e3f06(%rdx)
+   1800683f7:	add    %bh,0x3f(%rsi,%rax,1)
+   1800683fb:	outsb  %ds:(%rsi),(%dx)
+   1800683fc:	(bad)
    1800683fd:	pop    %rdi
    1800683fe:	jo     0x18006846f
    180068400:	insb   (%dx),%es:(%rdi)
    180068401:	jns    0x18006846b
    180068403:	gs fs jb 0x180068476
    180068407:	outsb  %ds:(%rsi),(%dx)
    180068408:	pop    %rdi
@@ -148935,15 +148935,15 @@
    180068428:	rex push %rcx
    18006842a:	rex.RB
    18006842b:	rex.X
    18006842c:	rex.B
    18006842d:	rex.RB
    18006842e:	rex.WB
    18006842f:	rex pop %rdx
-   180068431:	add    %dh,%cl
+   180068431:	add    %ch,%bl
    180068433:	(bad)
    180068434:	(bad)
    180068435:	jo     0x1800684a6
    180068437:	insb   (%dx),%es:(%rdi)
    180068438:	jns    0x1800684a2
    18006843a:	gs fs jb 0x1800684ad
    18006843e:	outsb  %ds:(%rsi),(%dx)
@@ -148976,15 +148976,15 @@
    180068470:	outsb  %ds:(%rsi),(%dx)
    180068471:	push   %rsi
    180068472:	gs jb  0x1800684e9
    180068475:	gs js  0x1800684b8
    180068478:	xor    0x40(%rax),%al
    18006847b:	pop    %rdx
    18006847c:	add    %al,(%rax)
-   18006847e:	jle    0x180068486
+   18006847e:	js     0x180068486
    180068480:	(bad)
    180068481:	outsb  %ds:(%rsi),(%dx)
    180068482:	(bad)
    180068483:	pop    %rdi
    180068484:	jo     0x1800684f5
    180068486:	insb   (%dx),%es:(%rdi)
    180068487:	jns    0x1800684f0
@@ -149003,15 +149003,16 @@
    1800684a2:	fs gs rex
    1800684a5:	rex push %rcx
    1800684a7:	rex.RB
    1800684a8:	rex.X
    1800684a9:	rex.B
    1800684aa:	rex.WB pop %r8
    1800684ac:	pop    %rdx
-   1800684ad:	add    %bh,0x3f(%rsi,%rax,1)
+   1800684ad:	add    %dh,0x6(%rsi)
+   1800684b0:	(bad)
    1800684b1:	outsb  %ds:(%rsi),(%dx)
    1800684b2:	(bad)
    1800684b3:	pop    %rdi
    1800684b4:	jo     0x180068525
    1800684b6:	insb   (%dx),%es:(%rdi)
    1800684b7:	jns    0x180068520
    1800684b9:	outsl  %ds:(%rsi),(%dx)
@@ -149033,15 +149034,15 @@
    1800684df:	rex.RB
    1800684e0:	rex.X
    1800684e1:	rex.B
    1800684e2:	rex.RB
    1800684e3:	rex.WB
    1800684e4:	rex pop %rdx
    1800684e6:	add    %al,(%rax)
-   1800684e8:	movb   $0x3f,(%rsi)
+   1800684e8:	rolb   $0x3f,(%rsi)
    1800684eb:	jo     0x18006855c
    1800684ed:	insb   (%dx),%es:(%rdi)
    1800684ee:	jns    0x180068557
    1800684f0:	outsl  %ds:(%rsi),(%dx)
    1800684f1:	outsb  %ds:(%rsi),(%dx)
    1800684f2:	pop    %rdi
    1800684f3:	jbe    0x18006855a
@@ -149073,15 +149074,15 @@
    180068522:	outsb  %ds:(%rsi),(%dx)
    180068523:	push   %rsi
    180068524:	gs jb  0x18006859b
    180068527:	gs js  0x18006856a
    18006852a:	xor    0x40(%rax),%al
    18006852d:	pop    %rdx
    18006852e:	add    %al,(%rax)
-   180068530:	mov    $0x6,%dh
+   180068530:	mov    $0x6,%al
    180068532:	(bad)
    180068533:	jo     0x1800685a4
    180068535:	insb   (%dx),%es:(%rdi)
    180068536:	jns    0x18006859f
    180068538:	outsl  %ds:(%rsi),(%dx)
    180068539:	outsb  %ds:(%rsi),(%dx)
    18006853a:	pop    %rdi
@@ -149116,15 +149117,15 @@
    180068573:	(bad)
    180068578:	(bad)
    180068579:	outsb  %ds:(%rsi),(%dx)
    18006857a:	(bad)
    18006857b:	addr32 gs jb 0x1800685bf
    18006857f:	xor    0x58(%rax),%al
    180068582:	pop    %rdx
-   180068583:	add    %ah,0x3(%rax)
+   180068583:	add    %bl,0x3(%rsi)
    180068586:	(bad)
    180068587:	movsxd 0x6e(%rdi,%rbp,2),%ebp
    18006858b:	gs rex (bad)
    18006858e:	and    $0x54,%al
    180068590:	jb     0x1800685fb
    180068592:	(bad)
    180068593:	outsb  %ds:(%rsi),(%dx)
@@ -149196,15 +149197,15 @@
    18006861b:	fs rex
    18006861d:	rex
    18006861e:	rex jae 0x180068695
    180068621:	fs rex
    180068623:	rex pop %rax
    180068625:	pop    %rdx
    180068626:	add    %al,(%rax)
-   180068628:	in     $0x3,%eax
+   180068628:	jrcxz  0x18006862d
    18006862a:	(bad)
    18006862b:	movsxd 0x65(%rdx),%esi
    18006862e:	(bad)
    18006862f:	je     0x180068696
    180068631:	rex (bad)
    180068633:	and    $0x53,%al
    180068635:	jne    0x1800686a9
@@ -149279,15 +149280,15 @@
    1800686cf:	movsxd 0x4d(%rbp),%esp
    1800686d2:	gs jae 0x18006873d
    1800686d5:	rex and $0x30,%al
    1800686d8:	xor    0x32(%rax),%al
    1800686db:	rex
    1800686dc:	rex pop %rdx
    1800686de:	add    %al,(%rax)
-   1800686e0:	push   %rbp
+   1800686e0:	push   %rbx
    1800686e1:	add    $0x6764653f,%eax
    1800686e6:	gs pop %rdi
    1800686e8:	jbe    0x18006874f
    1800686ea:	jb     0x180068760
    1800686ec:	gs js  0x18006872f
    1800686ef:	rex.RXB jb 0x180068753
    1800686f2:	jo     0x18006875c
@@ -149305,15 +149306,15 @@
    180068705:	rex.RB
    180068706:	fs addr32 gs push %rsi
    18006870a:	gs jb  0x180068781
    18006870d:	gs js  0x180068750
    180068710:	xor    0x40(%rax),%al
    180068713:	pop    %rdx
    180068714:	add    %al,(%rax)
-   180068716:	pop    %rcx
+   180068716:	push   %rdi
    180068717:	add    $0x6764653f,%eax
    18006871c:	gs pop %rdi
    18006871e:	jbe    0x180068785
    180068720:	jb     0x180068796
    180068722:	imul   $0x72474073,0x65(%rbx),%esp
    180068729:	(bad)
    18006872a:	jo     0x180068794
@@ -149334,16 +149335,16 @@
    180068746:	xor    %eax,0x73(%rax)
    180068749:	je     0x1800687af
    18006874b:	rex
    18006874c:	rex
    18006874d:	rex.WB
    18006874e:	rex pop %rdx
    180068750:	add    %al,(%rax)
-   180068752:	cmp    $0x64653f05,%eax
-   180068757:	addr32 gs pop %rdi
+   180068752:	cmp    0x6764653f(%rip),%eax        # 0x1e76aec97
+   180068758:	gs pop %rdi
    18006875a:	(bad)
    18006875b:	je     0x1800687d1
    18006875d:	jb     0x1800687c8
    18006875f:	(bad)
    180068764:	insl   (%dx),%es:(%rdi)
    180068765:	(bad)
    180068766:	outsb  %ds:(%rsi),(%dx)
@@ -149367,16 +149368,16 @@
    18006878b:	(bad)
    18006878c:	outsb  %ds:(%rsi),(%dx)
    18006878d:	(bad)
    18006878e:	addr32 gs jb 0x1800687d2
    180068792:	xor    0x58(%rax),%al
    180068795:	pop    %rdx
    180068796:	add    %al,(%rax)
-   180068798:	iret
-   180068799:	add    %edi,(%rdi)
+   180068798:	int    $0x1
+   18006879a:	(bad)
    18006879b:	(bad)
    18006879c:	xor    %dl,0x6f(%rax)
    18006879f:	insb   (%dx),%es:(%rdi)
    1800687a0:	jns    0x180068809
    1800687a2:	outsl  %ds:(%rsi),(%dx)
    1800687a3:	outsb  %ds:(%rsi),(%dx)
    1800687a4:	rex.RB
@@ -149385,16 +149386,15 @@
    1800687ac:	fs gs rex
    1800687af:	rex push %rcx
    1800687b1:	rex.RB
    1800687b2:	rex.B
    1800687b3:	rex.B
    1800687b4:	rex pop %rax
    1800687b6:	pop    %rdx
-   1800687b7:	add    %ah,0x303f3f01(%rsi)
-   1800687bd:	(bad)
+   1800687b7:	add    %ah,0x3f303f3f(%rcx,%rax,1)
    1800687be:	and    $0x54,%al
    1800687c0:	jb     0x18006882b
    1800687c2:	(bad)
    1800687c3:	outsb  %ds:(%rsi),(%dx)
    1800687c4:	addr32 jne 0x180068833
    1800687c7:	(bad)
    1800687c8:	je     0x18006882f
@@ -149420,15 +149420,15 @@
    1800687f5:	push   %rcx
    1800687f6:	rex.RB
    1800687f7:	push   %r14
    1800687f9:	xor    %dh,(%rcx)
    1800687fb:	rex
    1800687fc:	rex pop %rdx
    1800687fe:	add    %al,(%rax)
-   180068800:	rex.RXB add (%r15),%r15b
+   180068800:	add    (%r15),%r15b
    180068803:	(bad)
    180068804:	xor    %edi,(%rdi)
    180068806:	and    $0x54,%al
    180068808:	jb     0x180068873
    18006880a:	(bad)
    18006880b:	outsb  %ds:(%rsi),(%dx)
    18006880c:	addr32 jne 0x18006887b
@@ -149450,15 +149450,15 @@
    180068832:	fs gs rex
    180068835:	rex push %rcx
    180068837:	rex.RB
    180068838:	rex.B
    180068839:	rex.B
    18006883a:	rex pop %rax
    18006883c:	pop    %rdx
-   18006883d:	add    %dh,%bl
+   18006883d:	add    %dh,%cl
    18006883f:	add    (%rdi),%edi
    180068841:	movsxd 0x65(%rdx),%esi
    180068844:	(bad)
    180068845:	je     0x1800688ac
    180068847:	rex (bad)
    180068849:	and    $0x54,%al
    18006884b:	jb     0x1800688b6
@@ -149515,15 +149515,15 @@
    1800688b4:	push   %rsi
    1800688b5:	(bad)
    1800688b6:	and    $0x50,%al
    1800688b8:	outsl  %ds:(%rsi),(%dx)
    1800688b9:	imul   $0x30302440,0x74(%rsi),%ebp
    1800688c0:	rex xor 0x40(%rax),%al
    1800688c4:	pop    %rdx
-   1800688c5:	add    %al,0x69663f05(%rbp)
+   1800688c5:	add    %al,0x69663f05(%rbx)
    1800688cb:	outsb  %ds:(%rsi),(%dx)
    1800688cc:	fs rex (bad)
    1800688cf:	and    $0x54,%al
    1800688d1:	jb     0x18006893c
    1800688d3:	(bad)
    1800688d4:	outsb  %ds:(%rsi),(%dx)
    1800688d5:	addr32 jne 0x180068944
@@ -149572,15 +149572,15 @@
    18006892d:	addr32 pop %rdi
    18006892f:	jbe    0x18006899a
    180068931:	gs ja  0x180068974
    180068934:	(bad)
    180068935:	(bad)
    18006893a:	rex pop %rdx
    18006893c:	add    %al,(%rax)
-   18006893e:	js     0x180068947
+   18006893e:	jb     0x180068947
    180068940:	(bad)
    180068941:	jae    0x1800689a8
    180068943:	je     0x1800689a4
    180068945:	jbe    0x1800689a8
    180068947:	insb   (%dx),%es:(%rdi)
    180068948:	jne    0x1800689af
    18006894a:	rex (bad)
@@ -149612,17 +149612,15 @@
    180068981:	rex.WB push %r14
    180068983:	(bad)
    180068984:	and    $0x50,%al
    180068986:	outsl  %ds:(%rsi),(%dx)
    180068987:	imul   $0x30302440,0x74(%rsi),%ebp
    18006898e:	rex xor 0x40(%rax),%al
    180068992:	pop    %rdx
-   180068993:	add    %dl,(%rbx)
-   180068995:	or     %bh,(%rdi)
-   180068997:	jbe    0x1800689fa
+   180068993:	add    %cl,0x61763f08(%rip)        # 0x1e17cc8a1
    180068999:	insb   (%dx),%es:(%rdi)
    18006899a:	jne    0x180068a01
    18006899c:	rex (bad)
    18006899e:	and    $0x54,%al
    1800689a0:	jb     0x180068a0b
    1800689a2:	(bad)
    1800689a3:	outsb  %ds:(%rsi),(%dx)
@@ -149652,16 +149650,16 @@
    1800689d4:	rex.X push %rsi
    1800689d6:	(bad)
    1800689d7:	and    $0x50,%al
    1800689d9:	outsl  %ds:(%rsi),(%dx)
    1800689da:	imul   $0x30302440,0x74(%rsi),%ebp
    1800689e1:	rex xor 0x49(%rax),%al
    1800689e5:	rex pop %rdx
-   1800689e7:	add    %dl,(%rdx)
-   1800689e9:	or     %bh,(%rdi)
+   1800689e7:	add    %cl,(%rax,%rcx,1)
+   1800689ea:	(bad)
    1800689eb:	jbe    0x180068a4e
    1800689ed:	insb   (%dx),%es:(%rdi)
    1800689ee:	jne    0x180068a55
    1800689f0:	rex (bad)
    1800689f2:	and    $0x54,%al
    1800689f4:	jb     0x180068a5f
    1800689f6:	(bad)
@@ -149698,15 +149696,15 @@
    180068a3b:	(bad)
    180068a3c:	and    $0x50,%al
    180068a3e:	outsl  %ds:(%rsi),(%dx)
    180068a3f:	imul   $0x31302440,0x74(%rsi),%ebp
    180068a46:	rex xor 0x49(%rax),%al
    180068a4a:	rex pop %rdx
    180068a4c:	add    %al,(%rax)
-   180068a4e:	jge    0x180068a56
+   180068a4e:	ja     0x180068a56
    180068a50:	(bad)
    180068a51:	outsb  %ds:(%rsi),(%dx)
    180068a52:	(bad)
    180068a53:	pop    %rdi
    180068a54:	jo     0x180068ac5
    180068a56:	insb   (%dx),%es:(%rdi)
    180068a57:	jns    0x180068ac0
@@ -149725,15 +149723,15 @@
    180068a72:	fs gs rex
    180068a75:	rex push %rcx
    180068a77:	rex.RB
    180068a78:	rex.X
    180068a79:	rex.B
    180068a7a:	rex.WB pop %r8
    180068a7c:	pop    %rdx
-   180068a7d:	add    %bh,0x6(%rbx)
+   180068a7d:	add    %dh,0x6(%rbp)
    180068a80:	(bad)
    180068a81:	outsb  %ds:(%rsi),(%dx)
    180068a82:	(bad)
    180068a83:	pop    %rdi
    180068a84:	jo     0x180068af5
    180068a86:	insb   (%dx),%es:(%rdi)
    180068a87:	jns    0x180068af0
@@ -149756,16 +149754,15 @@
    180068aaf:	rex.RB
    180068ab0:	rex.X
    180068ab1:	rex.B
    180068ab2:	rex.RB
    180068ab3:	rex.WB
    180068ab4:	rex pop %rdx
    180068ab6:	add    %al,(%rax)
-   180068ab8:	(bad)
-   180068abb:	jo     0x180068b2c
+   180068ab8:	mov    $0x6f703f06,%edi
    180068abd:	insb   (%dx),%es:(%rdi)
    180068abe:	jns    0x180068b27
    180068ac0:	outsl  %ds:(%rsi),(%dx)
    180068ac1:	outsb  %ds:(%rsi),(%dx)
    180068ac2:	pop    %rdi
    180068ac3:	jbe    0x180068b2a
    180068ac5:	jb     0x180068b3b
@@ -149796,15 +149793,17 @@
    180068af2:	outsb  %ds:(%rsi),(%dx)
    180068af3:	push   %rsi
    180068af4:	gs jb  0x180068b6b
    180068af7:	gs js  0x180068b3a
    180068afa:	xor    0x40(%rax),%al
    180068afd:	pop    %rdx
    180068afe:	add    %al,(%rax)
-   180068b00:	movl   $0x6c6f703f,(%rsi)
+   180068b00:	roll   $0x3f,(%rsi)
+   180068b03:	jo     0x180068b74
+   180068b05:	insb   (%dx),%es:(%rdi)
    180068b06:	jns    0x180068b6f
    180068b08:	outsl  %ds:(%rsi),(%dx)
    180068b09:	outsb  %ds:(%rsi),(%dx)
    180068b0a:	pop    %rdi
    180068b0b:	jbe    0x180068b72
    180068b0d:	jb     0x180068b83
    180068b0f:	imul   $0x243f4073,0x65(%rbx),%esp
@@ -149843,16 +149842,15 @@
    180068b59:	fs rex
    180068b5b:	rex
    180068b5c:	rex (bad)
    180068b5e:	(bad)
    180068b63:	rex.WB
    180068b64:	rex pop %rdx
    180068b66:	add    %al,(%rax)
-   180068b68:	push   %rcx
-   180068b69:	add    (%rdi),%edi
+   180068b68:	rex.WRXB add (%r15),%r15
    180068b6b:	movsxd 0x6e(%rdi,%rbp,2),%ebp
    180068b6f:	gs rex (bad)
    180068b72:	and    $0x45,%al
    180068b74:	fs addr32 gs fs rex.XB jne 0x180068bed
    180068b7b:	jbe    0x180068be2
    180068b7d:	rex and $0x30,%al
    180068b80:	xor    %eax,0x67(%rax)
@@ -149898,16 +149896,16 @@
    180068be1:	rex jae 0x180068c58
    180068be4:	fs rex
    180068be6:	rex
    180068be7:	rex jae 0x180068c5e
    180068bea:	fs rex
    180068bec:	rex pop %rax
    180068bee:	pop    %rdx
-   180068bef:	add    %bh,0x6572633f(%rbx,%rax,1)
-   180068bf6:	(bad)
+   180068bef:	add    %bh,0x72633f03(%rdx)
+   180068bf5:	gs (bad)
    180068bf7:	je     0x180068c5e
    180068bf9:	rex (bad)
    180068bfb:	and    $0x45,%al
    180068bfd:	fs addr32 gs fs rex.XB jne 0x180068c76
    180068c04:	jbe    0x180068c6b
    180068c06:	rex.X jne 0x180068c72
    180068c09:	insb   (%dx),%es:(%rdi)
```

## Comparing `OpenGeode_Geosciences-7.1.2.dist-info/METADATA` & `OpenGeode_Geosciences-7.1.2rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Geosciences
-Version: 7.1.2
+Version: 7.1.2rc1
 Summary: OpenGeode module for Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.4.2)
+Requires-Dist: opengeode-core (==14.*,>=14.4.2rc1)
 
 <h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.1.2 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.1.2rc1 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown Requires-Dist: opengeode-core (==14.*,>=14.4.2)
+markdown Requires-Dist: opengeode-core (==14.*,>=14.4.2rc1)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

## Comparing `OpenGeode_Geosciences-7.1.2.dist-info/RECORD` & `OpenGeode_Geosciences-7.1.2rc1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 opengeode_geosciences/__init__.py,sha256=w7_ys_rdYFV6X9-DHDK4aHD3C7a7YbuiKhXh-gdoyq0,199
 opengeode_geosciences/explicit.py,sha256=uSrCUigVUNQlZUlZGI6tLpCACmWLqC3zJdI9V9p2L9w,1239
 opengeode_geosciences/implicit.py,sha256=1h6T21wYBxmNpkFTsSbPw-sFx79T_iZGANQRnwCtmho,1239
-opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll,sha256=sxqKycrQY9KdmjQCh9tfabUG7qGAbW-LDG_I0zShMdE,573440
-opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll,sha256=XY9qPl1LIV0_cjHmmWadLYVHBujtk9AuaFqE6izEtkw,482304
-opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd,sha256=SnySwlGOv-Kkg3VhnjtgHmGMfg1OTqO4RLBTFmpEdLM,387072
-opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd,sha256=nfpyWXWa6sO9EwNAnxop6XYNr8iGRbLWl9hwyHDYvMg,334336
-OpenGeode_Geosciences-7.1.2.dist-info/METADATA,sha256=7xx5i5GhXFjBW_UztOjqsO0vlxSVZ5Js7_0MsHivJ0k,3232
-OpenGeode_Geosciences-7.1.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Geosciences-7.1.2.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
-OpenGeode_Geosciences-7.1.2.dist-info/RECORD,,
+opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll,sha256=GmXA3bq7v7drLH7A2v7AKTbmkzj2x37P7XdONKoz-i4,573440
+opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll,sha256=Iw57ZaTwyfYioTLaqSLp5HlNCMHdWmrjE4Hj8CLFCKY,482304
+opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd,sha256=TNP3pwUqr_2grsjz3SuXFrky_2IJf9b11KKcwbrWqLs,387072
+opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd,sha256=YL-Tlsk2wcNOWOn5Ik5e7a7OCsC_GCo17S4lkX9zFdU,334336
+OpenGeode_Geosciences-7.1.2rc1.dist-info/METADATA,sha256=O_T5ZCKYcU81ooBZOLEJcM9rO5xJIENL3jfxzCOOQaw,3238
+OpenGeode_Geosciences-7.1.2rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_Geosciences-7.1.2rc1.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
+OpenGeode_Geosciences-7.1.2rc1.dist-info/RECORD,,
```

