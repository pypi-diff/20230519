# Comparing `tmp/rdkit-stubs-0.3.tar.gz` & `tmp/rdkit-stubs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdkit-stubs-0.3.tar", last modified: Tue May  9 23:15:08 2023, max compression
+gzip compressed data, was "rdkit-stubs-0.4.tar", last modified: Fri May 19 16:46:36 2023, max compression
```

## Comparing `rdkit-stubs-0.3.tar` & `rdkit-stubs-0.4.tar`

### file list

```diff
@@ -1,417 +1,417 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/
--rw-rw-r--   0 a         (1000) a         (1000)    11336 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/LICENSE-APACHE
--rw-rw-r--   0 a         (1000) a         (1000)     1047 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/LICENSE-MIT
--rw-rw-r--   0 a         (1000) a         (1000)     1662 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)     1256 2022-11-09 23:57:03.000000 rdkit-stubs-0.3/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.308090 rdkit-stubs-0.3/rdkit-stubs/
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.308090 rdkit-stubs-0.3/rdkit-stubs/Avalon/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Avalon/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1563 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Avalon/pyAvalonTools.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.316090 rdkit-stubs-0.3/rdkit-stubs/Chem/
--rw-rw-r--   0 a         (1000) a         (1000)     4488 2022-11-10 00:07:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AllChem.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/
--rw-rw-r--   0 a         (1000) a         (1000)      766 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Pairs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      698 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Sheridan.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      664 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Torsions.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      483 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Utils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1282 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/BRICS.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2245 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/BuildFragmentCatalog.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/
--rw-rw-r--   0 a         (1000) a         (1000)      327 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/AlignDepict.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      241 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/BulkTester.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      441 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/DescriptorUtilities.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      319 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/SDFToCSV.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      923 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/TemplateExpand.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      178 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemicalFeatures.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       76 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ChemicalForceFields.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      822 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Crippen.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1940 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/DSViewer.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1387 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Descriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      317 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Descriptors3D.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/
--rw-rw-r--   0 a         (1000) a         (1000)     2060 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/IPythonConsole.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1178 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/InteractiveRenderer.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3215 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/MolDrawing.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1797 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/SimilarityMaps.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     5666 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1102 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/aggCanvas.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1588 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/cairoCanvas.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      536 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/canvasbase.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      743 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/mplCanvas.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      736 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/qtCanvas.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     7785 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/rdMolDraw2D.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      859 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/spingCanvas.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/
--rw-rw-r--   0 a         (1000) a         (1000)      190 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/AtomTypes.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      347 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/EState.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      393 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/EState_VSA.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      147 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/Fingerprinter.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       81 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EState/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      429 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EnumerateHeterocycles.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1587 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/EnumerateStereoisomers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       81 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FastSDMolSupplier.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      371 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatFinderCLI.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/
--rw-rw-r--   0 a         (1000) a         (1000)      609 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMapParser.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      453 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMapPoint.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      887 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMapUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1485 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMaps.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.320090 rdkit-stubs-0.3/rdkit-stubs/Chem/Features/
--rw-rw-r--   0 a         (1000) a         (1000)      823 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Features/FeatDirUtilsRD.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1332 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Features/ShowFeats.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Features/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      295 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FilterCatalog.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/
--rw-rw-r--   0 a         (1000) a         (1000)      546 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/ClusterMols.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1022 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/DbFpSupplier.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1983 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/FingerprintMols.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      756 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/MolSimilarity.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1290 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/SimilarityScreener.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/Fraggle/
--rw-rw-r--   0 a         (1000) a         (1000)      867 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fraggle/FraggleSim.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fraggle/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      492 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FragmentCatalog.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      511 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FragmentMatcher.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      269 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Fragments.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      867 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/FunctionalGroups.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1745 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/GraphDescriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      162 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Graphs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      660 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Lipinski.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      356 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MACCSkeys.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      548 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MCS.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       38 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolCatalog.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/
--rw-rw-r--   0 a         (1000) a         (1000)      915 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/FingerprintUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1206 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/Loader_orig.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1222 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/Loader_sa.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/
--rw-rw-r--   0 a         (1000) a         (1000)      655 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/InchiInfo.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2096 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/MolKey.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/
--rw-rw-r--   0 a         (1000) a         (1000)      742 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1219 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/charge.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      154 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/errors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      891 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/fragment.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      265 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/metal.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      748 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/normalize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     9763 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/rdMolStandardize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      740 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/resonance.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2389 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/standardize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1453 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/tautomer.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       61 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/utils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      853 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/validate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1244 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/validations.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      959 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/MolSurf.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2918 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/PandasTools.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.324090 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/
--rw-rw-r--   0 a         (1000) a         (1000)      399 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/Generate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      221 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/Gobbi_Pharm2D.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      465 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/LazyGenerator.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      364 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/Matcher.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1638 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/SigFactory.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1051 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/Utils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      177 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/
--rw-rw-r--   0 a         (1000) a         (1000)     2830 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/EmbedLib.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      259 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/ExcludedVolume.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1626 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/Pharmacophore.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      236 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/PropertyMol.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2221 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/PyMol.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1149 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/QED.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      154 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Randomize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      633 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Recap.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       82 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ReducedGraphs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      292 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/SATIS.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1200 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/SaltRemover.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/
--rw-rw-r--   0 a         (1000) a         (1000)      595 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/MurckoScaffold.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2487 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/rdScaffoldNetwork.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/ShowMols.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/SimpleEnum/
--rw-rw-r--   0 a         (1000) a         (1000)      483 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/SimpleEnum/Enumerator.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/SimpleEnum/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/
--rw-rw-r--   0 a         (1000) a         (1000)     1102 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/BuilderUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2753 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeAligner.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1006 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeBuilder.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      938 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeObjects.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      513 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/testCombined.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/Suppliers/
--rw-rw-r--   0 a         (1000) a         (1000)     1075 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Suppliers/DbMolSupplier.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      234 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Suppliers/MolSupplier.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/Suppliers/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      303 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/TemplateAlign.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1649 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/TorsionFingerprints.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     4355 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/Chem/fmcs/
--rw-rw-r--   0 a         (1000) a         (1000)       35 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/fmcs/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     9857 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/fmcs/fmcs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      912 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/inchi.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1369 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdAbbreviations.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       63 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdCIPLabeler.pyi
--rw-rw-r--   0 a         (1000) a         (1000)    12742 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdChemReactions.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      905 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdChemicalFeatures.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      883 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdCoordGen.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      386 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdDepictor.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1341 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdDeprotect.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1271 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdDistGeom.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      823 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdEHTTools.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     4345 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdFMCS.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3477 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdFingerprintGenerator.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      879 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdForceFieldHelpers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1337 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdFreeSASA.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1165 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMHFPFingerprint.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      150 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMMPA.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      910 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolAlign.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1779 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolCatalog.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1610 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolChemicalFeatures.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     8906 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolDescriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      652 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolEnumerator.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1022 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolHash.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      462 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolInterchange.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      877 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolTransforms.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       71 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdPartialCharges.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3544 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdRGroupDecomposition.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      181 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdReducedGraphs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      117 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdSLNParse.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      355 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdShapeHelpers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     4807 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdSubstructLibrary.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      850 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdTautomerQuery.pyi
--rw-rw-r--   0 a         (1000) a         (1000)    41181 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdchem.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     8330 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdfiltercatalog.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2533 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdfragcatalog.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      237 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdinchi.pyi
--rw-rw-r--   0 a         (1000) a         (1000)    13640 2023-05-09 23:02:35.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdmolfiles.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     9212 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdmolops.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     4367 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdqueries.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1219 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Chem/rdtrajectory.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/DataManip/
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/DataManip/Metric/
--rw-rw-r--   0 a         (1000) a         (1000)       91 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataManip/Metric/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      150 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataManip/Metric/rdMetricMatrixCalc.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       50 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataManip/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.328090 rdkit-stubs-0.3/rdkit-stubs/DataStructs/
--rw-rw-r--   0 a         (1000) a         (1000)      362 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/BitEnsemble.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      375 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/BitEnsembleDb.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      143 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/BitUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      712 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/HierarchyVis.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      316 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/LazySignature.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      442 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/TopNContainer.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      904 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/VectCollection.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      291 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)    16564 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/DataStructs/cDataStructs.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/Dbase/
--rw-rw-r--   0 a         (1000) a         (1000)     1753 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbConnection.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      900 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbInfo.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      416 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbModule.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1718 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbReport.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1294 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbResultSet.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1989 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/DbUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      765 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/StorageUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Dbase/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/DistanceGeometry/
--rw-rw-r--   0 a         (1000) a         (1000)      108 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DistanceGeometry/DistGeom.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       46 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/DistanceGeometry/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/ForceField/
--rw-rw-r--   0 a         (1000) a         (1000)       44 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ForceField/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3387 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/ForceField/rdForceField.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/Geometry/
--rw-rw-r--   0 a         (1000) a         (1000)       85 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Geometry/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     6816 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/Geometry/rdGeometry.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/ML/
--rw-rw-r--   0 a         (1000) a         (1000)      452 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/AnalyzeComposite.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1012 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/BuildComposite.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/
--rw-rw-r--   0 a         (1000) a         (1000)      237 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Butina.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      289 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/ClusterUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2525 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/ClusterVis.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      124 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Clustering.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1529 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Clusters.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      487 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Murtagh.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      256 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Resemblance.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      117 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Standardize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      152 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/murtagh_test.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.332090 rdkit-stubs-0.3/rdkit-stubs/ML/Composite/
--rw-rw-r--   0 a         (1000) a         (1000)      196 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Composite/AdjustComposite.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2719 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Composite/Composite.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Composite/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      502 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/CompositeRun.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.336090 rdkit-stubs-0.3/rdkit-stubs/ML/Data/
--rw-rw-r--   0 a         (1000) a         (1000)     1537 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/DataUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      199 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/FindQuantBounds.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1902 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/MLData.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      835 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/Quantize.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      583 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/SplitData.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      407 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/Stats.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      217 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/Transforms.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      124 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Data/cQuantize.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.336090 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/
--rw-rw-r--   0 a         (1000) a         (1000)      830 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/BuildQuantTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      751 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/BuildSigTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      717 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/CrossValidate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      907 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/DecTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1277 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/Forest.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      533 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/ID3.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      377 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/PruneTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      515 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/QuantTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      345 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/SigTree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1634 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/Tree.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      169 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/TreeUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      995 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/TreeVis.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      214 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/randomtest.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.336090 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/
--rw-rw-r--   0 a         (1000) a         (1000)     1657 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/CompoundDescriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      405 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/Descriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      701 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/MoleculeDescriptors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      757 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/Parser.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      704 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/EnrichPlot.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      965 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/GrowComposite.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.336090 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/
--rw-rw-r--   0 a         (1000) a         (1000)      471 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/BitClusterer.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      425 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/BitRank.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       47 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      226 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/entropy.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1553 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/rdInfoTheory.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/
--rw-rw-r--   0 a         (1000) a         (1000)      716 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/CrossValidate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      177 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/DistFunctions.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      525 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNClassificationModel.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      837 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNModel.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      581 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNRegressionModel.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/KNN/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/MLUtils/
--rw-rw-r--   0 a         (1000) a         (1000)      432 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/MLUtils/VoteImg.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/MLUtils/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      176 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/MatOps.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/ModelPackage/
--rw-rw-r--   0 a         (1000) a         (1000)      390 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/ModelPackage/PackageUtils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1048 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/ModelPackage/Packager.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/ModelPackage/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/
--rw-rw-r--   0 a         (1000) a         (1000)     1421 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/ClassificationModel.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      740 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/CrossValidate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       35 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/
--rw-rw-r--   0 a         (1000) a         (1000)      463 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/ActFuncs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      485 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/CrossValidate.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      620 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/NetNode.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1190 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/Network.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      507 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/Trainers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Neural/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/SLT/
--rw-rw-r--   0 a         (1000) a         (1000)      223 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/SLT/Risk.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/SLT/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/ML/Scoring/
--rw-rw-r--   0 a         (1000) a         (1000)      225 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Scoring/Scoring.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/Scoring/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2797 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/ScreenComposite.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      391 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/ML/files.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/Numerics/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Numerics/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       79 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/Numerics/rdAlignment.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      114 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/RDConfig.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      666 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/RDLogger.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      166 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/RDPaths.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       92 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/RDRandom.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/
--rw-rw-r--   0 a         (1000) a         (1000)     1338 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/SimilarityPickers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      152 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1829 2022-11-09 23:57:57.000000 rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/rdSimDivPickers.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1060 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/TestRunner.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.340090 rdkit-stubs-0.3/rdkit-stubs/VLib/
--rw-rw-r--   0 a         (1000) a         (1000)      426 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/Filter.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      775 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/Node.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/
--rw-rw-r--   0 a         (1000) a         (1000)      462 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/DbMolSupply.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1253 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/DbPickleSupplier.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      382 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SDSupply.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      406 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmartsMolFilter.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      499 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmartsRemover.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      352 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmilesDupeFilter.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      553 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmilesOutput.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      536 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmilesSupply.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      128 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      384 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/demo.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      369 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/Output.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      418 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/Supply.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      302 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/Transform.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       54 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/VLib/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      162 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     7877 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/rdBase.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/
--rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3375 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfdoc.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     6354 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfgen.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       75 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfgeom.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      432 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfmetrics.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      475 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfutils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     4210 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pidPDF.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/PIL/
--rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PIL/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1976 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PIL/pidPIL.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/PS/
--rw-rw-r--   0 a         (1000) a         (1000)       21 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PS/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       91 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PS/fontinfo.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       57 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PS/latin1MetricsCache.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     5577 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PS/pidPS.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      229 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/PS/psmetrics.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/Pyart/
--rw-rw-r--   0 a         (1000) a         (1000)        1 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/Pyart/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.344090 rdkit-stubs-0.3/rdkit-stubs/sping/Qt/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/Qt/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1904 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/Qt/pidQt.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1814 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/Qt/pidQt4.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/sping/ReportLab/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/ReportLab/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2160 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/ReportLab/pidReportLab.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/sping/SVG/
--rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/SVG/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     2818 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/SVG/pidSVG.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/sping/TK/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/TK/__init__.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/sping/WX/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/WX/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      104 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     3670 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/colors.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      422 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/pagesizes.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     5561 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/pid.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1889 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/stringformat.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/sping/util/
--rw-rw-r--   0 a         (1000) a         (1000)      612 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/util/HTMLPiddler.pyi
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/util/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)       64 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/sping/utils.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit-stubs/utils/
--rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/__init__.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      259 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/cactvs.pyi
--rw-rw-r--   0 a         (1000) a         (1000)     1212 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/chemdraw.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      449 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/chemdraw_qax.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      428 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/chemutils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      238 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/comhack.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      112 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/fileutils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      128 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/listutils.pyi
--rw-rw-r--   0 a         (1000) a         (1000)      350 2022-11-09 23:55:29.000000 rdkit-stubs-0.3/rdkit-stubs/utils/spiral.pyi
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/rdkit_stubs.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)     1662 2023-05-09 23:15:08.000000 rdkit-stubs-0.3/rdkit_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    12937 2023-05-09 23:15:08.000000 rdkit-stubs-0.3/rdkit_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-09 23:15:08.000000 rdkit-stubs-0.3/rdkit_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        6 2023-05-09 23:15:08.000000 rdkit-stubs-0.3/rdkit_stubs.egg-info/requires.txt
--rw-rw-r--   0 a         (1000) a         (1000)       12 2023-05-09 23:15:08.000000 rdkit-stubs-0.3/rdkit_stubs.egg-info/top_level.txt
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/setup.cfg
--rw-rw-r--   0 a         (1000) a         (1000)     1190 2023-05-09 22:46:28.000000 rdkit-stubs-0.3/setup.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-09 23:15:08.348090 rdkit-stubs-0.3/test/
--rw-rw-r--   0 a         (1000) a         (1000)     1009 2023-05-09 22:56:09.000000 rdkit-stubs-0.3/test/test_stubs.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.164295 rdkit-stubs-0.4/
+-rw-rw-r--   0 a         (1000) a         (1000)    11336 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/LICENSE-APACHE
+-rw-rw-r--   0 a         (1000) a         (1000)     1047 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/LICENSE-MIT
+-rw-rw-r--   0 a         (1000) a         (1000)     1698 2023-05-19 16:46:36.164295 rdkit-stubs-0.4/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)     1256 2022-11-09 23:57:03.000000 rdkit-stubs-0.4/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.084294 rdkit-stubs-0.4/rdkit-stubs/
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.084294 rdkit-stubs-0.4/rdkit-stubs/Avalon/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Avalon/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1563 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Avalon/pyAvalonTools.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.104294 rdkit-stubs-0.4/rdkit-stubs/Chem/
+-rw-rw-r--   0 a         (1000) a         (1000)     4488 2022-11-10 00:07:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AllChem.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.104294 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/
+-rw-rw-r--   0 a         (1000) a         (1000)      766 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Pairs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      698 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Sheridan.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      664 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Torsions.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      483 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Utils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1282 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/BRICS.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2245 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/BuildFragmentCatalog.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.104294 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/
+-rw-rw-r--   0 a         (1000) a         (1000)      327 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/AlignDepict.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      241 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/BulkTester.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      441 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/DescriptorUtilities.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      319 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/SDFToCSV.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      923 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/TemplateExpand.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      178 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemicalFeatures.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       76 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ChemicalForceFields.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      822 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Crippen.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1940 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/DSViewer.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1387 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Descriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      317 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Descriptors3D.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.108294 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/
+-rw-rw-r--   0 a         (1000) a         (1000)     2060 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/IPythonConsole.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1178 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/InteractiveRenderer.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3215 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/MolDrawing.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1797 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/SimilarityMaps.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     5666 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1102 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/aggCanvas.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1588 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/cairoCanvas.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      536 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/canvasbase.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      743 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/mplCanvas.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      736 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/qtCanvas.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     7785 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/rdMolDraw2D.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      859 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/spingCanvas.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.108294 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/
+-rw-rw-r--   0 a         (1000) a         (1000)      190 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/AtomTypes.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      347 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/EState.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      393 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/EState_VSA.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      147 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/Fingerprinter.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       81 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EState/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      429 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EnumerateHeterocycles.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1587 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/EnumerateStereoisomers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       81 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FastSDMolSupplier.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      371 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatFinderCLI.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.112294 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/
+-rw-rw-r--   0 a         (1000) a         (1000)      609 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMapParser.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      453 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMapPoint.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      887 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMapUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1485 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMaps.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.112294 rdkit-stubs-0.4/rdkit-stubs/Chem/Features/
+-rw-rw-r--   0 a         (1000) a         (1000)      823 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Features/FeatDirUtilsRD.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1332 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Features/ShowFeats.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Features/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      295 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FilterCatalog.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.112294 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/
+-rw-rw-r--   0 a         (1000) a         (1000)      546 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/ClusterMols.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1022 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/DbFpSupplier.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1983 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/FingerprintMols.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      756 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/MolSimilarity.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1290 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/SimilarityScreener.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.112294 rdkit-stubs-0.4/rdkit-stubs/Chem/Fraggle/
+-rw-rw-r--   0 a         (1000) a         (1000)      867 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fraggle/FraggleSim.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fraggle/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      492 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FragmentCatalog.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      511 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FragmentMatcher.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      269 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Fragments.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      867 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/FunctionalGroups.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1745 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/GraphDescriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      162 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Graphs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      660 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Lipinski.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      356 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MACCSkeys.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      548 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MCS.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolCatalog.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.112294 rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/
+-rw-rw-r--   0 a         (1000) a         (1000)      915 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/FingerprintUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1206 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/Loader_orig.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1222 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/Loader_sa.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.116294 rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/
+-rw-rw-r--   0 a         (1000) a         (1000)      655 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/InchiInfo.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2096 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/MolKey.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.116294 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/
+-rw-rw-r--   0 a         (1000) a         (1000)      742 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1219 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/charge.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      154 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/errors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      891 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/fragment.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      265 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/metal.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      748 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/normalize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     9763 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/rdMolStandardize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      740 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/resonance.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2389 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/standardize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1453 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/tautomer.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       61 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/utils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      853 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/validate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1244 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/validations.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      959 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/MolSurf.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2918 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/PandasTools.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.120294 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/
+-rw-rw-r--   0 a         (1000) a         (1000)      399 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/Generate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      221 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/Gobbi_Pharm2D.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      465 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/LazyGenerator.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      364 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/Matcher.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1638 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/SigFactory.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1051 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/Utils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      177 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.120294 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/
+-rw-rw-r--   0 a         (1000) a         (1000)     2830 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/EmbedLib.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      259 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/ExcludedVolume.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1626 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/Pharmacophore.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      236 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/PropertyMol.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2221 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/PyMol.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1149 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/QED.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      154 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Randomize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      633 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Recap.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       82 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ReducedGraphs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      292 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/SATIS.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1200 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/SaltRemover.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.120294 rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/
+-rw-rw-r--   0 a         (1000) a         (1000)      595 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/MurckoScaffold.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2487 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/rdScaffoldNetwork.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/ShowMols.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.120294 rdkit-stubs-0.4/rdkit-stubs/Chem/SimpleEnum/
+-rw-rw-r--   0 a         (1000) a         (1000)      483 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/SimpleEnum/Enumerator.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/SimpleEnum/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.124295 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/
+-rw-rw-r--   0 a         (1000) a         (1000)     1102 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/BuilderUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2753 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeAligner.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1006 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeBuilder.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      938 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeObjects.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      513 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/testCombined.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.124295 rdkit-stubs-0.4/rdkit-stubs/Chem/Suppliers/
+-rw-rw-r--   0 a         (1000) a         (1000)     1075 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Suppliers/DbMolSupplier.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      234 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Suppliers/MolSupplier.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/Suppliers/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      303 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/TemplateAlign.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1649 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/TorsionFingerprints.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     4355 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.124295 rdkit-stubs-0.4/rdkit-stubs/Chem/fmcs/
+-rw-rw-r--   0 a         (1000) a         (1000)       35 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/fmcs/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     9857 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/fmcs/fmcs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      912 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/inchi.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1369 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdAbbreviations.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       63 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdCIPLabeler.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)    12742 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdChemReactions.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      905 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdChemicalFeatures.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      883 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdCoordGen.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      386 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdDepictor.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1341 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdDeprotect.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1271 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdDistGeom.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      823 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdEHTTools.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     4345 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdFMCS.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3477 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdFingerprintGenerator.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      879 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdForceFieldHelpers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1337 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdFreeSASA.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1165 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMHFPFingerprint.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      150 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMMPA.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      910 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolAlign.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1779 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolCatalog.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1610 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolChemicalFeatures.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     8906 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolDescriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      652 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolEnumerator.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1022 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolHash.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      462 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolInterchange.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      877 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolTransforms.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       71 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdPartialCharges.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3544 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdRGroupDecomposition.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      181 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdReducedGraphs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      117 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdSLNParse.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      355 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdShapeHelpers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     4807 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdSubstructLibrary.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      850 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdTautomerQuery.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)    41141 2023-05-19 16:05:14.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdchem.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     8330 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdfiltercatalog.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2533 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdfragcatalog.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      237 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdinchi.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)    14476 2023-05-19 16:05:14.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdmolfiles.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     9212 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdmolops.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     4490 2023-05-19 16:05:14.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdqueries.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1219 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Chem/rdtrajectory.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.124295 rdkit-stubs-0.4/rdkit-stubs/DataManip/
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.124295 rdkit-stubs-0.4/rdkit-stubs/DataManip/Metric/
+-rw-rw-r--   0 a         (1000) a         (1000)       91 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataManip/Metric/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      150 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataManip/Metric/rdMetricMatrixCalc.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       50 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataManip/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.128295 rdkit-stubs-0.4/rdkit-stubs/DataStructs/
+-rw-rw-r--   0 a         (1000) a         (1000)      362 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/BitEnsemble.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      375 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/BitEnsembleDb.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      143 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/BitUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      712 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/HierarchyVis.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      316 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/LazySignature.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      442 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/TopNContainer.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      904 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/VectCollection.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      291 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)    16564 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/DataStructs/cDataStructs.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.128295 rdkit-stubs-0.4/rdkit-stubs/Dbase/
+-rw-rw-r--   0 a         (1000) a         (1000)     1753 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbConnection.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      900 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbInfo.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      416 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbModule.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1718 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbReport.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1294 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbResultSet.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1989 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/DbUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      765 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/StorageUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Dbase/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.128295 rdkit-stubs-0.4/rdkit-stubs/DistanceGeometry/
+-rw-rw-r--   0 a         (1000) a         (1000)      108 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DistanceGeometry/DistGeom.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       46 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/DistanceGeometry/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.128295 rdkit-stubs-0.4/rdkit-stubs/ForceField/
+-rw-rw-r--   0 a         (1000) a         (1000)       44 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ForceField/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3387 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/ForceField/rdForceField.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.128295 rdkit-stubs-0.4/rdkit-stubs/Geometry/
+-rw-rw-r--   0 a         (1000) a         (1000)       85 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Geometry/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     6816 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/Geometry/rdGeometry.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.132295 rdkit-stubs-0.4/rdkit-stubs/ML/
+-rw-rw-r--   0 a         (1000) a         (1000)      452 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/AnalyzeComposite.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1012 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/BuildComposite.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.136295 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/
+-rw-rw-r--   0 a         (1000) a         (1000)      237 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Butina.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      289 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/ClusterUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2525 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/ClusterVis.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      124 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Clustering.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1529 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Clusters.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      487 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Murtagh.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      256 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Resemblance.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      117 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Standardize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      152 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/murtagh_test.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.136295 rdkit-stubs-0.4/rdkit-stubs/ML/Composite/
+-rw-rw-r--   0 a         (1000) a         (1000)      196 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Composite/AdjustComposite.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2719 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Composite/Composite.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Composite/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      502 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/CompositeRun.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.136295 rdkit-stubs-0.4/rdkit-stubs/ML/Data/
+-rw-rw-r--   0 a         (1000) a         (1000)     1537 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/DataUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      199 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/FindQuantBounds.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1902 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/MLData.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      835 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/Quantize.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      583 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/SplitData.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      407 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/Stats.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      217 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/Transforms.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      124 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Data/cQuantize.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.140295 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/
+-rw-rw-r--   0 a         (1000) a         (1000)      830 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/BuildQuantTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      751 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/BuildSigTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      717 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/CrossValidate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      907 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/DecTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1277 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/Forest.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      533 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/ID3.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      377 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/PruneTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      515 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/QuantTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      345 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/SigTree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1634 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/Tree.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      169 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/TreeUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      995 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/TreeVis.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      214 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/randomtest.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.140295 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/
+-rw-rw-r--   0 a         (1000) a         (1000)     1657 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/CompoundDescriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      405 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/Descriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      701 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/MoleculeDescriptors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      757 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/Parser.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      704 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/EnrichPlot.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      965 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/GrowComposite.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.144295 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/
+-rw-rw-r--   0 a         (1000) a         (1000)      471 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/BitClusterer.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      425 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/BitRank.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       47 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      226 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/entropy.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1553 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/rdInfoTheory.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.144295 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/
+-rw-rw-r--   0 a         (1000) a         (1000)      716 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/CrossValidate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      177 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/DistFunctions.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      525 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNClassificationModel.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      837 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNModel.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      581 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNRegressionModel.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/KNN/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.144295 rdkit-stubs-0.4/rdkit-stubs/ML/MLUtils/
+-rw-rw-r--   0 a         (1000) a         (1000)      432 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/MLUtils/VoteImg.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/MLUtils/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      176 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/MatOps.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.144295 rdkit-stubs-0.4/rdkit-stubs/ML/ModelPackage/
+-rw-rw-r--   0 a         (1000) a         (1000)      390 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/ModelPackage/PackageUtils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1048 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/ModelPackage/Packager.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/ModelPackage/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.144295 rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/
+-rw-rw-r--   0 a         (1000) a         (1000)     1421 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/ClassificationModel.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      740 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/CrossValidate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       35 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/
+-rw-rw-r--   0 a         (1000) a         (1000)      463 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/ActFuncs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      485 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/CrossValidate.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      620 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/NetNode.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1190 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/Network.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      507 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/Trainers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Neural/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/ML/SLT/
+-rw-rw-r--   0 a         (1000) a         (1000)      223 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/SLT/Risk.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/SLT/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/ML/Scoring/
+-rw-rw-r--   0 a         (1000) a         (1000)      225 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Scoring/Scoring.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/Scoring/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2797 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/ScreenComposite.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      391 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/ML/files.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/Numerics/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Numerics/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       79 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/Numerics/rdAlignment.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      114 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/RDConfig.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      666 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/RDLogger.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      166 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/RDPaths.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       92 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/RDRandom.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/
+-rw-rw-r--   0 a         (1000) a         (1000)     1338 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/SimilarityPickers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      152 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1829 2022-11-09 23:57:57.000000 rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/rdSimDivPickers.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1060 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/TestRunner.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.148295 rdkit-stubs-0.4/rdkit-stubs/VLib/
+-rw-rw-r--   0 a         (1000) a         (1000)      426 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/Filter.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      775 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/Node.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.152295 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/
+-rw-rw-r--   0 a         (1000) a         (1000)      462 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/DbMolSupply.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1253 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/DbPickleSupplier.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      382 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SDSupply.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      406 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmartsMolFilter.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      499 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmartsRemover.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      352 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmilesDupeFilter.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      553 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmilesOutput.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      536 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmilesSupply.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      128 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      384 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/demo.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      369 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/Output.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      418 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/Supply.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      302 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/Transform.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       54 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/VLib/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      162 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     7877 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/rdBase.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.152295 rdkit-stubs-0.4/rdkit-stubs/sping/
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.156295 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/
+-rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3375 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfdoc.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     6354 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfgen.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       75 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfgeom.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      432 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfmetrics.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      475 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfutils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     4210 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pidPDF.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.156295 rdkit-stubs-0.4/rdkit-stubs/sping/PIL/
+-rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PIL/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1976 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PIL/pidPIL.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.156295 rdkit-stubs-0.4/rdkit-stubs/sping/PS/
+-rw-rw-r--   0 a         (1000) a         (1000)       21 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PS/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       91 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PS/fontinfo.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       57 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PS/latin1MetricsCache.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     5577 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PS/pidPS.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      229 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/PS/psmetrics.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.156295 rdkit-stubs-0.4/rdkit-stubs/sping/Pyart/
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/Pyart/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.156295 rdkit-stubs-0.4/rdkit-stubs/sping/Qt/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/Qt/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1904 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/Qt/pidQt.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1814 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/Qt/pidQt4.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/sping/ReportLab/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/ReportLab/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2160 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/ReportLab/pidReportLab.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/sping/SVG/
+-rw-rw-r--   0 a         (1000) a         (1000)       22 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/SVG/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     2818 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/SVG/pidSVG.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/sping/TK/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/TK/__init__.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/sping/WX/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/WX/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      104 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     3670 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/colors.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      422 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/pagesizes.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     5561 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/pid.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1889 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/stringformat.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/sping/util/
+-rw-rw-r--   0 a         (1000) a         (1000)      612 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/util/HTMLPiddler.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/util/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)       64 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/sping/utils.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit-stubs/utils/
+-rw-rw-r--   0 a         (1000) a         (1000)        0 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/__init__.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      259 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/cactvs.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)     1212 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/chemdraw.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      449 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/chemdraw_qax.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      428 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/chemutils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      238 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/comhack.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      112 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/fileutils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      128 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/listutils.pyi
+-rw-rw-r--   0 a         (1000) a         (1000)      350 2022-11-09 23:55:29.000000 rdkit-stubs-0.4/rdkit-stubs/utils/spiral.pyi
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.160295 rdkit-stubs-0.4/rdkit_stubs.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)     1698 2023-05-19 16:46:36.000000 rdkit-stubs-0.4/rdkit_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    12937 2023-05-19 16:46:36.000000 rdkit-stubs-0.4/rdkit_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-19 16:46:36.000000 rdkit-stubs-0.4/rdkit_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        6 2023-05-19 16:46:36.000000 rdkit-stubs-0.4/rdkit_stubs.egg-info/requires.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       12 2023-05-19 16:46:36.000000 rdkit-stubs-0.4/rdkit_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-19 16:46:36.164295 rdkit-stubs-0.4/setup.cfg
+-rw-rw-r--   0 a         (1000) a         (1000)     1226 2023-05-19 16:46:00.000000 rdkit-stubs-0.4/setup.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-19 16:46:36.164295 rdkit-stubs-0.4/test/
+-rw-rw-r--   0 a         (1000) a         (1000)     1009 2023-05-09 22:56:09.000000 rdkit-stubs-0.4/test/test_stubs.py
```

### Comparing `rdkit-stubs-0.3/LICENSE-APACHE` & `rdkit-stubs-0.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/LICENSE-MIT` & `rdkit-stubs-0.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/PKG-INFO` & `rdkit-stubs-0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rdkit-stubs
-Version: 0.3
+Version: 0.4
 Summary: type stubs for rdkit
 Home-page: https://github.com/postera-ai/rdkit-stubs
