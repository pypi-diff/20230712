# Comparing `tmp/luna-0.13.0.tar.gz` & `tmp/luna-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/luna-0.13.0.tar", last modified: Sat May  6 21:57:40 2023, max compression
+gzip compressed data, was "dist/luna-0.13.1.tar", last modified: Wed Jul 12 12:21:01 2023, max compression
```

## Comparing `luna-0.13.0.tar` & `luna-0.13.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1203 2022-04-11 17:24:17.000000 luna-0.13.0/LICENSE
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      142 2023-05-06 18:48:23.000000 luna-0.13.0/MANIFEST.in
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-05-06 21:57:40.000000 luna-0.13.0/PKG-INFO
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4647 2023-05-06 18:48:23.000000 luna-0.13.0/README.rst
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/MyBio/
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/MyBio/PDB/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4087 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/AbstractPropertyMap.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12801 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Atom.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5593 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Chain.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19116 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/DSSP.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2695 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Dice.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11663 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Entity.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13625 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/FTMapParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9923 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/FragmentMapper.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11628 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/HSExposure.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2306 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/MMCIF2Dict.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    18386 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/MMCIFParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2614 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Model.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7538 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/NACCESS.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5146 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/NeighborSearch.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      556 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PDBExceptions.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14988 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/PDBIO.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20725 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PDBList.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22906 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/PDBParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3339 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PSEA.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14359 2023-04-21 12:53:04.000000 luna-0.13.0/luna/MyBio/PDB/Polypeptide.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10871 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Residue.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    23405 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/ResidueDepth.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2949 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Selection.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1917 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Structure.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3573 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/StructureAlignment.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14154 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/StructureBuilder.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2265 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Superimposer.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9473 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Vector.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2101 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8731 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/parse_pdb_header.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2917 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/extractor.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9607 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/neighbors.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3608 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/selector.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19698 2023-05-06 20:52:29.000000 luna-0.13.0/luna/MyBio/util.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      954 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/version_control.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       83 2022-04-11 17:24:17.000000 luna-0.13.0/luna/__init__.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/align/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/align/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9316 2023-05-06 17:09:37.000000 luna-0.13.0/luna/align/tmalign.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/analysis/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/analysis/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6778 2023-05-06 17:09:37.000000 luna-0.13.0/luna/analysis/residues.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3165 2023-05-06 17:09:37.000000 luna-0.13.0/luna/analysis/summary.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/config/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-05 18:25:54.000000 luna-0.13.0/luna/config/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1008 2022-10-05 18:25:54.000000 luna-0.13.0/luna/config/default.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20345 2023-05-06 18:48:23.000000 luna-0.13.0/luna/config/params.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/data/
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/data/.ipynb_checkpoints/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1702 2023-04-28 13:49:04.000000 luna-0.13.0/luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6803 2022-04-11 17:24:17.000000 luna-0.13.0/luna/data/BaseFeatures.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6982 2023-04-10 15:02:48.000000 luna-0.13.0/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    33752 2023-05-06 17:09:37.000000 luna-0.13.0/luna/data/LUNA.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1669 2022-04-11 17:24:17.000000 luna-0.13.0/luna/data/MinimalFeatures.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)  4170251 2022-04-11 17:24:18.000000 luna-0.13.0/luna/data/ligand_expo.tsv
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9049 2022-07-13 19:01:51.000000 luna-0.13.0/luna/data/precomputed_residue_atom_features.json
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)   102236 2023-05-06 17:09:37.000000 luna-0.13.0/luna/data/precomputed_residue_data.json
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/docking/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/__init__.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/docking/dock6/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4184 2023-05-06 21:26:36.000000 luna-0.13.0/luna/docking/dock6/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4705 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/default.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11148 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/ligands.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1623 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/params.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/interaction/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/interaction/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2434 2022-10-05 18:25:54.000000 luna-0.13.0/luna/interaction/bind.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)   157331 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/calc.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7066 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/config.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2951 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/config.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14309 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/contact.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1721 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/cov.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      308 2022-10-05 18:25:54.000000 luna-0.13.0/luna/interaction/filter.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    27574 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/filter.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/interaction/fp/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/interaction/fp/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    42211 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/fp/fingerprint.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    52388 2023-05-06 19:42:57.000000 luna-0.13.0/luna/interaction/fp/shell.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      542 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/fp/type.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6724 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/fp/view.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20615 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/type.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11615 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/view.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/mol/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/mol/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10165 2023-05-06 18:48:23.000000 luna-0.13.0/luna/mol/atom.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5464 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/charge_model.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4678 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/clustering.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7793 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/depiction.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56156 2023-05-06 18:48:23.000000 luna-0.13.0/luna/mol/entry.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9823 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/features.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13252 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/fingerprint.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56203 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/groups.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1149 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/precomp_data.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    55074 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/standardiser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4744 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/templates.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22804 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/validator.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    64690 2023-05-06 17:09:37.000000 luna-0.13.0/luna/projects.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19360 2023-05-06 18:48:23.000000 luna-0.13.0/luna/run.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/util/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6256 2022-10-05 18:25:54.000000 luna-0.13.0/luna/util/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2185 2023-05-06 18:48:23.000000 luna-0.13.0/luna/util/config.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9496 2023-05-06 20:09:15.000000 luna-0.13.0/luna/util/default_values.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1580 2023-05-06 19:59:06.000000 luna-0.13.0/luna/util/exceptions.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11071 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/file.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10054 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/jobs.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      433 2022-10-05 18:25:54.000000 luna-0.13.0/luna/util/logging.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3590 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/logging.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      183 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/logging_ini.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2728 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/math.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3294 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/multiprocessing_logging.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8153 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/progress_tracker.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6386 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/stringcase.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      762 2023-05-06 18:09:52.000000 luna-0.13.0/luna/version.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/wrappers/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4003 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/antechamber.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    36639 2023-05-06 20:48:45.000000 luna-0.13.0/luna/wrappers/base.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2123 2022-10-06 13:43:51.000000 luna-0.13.0/luna/wrappers/cgo_arrow.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/chemaxon/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chemaxon/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6300 2023-05-06 21:03:44.000000 luna-0.13.0/luna/wrappers/chemaxon/conformer.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2727 2023-05-06 20:05:05.000000 luna-0.13.0/luna/wrappers/chemaxon/stereoisomers.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8454 2023-05-06 20:04:50.000000 luna-0.13.0/luna/wrappers/chemaxon/tautomers.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      281 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chemaxon/util.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/chimera/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1558 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chimera/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1395 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chimera/add_charges.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1628 2022-04-11 17:24:18.000000 luna-0.13.0/luna/wrappers/cif.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7313 2023-05-06 20:44:51.000000 luna-0.13.0/luna/wrappers/obabel.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    37884 2023-05-06 17:09:37.000000 luna-0.13.0/luna/wrappers/pymol.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14407 2023-05-06 17:09:37.000000 luna-0.13.0/luna/wrappers/rdkit.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna.egg-info/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/PKG-INFO
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3384 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/SOURCES.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        1 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/dependency_links.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       43 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/entry_points.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      127 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/requires.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        5 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/top_level.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       38 2023-05-06 21:57:40.000000 luna-0.13.0/setup.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3071 2022-04-11 17:24:18.000000 luna-0.13.0/setup.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1203 2022-04-11 17:24:17.000000 luna-0.13.1/LICENSE
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      142 2023-05-06 18:48:23.000000 luna-0.13.1/MANIFEST.in
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-07-12 12:21:01.000000 luna-0.13.1/PKG-INFO
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4647 2023-05-06 18:48:23.000000 luna-0.13.1/README.rst
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/MyBio/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/MyBio/PDB/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4087 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/AbstractPropertyMap.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12801 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/PDB/Atom.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5593 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Chain.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19116 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/DSSP.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2695 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Dice.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11663 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Entity.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13625 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/FTMapParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9923 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/FragmentMapper.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11628 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/HSExposure.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2306 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/MMCIF2Dict.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    18386 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/MMCIFParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2614 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/PDB/Model.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7538 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/NACCESS.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5146 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/NeighborSearch.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      556 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/PDBExceptions.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14988 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/PDB/PDBIO.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20725 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/PDBList.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22906 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/PDB/PDBParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3339 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/PSEA.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14359 2023-04-21 12:53:04.000000 luna-0.13.1/luna/MyBio/PDB/Polypeptide.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10871 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/PDB/Residue.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    23405 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/ResidueDepth.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2949 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Selection.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1917 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Structure.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3573 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/StructureAlignment.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14154 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/StructureBuilder.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2265 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Superimposer.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9473 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/Vector.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2101 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8731 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/PDB/parse_pdb_header.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2917 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/extractor.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9607 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/neighbors.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3608 2023-05-06 17:09:37.000000 luna-0.13.1/luna/MyBio/selector.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19698 2023-05-06 20:52:29.000000 luna-0.13.1/luna/MyBio/util.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      954 2022-04-11 17:24:17.000000 luna-0.13.1/luna/MyBio/version_control.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       83 2022-04-11 17:24:17.000000 luna-0.13.1/luna/__init__.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/align/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.1/luna/align/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9316 2023-05-06 17:09:37.000000 luna-0.13.1/luna/align/tmalign.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/analysis/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.1/luna/analysis/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6778 2023-05-06 17:09:37.000000 luna-0.13.1/luna/analysis/residues.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3165 2023-05-06 17:09:37.000000 luna-0.13.1/luna/analysis/summary.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/config/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-05 18:25:54.000000 luna-0.13.1/luna/config/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1008 2022-10-05 18:25:54.000000 luna-0.13.1/luna/config/default.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20345 2023-07-12 12:12:53.000000 luna-0.13.1/luna/config/params.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/data/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/data/.ipynb_checkpoints/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1702 2023-04-28 13:49:04.000000 luna-0.13.1/luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6803 2022-04-11 17:24:17.000000 luna-0.13.1/luna/data/BaseFeatures.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6982 2023-04-10 15:02:48.000000 luna-0.13.1/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    33752 2023-05-06 17:09:37.000000 luna-0.13.1/luna/data/LUNA.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1669 2022-04-11 17:24:17.000000 luna-0.13.1/luna/data/MinimalFeatures.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)  4170251 2022-04-11 17:24:18.000000 luna-0.13.1/luna/data/ligand_expo.tsv
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9049 2022-07-13 19:01:51.000000 luna-0.13.1/luna/data/precomputed_residue_atom_features.json
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)   102236 2023-05-06 17:09:37.000000 luna-0.13.1/luna/data/precomputed_residue_data.json
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/docking/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.1/luna/docking/__init__.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/docking/dock6/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4184 2023-07-12 12:14:24.000000 luna-0.13.1/luna/docking/dock6/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4705 2023-05-06 19:59:06.000000 luna-0.13.1/luna/docking/dock6/default.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11154 2023-07-12 12:14:24.000000 luna-0.13.1/luna/docking/dock6/ligands.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1623 2023-05-06 19:59:06.000000 luna-0.13.1/luna/docking/dock6/params.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/interaction/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.1/luna/interaction/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2434 2022-10-05 18:25:54.000000 luna-0.13.1/luna/interaction/bind.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)   157331 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/calc.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7066 2023-05-06 17:09:37.000000 luna-0.13.1/luna/interaction/config.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2951 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/config.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14309 2023-05-06 17:09:37.000000 luna-0.13.1/luna/interaction/contact.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1721 2023-05-06 17:09:37.000000 luna-0.13.1/luna/interaction/cov.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      308 2022-10-05 18:25:54.000000 luna-0.13.1/luna/interaction/filter.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    27574 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/filter.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/interaction/fp/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.1/luna/interaction/fp/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    42211 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/fp/fingerprint.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    52388 2023-05-06 19:42:57.000000 luna-0.13.1/luna/interaction/fp/shell.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      542 2023-05-06 17:09:37.000000 luna-0.13.1/luna/interaction/fp/type.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6724 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/fp/view.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20615 2023-05-06 17:09:37.000000 luna-0.13.1/luna/interaction/type.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11615 2023-05-06 18:48:23.000000 luna-0.13.1/luna/interaction/view.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/mol/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.1/luna/mol/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10165 2023-05-06 18:48:23.000000 luna-0.13.1/luna/mol/atom.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5464 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/charge_model.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4678 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/clustering.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7793 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/depiction.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56355 2023-07-12 12:14:24.000000 luna-0.13.1/luna/mol/entry.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9823 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/features.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13252 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/fingerprint.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56203 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/groups.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1149 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/precomp_data.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    55074 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/standardiser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4744 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/templates.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22804 2023-05-06 17:09:37.000000 luna-0.13.1/luna/mol/validator.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    64690 2023-05-06 17:09:37.000000 luna-0.13.1/luna/projects.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19360 2023-07-12 12:13:49.000000 luna-0.13.1/luna/run.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/util/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6256 2022-10-05 18:25:54.000000 luna-0.13.1/luna/util/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2185 2023-05-06 18:48:23.000000 luna-0.13.1/luna/util/config.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9496 2023-05-06 20:09:15.000000 luna-0.13.1/luna/util/default_values.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1580 2023-05-06 19:59:06.000000 luna-0.13.1/luna/util/exceptions.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11071 2023-05-06 17:09:37.000000 luna-0.13.1/luna/util/file.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10054 2023-05-06 17:09:37.000000 luna-0.13.1/luna/util/jobs.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      433 2022-10-05 18:25:54.000000 luna-0.13.1/luna/util/logging.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3590 2023-05-06 17:09:37.000000 luna-0.13.1/luna/util/logging.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      183 2022-04-11 17:24:18.000000 luna-0.13.1/luna/util/logging_ini.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2728 2022-04-11 17:24:18.000000 luna-0.13.1/luna/util/math.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3294 2023-05-06 17:09:37.000000 luna-0.13.1/luna/util/multiprocessing_logging.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8153 2023-05-06 17:09:37.000000 luna-0.13.1/luna/util/progress_tracker.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6386 2022-04-11 17:24:18.000000 luna-0.13.1/luna/util/stringcase.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      762 2023-07-12 12:15:59.000000 luna-0.13.1/luna/version.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/wrappers/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.1/luna/wrappers/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4003 2023-05-06 19:59:06.000000 luna-0.13.1/luna/wrappers/antechamber.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    36639 2023-05-06 20:48:45.000000 luna-0.13.1/luna/wrappers/base.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2123 2022-10-06 13:43:51.000000 luna-0.13.1/luna/wrappers/cgo_arrow.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/wrappers/chemaxon/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.1/luna/wrappers/chemaxon/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6300 2023-05-06 21:03:44.000000 luna-0.13.1/luna/wrappers/chemaxon/conformer.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2727 2023-05-06 20:05:05.000000 luna-0.13.1/luna/wrappers/chemaxon/stereoisomers.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8454 2023-05-06 20:04:50.000000 luna-0.13.1/luna/wrappers/chemaxon/tautomers.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      281 2023-05-06 19:59:06.000000 luna-0.13.1/luna/wrappers/chemaxon/util.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna/wrappers/chimera/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1625 2023-07-12 12:14:24.000000 luna-0.13.1/luna/wrappers/chimera/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1395 2023-05-06 19:59:06.000000 luna-0.13.1/luna/wrappers/chimera/add_charges.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1628 2022-04-11 17:24:18.000000 luna-0.13.1/luna/wrappers/cif.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7313 2023-05-06 20:44:51.000000 luna-0.13.1/luna/wrappers/obabel.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    37884 2023-05-06 17:09:37.000000 luna-0.13.1/luna/wrappers/pymol.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14407 2023-05-06 17:09:37.000000 luna-0.13.1/luna/wrappers/rdkit.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/PKG-INFO
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3384 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/SOURCES.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        1 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/dependency_links.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       43 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/entry_points.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      127 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/requires.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        5 2023-07-12 12:21:01.000000 luna-0.13.1/luna.egg-info/top_level.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       38 2023-07-12 12:21:01.000000 luna-0.13.1/setup.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3071 2022-04-11 17:24:18.000000 luna-0.13.1/setup.py
```

### Comparing `luna-0.13.0/LICENSE` & `luna-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/PKG-INFO` & `luna-0.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: luna
-Version: 0.13.0
+Version: 0.13.1
 Summary: LUNA: drug discovery toolkit
 Home-page: https://github.com/keiserlab/LUNA
-Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.0
+Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.1
 Author: Alexandre Fassio
 Author-email: afassio@keiserlab.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/keiserlab/LUNA/issues
 Project-URL: Source, https://github.com/keiserlab/LUNA/
 Keywords: luna eifp fifp hifp ifp interaction fingerprint protein-ligand molecule docking
 Platform: UNKNOWN
```

### Comparing `luna-0.13.0/README.rst` & `luna-0.13.1/README.rst`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/AbstractPropertyMap.py` & `luna-0.13.1/luna/MyBio/PDB/AbstractPropertyMap.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Atom.py` & `luna-0.13.1/luna/MyBio/PDB/Atom.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Chain.py` & `luna-0.13.1/luna/MyBio/PDB/Chain.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/DSSP.py` & `luna-0.13.1/luna/MyBio/PDB/DSSP.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Dice.py` & `luna-0.13.1/luna/MyBio/PDB/Dice.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Entity.py` & `luna-0.13.1/luna/MyBio/PDB/Entity.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/FTMapParser.py` & `luna-0.13.1/luna/MyBio/PDB/FTMapParser.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/FragmentMapper.py` & `luna-0.13.1/luna/MyBio/PDB/FragmentMapper.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/HSExposure.py` & `luna-0.13.1/luna/MyBio/PDB/HSExposure.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/MMCIF2Dict.py` & `luna-0.13.1/luna/MyBio/PDB/MMCIF2Dict.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/MMCIFParser.py` & `luna-0.13.1/luna/MyBio/PDB/MMCIFParser.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Model.py` & `luna-0.13.1/luna/MyBio/PDB/Model.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/NACCESS.py` & `luna-0.13.1/luna/MyBio/PDB/NACCESS.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/NeighborSearch.py` & `luna-0.13.1/luna/MyBio/PDB/NeighborSearch.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/PDBExceptions.py` & `luna-0.13.1/luna/MyBio/PDB/PDBExceptions.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/PDBIO.py` & `luna-0.13.1/luna/MyBio/PDB/PDBIO.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/PDBList.py` & `luna-0.13.1/luna/MyBio/PDB/PDBList.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/PDBParser.py` & `luna-0.13.1/luna/MyBio/PDB/PDBParser.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/PSEA.py` & `luna-0.13.1/luna/MyBio/PDB/PSEA.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Polypeptide.py` & `luna-0.13.1/luna/MyBio/PDB/Polypeptide.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Residue.py` & `luna-0.13.1/luna/MyBio/PDB/Residue.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/ResidueDepth.py` & `luna-0.13.1/luna/MyBio/PDB/ResidueDepth.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Selection.py` & `luna-0.13.1/luna/MyBio/PDB/Selection.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Structure.py` & `luna-0.13.1/luna/MyBio/PDB/Structure.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/StructureAlignment.py` & `luna-0.13.1/luna/MyBio/PDB/StructureAlignment.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/StructureBuilder.py` & `luna-0.13.1/luna/MyBio/PDB/StructureBuilder.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Superimposer.py` & `luna-0.13.1/luna/MyBio/PDB/Superimposer.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/Vector.py` & `luna-0.13.1/luna/MyBio/PDB/Vector.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/__init__.py` & `luna-0.13.1/luna/MyBio/PDB/__init__.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/PDB/parse_pdb_header.py` & `luna-0.13.1/luna/MyBio/PDB/parse_pdb_header.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/extractor.py` & `luna-0.13.1/luna/MyBio/extractor.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/neighbors.py` & `luna-0.13.1/luna/MyBio/neighbors.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/selector.py` & `luna-0.13.1/luna/MyBio/selector.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/util.py` & `luna-0.13.1/luna/MyBio/util.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/MyBio/version_control.py` & `luna-0.13.1/luna/MyBio/version_control.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/align/tmalign.py` & `luna-0.13.1/luna/align/tmalign.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/analysis/residues.py` & `luna-0.13.1/luna/analysis/residues.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/analysis/summary.py` & `luna-0.13.1/luna/analysis/summary.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/config/default.cfg` & `luna-0.13.1/luna/config/default.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/config/params.py` & `luna-0.13.1/luna/config/params.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `luna-0.13.1/luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/BaseFeatures.fdef` & `luna-0.13.1/luna/data/BaseFeatures.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef` & `luna-0.13.1/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/LUNA.fdef` & `luna-0.13.1/luna/data/LUNA.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/MinimalFeatures.fdef` & `luna-0.13.1/luna/data/MinimalFeatures.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/ligand_expo.tsv` & `luna-0.13.1/luna/data/ligand_expo.tsv`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/precomputed_residue_atom_features.json` & `luna-0.13.1/luna/data/precomputed_residue_atom_features.json`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/data/precomputed_residue_data.json` & `luna-0.13.1/luna/data/precomputed_residue_data.json`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/docking/dock6/__init__.py` & `luna-0.13.1/luna/docking/dock6/__init__.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/docking/dock6/default.cfg` & `luna-0.13.1/luna/docking/dock6/default.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/docking/dock6/ligands.py` & `luna-0.13.1/luna/docking/dock6/ligands.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             ligand_file = None
             logger.exception(e)
             raise
 
         # Safe finish: set back the working directory to its initial value.
         finally:
             os.chdir(cur_path)
-            if ligand_file and os.path.exists(ligand_file):
-                os.rename(ligand_file, Path(output_file).absolute())
-            remove_directory(tmp_path)
+            # if ligand_file and os.path.exists(ligand_file):
+            #     os.rename(ligand_file, Path(output_file).absolute())
+            # remove_directory(tmp_path)
 
     def to_canonical_form(self, ligand_input):
         return convert_molecule(ligand_input, input_format="smi",
                                 output_format="can")
 
     def add_h_to_ligand(self, ligand_input):
         # If it is a string, but not a file path.
```

