# Comparing `tmp/multiversx_sdk_cli-6.1.3.tar.gz` & `tmp/multiversx_sdk_cli-6.2.0.tar.gz`

## Comparing `multiversx_sdk_cli-6.1.3.tar` & `multiversx_sdk_cli-6.2.0.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_block.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    19588 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_network.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_testnet.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/diskcache.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_activation.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_checks.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_registry.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_clang.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_cpp.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_sol.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates_repository.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/__init__.py
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/config.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/core.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/genesis.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/genesis_json.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/node_config_toml.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/nodes_setup_json.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0    10661 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/setup.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/wallets.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/README.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/pyproject.toml
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_block.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    20227 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_network.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_testnet.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/diskcache.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_activation.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_checks.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_registry.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_clang.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_cpp.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_sol.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates_config.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates_repository.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/__init__.py
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/config.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/core.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/genesis.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/genesis_json.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/node_config_toml.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0    10661 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/setup.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/wallets.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/README.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.2.0/PKG-INFO
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_block.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_block.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     trigger_contract_verification
 from multiversx_sdk_cli.contracts import CodeMetadata, SmartContract
 from multiversx_sdk_cli.docker import is_docker_installed, run_docker
 from multiversx_sdk_cli.errors import DockerMissingError
 from multiversx_sdk_cli.projects import load_project
 from multiversx_sdk_cli.projects.core import get_project_paths_recursively
 from multiversx_sdk_cli.transactions import Transaction
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 logger = logging.getLogger("cli.contracts")
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "contract", "Build, deploy, upgrade and interact with Smart Contracts")
     subparsers = parser.add_subparsers()
@@ -71,15 +72,15 @@
     output_description = CLIOutputBuilder.describe(with_contract=True, with_transaction_on_network=True, with_simulation=True)
     sub = cli_shared.add_command_subparser(subparsers, "contract", "deploy", f"Deploy a Smart Contract.{output_description}")
     _add_project_or_bytecode_arg(sub)
     _add_metadata_arg(sub)
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
 
@@ -87,15 +88,15 @@
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "call",
                                            f"Interact with a Smart Contract (execute function).{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_function_arg(sub)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub, relay=True)
@@ -106,15 +107,15 @@
                                            f"Upgrade a previously-deployed Smart Contract.{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
     _add_project_or_bytecode_arg(sub)
     _add_metadata_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
 
@@ -290,27 +291,32 @@
     project_paths = get_project_paths(args)
     for project in project_paths:
         projects.run_tests(project, args)
 
 
 def deploy(args: Any):
     logger.debug("deploy")
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
 
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     sender = _prepare_sender(args)
 
-    tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, chain, version)
+    tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+
     logger.info("Contract address: %s", contract.address)
     utils.log_explorer_contract_address(chain, contract.address)
 
     _send_or_simulate(tx, contract, args)
 
 
 def _prepare_contract(args: Any) -> SmartContract:
@@ -362,29 +368,34 @@
         raise errors.NoWalletProvided()
 
     return sender
 
 
 def call(args: Any):
     logger.debug("call")
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
 
     contract_address = args.contract
     function = args.function
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
     chain = args.chain
     version = args.version
 
     contract = SmartContract(contract_address)
     sender = _prepare_sender(args)
 
-    tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, chain, version)
+    tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+
     _send_or_simulate(tx, contract, args)
 
 
 def upgrade(args: Any):
     logger.debug("upgrade")
     cli_shared.check_broadcast_args(args)
 
@@ -396,15 +407,19 @@
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     contract.address = Address(contract_address)
     sender = _prepare_sender(args)
 
