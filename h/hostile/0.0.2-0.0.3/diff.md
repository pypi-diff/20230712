# Comparing `tmp/hostile-0.0.2.tar.gz` & `tmp/hostile-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostile-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hostile-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hostile-0.0.2.tar` & `hostile-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      672 2023-06-23 11:14:47.624384 hostile-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1971 2023-07-06 18:18:11.923048 hostile-0.0.2/.gitignore
--rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-0.0.2/LICENSE
--rw-r--r--   0        0        0     3584 2023-07-06 18:18:11.923306 hostile-0.0.2/README.md
--rw-r--r--   0        0        0      178 2023-06-21 13:48:03.074531 hostile-0.0.2/environment.yml
--rw-r--r--   0        0        0     5403 2023-07-06 18:18:11.923619 hostile-0.0.2/paper/supplementary-table-1.tsv
--rw-r--r--   0        0        0    39955 2023-07-06 18:18:11.923951 hostile-0.0.2/paper/supplementary-table-2.tsv
--rw-r--r--   0        0        0      647 2023-06-20 13:38:38.854302 hostile-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       46 2023-07-06 18:20:24.201153 hostile-0.0.2/src/hostile/__init__.py
--rw-r--r--   0        0        0     6139 2023-07-06 18:18:11.924322 hostile-0.0.2/src/hostile/aligner.py
--rw-r--r--   0        0        0     2664 2023-06-28 16:38:34.717809 hostile-0.0.2/src/hostile/cli.py
--rw-r--r--   0        0        0     7625 2023-07-06 18:18:11.924493 hostile-0.0.2/src/hostile/lib.py
--rw-r--r--   0        0        0     2809 2023-06-28 17:00:15.389198 hostile-0.0.2/src/hostile/util.py
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-0.0.2/tests/data/MN908947/MN908947.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-0.0.2/tests/data/MN908947/MN908947.2.bt2
--rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-0.0.2/tests/data/MN908947/MN908947.3.bt2
--rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-0.0.2/tests/data/MN908947/MN908947.4.bt2
--rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-0.0.2/tests/data/MN908947/MN908947.fasta.gz
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-0.0.2/tests/data/MN908947/MN908947.rev.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-0.0.2/tests/data/MN908947/MN908947.rev.2.bt2
--rw-r--r--   0        0        0     3562 2023-05-25 19:01:02.910477 hostile-0.0.2/tests/data/h37rv_10.r1.fastq
--rw-r--r--   0        0        0     1508 2023-05-25 19:01:02.910477 hostile-0.0.2/tests/data/h37rv_10.r1.fastq.gz
--rw-r--r--   0        0        0     3562 2023-05-25 19:01:13.127122 hostile-0.0.2/tests/data/h37rv_10.r2.fastq
--rw-r--r--   0        0        0     1501 2023-05-25 19:01:13.127122 hostile-0.0.2/tests/data/h37rv_10.r2.fastq.gz
--rw-r--r--   0        0        0    19004 2023-05-31 15:32:30.691759 hostile-0.0.2/tests/data/human.1k.fa.gz
--rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 hostile-0.0.2/tests/data/human_1_1.fastq.gz
--rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 hostile-0.0.2/tests/data/human_1_2.fastq.gz
--rw-r--r--   0        0        0     3497 2023-07-06 18:18:11.925318 hostile-0.0.2/tests/data/mixed_human_100_1.fastq.gz
--rw-r--r--   0        0        0     3798 2023-07-06 18:18:11.925658 hostile-0.0.2/tests/data/mixed_human_100_2.fastq.gz
--rw-r--r--   0        0        0      239 2023-07-06 18:18:11.925871 hostile-0.0.2/tests/data/tuberculosis_1_1.fastq.gz
--rw-r--r--   0        0        0      232 2023-07-06 18:18:11.926049 hostile-0.0.2/tests/data/tuberculosis_1_2.fastq.gz
--rw-r--r--   0        0        0     1799 2023-06-28 15:12:22.450633 hostile-0.0.2/tests/test_all.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 hostile-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-07-10 14:24:39.989614 hostile-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1840 2023-07-10 14:19:21.498360 hostile-0.0.3/.gitignore
+-rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8865 2023-07-12 15:00:01.077040 hostile-0.0.3/README.md
+-rw-r--r--   0        0        0      199 2023-07-12 08:28:57.211688 hostile-0.0.3/environment.yml
+-rw-r--r--   0        0        0   121111 2023-07-06 23:30:48.068804 hostile-0.0.3/paper/preprint.pdf
+-rw-r--r--   0        0        0     5403 2023-07-06 18:18:11.923619 hostile-0.0.3/paper/supplementary-table-1.tsv
+-rw-r--r--   0        0        0    39955 2023-07-06 18:18:11.923951 hostile-0.0.3/paper/supplementary-table-2.tsv
+-rw-r--r--   0        0        0    95229 2023-07-06 23:30:59.338804 hostile-0.0.3/paper/supplementary-text.pdf
+-rw-r--r--   0        0        0      669 2023-07-12 08:28:40.211794 hostile-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-07-12 15:01:44.689339 hostile-0.0.3/src/hostile/__init__.py
+-rw-r--r--   0        0        0     6952 2023-07-12 14:34:55.899926 hostile-0.0.3/src/hostile/aligner.py
+-rw-r--r--   0        0        0     3981 2023-07-12 14:59:11.724536 hostile-0.0.3/src/hostile/cli.py
+-rw-r--r--   0        0        0    10523 2023-07-12 14:51:23.870446 hostile-0.0.3/src/hostile/lib.py
+-rw-r--r--   0        0        0     2794 2023-07-12 10:56:47.727510 hostile-0.0.3/src/hostile/util.py
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-0.0.3/tests/data/MN908947/MN908947.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-0.0.3/tests/data/MN908947/MN908947.2.bt2
+-rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-0.0.3/tests/data/MN908947/MN908947.3.bt2
+-rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-0.0.3/tests/data/MN908947/MN908947.4.bt2
+-rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-0.0.3/tests/data/MN908947/MN908947.fasta.gz
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-0.0.3/tests/data/MN908947/MN908947.rev.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-0.0.3/tests/data/MN908947/MN908947.rev.2.bt2
+-rw-r--r--   0        0        0      811 2023-07-10 11:24:36.269899 hostile-0.0.3/tests/data/MN908947/partial-for-mask-testing.fa.gz
+-rw-r--r--   0        0        0     3562 2023-05-25 19:01:02.910477 hostile-0.0.3/tests/data/h37rv_10.r1.fastq
+-rw-r--r--   0        0        0     1508 2023-05-25 19:01:02.910477 hostile-0.0.3/tests/data/h37rv_10.r1.fastq.gz
+-rw-r--r--   0        0        0     3562 2023-05-25 19:01:13.127122 hostile-0.0.3/tests/data/h37rv_10.r2.fastq
+-rw-r--r--   0        0        0     1501 2023-05-25 19:01:13.127122 hostile-0.0.3/tests/data/h37rv_10.r2.fastq.gz
+-rw-r--r--   0        0        0    19004 2023-05-31 15:32:30.691759 hostile-0.0.3/tests/data/human.1k.fa.gz
+-rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 hostile-0.0.3/tests/data/human_1_1.fastq.gz
+-rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 hostile-0.0.3/tests/data/human_1_2.fastq.gz
+-rw-r--r--   0        0        0     3497 2023-07-06 18:18:11.925318 hostile-0.0.3/tests/data/mixed_human_100_1.fastq.gz
+-rw-r--r--   0        0        0     3798 2023-07-06 18:18:11.925658 hostile-0.0.3/tests/data/mixed_human_100_2.fastq.gz
+-rw-r--r--   0        0        0      239 2023-07-06 18:18:11.925871 hostile-0.0.3/tests/data/tuberculosis_1_1.fastq.gz
+-rw-r--r--   0        0        0      232 2023-07-06 18:18:11.926049 hostile-0.0.3/tests/data/tuberculosis_1_2.fastq.gz
+-rw-r--r--   0        0        0     6079 2023-07-12 14:51:23.772141 hostile-0.0.3/tests/test_all.py
+-rw-r--r--   0        0        0     9455 1970-01-01 00:00:00.000000 hostile-0.0.3/PKG-INFO
```

### Comparing `hostile-0.0.2/.github/workflows/test.yml` & `hostile-0.0.3/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -15,12 +15,12 @@
         uses: s-weigand/setup-conda@v1
         with:
           update-conda: true
           python-version: ${{ matrix.python-version }}
           conda-channels: conda-forge, bioconda
       - name: Install
         run: |