### Comparing `luna-0.13.0/luna/docking/dock6/params.py` & `luna-0.13.1/luna/docking/dock6/params.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/bind.cfg` & `luna-0.13.1/luna/interaction/bind.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/calc.py` & `luna-0.13.1/luna/interaction/calc.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/config.cfg` & `luna-0.13.1/luna/interaction/config.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/config.py` & `luna-0.13.1/luna/interaction/config.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/contact.py` & `luna-0.13.1/luna/interaction/contact.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/cov.py` & `luna-0.13.1/luna/interaction/cov.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/filter.py` & `luna-0.13.1/luna/interaction/filter.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/fp/fingerprint.py` & `luna-0.13.1/luna/interaction/fp/fingerprint.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/fp/shell.py` & `luna-0.13.1/luna/interaction/fp/shell.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/fp/type.py` & `luna-0.13.1/luna/interaction/fp/type.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/fp/view.py` & `luna-0.13.1/luna/interaction/fp/view.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/type.py` & `luna-0.13.1/luna/interaction/type.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/interaction/view.py` & `luna-0.13.1/luna/interaction/view.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/atom.py` & `luna-0.13.1/luna/mol/atom.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/charge_model.py` & `luna-0.13.1/luna/mol/charge_model.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/clustering.py` & `luna-0.13.1/luna/mol/clustering.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/depiction.py` & `luna-0.13.1/luna/mol/depiction.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/entry.py` & `luna-0.13.1/luna/mol/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,18 +289,20 @@
             Pathname of the molecular file.
 
             .. note::
                 Mandatory if there is any line containing only the ligand name.
                 This only applies to ligands that will be read from
                 multimolecular files.
         entries_sep : str
