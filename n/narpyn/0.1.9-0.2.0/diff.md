# Comparing `tmp/narpyn-0.1.9.tar.gz` & `tmp/narpyn-0.2.0.tar.gz`

## Comparing `narpyn-0.1.9.tar` & `narpyn-0.2.0.tar`

### file list

```diff
@@ -1,168 +1,17 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 narpyn-0.1.9/.gitattributes
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 narpyn-0.1.9/.gitmodules
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 narpyn-0.1.9/build_ona.sh
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 narpyn-0.1.9/build_package.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.9/narpyn/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.9/narpyn/ona/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 narpyn-0.1.9/narpyn/ona/nar.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 narpyn-0.1.9/narpyn/ona/narsese.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 narpyn-0.1.9/narpyn/ona/NAR/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/.git
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/.gitignore
--rwxr-xr-x   0        0        0     3350 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/Dockerfile
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/LICENSE
--rwxr-xr-x   0        0        0     8257 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/README.md
--rwxr-xr-x   0        0        0      755 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/build.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/docker-compose.yml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/install_python_dependencies.sh
--rwxr-xr-x   0        0        0     1701 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/libbuild.sh
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/babi1.english
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/dialog.english
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/disambiguate.english
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/grammar.english
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/prepositions.english
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/robotQA.english
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/story1.english
--rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/story2.english
--rwxr-xr-x   0        0        0      371 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/story3.english
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/english/story4.english
--rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/activequestion.nal
--rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/asthma.nal
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/asthma2.nal
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/avoid.nal
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/avoid2.nal
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/avoid3.nal
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/catCAT.nal
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/categoryformationanddetection.nal
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/circus.nal
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave0.nal
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave1.nal
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave2.nal
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave3.nal
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave4.nal
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/clapwave5.nal
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/diagnostic.nal
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/door.nal
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/door2.nal
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/door3.nal
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/duck.nal
--rwxr-xr-x   0        0        0    14725 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/example1.nal
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/example2.nal
--rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/example3.nal
--rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/example4.nal
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/greenplant.nal
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/latch.nal
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/map.nal
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/map2.nal
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/marshmallow.nal
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/numbers.nal
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/pickbrighter.nal
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/plandeep.nal
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/prefergeneral.nal
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/prefernext.nal
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/preferspecific.nal
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/propertymatching.nal
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/relationalnetwork.nal
--rwxr-xr-x   0        0        0     3820 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/school.nal
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/self.nal
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/self2.nal
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/self3.nal
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/similarities.nal
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/spatial.nal
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/spatial3.nal
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/spatial4.nal
--rwxr-xr-x   0        0        0     1371 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/symmetry.nal
--rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/toothbrush.nal
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/examples/nal/whatwarmer.nal
--rwxr-xr-x   0        0        0     2403 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Concept.h
--rwxr-xr-x   0        0        0     7741 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Config.h
--rwxr-xr-x   0        0        0    35264 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Cycle.c
--rwxr-xr-x   0        0        0     1799 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Cycle.h
--rwxr-xr-x   0        0        0    26640 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Decision.c
--rwxr-xr-x   0        0        0     3336 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Decision.h
--rwxr-xr-x   0        0        0     2753 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Event.c
--rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Event.h
--rwxr-xr-x   0        0        0     2150 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Globals.c
--rwxr-xr-x   0        0        0     2673 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Globals.h
--rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/HashTable.c
--rwxr-xr-x   0        0        0     2640 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/HashTable.h
--rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Implication.h
--rwxr-xr-x   0        0        0     9629 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Inference.c
--rwxr-xr-x   0        0        0     2972 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Inference.h
--rwxr-xr-x   0        0        0     5349 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/InvertedAtomIndex.c
--rwxr-xr-x   0        0        0     2334 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/InvertedAtomIndex.h
--rwxr-xr-x   0        0        0    18958 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Memory.c
--rwxr-xr-x   0        0        0     4219 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Memory.h
--rwxr-xr-x   0        0        0    20399 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NAL.c
--rwxr-xr-x   0        0        0    14959 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NAL.h
--rwxr-xr-x   0        0        0    11792 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NAR.c
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NAR.h
--rwxr-xr-x   0        0        0    28145 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Narsese.c
--rwxr-xr-x   0        0        0     4422 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Narsese.h
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/OccurrenceTimeIndex.c
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/OccurrenceTimeIndex.h
--rwxr-xr-x   0        0        0     6777 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/PriorityQueue.c
--rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/PriorityQueue.h
--rwxr-xr-x   0        0        0     1922 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/RuleTable.h
--rwxr-xr-x   0        0        0    14924 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Shell.c
--rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Shell.h
--rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stack.c
--rwxr-xr-x   0        0        0     1814 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stack.h
--rwxr-xr-x   0        0        0     3850 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stamp.c
--rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stamp.h
--rwxr-xr-x   0        0        0     3835 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stats.c
--rwxr-xr-x   0        0        0     1668 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Stats.h
--rwxr-xr-x   0        0        0     4506 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Table.c
--rwxr-xr-x   0        0        0     2530 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Table.h
--rwxr-xr-x   0        0        0     3651 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Term.c
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Term.h
--rwxr-xr-x   0        0        0     7595 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Truth.c
--rwxr-xr-x   0        0        0     3383 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Truth.h
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Usage.c
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Usage.h
--rwxr-xr-x   0        0        0    18602 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Variable.c
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/Variable.h
--rwxr-xr-x   0        0        0     5197 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/main.c
--rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/Metric.c
--rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/Metric.h
--rwxr-xr-x   0        0        0     2300 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/UDP.c
--rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/UDP.h
--rwxr-xr-x   0        0        0     3997 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/UDPNAR.c
--rwxr-xr-x   0        0        0     1667 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/NetworkNAR/UDPNAR.h
--rwxr-xr-x   0        0        0     4565 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Alien_Test.h
--rwxr-xr-x   0        0        0     1645 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Alphabet_Test.h
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Bandrobot_Test.h
--rwxr-xr-x   0        0        0     2938 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Cartpole_Test.h
--rwxr-xr-x   0        0        0     3458 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Follow_Test.h
--rwxr-xr-x   0        0        0     2767 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Multistep2_Test.h
--rwxr-xr-x   0        0        0     3034 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Multistep_Test.h
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Pong2_Test.h
--rwxr-xr-x   0        0        0     4272 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Pong_Test.h
--rwxr-xr-x   0        0        0     2084 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Procedure_Test.h
--rwxr-xr-x   0        0        0    16593 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Robot_Test.h
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Sequence_Test.h
--rwxr-xr-x   0        0        0    17000 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/Testchamber_Test.h
--rwxr-xr-x   0        0        0     2193 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/UDPNAR_Test.h
--rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/system_tests/system_tests.h
--rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/HashTable_Test.h
--rwxr-xr-x   0        0        0     4433 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/InvertedAtomIndex_Test.h
--rwxr-xr-x   0        0        0     2080 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/Memory_Test.h
--rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/Narsese_Test.h
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/OccurrenceTimeIndex_Test.h
--rwxr-xr-x   0        0        0     2280 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/PriorityQueue_Test.h
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/RuleTable_Test.h
--rwxr-xr-x   0        0        0     2426 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/Stack_Test.h
--rwxr-xr-x   0        0        0     1571 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/Stamp_Test.h
--rwxr-xr-x   0        0        0     2464 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/Table_Test.h
--rwxr-xr-x   0        0        0     2161 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/UDP_Test.h
--rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 narpyn-0.1.9/ona/src/unit_tests/unit_tests.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.9/tests/ona/__init__.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 narpyn-0.1.9/tests/ona/test_nar.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 narpyn-0.1.9/tests/ona/test_narsese.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 narpyn-0.1.9/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 narpyn-0.1.9/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 narpyn-0.1.9/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 narpyn-0.1.9/hatch.toml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 narpyn-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 narpyn-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 narpyn-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 narpyn-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    44803 2020-02-02 00:00:00.000000 narpyn-0.2.0/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.2.0/narpyn/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.2.0/narpyn/ona/__init__.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 narpyn-0.2.0/narpyn/ona/nar.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 narpyn-0.2.0/narpyn/ona/narsese.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 narpyn-0.2.0/narpyn/ona/NAR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.2.0/tests/ona/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 narpyn-0.2.0/tests/ona/test_nar.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 narpyn-0.2.0/tests/ona/test_narsese.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 narpyn-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 narpyn-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 narpyn-0.2.0/README.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 narpyn-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 narpyn-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 narpyn-0.2.0/PKG-INFO
```