-          conda install bowtie2 minimap2 samtools gawk
+          conda install bowtie2>=2.5.1 minimap2>=2.26 samtools>=1.17 gawk>=5.1.0 bedtools>=2.31.0
           pip install '.[dev]'
       - name: Test
         run: |
           python -m pytest
```

### Comparing `hostile-0.0.2/.gitignore` & `hostile-0.0.3/.gitignore`

 * *Files 24% similar despite different names*

```diff
@@ -128,13 +128,8 @@
 # Pyre type checker
 .pyre/
 
 .DS_Store
 
 .vscode
 
-test.sam
-tests/data/h37rv_10_2.r1.fastq.gz
-tests/data/h37rv_10_2.r2.fastq.gz
-tests/data/human-index
-tests/data/human-t2t-hla.fa.gz
 tests/data/mtb-jeff
```

### Comparing `hostile-0.0.2/LICENSE` & `hostile-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/paper/supplementary-table-1.tsv` & `hostile-0.0.3/paper/supplementary-table-1.tsv`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/paper/supplementary-table-2.tsv` & `hostile-0.0.3/paper/supplementary-table-2.tsv`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/pyproject.toml` & `hostile-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "hostile"
 authors = [{name = "Bede Constantinides", email = "bedeabc@gmail.com"}]
 license = {file = "LICENSE"}
+readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">=3.10"
 dependencies = [
   "defopt>=6.4.0",
   "httpx>=0.24.1",
   "platformdirs>=3.5.1",
-  "tqdm>=4.65.0"
+  "tqdm>=4.65.0",
 ]
 
 [project.urls]
 Home = "https://github.com/bede/hostile"
 
 [project.scripts]
 hostile = "hostile.cli:main"
```

### Comparing `hostile-0.0.2/src/hostile/aligner.py` & `hostile-0.0.3/src/hostile/aligner.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,119 +25,143 @@
         self.ref_archive_url = f"{self.cdn_base_url}/{self.ref_archive_fn}"
         self.idx_archive_url = f"{self.cdn_base_url}/{self.idx_archive_fn}"
         self.ref_archive_path = self.working_dir / self.ref_archive_fn
         self.idx_archive_path = self.working_dir / self.idx_archive_fn
         self.idx_path = self.working_dir / self.idx_name
         Path(self.working_dir).mkdir(exist_ok=True, parents=True)
 
-    def check(self):
-        logging.info(f"Found {self.name}")
-        if self.name == "Bowtie2":
-            if not all(path.exists() for path in self.idx_paths):
-                self.working_dir.mkdir(exist_ok=True, parents=True)
-                logging.info(f"Fetching human index")
-                util.download(self.idx_archive_url, self.idx_archive_path)
-                util.untar_file(self.idx_archive_path, self.working_dir)
-                self.idx_archive_path.unlink()
-                logging.info(f"Saved human index ({self.idx_path})")
-            else:
-                logging.info(f"Found cached human index ({self.idx_path})")
-        elif self.name == "Minimap2":
-            if not self.ref_archive_path.exists():
-                util.download(self.ref_archive_url, self.ref_archive_path)
-                logging.info(f"Saved human reference ({self.ref_archive_path})")
-            else:
-                logging.info(f"Found cached human reference ({self.ref_archive_path})")
+    def check(self, using_custom_index: bool):
+        """Test aligner and check/download a ref/index if necessary"""
+        if not using_custom_index:  # Check for and if necessary fetch a genome/index
+            if self.name == "Bowtie2":
+                if not all(path.exists() for path in self.idx_paths):
+                    self.working_dir.mkdir(exist_ok=True, parents=True)
+                    logging.info(f"Fetching human index")
+                    util.download(self.idx_archive_url, self.idx_archive_path)
+                    util.untar_file(self.idx_archive_path, self.working_dir)
+                    self.idx_archive_path.unlink()
+                    logging.info(f"Saved human index ({self.idx_path})")
+                else:
+                    logging.info(f"Found cached index ({self.idx_path})")
+            elif self.name == "Minimap2":
+                if not self.ref_archive_path.exists():
+                    util.download(self.ref_archive_url, self.ref_archive_path)
+                    logging.info(f"Saved human reference ({self.ref_archive_path})")
+                else:
+                    logging.info(f"Found cached reference ({self.ref_archive_path})")
         try:
-            util.run(f"{self.bin_path} --help", cwd=self.working_dir)
+            util.run(f"{self.bin_path} --version", cwd=self.working_dir)
         except subprocess.CalledProcessError:
+            logging.warning(f"Failed to execute {self.bin_path}")
             raise RuntimeError(f"Failed to execute {self.bin_path}")
 
     def gen_clean_cmd(
         self,
         fastq: Path,
         out_dir: Path,
-        custom_index: Path | None = None,
-        threads: int = 2,
+        index: Path | None,
+        rename: bool,
+        threads: int,
+        force: bool,
     ) -> str:
         fastq, out_dir = Path(fastq), Path(out_dir)
         out_dir.mkdir(exist_ok=True, parents=True)
         fastq_stem = util.fastq_path_to_stem(fastq)
         fastq_out_path = out_dir / f"{fastq_stem}.clean.fastq.gz"
         count_before_path = out_dir / f"{fastq_stem}.reads_in.txt"
         count_after_path = out_dir / f"{fastq_stem}.reads_out.txt"
-        if custom_index:
-            self.idx_path = Path(custom_index)
-            self.ref_archive_path = Path(custom_index)
-            logging.info(f"Using custom index {custom_index}")
+        if not force and fastq_out_path.exists():
+            raise FileExistsError(
+                f"Output file already exists. Use --force to overwrite"
+            )
+        if index:
+            self.idx_path = Path(index)
+            self.ref_archive_path = Path(index)
+            logging.info(f"Using custom index {index}")
         cmd_template = {  # Templating for Aligner.cmd
             "{BIN_PATH}": str(self.bin_path),
             "{REF_ARCHIVE_PATH}": str(self.ref_archive_path),
             "{INDEX_PATH}": str(self.idx_path),
             "{FASTQ}": str(fastq),
             "{THREADS}": str(threads),
         }
         for k in cmd_template.keys():
             self.cmd = self.cmd.replace(k, cmd_template[k])
+        rename_cmd = (
+            ' | awk \'BEGIN{{FS=OFS="\\t"}} {{$1=int((NR+1)/2)" "; print $0}}\''
+            if rename
+            else ""
+        )
         cmd = (
             # Align, stream reads to stdout in SAM format
             f"{self.cmd}"
             # Count reads in stream before filtering (2048 + 256 = 2304)
             f" | tee >(samtools view -F 2304 -c - > '{count_before_path}')"
             # Discard mapped reads
-            f" | samtools view --threads {int(threads/2)} -f 4 -"
+            f" | samtools view -f 4 -"
             # Count reads in stream after filtering
             f" | tee >(samtools view -F 256 -c - > '{count_after_path}')"
-            # Replace paired read headers with integers
-            f' | awk \'BEGIN{{FS=OFS="\\t"}} {{$1=int((NR+1)/2)" "; print $0}}\''
+            # Optionally replace paired read headers with integers
+            f"{rename_cmd}"
             # Stream remaining records into fastq files
-            f" | samtools fastq --threads {int(threads/2)} -c 6 -0 '{fastq_out_path}'"
+            f" | samtools fastq --threads 2 -c 6 -0 '{fastq_out_path}'"
         )
         logging.debug(f"{cmd}")
         return cmd
 
     def gen_paired_clean_cmd(
         self,
         fastq1: Path,
         fastq2: Path,
         out_dir: Path,
-        custom_index: Path | None = None,
-        threads: int = 2,
+        index: Path | None,
+        rename: bool,
+        threads: int,
+        force: bool,
     ) -> str:
         fastq1, fastq2, out_dir = Path(fastq1), Path(fastq2), Path(out_dir)
         out_dir.mkdir(exist_ok=True, parents=True)
         fastq1_stem = util.fastq_path_to_stem(fastq1)
         fastq2_stem = util.fastq_path_to_stem(fastq2)
         fastq1_out_path = out_dir / f"{fastq1_stem}.clean_1.fastq.gz"
         fastq2_out_path = out_dir / f"{fastq2_stem}.clean_2.fastq.gz"
         count_before_path = out_dir / f"{fastq1_stem}.reads_in.txt"
         count_after_path = out_dir / f"{fastq1_stem}.reads_out.txt"
