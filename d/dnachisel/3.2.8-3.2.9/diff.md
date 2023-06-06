# Comparing `tmp/dnachisel-3.2.8.tar.gz` & `tmp/dnachisel-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dnachisel-3.2.8.tar", last modified: Tue Sep  7 12:49:02 2021, max compression
+gzip compressed data, was "dnachisel-3.2.9.tar", last modified: Thu May  5 16:31:58 2022, max compression
```

## Comparing `dnachisel-3.2.8.tar` & `dnachisel-3.2.9.tar`

### file list

```diff
@@ -1,383 +1,198 @@
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/
--rw-r--r--   0 peter     (1001) peter     (1001)     8512 2020-08-10 12:55:43.000000 dnachisel-3.2.8/ez_setup.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     1081 2020-09-06 16:13:31.000000 dnachisel-3.2.8/LICENCE.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)     1510 2020-09-06 16:13:31.000000 dnachisel-3.2.8/setup.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/MutationSpace/
--rw-r--r--   0 peter     (1001) peter     (1001)     5118 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/MutationSpace/MutationChoice.py
--rw-rw-r--   0 peter     (1001) peter     (1001)    10656 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/MutationSpace/MutationSpace.py
--rw-r--r--   0 peter     (1001) peter     (1001)      131 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/MutationSpace/__init__.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/
--rw-rw-r--   0 peter     (1001) peter     (1001)     2515 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceRegionsCompatibility.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     3070 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AllowPrimer.py
--rw-rw-r--   0 peter     (1001) peter     (1001)    11935 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceChanges.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     4627 2021-07-21 11:43:14.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceSequence.py
--rw-r--r--   0 peter     (1001) peter     (1001)     4665 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidBlastMatches.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1156 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/SequenceLengthBounds.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     7989 2021-09-07 12:48:33.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforcePatternOccurence.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/
--rw-r--r--   0 peter     (1001) peter     (1001)     3377 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/BaseCodonOptimizationClass.py
--rw-r--r--   0 peter     (1001) peter     (1001)     5353 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/MaximizeCAI.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     4405 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/CodonOptimize.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     6606 2021-07-21 11:43:14.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/HarmonizeRCA.py
--rw-r--r--   0 peter     (1001) peter     (1001)     4895 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/AvoidRareCodons.py
--rw-r--r--   0 peter     (1001) peter     (1001)      346 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/__init__.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     8080 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/MatchTargetCodonUsage.py
--rw-r--r--   0 peter     (1001) peter     (1001)     4860 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidMatches.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2176 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/TerminalSpecification.py
--rw-r--r--   0 peter     (1001) peter     (1001)     3320 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidHairpins.py
--rw-rw-r--   0 peter     (1001) peter     (1001)    11007 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/UniquifyAllKmers.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2342 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/CodonSpecification.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2693 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/__init__.py
--rw-r--r--   0 peter     (1001) peter     (1001)     6509 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidChanges.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     7026 2021-04-17 16:52:29.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceGCContent.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1970 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidStopCodons.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2596 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidHeterodimerization.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     4006 2021-09-07 12:48:33.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidPattern.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     2560 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceMeltingTemperature.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1108 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceTerminalGCContent.py
--rw-r--r--   0 peter     (1001) peter     (1001)     3293 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceChoice.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     8936 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceTranslation.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     6404 2021-09-07 12:48:33.000000 dnachisel-3.2.8/dnachisel/Location.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/
--rw-r--r--   0 peter     (1001) peter     (1001)     7154 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/RecordRepresentationMixin.py
--rw-r--r--   0 peter     (1001) peter     (1001)     8618 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/ObjectivesMaximizerMixin.py
--rw-r--r--   0 peter     (1001) peter     (1001)      296 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/__init__.py
--rw-r--r--   0 peter     (1001) peter     (1001)    15803 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/ConstraintsSolverMixin.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     9409 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/DnaOptimizationProblem.py
--rw-r--r--   0 peter     (1001) peter     (1001)      284 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/__init__.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     7668 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/CircularDnaOptimizationProblem.py
--rw-r--r--   0 peter     (1001) peter     (1001)      500 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/NoSolutionError.py
--rw-rw-r--   0 peter     (1001) peter     (1001)       22 2021-09-07 12:48:33.000000 dnachisel-3.2.8/dnachisel/version.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/biotools/
--rw-rw-r--   0 peter     (1001) peter     (1001)     3810 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/biotools/sequences_operations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1211 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/gc_content.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2970 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/blast_sequence.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1491 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/enzymes_operations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1280 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/sequences_differences.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2537 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/bowtie.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/biotools/data/
--rw-r--r--   0 peter     (1001) peter     (1001)       81 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/data/iupac_notation.csv
--rw-r--r--   0 peter     (1001) peter     (1001)      132 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/data/nucleotide_to_regexpr.csv
--rw-rw-r--   0 peter     (1001) peter     (1001)      470 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/biotools/data/README.md
--rw-r--r--   0 peter     (1001) peter     (1001)       68 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/data/complements.csv
--rw-r--r--   0 peter     (1001) peter     (1001)     1378 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/formatting_operations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     3114 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/indices_operations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2028 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/random_sequences.py
--rw-r--r--   0 peter     (1001) peter     (1001)     2208 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/biotools/__init__.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     1976 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/biotools/biotables.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     7189 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/biotools/genbank_operations.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/utils/
--rw-r--r--   0 peter     (1001) peter     (1001)     1250 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/utils/utils.py
--rw-r--r--   0 peter     (1001) peter     (1001)      178 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/utils/__init__.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     3075 2021-04-17 16:51:41.000000 dnachisel-3.2.8/dnachisel/__init__.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/Specification/
--rw-r--r--   0 peter     (1001) peter     (1001)     8923 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/Specification.py
--rw-r--r--   0 peter     (1001) peter     (1001)     6223 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/FeatureRepresentationMixin.py
--rw-rw-r--   0 peter     (1001) peter     (1001)      567 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/Specification/SpecificationSet.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/
--rw-r--r--   0 peter     (1001) peter     (1001)     1152 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/ProblemObjectivesEvaluations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     5448 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/SpecEvaluation.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1727 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/ProblemConstraintsEvaluations.py
--rw-r--r--   0 peter     (1001) peter     (1001)      364 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/__init__.py
--rw-r--r--   0 peter     (1001) peter     (1001)     6625 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/SpecEvaluations.py
--rw-r--r--   0 peter     (1001) peter     (1001)      130 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/Specification/__init__.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/SequencePattern/
--rw-rw-r--   0 peter     (1001) peter     (1001)     7781 2021-01-05 14:55:36.000000 dnachisel-3.2.8/dnachisel/SequencePattern/MotifPssmPattern.py
--rw-r--r--   0 peter     (1001) peter     (1001)      828 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/SequencePattern/HomopolymerPattern.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     5808 2021-01-05 14:55:36.000000 dnachisel-3.2.8/dnachisel/SequencePattern/SequencePattern.py
--rw-r--r--   0 peter     (1001) peter     (1001)      613 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/SequencePattern/__init__.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     1781 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/SequencePattern/DnaNotationPattern.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     1112 2021-01-05 14:55:36.000000 dnachisel-3.2.8/dnachisel/SequencePattern/RepeatedKmerPattern.py
--rw-r--r--   0 peter     (1001) peter     (1001)      932 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/SequencePattern/EnzymeSitePattern.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/reports/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/reports/constraints_reports/
--rw-r--r--   0 peter     (1001) peter     (1001)     1077 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/constraints_reports/GraphicTranslator.py
--rw-r--r--   0 peter     (1001) peter     (1001)     5119 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/constraints_reports/constraints_reports.py
--rw-r--r--   0 peter     (1001) peter     (1001)      427 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/constraints_reports/__init__.py
--rw-r--r--   0 peter     (1001) peter     (1001)     3025 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/constraints_reports/constraints_breaches_dataframe.py
--rw-rw-r--   0 peter     (1001) peter     (1001)    14144 2021-01-07 13:13:17.000000 dnachisel-3.2.8/dnachisel/reports/optimization_reports.py
--rw-r--r--   0 peter     (1001) peter     (1001)      377 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/tools.py
--rw-r--r--   0 peter     (1001) peter     (1001)     1835 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/SpecAnnotationsTranslator.py
--rw-r--r--   0 peter     (1001) peter     (1001)      315 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/__init__.py
--rw-r--r--   0 peter     (1001) peter     (1001)      826 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/colors_cycle.py
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel/reports/assets/
--rw-rw-r--   0 peter     (1001) peter     (1001)     2726 2021-07-21 11:43:14.000000 dnachisel-3.2.8/dnachisel/reports/assets/optimization_report.pug
--rw-r--r--   0 peter     (1001) peter     (1001)        0 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/assets/style.css
--rw-r--r--   0 peter     (1001) peter     (1001)    20513 2020-08-10 12:55:43.000000 dnachisel-3.2.8/dnachisel/reports/assets/logo.png
--rw-rw-r--   0 peter     (1001) peter     (1001)       38 2021-09-07 12:49:02.000000 dnachisel-3.2.8/setup.cfg
--rw-rw-r--   0 peter     (1001) peter     (1001)     3029 2020-09-06 16:13:31.000000 dnachisel-3.2.8/pypi-readme.rst
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/
--rw-r--r--   0 peter     (1001) peter     (1001)    17220 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1001) peter     (1001)      134 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/requires.txt
--rw-r--r--   0 peter     (1001) peter     (1001)        1 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1001) peter     (1001)     3371 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1001) peter     (1001)       10 2021-09-07 12:49:02.000000 dnachisel-3.2.8/dnachisel.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/
--rw-rw-r--   0 peter     (1001) peter     (1001)      466 2021-09-07 12:48:33.000000 dnachisel-3.2.8/docs/notes.rst
--rw-r--r--   0 peter     (1001) peter     (1001)     6707 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/make.bat
--rw-r--r--   0 peter     (1001) peter     (1001)     1399 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/examples.rst
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/genbank/
--rw-rw-r--   0 peter     (1001) peter     (1001)    11554 2021-07-21 11:43:14.000000 dnachisel-3.2.8/docs/genbank/genbank_api.rst
--rw-rw-r--   0 peter     (1001) peter     (1001)     2209 2021-01-07 13:13:17.000000 dnachisel-3.2.8/docs/genbank/genbank_notes.rst
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_static/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_static/css/
--rw-r--r--   0 peter     (1001) peter     (1001)     1478 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/css/custom.css
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_static/images/
--rw-r--r--   0 peter     (1001) peter     (1001)     8498 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/old_html_logo.png
--rw-r--r--   0 peter     (1001) peter     (1001)     1299 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/pw_maze_dark.png
--rw-r--r--   0 peter     (1001) peter     (1001)    87760 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/report_screenshot.png
--rw-r--r--   0 peter     (1001) peter     (1001)    93263 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/example_sequence.png
--rw-r--r--   0 peter     (1001) peter     (1001)     3121 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/confectionary.png
--rw-r--r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/pw_maze_black.png
--rw-r--r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/pw_maze_black (copy).png
--rw-r--r--   0 peter     (1001) peter     (1001)   896059 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/dnachisel_algorithm.gif
--rw-r--r--   0 peter     (1001) peter     (1001)    16412 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/html_logo.png
--rw-r--r--   0 peter     (1001) peter     (1001)     2138 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/geometry2.png
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/
--rw-r--r--   0 peter     (1001) peter     (1001)     6190 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_cg_obj.png
--rw-r--r--   0 peter     (1001) peter     (1001)     5682 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting_obj.png
--rw-r--r--   0 peter     (1001) peter     (1001)    10389 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_sequence.png
--rw-r--r--   0 peter     (1001) peter     (1001)    10654 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/all_unique_kmers_here.png
--rw-r--r--   0 peter     (1001) peter     (1001)    12703 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting_and_kmers.png
--rw-r--r--   0 peter     (1001) peter     (1001)     8450 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/use_best_codon.png
--rw-r--r--   0 peter     (1001) peter     (1001)     6237 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/change_objective.png
--rw-r--r--   0 peter     (1001) peter     (1001)    14900 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/cds_enforce.png
--rw-r--r--   0 peter     (1001) peter     (1001)     8402 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_regex.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9408 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/allow_primer.png
--rw-r--r--   0 peter     (1001) peter     (1001)    13430 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/multiple_specs.png
--rw-r--r--   0 peter     (1001) peter     (1001)    11048 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_enzyme.png
--rw-r--r--   0 peter     (1001) peter     (1001)     4773 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/keep_obj.png
--rw-r--r--   0 peter     (1001) peter     (1001)    12612 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_matches_mismatches.png
--rw-r--r--   0 peter     (1001) peter     (1001)     6975 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_cg.png
--rw-r--r--   0 peter     (1001) peter     (1001)     7645 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/gc_range.png
--rw-r--r--   0 peter     (1001) peter     (1001)     7807 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_kmer.png
--rw-r--r--   0 peter     (1001) peter     (1001)     7297 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting.png
--rw-r--r--   0 peter     (1001) peter     (1001)     5678 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/cds.png
--rw-r--r--   0 peter     (1001) peter     (1001)     6309 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/change.png
--rw-r--r--   0 peter     (1001) peter     (1001)    12056 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/myspec.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9706 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/insert_several.png
--rw-r--r--   0 peter     (1001) peter     (1001)     5921 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/keep.png
--rw-r--r--   0 peter     (1001) peter     (1001)      124 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/README.md
--rw-r--r--   0 peter     (1001) peter     (1001)     8337 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/gc_target.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9306 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_noisoleucine.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9026 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/boosting.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    10180 2021-07-21 11:43:14.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/harmonize_rca.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9955 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/all_unique_kmers.png
--rw-r--r--   0 peter     (1001) peter     (1001)    25370 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_blast.png
--rw-r--r--   0 peter     (1001) peter     (1001)     1903 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/generate_annotations.py
--rw-r--r--   0 peter     (1001) peter     (1001)     9137 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/codon_optimize.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     2421 2021-07-21 11:43:14.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/examples.csv
--rw-r--r--   0 peter     (1001) peter     (1001)     9056 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/insert.png
--rw-r--r--   0 peter     (1001) peter     (1001)     9934 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_matches.png
--rw-r--r--   0 peter     (1001) peter     (1001)     8032 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/choice.png
--rw-r--r--   0 peter     (1001) peter     (1001)    22054 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_non_unique_segments.png
--rw-r--r--   0 peter     (1001) peter     (1001)     8238 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/genbank_annotations/match_codon_usage.png
--rw-r--r--   0 peter     (1001) peter     (1001)    16412 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/title.png
--rw-r--r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_static/images/pw_maze_white.png
--rw-r--r--   0 peter     (1001) peter     (1001)     1551 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/favicon.png
--rw-r--r--   0 peter     (1001) peter     (1001)      114 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/build_and_deploy.sh
--rw-r--r--   0 peter     (1001) peter     (1001)      211 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/README.md
--rw-r--r--   0 peter     (1001) peter     (1001)        7 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/.gitignore
--rw-r--r--   0 peter     (1001) peter     (1001)     1340 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/index.rst
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/
--rw-rw-r--   0 peter     (1001) peter     (1001)     8504 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/py-modindex.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    25394 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/searchindex.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    11858 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/examples.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_sources/
--rw-rw-r--   0 peter     (1001) peter     (1001)     1399 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/examples.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)      466 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/notes.rst.txt
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_sources/genbank/
--rw-rw-r--   0 peter     (1001) peter     (1001)     2209 2021-01-07 13:13:17.000000 dnachisel-3.2.8/docs/_build/html/_sources/genbank/genbank_notes.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)    11554 2021-06-14 23:52:23.000000 dnachisel-3.2.8/docs/_build/html/_sources/genbank/genbank_api.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)      211 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/README.md.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)     1340 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/
--rw-rw-r--   0 peter     (1001) peter     (1001)     2316 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/core_classes.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)      108 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/constraints_reports.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)     1960 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/builtin_specifications.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)       65 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/biotools.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)       85 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/reports.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)      574 2021-01-07 13:13:17.000000 dnachisel-3.2.8/docs/_build/html/_sources/ref/cli.rst.txt
--rw-rw-r--   0 peter     (1001) peter     (1001)     1785 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/objects.inv
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/genbank/
--rw-rw-r--   0 peter     (1001) peter     (1001)    28400 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/genbank/genbank_api.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    12041 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/genbank/genbank_notes.html
--rw-rw-r--   0 peter     (1001) peter     (1001)     7464 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/search.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_static/
--rw-rw-r--   0 peter     (1001) peter     (1001)     2137 2020-09-04 10:31:03.000000 dnachisel-3.2.8/docs/_build/html/_static/sphinx_press_theme.css
--rw-rw-r--   0 peter     (1001) peter     (1001)       90 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/plus.png
--rw-rw-r--   0 peter     (1001) peter     (1001)   114436 2020-09-04 10:31:03.000000 dnachisel-3.2.8/docs/_build/html/_static/theme-vendors.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    17024 2020-09-04 10:31:03.000000 dnachisel-3.2.8/docs/_build/html/_static/theme.css
--rw-rw-r--   0 peter     (1001) peter     (1001)    10847 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 peter     (1001) peter     (1001)      286 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/file.png
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_static/css/
--rw-rw-r--   0 peter     (1001) peter     (1001)     1478 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/css/custom.css
--rw-rw-r--   0 peter     (1001) peter     (1001)       90 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/minus.png
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_static/images/
--rw-rw-r--   0 peter     (1001) peter     (1001)     8498 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/old_html_logo.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     1299 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/pw_maze_dark.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    87760 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/report_screenshot.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    93263 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/example_sequence.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     3121 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/confectionary.png
--rw-rw-r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/pw_maze_black.png
--rw-rw-r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/pw_maze_black (copy).png
--rw-rw-r--   0 peter     (1001) peter     (1001)   896059 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/dnachisel_algorithm.gif
--rw-rw-r--   0 peter     (1001) peter     (1001)    16412 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/html_logo.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     2138 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/geometry2.png
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/
--rw-rw-r--   0 peter     (1001) peter     (1001)     6190 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_cg_obj.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     5682 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/enforce_melting_obj.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    10389 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/enforce_sequence.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    10654 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/all_unique_kmers_here.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    12703 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/enforce_melting_and_kmers.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     8450 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/use_best_codon.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     6237 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/change_objective.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    14900 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/cds_enforce.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     8402 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_regex.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9408 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/allow_primer.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    13430 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/multiple_specs.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    11048 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_enzyme.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     4773 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/keep_obj.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    12612 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_matches_mismatches.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     6975 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_cg.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     7645 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/gc_range.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     7807 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_kmer.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     7297 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/enforce_melting.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     5678 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/cds.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     6309 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/change.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    12056 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/myspec.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9706 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/insert_several.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     5921 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/keep.png
--rw-rw-r--   0 peter     (1001) peter     (1001)      124 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/README.md
--rw-rw-r--   0 peter     (1001) peter     (1001)     8337 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/gc_target.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9306 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_pattern_noisoleucine.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9026 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/boosting.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    10180 2021-06-15 17:08:53.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/harmonize_rca.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9955 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/all_unique_kmers.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    25370 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_blast.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     1903 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/generate_annotations.py
--rw-rw-r--   0 peter     (1001) peter     (1001)     9137 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/codon_optimize.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     2421 2021-06-15 17:11:24.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/examples.csv
--rw-rw-r--   0 peter     (1001) peter     (1001)     9056 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/insert.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     9934 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_matches.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     8032 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/choice.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    22054 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/avoid_non_unique_segments.png
--rw-rw-r--   0 peter     (1001) peter     (1001)     8238 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/genbank_annotations/match_codon_usage.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    16412 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/title.png
--rw-rw-r--   0 peter     (1001) peter     (1001)      600 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/images/pw_maze_white.png
--rw-rw-r--   0 peter     (1001) peter     (1001)   287630 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    16412 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/_build/html/_static/html_logo.png
--rw-rw-r--   0 peter     (1001) peter     (1001)    16288 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    13633 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_static/basic.css
--rw-rw-r--   0 peter     (1001) peter     (1001)     9354 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    89476 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 peter     (1001) peter     (1001)     4557 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 peter     (1001) peter     (1001)     5114 2020-09-04 10:31:03.000000 dnachisel-3.2.8/docs/_build/html/_static/theme.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    35168 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 peter     (1001) peter     (1001)      355 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    12140 2020-09-02 19:18:24.000000 dnachisel-3.2.8/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 peter     (1001) peter     (1001)    32492 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/genindex.html
--rw-rw-r--   0 peter     (1001) peter     (1001)     7099 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/README.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    21608 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/index.html
--rw-rw-r--   0 peter     (1001) peter     (1001)      230 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/.buildinfo
--rw-rw-r--   0 peter     (1001) peter     (1001)     8430 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/notes.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/MutationSpace/
--rw-rw-r--   0 peter     (1001) peter     (1001)    52760 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/MutationSpace/MutationSpace.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    28238 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/MutationSpace/MutationChoice.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/
--rw-rw-r--   0 peter     (1001) peter     (1001)    15195 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidStopCodons.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    25273 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforceSequence.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    11646 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/SequenceLengthBounds.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    17535 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforceRegionsCompatibility.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/
--rw-rw-r--   0 peter     (1001) peter     (1001)    16622 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/CodonOptimize.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    30565 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/MatchTargetCodonUsage.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    28383 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/HarmonizeRCA.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    24160 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/MaximizeCAI.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    23253 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/codon_optimization/AvoidRareCodons.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    21719 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidPattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    23313 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidMatches.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    25321 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidBlastMatches.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    33959 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidChanges.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    37385 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforceGCContent.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    15680 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AllowPrimer.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    17233 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforceMeltingTemperature.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    38000 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforceTranslation.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    35610 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/EnforcePatternOccurence.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    48063 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/UniquifyAllKmers.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    21317 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/builtin_specifications/AvoidHairpins.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    34955 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/Location.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/DnaOptimizationProblem/
--rw-rw-r--   0 peter     (1001) peter     (1001)    33508 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/DnaOptimizationProblem/DnaOptimizationProblem.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    36352 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/DnaOptimizationProblem/CircularDnaOptimizationProblem.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/
--rw-rw-r--   0 peter     (1001) peter     (1001)    19900 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/bowtie.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    11276 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/gc_content.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    14695 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/random_sequences.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    20840 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/sequences_operations.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    19339 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/indices_operations.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    13820 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/formatting_operations.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    21467 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/blast_sequence.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    36848 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/genbank_operations.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    12216 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/enzymes_operations.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    13180 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/biotools/sequences_differences.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/Specification/
--rw-rw-r--   0 peter     (1001) peter     (1001)    32190 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/Specification/Specification.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/
--rw-rw-r--   0 peter     (1001) peter     (1001)    10722 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/HomopolymerPattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    26869 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/SequencePattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    14725 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/DnaNotationPattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    12004 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/RepeatedKmerPattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    11190 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/EnzymeSitePattern.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    33515 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/SequencePattern/MotifPssmPattern.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/constraints_reports/
--rw-rw-r--   0 peter     (1001) peter     (1001)    27347 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/constraints_reports/constraints_reports.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    17181 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/constraints_reports/constraints_breaches_dataframe.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    13181 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/constraints_reports/GraphicTranslator.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    65579 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/dnachisel/reports/optimization_reports.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    12398 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/_modules/index.html
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/html/ref/
--rw-rw-r--   0 peter     (1001) peter     (1001)    20011 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/ref/constraints_reports.html
--rw-rw-r--   0 peter     (1001) peter     (1001)     9459 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/ref/cli.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    84926 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/ref/builtin_specifications.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    93890 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/ref/core_classes.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    12721 2021-09-07 11:45:42.000000 dnachisel-3.2.8/docs/_build/html/ref/reports.html
--rw-rw-r--   0 peter     (1001) peter     (1001)    46795 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/ref/biotools.html
--rw-rw-r--   0 peter     (1001) peter     (1001)        0 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/html/.nojekyll
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/doctrees/
--rw-rw-r--   0 peter     (1001) peter     (1001)   365589 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 peter     (1001) peter     (1001)     3682 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/notes.doctree
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/doctrees/genbank/
--rw-rw-r--   0 peter     (1001) peter     (1001)    53224 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/genbank/genbank_api.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)     9887 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/genbank/genbank_notes.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)     2913 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/README.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)    36587 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)    13573 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/examples.doctree
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/
--rw-rw-r--   0 peter     (1001) peter     (1001)   261723 2021-09-07 11:45:40.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/builtin_specifications.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)     6306 2021-09-07 11:45:40.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/cli.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)   137239 2021-09-07 11:45:39.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/biotools.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)   273047 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/core_classes.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)    23729 2021-09-07 11:45:41.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/reports.doctree
--rw-rw-r--   0 peter     (1001) peter     (1001)    39712 2021-09-07 11:45:40.000000 dnachisel-3.2.8/docs/_build/doctrees/ref/constraints_reports.doctree
--rw-r--r--   0 peter     (1001) peter     (1001)    10829 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/conf.py
--rw-r--r--   0 peter     (1001) peter     (1001)     6878 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/Makefile
--rwxr-xr-x   0 peter     (1001) peter     (1001)       51 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/makehtml.sh
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/docs/ref/
--rw-r--r--   0 peter     (1001) peter     (1001)     1960 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/ref/builtin_specifications.rst
--rw-r--r--   0 peter     (1001) peter     (1001)       65 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/ref/biotools.rst
--rw-r--r--   0 peter     (1001) peter     (1001)       85 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/ref/reports.rst
--rw-r--r--   0 peter     (1001) peter     (1001)     2316 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/ref/core_classes.rst
--rw-r--r--   0 peter     (1001) peter     (1001)      108 2020-08-10 12:55:43.000000 dnachisel-3.2.8/docs/ref/constraints_reports.rst
--rw-rw-r--   0 peter     (1001) peter     (1001)      574 2021-09-07 12:48:33.000000 dnachisel-3.2.8/docs/ref/cli.rst
--rw-rw-r--   0 peter     (1001) peter     (1001)     3371 2021-09-07 12:49:02.000000 dnachisel-3.2.8/PKG-INFO
--rw-r--r--   0 peter     (1001) peter     (1001)      162 2020-08-10 12:55:43.000000 dnachisel-3.2.8/MANIFEST.in
--rw-rw-r--   0 peter     (1001) peter     (1001)     7939 2021-07-21 11:43:14.000000 dnachisel-3.2.8/README.rst
-drwxrwxr-x   0 peter     (1001) peter     (1001)        0 2021-09-07 12:49:02.000000 dnachisel-3.2.8/scripts/
--rwxrwxr-x   0 peter     (1001) peter     (1001)     2677 2021-09-07 12:48:33.000000 dnachisel-3.2.8/scripts/dnachisel
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.254294 dnachisel-3.2.9/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1081 2022-01-21 13:20:47.000000 dnachisel-3.2.9/LICENCE.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      162 2022-01-21 13:20:47.000000 dnachisel-3.2.9/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3371 2022-05-05 16:31:58.254294 dnachisel-3.2.9/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7939 2022-01-21 13:20:47.000000 dnachisel-3.2.9/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.174295 dnachisel-3.2.9/dnachisel/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.178295 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7668 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/CircularDnaOptimizationProblem.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9409 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/DnaOptimizationProblem.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      500 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/NoSolutionError.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      284 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.182295 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    15803 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/ConstraintsSolverMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8618 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/ObjectivesMaximizerMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7154 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/RecordRepresentationMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      296 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6404 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Location.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.182295 dnachisel-3.2.9/dnachisel/MutationSpace/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5118 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/MutationSpace/MutationChoice.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10656 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/MutationSpace/MutationSpace.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      131 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/MutationSpace/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.186295 dnachisel-3.2.9/dnachisel/SequencePattern/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1781 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/DnaNotationPattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      932 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/EnzymeSitePattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      828 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/HomopolymerPattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7781 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/MotifPssmPattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1112 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/RepeatedKmerPattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5808 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/SequencePattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      613 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/SequencePattern/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.186295 dnachisel-3.2.9/dnachisel/Specification/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6223 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/FeatureRepresentationMixin.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.190295 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1727 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/ProblemConstraintsEvaluations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1152 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/ProblemObjectivesEvaluations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5448 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/SpecEvaluation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6625 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/SpecEvaluations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      364 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8923 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/Specification.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      567 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/SpecificationSet.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      130 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/Specification/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3075 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.198294 dnachisel-3.2.9/dnachisel/biotools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2208 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1976 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/biotables.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2970 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/blast_sequence.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2537 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/bowtie.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.198294 dnachisel-3.2.9/dnachisel/biotools/data/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      470 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/data/README.md
+-rw-rw-r--   0 peter     (1000) peter     (1000)       68 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/data/complements.csv
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/data/iupac_notation.csv
+-rw-rw-r--   0 peter     (1000) peter     (1000)      132 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/data/nucleotide_to_regexpr.csv
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1491 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/enzymes_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1378 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/formatting_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1211 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/gc_content.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7189 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/genbank_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3114 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/indices_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2028 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/random_sequences.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1280 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/sequences_differences.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3810 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/biotools/sequences_operations.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.202294 dnachisel-3.2.9/dnachisel/builtin_specifications/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3070 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AllowPrimer.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4665 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidBlastMatches.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6509 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidChanges.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3320 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidHairpins.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2596 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidHeterodimerization.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4860 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidMatches.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4006 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidPattern.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1970 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidStopCodons.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2342 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/CodonSpecification.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11935 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceChanges.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3293 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceChoice.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7026 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceGCContent.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2560 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceMeltingTemperature.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7989 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforcePatternOccurence.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2515 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceRegionsCompatibility.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4627 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceSequence.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1108 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceTerminalGCContent.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8936 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceTranslation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/SequenceLengthBounds.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2176 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/TerminalSpecification.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11007 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/UniquifyAllKmers.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2693 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.206294 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4895 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/AvoidRareCodons.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3377 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/BaseCodonOptimizationClass.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4405 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/CodonOptimize.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6606 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/HarmonizeRCA.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8080 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/MatchTargetCodonUsage.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5353 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/MaximizeCAI.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      346 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.210294 dnachisel-3.2.9/dnachisel/reports/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1835 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/SpecAnnotationsTranslator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      315 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.210294 dnachisel-3.2.9/dnachisel/reports/assets/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    20513 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/assets/logo.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2726 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/assets/optimization_report.pug
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/assets/style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)      826 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/colors_cycle.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.210294 dnachisel-3.2.9/dnachisel/reports/constraints_reports/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1077 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/constraints_reports/GraphicTranslator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      427 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/constraints_reports/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3025 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/constraints_reports/constraints_breaches_dataframe.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5119 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/constraints_reports/constraints_reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14144 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/optimization_reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      377 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/reports/tools.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.214294 dnachisel-3.2.9/dnachisel/utils/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      178 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/utils/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1250 2022-01-21 13:20:47.000000 dnachisel-3.2.9/dnachisel/utils/utils.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2022-05-05 16:31:46.000000 dnachisel-3.2.9/dnachisel/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.174295 dnachisel-3.2.9/dnachisel.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3371 2022-05-05 16:31:57.000000 dnachisel-3.2.9/dnachisel.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7736 2022-05-05 16:31:58.000000 dnachisel-3.2.9/dnachisel.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-05-05 16:31:57.000000 dnachisel-3.2.9/dnachisel.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      134 2022-05-05 16:31:57.000000 dnachisel-3.2.9/dnachisel.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       10 2022-05-05 16:31:57.000000 dnachisel-3.2.9/dnachisel.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.222294 dnachisel-3.2.9/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        7 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/.gitignore
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6878 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/Makefile
+-rw-rw-r--   0 peter     (1000) peter     (1000)      211 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.170295 dnachisel-3.2.9/docs/_static/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.222294 dnachisel-3.2.9/docs/_static/css/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1478 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/css/custom.css
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.234294 dnachisel-3.2.9/docs/_static/images/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3121 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/confectionary.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)   896059 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/dnachisel_algorithm.gif
+-rw-rw-r--   0 peter     (1000) peter     (1000)    93263 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/example_sequence.png
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.250294 dnachisel-3.2.9/docs/_static/images/genbank_annotations/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      124 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/README.md
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9955 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/all_unique_kmers.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10654 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/all_unique_kmers_here.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9408 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/allow_primer.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    25370 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_blast.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9934 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_matches.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12612 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_matches_mismatches.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    22054 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_non_unique_segments.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6975 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_cg.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6190 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_cg_obj.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11048 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_enzyme.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7807 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_kmer.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9306 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_noisoleucine.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8402 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_regex.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9026 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/boosting.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5678 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/cds.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14900 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/cds_enforce.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6309 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/change.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6237 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/change_objective.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8032 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/choice.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9137 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/codon_optimize.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7297 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12703 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting_and_kmers.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5682 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting_obj.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10389 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_sequence.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2421 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/examples.csv
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7645 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/gc_range.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8337 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/gc_target.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1903 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/generate_annotations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10180 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/harmonize_rca.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9056 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/insert.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9706 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/insert_several.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5921 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/keep.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4773 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/keep_obj.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8238 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/match_codon_usage.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    13430 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/multiple_specs.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12056 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/myspec.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8450 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/genbank_annotations/use_best_codon.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2138 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/geometry2.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    16412 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/html_logo.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8498 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/old_html_logo.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      600 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/pw_maze_black (copy).png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      600 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/pw_maze_black.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1299 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/pw_maze_dark.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      600 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/pw_maze_white.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    87760 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/report_screenshot.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)    16412 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/_static/images/title.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      114 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/build_and_deploy.sh
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10829 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/conf.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1399 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/examples.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1551 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/favicon.png
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.250294 dnachisel-3.2.9/docs/genbank/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11554 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/genbank/genbank_api.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2209 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/genbank/genbank_notes.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1340 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/index.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6707 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/make.bat
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       51 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/makehtml.sh
+-rw-rw-r--   0 peter     (1000) peter     (1000)      466 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/notes.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.254294 dnachisel-3.2.9/docs/ref/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       65 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/biotools.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1960 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/builtin_specifications.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)      574 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/cli.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)      108 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/constraints_reports.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2316 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/core_classes.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)       85 2022-01-21 13:20:47.000000 dnachisel-3.2.9/docs/ref/reports.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8512 2022-01-21 13:20:47.000000 dnachisel-3.2.9/ez_setup.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3029 2022-01-21 13:20:47.000000 dnachisel-3.2.9/pypi-readme.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 16:31:58.254294 dnachisel-3.2.9/scripts/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     2677 2022-01-21 13:20:47.000000 dnachisel-3.2.9/scripts/dnachisel
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-05-05 16:31:58.254294 dnachisel-3.2.9/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1510 2022-01-21 13:20:47.000000 dnachisel-3.2.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dnachisel-3.2.8/ez_setup.py` & `dnachisel-3.2.9/ez_setup.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/LICENCE.txt` & `dnachisel-3.2.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/setup.py` & `dnachisel-3.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/MutationSpace/MutationChoice.py` & `dnachisel-3.2.9/dnachisel/MutationSpace/MutationChoice.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/MutationSpace/MutationSpace.py` & `dnachisel-3.2.9/dnachisel/MutationSpace/MutationSpace.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceRegionsCompatibility.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceRegionsCompatibility.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AllowPrimer.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AllowPrimer.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceChanges.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceChanges.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceSequence.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceSequence.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidBlastMatches.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidBlastMatches.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/SequenceLengthBounds.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/SequenceLengthBounds.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforcePatternOccurence.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforcePatternOccurence.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/BaseCodonOptimizationClass.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/BaseCodonOptimizationClass.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/MaximizeCAI.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/MaximizeCAI.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/CodonOptimize.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/CodonOptimize.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/HarmonizeRCA.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/HarmonizeRCA.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/AvoidRareCodons.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/AvoidRareCodons.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/codon_optimization/MatchTargetCodonUsage.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/codon_optimization/MatchTargetCodonUsage.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidMatches.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidMatches.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/TerminalSpecification.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/TerminalSpecification.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidHairpins.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidHairpins.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/UniquifyAllKmers.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/UniquifyAllKmers.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/CodonSpecification.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/CodonSpecification.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/__init__.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidChanges.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidChanges.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceGCContent.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceGCContent.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidStopCodons.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidStopCodons.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidHeterodimerization.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidHeterodimerization.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/AvoidPattern.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/AvoidPattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceMeltingTemperature.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceMeltingTemperature.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceTerminalGCContent.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceTerminalGCContent.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceChoice.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceChoice.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/builtin_specifications/EnforceTranslation.py` & `dnachisel-3.2.9/dnachisel/builtin_specifications/EnforceTranslation.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Location.py` & `dnachisel-3.2.9/dnachisel/Location.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/RecordRepresentationMixin.py` & `dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/RecordRepresentationMixin.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/ObjectivesMaximizerMixin.py` & `dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/ObjectivesMaximizerMixin.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/mixins/ConstraintsSolverMixin.py` & `dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/mixins/ConstraintsSolverMixin.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/DnaOptimizationProblem.py` & `dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/DnaOptimizationProblem.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/DnaOptimizationProblem/CircularDnaOptimizationProblem.py` & `dnachisel-3.2.9/dnachisel/DnaOptimizationProblem/CircularDnaOptimizationProblem.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/sequences_operations.py` & `dnachisel-3.2.9/dnachisel/biotools/sequences_operations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/gc_content.py` & `dnachisel-3.2.9/dnachisel/biotools/gc_content.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/blast_sequence.py` & `dnachisel-3.2.9/dnachisel/biotools/blast_sequence.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/enzymes_operations.py` & `dnachisel-3.2.9/dnachisel/biotools/enzymes_operations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/sequences_differences.py` & `dnachisel-3.2.9/dnachisel/biotools/sequences_differences.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/bowtie.py` & `dnachisel-3.2.9/dnachisel/biotools/bowtie.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/formatting_operations.py` & `dnachisel-3.2.9/dnachisel/biotools/formatting_operations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/indices_operations.py` & `dnachisel-3.2.9/dnachisel/biotools/indices_operations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/random_sequences.py` & `dnachisel-3.2.9/dnachisel/biotools/random_sequences.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/__init__.py` & `dnachisel-3.2.9/dnachisel/biotools/__init__.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/biotables.py` & `dnachisel-3.2.9/dnachisel/biotools/biotables.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/biotools/genbank_operations.py` & `dnachisel-3.2.9/dnachisel/biotools/genbank_operations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/utils/utils.py` & `dnachisel-3.2.9/dnachisel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/__init__.py` & `dnachisel-3.2.9/dnachisel/__init__.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/Specification.py` & `dnachisel-3.2.9/dnachisel/Specification/Specification.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/FeatureRepresentationMixin.py` & `dnachisel-3.2.9/dnachisel/Specification/FeatureRepresentationMixin.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/SpecificationSet.py` & `dnachisel-3.2.9/dnachisel/Specification/SpecificationSet.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/ProblemObjectivesEvaluations.py` & `dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/ProblemObjectivesEvaluations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/SpecEvaluation.py` & `dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/SpecEvaluation.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/ProblemConstraintsEvaluations.py` & `dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/ProblemConstraintsEvaluations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/Specification/SpecEvaluation/SpecEvaluations.py` & `dnachisel-3.2.9/dnachisel/Specification/SpecEvaluation/SpecEvaluations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/MotifPssmPattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/MotifPssmPattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/HomopolymerPattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/HomopolymerPattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/SequencePattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/SequencePattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/__init__.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/__init__.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/DnaNotationPattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/DnaNotationPattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/RepeatedKmerPattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/RepeatedKmerPattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/SequencePattern/EnzymeSitePattern.py` & `dnachisel-3.2.9/dnachisel/SequencePattern/EnzymeSitePattern.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/constraints_reports/GraphicTranslator.py` & `dnachisel-3.2.9/dnachisel/reports/constraints_reports/GraphicTranslator.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/constraints_reports/constraints_reports.py` & `dnachisel-3.2.9/dnachisel/reports/constraints_reports/constraints_reports.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/constraints_reports/constraints_breaches_dataframe.py` & `dnachisel-3.2.9/dnachisel/reports/constraints_reports/constraints_breaches_dataframe.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/optimization_reports.py` & `dnachisel-3.2.9/dnachisel/reports/optimization_reports.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/SpecAnnotationsTranslator.py` & `dnachisel-3.2.9/dnachisel/reports/SpecAnnotationsTranslator.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/colors_cycle.py` & `dnachisel-3.2.9/dnachisel/reports/colors_cycle.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/assets/optimization_report.pug` & `dnachisel-3.2.9/dnachisel/reports/assets/optimization_report.pug`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel/reports/assets/logo.png` & `dnachisel-3.2.9/dnachisel/reports/assets/logo.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/pypi-readme.rst` & `dnachisel-3.2.9/pypi-readme.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/dnachisel.egg-info/PKG-INFO` & `dnachisel-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnachisel
-Version: 3.2.8
+Version: 3.2.9
 Summary: Optimize DNA sequences under constraints.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaChisel
 Author: Zulko
 License: MIT
 Keywords: DNA gene design codon optimization constraints synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnachisel-3.2.8/docs/make.bat` & `dnachisel-3.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/examples.rst` & `dnachisel-3.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/genbank/genbank_api.rst` & `dnachisel-3.2.9/docs/genbank/genbank_api.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/genbank/genbank_notes.rst` & `dnachisel-3.2.9/docs/genbank/genbank_notes.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/css/custom.css` & `dnachisel-3.2.9/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/old_html_logo.png` & `dnachisel-3.2.9/docs/_static/images/old_html_logo.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/pw_maze_dark.png` & `dnachisel-3.2.9/docs/_static/images/pw_maze_dark.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/report_screenshot.png` & `dnachisel-3.2.9/docs/_static/images/report_screenshot.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/example_sequence.png` & `dnachisel-3.2.9/docs/_static/images/example_sequence.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/confectionary.png` & `dnachisel-3.2.9/docs/_static/images/confectionary.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/pw_maze_black.png` & `dnachisel-3.2.9/docs/_static/images/pw_maze_black (copy).png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/pw_maze_black (copy).png` & `dnachisel-3.2.9/docs/_static/images/pw_maze_black.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/dnachisel_algorithm.gif` & `dnachisel-3.2.9/docs/_static/images/dnachisel_algorithm.gif`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/html_logo.png` & `dnachisel-3.2.9/docs/_static/images/html_logo.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/geometry2.png` & `dnachisel-3.2.9/docs/_static/images/geometry2.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_cg_obj.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_cg_obj.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting_obj.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting_obj.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_sequence.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_sequence.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/all_unique_kmers_here.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/all_unique_kmers_here.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting_and_kmers.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting_and_kmers.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/use_best_codon.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/use_best_codon.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/change_objective.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/change_objective.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/cds_enforce.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/cds_enforce.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_regex.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_regex.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/allow_primer.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/allow_primer.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/multiple_specs.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/multiple_specs.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_enzyme.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_enzyme.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/keep_obj.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/keep_obj.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_matches_mismatches.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_matches_mismatches.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_cg.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_cg.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/gc_range.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/gc_range.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_kmer.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_kmer.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/enforce_melting.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/enforce_melting.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/cds.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/cds.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/change.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/change.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/myspec.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/myspec.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/insert_several.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/insert_several.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/keep.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/keep.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/gc_target.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/gc_target.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_pattern_noisoleucine.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_pattern_noisoleucine.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/boosting.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/boosting.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/harmonize_rca.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/harmonize_rca.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/all_unique_kmers.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/all_unique_kmers.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_blast.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_blast.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/generate_annotations.py` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/generate_annotations.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/codon_optimize.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/codon_optimize.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/examples.csv` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/examples.csv`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/insert.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/insert.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_matches.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_matches.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/choice.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/choice.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/avoid_non_unique_segments.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/avoid_non_unique_segments.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/genbank_annotations/match_codon_usage.png` & `dnachisel-3.2.9/docs/_static/images/genbank_annotations/match_codon_usage.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/title.png` & `dnachisel-3.2.9/docs/_static/images/title.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_static/images/pw_maze_white.png` & `dnachisel-3.2.9/docs/_static/images/pw_maze_white.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/favicon.png` & `dnachisel-3.2.9/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/index.rst` & `dnachisel-3.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_build/html/_sources/ref/core_classes.rst.txt` & `dnachisel-3.2.9/docs/ref/core_classes.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_build/html/_sources/ref/builtin_specifications.rst.txt` & `dnachisel-3.2.9/docs/ref/builtin_specifications.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/_build/html/_sources/ref/cli.rst.txt` & `dnachisel-3.2.9/docs/ref/cli.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Command Line Interface
 ----------------------
 
-Installing the DNA Chisel python library automatically installs the
+Installing the DNA Chisel Python package automatically installs the
 ``dnachisel`` command line interface (CLI) accessible from the machine's terminal.
 
 This interface enables to get a problem as an annotated genbank and output
 the optimized sequence either as a single genbank or with a multi-file
 optimization report.
 
 Type ``dnachisel -h`` to display the documentation below, and see the
```

### Comparing `dnachisel-3.2.8/docs/conf.py` & `dnachisel-3.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/docs/Makefile` & `dnachisel-3.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/PKG-INFO` & `dnachisel-3.2.9/dnachisel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnachisel
-Version: 3.2.8
+Version: 3.2.9
 Summary: Optimize DNA sequences under constraints.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaChisel
 Author: Zulko
 License: MIT
 Keywords: DNA gene design codon optimization constraints synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnachisel-3.2.8/README.rst` & `dnachisel-3.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `dnachisel-3.2.8/scripts/dnachisel` & `dnachisel-3.2.9/scripts/dnachisel`

 * *Files identical despite different names*

