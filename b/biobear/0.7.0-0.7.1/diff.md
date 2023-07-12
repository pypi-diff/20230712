# Comparing `tmp/biobear-0.7.0.tar.gz` & `tmp/biobear-0.7.1.tar.gz`

## Comparing `biobear-0.7.0.tar` & `biobear-0.7.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.7.0/Cargo.toml
--rw-r--r--   0     1001      123     3295 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/biobear.svg
--rw-r--r--   0     1001      123      100 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/dependabot.yml
--rw-r--r--   0     1001      123     2428 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123      704 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      123      143 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/workflows/smoketest.py
--rw-r--r--   0     1001      123      940 2023-07-10 14:39:40.000000 biobear-0.7.0/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-07-10 14:39:40.000000 biobear-0.7.0/.gitignore
--rw-r--r--   0     1001      123     1606 2023-07-10 14:39:40.000000 biobear-0.7.0/CHANGELOG.md
--rw-r--r--   0     1001      123     1055 2023-07-10 14:39:40.000000 biobear-0.7.0/LICENSE
--rw-r--r--   0     1001      123       68 2023-07-10 14:39:40.000000 biobear-0.7.0/Makefile
--rw-r--r--   0     1001      123      895 2023-07-10 14:39:40.000000 biobear-0.7.0/README.md
--rw-r--r--   0     1001      123      224 2023-07-10 14:39:40.000000 biobear-0.7.0/cz.json
--rw-r--r--   0     1001      123      252 2023-07-10 14:39:40.000000 biobear-0.7.0/docs.bash
--rw-r--r--   0     1001      123      609 2023-07-10 14:39:40.000000 biobear-0.7.0/pyproject.toml
--rw-r--r--   0     1001      123     1299 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/__init__.py
--rw-r--r--   0     1001      123     1829 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123     1883 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      123     1309 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/compression.py
--rw-r--r--   0     1001      123     1520 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123     1516 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      858 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      123     1565 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123     1566 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      123     2338 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/reader.py
--rw-r--r--   0     1001      123     1887 2023-07-10 14:39:40.000000 biobear-0.7.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123   124562 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      123     6152 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     9521 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/index.bcf
--rw-r--r--   0     1001      123      143 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      123     8638 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      213 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.gff
--rw-r--r--   0     1001      123       91 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      123    17994 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.gtf
--rw-r--r--   0     1001      123     1478 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      123     4302 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      816 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123     1615 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_bcf_reader.py
--rw-r--r--   0     1001      123     1729 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123     1380 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      544 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_genbank_reader.py
--rw-r--r--   0     1001      123     1575 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123     1583 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_gtf_reader.py
--rw-r--r--   0     1001      123     1052 2023-07-10 14:39:40.000000 biobear-0.7.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-07-10 14:39:40.000000 biobear-0.7.0/requirements-dev.txt
--rw-r--r--   0     1001      123     3389 2023-07-10 14:39:40.000000 biobear-0.7.0/src/bam_reader.rs
--rw-r--r--   0     1001      123     3226 2023-07-10 14:39:40.000000 biobear-0.7.0/src/bcf_reader.rs
--rw-r--r--   0     1001      123     4488 2023-07-10 14:39:40.000000 biobear-0.7.0/src/exon_reader.rs
--rw-r--r--   0     1001      123      977 2023-07-10 14:39:40.000000 biobear-0.7.0/src/lib.rs
--rw-r--r--   0     1001      123     3226 2023-07-10 14:39:40.000000 biobear-0.7.0/src/vcf_reader.rs
--rw-r--r--   0     1001      123    92476 2023-07-10 14:39:47.000000 biobear-0.7.0/Cargo.lock
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 biobear-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.7.1/Cargo.toml
+-rw-r--r--   0     1001      123     3295 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/biobear.svg
+-rw-r--r--   0     1001      123      100 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2428 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      704 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      143 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      940 2023-07-12 03:44:27.000000 biobear-0.7.1/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-07-12 03:44:27.000000 biobear-0.7.1/.gitignore
+-rw-r--r--   0     1001      123     1653 2023-07-12 03:44:27.000000 biobear-0.7.1/CHANGELOG.md
+-rw-r--r--   0     1001      123     1055 2023-07-12 03:44:27.000000 biobear-0.7.1/LICENSE
+-rw-r--r--   0     1001      123       68 2023-07-12 03:44:27.000000 biobear-0.7.1/Makefile
+-rw-r--r--   0     1001      123      895 2023-07-12 03:44:27.000000 biobear-0.7.1/README.md
+-rw-r--r--   0     1001      123      224 2023-07-12 03:44:27.000000 biobear-0.7.1/cz.json
+-rw-r--r--   0     1001      123      252 2023-07-12 03:44:27.000000 biobear-0.7.1/docs.bash
+-rw-r--r--   0     1001      123      609 2023-07-12 03:44:27.000000 biobear-0.7.1/pyproject.toml
+-rw-r--r--   0     1001      123     1299 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     1829 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123     1883 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      123     1309 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/compression.py
+-rw-r--r--   0     1001      123     1520 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123     1516 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      858 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      123     1565 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123     1566 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      123     2338 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/reader.py
+-rw-r--r--   0     1001      123     1887 2023-07-12 03:44:27.000000 biobear-0.7.1/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123   124562 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      123     6152 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     9521 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/index.bcf
+-rw-r--r--   0     1001      123      143 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      123     8638 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      213 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123    17994 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.gtf
+-rw-r--r--   0     1001      123     1478 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      123     4302 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      816 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1615 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_bcf_reader.py
+-rw-r--r--   0     1001      123     1729 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1380 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      544 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_genbank_reader.py
+-rw-r--r--   0     1001      123     1575 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123     1583 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_gtf_reader.py
+-rw-r--r--   0     1001      123     1052 2023-07-12 03:44:27.000000 biobear-0.7.1/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-07-12 03:44:27.000000 biobear-0.7.1/requirements-dev.txt
+-rw-r--r--   0     1001      123     3389 2023-07-12 03:44:27.000000 biobear-0.7.1/src/bam_reader.rs
+-rw-r--r--   0     1001      123     3226 2023-07-12 03:44:27.000000 biobear-0.7.1/src/bcf_reader.rs
+-rw-r--r--   0     1001      123     4488 2023-07-12 03:44:27.000000 biobear-0.7.1/src/exon_reader.rs
+-rw-r--r--   0     1001      123      977 2023-07-12 03:44:27.000000 biobear-0.7.1/src/lib.rs
+-rw-r--r--   0     1001      123     3226 2023-07-12 03:44:27.000000 biobear-0.7.1/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    92936 2023-07-12 03:44:32.000000 biobear-0.7.1/Cargo.lock
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 biobear-0.7.1/PKG-INFO
```

### Comparing `biobear-0.7.0/.github/biobear.svg` & `biobear-0.7.1/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/.github/workflows/release.yml` & `biobear-0.7.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/.github/workflows/smoke-test.yml` & `biobear-0.7.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/.github/workflows/test.yml` & `biobear-0.7.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/.gitignore` & `biobear-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/CHANGELOG.md` & `biobear-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.7.1 (2023-07-11)
+
+### Feat
+
+- bump exon
+
 ## v0.7.0 (2023-07-10)
 
 ### Feat
 
 - add exhausted check to avoid panic (#43)
 - update exon (#42)
```

### Comparing `biobear-0.7.0/LICENSE` & `biobear-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/README.md` & `biobear-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/pyproject.toml` & `biobear-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/__init__.py` & `biobear-0.7.1/python/biobear/__init__.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/bam_reader.py` & `biobear-0.7.1/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/bcf_reader.py` & `biobear-0.7.1/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/compression.py` & `biobear-0.7.1/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/fasta_reader.py` & `biobear-0.7.1/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/fastq_reader.py` & `biobear-0.7.1/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/genbank_reader.py` & `biobear-0.7.1/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/gff_reader.py` & `biobear-0.7.1/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/gtf_reader.py` & `biobear-0.7.1/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/reader.py` & `biobear-0.7.1/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/biobear/vcf_reader.py` & `biobear-0.7.1/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/BGC0000404.gbk` & `biobear-0.7.1/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/bedcov.bam` & `biobear-0.7.1/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/bedcov.bam.bai` & `biobear-0.7.1/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/file.vcf` & `biobear-0.7.1/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/index.bcf` & `biobear-0.7.1/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/index.vcf.gz` & `biobear-0.7.1/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/test.gtf` & `biobear-0.7.1/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/test.gtf.gz` & `biobear-0.7.1/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/vcf_file.vcf` & `biobear-0.7.1/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.7.1/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_bam_reader.py` & `biobear-0.7.1/python/tests/test_bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_bcf_reader.py` & `biobear-0.7.1/python/tests/test_bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_fasta_reader.py` & `biobear-0.7.1/python/tests/test_fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_fastq_reader.py` & `biobear-0.7.1/python/tests/test_fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_genbank_reader.py` & `biobear-0.7.1/python/tests/test_genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_gff_reader.py` & `biobear-0.7.1/python/tests/test_gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_gtf_reader.py` & `biobear-0.7.1/python/tests/test_gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/python/tests/test_vcf_reader.py` & `biobear-0.7.1/python/tests/test_vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/src/bam_reader.rs` & `biobear-0.7.1/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/src/bcf_reader.rs` & `biobear-0.7.1/src/bcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/src/exon_reader.rs` & `biobear-0.7.1/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/src/lib.rs` & `biobear-0.7.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/src/vcf_reader.rs` & `biobear-0.7.1/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.0/Cargo.lock` & `biobear-0.7.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "indexmap",
+ "indexmap 1.9.3",
  "lexical-core",
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
@@ -656,15 +656,15 @@
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "pyo3",
  "tokio",
 ]
@@ -972,20 +972,20 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown 0.12.3",
+ "hashbrown 0.14.0",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
@@ -1010,15 +1010,15 @@
  "datafusion-physical-expr",
  "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
  "glob",
  "hashbrown 0.14.0",
- "indexmap",
+ "indexmap 1.9.3",
  "itertools 0.11.0",
  "lazy_static",
  "log",
  "num_cpus",
  "object_store",
  "parking_lot",
  "parquet",
@@ -1117,15 +1117,15 @@
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-row",
  "half",
  "hashbrown 0.14.0",
- "indexmap",
+ "indexmap 1.9.3",
  "itertools 0.11.0",
  "lazy_static",
  "libc",
  "md-5",
  "paste",
  "petgraph",
  "rand",
@@ -1190,14 +1190,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "err-derive"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c34a887c8df3ed90498c1c437ce21f211c8e27672921a8ffa293cb8d6d4caa9e"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
@@ -1226,17 +1232,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "exon"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69499b1a5fa88a8bc2cecf6b539ac9894a722828e765526de2db9ac47e576240"
+checksum = "8e4de1173112b783f139d84209b8b0d92be65365bda4e2d52941d81b133de96d"
 dependencies = [
  "arrow",
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "base64",
  "byteorder",
@@ -1452,15 +1458,15 @@
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap",
+ "indexmap 1.9.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1601,15 +1607,15 @@
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d78e1e73ec14cf7375674f74d7dde185c8206fd9dea6fb6295e8a98098aaa97"
 dependencies = [
  "futures-util",
  "http",
  "hyper",
- "rustls 0.21.3",
+ "rustls 0.21.5",
  "tokio",
  "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.57"
@@ -1650,14 +1656,24 @@
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
@@ -1948,17 +1964,17 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "noodles"
-version = "0.40.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc887b6b9f871fe07e545828e7400e547ad84ae8c3cef9a66cf63841dcea79f9"
+checksum = "57213e65425cd2be8923d39ad3cd13c0847949dc9ed3e1bef73f2733d84c0570"
 dependencies = [
  "noodles-bam",
  "noodles-bcf",
  "noodles-bed",
  "noodles-bgzf",
  "noodles-core",
  "noodles-cram",
@@ -1970,51 +1986,50 @@
  "noodles-sam",
  "noodles-tabix",
  "noodles-vcf",
 ]
 
 [[package]]
 name = "noodles-bam"
-version = "0.34.0"
+version = "0.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f8776cf0ea855608b33c7fb57519dcfe1e6400887cdb98ffef9ad9d195f98c"
+checksum = "7fe7adec46a8667c07fa94df7e85994a41b1c03f04e03302629d9024691b2505"
 dependencies = [
  "bit-vec",
  "byteorder",
  "bytes",
  "futures",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
- "noodles-fasta",
  "noodles-sam",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-bcf"
-version = "0.28.0"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eeafbede29abef465759b6557797a33cbe2a8bc17294285817ee6eab2d40342f"
+checksum = "dcf196464f5d391d2199d86f7d8965349c80143414a88676405859c16c75da3a"
 dependencies = [
  "byteorder",
  "futures",
- "indexmap",
+ "indexmap 2.0.0",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-vcf",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-bed"
-version = "0.9.0"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b38ee2f4f77aaa22b9f54c81335f1e874c4c5bba7e1ed7841c594a0b44ff008f"
+checksum = "deba180b7b94c524307da91d5bc983e0ccb9a08c4e24384cc8f93e0210af254a"
 dependencies = [
  "noodles-core",
 ]
 
 [[package]]
 name = "noodles-bgzf"
 version = "0.22.0"
@@ -2029,23 +2044,23 @@
  "pin-project-lite",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "noodles-core"
-version = "0.11.0"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72f9ab09e13392e71797e7502109575d2aae5cb2002bd2304647f7746215c2fe"
+checksum = "94fbe3192fe33acacabaedd387657f39b0fc606f1996d546db0dfe14703b843a"
 
 [[package]]
 name = "noodles-cram"
-version = "0.31.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ad9e48f976e3589764f382a399b1fd4ae637356e4013f70c721e830d7456d3"
+checksum = "6fd08805b7505def607baea746f79ed4138f796cc9de8d665c7c34c8c011ae05"
 dependencies = [
  "async-compression",
  "bitflags 2.3.3",
  "byteorder",
  "bytes",
  "bzip2",
  "flate2",
@@ -2058,31 +2073,31 @@
  "pin-project-lite",
  "tokio",
  "xz2",
 ]
 
 [[package]]
 name = "noodles-csi"
-version = "0.19.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfdb6d7fc962544e61761f95bd6e86e370f3fd2d7c0e76a0d27f56595c9d784b"
+checksum = "55329e145d9b5ba58299e3f9e36512d143e19379f13c3480db7346bcfaadc679"
 dependencies = [
  "bit-vec",
  "byteorder",
- "indexmap",
+ "indexmap 2.0.0",
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-fasta"
-version = "0.23.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642d6f9e977a202d7efee2ee061944af786f5bced0eec977321f5b16bade80ca"
+checksum = "e096096e1c04ab76fe034ea499c692d8a4401a321155b542cd8ea3b1f7d08d12"
 dependencies = [
  "bytes",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
@@ -2096,90 +2111,89 @@
  "futures",
  "memchr",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-gff"
-version = "0.13.0"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af37462bda52596ed525efed54715049dc7a8b63a83653e0846b9aab77a1add2"
+checksum = "112d886335b986e5716de8c02291565813fd3be65053e3f5774b95399434af4f"
 dependencies = [
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "percent-encoding",
 ]
 
 [[package]]
 name = "noodles-gtf"
-version = "0.11.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26791c63a9d6b286631c6a816242237109e578f149426c6f4b18293da4da7016"
+checksum = "096367bb382b244da2dc087a9628daecae299a5641f6572f28627f2001187465"
 dependencies = [
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
 ]
 
 [[package]]
 name = "noodles-sam"
-version = "0.31.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaa33250687c537cc88ae573f264ea9b3352770209134cfa1f047c05c352e724"
+checksum = "40acd01b9fa3935af0c2623ff6c8709c19fe45c0d63bd32931d2cf9939dc690c"
 dependencies = [
  "bitflags 2.3.3",
  "futures",
- "indexmap",
+ "indexmap 2.0.0",
  "lexical-core",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
- "noodles-fasta",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-tabix"
-version = "0.22.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a775d5b16637bbfa0d6bd2a1ff06d4eba409235a5ca9df727a060b785c0f28c5"
+checksum = "9056c1880629bbd50c7737c4d2cffcfb3610045a024776dad5cd606dd88feefc"
 dependencies = [
  "bit-vec",
  "byteorder",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-vcf"
-version = "0.31.0"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a31dbdd18b80ce1918e8862af5b2a303f381a36479d56fd6a3b1df5e5f639ad5"
+checksum = "90ef8021080bdca5eb1328716ed418b0813deb950a244d2faf15e977a565048f"
 dependencies = [
  "futures",
- "indexmap",
+ "indexmap 2.0.0",
  "memchr",
  "nom 7.1.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-tabix",
  "percent-encoding",
  "tokio",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -2405,15 +2419,15 @@
 [[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
- "indexmap",
+ "indexmap 1.9.3",
 ]
 
 [[package]]
 name = "phf"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
@@ -2708,17 +2722,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ab07dc67230e4a4718e70fd5c20055a4334b121f1f9db8fe63ef39ce9b8c846"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
@@ -2735,15 +2749,15 @@
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.3",
+ "rustls 0.21.5",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tokio-rustls 0.24.1",
  "tokio-util",
@@ -2811,17 +2825,17 @@
  "ring",
  "sct",
  "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.3"
+version = "0.21.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b19faa85ecb5197342b54f987b142fb3e30d0c90da40f80ef4fa9a726e6676ed"
+checksum = "79ea77c539259495ce8ca47f53e66ae0330a8819f67e23ac96ca02f50e7b7d36"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2964,17 +2978,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.100"
+version = "1.0.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
+checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3197,17 +3211,17 @@
  "quote",
  "syn 1.0.109",
  "unicode-xid",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "tempfile"
 version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
@@ -3323,15 +3337,15 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.3",
+ "rustls 0.21.5",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `biobear-0.7.0/PKG-INFO` & `biobear-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobear
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow>=12
 License-File: LICENSE
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
 Requires-Python: >=3.8
```