-        if custom_index:
-            self.idx_path = Path(custom_index)
-            self.ref_archive_path = Path(custom_index)
-            logging.info(f"Using custom index ({custom_index})")
+        if not force and (fastq1_out_path.exists() or fastq2_out_path.exists()):
+            raise FileExistsError(
+                f"Output files already exist. Use --force to overwrite"
+            )
+        if index:
+            self.idx_path = Path(index)
+            self.ref_archive_path = Path(index)
+            logging.info(f"Using custom index ({index})")
         cmd_template = {  # Templating for Aligner.cmd
             "{BIN_PATH}": str(self.bin_path),
             "{REF_ARCHIVE_PATH}": str(self.ref_archive_path),
             "{INDEX_PATH}": str(self.idx_path),
             "{FASTQ1}": str(fastq1),
             "{FASTQ2}": str(fastq2),
             "{THREADS}": str(threads),
         }
         for k in cmd_template.keys():
             self.paired_cmd = self.paired_cmd.replace(k, cmd_template[k])
+        rename_cmd = (
+            f' | awk \'BEGIN{{FS=OFS="\\t"}} {{$1=int((NR+1)/2)" "; print $0}}\''
+            if rename
+            else ""
+        )
         cmd = (
             # Align, stream reads to stdout in SAM format
             f"{self.paired_cmd}"
             # Count reads in stream before filtering (2048 + 256 = 2304)
             f" | tee >(samtools view -F 2304 -c - > '{count_before_path}')"
             # Discard mapped reads and reads with mapped mates
             f" | samtools view -f 12 -"
             # Count reads in stream after filtering
             f" | tee >(samtools view -F 256 -c - > '{count_after_path}')"
-            # Replace paired read headers with integers
-            f' | awk \'BEGIN{{FS=OFS="\\t"}} {{$1=int((NR+1)/2)" "; print $0}}\''
+            # Optionally replace paired read headers with integers
+            f"{rename_cmd}"
             # Stream remaining records into fastq files
             f" | samtools fastq --threads 2 -c 6 -N -1 '{fastq1_out_path}' -2 '{fastq2_out_path}'"
         )
         logging.debug(f"{cmd}")
         return cmd
```

### Comparing `hostile-0.0.2/src/hostile/lib.py` & `hostile-0.0.3/src/hostile/lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+import gzip
 import json
 import multiprocessing
+import shutil
 
 from enum import Enum
 from dataclasses import dataclass
 from pathlib import Path
 
 from platformdirs import user_data_dir
 
@@ -16,15 +18,15 @@
 
 
 CWD = Path.cwd().resolve()
 XDG_DATA_DIR = Path(user_data_dir("hostile", "Bede Constantinides"))
 THREADS = multiprocessing.cpu_count()
 
 
