# Comparing `tmp/viggofiscal-1.3.8.tar.gz` & `tmp/viggofiscal-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggofiscal-1.3.8.tar", last modified: Tue Apr 18 15:07:13 2023, max compression
+gzip compressed data, was "viggofiscal-1.3.9.tar", last modified: Mon May 15 18:57:38 2023, max compression
```

## Comparing `viggofiscal-1.3.8.tar` & `viggofiscal-1.3.9.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:07:13.990146 viggofiscal-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.978146 viggofiscal-1.3.8/viggofiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.978146 viggofiscal-1.3.8/viggofiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.978146 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.982146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstipi/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/domain_org/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/origem/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/origem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/origem/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/uficms/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/uficms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.986146 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/unidade_medida/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 15:06:17.000000 viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:07:13.978146 viggofiscal-1.3.8/viggofiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 15:07:13.000000 viggofiscal-1.3.8/viggofiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-18 15:07:13.000000 viggofiscal-1.3.8/viggofiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:07:13.000000 viggofiscal-1.3.8/viggofiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:07:13.000000 viggofiscal-1.3.8/viggofiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 15:07:13.000000 viggofiscal-1.3.8/viggofiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.323838 viggofiscal-1.3.9/viggofiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.323838 viggofiscal-1.3.9/viggofiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.323838 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.327839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/domain_org/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.331838 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/origem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/origem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/origem/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.335839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/uficms/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/uficms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.339839 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/unidade_medida/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-15 18:56:30.000000 viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:38.323838 viggofiscal-1.3.9/viggofiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 18:57:38.000000 viggofiscal-1.3.9/viggofiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-15 18:57:38.000000 viggofiscal-1.3.9/viggofiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:57:38.000000 viggofiscal-1.3.9/viggofiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 18:57:38.000000 viggofiscal-1.3.9/viggofiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 18:57:38.000000 viggofiscal-1.3.9/viggofiscal.egg-info/top_level.txt
```

### Comparing `viggofiscal-1.3.8/viggofiscal/__init__.py` & `viggofiscal-1.3.9/viggofiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 
 
 class PisCofins01_02():
 
     def __init__(self, valor_produto: float, valor_frete: float,
                  valor_seguro: float, despesas_acessorias: float,
                  valor_desconto: float, aliquota_pis: float,
-                 aliquota_icms: float):
+                 valor_icms: float = 0):
         self.valor_produto = float(valor_produto)
         self.valor_frete = float(valor_frete)
         self.valor_seguro = float(valor_seguro)
         self.despesas_acessorias = float(despesas_acessorias)
         self.valor_desconto = float(valor_desconto)
         self.aliquota_pis = float(aliquota_pis)
-        self.aliquota_icms = float(aliquota_icms)
+        self.valor_icms = float(valor_icms)
 
     def base_pis_normal(self):
         base_pis = BasePis(
             self.valor_produto, self.valor_frete, self.valor_seguro,
             self.despesas_acessorias, self.valor_desconto, 0.0)
         return round_abnt(base_pis.calcular_base_pis(), 2)
 
-    def valor_icms(self):
-        valor_icms = (self.base_pis_normal() * (self.aliquota_icms / 100))
-        return round_abnt(valor_icms, 2)
+    # def valor_icms(self):
+    #     valor_icms = (self.base_pis_normal() * (self.aliquota_icms / 100))
+    #     return round_abnt(valor_icms, 2)
 
     def base_pis_menos_icms(self):
-        valor_icms = self.valor_icms()
+        # valor_icms = self.valor_icms()
         base_pis = BasePis(
             self.valor_produto, self.valor_frete, self.valor_seguro,
-            self.despesas_acessorias, self.valor_desconto, valor_icms)
+            self.despesas_acessorias, self.valor_desconto, self.valor_icms)
         return round_abnt(base_pis.calcular_base_pis(), 2)
 
     def valor_pis(self):
         valor_pis = (self.base_pis_menos_icms() * (self.aliquota_pis / 100))
         return round_abnt(valor_pis, 2)
```

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/calculo_fiscal/utils.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/calculo_fiscal/utils.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cfop/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cfop/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from enum import Enum, IntEnum
 from sqlalchemy import UniqueConstraint, orm
-import sqlalchemy
 
 from viggocore.database import db
 from viggocore.common.subsystem import entity
 
 
 class CodigoSegurancaContribuinte(entity.Entity, db.Model):
```

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/csticms/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/csticms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstipi/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstipi/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/cstpis/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/cstpis/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/domain_org/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,49 @@
-from enum import Enum
-import sqlalchemy
-from sqlalchemy import orm, ForeignKeyConstraint
+from sqlalchemy.sql.schema import UniqueConstraint
 
 from viggocore.database import db
 from viggocore.common.subsystem import entity
 
 
-class Crt(Enum):
-    SIMPLES_NACIONAL = 1
-    SN_EXC_REC_BRUTA = 2
-    REGIME_NORMAL = 3
-    MEI = 4
+class NcmIbptErro(entity.Entity, db.Model):
 
-
-class RegPisCofins(Enum):
-    CUMULATIVO = 1
-    NAO_CUMULATIVO = 2
-
-
-class DomainOrg(entity.Entity, db.Model):
-
-    attributes = ['crt', 'cpf_cnpj', 'insc_est', 'razao_social',
-                  'nome_fantasia', 'insc_mun', 'cnae', 'cpf_cnpj_contador',
-                  'reg_pis_cofins', 'aliq_pis', 'aliq_cofins', 'cred_sn',
-                  'email', 'fone']
+    attributes = ['ncm', 'uf', 'chave', 'versao', 'tipo',
+                  'filename', 'msg_erro', 'erro_em', 'extipi', 'corrigido']
     attributes += entity.Entity.attributes
 
