# Comparing `tmp/hisv-1.0.6-py3-none-any.whl.zip` & `tmp/hisv-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18761 bytes, number of entries: 16
--rwxrwxrwx  2.0 unx      141 b- defN 23-Jul-11 03:23 hisv/__init__.py
+Zip file size: 18898 bytes, number of entries: 16
+-rwxrwxrwx  2.0 unx      141 b- defN 23-Jul-12 13:54 hisv/__init__.py
 -rwxrwxrwx  2.0 unx     3529 b- defN 23-Jul-10 02:20 hisv/bamToMatrix.py
 -rwxrwxrwx  2.0 unx     3338 b- defN 23-Jul-09 13:30 hisv/combineIntraResult.py
 -rwxrwxrwx  2.0 unx     3331 b- defN 23-Jul-09 13:30 hisv/combineResult.py
 -rwxrwxrwx  2.0 unx     3539 b- defN 23-Jul-10 02:20 hisv/coolToMatrix.py
 -rwxrwxrwx  2.0 unx     3344 b- defN 23-Jul-10 01:40 hisv/hicToMatrix.py
 -rwxrwxrwx  2.0 unx     4448 b- defN 23-Jul-10 13:03 hisv/normCove.py
--rwxrwxrwx  2.0 unx    15354 b- defN 23-Jul-11 03:24 hisv-1.0.6.data/scripts/HiSV
--rwxrwxrwx  2.0 unx     6751 b- defN 23-Jul-11 03:24 hisv-1.0.6.data/scripts/SV_type
--rwxrwxrwx  2.0 unx     7907 b- defN 23-Jul-11 03:24 hisv-1.0.6.data/scripts/determin_breakpoint
--rwxrwxrwx  2.0 unx     2746 b- defN 23-Jul-11 03:24 hisv-1.0.6.data/scripts/hiccovert
--rwxrwxrwx  2.0 unx     1107 b- defN 23-Jul-11 03:24 hisv-1.0.6.dist-info/LICENSE
--rwxrwxrwx  2.0 unx      633 b- defN 23-Jul-11 03:24 hisv-1.0.6.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-11 03:24 hisv-1.0.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        5 b- defN 23-Jul-11 03:24 hisv-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1268 b- defN 23-Jul-11 03:24 hisv-1.0.6.dist-info/RECORD
-16 files, 57533 bytes uncompressed, 16691 bytes compressed:  71.0%
+-rwxrwxrwx  2.0 unx    15569 b- defN 23-Jul-12 13:57 hisv-1.0.7.data/scripts/HiSV
+-rwxrwxrwx  2.0 unx     6702 b- defN 23-Jul-12 13:57 hisv-1.0.7.data/scripts/SV_type
+-rwxrwxrwx  2.0 unx     7907 b- defN 23-Jul-12 13:57 hisv-1.0.7.data/scripts/determin_breakpoint
+-rwxrwxrwx  2.0 unx     2959 b- defN 23-Jul-12 13:57 hisv-1.0.7.data/scripts/hiccovert
+-rwxrwxrwx  2.0 unx     1107 b- defN 23-Jul-12 13:57 hisv-1.0.7.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx      633 b- defN 23-Jul-12 13:57 hisv-1.0.7.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-12 13:57 hisv-1.0.7.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        5 b- defN 23-Jul-12 13:57 hisv-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1268 b- defN 23-Jul-12 13:57 hisv-1.0.7.dist-info/RECORD
+16 files, 57912 bytes uncompressed, 16828 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -15,35 +15,35 @@
 
 Filename: hisv/hicToMatrix.py
 Comment: 
 
 Filename: hisv/normCove.py
 Comment: 
 
-Filename: hisv-1.0.6.data/scripts/HiSV
+Filename: hisv-1.0.7.data/scripts/HiSV
 Comment: 
 
-Filename: hisv-1.0.6.data/scripts/SV_type
+Filename: hisv-1.0.7.data/scripts/SV_type
 Comment: 
 
-Filename: hisv-1.0.6.data/scripts/determin_breakpoint
+Filename: hisv-1.0.7.data/scripts/determin_breakpoint
 Comment: 
 
