# Comparing `tmp/libzac-0.0.8-py3-none-any.whl.zip` & `tmp/libzac-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14647 bytes, number of entries: 13
+Zip file size: 14632 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-19 08:09 libzac/__init__.py
--rw-rw-rw-  2.0 fat     5564 b- defN 23-Jun-19 09:14 libzac/bitfield.py
+-rw-rw-rw-  2.0 fat     6198 b- defN 23-Jul-12 03:11 libzac/bitfield.py
 -rw-rw-rw-  2.0 fat     1960 b- defN 23-May-17 07:50 libzac/dsp.py
 -rw-rw-rw-  2.0 fat     4978 b- defN 23-Jun-19 08:10 libzac/e.py
 -rw-rw-rw-  2.0 fat     3007 b- defN 23-May-17 07:56 libzac/io.py
 -rw-rw-rw-  2.0 fat     1510 b- defN 23-May-23 02:36 libzac/math.py
 -rw-rw-rw-  2.0 fat     3074 b- defN 23-May-17 08:19 libzac/plt.py
--rw-rw-rw-  2.0 fat     9564 b- defN 23-Jun-20 02:04 libzac/reg.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1734 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      947 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/RECORD
-13 files, 33658 bytes uncompressed, 13105 bytes compressed:  61.1%
+-rw-rw-rw-  2.0 fat     8751 b- defN 23-Jul-12 03:13 libzac/reg.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1734 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      947 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/RECORD
+13 files, 33479 bytes uncompressed, 13090 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: libzac/plt.py
 Comment: 
 
 Filename: libzac/reg.py
 Comment: 
 
-Filename: libzac-0.0.8.dist-info/LICENSE
+Filename: libzac-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: libzac-0.0.8.dist-info/METADATA
+Filename: libzac-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: libzac-0.0.8.dist-info/WHEEL
+Filename: libzac-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: libzac-0.0.8.dist-info/top_level.txt
+Filename: libzac-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: libzac-0.0.8.dist-info/RECORD
+Filename: libzac-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libzac/bitfield.py

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Any
 import numpy as np
 from .e import eread, ewrite
 
 ########## used for debug without actually read/wrtie memory #############
 # eread = lambda addr,length: np.random.randint(0,255,length,dtype="u1")
 # ewrite = lambda addr,value: None
@@ -91,14 +92,28 @@
         self._data = int.from_bytes(r.tobytes(), self.__ENDIANESS)
 
     def write(self, verbose=False):
         if verbose:
             print(f"write {self.hex} @ {self.addr}")
         ewrite(self.addr, self.hex) # write `self.size` bytes to memory at address `self.addr`
 
+    def diff(self, another:bitfield):
+        if isinstance(another, type(self)):
+            s = ""
+            for this,that in zip(str(self).splitlines(), str(another).splitlines()):
+                this_value = this.split("=")[1]
+                that_value = that.split("=")[1]
+                if this_value == that_value:
+                    s += this+"\n"
+                else:
+                    s += this + " =>" + that_value + "\n"
+            return s
+        else:
+            raise TypeError(f'Try to diff "{another.__class__.__name__}" to "{self.__class__.__name__}"')
+
 if __name__ == "__main__":
     # following C bitfield struct `Example` has total 24 bits, which is 3 bytes
     # GCC's `__attribute__((packed))` minimize memory usage, no padding between members
     # ```c
     # typedef struct
     # {
     # 	volatile unsigned short A	    :8;
```

## libzac/reg.py

```diff
@@ -103,18 +103,18 @@
     return table
 
 def keep_rename_columns(table:pd.DataFrame) -> None:
     """only keep columns in `names`, and rename them to dict keys"""
     names = {
         "write addr":["Write Address"],
         "read addr":["Read Address"],
-        addr_name:[addr_name,"地址","addr"],
+        addr_name:[addr_name,"地址","addr","Address"],
         reg_name:[reg_name,"寄存器","reg_name","Type"],
-        width_name:[width_name,"位置","width","Bit"],
-        domain_name:[domain_name,"域名","field_name","Register Name"],
+        width_name:[width_name,"位置","width","Bit","Bit location"],
+        domain_name:[domain_name,"域名","field_name","Register Name","name"],
         access_name:[access_name,"RW","access","读写"],
         init_name:[init_name,"original","initVal\n（HEX）","初始值","Default Value"],
         description_name:[description_name,"Description","描述","Note"],
     }
     for col in table.columns:
         for k,v in names.items():
             if col in v:
@@ -136,43 +136,43 @@
     table.loc[domain_na,(domain_name)] = table.loc[domain_na,(reg_name)] + "_reserved"
     # replace " " and "[]" with "_"
     table[reg_name].replace(r"[ \[\]:]","_",regex=True,inplace=True)
     table[domain_name].replace(r"[ \[\]:]","_",regex=True,inplace=True)
     # remove [] from width
     table[width_name].replace("[\[\]]","",regex=True,inplace=True)
     # "W"->"WO", "R"->"RO", else->"RW" # disable when use diff compare generated file with original reg_struct.h
