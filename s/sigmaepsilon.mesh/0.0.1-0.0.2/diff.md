# Comparing `tmp/sigmaepsilon.mesh-0.0.1.tar.gz` & `tmp/sigmaepsilon.mesh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon.mesh-0.0.1.tar", last modified: Wed Jul 12 17:23:53 2023, max compression
+gzip compressed data, was "sigmaepsilon.mesh-0.0.2.tar", last modified: Wed Jul 12 18:56:36 2023, max compression
```

## Comparing `sigmaepsilon.mesh-0.0.1.tar` & `sigmaepsilon.mesh-0.0.2.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.095466 sigmaepsilon.mesh-0.0.1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.059464 sigmaepsilon.mesh-0.0.1/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8523 2023-07-12 17:23:53.095466 sigmaepsilon.mesh-0.0.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6221 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.059464 sigmaepsilon.mesh-0.0.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.059464 sigmaepsilon.mesh-0.0.1/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/README_link.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.063464 sigmaepsilon.mesh-0.0.1/docs/source/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/logo.PNG
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot4a.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot5.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot6.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/plot7.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_5.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.063464 sigmaepsilon.mesh-0.0.1/docs/source/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_cells.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_db.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_recipes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_space.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_topo.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api/api_utils.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6371 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/doc_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.071465 sigmaepsilon.mesh-0.0.1/docs/source/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/compound1.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/compound2.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/compound3.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/cylinder.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/disc.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/grids2d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/grids3d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/import_file.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/import_gmsh.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/import_pyvista.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/joint_cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/lighting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples/trigridQ4.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/examples_gallery.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/logo.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.075465 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/data.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/grids.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/io.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_analysis.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_composition.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_structure.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/plotting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/points_and_pointclouds.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/shape_function_generation.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/trafo_geom.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/notebooks/trafo_topo.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/references.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/refs.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/docs/source/user_guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/logo.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/requirements-dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/requirements-devops.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/requirements-test.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 17:23:53.095466 sigmaepsilon.mesh-0.0.1/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.055464 sigmaepsilon.mesh-0.0.1/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.055464 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.083465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/abcdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/akwrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36505 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/celldata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.083465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4034 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2082 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2089 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1401 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/extrude.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/grid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.083465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/inp2stl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/line.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/linedata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/mesh1d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    83946 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polydata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polygon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polyhedron.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/pop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13756 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14606 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.087465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/frame.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tetmesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tetrahedralize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/topoarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/triang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/trimesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.087465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.091465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/gauss.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1622 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4612 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2630 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1372 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/knn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/locate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/space.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topodata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.091465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28958 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/voxelize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/vtkcelltypes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/vtkutils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.075465 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8523 2023-07-12 17:23:52.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5400 2023-07-12 17:23:53.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 17:23:52.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2023-07-12 17:23:52.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-12 17:23:52.000000 sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:53.095466 sigmaepsilon.mesh-0.0.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2063 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_compound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_geom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1044 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_hex.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_mesh_anal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_meshing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1548 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_topo_tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2384 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tests/test_tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-12 17:23:12.000000 sigmaepsilon.mesh-0.0.1/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8593 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6291 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/README_link.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.885482 sigmaepsilon.mesh-0.0.2/docs/source/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/logo.PNG
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4a.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot5.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot6.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot7.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_5.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.885482 sigmaepsilon.mesh-0.0.2/docs/source/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_cells.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_db.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_recipes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_space.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_topo.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_utils.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/doc_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.893482 sigmaepsilon.mesh-0.0.2/docs/source/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound1.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound2.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound3.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/cylinder.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/disc.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/grids2d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/grids3d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_file.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_gmsh.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_pyvista.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/joint_cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/lighting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/trigridQ4.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples_gallery.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/logo.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.897482 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/data.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/grids.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_analysis.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_composition.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_structure.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/plotting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/points_and_pointclouds.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/shape_function_generation.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_geom.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_topo.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/references.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/refs.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/user_guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/logo.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-devops.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-test.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.877482 sigmaepsilon.mesh-0.0.2/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.877482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/abcdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/akwrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36505 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/celldata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4034 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2082 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2089 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1401 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/downloads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/extrude.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/grid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/inp2stl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/line.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/linedata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/mesh1d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pointdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    83946 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polydata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polygon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polyhedron.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13756 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14606 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/section.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/frame.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetmesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetrahedralize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/topoarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/triang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/trimesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/gauss.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1622 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4612 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2630 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1372 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/knn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/locate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/space.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topodata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28958 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/voxelize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkcelltypes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkutils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.897482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8593 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5400 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2063 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_cells.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_compound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_geom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1044 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_hex.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_mesh_anal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_meshing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1548 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_topo_tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2384 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tox.ini
```

### Comparing `sigmaepsilon.mesh-0.0.1/.circleci/config.yml` & `sigmaepsilon.mesh-0.0.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/.gitignore` & `sigmaepsilon.mesh-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/.readthedocs.yaml` & `sigmaepsilon.mesh-0.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/LICENSE` & `sigmaepsilon.mesh-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/PKG-INFO` & `sigmaepsilon.mesh-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -44,16 +44,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # **SigmaEpsilon.Mesh** - A Python Library for Polygonal Meshes
 
 ![ ](logo.png)
 
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh.svg?style=shield)](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon.mesh/badge/?version=latest)](https://sigmaepsilon.mesh.readthedocs.io/en/latest/?badge=latest)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 > **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
```

### Comparing `sigmaepsilon.mesh-0.0.1/README.md` & `sigmaepsilon.mesh-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # **SigmaEpsilon.Mesh** - A Python Library for Polygonal Meshes
 
 ![ ](logo.png)
 
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh.svg?style=shield)](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon.mesh/badge/?version=latest)](https://sigmaepsilon.mesh.readthedocs.io/en/latest/?badge=latest)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 > **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
```

### Comparing `sigmaepsilon.mesh-0.0.1/docs/Makefile` & `sigmaepsilon.mesh-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/make.bat` & `sigmaepsilon.mesh-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/logo.PNG` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/logo.PNG`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot1.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot2.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot3.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot4.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot4a.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4a.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot5.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot6.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot6.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/plot7.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot7.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_1.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_2.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_3.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_4.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/_static/readme_5.png` & `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/api/api_cells.rst` & `sigmaepsilon.mesh-0.0.2/docs/source/api/api_cells.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/api/api_db.rst` & `sigmaepsilon.mesh-0.0.2/docs/source/api/api_db.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/conf.py` & `sigmaepsilon.mesh-0.0.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 generate_examples_gallery_rst(
     title="Examples", filename="examples_gallery", foldername="examples", reversed=True
 )
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = library.__project_name__
+project = library.__pkg_name__
 copyright = "2014-%s, Bence Balogh" % date.today().year
 author = "Bence Balogh"
 
 
 def setup(app: Config):
     app.add_config_value("project_name", project, "html")
```

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/doc_utils.py` & `sigmaepsilon.mesh-0.0.2/docs/source/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/compound1.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound1.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/compound2.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound2.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/compound3.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound3.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/cube.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/cylinder.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/cylinder.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/disc.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/disc.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/grids2d.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/grids2d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/grids3d.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/grids3d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/import_file.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_file.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/import_gmsh.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_gmsh.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/import_pyvista.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_pyvista.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/joint_cube.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/joint_cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/lighting.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/lighting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/examples/trigridQ4.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/examples/trigridQ4.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/logo.png` & `sigmaepsilon.mesh-0.0.2/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/data.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/data.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/grids.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/grids.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/io.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_analysis.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_composition.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_composition.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/mesh_structure.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_structure.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/plotting.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/points_and_pointclouds.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/points_and_pointclouds.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/shape_function_generation.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/shape_function_generation.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/trafo_geom.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_geom.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/notebooks/trafo_topo.ipynb` & `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_topo.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/docs/source/references.bib` & `sigmaepsilon.mesh-0.0.2/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/logo.png` & `sigmaepsilon.mesh-0.0.2/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/pyproject.toml` & `sigmaepsilon.mesh-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel>=0.38.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigmaepsilon.mesh"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Python package to build, manipulate and analyze polygonal meshes."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/__init__.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .topoarray import TopologyArray
 from .trimesh import TriMesh
 from .tetmesh import TetMesh
 from .triang import triangulate
 from .grid import grid, Grid
 from .tetrahedralize import tetrahedralize
 from .config import load_pyproject_config
+import importlib.metadata
 
 __all__ = [
     "PointCloud",
     "CartesianFrame",
     "PolyData",
     "LineData",
     "PolyData1d",
@@ -28,10 +29,10 @@
     "grid",
     "Grid",
     "tetrahedralize",
 ]
 
 # _config = load_pyproject_config()
 
-__version__ = "0.0.1"
-__description__ = "A Python package to build, manipulate and analyze polygonal meshes."
 __pkg_name__ = "sigmaepsilon.mesh"  # for Sphinx
+__version__ = importlib.metadata.version(__pkg_name__)
+__description__ = "A Python package to build, manipulate and analyze polygonal meshes."
```

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/abcdata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/abcdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/akwrap.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/akwrap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/base.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/base.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cell.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cell.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/celldata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/celldata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/__init__.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/h27.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h27.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/h8.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h8.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/l2.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/l3.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/q4.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/q9.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q9.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/t3.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/t6.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/tet10.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet10.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/tet4.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/w18.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w18.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/cells/w6.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/config.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/config.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/downloads.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/extrude.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/extrude.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/grid.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/grid.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/inp2stl.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/inp2stl.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/io/io.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/line.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/line.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/linedata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/linedata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/mesh1d.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/mesh1d.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/pointdata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pointdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polydata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polydata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polygon.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polygon.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/polyhedron.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polyhedron.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/pop.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pop.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/recipes.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/recipes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/section.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/section.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/frame.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/frame.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/point.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/point.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/space/pointcloud.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tetmesh.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetmesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tetrahedralize.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetrahedralize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/tile.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tile.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/topoarray.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/topoarray.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/triang.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/triang.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/trimesh.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/trimesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/gauss.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/gauss.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/h27.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h27.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/h8.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h8.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/l2.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/q4.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/q9.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q9.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/t3.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/t6.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/tet10.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet10.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/tet4.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/utils.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/w18.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w18.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/cells/w6.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/colors.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/colors.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/knn.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/knn.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/locate.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/locate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/space.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/space.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/tet.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tet.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topodata.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topodata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/topo.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/topo.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/topology/tr.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/tri.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tri.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/utils/utils.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/voxelize.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/voxelize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/vtkcelltypes.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkcelltypes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon/mesh/vtkutils.py` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkutils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/PKG-INFO` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -44,16 +44,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # **SigmaEpsilon.Mesh** - A Python Library for Polygonal Meshes
 
 ![ ](logo.png)
 
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh.svg?style=shield)](https://circleci.com/gh/dewloosh/sigmaepsilon.mesh)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon.mesh/badge/?version=latest)](https://sigmaepsilon.mesh.readthedocs.io/en/latest/?badge=latest)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 > **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
```

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/SOURCES.txt` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/src/sigmaepsilon.mesh.egg-info/requires.txt` & `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_cells.py` & `sigmaepsilon.mesh-0.0.2/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_compound.py` & `sigmaepsilon.mesh-0.0.2/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_geom.py` & `sigmaepsilon.mesh-0.0.2/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_hex.py` & `sigmaepsilon.mesh-0.0.2/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_io.py` & `sigmaepsilon.mesh-0.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_linalg.py` & `sigmaepsilon.mesh-0.0.2/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_mesh_anal.py` & `sigmaepsilon.mesh-0.0.2/tests/test_mesh_anal.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_meshing.py` & `sigmaepsilon.mesh-0.0.2/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_pointcloud.py` & `sigmaepsilon.mesh-0.0.2/tests/test_pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_recipes.py` & `sigmaepsilon.mesh-0.0.2/tests/test_recipes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_tet.py` & `sigmaepsilon.mesh-0.0.2/tests/test_tet.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_topo_tr.py` & `sigmaepsilon.mesh-0.0.2/tests/test_topo_tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.1/tests/test_tri.py` & `sigmaepsilon.mesh-0.0.2/tests/test_tri.py`

 * *Files identical despite different names*