-Filename: hisv-1.0.6.data/scripts/hiccovert
+Filename: hisv-1.0.7.data/scripts/hiccovert
 Comment: 
 
-Filename: hisv-1.0.6.dist-info/LICENSE
+Filename: hisv-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: hisv-1.0.6.dist-info/METADATA
+Filename: hisv-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: hisv-1.0.6.dist-info/WHEEL
+Filename: hisv-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: hisv-1.0.6.dist-info/top_level.txt
+Filename: hisv-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hisv-1.0.6.dist-info/RECORD
+Filename: hisv-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hisv/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Created on July 10 2023
 
 @author: Li Junping
 """
 __author__ = 'Li Junping'
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 
 Me = __file__
```

## Comparing `hisv-1.0.6.data/scripts/HiSV` & `hisv-1.0.7.data/scripts/HiSV`

 * *Files 9% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 else:
                     matrix[r][c] = (matrix[r][c] - Diagonal_mean[d]) / Diagonal_std[d]
             r += 1
             c += 1
     return matrix
 
 
-def call_intra_sv(i, chr_id, chr_intra_count, chr_inter_count, intra_hicfile, inter_hicfile, win, cutoff, name,
+def call_intra_sv(i, chr_id, chr_intra_count, chr_inter_count, intra_hicfile, inter_hicfile, win, reg, cutoff, name,
                   intra_binSize, inter_binSize, output):
     """
     Call SVs for each chromosome (including intra- and inter chromosomal)
     :param i: Chrom index
     :param chr_id: ChromID
     :param hicfile: current chromosomal hic matrix file
     :param win: local region window.
