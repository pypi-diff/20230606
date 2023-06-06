# Comparing `tmp/viggofiscal-1.5.0.tar.gz` & `tmp/viggofiscal-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggofiscal-1.5.0.tar", last modified: Mon Jun  5 18:46:44 2023, max compression
+gzip compressed data, was "viggofiscal-1.5.1.tar", last modified: Tue Jun  6 12:18:18 2023, max compression
```

## Comparing `viggofiscal-1.5.0.tar` & `viggofiscal-1.5.1.tar`

### file list

```diff
@@ -1,148 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.727410 viggofiscal-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 18:46:44.727410 viggofiscal-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-05 18:46:44.727410 viggofiscal-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.707409 viggofiscal-1.5.0/viggofiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.707409 viggofiscal-1.5.0/viggofiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.711409 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.715409 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstipi/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.719410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/natureza_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/origem/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/origem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/origem/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/regra_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.723410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.727410 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/unidade_medida/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 18:45:43.000000 viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:44.707409 viggofiscal-1.5.0/viggofiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 18:46:44.000000 viggofiscal-1.5.0/viggofiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-05 18:46:44.000000 viggofiscal-1.5.0/viggofiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:46:44.000000 viggofiscal-1.5.0/viggofiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 18:46:44.000000 viggofiscal-1.5.0/viggofiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 18:46:44.000000 viggofiscal-1.5.0/viggofiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.786395 viggofiscal-1.5.1/viggofiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.786395 viggofiscal-1.5.1/viggofiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.786395 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.790395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/natureza_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/origem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/origem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/origem/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.794395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/regra_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.798395 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/unidade_medida/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-06 12:17:33.000000 viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:18:18.786395 viggofiscal-1.5.1/viggofiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 12:18:18.000000 viggofiscal-1.5.1/viggofiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-06 12:18:18.000000 viggofiscal-1.5.1/viggofiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:18:18.000000 viggofiscal-1.5.1/viggofiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:18:18.000000 viggofiscal-1.5.1/viggofiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 12:18:18.000000 viggofiscal-1.5.1/viggofiscal.egg-info/top_level.txt
```

### Comparing `viggofiscal-1.5.0/viggofiscal/__init__.py` & `viggofiscal-1.5.1/viggofiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/calculo_fiscal/utils.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/calculo_fiscal/utils.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cfop/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cfop/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/csticms/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/csticms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstipi/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstipi/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/cstpis/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/cstpis/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/domain_org/router.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/domain_org/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/origem/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/origem/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/portaria/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/portaria/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     AD_VALOREM = 'AD_VALOREM'
     ESPECIFICA = 'ESPECIFICA'
 
 
 class RegraFiscalModelo(IntEnum):
     NFE = 55
     NFCE = 65
+    NFE_NFCE = 5565
 
 
 class RegraFiscal(entity.Entity, db.Model):
 
     attributes = ['domain_org_id', 'cstcofins_id', 'csticms_id', 'cstpis_id',
                   'cfop_id', 'cstipi_id', 'descricao', 'aliq_especifica_icms',
                   'aliq_especifica_icms_st', 'aliq_reducao_base_icms',
@@ -116,15 +117,15 @@
         self.modelo = modelo
 
     def is_stable(self):
         # validação se icms_sob_ipi
         if (self.icms_sob_ipi is True and
            (self.tipo_ipi is None and self.cstipi_id is None)):
             raise exception.BadRequest(
-                'Se icms_sob_ipi é verdadeiro então' +
+                'Se icms_sob_ipi é verdadeiro então ' +
                 'tipo_ipi e cstipi_id devem ser informados.')
 
         # TODO(JorgeSilva): verificar como fazer essas validações do tipo de
         # icms pois na criação eu ainda n tenho os backrefs.
         # # validações por tipo de icms
         # if self.csticms.cstcsosn == 20 and self.aliq_reducao_base_icms <= 0:
         #     raise exception.BadRequest('Se o cst_icms for igual a 20 a ' +
```

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/controller.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/terminal/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/terminal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py` & `viggofiscal-1.5.1/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.5.0/viggofiscal.egg-info/SOURCES.txt` & `viggofiscal-1.5.1/viggofiscal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
 viggofiscal/subsystem/parametrizacao/origem/__init__.py
 viggofiscal/subsystem/parametrizacao/origem/resource.py
 viggofiscal/subsystem/parametrizacao/portaria/__init__.py
 viggofiscal/subsystem/parametrizacao/portaria/manager.py
 viggofiscal/subsystem/parametrizacao/portaria/resource.py
 viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
+viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py
 viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
```