-Author: Andrew Dirksen
-Author-email: andrew@dirksen.com
+Author: Andrew Dirksen, Ryan Rightmer
+Author-email: andrew@dirksen.com, rrightmer@gmail.com
 License: MIT OR Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Typing :: Stubs Only
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
```

### Comparing `rdkit-stubs-0.3/README.md` & `rdkit-stubs-0.4/README.md`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Avalon/pyAvalonTools.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Avalon/pyAvalonTools.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/AllChem.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/AllChem.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Pairs.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Pairs.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Sheridan.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Sheridan.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/AtomPairs/Torsions.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/AtomPairs/Torsions.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/BRICS.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/BRICS.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/BuildFragmentCatalog.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/BuildFragmentCatalog.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/ChemUtils/TemplateExpand.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/ChemUtils/TemplateExpand.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Crippen.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Crippen.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/DSViewer.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/DSViewer.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Descriptors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Descriptors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/IPythonConsole.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/IPythonConsole.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/InteractiveRenderer.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/InteractiveRenderer.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/MolDrawing.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/MolDrawing.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/SimilarityMaps.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/SimilarityMaps.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/__init__.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/aggCanvas.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/aggCanvas.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/cairoCanvas.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/cairoCanvas.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/canvasbase.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/canvasbase.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/mplCanvas.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/mplCanvas.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/qtCanvas.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/qtCanvas.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/rdMolDraw2D.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/rdMolDraw2D.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Draw/spingCanvas.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Draw/spingCanvas.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/EnumerateStereoisomers.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/EnumerateStereoisomers.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMapParser.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMapParser.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMapUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMapUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/FeatMaps/FeatMaps.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/FeatMaps/FeatMaps.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Features/FeatDirUtilsRD.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Features/FeatDirUtilsRD.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Features/ShowFeats.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Features/ShowFeats.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/ClusterMols.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/ClusterMols.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/DbFpSupplier.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/DbFpSupplier.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/FingerprintMols.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/FingerprintMols.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/MolSimilarity.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/MolSimilarity.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fingerprints/SimilarityScreener.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fingerprints/SimilarityScreener.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Fraggle/FraggleSim.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Fraggle/FraggleSim.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/FunctionalGroups.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/FunctionalGroups.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/GraphDescriptors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/GraphDescriptors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Lipinski.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Lipinski.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MCS.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MCS.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/FingerprintUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/FingerprintUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/Loader_orig.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/Loader_orig.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolDb/Loader_sa.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolDb/Loader_sa.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/InchiInfo.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/InchiInfo.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolKey/MolKey.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolKey/MolKey.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/__init__.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/charge.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/charge.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/fragment.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/fragment.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/normalize.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/normalize.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/rdMolStandardize.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/rdMolStandardize.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/resonance.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/resonance.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/standardize.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/standardize.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/tautomer.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/tautomer.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/validate.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/validate.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolStandardize/validations.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolStandardize/validations.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/MolSurf.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/MolSurf.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/PandasTools.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/PandasTools.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/SigFactory.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/SigFactory.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm2D/Utils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm2D/Utils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/EmbedLib.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/EmbedLib.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Pharm3D/Pharmacophore.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Pharm3D/Pharmacophore.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/PyMol.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/PyMol.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/QED.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/QED.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Recap.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Recap.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/SaltRemover.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/SaltRemover.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/MurckoScaffold.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/MurckoScaffold.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Scaffolds/rdScaffoldNetwork.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Scaffolds/rdScaffoldNetwork.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/BuilderUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/BuilderUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeAligner.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeAligner.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeBuilder.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeBuilder.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/SubshapeObjects.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/SubshapeObjects.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Subshape/testCombined.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Subshape/testCombined.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/Suppliers/DbMolSupplier.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/Suppliers/DbMolSupplier.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/TorsionFingerprints.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/TorsionFingerprints.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/__init__.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/fmcs/fmcs.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/fmcs/fmcs.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/inchi.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/inchi.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdAbbreviations.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdAbbreviations.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdChemReactions.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdChemReactions.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdChemicalFeatures.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdChemicalFeatures.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdCoordGen.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdCoordGen.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdDeprotect.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdDeprotect.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdDistGeom.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdDistGeom.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdEHTTools.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdEHTTools.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdFMCS.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdFMCS.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdFingerprintGenerator.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdFingerprintGenerator.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdForceFieldHelpers.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdForceFieldHelpers.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdFreeSASA.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdFreeSASA.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMHFPFingerprint.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMHFPFingerprint.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolAlign.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolAlign.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolCatalog.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolCatalog.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolChemicalFeatures.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolChemicalFeatures.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolDescriptors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolDescriptors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolEnumerator.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolEnumerator.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolHash.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolHash.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdMolTransforms.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdMolTransforms.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdRGroupDecomposition.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdRGroupDecomposition.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdSubstructLibrary.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdSubstructLibrary.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdTautomerQuery.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdTautomerQuery.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdchem.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdchem.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Iterable
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Optional, Sequence
 
 from typing import overload
 
 ALLOW_CHARGE_SEPARATION: ResonanceFlags
 ALLOW_INCOMPLETE_OCTETS: ResonanceFlags
 AllProps: PropertyPickleOptions
 AtomProps: PropertyPickleOptions
@@ -33,16 +33,15 @@
     __instance_size__: ClassVar[int] = ...
     @classmethod
     def __init__(cls, *args, **kwargs) -> None: ...
     @classmethod
     def ClearProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def DescribeQuery(cls, RDKit) -> Any: ...
-    @classmethod
-    def GetAtomMapNum(cls, RDKit) -> Any: ...
+    def GetAtomMapNum(self) -> int: ...
     def GetAtomicNum(self) -> int: ...
     @classmethod
     def GetBonds(cls, RDKit) -> Any: ...
     @classmethod
     def GetBoolProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetChiralTag(cls, RDKit) -> Any: ...
@@ -54,16 +53,15 @@
     def GetExplicitBitVectProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetExplicitValence(cls, RDKit) -> Any: ...
     @classmethod
     def GetFormalCharge(cls, RDKit) -> Any: ...
     @classmethod
     def GetHybridization(cls, RDKit) -> Any: ...
-    @classmethod
-    def GetIdx(cls, RDKit) -> Any: ...
+    def GetIdx(self) -> int: ...
     @classmethod
     def GetImplicitValence(cls, RDKit) -> Any: ...
     @classmethod
     def GetIntProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetIsAromatic(cls, RDKit) -> Any: ...
     @classmethod
@@ -90,16 +88,15 @@
     def GetProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetPropNames(cls, RDKit) -> Any: ...
     @classmethod
     def GetPropsAsDict(cls, RDKit) -> Any: ...
     @classmethod
     def GetQueryType(cls, RDKit) -> Any: ...
-    @classmethod
-    def GetSmarts(cls, RDKit) -> Any: ...
+    def GetSmarts(self, doKekule: Optional[bool]=False, allHsExplicit: Optional[bool]=False, isomericSmiles: Optional[bool]=True) -> str: ...
     @classmethod
     def GetSymbol(cls, RDKit) -> Any: ...
     @classmethod
     def GetTotalDegree(cls, RDKit) -> Any: ...
     @classmethod
     def GetTotalNumHs(cls, RDKit) -> Any: ...
     @classmethod
@@ -138,16 +135,15 @@
     def SetFormalCharge(cls, RDKit, int) -> Any: ...
     @classmethod
     def SetHybridization(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def SetIntProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def SetIsAromatic(cls, RDKit, bool) -> Any: ...
-    @classmethod
-    def SetIsotope(cls, RDKit, unsignedint) -> Any: ...
+    def SetIsotope(self, arg1: int) -> None: ...
     @classmethod
     def SetMonomerInfo(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def SetNoImplicit(cls, RDKit, bool) -> Any: ...
     @classmethod
     def SetNumExplicitHs(cls, RDKit, unsignedint) -> Any: ...
     @classmethod
@@ -265,16 +261,15 @@
     def GetBoolProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetDoubleProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetEndAtom(cls, RDKit) -> Any: ...
     @classmethod
     def GetEndAtomIdx(cls, RDKit) -> Any: ...
-    @classmethod
-    def GetIdx(cls, RDKit) -> Any: ...
+    def GetIdx(self) -> int: ...
     @classmethod
     def GetIntProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetIsAromatic(cls, RDKit) -> Any: ...
     @classmethod
     def GetIsConjugated(cls, RDKit) -> Any: ...
     @classmethod
@@ -528,19 +523,17 @@
     def Compute2DCoords(cls, RDKit) -> Any: ...
     @classmethod
     def ComputeGasteigerCharges(cls, RDKit) -> Any: ...
     @classmethod
     def Debug(cls, RDKit) -> Any: ...
     @classmethod
     def GetAromaticAtoms(cls, boost) -> Any: ...
-    @classmethod
-    def GetAtomWithIdx(cls, RDKit, unsignedint) -> Any: ...
+    def GetAtomWithIdx(self, idx: int) -> Atom: ...
     def GetAtoms(self) -> Iterable[Atom]: ...
-    @classmethod
-    def GetAtomsMatchingQuery(cls, boost, RDKit) -> Any: ...
+    def GetAtomsMatchingQuery(self, arg2: QueryAtom) -> Sequence[Atom]: ...
     @classmethod
     def GetBondBetweenAtoms(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetBondWithIdx(cls, RDKit, unsignedint) -> Any: ...
     @classmethod
     def GetBonds(cls, boost) -> Any: ...
     @classmethod
@@ -555,16 +548,15 @@
     def GetIntProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetNumAtoms(cls, RDKit) -> Any: ...
     @classmethod
     def GetNumBonds(cls, RDKit) -> Any: ...
     @classmethod
     def GetNumConformers(cls, RDKit) -> Any: ...
-    @classmethod
-    def GetNumHeavyAtoms(cls, RDKit) -> Any: ...
+    def GetNumHeavyAtoms(self) -> int: ...
     @classmethod
     def GetProp(cls, *args, **kwargs) -> Any: ...
     @classmethod
     def GetPropNames(cls, RDKit) -> Any: ...
     @classmethod
     def GetPropsAsDict(cls, RDKit) -> Any: ...
     @classmethod
```

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdfiltercatalog.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdfiltercatalog.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdfragcatalog.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdfragcatalog.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdmolfiles.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdmolfiles.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from types import TracebackType
-from typing import IO, Any, ClassVar, List, Optional, TextIO, Tuple, Union, overload
+from typing import IO, Any, ClassVar, Iterable, List, Optional, TextIO, Tuple, Union, overload
 
 from rdkit.Chem import Mol