-    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version)
+    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian_address, args.options)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+
     _send_or_simulate(tx, contract, args)
 
 
 def query(args: Any):
     logger.debug("query")
 
     contract_address = args.contract
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_delegation.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,20 +127,21 @@
     _add_common_arguments(args, sub)
     sub.set_defaults(func=set_metadata)
 
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
 
 
 def do_create_delegation_contract(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_create_new_staking_contract(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
@@ -156,102 +157,114 @@
         contract_address = transaction_events[0].address
         print(contract_address.bech32())
     else:
         raise errors.ProgrammingError("Tx has more than one event. Make sure it's a staking provider SC Deploy transaction.")
 
 
 def add_new_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_add_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def remove_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_remove_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def stake_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_stake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unbond_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unbond_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unstake_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unstake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unjail_nodes(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unjail_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def change_service_fee(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_change_service_fee(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
+
 def modify_delegation_cap(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_modify_delegation_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def automatic_activation(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_automatic_activation(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def redelegate_cap(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_redelegate_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def set_metadata(args: Any):
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_set_metadata(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, List
 from prettytable import PrettyTable
 
 from multiversx_sdk_cli import cli_shared
 from multiversx_sdk_cli.dns import (name_hash, dns_address_for_name, register, resolve, registration_cost,
-                        validate_name, version, compute_dns_address_for_shard_id)
+                                    validate_name, version, compute_dns_address_for_shard_id)
 from multiversx_sdk_cli.accounts import Address
 from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "dns", "Operations related to the Domain Name Service")
     subparsers = parser.add_subparsers()
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "register", "Send a register transaction to the appropriate DNS contract from given user and with given name")
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_broadcast_args(sub, relay=True)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     sub.add_argument("--name", help="the name to register")
     sub.set_defaults(func=register)
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "resolve", "Find the address for a name")
     _add_name_arg(sub)
     cli_shared.add_proxy_arg(sub)
     sub.set_defaults(func=dns_resolve)
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_network.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_network.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 from multiversx_sdk_cli.simulation import Simulator
 from multiversx_sdk_cli.transactions import Transaction
+from multiversx_sdk_cli.constants import TRANSACTION_OPTIONS_TX_GUARDED
 
 
 def wider_help_formatter(prog: Text):
     return argparse.RawDescriptionHelpFormatter(prog, max_help_position=50, width=120)
 
 
 def add_group_subparser(subparsers: Any, group: str, description: str) -> Any:
@@ -51,15 +52,15 @@
         command,
         usage=f"mxpy {group} {command} [-h] ...",
         description=description,
         formatter_class=wider_help_formatter
     )
 
 
-def add_tx_args(args: List[str], sub: Any, with_nonce: bool = True, with_receiver: bool = True, with_data: bool = True, with_estimate_gas: bool = False):
+def add_tx_args(args: List[str], sub: Any, with_nonce: bool = True, with_receiver: bool = True, with_data: bool = True, with_estimate_gas: bool = False, with_guardian: bool = False):
     if with_nonce:
         sub.add_argument("--nonce", type=int, required=not ("--recall-nonce" in args), help="# the nonce for the transaction")
         sub.add_argument("--recall-nonce", action="store_true", default=False, help="⭮ whether to recall the nonce when creating the transaction (default: %(default)s)")
 
     if with_receiver:
         sub.add_argument("--receiver", required=True, help="🖄 the address of the receiver")
         sub.add_argument("--receiver-username", required=False, help="🖄 the username of the receiver")
@@ -72,14 +73,20 @@
     sub.add_argument("--value", default="0", help="the value to transfer (default: %(default)s)")
 
     if with_data:
         sub.add_argument("--data", default="", help="the payload, or 'memo' of the transaction (default: %(default)s)")
 
     sub.add_argument("--chain", default=config.get_chain_id(), help="the chain identifier (default: %(default)s)")
     sub.add_argument("--version", type=int, default=config.get_tx_version(), help="the transaction version (default: %(default)s)")
+
+    if with_guardian:
+        sub.add_argument("--guardian", type=str, help="the address of the guradian")
+        sub.add_argument("--guardian-service-url", type=str, help="the url of the guardian service")
+        sub.add_argument("--guardian-2fa-code", type=str, help="the 2fa code for the guardian")
+
     sub.add_argument("--options", type=int, default=0, help="the transaction options (default: 0)")
 
 
 def add_wallet_args(args: List[str], sub: Any):
     sub.add_argument("--pem", required=check_if_sign_method_required(args, "--pem"), help="🔑 the PEM file, if keyfile not provided")
     sub.add_argument("--pem-index", default=0, help="🔑 the index in the PEM file (default: %(default)s)")
     sub.add_argument("--keyfile", required=check_if_sign_method_required(args, "--keyfile"), help="🔑 a JSON keyfile, if PEM not provided")
@@ -143,14 +150,23 @@
 def check_broadcast_args(args: Any):
     if hasattr(args, "relay") and args.relay and args.send:
         raise errors.BadUsage("Cannot directly send a relayed transaction. Use 'mxpy tx new --relay' first, then 'mxpy tx send --data-file'")
     if args.send and args.simulate:
         raise errors.BadUsage("Cannot both 'simulate' and 'send' a transaction")
 
 
+def check_guardian_args(args: Any):
+    if any([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
+        if not all([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
+            raise errors.BadUsage("All guardian arguments must be provided")
+
+        if not args.options & TRANSACTION_OPTIONS_TX_GUARDED == TRANSACTION_OPTIONS_TX_GUARDED:
+            raise errors.BadUsage("For guarded transactions the guarded flag must be set.")
+
+
 def send_or_simulate(tx: Transaction, args: Any, dump_output: bool = True) -> CLIOutputBuilder:
     proxy = ProxyNetworkProvider(args.proxy)
 
     is_set_wait_result = hasattr(args, "wait_result") and args.wait_result
     is_set_send = hasattr(args, "send") and args.send
     is_set_simulate = hasattr(args, "simulate") and args.simulate
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_testnet.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_testnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from argparse import FileType
 from pathlib import Path
 from typing import Any, List
 
 from multiversx_sdk_cli import cli_shared, utils
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
 from multiversx_sdk_cli.transactions import Transaction, do_prepare_transaction
@@ -39,21 +38,22 @@
 
     parser.epilog = cli_shared.build_group_epilog(subparsers)
     return subparsers
 
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_wallet_args(args, sub)
-    cli_shared.add_tx_args(args, sub)
+    cli_shared.add_tx_args(args, sub, with_guardian=True)
     sub.add_argument("--data-file", type=str, default=None, help="a file containing transaction data")
 
 
 def create_transaction(args: Any):
     args = utils.as_object(args)
 
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
 
     if args.data_file:
         args.data = Path(args.data_file).read_text()
 
     tx = do_prepare_transaction(args)
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     parser.epilog = cli_shared.build_group_epilog(subparsers)
     return subparsers
 
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
-    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True)
+    cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
 
 
 def _add_nodes_arg(sub: Any):
     sub.add_argument("--nodes-public-keys", required=True, help="the public keys of the nodes as CSV (addrA,addrB)")
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         raise errors.ConfigurationProtectedError(name)
 
 
 def get_defaults() -> Dict[str, Any]:
     return {
         "proxy": "https://testnet-gateway.multiversx.com",
         "chainID": "T",
-        "txVersion": "1",
+        "txVersion": "2",
         "dependencies.vmtools.tag": "latest",
         "dependencies.mx_sdk_rs.tag": "latest",
         "dependencies.vmtools.urlTemplate.linux": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.osx": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.windows": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.llvm.tag": "v9-19feb",
         # ide.elrond.com will be removed, TBD if clang will still be downloaded
@@ -185,15 +185,15 @@
         "dependencies.wasm-opt.tag": "latest",
         "dependencies.twiggy.tag": "latest",
         "dependencies.testwallets.tag": "latest",
         "dependencies.testwallets.urlTemplate.linux": "https://github.com/multiversx/mx-sdk-testwallets/archive/{TAG}.tar.gz",
         "dependencies.testwallets.urlTemplate.osx": "https://github.com/multiversx/mx-sdk-testwallets/archive/{TAG}.tar.gz",
         "dependencies.testwallets.urlTemplate.windows": "https://github.com/multiversx/mx-sdk-testwallets/archive/{TAG}.tar.gz",
         "dependencies.wasm-opt.resolution": "SDK",
-        "dependencies.wasm-opt.tag": "version_105",
+        "dependencies.wasm-opt.tag": "version_112",
         "dependencies.wasm-opt.urlTemplate.linux": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-linux.tar.gz",
         "dependencies.wasm-opt.urlTemplate.osx": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-macos.tar.gz",
         "dependencies.wasm-opt.urlTemplate.windows": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-windows.tar.gz",
         "testnet.validate_expected_keys": "false",
         "github_api_token": "",
     }
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/contract_verification.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 class SmartContract:
     def __init__(self, address: Optional[Address] = None, bytecode=None, metadata=None):
         self.address = Address(address)
         self.bytecode = bytecode
         self.metadata = metadata or CodeMetadata()
 
-    def deploy(self, owner: Account, arguments: List[Any], gas_price: int, gas_limit: int, value: int, chain: str, version: int) -> Transaction:
+    def deploy(self, owner: Account, arguments: List[Any], gas_price: int, gas_limit: int, value: int, chain: str, version: int, guardian: str, options: int) -> Transaction:
         self.owner = owner
         self.compute_address()
 
         arguments = arguments or []
         gas_price = int(gas_price)
         gas_limit = int(gas_limit)
         value = value or 0
@@ -82,14 +82,16 @@
         tx.sender = owner.address.bech32()
         tx.receiver = Address.zero().bech32()
         tx.gasPrice = gas_price
         tx.gasLimit = gas_limit
         tx.data = self.prepare_deploy_transaction_data(arguments)
         tx.chainID = chain
         tx.version = version
+        tx.guardian = guardian
+        tx.options = options
 
         tx.sign(owner)
         return tx
 
     def prepare_deploy_transaction_data(self, arguments: List[Any]):
         tx_data = f"{self.bytecode}@{constants.VM_TYPE_WASM_VM}@{self.metadata.to_hex()}"
 
@@ -105,15 +107,15 @@
         owner_bytes = self.owner.address.pubkey()
         nonce_bytes = self.owner.nonce.to_bytes(8, byteorder="little")
         bytes_to_hash = owner_bytes + nonce_bytes
         address = keccak.new(digest_bits=256).update(bytes_to_hash).digest()
         address = bytes([0] * 8) + bytes([5, 0]) + address[10:30] + owner_bytes[30:]
         self.address = Address(address)
 
-    def execute(self, caller: Account, function: str, arguments: List[str], gas_price: int, gas_limit: int, value: int, chain: str, version: int) -> Transaction:
+    def execute(self, caller: Account, function: str, arguments: List[str], gas_price: int, gas_limit: int, value: int, chain: str, version: int, guardian: str, options: int) -> Transaction:
         self.caller = caller
 
         arguments = arguments or []
         gas_price = int(gas_price)
         gas_limit = int(gas_limit)
         value = value or 0
 
@@ -123,27 +125,29 @@
         tx.sender = caller.address.bech32()
         tx.receiver = self.address.bech32()
         tx.gasPrice = gas_price
         tx.gasLimit = gas_limit
         tx.data = self.prepare_execute_transaction_data(function, arguments)
         tx.chainID = chain
         tx.version = version
+        tx.guardian = guardian
+        tx.options = options
 
         tx.sign(caller)
         return tx
 
     def prepare_execute_transaction_data(self, function: str, arguments: List[Any]):
         tx_data = function
 
         for arg in arguments:
             tx_data += f"@{_prepare_argument(arg)}"
 
         return tx_data
 
-    def upgrade(self, owner: Account, arguments: List[Any], gas_price: int, gas_limit: int, value: int, chain: str, version: int) -> Transaction:
+    def upgrade(self, owner: Account, arguments: List[Any], gas_price: int, gas_limit: int, value: int, chain: str, version: int, guardian: str, options: int) -> Transaction:
         self.owner = owner
 
         arguments = arguments or []
         gas_price = int(gas_price or config.DEFAULT_GAS_PRICE)
         gas_limit = int(gas_limit)
         value = value or 0
 
@@ -153,14 +157,16 @@
         tx.sender = owner.address.bech32()
         tx.receiver = self.address.bech32()
         tx.gasPrice = gas_price
         tx.gasLimit = gas_limit
         tx.data = self.prepare_upgrade_transaction_data(arguments)
         tx.chainID = chain
         tx.version = version
+        tx.guardian = guardian
+        tx.options = options
 
         tx.sign(owner)
         return tx
 
     def prepare_upgrade_transaction_data(self, arguments: List[Any]):
         tx_data = f"upgradeContract@{self.bytecode}@{self.metadata.to_hex()}"
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/diskcache.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/diskcache.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     contract = SmartContract(dns_address)
     contract.query(proxy, "validateName", [name_arg])
 
 
 def register(args: Any):
     args = utils.as_object(args)
 
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     args.receiver = dns_address_for_name(args.name).bech32()
     args.data = dns_register_data(args.name)
 
     tx = do_prepare_transaction(args)
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,7 +179,12 @@
     def __init__(self, message: str):
         super().__init__("Ledger error: " + message)
 
 
 class DockerMissingError(KnownError):
     def __init__(self):
         super().__init__("Docker is not installed! Please visit https://docs.docker.com/get-docker/ to install docker.")
+
+
+class GuardianServiceError(KnownError):
+    def __init__(self, message: str):
+        super().__init__(message)
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/guards.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/guards.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import OrderedDict
 from typing import Any, Dict, List, Protocol, Sequence, TextIO, Tuple
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
 from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.interfaces import ITransaction
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 logger = logging.getLogger("transactions")
 
 
 class ITransactionOnNetwork(Protocol):
     hash: str
     is_completed: bool
@@ -44,14 +45,16 @@
         self.gasPrice = 0
         self.gasLimit = 0
         self.data: str = ""
         self.chainID = ""
         self.version = 0
         self.options = 0
         self.signature = ""
+        self.guardian = ""
+        self.guardian_signature = ""
 
     # The data field is base64-encoded. Here, we only support utf-8 "data" at this moment.
     def data_encoded(self) -> str:
         return self._field_encoded("data")
 
     # Useful when loading a tx from a file (when data is already encoded in base64)
     def data_decoded(self) -> str:
@@ -176,14 +179,20 @@
 
         if self.options:
             dictionary["options"] = int(self.options)
 
         if self.signature:
             dictionary["signature"] = self.signature
 
+        if self.guardian:
+            dictionary["guardian"] = self.guardian
+
+        if self.guardian_signature:
+            dictionary["guardianSignature"] = self.guardian_signature
+
         return dictionary
 
     # Creates the payload for a "user" / "inner" transaction
     def to_dictionary_as_inner(self) -> Dict[str, Any]:
         dictionary = self.to_dictionary()
         dictionary["receiver"] = base64.b64encode(Address(self.receiver).pubkey()).decode()
         dictionary["sender"] = base64.b64encode(Address(self.sender).pubkey()).decode()
@@ -263,10 +272,15 @@
     tx.receiverUsername = getattr(args, "receiver_username", "")
     tx.gasPrice = int(args.gas_price)
     tx.gasLimit = int(args.gas_limit)
     tx.data = args.data
     tx.chainID = args.chain
     tx.version = int(args.version)
     tx.options = int(args.options)
+    tx.guardian = args.guardian
 
     tx.sign(account)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
+
     return tx
```

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/delegation/__init__.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/dependencies/modules.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_activation.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_activation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_checks.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_checks.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/eei_registry.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/eei_registry.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_clang.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_clang.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_cpp.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_cpp.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/shared.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates_config.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/templates_repository.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/templates_repository.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/config.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/core.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/genesis.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/genesis.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/genesis_json.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/genesis_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/node_config_toml.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/node_config_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/nodes_setup_json.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/nodes_setup_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/p2p_toml.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/setup.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/setup.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/testnet/wallets.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/testnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-6.2.0/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/LICENSE` & `multiversx_sdk_cli-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/README.md` & `multiversx_sdk_cli-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.1.3/pyproject.toml` & `multiversx_sdk_cli-6.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "6.1.3"
+version = "6.2.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_cli-6.1.3/PKG-INFO` & `multiversx_sdk_cli-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-cli
-Version: 6.1.3
+Version: 6.2.0
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

