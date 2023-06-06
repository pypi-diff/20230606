# Comparing `tmp/pynguin-0.9.1.tar.gz` & `tmp/pynguin-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynguin-0.9.1.tar", max compression
+gzip compressed data, was "pynguin-0.9.2.tar", max compression
```

## Comparing `pynguin-0.9.1.tar` & `pynguin-0.9.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0     7843 2021-06-17 11:26:01.408051 pynguin-0.9.1/LICENSE.rst
-drwxr-xr-x   0        0        0        0 2021-06-17 11:26:01.408639 pynguin-0.9.1/LICENSES/
--rw-r--r--   0        0        0     5431 2021-06-17 11:26:38.526167 pynguin-0.9.1/README.md
--rw-r--r--   0        0        0      849 2021-06-17 11:26:01.414882 pynguin-0.9.1/pynguin/__init__.py
--rw-r--r--   0        0        0      391 2021-06-17 11:26:01.415042 pynguin-0.9.1/pynguin/__main__.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.415265 pynguin-0.9.1/pynguin/analyses/__init__.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.415464 pynguin-0.9.1/pynguin/analyses/controlflow/__init__.py
--rw-r--r--   0        0        0     7807 2021-06-17 11:26:01.415646 pynguin-0.9.1/pynguin/analyses/controlflow/cfg.py
--rw-r--r--   0        0        0     3241 2021-06-17 11:26:01.415826 pynguin-0.9.1/pynguin/analyses/controlflow/controldependencegraph.py
--rw-r--r--   0        0        0     4650 2021-06-17 11:26:01.416035 pynguin-0.9.1/pynguin/analyses/controlflow/dominatortree.py
--rw-r--r--   0        0        0     8048 2021-06-17 11:26:01.416213 pynguin-0.9.1/pynguin/analyses/controlflow/programgraph.py
--rw-r--r--   0        0        0      143 2021-06-17 11:26:01.416453 pynguin-0.9.1/pynguin/analyses/module/__init__.py
--rw-r--r--   0        0        0     8313 2021-06-17 11:26:01.416756 pynguin-0.9.1/pynguin/analyses/module/inheritance.py
--rw-r--r--   0        0        0    11271 2021-06-17 11:26:01.416955 pynguin-0.9.1/pynguin/analyses/module/typeinformation.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.417222 pynguin-0.9.1/pynguin/analyses/seeding/__init__.py
--rw-r--r--   0        0        0     9717 2021-06-17 11:26:01.417396 pynguin-0.9.1/pynguin/analyses/seeding/constantseeding.py
--rw-r--r--   0        0        0     7297 2021-06-17 11:26:01.417565 pynguin-0.9.1/pynguin/analyses/seeding/initialpopulationseeding.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.417751 pynguin-0.9.1/pynguin/analyses/seeding/testimport/__init__.py
--rw-r--r--   0        0        0    23003 2021-06-17 11:26:01.417994 pynguin-0.9.1/pynguin/analyses/seeding/testimport/ast_to_statement.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.418260 pynguin-0.9.1/pynguin/assertion/__init__.py
--rw-r--r--   0        0        0     2131 2021-06-17 11:26:01.418462 pynguin-0.9.1/pynguin/assertion/assertion.py
--rw-r--r--   0        0        0     4829 2021-06-17 11:26:01.418630 pynguin-0.9.1/pynguin/assertion/assertion_to_ast.py
--rw-r--r--   0        0        0     4107 2021-06-17 11:26:01.418784 pynguin-0.9.1/pynguin/assertion/assertiongenerator.py
--rw-r--r--   0        0        0     1461 2021-06-17 11:26:01.418943 pynguin-0.9.1/pynguin/assertion/assertiontraceobserver.py
--rw-r--r--   0        0        0      660 2021-06-17 11:26:01.419092 pynguin-0.9.1/pynguin/assertion/assertionvisitor.py
--rw-r--r--   0        0        0      709 2021-06-17 11:26:01.419224 pynguin-0.9.1/pynguin/assertion/noneassertion.py
--rw-r--r--   0        0        0     3442 2021-06-17 11:26:01.419393 pynguin-0.9.1/pynguin/assertion/noneassertionobserver.py
--rw-r--r--   0        0        0     1353 2021-06-17 11:26:01.419550 pynguin-0.9.1/pynguin/assertion/nonetraceentry.py
--rw-r--r--   0        0        0     2585 2021-06-17 11:26:01.419843 pynguin-0.9.1/pynguin/assertion/outputtrace.py
--rw-r--r--   0        0        0      613 2021-06-17 11:26:01.420040 pynguin-0.9.1/pynguin/assertion/outputtraceentry.py
--rw-r--r--   0        0        0      736 2021-06-17 11:26:01.420179 pynguin-0.9.1/pynguin/assertion/primitiveassertion.py
--rw-r--r--   0        0        0     3630 2021-06-17 11:26:01.420305 pynguin-0.9.1/pynguin/assertion/primitiveassertionobserver.py
--rw-r--r--   0        0        0     1205 2021-06-17 11:26:01.420459 pynguin-0.9.1/pynguin/assertion/primitivetraceentry.py
--rw-r--r--   0        0        0     4796 2021-06-17 11:26:01.420635 pynguin-0.9.1/pynguin/cli.py
--rw-r--r--   0        0        0    15819 2021-06-17 11:26:01.420847 pynguin-0.9.1/pynguin/configuration.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.421040 pynguin-0.9.1/pynguin/coverage/__init__.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.421233 pynguin-0.9.1/pynguin/coverage/branch/__init__.py
--rw-r--r--   0        0        0     2147 2021-06-17 11:26:01.421398 pynguin-0.9.1/pynguin/coverage/branch/branchcoveragefactory.py
--rw-r--r--   0        0        0     3869 2021-06-17 11:26:01.421573 pynguin-0.9.1/pynguin/coverage/branch/branchcoveragegoal.py
--rw-r--r--   0        0        0     2248 2021-06-17 11:26:01.421732 pynguin-0.9.1/pynguin/coverage/branch/branchcoveragetestfitness.py
--rw-r--r--   0        0        0     7616 2021-06-17 11:26:01.421991 pynguin-0.9.1/pynguin/coverage/controlflowdistance.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.422195 pynguin-0.9.1/pynguin/ga/__init__.py
--rw-r--r--   0        0        0     8205 2021-06-17 11:26:01.422371 pynguin-0.9.1/pynguin/ga/chromosome.py
--rw-r--r--   0        0        0     2081 2021-06-17 11:26:01.422553 pynguin-0.9.1/pynguin/ga/chromosomeconverter.py
--rw-r--r--   0        0        0      683 2021-06-17 11:26:01.422831 pynguin-0.9.1/pynguin/ga/chromosomefactory.py
--rw-r--r--   0        0        0      696 2021-06-17 11:26:01.423027 pynguin-0.9.1/pynguin/ga/chromosomevisitor.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.423241 pynguin-0.9.1/pynguin/ga/comparators/__init__.py
--rw-r--r--   0        0        0     2408 2021-06-17 11:26:01.423390 pynguin-0.9.1/pynguin/ga/comparators/dominancecomparator.py
--rw-r--r--   0        0        0     1725 2021-06-17 11:26:01.423536 pynguin-0.9.1/pynguin/ga/comparators/preferencesortingcomparator.py
--rw-r--r--   0        0        0     2066 2021-06-17 11:26:01.423695 pynguin-0.9.1/pynguin/ga/fitnessfunction.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.423896 pynguin-0.9.1/pynguin/ga/fitnessfunctions/__init__.py
--rw-r--r--   0        0        0     1198 2021-06-17 11:26:01.424067 pynguin-0.9.1/pynguin/ga/fitnessfunctions/abstracttestcasefitnessfunction.py
--rw-r--r--   0        0        0     1517 2021-06-17 11:26:01.424235 pynguin-0.9.1/pynguin/ga/fitnessfunctions/abstracttestsuitefitnessfunction.py
--rw-r--r--   0        0        0     1297 2021-06-17 11:26:01.424445 pynguin-0.9.1/pynguin/ga/fitnessfunctions/branchdistancetestcasefitness.py
--rw-r--r--   0        0        0     1315 2021-06-17 11:26:01.424606 pynguin-0.9.1/pynguin/ga/fitnessfunctions/branchdistancetestsuitefitness.py
--rw-r--r--   0        0        0     4367 2021-06-17 11:26:01.424833 pynguin-0.9.1/pynguin/ga/fitnessfunctions/fitness_utilities.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.425063 pynguin-0.9.1/pynguin/ga/operators/__init__.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.425272 pynguin-0.9.1/pynguin/ga/operators/crossover/__init__.py
--rw-r--r--   0        0        0      761 2021-06-17 11:26:01.425671 pynguin-0.9.1/pynguin/ga/operators/crossover/crossover.py
--rw-r--r--   0        0        0     1401 2021-06-17 11:26:01.425861 pynguin-0.9.1/pynguin/ga/operators/crossover/singlepointrelativecrossover.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.426122 pynguin-0.9.1/pynguin/ga/operators/ranking/__init__.py
--rw-r--r--   0        0        0     1793 2021-06-17 11:26:01.426291 pynguin-0.9.1/pynguin/ga/operators/ranking/crowdingdistance.py
--rw-r--r--   0        0        0     6425 2021-06-17 11:26:01.426478 pynguin-0.9.1/pynguin/ga/operators/ranking/rankingfunction.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.426670 pynguin-0.9.1/pynguin/ga/operators/selection/__init__.py
--rw-r--r--   0        0        0     1289 2021-06-17 11:26:01.426839 pynguin-0.9.1/pynguin/ga/operators/selection/rankselection.py
--rw-r--r--   0        0        0     1718 2021-06-17 11:26:01.426999 pynguin-0.9.1/pynguin/ga/operators/selection/selection.py
--rw-r--r--   0        0        0     1330 2021-06-17 11:26:01.427175 pynguin-0.9.1/pynguin/ga/operators/selection/tournamentselection.py
--rw-r--r--   0        0        0      959 2021-06-17 11:26:01.427328 pynguin-0.9.1/pynguin/ga/postprocess.py
--rw-r--r--   0        0        0    10420 2021-06-17 11:26:01.427551 pynguin-0.9.1/pynguin/ga/testcasechromosome.py
--rw-r--r--   0        0        0     1301 2021-06-17 11:26:01.427691 pynguin-0.9.1/pynguin/ga/testcasechromosomefactory.py
--rw-r--r--   0        0        0     2644 2021-06-17 11:26:01.427828 pynguin-0.9.1/pynguin/ga/testcasefactory.py
--rw-r--r--   0        0        0     6751 2021-06-17 11:26:01.428038 pynguin-0.9.1/pynguin/ga/testsuitechromosome.py
--rw-r--r--   0        0        0     1691 2021-06-17 11:26:01.428185 pynguin-0.9.1/pynguin/ga/testsuitechromosomefactory.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.428376 pynguin-0.9.1/pynguin/generation/__init__.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.428627 pynguin-0.9.1/pynguin/generation/algorithms/__init__.py
--rw-r--r--   0        0        0     5790 2021-06-17 11:26:01.428850 pynguin-0.9.1/pynguin/generation/algorithms/abstractmosastrategy.py
--rw-r--r--   0        0        0     4288 2021-06-17 11:26:01.429018 pynguin-0.9.1/pynguin/generation/algorithms/archive.py
--rw-r--r--   0        0        0    14380 2021-06-17 11:26:01.429221 pynguin-0.9.1/pynguin/generation/algorithms/dynamosastrategy.py
--rw-r--r--   0        0        0     9960 2021-06-17 11:26:01.429425 pynguin-0.9.1/pynguin/generation/algorithms/mioarchive.py
--rw-r--r--   0        0        0     7035 2021-06-17 11:26:01.429596 pynguin-0.9.1/pynguin/generation/algorithms/mioteststrategy.py
--rw-r--r--   0        0        0     4107 2021-06-17 11:26:01.429737 pynguin-0.9.1/pynguin/generation/algorithms/mosastrategy.py
--rw-r--r--   0        0        0     4034 2021-06-17 11:26:01.429901 pynguin-0.9.1/pynguin/generation/algorithms/randomsearchstrategy.py
--rw-r--r--   0        0        0     7995 2021-06-17 11:26:01.430131 pynguin-0.9.1/pynguin/generation/algorithms/randomteststrategy.py
--rw-r--r--   0        0        0     7039 2021-06-17 11:26:01.430307 pynguin-0.9.1/pynguin/generation/algorithms/testgenerationstrategy.py
--rw-r--r--   0        0        0     5597 2021-06-17 11:26:01.430517 pynguin-0.9.1/pynguin/generation/algorithms/wholesuiteteststrategy.py
--rw-r--r--   0        0        0     1901 2021-06-17 11:26:01.430671 pynguin-0.9.1/pynguin/generation/algorithms/wraptestsuitemixin.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.430866 pynguin-0.9.1/pynguin/generation/export/__init__.py
--rw-r--r--   0        0        0     3929 2021-06-17 11:26:01.431082 pynguin-0.9.1/pynguin/generation/export/abstractexporter.py
--rw-r--r--   0        0        0     1694 2021-06-17 11:26:01.431348 pynguin-0.9.1/pynguin/generation/export/exportprovider.py
--rw-r--r--   0        0        0      600 2021-06-17 11:26:01.431650 pynguin-0.9.1/pynguin/generation/export/noneexporter.py
--rw-r--r--   0        0        0     1083 2021-06-17 11:26:01.431945 pynguin-0.9.1/pynguin/generation/export/pytestexporter.py
--rw-r--r--   0        0        0    10420 2021-06-17 11:26:01.432366 pynguin-0.9.1/pynguin/generation/generationalgorithmfactory.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.432726 pynguin-0.9.1/pynguin/generation/stoppingconditions/__init__.py
--rw-r--r--   0        0        0     5330 2021-06-17 11:26:01.432985 pynguin-0.9.1/pynguin/generation/stoppingconditions/stoppingcondition.py
--rw-r--r--   0        0        0    12672 2021-06-17 11:26:01.433296 pynguin-0.9.1/pynguin/generator.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.433672 pynguin-0.9.1/pynguin/instrumentation/__init__.py
--rw-r--r--   0        0        0    32468 2021-06-17 11:26:01.434084 pynguin-0.9.1/pynguin/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     5401 2021-06-17 11:26:01.434391 pynguin-0.9.1/pynguin/instrumentation/machinery.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.434730 pynguin-0.9.1/pynguin/setup/__init__.py
--rw-r--r--   0        0        0     6460 2021-06-17 11:26:01.435003 pynguin-0.9.1/pynguin/setup/testcluster.py
--rw-r--r--   0        0        0     9873 2021-06-17 11:26:01.435284 pynguin-0.9.1/pynguin/setup/testclustergenerator.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.435618 pynguin-0.9.1/pynguin/testcase/__init__.py
--rw-r--r--   0        0        0     4956 2021-06-17 11:26:01.435882 pynguin-0.9.1/pynguin/testcase/defaulttestcase.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.436214 pynguin-0.9.1/pynguin/testcase/execution/__init__.py
--rw-r--r--   0        0        0     4172 2021-06-17 11:26:01.436480 pynguin-0.9.1/pynguin/testcase/execution/executioncontext.py
--rw-r--r--   0        0        0     1654 2021-06-17 11:26:01.436720 pynguin-0.9.1/pynguin/testcase/execution/executionobserver.py
--rw-r--r--   0        0        0     3277 2021-06-17 11:26:01.436962 pynguin-0.9.1/pynguin/testcase/execution/executionresult.py
--rw-r--r--   0        0        0     1598 2021-06-17 11:26:01.437190 pynguin-0.9.1/pynguin/testcase/execution/executiontrace.py
--rw-r--r--   0        0        0    14679 2021-06-17 11:26:01.437490 pynguin-0.9.1/pynguin/testcase/execution/executiontracer.py
--rw-r--r--   0        0        0     5752 2021-06-17 11:26:01.437807 pynguin-0.9.1/pynguin/testcase/execution/testcaseexecutor.py
--rw-r--r--   0        0        0    13515 2021-06-17 11:26:01.438113 pynguin-0.9.1/pynguin/testcase/statement_to_ast.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.438463 pynguin-0.9.1/pynguin/testcase/statements/__init__.py
--rw-r--r--   0        0        0     2252 2021-06-17 11:26:01.438866 pynguin-0.9.1/pynguin/testcase/statements/assignmentstatement.py
--rw-r--r--   0        0        0    12595 2021-06-17 11:26:01.439134 pynguin-0.9.1/pynguin/testcase/statements/collectionsstatements.py
--rw-r--r--   0        0        0     3149 2021-06-17 11:26:01.439413 pynguin-0.9.1/pynguin/testcase/statements/fieldstatement.py
--rw-r--r--   0        0        0    14666 2021-06-17 11:26:01.439675 pynguin-0.9.1/pynguin/testcase/statements/parametrizedstatements.py
--rw-r--r--   0        0        0    14537 2021-06-17 11:26:01.439973 pynguin-0.9.1/pynguin/testcase/statements/primitivestatements.py
--rw-r--r--   0        0        0     5116 2021-06-17 11:26:01.440276 pynguin-0.9.1/pynguin/testcase/statements/statement.py
--rw-r--r--   0        0        0     2948 2021-06-17 11:26:01.440509 pynguin-0.9.1/pynguin/testcase/statements/statementvisitor.py
--rw-r--r--   0        0        0     8299 2021-06-17 11:26:01.440827 pynguin-0.9.1/pynguin/testcase/testcase.py
--rw-r--r--   0        0        0     2780 2021-06-17 11:26:01.441096 pynguin-0.9.1/pynguin/testcase/testcase_to_ast.py
--rw-r--r--   0        0        0      520 2021-06-17 11:26:01.441487 pynguin-0.9.1/pynguin/testcase/testcasevisitor.py
--rw-r--r--   0        0        0    47768 2021-06-17 11:26:01.442041 pynguin-0.9.1/pynguin/testcase/testfactory.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.442461 pynguin-0.9.1/pynguin/testcase/variable/__init__.py
--rw-r--r--   0        0        0     5246 2021-06-17 11:26:01.442840 pynguin-0.9.1/pynguin/testcase/variable/variablereference.py
--rw-r--r--   0        0        0      928 2021-06-17 11:26:01.443096 pynguin-0.9.1/pynguin/testcase/variable/variablereferenceimpl.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.443658 pynguin-0.9.1/pynguin/typeinference/__init__.py
--rw-r--r--   0        0        0     1002 2021-06-17 11:26:01.443968 pynguin-0.9.1/pynguin/typeinference/nonstrategy.py
--rw-r--r--   0        0        0     3983 2021-06-17 11:26:01.444266 pynguin-0.9.1/pynguin/typeinference/strategy.py
--rw-r--r--   0        0        0     6819 2021-06-17 11:26:01.444574 pynguin-0.9.1/pynguin/typeinference/stubstrategy.py
--rw-r--r--   0        0        0     1669 2021-06-17 11:26:01.444841 pynguin-0.9.1/pynguin/typeinference/typehintsstrategy.py
--rw-r--r--   0        0        0     2926 2021-06-17 11:26:01.445202 pynguin-0.9.1/pynguin/typeinference/typeinference.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.445478 pynguin-0.9.1/pynguin/utils/__init__.py
--rw-r--r--   0        0        0      771 2021-06-17 11:26:01.445668 pynguin-0.9.1/pynguin/utils/ast_util.py
--rw-r--r--   0        0        0     1634 2021-06-17 11:26:01.445834 pynguin-0.9.1/pynguin/utils/atomicinteger.py
--rw-r--r--   0        0        0      254 2021-06-17 11:26:01.445976 pynguin-0.9.1/pynguin/utils/console.py
--rw-r--r--   0        0        0      791 2021-06-17 11:26:01.446205 pynguin-0.9.1/pynguin/utils/exceptions.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.446533 pynguin-0.9.1/pynguin/utils/generic/__init__.py
--rw-r--r--   0        0        0     7814 2021-06-17 11:26:01.446765 pynguin-0.9.1/pynguin/utils/generic/genericaccessibleobject.py
--rw-r--r--   0        0        0     1350 2021-06-17 11:26:01.446960 pynguin-0.9.1/pynguin/utils/namingscope.py
--rw-r--r--   0        0        0     4600 2021-06-17 11:26:01.447136 pynguin-0.9.1/pynguin/utils/randomness.py
--rw-r--r--   0        0        0      145 2021-06-17 11:26:01.447348 pynguin-0.9.1/pynguin/utils/statistics/__init__.py
--rw-r--r--   0        0        0     7123 2021-06-17 11:26:01.447569 pynguin-0.9.1/pynguin/utils/statistics/outputvariablefactory.py
--rw-r--r--   0        0        0     3834 2021-06-17 11:26:01.447748 pynguin-0.9.1/pynguin/utils/statistics/runtimevariable.py
--rw-r--r--   0        0        0    16971 2021-06-17 11:26:01.448139 pynguin-0.9.1/pynguin/utils/statistics/statistics.py
--rw-r--r--   0        0        0     2963 2021-06-17 11:26:01.448501 pynguin-0.9.1/pynguin/utils/statistics/statisticsbackend.py
--rw-r--r--   0        0        0     2288 2021-06-17 11:26:01.448822 pynguin-0.9.1/pynguin/utils/statistics/timer.py
--rw-r--r--   0        0        0     4378 2021-06-17 11:26:01.449267 pynguin-0.9.1/pynguin/utils/statistics/timers.py
--rw-r--r--   0        0        0     6742 2021-06-17 11:26:01.449588 pynguin-0.9.1/pynguin/utils/type_utils.py
--rw-r--r--   0        0        0     3474 2021-06-17 11:26:01.449905 pynguin-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     7349 2021-06-17 11:29:21.725829 pynguin-0.9.1/setup.py
--rw-r--r--   0        0        0     7069 2021-06-17 11:29:21.726325 pynguin-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     7843 2021-06-17 11:26:01.408051 pynguin-0.9.2/LICENSE.rst
+drwxr-xr-x   0        0        0        0 2021-06-17 11:26:01.408639 pynguin-0.9.2/LICENSES/
+-rw-r--r--   0        0        0     5552 2021-06-21 11:38:12.188243 pynguin-0.9.2/README.md
+-rw-r--r--   0        0        0      849 2021-06-17 11:29:58.590061 pynguin-0.9.2/pynguin/__init__.py
+-rw-r--r--   0        0        0      391 2021-06-17 11:26:01.415042 pynguin-0.9.2/pynguin/__main__.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.415265 pynguin-0.9.2/pynguin/analyses/__init__.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.415464 pynguin-0.9.2/pynguin/analyses/controlflow/__init__.py
+-rw-r--r--   0        0        0     7807 2021-06-17 11:26:01.415646 pynguin-0.9.2/pynguin/analyses/controlflow/cfg.py
+-rw-r--r--   0        0        0     3241 2021-06-17 11:26:01.415826 pynguin-0.9.2/pynguin/analyses/controlflow/controldependencegraph.py
+-rw-r--r--   0        0        0     4650 2021-06-17 11:26:01.416035 pynguin-0.9.2/pynguin/analyses/controlflow/dominatortree.py
+-rw-r--r--   0        0        0     8048 2021-06-17 11:26:01.416213 pynguin-0.9.2/pynguin/analyses/controlflow/programgraph.py
+-rw-r--r--   0        0        0      143 2021-06-17 11:26:01.416453 pynguin-0.9.2/pynguin/analyses/module/__init__.py
+-rw-r--r--   0        0        0     8313 2021-06-17 11:26:01.416756 pynguin-0.9.2/pynguin/analyses/module/inheritance.py
+-rw-r--r--   0        0        0    11271 2021-06-17 11:26:01.416955 pynguin-0.9.2/pynguin/analyses/module/typeinformation.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.417222 pynguin-0.9.2/pynguin/analyses/seeding/__init__.py
+-rw-r--r--   0        0        0     9717 2021-06-17 11:26:01.417396 pynguin-0.9.2/pynguin/analyses/seeding/constantseeding.py
+-rw-r--r--   0        0        0     7297 2021-06-17 11:26:01.417565 pynguin-0.9.2/pynguin/analyses/seeding/initialpopulationseeding.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.417751 pynguin-0.9.2/pynguin/analyses/seeding/testimport/__init__.py
+-rw-r--r--   0        0        0    23003 2021-06-17 11:26:01.417994 pynguin-0.9.2/pynguin/analyses/seeding/testimport/ast_to_statement.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.418260 pynguin-0.9.2/pynguin/assertion/__init__.py
+-rw-r--r--   0        0        0     2131 2021-06-17 11:26:01.418462 pynguin-0.9.2/pynguin/assertion/assertion.py
+-rw-r--r--   0        0        0     4829 2021-06-17 11:26:01.418630 pynguin-0.9.2/pynguin/assertion/assertion_to_ast.py
+-rw-r--r--   0        0        0     4107 2021-06-17 11:26:01.418784 pynguin-0.9.2/pynguin/assertion/assertiongenerator.py
+-rw-r--r--   0        0        0     1461 2021-06-17 11:26:01.418943 pynguin-0.9.2/pynguin/assertion/assertiontraceobserver.py
+-rw-r--r--   0        0        0      660 2021-06-17 11:26:01.419092 pynguin-0.9.2/pynguin/assertion/assertionvisitor.py
+-rw-r--r--   0        0        0      709 2021-06-17 11:26:01.419224 pynguin-0.9.2/pynguin/assertion/noneassertion.py
+-rw-r--r--   0        0        0     3442 2021-06-17 11:26:01.419393 pynguin-0.9.2/pynguin/assertion/noneassertionobserver.py
+-rw-r--r--   0        0        0     1353 2021-06-17 11:26:01.419550 pynguin-0.9.2/pynguin/assertion/nonetraceentry.py
+-rw-r--r--   0        0        0     2585 2021-06-17 11:26:01.419843 pynguin-0.9.2/pynguin/assertion/outputtrace.py
+-rw-r--r--   0        0        0      613 2021-06-17 11:26:01.420040 pynguin-0.9.2/pynguin/assertion/outputtraceentry.py
+-rw-r--r--   0        0        0      736 2021-06-17 11:26:01.420179 pynguin-0.9.2/pynguin/assertion/primitiveassertion.py
+-rw-r--r--   0        0        0     3630 2021-06-17 11:26:01.420305 pynguin-0.9.2/pynguin/assertion/primitiveassertionobserver.py
+-rw-r--r--   0        0        0     1205 2021-06-17 11:26:01.420459 pynguin-0.9.2/pynguin/assertion/primitivetraceentry.py
+-rw-r--r--   0        0        0     5251 2021-06-21 11:38:12.189874 pynguin-0.9.2/pynguin/cli.py
+-rw-r--r--   0        0        0    15819 2021-06-17 11:26:01.420847 pynguin-0.9.2/pynguin/configuration.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.421040 pynguin-0.9.2/pynguin/coverage/__init__.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.421233 pynguin-0.9.2/pynguin/coverage/branch/__init__.py
+-rw-r--r--   0        0        0     2147 2021-06-17 11:26:01.421398 pynguin-0.9.2/pynguin/coverage/branch/branchcoveragefactory.py
+-rw-r--r--   0        0        0     3869 2021-06-17 11:26:01.421573 pynguin-0.9.2/pynguin/coverage/branch/branchcoveragegoal.py
+-rw-r--r--   0        0        0     2248 2021-06-17 11:26:01.421732 pynguin-0.9.2/pynguin/coverage/branch/branchcoveragetestfitness.py
+-rw-r--r--   0        0        0     7616 2021-06-17 11:26:01.421991 pynguin-0.9.2/pynguin/coverage/controlflowdistance.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.422195 pynguin-0.9.2/pynguin/ga/__init__.py
+-rw-r--r--   0        0        0     8205 2021-06-17 11:26:01.422371 pynguin-0.9.2/pynguin/ga/chromosome.py
+-rw-r--r--   0        0        0     2081 2021-06-17 11:26:01.422553 pynguin-0.9.2/pynguin/ga/chromosomeconverter.py
+-rw-r--r--   0        0        0      683 2021-06-17 11:26:01.422831 pynguin-0.9.2/pynguin/ga/chromosomefactory.py
+-rw-r--r--   0        0        0      696 2021-06-17 11:26:01.423027 pynguin-0.9.2/pynguin/ga/chromosomevisitor.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.423241 pynguin-0.9.2/pynguin/ga/comparators/__init__.py
+-rw-r--r--   0        0        0     2408 2021-06-17 11:26:01.423390 pynguin-0.9.2/pynguin/ga/comparators/dominancecomparator.py
+-rw-r--r--   0        0        0     1725 2021-06-17 11:26:01.423536 pynguin-0.9.2/pynguin/ga/comparators/preferencesortingcomparator.py
+-rw-r--r--   0        0        0     2066 2021-06-17 11:26:01.423695 pynguin-0.9.2/pynguin/ga/fitnessfunction.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.423896 pynguin-0.9.2/pynguin/ga/fitnessfunctions/__init__.py
+-rw-r--r--   0        0        0     1198 2021-06-17 11:26:01.424067 pynguin-0.9.2/pynguin/ga/fitnessfunctions/abstracttestcasefitnessfunction.py
+-rw-r--r--   0        0        0     1517 2021-06-17 11:26:01.424235 pynguin-0.9.2/pynguin/ga/fitnessfunctions/abstracttestsuitefitnessfunction.py
+-rw-r--r--   0        0        0     1297 2021-06-17 11:26:01.424445 pynguin-0.9.2/pynguin/ga/fitnessfunctions/branchdistancetestcasefitness.py
+-rw-r--r--   0        0        0     1315 2021-06-17 11:26:01.424606 pynguin-0.9.2/pynguin/ga/fitnessfunctions/branchdistancetestsuitefitness.py
+-rw-r--r--   0        0        0     4367 2021-06-17 11:26:01.424833 pynguin-0.9.2/pynguin/ga/fitnessfunctions/fitness_utilities.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.425063 pynguin-0.9.2/pynguin/ga/operators/__init__.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.425272 pynguin-0.9.2/pynguin/ga/operators/crossover/__init__.py
+-rw-r--r--   0        0        0      761 2021-06-17 11:26:01.425671 pynguin-0.9.2/pynguin/ga/operators/crossover/crossover.py
+-rw-r--r--   0        0        0     1401 2021-06-17 11:26:01.425861 pynguin-0.9.2/pynguin/ga/operators/crossover/singlepointrelativecrossover.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.426122 pynguin-0.9.2/pynguin/ga/operators/ranking/__init__.py
+-rw-r--r--   0        0        0     1793 2021-06-17 11:26:01.426291 pynguin-0.9.2/pynguin/ga/operators/ranking/crowdingdistance.py
+-rw-r--r--   0        0        0     6425 2021-06-17 11:26:01.426478 pynguin-0.9.2/pynguin/ga/operators/ranking/rankingfunction.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.426670 pynguin-0.9.2/pynguin/ga/operators/selection/__init__.py
+-rw-r--r--   0        0        0     1289 2021-06-17 11:26:01.426839 pynguin-0.9.2/pynguin/ga/operators/selection/rankselection.py
+-rw-r--r--   0        0        0     1718 2021-06-17 11:26:01.426999 pynguin-0.9.2/pynguin/ga/operators/selection/selection.py
+-rw-r--r--   0        0        0     1330 2021-06-17 11:26:01.427175 pynguin-0.9.2/pynguin/ga/operators/selection/tournamentselection.py
+-rw-r--r--   0        0        0      959 2021-06-17 11:26:01.427328 pynguin-0.9.2/pynguin/ga/postprocess.py
+-rw-r--r--   0        0        0    10420 2021-06-17 11:26:01.427551 pynguin-0.9.2/pynguin/ga/testcasechromosome.py
+-rw-r--r--   0        0        0     1301 2021-06-17 11:26:01.427691 pynguin-0.9.2/pynguin/ga/testcasechromosomefactory.py
+-rw-r--r--   0        0        0     2644 2021-06-17 11:26:01.427828 pynguin-0.9.2/pynguin/ga/testcasefactory.py
+-rw-r--r--   0        0        0     6751 2021-06-17 11:26:01.428038 pynguin-0.9.2/pynguin/ga/testsuitechromosome.py
+-rw-r--r--   0        0        0     1691 2021-06-17 11:26:01.428185 pynguin-0.9.2/pynguin/ga/testsuitechromosomefactory.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.428376 pynguin-0.9.2/pynguin/generation/__init__.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.428627 pynguin-0.9.2/pynguin/generation/algorithms/__init__.py
+-rw-r--r--   0        0        0     5790 2021-06-17 11:26:01.428850 pynguin-0.9.2/pynguin/generation/algorithms/abstractmosastrategy.py
+-rw-r--r--   0        0        0     4288 2021-06-17 11:26:01.429018 pynguin-0.9.2/pynguin/generation/algorithms/archive.py
+-rw-r--r--   0        0        0    14380 2021-06-17 11:26:01.429221 pynguin-0.9.2/pynguin/generation/algorithms/dynamosastrategy.py
+-rw-r--r--   0        0        0     9960 2021-06-17 11:26:01.429425 pynguin-0.9.2/pynguin/generation/algorithms/mioarchive.py
+-rw-r--r--   0        0        0     7035 2021-06-17 11:26:01.429596 pynguin-0.9.2/pynguin/generation/algorithms/mioteststrategy.py
+-rw-r--r--   0        0        0     4107 2021-06-17 11:26:01.429737 pynguin-0.9.2/pynguin/generation/algorithms/mosastrategy.py
+-rw-r--r--   0        0        0     4034 2021-06-17 11:26:01.429901 pynguin-0.9.2/pynguin/generation/algorithms/randomsearchstrategy.py
+-rw-r--r--   0        0        0     7995 2021-06-17 11:26:01.430131 pynguin-0.9.2/pynguin/generation/algorithms/randomteststrategy.py
+-rw-r--r--   0        0        0     7039 2021-06-17 11:26:01.430307 pynguin-0.9.2/pynguin/generation/algorithms/testgenerationstrategy.py
+-rw-r--r--   0        0        0     5597 2021-06-17 11:26:01.430517 pynguin-0.9.2/pynguin/generation/algorithms/wholesuiteteststrategy.py
+-rw-r--r--   0        0        0     1901 2021-06-17 11:26:01.430671 pynguin-0.9.2/pynguin/generation/algorithms/wraptestsuitemixin.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.430866 pynguin-0.9.2/pynguin/generation/export/__init__.py
+-rw-r--r--   0        0        0     3929 2021-06-17 11:26:01.431082 pynguin-0.9.2/pynguin/generation/export/abstractexporter.py
+-rw-r--r--   0        0        0     1694 2021-06-17 11:26:01.431348 pynguin-0.9.2/pynguin/generation/export/exportprovider.py
+-rw-r--r--   0        0        0      600 2021-06-17 11:26:01.431650 pynguin-0.9.2/pynguin/generation/export/noneexporter.py
+-rw-r--r--   0        0        0     1083 2021-06-17 11:26:01.431945 pynguin-0.9.2/pynguin/generation/export/pytestexporter.py
+-rw-r--r--   0        0        0    10420 2021-06-17 11:26:01.432366 pynguin-0.9.2/pynguin/generation/generationalgorithmfactory.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.432726 pynguin-0.9.2/pynguin/generation/stoppingconditions/__init__.py
+-rw-r--r--   0        0        0     5330 2021-06-17 11:26:01.432985 pynguin-0.9.2/pynguin/generation/stoppingconditions/stoppingcondition.py
+-rw-r--r--   0        0        0    12672 2021-06-17 11:26:01.433296 pynguin-0.9.2/pynguin/generator.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.433672 pynguin-0.9.2/pynguin/instrumentation/__init__.py
+-rw-r--r--   0        0        0    32468 2021-06-17 11:26:01.434084 pynguin-0.9.2/pynguin/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     5401 2021-06-17 11:26:01.434391 pynguin-0.9.2/pynguin/instrumentation/machinery.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.434730 pynguin-0.9.2/pynguin/setup/__init__.py
+-rw-r--r--   0        0        0     6460 2021-06-17 11:26:01.435003 pynguin-0.9.2/pynguin/setup/testcluster.py
+-rw-r--r--   0        0        0     9873 2021-06-17 11:26:01.435284 pynguin-0.9.2/pynguin/setup/testclustergenerator.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.435618 pynguin-0.9.2/pynguin/testcase/__init__.py
+-rw-r--r--   0        0        0     4956 2021-06-17 11:26:01.435882 pynguin-0.9.2/pynguin/testcase/defaulttestcase.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.436214 pynguin-0.9.2/pynguin/testcase/execution/__init__.py
+-rw-r--r--   0        0        0     4172 2021-06-17 11:26:01.436480 pynguin-0.9.2/pynguin/testcase/execution/executioncontext.py
+-rw-r--r--   0        0        0     1654 2021-06-17 11:26:01.436720 pynguin-0.9.2/pynguin/testcase/execution/executionobserver.py
+-rw-r--r--   0        0        0     3277 2021-06-17 11:26:01.436962 pynguin-0.9.2/pynguin/testcase/execution/executionresult.py
+-rw-r--r--   0        0        0     1598 2021-06-17 11:26:01.437190 pynguin-0.9.2/pynguin/testcase/execution/executiontrace.py
+-rw-r--r--   0        0        0    14679 2021-06-17 11:26:01.437490 pynguin-0.9.2/pynguin/testcase/execution/executiontracer.py
+-rw-r--r--   0        0        0     5752 2021-06-17 11:26:01.437807 pynguin-0.9.2/pynguin/testcase/execution/testcaseexecutor.py
+-rw-r--r--   0        0        0    13515 2021-06-17 11:26:01.438113 pynguin-0.9.2/pynguin/testcase/statement_to_ast.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.438463 pynguin-0.9.2/pynguin/testcase/statements/__init__.py
+-rw-r--r--   0        0        0     2252 2021-06-17 11:26:01.438866 pynguin-0.9.2/pynguin/testcase/statements/assignmentstatement.py
+-rw-r--r--   0        0        0    12595 2021-06-17 11:26:01.439134 pynguin-0.9.2/pynguin/testcase/statements/collectionsstatements.py
+-rw-r--r--   0        0        0     3149 2021-06-17 11:26:01.439413 pynguin-0.9.2/pynguin/testcase/statements/fieldstatement.py
+-rw-r--r--   0        0        0    14666 2021-06-17 11:26:01.439675 pynguin-0.9.2/pynguin/testcase/statements/parametrizedstatements.py
+-rw-r--r--   0        0        0    14537 2021-06-17 11:26:01.439973 pynguin-0.9.2/pynguin/testcase/statements/primitivestatements.py
+-rw-r--r--   0        0        0     5116 2021-06-17 11:26:01.440276 pynguin-0.9.2/pynguin/testcase/statements/statement.py
+-rw-r--r--   0        0        0     2948 2021-06-17 11:26:01.440509 pynguin-0.9.2/pynguin/testcase/statements/statementvisitor.py
+-rw-r--r--   0        0        0     8299 2021-06-17 11:26:01.440827 pynguin-0.9.2/pynguin/testcase/testcase.py
+-rw-r--r--   0        0        0     2780 2021-06-17 11:26:01.441096 pynguin-0.9.2/pynguin/testcase/testcase_to_ast.py
+-rw-r--r--   0        0        0      520 2021-06-17 11:26:01.441487 pynguin-0.9.2/pynguin/testcase/testcasevisitor.py
+-rw-r--r--   0        0        0    47768 2021-06-17 11:26:01.442041 pynguin-0.9.2/pynguin/testcase/testfactory.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.442461 pynguin-0.9.2/pynguin/testcase/variable/__init__.py
+-rw-r--r--   0        0        0     5246 2021-06-17 11:26:01.442840 pynguin-0.9.2/pynguin/testcase/variable/variablereference.py
+-rw-r--r--   0        0        0      928 2021-06-17 11:26:01.443096 pynguin-0.9.2/pynguin/testcase/variable/variablereferenceimpl.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.443658 pynguin-0.9.2/pynguin/typeinference/__init__.py
+-rw-r--r--   0        0        0     1002 2021-06-17 11:26:01.443968 pynguin-0.9.2/pynguin/typeinference/nonstrategy.py
+-rw-r--r--   0        0        0     3983 2021-06-17 11:26:01.444266 pynguin-0.9.2/pynguin/typeinference/strategy.py
+-rw-r--r--   0        0        0     6819 2021-06-17 11:26:01.444574 pynguin-0.9.2/pynguin/typeinference/stubstrategy.py
+-rw-r--r--   0        0        0     1669 2021-06-17 11:26:01.444841 pynguin-0.9.2/pynguin/typeinference/typehintsstrategy.py
+-rw-r--r--   0        0        0     2926 2021-06-17 11:26:01.445202 pynguin-0.9.2/pynguin/typeinference/typeinference.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.445478 pynguin-0.9.2/pynguin/utils/__init__.py
+-rw-r--r--   0        0        0      771 2021-06-17 11:26:01.445668 pynguin-0.9.2/pynguin/utils/ast_util.py
+-rw-r--r--   0        0        0     1634 2021-06-17 11:26:01.445834 pynguin-0.9.2/pynguin/utils/atomicinteger.py
+-rw-r--r--   0        0        0      254 2021-06-17 11:26:01.445976 pynguin-0.9.2/pynguin/utils/console.py
+-rw-r--r--   0        0        0      791 2021-06-17 11:26:01.446205 pynguin-0.9.2/pynguin/utils/exceptions.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.446533 pynguin-0.9.2/pynguin/utils/generic/__init__.py
+-rw-r--r--   0        0        0     7814 2021-06-17 11:26:01.446765 pynguin-0.9.2/pynguin/utils/generic/genericaccessibleobject.py
+-rw-r--r--   0        0        0     1350 2021-06-17 11:26:01.446960 pynguin-0.9.2/pynguin/utils/namingscope.py
+-rw-r--r--   0        0        0     4600 2021-06-17 11:26:01.447136 pynguin-0.9.2/pynguin/utils/randomness.py
+-rw-r--r--   0        0        0      145 2021-06-17 11:26:01.447348 pynguin-0.9.2/pynguin/utils/statistics/__init__.py
+-rw-r--r--   0        0        0     7123 2021-06-17 11:26:01.447569 pynguin-0.9.2/pynguin/utils/statistics/outputvariablefactory.py
+-rw-r--r--   0        0        0     3834 2021-06-17 11:26:01.447748 pynguin-0.9.2/pynguin/utils/statistics/runtimevariable.py
+-rw-r--r--   0        0        0    16971 2021-06-17 11:26:01.448139 pynguin-0.9.2/pynguin/utils/statistics/statistics.py
+-rw-r--r--   0        0        0     2963 2021-06-17 11:26:01.448501 pynguin-0.9.2/pynguin/utils/statistics/statisticsbackend.py
+-rw-r--r--   0        0        0     2288 2021-06-17 11:26:01.448822 pynguin-0.9.2/pynguin/utils/statistics/timer.py
+-rw-r--r--   0        0        0     4378 2021-06-17 11:26:01.449267 pynguin-0.9.2/pynguin/utils/statistics/timers.py
+-rw-r--r--   0        0        0     6742 2021-06-17 11:26:01.449588 pynguin-0.9.2/pynguin/utils/type_utils.py
+-rw-r--r--   0        0        0     3474 2021-06-17 11:29:41.658139 pynguin-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7472 2021-06-21 11:44:57.705357 pynguin-0.9.2/setup.py
+-rw-r--r--   0        0        0     7190 2021-06-21 11:44:57.705882 pynguin-0.9.2/PKG-INFO
```

### Comparing `pynguin-0.9.1/LICENSE.rst` & `pynguin-0.9.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/README.md` & `pynguin-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
 Make sure that your version of `pip` is the same as the Python 3.8 interpreted or a
 virtual environment that uses Python 3.8 as its interpreter, as any older version is
 not supported by Pynguin!
 
 ## Using Pynguin
 