-    # table.loc[table[access_name]=="W",(access_name)] = "WO"
-    # table.loc[table[access_name]=="R",(access_name)] = "RO"
-    # table.loc[table[access_name].isna(),(access_name)] = "RW"
-    # table.loc[~((table[access_name]=="WO") | (table[access_name]=="RO")),(access_name)] = "RW"
+    table.loc[table[access_name]=="W",(access_name)] = "WO"
+    table.loc[table[access_name]=="R",(access_name)] = "RO"
+    table.loc[table[access_name].isna(),(access_name)] = "RW"
+    table.loc[~((table[access_name]=="WO") | (table[access_name]=="RO")),(access_name)] = "RW"
     # if description is nan, use "" as default
     table.loc[table[description_name].isna(),(description_name)] = ""
     table[description_name].replace("None","",regex=True,inplace=True)
     # reg is upper case, domain is lower case
     table[reg_name] = table[reg_name].str.upper()
     table[domain_name] = table[domain_name].str.lower()
 
 def read_yc_reg(wb:__workbook_type, sheet_name:str) -> pd.DataFrame:
     """read table from workbook then format it"""
     table = read_excel(wb,sheet_name)
     keep_rename_columns(table)
     format_table(table)
     return table
 
-def read_yc_reg_from_file(filename:str):
+def read_yc_reg_from_file(filename:str) -> dict[str:pd.DataFrame]:
     wb = openpyxl.load_workbook(filename)
     tables = {sheet_name:read_yc_reg(wb, sheet_name) for sheet_name in wb.sheetnames if sheet_name != 'lpm'}
     return tables
 
-def keep_only_rows(table:pd.DataFrame, keep_list:list, col:str = addr_name):
+def keep_only_rows(table:pd.DataFrame, keep_list:list, col:str = addr_name) -> pd.DataFrame:
     return table.loc[table[col].isin(keep_list)]
 
 def efile_to_hashmap(filename:str) -> dict:
     """convert an `e [addr]l[size]` output file to dict where key is addr and value is data"""
-    return {f"{a:x}":d for d,a in zip(e2int(filename,"u1"))}
+    return {f"{a:x}":d for d,a in zip(*e2int(filename,"u1"))}
 
 def parse_width(width:Union[str,int]) -> tuple[int,int]:
     """parse_width('[x]/x') = (x,x);  parse_width('[x:y]/x:y') = (x,y)"""
     if isinstance(width, (np.integer, int)):
         return width, width
     if (not width) or (width == "nan"):
         raise ValueError(f"parse_width() failed: {type(width)}:{width}")
@@ -192,44 +192,25 @@
         num = (num >> start) & ((1<<bits)-1)
         return f"{num:0{((bits-1)//8+1)*2}x}"
     else:
         return "nan"
     
 def parse_table(table:pd.DataFrame, reg_map:dict, new_column:str) -> None:        
     """add new column named `new_column` to `table`, apply `parse_reg` to each row"""
-    table[new_column] = np.zeros(len(table),str)
+    table.loc[:,new_column] = np.zeros(len(table),str)
     for i in table.index:    
         try:
             start, stop = parse_width(table.loc[i,width_name])
             if start >= 0 and not pd.isna(table.loc[i,addr_name]):            
                 addr = re.search(r"[\da-f]{4,}",table.loc[i,addr_name])
                 if addr is not None:     
                     table.loc[i,new_column] = parse_reg(addr.group(), reg_map, start, stop)
-        except:
-            print(f"Unable to parse table line{i}: \n{table.loc[i]}")
-
-def read_yc_reg_map(table:pd.DataFrame, reg_map:dict, new_column=None) -> pd.DataFrame:
-    """apply `parse_table` to a copy of `table` with `reg_map`"""
-    table = table.copy()
-    new_column = "new" if new_column is None else new_column    
-    parse_table(table, reg_map, new_column)
-    return table
-
-def read_yc_reg_map_in_folder(table:pd.DataFrame, top_folder:str, sheet_name:str, suffix:str=""):
-    """apply `read_yc_reg_map` to every files start with `sheet_name` in a folder"""
-    table = table[table[access_name]=="RW"]
-    count = 0
-    for dir,_,files in os.walk(top_folder):
-        for f in files:
-            if f.startswith(sheet_name):
-                new_column = suffix + str(count) if suffix else f
-                reg_map = efile_to_hashmap(dir + "\\" + f)
-                table = read_yc_reg_map(table, reg_map, new_column=new_column)
-                count += 1
-    return table
+        except Exception as e:
+            print(f"Unable to parse table line {i}: \n{table.loc[i]}\n")
+            raise e
 
 def table2tree(table:pd.DataFrame, key:str) -> dict:
     """convert pandas Dataframe to tree like dict, use either `addr_name` or `reg_name` as `key`"""
     tree = {}
     old_key = ""
     for i in table.to_dict("records"):
         if tree.get(i[key],False):
```

## Comparing `libzac-0.0.8.dist-info/LICENSE` & `libzac-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libzac-0.0.8.dist-info/METADATA` & `libzac-0.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libzac
-Version: 0.0.8
+Version: 0.0.9
 Summary: A private use library
 Author-email: ZinGer_KyoN <zinger.kyon@gmail.com>
 License: MIT License        
         Copyright (c) 2022 YiChip Inc.        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