-    domain = orm.relationship(
-        'Domain', backref=orm.backref('domain_org_domain'))
+    ncm = db.Column(db.String(20), nullable=False)
+    uf = db.Column(db.CHAR(2), nullable=False)
+    chave = db.Column(db.String(100), nullable=False)
+    versao = db.Column(db.String(100), nullable=False)
+    tipo = db.Column(db.Numeric(3), nullable=False)
+    filename = db.Column(db.String(2000), nullable=False)
+    msg_erro = db.Column(db.String(2000), nullable=False)
+    erro_em = db.Column(db.DateTime(), nullable=False)
+    extipi = db.Column(db.Numeric(), nullable=True)
+    corrigido = db.Column(db.Boolean(), nullable=False,
+                          default=False, server_default='false')
+
+    __table_args__ = (
+        UniqueConstraint(
+            'ncm', 'uf', 'chave', 'versao', 'extipi', 'tipo',
+            name='ncm_ibpt_erro_ncm_uf_chave_versao_extipi_tipo_uk'),)
 
-    crt = db.Column(sqlalchemy.Enum(Crt), nullable=False)
-    cpf_cnpj = db.Column(db.String(14), nullable=False)
-    insc_est = db.Column(db.String(14), nullable=False)
-    razao_social = db.Column(db.String(100), nullable=False)
-    nome_fantasia = db.Column(db.String(100), nullable=False)
-    insc_mun = db.Column(db.String(15), nullable=True)
-    cnae = db.Column(db.String(15), nullable=True)
-    cpf_cnpj_contador = db.Column(db.String(14), nullable=True)
-    reg_pis_cofins = db.Column(sqlalchemy.Enum(RegPisCofins), nullable=True)
-    aliq_pis = db.Column(db.Numeric(7, 2), nullable=False,
-                         default=0, server_default="0.0")
-    aliq_cofins = db.Column(db.Numeric(7, 2), nullable=False,
-                            default=0, server_default="0.0")
-    cred_sn = db.Column(db.Numeric(7, 2), nullable=False,
-                        default=0, server_default="0.0")
-    email = db.Column(db.String(60), nullable=False)
-    fone = db.Column(db.String(60), nullable=True)
-
-    __table_args__ = (ForeignKeyConstraint(['id'], ['domain.id']),)
-
-    def __init__(self, id, crt, cpf_cnpj, insc_est, razao_social,
-                 nome_fantasia, email, insc_mun=None, cnae=None,
-                 cpf_cnpj_contador=None, reg_pis_cofins=None, aliq_pis=0.0,
-                 aliq_cofins=0.0, cred_sn=0.0, fone=None,
+    def __init__(self, id, ncm, uf, chave, versao, tipo, filename, msg_erro,
+                 erro_em, extipi=None, corrigido=False,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
-        self.crt = crt
-        self.cpf_cnpj = cpf_cnpj
-        self.insc_est = insc_est
-        self.razao_social = razao_social
-        self.nome_fantasia = nome_fantasia
-        self.insc_mun = insc_mun
-        self.cnae = cnae
-        self.cpf_cnpj_contador = cpf_cnpj_contador
-        self.reg_pis_cofins = reg_pis_cofins
-        self.aliq_pis = float(aliq_pis)
-        self.aliq_cofins = float(aliq_cofins)
-        self.cred_sn = float(cred_sn)
-        self.email = email
-        self.fone = fone
+        self.ncm = ncm
+        self.uf = uf
+        self.chave = chave
+        self.versao = versao
+        self.tipo = tipo
+        self.filename = filename
+        self.msg_erro = msg_erro
+        self.erro_em = erro_em
+        self.extipi = extipi
+        self.corrigido = corrigido
 
     @classmethod
     def individual(cls):
-        return 'domain_org'
+        return 'ncm_ibpt_erro'
```

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/origem/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/origem/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/portaria/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/portaria/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/uficms/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/uficms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py` & `viggofiscal-1.3.9/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.3.8/viggofiscal.egg-info/SOURCES.txt` & `viggofiscal-1.3.9/viggofiscal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,18 @@
 viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
 viggofiscal/subsystem/parametrizacao/cstipi/resource.py
 viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
 viggofiscal/subsystem/parametrizacao/cstpis/controller.py
 viggofiscal/subsystem/parametrizacao/cstpis/manager.py
 viggofiscal/subsystem/parametrizacao/cstpis/resource.py
 viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
+viggofiscal/subsystem/parametrizacao/domain_org/controller.py
 viggofiscal/subsystem/parametrizacao/domain_org/manager.py
 viggofiscal/subsystem/parametrizacao/domain_org/resource.py
+viggofiscal/subsystem/parametrizacao/domain_org/router.py
 viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
 viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
 viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
 viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
 viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
 viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
 viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
@@ -88,14 +90,15 @@
 viggofiscal/subsystem/parametrizacao/origem/resource.py
 viggofiscal/subsystem/parametrizacao/portaria/__init__.py
 viggofiscal/subsystem/parametrizacao/portaria/manager.py
 viggofiscal/subsystem/parametrizacao/portaria/resource.py
 viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
 viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
+viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
 viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
 viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
 viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
 viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
 viggofiscal/subsystem/parametrizacao/uficms/__init__.py
 viggofiscal/subsystem/parametrizacao/uficms/resource.py
```