### Comparing `narpyn-0.1.9/narpyn/ona/nar.py` & `narpyn-0.2.0/narpyn/ona/nar.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 from narpyn.ona.narsese import *
 
 logger = logging.getLogger(__name__)
 
 
 def send_input(process: subprocess.Popen, input_: str) -> None:
-    """Send input to NARS server"""
+    """Send input to ONA"""
     stdin, stdout = process.stdin, process.stdout
     if stdin is None or stdout is None:
         raise RuntimeError("Process has no stdin or stdout.")
 
     stdin.write(input_ + "\n")
     stdin.flush()
 
 
 def get_raw_output(process: subprocess.Popen) -> list[str]:
-    """Get raw output from NARS server"""
+    """Get raw output from ONA"""
     stdin, stdout = process.stdin, process.stdout
     if stdin is None or stdout is None:
         raise RuntimeError("Process has no stdin or stdout.")
 
     stdin.write("0\n")
     stdin.flush()
     ret: str = ""
@@ -31,14 +31,15 @@
             before.append(ret.strip())
         ret = stdout.readline()
     logger.debug("\n".join(before))
     return before
 
 
 def get_output(process: subprocess.Popen) -> dict[str, Any]:
+    """Get last output from ONA and parse it"""
     lines = get_raw_output(process)
     executions = [parse_execution(l) for l in lines if l.startswith("^")]
     inputs = [
         parse_task(l.split("Input: ")[1]) for l in lines if l.startswith("Input:")
     ]
     derivations = [
         parse_task(l.split("Derived: " if l.startswith("Derived:") else "Revised: ")[1])
```

### Comparing `narpyn-0.1.9/narpyn/ona/narsese.py` & `narpyn-0.2.0/narpyn/ona/narsese.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, Callable, Optional
 
 
-def narsify(observation):
+def gym_narsify(observation):
     """Convert a Gym observation to NARS input"""
-    return ",".join(str(x) for x in observation)
+    return "_".join(str(x) for x in observation)
 
 
 def loc(pos: tuple[int, int]) -> str:
     """Turn coordinates into a location string"""
     return f"loc_x{pos[0]}_y{pos[1]}"
 
 
@@ -32,28 +32,30 @@
 
 def nal_now(s: str) -> str:
     """Return NAL statement in the present"""
     return f"{s}. :|:"
 
 
 def parse_truth_value(tv_str: str) -> dict[str, float]:
+    """Parse a Truth Value into a dictionary"""
     splits = tv_str.split(" ")
     freq_s, conf_s = splits[0], splits[1]
     if freq_s[-1] == ",":
         freq_s = freq_s[:-1]
 
     frequency = float(freq_s.split("=")[1])
     confidence = float(conf_s.split("=")[1])
     return {
         "frequency": frequency,
         "confidence": confidence,
     }
 
 
 def parse_task(s: str) -> dict[str, Any]:
+    """Parse information about a task seen by the system"""
     m: dict[str, Any] = {"occurrenceTime": "eternal"}
     if " :|:" in s:
         m["occurrenceTime"] = "now"
         s = s.replace(" :|:", "")
         if "occurrenceTime" in s:
             m["occurrenceTime"] = s.split("occurrenceTime=")[1].split(" ")[0]
     sentence = (
@@ -69,14 +71,15 @@
     )
     if "Truth" in s:
         m["truth"] = parse_truth_value(s.split("Truth: ")[1])
     return m
 
 
 def parse_reason(sraw: str) -> Optional[dict[str, str]]:
+    """Parse ONA's justification for an action taken"""
     if "implication: " not in sraw:
         return None
     implication = parse_task(
         sraw.split("implication: ")[-1].split("precondition: ")[0]
     )  # last reason only (others couldn't be associated currently)
     precondition = parse_task(sraw.split("precondition: ")[-1].split("\n")[0])
     implication["occurrenceTime"] = "eternal"
@@ -85,27 +88,28 @@
     reason["desire"] = sraw.split("decision expectation=")[-1].split(" ")[0]
     reason["hypothesis"] = implication
     reason["precondition"] = precondition
     return reason
 
 
 def parse_execution(e: str) -> dict[str, Any]:
+    """Parse information about an operator executed"""
     op = e.split(" ")[0]
     argstr = e.split("args ")[1] if "args " in e else None
     if argstr is None:
         return {"operator": op, "arguments": []}
     return {
         "operator": op,
         "arguments": argstr[1:-1].split(" * ") if "*" in argstr else [argstr],
     }
 
 
 @dataclass
 class Goal:
-    """A goal"""
+    """A simple goal representation"""
 
     symbol: str
     satisfied: Callable
     knowledge: Optional[list[str]] = None
 
     def __repr__(self) -> str:
         return f"Goal {self.symbol}; {self.knowledge}"
```

### Comparing `narpyn-0.1.9/tests/ona/test_nar.py` & `narpyn-0.2.0/tests/ona/test_nar.py`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.9/tests/ona/test_narsese.py` & `narpyn-0.2.0/tests/ona/test_narsese.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from narpyn.ona.narsese import (
     Goal,
     ext,
+    gym_narsify,
     loc,
     nal_demand,
     nal_now,
-    narsify,
     parse_execution,
     parse_reason,
     parse_task,
     parse_truth_value,
     pos,
 )
 
 
 # Test narsify function
 def test_narsify():
-    assert narsify([1, 2, 3]) == "1,2,3"
-    assert narsify(["a", "b", "c"]) == "a,b,c"
-    assert narsify([]) == ""
+    assert gym_narsify([1, 2, 3]) == "1_2_3"
+    assert gym_narsify(["a", "b", "c"]) == "a_b_c"
+    assert gym_narsify([]) == ""
 
 
 # Test loc function
 def test_loc():
     assert loc((0, 0)) == "loc_x0_y0"
     assert loc((1, 2)) == "loc_x1_y2"
     assert loc((-1, -2)) == "loc_x-1_y-2"
```

### Comparing `narpyn-0.1.9/.gitignore` & `narpyn-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.9/LICENSE` & `narpyn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.9/hatch.toml` & `narpyn-0.2.0/hatch.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "coverage-badge",
 ]
 
 [envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report --show-missing",
+  "coverage json",
 ]