-ALIGNERS = Enum(
+ALIGNER = Enum(
     "Aligner",
     {
         "bowtie2": Aligner(
             name="Bowtie2",
             short_name="bt2",
             bin_path=Path("bowtie2"),
             cdn_base_url=f"https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o",
@@ -58,14 +60,16 @@
         ),
     },
 )
 
 
 @dataclass
 class SampleReport:
+    aligner: str
+    index: str
     fastq1_in_name: str
     fastq1_in_path: str
     fastq1_out_name: str
     fastq1_out_path: str
     reads_in: int
     reads_out: int
     reads_removed: int
@@ -73,15 +77,15 @@
     fastq2_in_name: str | None = None
     fastq2_in_path: str | None = None
     fastq2_out_name: str | None = None
     fastq2_out_path: str | None = None
 
 
 def gather_stats(
-    fastqs: list[Path, Path], out_dir: Path
+    fastqs: list[Path, Path], out_dir: Path, aligner: str, index: Path | None
 ) -> dict[str, dict[str : str | int | float]]:
     stats = []
     for fastq1 in fastqs:
         fastq1_stem = util.fastq_path_to_stem(fastq1)
         fastq1_out_path = out_dir / f"{fastq1_stem}.clean.fastq.gz"
         n_reads_in_path = out_dir / (fastq1_stem + ".reads_in.txt")
         n_reads_out_path = out_dir / (fastq1_stem + ".reads_out.txt")
@@ -90,30 +94,38 @@
         n_reads_removed = n_reads_in - n_reads_out
         n_reads_in_path.unlink()
         n_reads_out_path.unlink()
         try:
             proportion_removed = round(n_reads_removed / n_reads_in, 5)
         except ArithmeticError:  # ZeroDivisionError
             proportion_removed = float(0)
+        index_fmt = (
+            index
+            if index
+            else Path(ALIGNER[aligner].value.working_dir)
+            / Path(ALIGNER[aligner].value.idx_name)
+        )
         report = SampleReport(
+            aligner=aligner,
+            index=str(index_fmt),
             fastq1_in_name=fastq1.name,
             fastq1_in_path=str(fastq1),
             fastq1_out_name=fastq1_out_path.name,
             fastq1_out_path=str(fastq1_out_path),
             reads_in=n_reads_in,
             reads_out=n_reads_out,
             reads_removed=n_reads_removed,
             reads_removed_proportion=proportion_removed,
         ).__dict__
         stats.append({k: v for k, v in report.items() if v is not None})
     return stats
 
 
 def gather_stats_paired(
-    fastqs: list[tuple[Path, Path]], out_dir: Path
+    fastqs: list[tuple[Path, Path]], out_dir: Path, aligner: str, index: Path | None
 ) -> dict[str, dict[str : str | int | float]]:
     stats = []
     for fastq1, fastq2 in fastqs:
         fastq1_stem = util.fastq_path_to_stem(fastq1)
         fastq2_stem = util.fastq_path_to_stem(fastq2)
         fastq1_out_path = out_dir / f"{fastq1_stem}.clean_1.fastq.gz"
         fastq2_out_path = out_dir / f"{fastq2_stem}.clean_2.fastq.gz"
@@ -124,16 +136,24 @@
         n_reads_removed = n_reads_in - n_reads_out
         n_reads_in_path.unlink()
         n_reads_out_path.unlink()
         try:
             proportion_removed = round(n_reads_removed / n_reads_in, 5)
         except ArithmeticError:  # ZeroDivisionError
             proportion_removed = float(0)
+        index_fmt = (
+            index
+            if index
+            else Path(ALIGNER[aligner].value.working_dir)
+            / Path(ALIGNER[aligner].value.idx_name)
+        )
         stats.append(
             SampleReport(
+                aligner=aligner,
+                index=str(index_fmt),
                 fastq1_in_name=fastq1.name,
                 fastq2_in_name=fastq2.name,
                 fastq1_in_path=str(fastq1),
                 fastq2_in_path=str(fastq2),
                 fastq1_out_name=fastq1_out_path.name,
                 fastq2_out_name=fastq2_out_path.name,
                 fastq1_out_path=str(fastq1_out_path),
@@ -143,75 +163,131 @@
                 reads_removed=n_reads_removed,
                 reads_removed_proportion=proportion_removed,
             ).__dict__
         )
     return stats
 
 
+def choose_aligner(preferred_aligner: ALIGNER, using_custom_index: bool) -> ALIGNER:
+    """Fallback to Minimap2 from Bowtie2 if Bowtie2 isn't installed etc"""
+    aligner = preferred_aligner
+    try:
+        aligner.value.check(using_custom_index=using_custom_index)
+    except Exception as e:
+        if aligner == ALIGNER.bowtie2:
+            aligner = ALIGNER.minimap2
+            logging.warning(f"Using Minimap2 instead of Bowtie2")
+            aligner.value.check()
+        else:
+            raise e
+    return aligner
+
+
 def clean_fastqs(
     fastqs: list[Path],
-    custom_index: Path | None = None,
+    index: Path | None = None,
+    rename: bool = False,
     out_dir: Path = CWD,
+    aligner: ALIGNER = ALIGNER.minimap2,
     threads: int = THREADS,
-    aligner: ALIGNERS = ALIGNERS.bowtie2,
+    force: bool = False,
 ):
-    logging.info("Single read input")
+    if aligner == ALIGNER.bowtie2:
+        logging.info("Using Bowtie2")
+    elif aligner == ALIGNER.minimap2:
+        logging.info("Using Minimap2's long read preset (map-ont)")
+    fastqs = [Path(path).resolve() for path in fastqs]
+    if not all(fastq.is_file() for fastq in fastqs):
+        raise FileNotFoundError("One or more fastq files do not exist")
     Path(out_dir).mkdir(exist_ok=True, parents=True)
-    try:
-        aligner.value.check()
-    except Exception as e:
-        print(type(aligner))
-        previous_aligner = aligner.name
-        if aligner == ALIGNERS.bowtie2:
-            aligner = ALIGNERS.minimap2
-        elif aligner == ALIGNERS.minimap2:
-            aligner = ALIGNERS.bowtie2
-        logging.warning(f"Using {aligner.name} instead of {previous_aligner.name}")
-        aligner.value.check()
-
+    aligner = choose_aligner(aligner, using_custom_index=bool(index))
     backend_cmds = {
         fastq: aligner.value.gen_clean_cmd(
-            Path(fastq), custom_index=custom_index, out_dir=out_dir, threads=threads
+            Path(fastq),
+            out_dir=out_dir,
+            index=index,
+            rename=rename,
+            threads=threads,
+            force=force,
         )
         for fastq in fastqs
     }
     logging.info("Cleaning…")
     util.run_bash_parallel(backend_cmds, description="Cleaning")
-    stats = gather_stats(fastqs, out_dir=out_dir)
+    stats = gather_stats(fastqs, out_dir=out_dir, aligner=aligner.name, index=index)
     return stats
 
 
 def clean_paired_fastqs(
     fastqs: list[tuple[Path, Path]],
-    custom_index: Path | None = None,
+    index: Path | None = None,
+    rename: bool = False,
     out_dir: Path = CWD,
+    aligner: ALIGNER = ALIGNER.bowtie2,
     threads: int = THREADS,
-    aligner: ALIGNERS = ALIGNERS.bowtie2,
+    force: bool = False,
 ):
-    logging.info("Paired read input")
+    if aligner == ALIGNER.bowtie2:
+        logging.info("Using Bowtie2")
+    elif aligner == ALIGNER.minimap2:
+        logging.info("Using Minimap2's short read preset (sr)")
+    fastqs = [(Path(path1).resolve(), Path(path2).resolve()) for path1, path2 in fastqs]
+    if not all(path.is_file() for fastq_pair in fastqs for path in fastq_pair):
+        raise FileNotFoundError("One or more fastq files do not exist")
     Path(out_dir).mkdir(exist_ok=True, parents=True)
-    try:
-        aligner.value.check()
-    except Exception as e:
-        print(type(aligner))
-        previous_aligner = aligner.name
-        if aligner == ALIGNERS.bowtie2:
-            aligner = ALIGNERS.minimap2
-        elif aligner == ALIGNERS.minimap2:
-            aligner = ALIGNERS.bowtie2
-        logging.warning(f"Using {aligner.name} instead of {previous_aligner.name}")
-        aligner.value.check()
-
+    aligner = choose_aligner(aligner, using_custom_index=bool(index))
     backend_cmds = {
         p: aligner.value.gen_paired_clean_cmd(
             Path(p[0]),
             Path(p[1]),
-            custom_index=custom_index,
             out_dir=out_dir,
+            index=index,
+            rename=rename,
             threads=threads,
+            force=force,
         )
         for p in fastqs
     }
     logging.info("Cleaning…")
     util.run_bash_parallel(backend_cmds, description="Cleaning")
-    stats = gather_stats_paired(fastqs, out_dir=out_dir)
+    stats = gather_stats_paired(
+        fastqs, out_dir=out_dir, aligner=aligner.name, index=index
+    )
     return stats
+
+
+def mask(
+    reference: Path, target: Path, out_dir=Path("masked"), threads: int = 1
+) -> Path:
+    """Mask a fasta[.gz] reference genome against fasta.[gz] target genomes"""
+    reference_path, target_path = Path(reference), Path(target)
+    out_dir.mkdir(exist_ok=True, parents=True)
+    bed_path = out_dir / "mask.bed"
+    masked_reference_path = out_dir / "masked.fa"
+
+    if reference_path.suffix == ".gz":  # Decompress reference if necessary
+        new_reference_path = out_dir / reference_path.stem
+        logging.info(f"Decompressing reference into {new_reference_path}")
+        with gzip.open(reference_path, "rb") as in_fh:
+            with open(new_reference_path, "wb") as out_fh:
+                shutil.copyfileobj(in_fh, out_fh)
+        reference_path = new_reference_path
+
+    make_cmd = (
+        f"minimap2 -x asm10 -t {threads} '{reference_path}' '{target}'"
+        f" | awk -v OFS='\t' '{{print $6, $8, $9}}'"
+        f" | sort -k1,1 -k2,2n"
+        f" | bedtools merge -i stdin > '{bed_path}'"
+    )
+    logging.info(f"Making mask ({make_cmd=})")
+    make_cmd_run = util.run(make_cmd)
+    logging.info(make_cmd_run.stderr)
+
+    apply_cmd = (
+        f"bedtools maskfasta"
+        f" -fi '{reference_path}' -bed '{bed_path}' -fo '{masked_reference_path}'"
+    )
+    logging.info(f"Applying mask ({apply_cmd=})")
+    apply_cmd_run = util.run(apply_cmd)
+    logging.info(apply_cmd_run.stderr)
+
+    return masked_reference_path
```

### Comparing `hostile-0.0.2/src/hostile/util.py` & `hostile-0.0.3/src/hostile/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import concurrent.futures
-import logging
 import subprocess
 import tarfile
 
 from functools import partial
 from pathlib import Path
 
 import httpx
```

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.1.bt2` & `hostile-0.0.3/tests/data/MN908947/MN908947.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.2.bt2` & `hostile-0.0.3/tests/data/MN908947/MN908947.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.4.bt2` & `hostile-0.0.3/tests/data/MN908947/MN908947.4.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.fasta.gz` & `hostile-0.0.3/tests/data/MN908947/MN908947.fasta.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.rev.1.bt2` & `hostile-0.0.3/tests/data/MN908947/MN908947.rev.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/MN908947/MN908947.rev.2.bt2` & `hostile-0.0.3/tests/data/MN908947/MN908947.rev.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/h37rv_10.r1.fastq` & `hostile-0.0.3/tests/data/h37rv_10.r1.fastq`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/h37rv_10.r1.fastq.gz` & `hostile-0.0.3/tests/data/h37rv_10.r1.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/h37rv_10.r2.fastq` & `hostile-0.0.3/tests/data/h37rv_10.r2.fastq`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/h37rv_10.r2.fastq.gz` & `hostile-0.0.3/tests/data/h37rv_10.r2.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/human.1k.fa.gz` & `hostile-0.0.3/tests/data/human.1k.fa.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/mixed_human_100_1.fastq.gz` & `hostile-0.0.3/tests/data/mixed_human_100_1.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.2/tests/data/mixed_human_100_2.fastq.gz` & `hostile-0.0.3/tests/data/mixed_human_100_2.fastq.gz`

 * *Files identical despite different names*