+from rdkit.Chem.rdMolDescriptors import AtomPairsParameters
 
 
 class CXSmilesFields:
     CX_ALL: ClassVar[CXSmilesFields] = ...
     CX_ATOM_LABELS: ClassVar[CXSmilesFields] = ...
     CX_ATOM_PROPS: ClassVar[CXSmilesFields] = ...
     CX_COORDS: ClassVar[CXSmilesFields] = ...
@@ -369,15 +370,28 @@
 def CreateAtomIntPropertyList(*args, **kwargs) -> Any: ...
 def CreateAtomStringPropertyList(*args, **kwargs) -> Any: ...
 def MetadataFromPNGFile(boost) -> Any: ...
 def MetadataFromPNGString(boost) -> Any: ...
 def MolFragmentToCXSmarts(RDKit, boost) -> Any: ...
 def MolFragmentToCXSmiles(RDKit, boost) -> Any: ...
 def MolFragmentToSmarts(RDKit, boost) -> Any: ...
-def MolFragmentToSmiles(RDKit, boost) -> Any: ...
+def MolFragmentToSmiles(
+    mol: Mol,
+    atomsToUse: Iterable[int],
+    bondsToUse: Optional[Iterable[int]] = None,
+    atomSymbols: Optional[Iterable[str]] = None,
+    bondSymbols: Optional[Iterable[str]] = None,
+    isomericSmiles: Optional[bool] = True,
+    kekuleSmiles: Optional[bool] = False,
+    rootedAtAtom: Optional[int] = -1,
+    canonical: Optional[bool] = True,
+    allBondsExplicit: Optional[bool] = False,
+    allHsExplicit: Optional[bool] = False,
+    doRandom: Optional[bool] = False,
+) -> str: ...
 def MolFromFASTA(*args, **kwargs) -> Any: ...
 def MolFromHELM(boost) -> Any: ...
 def MolFromMol2Block(*args, **kwargs) -> Any: ...
 def MolFromMol2File(*args, **kwargs) -> Any: ...
 def MolFromMolBlock(boost) -> Any: ...
 def MolFromMolFile(*args, **kwargs) -> Any: ...
 def MolFromPDBBlock(boost) -> Any: ...