+cov-badge = "coverage-badge -fo coverage/coverage.svg"
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [envs.all]
 type = "container"
```

### Comparing `narpyn-0.1.9/pyproject.toml` & `narpyn-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.270"
 pytest = "^7.3.1"
 ipython = "^8.14.0"
+pre-commit = "^3.3.3"
 
 [project]
 name = "narpyn"
 dynamic = ["version"]
 description = "A Python API library for NARS"
 keywords = [
   "nars",
@@ -32,56 +33,48 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+  "ona>=0.9.2",
+]
 
-[project.scripts]
-NAR = "narpyn.ona.NAR:NAR"
+[project.urls]
+Homepage = "https://ntoxeg.github.io/narpyn/"
+Sponsor = "https://github.com/sponsors/ntoxeg"
+Tracker = "https://github.com/ntoxeg/narpyn/issues"
+Source = "https://github.com/ntoxeg/narpyn"
 
 [build-system]
-requires = ["hatchling>=1.17.0", "hatch-vcs"]
+requires = ["hatchling>=1.17.0", "hatch-vcs", "hatch-build-scripts"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
 
-[tool.hatch.build]
-artifacts = [
-    "*.so",
-    "*.dll",
-    "/narpyn/ona/NAR/NARexe",
-]
-
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
-  "/ona/misc",
-  "/ona/*.py",
 ]
 
 [tool.hatch.build.targets.wheel]
-pure_python = false
 exclude = [
-  "/ona",
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel.hooks.mypyc]
 enable-by-default = false
 dependencies = ["hatch-mypyc>=0.14.1"]
 require-runtime-dependencies = true
 mypy-args = [
   "--no-warn-unused-ignores",
 ]
-exclude = [
-  "/narpyn/ona/NAR"
-]
 
 [tool.ruff.isort]
 known-first-party = ["narpyn"]
 
 [terminal.styles]
 spinner = "dots"
 
@@ -97,9 +90,9 @@
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
-[tool.cibuildwheel]
-before-build = "./build_ona.sh"
+[tool.isort]
+profile = "black"
```