-            a separator for entries whose molecules lie all in the same PDB
-            file, not requiring, therefore, an additional molecular file.
-            Such entries cause the function to yield `ChainEntry` or
-            `MolEntry` objects. Default: ':'. E.g.: 3QQK:A:X02:497.
+            a separator for entries. For complexes where the ligand and the 
+            protein structure lie all in the same PDB file (e.g., complexes 
+            from the RCSB PDB), the separator must be the same used for 
+            entries provided at `input_file`. 
+            Default: ':'. E.g.: 3QQK:A:X02:497 or receptor:ZINC000649623159
+
         fields_sep : str
             a character used to separate fields in ``input_file`` for
             complexes whose protein structure is in a PDB file and
             whose ligand is on a molecular file. Such entries cause the
             function to yield `MolFileEntry` objects. Default: ','
 
             Each line should contain either the ligand name only or the
@@ -370,14 +372,15 @@
                                    f"in line #{c}. In this case, "
                                    "'pdb_id' and 'mol_file' are mandatory.")
                             raise IllegalArgumentError(msg)
 
                         yield MolFileEntry.from_mol_file(pdb_id, args[0],
                                                          mol_file,
                                                          is_multimol_file=True,
+                                                         sep=entries_sep,
                                                          **kwargs)
 
                     elif len(args) == 2:
                         yield ChainEntry.from_string(row, sep=entries_sep)
 
                     elif len(args) == 4:
                         yield MolEntry.from_string(row, sep=entries_sep)