+Before you continue, please read the [quick start guide](https://pynguin.readthedocs.io/en/latest/user/quickstart.html)
+
 Pynguin is a command-line application.
 Once you installed it to a virtual environment, you can invoke the tool by typing
 `pynguin` inside this virtual environment.
 Pynguin will then print a list of its command-line parameters.
 
 A minimal full command line to invoke Pynguin could be the following,
 where we assume that a project `foo` is located in `/tmp/foo`,
```

### Comparing `pynguin-0.9.1/pynguin/__init__.py` & `pynguin-0.9.2/pynguin/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Configuration = config.Configuration
 Algorithm = config.Algorithm
 ExportStrategy = config.ExportStrategy
 StatisticsBackend = config.StatisticsBackend
 StoppingCondition = config.StoppingCondition
 TypeInferenceStrategy = config.TypeInferenceStrategy
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __all__ = [
     "set_configuration",
     "run_pynguin",
     "Configuration",
     "__version__",
     "Algorithm",
     "ExportStrategy",
```

### Comparing `pynguin-0.9.1/pynguin/analyses/controlflow/cfg.py` & `pynguin-0.9.2/pynguin/analyses/controlflow/cfg.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/controlflow/controldependencegraph.py` & `pynguin-0.9.2/pynguin/analyses/controlflow/controldependencegraph.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/controlflow/dominatortree.py` & `pynguin-0.9.2/pynguin/analyses/controlflow/dominatortree.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/controlflow/programgraph.py` & `pynguin-0.9.2/pynguin/analyses/controlflow/programgraph.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/module/inheritance.py` & `pynguin-0.9.2/pynguin/analyses/module/inheritance.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/module/typeinformation.py` & `pynguin-0.9.2/pynguin/analyses/module/typeinformation.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/seeding/constantseeding.py` & `pynguin-0.9.2/pynguin/analyses/seeding/constantseeding.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/seeding/initialpopulationseeding.py` & `pynguin-0.9.2/pynguin/analyses/seeding/initialpopulationseeding.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/analyses/seeding/testimport/ast_to_statement.py` & `pynguin-0.9.2/pynguin/analyses/seeding/testimport/ast_to_statement.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/assertion.py` & `pynguin-0.9.2/pynguin/assertion/assertion.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/assertion_to_ast.py` & `pynguin-0.9.2/pynguin/assertion/assertion_to_ast.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/assertiongenerator.py` & `pynguin-0.9.2/pynguin/assertion/assertiongenerator.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/assertiontraceobserver.py` & `pynguin-0.9.2/pynguin/assertion/assertiontraceobserver.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/assertionvisitor.py` & `pynguin-0.9.2/pynguin/assertion/assertionvisitor.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/noneassertion.py` & `pynguin-0.9.2/pynguin/assertion/noneassertion.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/noneassertionobserver.py` & `pynguin-0.9.2/pynguin/assertion/noneassertionobserver.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/nonetraceentry.py` & `pynguin-0.9.2/pynguin/assertion/nonetraceentry.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/outputtrace.py` & `pynguin-0.9.2/pynguin/assertion/outputtrace.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/outputtraceentry.py` & `pynguin-0.9.2/pynguin/assertion/outputtraceentry.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/primitiveassertion.py` & `pynguin-0.9.2/pynguin/assertion/primitiveassertion.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/primitiveassertionobserver.py` & `pynguin-0.9.2/pynguin/assertion/primitiveassertionobserver.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/assertion/primitivetraceentry.py` & `pynguin-0.9.2/pynguin/assertion/primitivetraceentry.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/cli.py` & `pynguin-0.9.2/pynguin/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """Pynguin is an automated unit test generation framework for Python.
 
 This module provides the main entry location for the program execution from the command
 line.
 """
 import argparse
 import logging
+import os
 import sys
 from pathlib import Path
 from typing import List, Optional
 
 import simple_parsing
 from rich.logging import RichHandler
 from rich.traceback import install
@@ -114,14 +115,18 @@
             rich_tracebacks=True, log_time_format="[%X]", console=console
         )
         console_handler.setLevel(level)
         console_handler.setFormatter(logging.Formatter("%(message)s"))
         logger.addHandler(console_handler)
 
 
+_DANGER_ENV = "PYNGUIN_DANGER_AWARE"
+"""People may wipe their disk, so we give them a heads up."""
+
+
 def main(argv: List[str] = None) -> int:
     """Entry point for the CLI of the Pynguin automatic unit test generation framework.
 
     This method behaves like a standard UNIX command-line application, i.e.,
     the return value `0` signals a successful execution.  Any other return value
     signals some errors.  This is, e.g., the case if the framework was not able
     to generate one successfully running test case for the class under test.
@@ -129,14 +134,24 @@
     Args:
         argv: List of command-line arguments
 
     Returns:
         An integer representing the success of the program run.  0 means
         success, all non-zero exit codes indicate errors.
     """
+    if _DANGER_ENV not in os.environ:
+        print(
+            f"""Environment variable '{_DANGER_ENV}' not set.
+Aborting to avoid harming your system.
+Please refer to the documentation
+(https://pynguin.readthedocs.io/en/latest/user/quickstart.html)
+to see why this happens and what you must do to prevent it."""
+        )
+        return -1
+
     install()
     if argv is None:
         argv = sys.argv
     if len(argv) <= 1:
         argv.append("--help")
     argv = _expand_arguments_if_necessary(argv[1:])
```

### Comparing `pynguin-0.9.1/pynguin/configuration.py` & `pynguin-0.9.2/pynguin/configuration.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/coverage/branch/branchcoveragefactory.py` & `pynguin-0.9.2/pynguin/coverage/branch/branchcoveragefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/coverage/branch/branchcoveragegoal.py` & `pynguin-0.9.2/pynguin/coverage/branch/branchcoveragegoal.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/coverage/branch/branchcoveragetestfitness.py` & `pynguin-0.9.2/pynguin/coverage/branch/branchcoveragetestfitness.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/coverage/controlflowdistance.py` & `pynguin-0.9.2/pynguin/coverage/controlflowdistance.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/chromosome.py` & `pynguin-0.9.2/pynguin/ga/chromosome.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/chromosomeconverter.py` & `pynguin-0.9.2/pynguin/ga/chromosomeconverter.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/chromosomefactory.py` & `pynguin-0.9.2/pynguin/ga/chromosomefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/chromosomevisitor.py` & `pynguin-0.9.2/pynguin/ga/chromosomevisitor.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/comparators/dominancecomparator.py` & `pynguin-0.9.2/pynguin/ga/comparators/dominancecomparator.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/comparators/preferencesortingcomparator.py` & `pynguin-0.9.2/pynguin/ga/comparators/preferencesortingcomparator.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunction.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunction.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunctions/abstracttestcasefitnessfunction.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunctions/abstracttestcasefitnessfunction.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunctions/abstracttestsuitefitnessfunction.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunctions/abstracttestsuitefitnessfunction.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunctions/branchdistancetestcasefitness.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunctions/branchdistancetestcasefitness.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunctions/branchdistancetestsuitefitness.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunctions/branchdistancetestsuitefitness.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/fitnessfunctions/fitness_utilities.py` & `pynguin-0.9.2/pynguin/ga/fitnessfunctions/fitness_utilities.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/crossover/crossover.py` & `pynguin-0.9.2/pynguin/ga/operators/crossover/crossover.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/crossover/singlepointrelativecrossover.py` & `pynguin-0.9.2/pynguin/ga/operators/crossover/singlepointrelativecrossover.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/ranking/crowdingdistance.py` & `pynguin-0.9.2/pynguin/ga/operators/ranking/crowdingdistance.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/ranking/rankingfunction.py` & `pynguin-0.9.2/pynguin/ga/operators/ranking/rankingfunction.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/selection/rankselection.py` & `pynguin-0.9.2/pynguin/ga/operators/selection/rankselection.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/selection/selection.py` & `pynguin-0.9.2/pynguin/ga/operators/selection/selection.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/operators/selection/tournamentselection.py` & `pynguin-0.9.2/pynguin/ga/operators/selection/tournamentselection.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/postprocess.py` & `pynguin-0.9.2/pynguin/ga/postprocess.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/testcasechromosome.py` & `pynguin-0.9.2/pynguin/ga/testcasechromosome.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/testcasechromosomefactory.py` & `pynguin-0.9.2/pynguin/ga/testcasechromosomefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/testcasefactory.py` & `pynguin-0.9.2/pynguin/ga/testcasefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/testsuitechromosome.py` & `pynguin-0.9.2/pynguin/ga/testsuitechromosome.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/ga/testsuitechromosomefactory.py` & `pynguin-0.9.2/pynguin/ga/testsuitechromosomefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/abstractmosastrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/abstractmosastrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/archive.py` & `pynguin-0.9.2/pynguin/generation/algorithms/archive.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/dynamosastrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/dynamosastrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/mioarchive.py` & `pynguin-0.9.2/pynguin/generation/algorithms/mioarchive.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/mioteststrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/mioteststrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/mosastrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/mosastrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/randomsearchstrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/randomsearchstrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/randomteststrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/randomteststrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/testgenerationstrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/testgenerationstrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/wholesuiteteststrategy.py` & `pynguin-0.9.2/pynguin/generation/algorithms/wholesuiteteststrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/algorithms/wraptestsuitemixin.py` & `pynguin-0.9.2/pynguin/generation/algorithms/wraptestsuitemixin.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/export/abstractexporter.py` & `pynguin-0.9.2/pynguin/generation/export/abstractexporter.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/export/exportprovider.py` & `pynguin-0.9.2/pynguin/generation/export/exportprovider.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/export/noneexporter.py` & `pynguin-0.9.2/pynguin/generation/export/noneexporter.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/export/pytestexporter.py` & `pynguin-0.9.2/pynguin/generation/export/pytestexporter.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/generationalgorithmfactory.py` & `pynguin-0.9.2/pynguin/generation/generationalgorithmfactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generation/stoppingconditions/stoppingcondition.py` & `pynguin-0.9.2/pynguin/generation/stoppingconditions/stoppingcondition.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/generator.py` & `pynguin-0.9.2/pynguin/generator.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/instrumentation/instrumentation.py` & `pynguin-0.9.2/pynguin/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/instrumentation/machinery.py` & `pynguin-0.9.2/pynguin/instrumentation/machinery.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/setup/testcluster.py` & `pynguin-0.9.2/pynguin/setup/testcluster.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/setup/testclustergenerator.py` & `pynguin-0.9.2/pynguin/setup/testclustergenerator.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/defaulttestcase.py` & `pynguin-0.9.2/pynguin/testcase/defaulttestcase.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/executioncontext.py` & `pynguin-0.9.2/pynguin/testcase/execution/executioncontext.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/executionobserver.py` & `pynguin-0.9.2/pynguin/testcase/execution/executionobserver.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/executionresult.py` & `pynguin-0.9.2/pynguin/testcase/execution/executionresult.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/executiontrace.py` & `pynguin-0.9.2/pynguin/testcase/execution/executiontrace.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/executiontracer.py` & `pynguin-0.9.2/pynguin/testcase/execution/executiontracer.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/execution/testcaseexecutor.py` & `pynguin-0.9.2/pynguin/testcase/execution/testcaseexecutor.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statement_to_ast.py` & `pynguin-0.9.2/pynguin/testcase/statement_to_ast.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/assignmentstatement.py` & `pynguin-0.9.2/pynguin/testcase/statements/assignmentstatement.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/collectionsstatements.py` & `pynguin-0.9.2/pynguin/testcase/statements/collectionsstatements.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/fieldstatement.py` & `pynguin-0.9.2/pynguin/testcase/statements/fieldstatement.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/parametrizedstatements.py` & `pynguin-0.9.2/pynguin/testcase/statements/parametrizedstatements.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/primitivestatements.py` & `pynguin-0.9.2/pynguin/testcase/statements/primitivestatements.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/statement.py` & `pynguin-0.9.2/pynguin/testcase/statements/statement.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/statements/statementvisitor.py` & `pynguin-0.9.2/pynguin/testcase/statements/statementvisitor.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/testcase.py` & `pynguin-0.9.2/pynguin/testcase/testcase.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/testcase_to_ast.py` & `pynguin-0.9.2/pynguin/testcase/testcase_to_ast.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/testcasevisitor.py` & `pynguin-0.9.2/pynguin/testcase/testcasevisitor.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/testfactory.py` & `pynguin-0.9.2/pynguin/testcase/testfactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/variable/variablereference.py` & `pynguin-0.9.2/pynguin/testcase/variable/variablereference.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/testcase/variable/variablereferenceimpl.py` & `pynguin-0.9.2/pynguin/testcase/variable/variablereferenceimpl.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/typeinference/nonstrategy.py` & `pynguin-0.9.2/pynguin/typeinference/nonstrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/typeinference/strategy.py` & `pynguin-0.9.2/pynguin/typeinference/strategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/typeinference/stubstrategy.py` & `pynguin-0.9.2/pynguin/typeinference/stubstrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/typeinference/typehintsstrategy.py` & `pynguin-0.9.2/pynguin/typeinference/typehintsstrategy.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/typeinference/typeinference.py` & `pynguin-0.9.2/pynguin/typeinference/typeinference.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/ast_util.py` & `pynguin-0.9.2/pynguin/utils/ast_util.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/atomicinteger.py` & `pynguin-0.9.2/pynguin/utils/atomicinteger.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/exceptions.py` & `pynguin-0.9.2/pynguin/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/generic/genericaccessibleobject.py` & `pynguin-0.9.2/pynguin/utils/generic/genericaccessibleobject.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/namingscope.py` & `pynguin-0.9.2/pynguin/utils/namingscope.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/randomness.py` & `pynguin-0.9.2/pynguin/utils/randomness.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/outputvariablefactory.py` & `pynguin-0.9.2/pynguin/utils/statistics/outputvariablefactory.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/runtimevariable.py` & `pynguin-0.9.2/pynguin/utils/statistics/runtimevariable.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/statistics.py` & `pynguin-0.9.2/pynguin/utils/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/statisticsbackend.py` & `pynguin-0.9.2/pynguin/utils/statistics/statisticsbackend.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/timer.py` & `pynguin-0.9.2/pynguin/utils/statistics/timer.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/statistics/timers.py` & `pynguin-0.9.2/pynguin/utils/statistics/timers.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pynguin/utils/type_utils.py` & `pynguin-0.9.2/pynguin/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `pynguin-0.9.1/pyproject.toml` & `pynguin-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2019-2021 Pynguin Contributors
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 [tool.poetry]
 name = "pynguin"
-version = "0.9.1"
+version = "0.9.2"
 description = "Pynguin is a tool for automated unit test generation for Python"
 authors = ["Stephan Lukasczyk <stephan@lukasczyk.me>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/se2p/pynguin"
 documentation = "https://pynguin.readthedocs.io"
 keywords = [
```

### Comparing `pynguin-0.9.1/setup.py` & `pynguin-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,17 @@
  'typing_inspect>=0,<1']
 
 entry_points = \
 {'console_scripts': ['pynguin = pynguin.cli:main']}
 
 setup_kwargs = {
     'name': 'pynguin',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Pynguin is a tool for automated unit test generation for Python',
-    'long_description': '<!--\nSPDX-FileCopyrightText: 2019-2021 Pynguin Contributors\n\nSPDX-License-Identifier: CC-BY-4.0\n-->\n\n# Pynguin\n\nPynguin,\nthe\nPYthoN\nGeneral\nUnIt\ntest\ngeNerator,\nis a tool that allows developers to generate unit tests automatically.\n\nTesting software is a tedious task.\nThus, automated generation techniques have been proposed and mature tools exist—for\nstatically typed languages, such as Java.\nThere is, however, no fully-automated tool available that produces unit tests for\ngeneral-purpose programs in a dynamically typed language.\nPynguin is, to the best of our knowledge, the first tool that fills this gap\nand allows the automated generation of unit tests for Python programs.\n\nPynguin is developed at the\n[Chair of Software Engineering II](https://www.fim.uni-passau.de/lehrstuhl-fuer-software-engineering-ii/) \nof the [University of Passau](https://www.uni-passau.de).\n\n<details>\n<summary>Internal Pipeline Status</summary>\n\n[![pipeline status](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/badges/main/pipeline.svg)](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/-/commits/main)\n[![coverage report](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/badges/main/coverage.svg)](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/-/commits/main)  \n\n</details>\n\n[![License LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![PyPI version](https://badge.fury.io/py/pynguin.svg)](https://badge.fury.io/py/pynguin)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pynguin.svg)](https://github.com/se2p/pynguin)\n[![Documentation Status](https://readthedocs.org/projects/pynguin/badge/?version=latest)](https://pynguin.readthedocs.io/en/latest/?badge=latest)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3989840.svg)](https://doi.org/10.5281/zenodo.3989840)\n[![REUSE status](https://api.reuse.software/badge/github.com/se2p/pynguin)](https://api.reuse.software/info/github.com/se2p/pynguin)\n[![Downloads](https://static.pepy.tech/personalized-badge/pynguin?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/pynguin)\n\n\n![Pynguin Logo](https://raw.githubusercontent.com/se2p/pynguin/master/docs/source/_static/pynguin-logo.png "Pynguin Logo")\n\n## Attention\n\nPynguin executes the module under test!\nAs a consequence, depending on what code is in that module,\nrunning Pynguin can cause serious harm to your computer,\nfor example, wipe your entire hard disk!\nWe recommend running Pynguin in an isolated environment;\nfor example, a Docker container, to minimise the risk of damaging\nyour system.\n\n\n## Prerequisites\n\nBefore you begin, ensure you have met the following requirements:\n- You have installed Python 3.8 or 3.9 (we have not yet tested with Python 3.10, there might\n  be some problems due to changed internals regarding the byte-code instrumentation).\n- You have a recent Linux/macOS/Windows machine.\n\nPlease consider reading the [online documentation](https://pynguin.readthedocs.io)\nto start your Pynguin adventure.\n \n## Installing Pynguin\n\nPynguin can be easily installed using the `pip` tool by typing:\n```bash\npip install pynguin\n```\n\nMake sure that your version of `pip` is the same as the Python 3.8 interpreted or a\nvirtual environment that uses Python 3.8 as its interpreter, as any older version is\nnot supported by Pynguin!\n\n## Using Pynguin\n\nPynguin is a command-line application.\nOnce you installed it to a virtual environment, you can invoke the tool by typing\n`pynguin` inside this virtual environment.\nPynguin will then print a list of its command-line parameters.\n\nA minimal full command line to invoke Pynguin could be the following,\nwhere we assume that a project `foo` is located in `/tmp/foo`,\nwe want to store Pynguin\'s generated tests in `/tmp/testgen`,\nand we want to generate tests using a whole-suite approach for the module `foo.bar`\n(wrapped for better readability):\n```bash\npynguin \\\n  --algorithm WHOLE_SUITE \\\n  --project_path /tmp/foo \\\n  --output_path /tmp/testgen \\\n  --module_name foo.bar\n```\n\n## Contributing to Pynguin\n\nFor the development of Pynguin you will need the [`poetry`](https://python-poetry.org)\ndependency management and packaging tool.\nTo start developing, follow these steps:\n1. Clone the repository\n2. Change to the `pynguin` folder: `cd pynguin`\n3. Create a virtual environment and install dependencies using `poetry`: `poetry install`\n4. Make your changes\n5. Run `poetry shell` to switch to the virtual environment in your current shell\n6. Run `make check` to verify that your changes pass all checks\n\n   Please see the [`poetry` documentation](https://python-poetry.org/docs/) for more information on this tool.\n\n### Development using PyCharm.\n\nIf you want to use the PyCharm IDE you have to set up a few things:\n1. Import pynguin into PyCharm.\n2. Find the location of the virtual environment by running `poetry env info` in the project directory.\n3. Go to `Settings` / `Project: pynguin` / `Project interpreter`\n4. Add and use a new interpreter that points to the path of the virtual environment\n5. Set the default test runner to `pytest`\n\n## License\n\nThis project is licensed under the terms of the\n[GNU Lesser General Public License](LICENSE.rst).\n',
+    'long_description': '<!--\nSPDX-FileCopyrightText: 2019-2021 Pynguin Contributors\n\nSPDX-License-Identifier: CC-BY-4.0\n-->\n\n# Pynguin\n\nPynguin,\nthe\nPYthoN\nGeneral\nUnIt\ntest\ngeNerator,\nis a tool that allows developers to generate unit tests automatically.\n\nTesting software is a tedious task.\nThus, automated generation techniques have been proposed and mature tools exist—for\nstatically typed languages, such as Java.\nThere is, however, no fully-automated tool available that produces unit tests for\ngeneral-purpose programs in a dynamically typed language.\nPynguin is, to the best of our knowledge, the first tool that fills this gap\nand allows the automated generation of unit tests for Python programs.\n\nPynguin is developed at the\n[Chair of Software Engineering II](https://www.fim.uni-passau.de/lehrstuhl-fuer-software-engineering-ii/) \nof the [University of Passau](https://www.uni-passau.de).\n\n<details>\n<summary>Internal Pipeline Status</summary>\n\n[![pipeline status](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/badges/main/pipeline.svg)](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/-/commits/main)\n[![coverage report](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/badges/main/coverage.svg)](https://gitlab.infosun.fim.uni-passau.de/se2/pynguin/pynguin/-/commits/main)  \n\n</details>\n\n[![License LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![PyPI version](https://badge.fury.io/py/pynguin.svg)](https://badge.fury.io/py/pynguin)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pynguin.svg)](https://github.com/se2p/pynguin)\n[![Documentation Status](https://readthedocs.org/projects/pynguin/badge/?version=latest)](https://pynguin.readthedocs.io/en/latest/?badge=latest)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3989840.svg)](https://doi.org/10.5281/zenodo.3989840)\n[![REUSE status](https://api.reuse.software/badge/github.com/se2p/pynguin)](https://api.reuse.software/info/github.com/se2p/pynguin)\n[![Downloads](https://static.pepy.tech/personalized-badge/pynguin?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/pynguin)\n\n\n![Pynguin Logo](https://raw.githubusercontent.com/se2p/pynguin/master/docs/source/_static/pynguin-logo.png "Pynguin Logo")\n\n## Attention\n\nPynguin executes the module under test!\nAs a consequence, depending on what code is in that module,\nrunning Pynguin can cause serious harm to your computer,\nfor example, wipe your entire hard disk!\nWe recommend running Pynguin in an isolated environment;\nfor example, a Docker container, to minimise the risk of damaging\nyour system.\n\n\n## Prerequisites\n\nBefore you begin, ensure you have met the following requirements:\n- You have installed Python 3.8 or 3.9 (we have not yet tested with Python 3.10, there might\n  be some problems due to changed internals regarding the byte-code instrumentation).\n- You have a recent Linux/macOS/Windows machine.\n\nPlease consider reading the [online documentation](https://pynguin.readthedocs.io)\nto start your Pynguin adventure.\n \n## Installing Pynguin\n\nPynguin can be easily installed using the `pip` tool by typing:\n```bash\npip install pynguin\n```\n\nMake sure that your version of `pip` is the same as the Python 3.8 interpreted or a\nvirtual environment that uses Python 3.8 as its interpreter, as any older version is\nnot supported by Pynguin!\n\n## Using Pynguin\n\nBefore you continue, please read the [quick start guide](https://pynguin.readthedocs.io/en/latest/user/quickstart.html)\n\nPynguin is a command-line application.\nOnce you installed it to a virtual environment, you can invoke the tool by typing\n`pynguin` inside this virtual environment.\nPynguin will then print a list of its command-line parameters.\n\nA minimal full command line to invoke Pynguin could be the following,\nwhere we assume that a project `foo` is located in `/tmp/foo`,\nwe want to store Pynguin\'s generated tests in `/tmp/testgen`,\nand we want to generate tests using a whole-suite approach for the module `foo.bar`\n(wrapped for better readability):\n```bash\npynguin \\\n  --algorithm WHOLE_SUITE \\\n  --project_path /tmp/foo \\\n  --output_path /tmp/testgen \\\n  --module_name foo.bar\n```\n\n## Contributing to Pynguin\n\nFor the development of Pynguin you will need the [`poetry`](https://python-poetry.org)\ndependency management and packaging tool.\nTo start developing, follow these steps:\n1. Clone the repository\n2. Change to the `pynguin` folder: `cd pynguin`\n3. Create a virtual environment and install dependencies using `poetry`: `poetry install`\n4. Make your changes\n5. Run `poetry shell` to switch to the virtual environment in your current shell\n6. Run `make check` to verify that your changes pass all checks\n\n   Please see the [`poetry` documentation](https://python-poetry.org/docs/) for more information on this tool.\n\n### Development using PyCharm.\n\nIf you want to use the PyCharm IDE you have to set up a few things:\n1. Import pynguin into PyCharm.\n2. Find the location of the virtual environment by running `poetry env info` in the project directory.\n3. Go to `Settings` / `Project: pynguin` / `Project interpreter`\n4. Add and use a new interpreter that points to the path of the virtual environment\n5. Set the default test runner to `pytest`\n\n## License\n\nThis project is licensed under the terms of the\n[GNU Lesser General Public License](LICENSE.rst).\n',
     'author': 'Stephan Lukasczyk',
     'author_email': 'stephan@lukasczyk.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/se2p/pynguin',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pynguin-0.9.1/PKG-INFO` & `pynguin-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynguin
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pynguin is a tool for automated unit test generation for Python
 Home-page: https://github.com/se2p/pynguin
 License: LGPL-3.0-or-later
 Keywords: unit test,random testing,search based,test generation
 Author: Stephan Lukasczyk
 Author-email: stephan@lukasczyk.me
 Requires-Python: >=3.8,<4.0
@@ -116,14 +116,16 @@
 
 Make sure that your version of `pip` is the same as the Python 3.8 interpreted or a
 virtual environment that uses Python 3.8 as its interpreter, as any older version is
 not supported by Pynguin!
 
 ## Using Pynguin
 
+Before you continue, please read the [quick start guide](https://pynguin.readthedocs.io/en/latest/user/quickstart.html)
+
 Pynguin is a command-line application.
 Once you installed it to a virtual environment, you can invoke the tool by typing
 `pynguin` inside this virtual environment.
 Pynguin will then print a list of its command-line parameters.
 
 A minimal full command line to invoke Pynguin could be the following,
 where we assume that a project `foo` is located in `/tmp/foo`,
```