@@ -412,15 +426,24 @@
 ) -> str: ...
 def MolToMolFile(*args, **kwargs) -> Any: ...
 def MolToPDBBlock(RDKit) -> Any: ...
 def MolToPDBFile(*args, **kwargs) -> Any: ...
 def MolToRandomSmilesVect(*args, **kwargs) -> Any: ...
 def MolToSequence(RDKit) -> Any: ...
 def MolToSmarts(RDKit) -> Any: ...
-def MolToSmiles(RDKit) -> Any: ...
+def MolToSmiles(
+    mol: Mol,
+    isomericSmiles: Optional[bool] = True,
+    kekuleSmiles: Optional[bool] = False,
+    rootedAtAtom: Optional[int] = -1,
+    canonical: Optional[bool] = True,
+    allBondsExplicit: Optional[bool] = False,
+    allHsExplicit: Optional[bool] = False,
+    doRandom: Optional[bool] = False,
+) -> str: ...
 def MolToTPLBlock(RDKit) -> Any: ...
 def MolToTPLFile(*args, **kwargs) -> Any: ...
 def MolToV3KMolBlock(RDKit) -> Any: ...
 def MolToV3KMolFile(*args, **kwargs) -> Any: ...
 def MolToXYZBlock(RDKit) -> Any: ...
 def MolToXYZFile(*args, **kwargs) -> Any: ...
 def MolsFromPNGFile(*args, **kwargs) -> Any: ...