@@ -390,14 +393,15 @@
                         curr_mol_file, is_multimol) = args
                     is_multimol = ast.literal_eval(is_multimol)
 
                     cls = MolFileEntry
                     yield cls.from_mol_file(curr_pdb_id, curr_mol_id,
                                             curr_mol_file,
                                             is_multimol_file=is_multimol,
+                                            sep=entries_sep,
                                             **kwargs)
                 else:
                     has_error = True
 
                 if has_error:
                     msg = (f"Invalid number of arguments found in line #{c}. "
                            "You should provide either one or four arguments. "
```

### Comparing `luna-0.13.0/luna/mol/features.py` & `luna-0.13.1/luna/mol/features.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/fingerprint.py` & `luna-0.13.1/luna/mol/fingerprint.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/groups.py` & `luna-0.13.1/luna/mol/groups.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/precomp_data.py` & `luna-0.13.1/luna/mol/precomp_data.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/standardiser.py` & `luna-0.13.1/luna/mol/standardiser.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/templates.py` & `luna-0.13.1/luna/mol/templates.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/mol/validator.py` & `luna-0.13.1/luna/mol/validator.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/projects.py` & `luna-0.13.1/luna/projects.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/run.py` & `luna-0.13.1/luna/run.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/__init__.py` & `luna-0.13.1/luna/util/__init__.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/config.py` & `luna-0.13.1/luna/util/config.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/default_values.py` & `luna-0.13.1/luna/util/default_values.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/exceptions.py` & `luna-0.13.1/luna/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/file.py` & `luna-0.13.1/luna/util/file.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/jobs.py` & `luna-0.13.1/luna/util/jobs.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/logging.py` & `luna-0.13.1/luna/util/logging.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/math.py` & `luna-0.13.1/luna/util/math.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/multiprocessing_logging.py` & `luna-0.13.1/luna/util/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/progress_tracker.py` & `luna-0.13.1/luna/util/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/util/stringcase.py` & `luna-0.13.1/luna/util/stringcase.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/version.py` & `luna-0.13.1/luna/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
        - MINOR stands for updates that "break" the compatibility
             between pharmacophoric perception, interactions,
             and interaction fingerprints;
 
        - PATCH stands for backward compatible bug fixes.
 """
-version_info = (0, 13, 0)
+version_info = (0, 13, 1)
 version = '.'.join(str(c) for c in version_info)
 __version__ = version
 
 
 def has_version_compatibility(v):
     version_to_check = v
     if isinstance(v, str):
```

### Comparing `luna-0.13.0/luna/wrappers/antechamber.py` & `luna-0.13.1/luna/wrappers/antechamber.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/base.py` & `luna-0.13.1/luna/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/cgo_arrow.py` & `luna-0.13.1/luna/wrappers/cgo_arrow.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/chemaxon/conformer.py` & `luna-0.13.1/luna/wrappers/chemaxon/conformer.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/chemaxon/stereoisomers.py` & `luna-0.13.1/luna/wrappers/chemaxon/stereoisomers.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/chemaxon/tautomers.py` & `luna-0.13.1/luna/wrappers/chemaxon/tautomers.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/chimera/__init__.py` & `luna-0.13.1/luna/wrappers/chimera/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 from subprocess import Popen, PIPE
-from os.path import exists
+import os
 
 from luna.util.exceptions import IllegalArgumentError, ProcessingFailed
 from luna.wrappers.chimera.add_charges import CHARGE_METHODS
 from luna.util.file import is_file_valid
 
 
 import logging
@@ -22,25 +22,31 @@
     if not isinstance(output_file, str):
         raise IllegalArgumentError("'output_file' must be a string.")
 
     if charge_method not in CHARGE_METHODS:
         raise IllegalArgumentError("The charge method '%s' is not "
                                    "accepted by Chimera." % charge_method)
 
-    script = str(Path(__file__).parent) + "/add_charges.py"
+    cur_path = os.path.abspath(os.getcwd())
+    os.chdir(Path(__file__).parent)
+
+    script = "add_charges.py"
+
     command = (f"chimera --nogui --nostatus --script '{script} "
                f"-i \"{input_file}\" -o \"{output_file}\" "
                f"-nc {total_charge} -c {charge_method}'")
 
     p = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
     try:
         stdout, stderr = p.communicate()
     except Exception:
         p.kill()
         raise
 
-    if exists(output_file):
+    if os.path.exists(output_file):
         logger.debug("File '%s' created with success." % output_file)
     else:
         logger.error(stderr.decode())
         raise ProcessingFailed("Chimera could not add charges "
                                "to the provided molecule.")
+
+    os.chdir(cur_path)
```

### Comparing `luna-0.13.0/luna/wrappers/chimera/add_charges.py` & `luna-0.13.1/luna/wrappers/chimera/add_charges.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/cif.py` & `luna-0.13.1/luna/wrappers/cif.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/obabel.py` & `luna-0.13.1/luna/wrappers/obabel.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/pymol.py` & `luna-0.13.1/luna/wrappers/pymol.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna/wrappers/rdkit.py` & `luna-0.13.1/luna/wrappers/rdkit.py`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/luna.egg-info/PKG-INFO` & `luna-0.13.1/luna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: luna
-Version: 0.13.0
+Version: 0.13.1
 Summary: LUNA: drug discovery toolkit
 Home-page: https://github.com/keiserlab/LUNA
-Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.0
+Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.1
 Author: Alexandre Fassio
 Author-email: afassio@keiserlab.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/keiserlab/LUNA/issues
 Project-URL: Source, https://github.com/keiserlab/LUNA/
 Keywords: luna eifp fifp hifp ifp interaction fingerprint protein-ligand molecule docking
 Platform: UNKNOWN
```

### Comparing `luna-0.13.0/luna.egg-info/SOURCES.txt` & `luna-0.13.1/luna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luna-0.13.0/setup.py` & `luna-0.13.1/setup.py`

 * *Files identical despite different names*