@@ -129,15 +129,15 @@
         chrlist = [chr_id[i], chr_id[j]]
         print("Read Hi-C matrix file: ", chrlist)
 
         if i == j:
             # intra_chromosomal
             score_result_file = os.path.join(output, name + '_%skb_%s_%s_HiSV_score.txt' % (str(intra_binSize // 1000),
                                                                                             chr_id[i], chr_id[j]))
-            # matrix_file = os.path.join(hicfile, '%s.txt' % (chr_id[i]))
+
             matrix_file = os.path.join(intra_hicfile, name + '_%skb_%s_%s_matrix.txt' % (str(intra_binSize // 1000),
                                                                                          chr_id[i], chr_id[j]))
             print(matrix_file)
             contact_matrix = np.loadtxt(matrix_file)
             if np.shape(contact_matrix)[0] != chr_intra_count[i]:
                 print("The binsize setting does not match the matrix file.")
                 sys.exit(-1)
@@ -146,15 +146,15 @@
             contact_matrix[il] = 0
             # print('Z-score for distance')
             # z-score for distance normalization
             Dist_norm_matrix = Distance_normalization(contact_matrix)
             # print('local saliency')
             # calculating local saliency
             local_sali_matrix = local_saliency(Dist_norm_matrix, win)
-            tv_param = 0.2
+            tv_param = reg
             score = ptv.tv1_2d(local_sali_matrix, tv_param, n_threads=1, max_iters=0, method='dr')
             np.savetxt(score_result_file, score, fmt="%1.2f")
             raw_num = col_num = np.shape(score)[0]
 
             for m in range(raw_num):
                 for n in range(col_num):
                     if score[m][n] > cutoff:
@@ -174,15 +174,15 @@
                 print("The binsize setting does not match the matrix file.")
                 sys.exit(-1)
             raw_num = np.shape(contact_matrix)[0]
             col_num = np.shape(contact_matrix)[1]
 
             # calculating local saliency
             local_sali_matrix = local_saliency(contact_matrix, 10)
-            tv_param = 0.2
+            tv_param = reg
             score = ptv.tv1_2d(local_sali_matrix, tv_param, n_threads=1, max_iters=0, method='dr')
             np.savetxt(score_result_file, score, fmt="%1.2f")
             for m in range(raw_num):
                 for n in range(col_num):
                     if score[m][n] > cutoff:
                         inter_chrom1.append(chr_id[i])
                         inter_chrom2.append(chr_id[j])
@@ -197,37 +197,42 @@
                                      formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument('--inter_hic', help='inter chromosomal hi-c contact matrix.')
     parser.add_argument('--intra_hic', help='intra chromosomal hi-c contact matrix.')
     parser.add_argument('--intra_binsize', type=int, default=50000, help='Resolution of intra Hi-C contact matrix.')
     parser.add_argument('--inter_binsize', type=int, default=50000, help='Resolution of inter Hi-C contact matrix.')
     parser.add_argument('--window', type=int, default=10, help='''Local region window.''')
+    parser.add_argument('--regularization', type=float, default=0.2, help='The regularization parameter')
     parser.add_argument('--cutoff', type=float, default=0.6, help='''Threshold for filtering SV segments''')
     parser.add_argument('--ref', help='Reference Genome length file')
     parser.add_argument('--name', help='Sample name')
     parser.add_argument('--cores', type=int, help='The number of cores used for parallel computing')
     parser.add_argument('--output', help='''Output file path.''')
 
     ## Parse the command-line arguments
     commands = sys.argv[1:]
     if not commands:
         commands.append('-h')
     args = parser.parse_args(commands)
     return args, commands
 
 
-def run_HiSV(ref_file, inter_binSize, intra_binSize, win, cutoff, n_cores, intra_hicfile, inter_hicfile, name, output):
+def run_HiSV(ref_file, inter_binSize, intra_binSize, win, reg, cutoff, n_cores, intra_hicfile, inter_hicfile, name, output):
     if not os.path.exists(output):
         os.makedirs(output)
 
     if cutoff > 1 or cutoff < 0:
         print("Cut-off parameter should be in the range 0-1.")
         # sys.exit(-1)
         return "Parameter Error."
 
+    if reg > 1 or reg < 0:
+        print("Regularization parameter should be in the range 0-1.")
+        return "Parameter Error."
+
     if not isinstance(win, int) or win < 0:
         print("The Win parameter should be an integer greater than 0.")
         # sys.exit(-1)
         return "Parameter Error."
 
     if not os.path.exists(intra_hicfile):
         print("Intra_hicfile does not exist")
@@ -258,30 +263,30 @@
     chr_id, chr_intra_count, chr_inter_count = read_reflen(ref_file, inter_binSize=inter_binSize,
                                                             intra_binSize=intra_binSize)
 
     # Determine whether the hi-c matrix file is consistent with the reference file
     for i in range(len(chr_id)):
         for j in range(i, len(chr_id)):
             if i == j:
-                matrix_file = os.path.join(intra_hicfile, name + '_%skb_%s_%s_matrix.txt' % (str(inter_binSize // 1000),
+                matrix_file = os.path.join(intra_hicfile, name + '_%skb_%s_%s_matrix.txt' % (str(intra_binSize // 1000),
                                                                                              chr_id[i], chr_id[j]))
             else:
                 matrix_file = os.path.join(inter_hicfile, name + '_%skb_%s_%s_matrix.txt' % (str(inter_binSize // 1000),
                                                                                              chr_id[i], chr_id[j]))
             if not os.path.exists(matrix_file):
                 print("The required matrix file should exist in the current folder.")
                 return "Matrix file Error."
 
     # the number of chrom
     chr_count = len(chr_id)
     # multi-processing
     p = multiprocessing.Pool(processes=n_cores)
     # i, chr_id, intra_hicfile, inter_hicfile, win, cutoff, name, binSize
     async_results = [p.apply_async(call_intra_sv, args=(i, chr_id, chr_intra_count, chr_inter_count, intra_hicfile,
-                                                        inter_hicfile, win, cutoff, name, intra_binSize,
+                                                        inter_hicfile, win, reg, cutoff, name, intra_binSize,
                                                         inter_binSize, output)) for i in range(chr_count)]
 
     p.close()
     p.join()
 
     for ar in async_results:
         cur_chrom_result = ar.get()
@@ -345,16 +350,17 @@
     if not os.path.exists(output):
         os.makedirs(output)
     ref_file = args.ref
     inter_binSize = args.inter_binsize
     intra_binSize = args.intra_binsize
     win = args.window
     cutoff = args.cutoff
+    reg = args.regularization
     n_cores = args.cores
     intra_hicfile = args.intra_hic
     inter_hicfile = args.inter_hic
     name = args.name
     # ref_file, inter_binSize, intra_binSize, win, cutoff, n_cores, intra_hicfile, inter_hicfile, name, output
-    run_HiSV(ref_file, inter_binSize, intra_binSize, win, cutoff, n_cores, intra_hicfile, inter_hicfile, name, output)
+    run_HiSV(ref_file, inter_binSize, intra_binSize, win, reg, cutoff, n_cores, intra_hicfile, inter_hicfile, name, output)
     end_t = datetime.datetime.now()
     elapsed_sec = (end_t - start_t).total_seconds()
     print("running time: " + "{:.2f}".format(elapsed_sec) + " seconds")
```

## Comparing `hisv-1.0.6.data/scripts/SV_type` & `hisv-1.0.7.data/scripts/SV_type`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
             print("matrix file does not exist.")
             sys.exit(-1)
 
     for i in range(len(chr_list)):
         chrID = chr_list[i]
         matrix_file = os.path.join(hicfile, name + '_%skb_%s_%s_matrix.txt' % (str(binSize // 1000),
                                                                                chrID, chrID))
-        contact_matrix = np.loadtxt(matrix_file)
         normed_coverage = normCove.normalized_coverage(matrix_file, gc_file, mapscore_file, cutsites_file,
                                                        binSize, chrID)
         coverList = coverList.append({'chrom': chrID, 'coverage': normed_coverage}, ignore_index=True)
 
     # Define the type for each SV event
     for i in result.index:
         row = result.loc[i]
```

## Comparing `hisv-1.0.6.data/scripts/determin_breakpoint` & `hisv-1.0.7.data/scripts/determin_breakpoint`

 * *Files identical despite different names*

## Comparing `hisv-1.0.6.data/scripts/hiccovert` & `hisv-1.0.7.data/scripts/hiccovert`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!python
 from optparse import OptionParser
 import hisv.coolToMatrix as coolToM
 import hisv.hicToMatrix as hicToM
 import hisv.bamToMatrix as bamToM
 import os
 import argparse, sys
+import datetime
 
 
 def getargs():
 
     ## Construct an ArgumentParser object for command-line arguments
     parser = argparse.ArgumentParser(description='''Convert Hi-C files in different formats 
                                                     into matrix form as HiSV input.''',
@@ -29,14 +30,15 @@
     if not commands:
         commands.append('-h')
     args = parser.parse_args(commands)
     return args, commands
 
 
 def run():
+    start_t = datetime.datetime.now()
     args, commands = getargs()
     output = args.output
     if not os.path.exists(output):
         os.makedirs(output)
     hicfile = args.hic_file
     ref_file = args.ref
     name = args.name
@@ -62,10 +64,12 @@
         coolToM.coolToMatrix(hicfile, ref_file, binSize, output, name, n_cores)
     elif covert_type == 'cool':
         coolToM.coolToMatrix(hicfile, ref_file, binSize, output, name, n_cores)
     elif covert_type == 'hic':
         hicToM.hicToMatrix(hicfile, binSize, ref_file, output, name, n_cores)
     else:
         bamToM.bamToMatrix(hicfile, ref_file, binSize, output, name, n_cores)
-
+    end_t = datetime.datetime.now()
+    elapsed_sec = (end_t - start_t).total_seconds()
+    print("running time: " + "{:.2f}".format(elapsed_sec) + " seconds")
 if __name__ == '__main__':
     run()
```

## Comparing `hisv-1.0.6.dist-info/LICENSE` & `hisv-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hisv-1.0.6.dist-info/METADATA` & `hisv-1.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hisv
-Version: 1.0.6
+Version: 1.0.7
 Summary: A computational pipeline for structural variation detection from Hi-C data
 Home-page: https://github.com/GaoLabXDU/HiSV
 Author: Li Junping
 Author-email: lijunping02@qq.com
 License: MIT Licence
 Keywords: Hi-C,structural variation,control-free
 Platform: any
```

## Comparing `hisv-1.0.6.dist-info/RECORD` & `hisv-1.0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-hisv/__init__.py,sha256=cx9IFqZJbYCtEUAYGc5Gei7NOlRA1obK1RsRVb7aHsM,141
+hisv/__init__.py,sha256=ZRufjNpdhB5LlCOcHkt4Yut5vE9umWN2y8V8S_Rg0-w,141
 hisv/bamToMatrix.py,sha256=IJCcgOlpp9iggV7cMRGG9ctwGKFyFi6-0BiT38CB6_E,3529
 hisv/combineIntraResult.py,sha256=er2qIdup2f7ninlqGFBoeqMAWm5Hj_8Do3af-Y9lC_A,3338
 hisv/combineResult.py,sha256=3GoHbVlvGwf-6Nms_-klBz4NEs48twmyPOnDojAdL-Q,3331
 hisv/coolToMatrix.py,sha256=CGl3lI0lY7Dn0tLHEOpZgD6Yu85mCr9UlkWv9eUJdZs,3539
 hisv/hicToMatrix.py,sha256=sEpJLdEbI19-bJu9cNwGTmHyUyvbw8ky4_n4oQcKBA8,3344
 hisv/normCove.py,sha256=hVVC_nFL_ZfWcZiqHr0dVi5Df_Vchlia0ZEUc4JHJBY,4448
-hisv-1.0.6.data/scripts/HiSV,sha256=8hHT6mfxUyIfdnAZ6dvaGiIjxpSLHzvltb2NDvPEVHA,15354
-hisv-1.0.6.data/scripts/SV_type,sha256=s_pi-D4tj0FCecUpUs3iYTqw70MX4_E8r9Qy-k0xnYE,6751
-hisv-1.0.6.data/scripts/determin_breakpoint,sha256=Kbl4FgQnO7Xs9aT_wmxLJnkkbleKh-9PztHyrXqcWVg,7907
-hisv-1.0.6.data/scripts/hiccovert,sha256=gQNiZ_QHZI58HE0hBfNqNkye70sDMApwooSbd4vu5yo,2746
-hisv-1.0.6.dist-info/LICENSE,sha256=ttLko2ScLpI7e3qXlcEi7zFe5EySPXa775VTlXhaKxA,1107
-hisv-1.0.6.dist-info/METADATA,sha256=bhouDIxB-YGWlLLVf5vVHtBsQsGNQ5fuWEcvplF9WuA,633
-hisv-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hisv-1.0.6.dist-info/top_level.txt,sha256=x3xGbd2S2y3Rn7jINUhyS0kB2iazRfeJjg3OUHaeUeU,5
-hisv-1.0.6.dist-info/RECORD,,
+hisv-1.0.7.data/scripts/HiSV,sha256=uhOaDKc3cwWRQ6KNHlcJRJGSZTmrp8d3ueDptFmGs1I,15569
+hisv-1.0.7.data/scripts/SV_type,sha256=_eVbyMzL-OYOMtCYy18Mj67Ik3gQJCX6IoM9eQATHLE,6702
+hisv-1.0.7.data/scripts/determin_breakpoint,sha256=Kbl4FgQnO7Xs9aT_wmxLJnkkbleKh-9PztHyrXqcWVg,7907
+hisv-1.0.7.data/scripts/hiccovert,sha256=Z94EYQWKZELH-uK1_FNkIVgElIkkipN_dJRMNJdyF3w,2959
+hisv-1.0.7.dist-info/LICENSE,sha256=ttLko2ScLpI7e3qXlcEi7zFe5EySPXa775VTlXhaKxA,1107
+hisv-1.0.7.dist-info/METADATA,sha256=VjtyoIvIMxlnAvYrPysPPSUxNmoXRY4sHOrGOdpyjac,633
+hisv-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hisv-1.0.7.dist-info/top_level.txt,sha256=x3xGbd2S2y3Rn7jINUhyS0kB2iazRfeJjg3OUHaeUeU,5
+hisv-1.0.7.dist-info/RECORD,,
```