```

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdmolops.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdmolops.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdqueries.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdqueries.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any
+from typing import Any, Optional
+
+from rdkit.Chem.rdchem import QueryAtom
 
 def AAtomQueryAtom(*args, **kwargs) -> Any: ...
 def AHAtomQueryAtom(*args, **kwargs) -> Any: ...
 def AtomNumEqualsQueryAtom(*args, **kwargs) -> Any: ...
 def AtomNumGreaterQueryAtom(*args, **kwargs) -> Any: ...
 def AtomNumLessQueryAtom(*args, **kwargs) -> Any: ...
 def ExplicitDegreeEqualsQueryAtom(*args, **kwargs) -> Any: ...
@@ -19,15 +21,15 @@
 def HCountLessQueryAtom(*args, **kwargs) -> Any: ...
 def HasBitVectPropWithValueQueryAtom(*args, **kwargs) -> Any: ...
 def HasBoolPropWithValueQueryAtom(*args, **kwargs) -> Any: ...
 def HasBoolPropWithValueQueryBond(*args, **kwargs) -> Any: ...
 def HasChiralTagQueryAtom(*args, **kwargs) -> Any: ...
 def HasDoublePropWithValueQueryAtom(*args, **kwargs) -> Any: ...
 def HasDoublePropWithValueQueryBond(*args, **kwargs) -> Any: ...
-def HasIntPropWithValueQueryAtom(*args, **kwargs) -> Any: ...
+def HasIntPropWithValueQueryAtom(propname: str, val: int, negate: Optional[bool]=False, tolerance: Optional[int]=0) -> QueryAtom: ...
 def HasIntPropWithValueQueryBond(*args, **kwargs) -> Any: ...
 def HasPropQueryAtom(*args, **kwargs) -> Any: ...
 def HasPropQueryBond(*args, **kwargs) -> Any: ...
 def HasStringPropWithValueQueryAtom(*args, **kwargs) -> Any: ...
 def HasStringPropWithValueQueryBond(*args, **kwargs) -> Any: ...
 def HybridizationEqualsQueryAtom(*args, **kwargs) -> Any: ...
 def HybridizationGreaterQueryAtom(*args, **kwargs) -> Any: ...
```

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Chem/rdtrajectory.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Chem/rdtrajectory.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/DataStructs/HierarchyVis.pyi` & `rdkit-stubs-0.4/rdkit-stubs/DataStructs/HierarchyVis.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/DataStructs/VectCollection.pyi` & `rdkit-stubs-0.4/rdkit-stubs/DataStructs/VectCollection.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/DataStructs/cDataStructs.pyi` & `rdkit-stubs-0.4/rdkit-stubs/DataStructs/cDataStructs.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/DbConnection.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/DbConnection.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/DbInfo.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/DbInfo.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/DbReport.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/DbReport.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/DbResultSet.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/DbResultSet.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/DbUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/DbUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Dbase/StorageUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Dbase/StorageUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ForceField/rdForceField.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ForceField/rdForceField.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/Geometry/rdGeometry.pyi` & `rdkit-stubs-0.4/rdkit-stubs/Geometry/rdGeometry.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/BuildComposite.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/BuildComposite.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/ClusterVis.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/ClusterVis.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Cluster/Clusters.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Cluster/Clusters.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Composite/Composite.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Composite/Composite.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Data/DataUtils.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Data/DataUtils.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Data/MLData.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Data/MLData.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Data/Quantize.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Data/Quantize.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Data/SplitData.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Data/SplitData.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/BuildQuantTree.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/BuildQuantTree.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/BuildSigTree.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/BuildSigTree.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/CrossValidate.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/CrossValidate.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/DecTree.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/DecTree.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/Forest.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/Forest.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/ID3.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/ID3.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/QuantTree.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/QuantTree.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/Tree.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/Tree.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/DecTree/TreeVis.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/DecTree/TreeVis.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/CompoundDescriptors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/CompoundDescriptors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/MoleculeDescriptors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/MoleculeDescriptors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Descriptors/Parser.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Descriptors/Parser.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/EnrichPlot.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/EnrichPlot.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/GrowComposite.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/GrowComposite.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/InfoTheory/rdInfoTheory.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/InfoTheory/rdInfoTheory.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/KNN/CrossValidate.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/KNN/CrossValidate.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNClassificationModel.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNClassificationModel.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNModel.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNModel.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/KNN/KNNRegressionModel.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/KNN/KNNRegressionModel.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/ModelPackage/Packager.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/ModelPackage/Packager.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/ClassificationModel.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/ClassificationModel.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/NaiveBayes/CrossValidate.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/NaiveBayes/CrossValidate.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Neural/NetNode.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Neural/NetNode.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/Neural/Network.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/Neural/Network.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/ML/ScreenComposite.pyi` & `rdkit-stubs-0.4/rdkit-stubs/ML/ScreenComposite.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/RDLogger.pyi` & `rdkit-stubs-0.4/rdkit-stubs/RDLogger.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/SimilarityPickers.pyi` & `rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/SimilarityPickers.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/SimDivFilters/rdSimDivPickers.pyi` & `rdkit-stubs-0.4/rdkit-stubs/SimDivFilters/rdSimDivPickers.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/TestRunner.pyi` & `rdkit-stubs-0.4/rdkit-stubs/TestRunner.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/VLib/Node.pyi` & `rdkit-stubs-0.4/rdkit-stubs/VLib/Node.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/DbPickleSupplier.pyi` & `rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/DbPickleSupplier.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmilesOutput.pyi` & `rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmilesOutput.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/VLib/NodeLib/SmilesSupply.pyi` & `rdkit-stubs-0.4/rdkit-stubs/VLib/NodeLib/SmilesSupply.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/rdBase.pyi` & `rdkit-stubs-0.4/rdkit-stubs/rdBase.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfdoc.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfdoc.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pdfgen.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pdfgen.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/PDF/pidPDF.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/PDF/pidPDF.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/PIL/pidPIL.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/PIL/pidPIL.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/PS/pidPS.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/PS/pidPS.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/Qt/pidQt.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/Qt/pidQt.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/Qt/pidQt4.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/Qt/pidQt4.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/ReportLab/pidReportLab.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/ReportLab/pidReportLab.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/SVG/pidSVG.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/SVG/pidSVG.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/colors.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/colors.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/pid.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/pid.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/stringformat.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/stringformat.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/sping/util/HTMLPiddler.pyi` & `rdkit-stubs-0.4/rdkit-stubs/sping/util/HTMLPiddler.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit-stubs/utils/chemdraw.pyi` & `rdkit-stubs-0.4/rdkit-stubs/utils/chemdraw.pyi`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/rdkit_stubs.egg-info/PKG-INFO` & `rdkit-stubs-0.4/rdkit_stubs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rdkit-stubs
-Version: 0.3
+Version: 0.4
 Summary: type stubs for rdkit
 Home-page: https://github.com/postera-ai/rdkit-stubs
-Author: Andrew Dirksen
-Author-email: andrew@dirksen.com
+Author: Andrew Dirksen, Ryan Rightmer
+Author-email: andrew@dirksen.com, rrightmer@gmail.com
 License: MIT OR Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Typing :: Stubs Only
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
```

### Comparing `rdkit-stubs-0.3/rdkit_stubs.egg-info/SOURCES.txt` & `rdkit-stubs-0.4/rdkit_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdkit-stubs-0.3/setup.py` & `rdkit-stubs-0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 long_description = (Path(__file__).parent.resolve() / "README.md").read_text(
     encoding="utf-8"
 )
 
 
 setup(
     name="rdkit-stubs",
-    version="0.3",
+    version="0.4",
     description="type stubs for rdkit",
-    author="Andrew Dirksen",
-    author_email="andrew@dirksen.com",
+    author="Andrew Dirksen, Ryan Rightmer",
+    author_email="andrew@dirksen.com, rrightmer@gmail.com",
     license="MIT OR Apache-2.0",
     url="https://github.com/postera-ai/rdkit-stubs",
     packages=["rdkit-stubs"],
     package_data={"rdkit-stubs": list_package_files()},
     classifiers=[
         "Development Status :: 1 - Planning",
         "Typing :: Stubs Only",
```

### Comparing `rdkit-stubs-0.3/test/test_stubs.py` & `rdkit-stubs-0.4/test/test_stubs.py`

 * *Files identical despite different names*

