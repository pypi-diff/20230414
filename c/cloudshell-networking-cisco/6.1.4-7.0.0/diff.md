# Comparing `tmp/cloudshell-networking-cisco-6.1.4.zip` & `tmp/cloudshell-networking-cisco-7.0.0.zip`

## zipinfo {}

```diff
@@ -1,121 +1,127 @@
-Zip file size: 281608 bytes, number of entries: 119
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/integration-tests/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/
--rw-r--r--  2.0 unx       51 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/test_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/setup.cfg
--rw-r--r--  2.0 unx        6 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/version.txt
--rw-r--r--  2.0 unx      855 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/setup.py
--rw-r--r--  2.0 unx      157 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/pyproject.toml
--rw-r--r--  2.0 unx      164 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/requirements.txt
--rw-r--r--  2.0 unx     1228 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tox.ini
--rw-r--r--  2.0 unx       71 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/dev_requirements.txt
--rw-r--r--  2.0 unx      359 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/PKG-INFO
--rw-r--r--  2.0 unx      948 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/README.md
--rw-r--r--  2.0 unx       66 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/MANIFEST.in
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/runners/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/__init__.py
--rw-r--r--  2.0 unx     1331 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/test_cisco_snmp_autoload.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/
--rw-r--r--  2.0 unx     2343 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py
--rw-r--r--  2.0 unx    16208 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_vlan_actions.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/__init__.py
--rw-r--r--  2.0 unx     2148 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_iface_actions.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/__init__.py
--rw-r--r--  2.0 unx    37432 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/system_actions_output.py
--rw-r--r--  2.0 unx     9723 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py
--rw-r--r--  2.0 unx     1945 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py
--rw-r--r--  2.0 unx     3275 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py
--rw-r--r--  2.0 unx     2763 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_restore_configuration_flow.py
--rw-r--r--  2.0 unx     9275 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_connectivity_flow.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/__init__.py
--rw-r--r--  2.0 unx     7615 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_enable_snmp_flow.py
--rw-r--r--  2.0 unx     1760 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_firmware_flow.py
--rw-r--r--  2.0 unx     2344 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_save_configuration_flow.py
--rw-r--r--  2.0 unx     4418 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_disable_snmp_flow.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/runners/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/__init__.py
--rw-r--r--  2.0 unx     4961 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/tests_cisco_cli_handler.py
--rw-r--r--  2.0 unx       20 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/__init__.py
--rw-r--r--  2.0 unx     4703 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/test_configuration_templates.py
--rw-r--r--  2.0 unx      625 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/integration-tests/test_cisco_structure_data.py
--rw-r--r--  2.0 unx    37585 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/integration-tests/test_cisco_autoload.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/integration-tests/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/top_level.txt
--rw-r--r--  2.0 unx      164 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/requires.txt
--rw-r--r--  2.0 unx     4759 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      359 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/__init__.py
--rw-r--r--  2.0 unx       68 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cisco_constants.py
--rw-r--r--  2.0 unx      358 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_if_table.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/__init__.py
--rw-r--r--  2.0 unx     2719 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_snmp_if_port.py
--rw-r--r--  2.0 unx     1349 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_port_attrs_service.py
--rw-r--r--  2.0 unx      229 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_snmp_if_port_channel.py
--rw-r--r--  2.0 unx      486 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_generic_snmp_autoload.py
--rw-r--r--  2.0 unx      810 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/console_ssh_session.py
--rw-r--r--  2.0 unx     1879 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/console_telnet_session.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/__init__.py
--rw-r--r--  2.0 unx    12888 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/system_actions.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/__init__.py
--rw-r--r--  2.0 unx     9790 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py
--rw-r--r--  2.0 unx    11052 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py
--rw-r--r--  2.0 unx     6079 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/iface_actions.py
--rw-r--r--  2.0 unx     9537 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py
--rw-r--r--  2.0 unx      123 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_run_command_flow.py
--rw-r--r--  2.0 unx     4031 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_configuration_flow.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/__init__.py
--rw-r--r--  2.0 unx     3867 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py
--rw-r--r--  2.0 unx     3009 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_autoload_flow.py
--rw-r--r--  2.0 unx      106 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_state_flow.py
--rw-r--r--  2.0 unx     5235 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py
--rw-r--r--  2.0 unx     7019 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/__init__.py
--rw-r--r--  2.0 unx     1417 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py
--rw-r--r--  2.0 unx     2760 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_cli_handler.py
--rw-r--r--  2.0 unx     4660 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_command_modes.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/__init__.py
--rw-r--r--  2.0 unx    10641 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-SMI.py
--rw-r--r--  2.0 unx    21732 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.py
--rw-r--r--  2.0 unx    77922 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.py
--rw-r--r--  2.0 unx     7749 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-ST-TC.py
--rw-r--r--  2.0 unx    15609 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-CONFIG-COPY-MIB.py
--rw-r--r--  2.0 unx    22985 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-TC.py
--rw-r--r--  2.0 unx       96 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/__init__.py
--rw-r--r--  2.0 unx    11678 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/device_names_map.csv
--rw-r--r--  2.0 unx    38772 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.py
--rw-r--r--  2.0 unx   263265 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.py
--rw-r--r--  2.0 unx   179774 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.py
--rw-r--r--  2.0 unx   890185 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.py
--rw-r--r--  2.0 unx     1167 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/iface.py
--rw-r--r--  2.0 unx      373 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/firmware.py
--rw-r--r--  2.0 unx     2112 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py
--rw-r--r--  2.0 unx     5252 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/configuration.py
--rw-r--r--  2.0 unx       76 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/__init__.py
--rw-r--r--  2.0 unx     1538 b- defN 21-Jun-28 12:27 cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/add_remove_vlan.py
-119 files, 1801576 bytes uncompressed, 253660 bytes compressed:  85.9%
+Zip file size: 281674 bytes, number of entries: 125
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/PKG-INFO
+-rw-r--r--  2.0 unx     1081 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tox.ini
+-rw-r--r--  2.0 unx      843 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/setup.py
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/setup.cfg
+-rw-r--r--  2.0 unx      948 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/README.md
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/version.txt
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx      174 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/requirements.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/test_requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/sessions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/__init__.py
+-rw-r--r--  2.0 unx       68 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cisco_constants.py
+-rw-r--r--  2.0 unx      123 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_run_command_flow.py
+-rw-r--r--  2.0 unx     3835 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py
+-rw-r--r--  2.0 unx     5079 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/__init__.py
+-rw-r--r--  2.0 unx      106 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_state_flow.py
+-rw-r--r--  2.0 unx     7007 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py
+-rw-r--r--  2.0 unx     9750 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py
+-rw-r--r--  2.0 unx     2836 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_autoload_flow.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_configuration_flow.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/
+-rw-r--r--  2.0 unx      506 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/cisco_snmp_if_port.py
+-rw-r--r--  2.0 unx     1305 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/cisco_generic_snmp_autoload.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/__init__.py
+-rw-r--r--  2.0 unx      360 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/snmp_constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/__init__.py
+-rw-r--r--  2.0 unx     1947 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_neighbours.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_duplex_table.py
+-rw-r--r--  2.0 unx      877 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_duplex.py
+-rw-r--r--  2.0 unx     1009 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_snmp_port_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/__init__.py
+-rw-r--r--  2.0 unx      902 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_auto_neg.py
+-rw-r--r--  2.0 unx     2175 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/cisco_sys_info_table.py
+-rw-r--r--  2.0 unx      564 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/cisco_ports_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/__init__.py
+-rw-r--r--  2.0 unx    11020 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py
+-rw-r--r--  2.0 unx     6038 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/iface_actions.py
+-rw-r--r--  2.0 unx    12745 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/system_actions.py
+-rw-r--r--  2.0 unx    10160 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py
+-rw-r--r--  2.0 unx     3305 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_cli_handler.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/__init__.py
+-rw-r--r--  2.0 unx     4506 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_command_modes.py
+-rw-r--r--  2.0 unx      348 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/firmware.py
+-rw-r--r--  2.0 unx     5363 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/configuration.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/__init__.py
+-rw-r--r--  2.0 unx     1514 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/add_remove_vlan.py
+-rw-r--r--  2.0 unx     2088 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py
+-rw-r--r--  2.0 unx     1143 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/iface.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/cisco_errors.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/sessions/__init__.py
+-rw-r--r--  2.0 unx     1074 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/__init__.py
+-rw-r--r--  2.0 unx    33074 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.json
+-rw-r--r--  2.0 unx    10222 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-SMI.json
+-rw-r--r--  2.0 unx  1382575 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.json
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/__init__.py
+-rw-r--r--  2.0 unx    92788 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.json
+-rw-r--r--  2.0 unx    35473 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-TC.json
+-rw-r--r--  2.0 unx   331332 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.json
+-rw-r--r--  2.0 unx    50241 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.json
+-rw-r--r--  2.0 unx   389549 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.json
+-rw-r--r--  2.0 unx    11678 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/device_names_map.csv
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/runners/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/__init__.py
+-rw-r--r--  2.0 unx    10902 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_connectivity_flow.py
+-rw-r--r--  2.0 unx     7563 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_enable_snmp_flow.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/__init__.py
+-rw-r--r--  2.0 unx     2989 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_restore_configuration_flow.py
+-rw-r--r--  2.0 unx     1825 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_firmware_flow.py
+-rw-r--r--  2.0 unx     2594 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_save_configuration_flow.py
+-rw-r--r--  2.0 unx     4315 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_disable_snmp_flow.py
+-rw-r--r--  2.0 unx     6980 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/test_cisco_if_port.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/__init__.py
+-rw-r--r--  2.0 unx     1477 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/test_cisco_snmp_autoload.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/
+-rw-r--r--  2.0 unx     2352 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/__init__.py
+-rw-r--r--  2.0 unx     2157 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_iface_actions.py
+-rw-r--r--  2.0 unx    16217 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_vlan_actions.py
+-rw-r--r--  2.0 unx    37432 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/system_actions_output.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py
+-rw-r--r--  2.0 unx     1877 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py
+-rw-r--r--  2.0 unx    10206 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/__init__.py
+-rw-r--r--  2.0 unx     4970 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/tests_cisco_cli_handler.py
+-rw-r--r--  2.0 unx     4553 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/test_configuration_templates.py
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/tests/networking/cisco/runners/__init__.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/requires.txt
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5140 b- defN 23-Apr-14 12:59 cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/SOURCES.txt
+125 files, 2572942 bytes uncompressed, 251776 bytes compressed:  90.2%
```

## zipnote {}

```diff
@@ -1,358 +1,376 @@
-Filename: cloudshell-networking-cisco-6.1.4/
+Filename: cloudshell-networking-cisco-7.0.0/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/integration-tests/
+Filename: cloudshell-networking-cisco-7.0.0/tests/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/
+Filename: cloudshell-networking-cisco-7.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/test_requirements.txt
+Filename: cloudshell-networking-cisco-7.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/setup.cfg
+Filename: cloudshell-networking-cisco-7.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/version.txt
+Filename: cloudshell-networking-cisco-7.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/setup.py
+Filename: cloudshell-networking-cisco-7.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/pyproject.toml
+Filename: cloudshell-networking-cisco-7.0.0/README.md
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/requirements.txt
+Filename: cloudshell-networking-cisco-7.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tox.ini
+Filename: cloudshell-networking-cisco-7.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/dev_requirements.txt
+Filename: cloudshell-networking-cisco-7.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/PKG-INFO
+Filename: cloudshell-networking-cisco-7.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/README.md
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/MANIFEST.in
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/runners/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/sessions/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/test_cisco_snmp_autoload.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/autoload/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cisco_constants.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_run_command_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_vlan_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_iface_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_state_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/system_actions_output.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_autoload_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_configuration_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_restore_configuration_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_connectivity_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/cisco_snmp_if_port.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_enable_snmp_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/cisco_generic_snmp_autoload.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_firmware_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_save_configuration_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/snmp_constants.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_disable_snmp_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/constants/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/runners/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_neighbours.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_duplex_table.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/tests_cisco_cli_handler.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_duplex.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_snmp_port_table.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/test_configuration_templates.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/integration-tests/test_cisco_structure_data.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_auto_neg.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/integration-tests/test_cisco_autoload.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/cisco_sys_info_table.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/integration-tests/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/cisco_ports_table.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/top_level.txt
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/autoload/table_services/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/requires.txt
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/SOURCES.txt
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/PKG-INFO
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/iface_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/dependency_links.txt
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/system_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_cli_handler.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_command_modes.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/firmware.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/configuration.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/add_remove_vlan.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/iface.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/errors/cisco_errors.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/sessions/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cisco_constants.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_if_table.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_snmp_if_port.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-SMI.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_port_attrs_service.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_snmp_if_port_channel.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/autoload/cisco_generic_snmp_autoload.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/console_ssh_session.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-TC.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/console_telnet_session.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/sessions/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/system_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.json
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/device_names_map.csv
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/iface_actions.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_run_command_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_configuration_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_autoload_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_state_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/runners/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_connectivity_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_enable_snmp_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_cli_handler.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_restore_configuration_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_command_modes.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_firmware_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_save_configuration_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-SMI.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_disable_snmp_flow.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/test_cisco_if_port.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-ST-TC.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/autoload/test_cisco_snmp_autoload.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-CONFIG-COPY-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-TC.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/device_names_map.csv
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_iface_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_vlan_actions.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/system_actions_output.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/iface.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/firmware.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/configuration.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/tests_cisco_cli_handler.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/__init__.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/test_configuration_templates.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/add_remove_vlan.py
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/tests/networking/cisco/runners/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/requires.txt
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/PKG-INFO
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/dependency_links.txt
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/top_level.txt
+Comment: 
+
+Filename: cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-networking-cisco-6.1.4/setup.py` & `cloudshell-networking-cisco-7.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,12 +17,11 @@
     author="QualiSystems",
     author_email="info@qualisystems.com",
     packages=find_packages(),
     install_requires=required,
     tests_require=required_for_tests,
     version=version_from_file,
     description="QualiSystems networking cisco specific package",
+    long_description="QualiSystems networking cisco specific package",
     include_package_data=True,
-    python_requires=(
-        ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, <4"
-    ),
+    python_requires="~=3.7",
 )
```

## Comparing `cloudshell-networking-cisco-6.1.4/tox.ini` & `cloudshell-networking-cisco-7.0.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 # tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
-[DEFAULT]
-package-name = cloudshell.networking.cisco
 
 [tox]
 envlist =
-    py{27,37}-{master,dev}
+    py{37,39}-{master,dev}
     pre-commit
     build
 distshare = dist
 
 [testenv]
 skip_install:
     dev: true
 deps =
     master: -r test_requirements.txt
     dev: -r dev_requirements.txt
 commands =
-    nosetests --with-coverage --cover-package={[DEFAULT]package-name} tests
+    pytest --cov=cloudshell.networking.cisco tests --cov-report=xml
 
 [testenv:pre-commit]
 basepython = python3
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
 
 [testenv:build]
 skip_install = true
 commands =
     python setup.py -q sdist --format zip
-    python setup.py -q bdist_wheel --universal
+    python setup.py -q bdist_wheel
 
 [isort]
-line_length = 88
-forced_separate = %(package-name)s,tests
-multi_line_output = 3
-include_trailing_comma = True
-combine_as_imports = 1
-skip = mibs
+profile=black
+forced_separate = cloudshell.networking.cisco,tests
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
-ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203
+ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203,E501
 exclude = mibs
```

## Comparing `cloudshell-networking-cisco-6.1.4/README.md` & `cloudshell-networking-cisco-7.0.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from cloudshell.networking.cisco.command_actions.enable_disable_snmp_actions import (
     EnableDisableSnmpActions,
 )
 
 try:
     from unittest.mock import MagicMock, create_autospec
 except ImportError:
-    from mock import MagicMock, create_autospec
+    from unittest.mock import MagicMock, create_autospec
 
 
 def return_cmd(cmd, **kwargs):
     return cmd
 
 
 class TestCiscoEnableSNMPActions(TestCase):
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_vlan_actions.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_vlan_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     AddRemoveVlanActions,
 )
 from cloudshell.networking.cisco.command_templates.add_remove_vlan import L2_TUNNEL
 
 try:
     from unittest.mock import MagicMock, create_autospec, patch
 except ImportError:
-    from mock import MagicMock, create_autospec, patch
+    from unittest.mock import MagicMock, create_autospec, patch
 
 
 class TestAddRemoveVlanActions(TestCase):
     def setUp(self):
         self._cli_service = create_autospec(CliServiceImpl)
         self._handler = AddRemoveVlanActions(self._cli_service, MagicMock())
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/test_iface_actions.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/test_iface_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cloudshell.cli.service.cli_service_impl import CliServiceImpl
 
 from cloudshell.networking.cisco.command_actions.iface_actions import IFaceActions
 
 try:
     from unittest.mock import MagicMock, create_autospec, patch
 except ImportError:
-    from mock import MagicMock, create_autospec, patch
+    from unittest.mock import MagicMock, create_autospec, patch
 
 
 class TestAddRemoveVlanActions(TestCase):
     def setUp(self):
         self._cli_service = create_autospec(CliServiceImpl)
         self._handler = IFaceActions(self._cli_service, MagicMock())
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/system_actions_output.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/system_actions_output.py`

 * *Files identical despite different names*

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_prepare_action_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 from unittest import TestCase
 
+from cloudshell.shell.flows.utils.url import BasicLocalUrl, RemoteURL
+
 from cloudshell.networking.cisco.command_actions.system_actions import SystemActions
 
 try:
     from unittest.mock import MagicMock
 except ImportError:
-    from mock import MagicMock
+    from unittest.mock import MagicMock
 
 
 class TestCiscoSystemActions(TestCase):
-    TEST_RUNNING_CONFIG_SHORT_PATH = "running-config"
-    TEST_RUNNING_CONFIG_FULL_PATH = "bootflash:/running-config"
-    TEST_RUNNING_CONFIG_REMOTE_TFTP_TEXT_PATH = "tftp://localhost/running-config"
-    TEST_RUNNING_CONFIG_REMOTE_TFTP_IP_PATH = "tftp://127.0.0.1/running-config"
-    TEST_RUNNING_CONFIG_REMOTE_FTP_TEXT_PATH = (
+    TEST_RUNNING_CONFIG_SHORT_PATH = BasicLocalUrl.from_str("running-config", "/")
+    TEST_RUNNING_CONFIG_FULL_PATH = BasicLocalUrl.from_str("bootflash:/running-config")
+    TEST_RUNNING_CONFIG_REMOTE_TFTP_TEXT_PATH = RemoteURL.from_str(
+        "tftp://localhost/running-config"
+    )
+    TEST_RUNNING_CONFIG_REMOTE_TFTP_IP_PATH = RemoteURL.from_str(
+        "tftp://127.0.0.1/running-config"
+    )
+    TEST_RUNNING_CONFIG_REMOTE_FTP_TEXT_PATH = RemoteURL.from_str(
         "ftp://user:pass@localhost/running-config"
     )
-    TEST_RUNNING_CONFIG_REMOTE_FTP_IP_PATH = "ftp://user:pass@127.0.0.1/running-config"
+    TEST_RUNNING_CONFIG_REMOTE_FTP_IP_PATH = RemoteURL.from_str(
+        "ftp://user:pass@127.0.0.1/running-config"
+    )
 
-    TEST_RESULT_TEXT_HOST = r"(?!/)localhost(?!/)\D*\s*$"
-    TEST_RESULT_IP_HOST = r"(?!/)127.0.0.1(?!/)\D*\s*$"
-    TEST_RESULT_PASSWORD = "[Pp]assword"
-    TEST_RESULT_SRC_FILE_NAME = "[\\[\\(].*running-config[\\)\\]]"
-    TEST_RESULT_DST_FILE_NAME = "[\\[\\(]running-config[\\)\\]]"
-    TEST_RESULT_FROM_REMOTE_DST_FILE_NAME = "(?!/)[\\[\\(]running-config[\\)\\]]"
+    TEST_RESULT_TEXT_HOST = SystemActions.HOSTNAME_PATTERN.format(host="localhost")
+    TEST_RESULT_IP_HOST = SystemActions.HOSTNAME_PATTERN.format(host="127.0.0.1")
+    TEST_RESULT_PASSWORD = SystemActions.PASSWORD_PATTERN
+    TEST_RESULT_SRC_FILE_NAME = SystemActions.SRC_FILE_NAME_PATTERN.format(
+        src_file_name="running-config"
+    )
+    TEST_RESULT_DST_FILE_NAME = SystemActions.DST_FILE_NAME_PATTERN.format(
+        dst_file_name="running-config"
+    )
+    TEST_RESULT_FROM_REMOTE_DST_FILE_NAME = SystemActions.DST_FILE_NAME_PATTERN.format(
+        dst_file_name="running-config"
+    )
 
     def setUp(self):
         self.system_action = SystemActions(cli_service=MagicMock(), logger=MagicMock())
 
     def test_prepare_action_map_tftp_text_path(self):
         short_path_action_map = self.system_action.prepare_action_map(
             self.TEST_RUNNING_CONFIG_SHORT_PATH,
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_restore_override.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
 from . import system_actions_output
 
 from cloudshell.networking.cisco.command_actions.system_actions import SystemActions
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoSystemActionsCopy(TestCase):
     def setUp(self):
         self.system_action = SystemActions(cli_service=MagicMock(), logger=MagicMock())
 
     def test_restore_override_success(self):
         with patch(
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_actions/system_actions/test_system_actions_copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
 from . import system_actions_output
 
 from cloudshell.networking.cisco.command_actions.system_actions import SystemActions
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoSystemActionsCopy(TestCase):
     def setUp(self):
         self.system_action = SystemActions(cli_service=MagicMock(), logger=MagicMock())
 
     def test_copy_success(self):
         with patch(
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_restore_configuration_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_restore_configuration_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
+
+from cloudshell.shell.flows.configuration.basic_flow import (
+    ConfigurationType,
+    RestoreMethod,
+)
+from cloudshell.shell.flows.utils.url import RemoteURL
 
 from cloudshell.networking.cisco.flows.cisco_configuration_flow import (
     CiscoConfigurationFlow,
 )
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoSaveConfigurationFlow(TestCase):
-    PATH = "ftp://admin:password@10.10.10.10/CloudShell/config"
+    PATH = RemoteURL.from_str("ftp://admin:password@10.10.10.10/CloudShell/config")
 
     def setUp(self):
         cli = MagicMock()
         logger = MagicMock()
         self.handler = CiscoConfigurationFlow(cli, MagicMock(), logger)
 
     @patch("cloudshell.networking.cisco.flows.cisco_configuration_flow.SystemActions")
     def test_restore_append_startup(self, sys_actions_mock):
         copy_mock = MagicMock()
         sys_actions_mock.return_value.copy = copy_mock
-        configuration_type = "startup"
-        restore_method = "append"
+        configuration_type = ConfigurationType.STARTUP
+        restore_method = RestoreMethod.APPEND
         vrf_management_name = MagicMock()
         self.handler._restore_flow(
             self.PATH, configuration_type, restore_method, vrf_management_name
         )
         copy_mock.assert_called_once()
 
     @patch("cloudshell.networking.cisco.flows.cisco_configuration_flow.SystemActions")
     def test_restore_append_running(self, sys_actions_mock):
         copy_mock = MagicMock()
         sys_actions_mock.return_value.copy = copy_mock
-        configuration_type = "running"
-        restore_method = "append"
+        configuration_type = ConfigurationType.RUNNING
+        restore_method = RestoreMethod.APPEND
         vrf_management_name = MagicMock()
         self.handler._restore_flow(
             self.PATH, configuration_type, restore_method, vrf_management_name
         )
         copy_mock.assert_called_once()
 
     @patch("cloudshell.networking.cisco.flows.cisco_configuration_flow.SystemActions")
     def test_restore_override_startup(self, sys_actions_mock):
         delete_mock = MagicMock()
         copy_mock = MagicMock()
         sys_actions_mock.return_value.delete_file = delete_mock
         sys_actions_mock.return_value.copy = copy_mock
-        configuration_type = "startup"
-        restore_method = "override"
+        configuration_type = ConfigurationType.STARTUP
+        restore_method = RestoreMethod.OVERRIDE
         vrf_management_name = MagicMock()
         self.handler._restore_flow(
             self.PATH, configuration_type, restore_method, vrf_management_name
         )
         delete_mock.assert_called_once()
         copy_mock.assert_called_once()
 
     @patch("cloudshell.networking.cisco.flows.cisco_configuration_flow.SystemActions")
     def test_restore_override_running(self, sys_actions_mock):
         override_running_mock = MagicMock()
         sys_actions_mock.return_value.override_running = override_running_mock
-        configuration_type = "running"
-        restore_method = "override"
+        configuration_type = ConfigurationType.RUNNING
+        restore_method = RestoreMethod.OVERRIDE
         vrf_management_name = MagicMock()
         self.handler._restore_flow(
             self.PATH, configuration_type, restore_method, vrf_management_name
         )
         override_running_mock.assert_called_once()
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_connectivity_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_connectivity_flow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,47 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, Mock, create_autospec, patch
 
 from cloudshell.cli.session.session_exceptions import CommandExecutionException
+from cloudshell.shell.flows.connectivity.models.connectivity_model import (
+    ConnectivityActionModel,
+    ConnectivityTypeEnum,
+)
 
 from cloudshell.networking.cisco.flows.cisco_connectivity_flow import (
     CiscoConnectivityFlow,
 )
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoAddVlanFlow(TestCase):
     def setUp(self):
         self._handler = CiscoConnectivityFlow(MagicMock(), MagicMock())
 
+    def create_vlan_model(
+        self,
+        action_id="id",
+        request_type=ConnectivityTypeEnum.SET_VLAN,
+        vlan_id="45",
+        port_mode="trunk",
+        port_name="Ethernet4-5",
+        qnq=False,
+        c_tag="",
+    ) -> ConnectivityActionModel:
+        action = create_autospec(ConnectivityActionModel)
+        action.action_id = action_id
+        action.type = request_type
+        action.connection_params = Mock(
+            vlan_id=vlan_id,
+            mode=Mock(value=port_mode),
+            vlan_service_attrs=Mock(qnq=qnq, ctag=c_tag),
+        )
+        action.action_target = Mock()
+        action.action_target.name = port_name
+        return action
+
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow.AddRemoveVlanActions"
     )
     @patch("cloudshell.networking.cisco.flows.cisco_connectivity_flow.IFaceActions")
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow."
         "CiscoConnectivityFlow._add_sub_interface_vlan"
@@ -27,129 +49,128 @@
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow."
         "CiscoConnectivityFlow._add_switchport_vlan"
     )
     def test_add_vlan_router_flow(
         self, add_vlan_mock, add_sub_iface_mock, iface_mock, vlan_actions_mock
     ):
-        port_mode = "trunk"
-        port_name = "Ethernet4-5"
-        converted_port_name = "Ethernet4/5"
-        vlan_id = "45"
-        qnq = False
-        c_tag = ""
+        action = self.create_vlan_model()
+        converted_port_name = action.action_target.name.replace("-", "/")
         iface_mock.return_value.get_port_name.return_value = converted_port_name
+
         add_vlan_mock.side_effect = [CommandExecutionException("failed")]
         add_sub_iface_mock.return_value = "interface {}.{}".format(
-            converted_port_name, vlan_id
+            converted_port_name, action.connection_params.vlan_id
         )
 
-        self._handler._add_vlan_flow(vlan_id, port_mode, port_name, qnq, c_tag)
+        self._handler._set_vlan(action)
 
-        iface_mock.return_value.get_port_name.assert_called_once_with(port_name)
+        iface_mock.return_value.get_port_name.assert_called_once_with(
+            action.action_target.name
+        )
 
         add_sub_iface_mock.assert_called_once_with(
             vlan_actions_mock.return_value,
             iface_mock.return_value,
-            vlan_id,
+            action.connection_params.vlan_id,
             converted_port_name,
-            port_mode,
-            qnq,
-            c_tag,
+            action.connection_params.mode.value,
+            action.connection_params.vlan_service_attrs.qnq,
+            action.connection_params.vlan_service_attrs.ctag,
         )
 
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow.AddRemoveVlanActions"
     )
     @patch("cloudshell.networking.cisco.flows.cisco_connectivity_flow.IFaceActions")
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow."
         "CiscoConnectivityFlow._add_switchport_vlan"
     )
     def test_add_vlan_switch_flow(self, add_vlan_mock, iface_mock, vlan_actions_mock):
-        port_mode = "trunk"
-        port_name = "Ethernet4-5"
-        response = MagicMock()
-        converted_port_name = "Ethernet4/5"
-        vlan_id = "45"
-        qnq = False
-        c_tag = ""
+        action = self.create_vlan_model()
+        response = "[ OK ] VLAN(s) {} configuration completed successfully".format(
+            action.connection_params.vlan_id
+        )
+        converted_port_name = action.action_target.name.replace("-", "/")
         iface_mock.return_value.get_port_name.return_value = converted_port_name
         add_vlan_mock.return_value = response
 
-        self._handler._add_vlan_flow(vlan_id, port_mode, port_name, qnq, c_tag)
-        iface_mock.return_value.get_port_name.assert_called_once_with(port_name)
+        self._handler._set_vlan(action)
+        iface_mock.return_value.get_port_name.assert_called_once_with(
+            action.action_target.name
+        )
         add_vlan_mock.assert_called_once_with(
             vlan_actions_mock.return_value,
             iface_mock.return_value,
-            vlan_id,
+            action.connection_params.vlan_id,
             converted_port_name,
-            port_mode,
-            qnq,
-            c_tag,
+            action.connection_params.mode.value,
+            action.connection_params.vlan_service_attrs.qnq,
+            action.connection_params.vlan_service_attrs.ctag,
         )
         vlan_mock = vlan_actions_mock.return_value
         vlan_mock.verify_interface_has_vlan_assigned.assert_called_once_with(
-            vlan_id, response
+            action.connection_params.vlan_id, response
         )
 
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow.AddRemoveVlanActions"
     )
     @patch("cloudshell.networking.cisco.flows.cisco_connectivity_flow.IFaceActions")
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow."
         "CiscoConnectivityFlow._remove_sub_interface"
     )
     def test_remove_flow_router(self, rm_sub_iface_mock, iface_mock, vlan_actions_mock):
-        port_mode = "trunk"
-        port_name = "Ethernet4-5"
-        converted_port_name = "Ethernet4/5"
-        converted_sub_port_name = "Ethernet4/5.45"
-        vlan_id = "45"
         output = "ip address 10.0.0.0/24"
+        action = self.create_vlan_model(request_type=ConnectivityTypeEnum.REMOVE_VLAN)
+        converted_port_name = action.action_target.name.replace("-", "/")
+        converted_sub_port_name = (
+            f"{converted_port_name}." f"{action.connection_params.vlan_id}"
+        )
         iface_obj_mock = iface_mock.return_value
         iface_obj_mock.get_port_name.return_value = converted_port_name
         iface_obj_mock.check_sub_interface_has_vlan.return_value = False
         iface_obj_mock.get_current_interface_config.return_value = output
         iface_obj_mock.get_sub_interfaces_config.return_value = [
             converted_sub_port_name
         ]
 
-        self._handler._remove_vlan_flow(vlan_id, port_name, port_mode)
+        self._handler._remove_vlan(action)
 
         iface_obj_mock = iface_mock.return_value
 
-        iface_obj_mock.get_port_name.assert_called_once_with(port_name)
+        iface_obj_mock.get_port_name.assert_called_once_with(action.action_target.name)
         iface_obj_mock.get_current_interface_config.assert_called_with(
             converted_sub_port_name
         )
 
         rm_sub_iface_mock.assert_called_once_with(
             converted_sub_port_name, iface_obj_mock
         )
 
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow.AddRemoveVlanActions"
     )
     @patch("cloudshell.networking.cisco.flows.cisco_connectivity_flow.IFaceActions")
     def test_remove_flow_switch(self, iface_mock, vlan_actions_mock):
-        port_mode = "trunk"
-        port_name = "Ethernet4-5"
-        converted_port_name = "Ethernet4/5"
-        vlan_id = "45"
+        action = self.create_vlan_model(request_type=ConnectivityTypeEnum.REMOVE_VLAN)
+        port_name = action.action_target.name
+        converted_port_name = action.action_target.name.replace("-", "/")
+        vlan_id = action.connection_params.vlan_id
         output = "switchport"
         result = "switchport allow vlan 45"
         iface_mock.return_value.get_port_name.return_value = converted_port_name
         vlan_mock = vlan_actions_mock.return_value
         vlan_mock.verify_interface_has_vlan_assigned.return_value = False
         iface_obj_mock = iface_mock.return_value
         iface_obj_mock.get_current_interface_config.side_effect = [output, result]
 
-        self._handler._remove_vlan_flow(vlan_id, port_name, port_mode)
+        self._handler._remove_vlan(action)
 
         iface_obj_mock.get_port_name.assert_called_once_with(port_name)
         iface_obj_mock.get_current_interface_config.assert_called_with(
             converted_port_name
         )
         iface_mock.return_value.enter_iface_config_mode.assert_called_once_with(
             converted_port_name
@@ -173,27 +194,30 @@
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow."
         "CiscoConnectivityFlow._remove_vlan_from_sub_interface"
     )
     def test_remove_all_flow_router(
         self, rm_sub_iface_mock, iface_mock, vlan_actions_mock
     ):
-        port_name = "Ethernet4-5"
-        converted_port_name = "Ethernet4/5"
+        action = self.create_vlan_model(
+            vlan_id="", request_type=ConnectivityTypeEnum.REMOVE_VLAN
+        )
+        port_name = action.action_target.name
+        converted_port_name = action.action_target.name.replace("-", "/")
         output = "ip address 10.0.0.0/24"
 
         iface_mock.return_value.get_port_name.return_value = converted_port_name
         vlan_actions_mock.return_value.verify_interface_configured.return_value = False
         iface_obj_mock = iface_mock.return_value
         iface_obj_mock.get_current_interface_config.return_value = output
         iface_obj_mock.get_sub_interfaces_config.return_value = [
             converted_port_name + ".45"
         ]
 
-        self._handler._remove_all_vlan_flow(port_name)
+        self._handler._remove_vlan(action)
 
         iface_obj_mock.get_port_name.assert_called_once_with(port_name)
         iface_obj_mock.get_current_interface_config.assert_called_once_with(
             converted_port_name
         )
         iface_obj_mock.get_sub_interfaces_config.assert_called_once()
         iface_obj_mock.check_sub_interface_has_vlan.assert_called_once()
@@ -201,23 +225,28 @@
         rm_sub_iface_mock.assert_called_once_with(converted_port_name, iface_obj_mock)
 
     @patch(
         "cloudshell.networking.cisco.flows.cisco_connectivity_flow.AddRemoveVlanActions"
     )
     @patch("cloudshell.networking.cisco.flows.cisco_connectivity_flow.IFaceActions")
     def test_remove_all_flow_switch(self, iface_mock, vlan_actions_mock):
-        port_name = "Ethernet4-5"
-        converted_port_name = "Ethernet4/5"
+        action = self.create_vlan_model(
+            vlan_id="", request_type=ConnectivityTypeEnum.REMOVE_VLAN
+        )
+        port_name = action.action_target.name
+        converted_port_name = action.action_target.name.replace("-", "/")
         output = "switchport"
         iface_mock.return_value.get_port_name.return_value = converted_port_name
-        vlan_actions_mock.return_value.verify_interface_configured.return_value = False
+        vlan_actions_mock.return_value.verify_interface_has_no_vlan_assigned.return_value = (
+            True
+        )
         iface_obj_mock = iface_mock.return_value
         iface_obj_mock.get_current_interface_config.return_value = output
 
-        self._handler._remove_all_vlan_flow(port_name)
+        self._handler._remove_vlan(action)
 
         iface_obj_mock.get_port_name.assert_called_once_with(port_name)
         iface_obj_mock.get_current_interface_config.assert_called_with(
             converted_port_name
         )
         iface_mock.return_value.enter_iface_config_mode.assert_called_once_with(
             converted_port_name
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_enable_snmp_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_enable_snmp_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
 from cloudshell.snmp.snmp_parameters import (
     SNMPReadParameters,
     SNMPV3Parameters,
     SNMPWriteParameters,
 )
 
 from cloudshell.networking.cisco.flows.cisco_enable_snmp_flow import CiscoEnableSnmpFlow
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoEnableSNMPFlow(TestCase):
     IP = "localhost"
     SNMP_WRITE_COMMUNITY = "private"
     SNMP_READ_COMMUNITY = "public"
     SNMP_USER = "admin"
     SNMP_PASSWORD = "P@ssw0rD"
@@ -94,18 +90,18 @@
 
         enable_flow = self._get_handler(create_group=False)
         self.snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user=self.SNMP_USER,
             snmp_password=self.SNMP_PASSWORD,
             snmp_private_key=self.SNMP_PRIVATE_KEY,
-            private_key_protocol="DES",
+            snmp_private_key_protocol="DES",
         )
 
-        with self.assertRaisesRegexp(Exception, "DES"):
+        with self.assertRaisesRegex(Exception, "DES"):
             enable_flow.enable_flow(self.snmp_v3_parameters)
 
         enable_snmp_view_mock.assert_not_called()
         enable_snmp_group_mock.assert_not_called()
         enable_snmp_mock.assert_not_called()
 
     @patch(
@@ -159,38 +155,38 @@
         snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user="",
             snmp_password=self.SNMP_PASSWORD,
             snmp_private_key=self.SNMP_PRIVATE_KEY,
         )
 
-        with self.assertRaisesRegexp(Exception, "SNMPv3 user is not defined"):
+        with self.assertRaisesRegex(Exception, "SNMPv3 user is not defined"):
             enable_flow.enable_flow(snmp_v3_parameters)
 
     def test_validate_snmp_v3_params_validates_password_and_raise(self):
         enable_flow = CiscoEnableSnmpFlow(cli_handler=MagicMock(), logger=MagicMock())
         snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user=self.SNMP_USER,
             snmp_password="",
             snmp_private_key=self.SNMP_PRIVATE_KEY,
-            auth_protocol=SNMPV3Parameters.AUTH_MD5,
+            snmp_auth_protocol=SNMPV3Parameters.AUTH_MD5,
         )
 
-        with self.assertRaisesRegexp(Exception, "SNMPv3 Password has to be specified"):
+        with self.assertRaisesRegex(Exception, "SNMPv3 Password has to be specified"):
             enable_flow.enable_flow(snmp_v3_parameters)
 
     def test_validate_snmp_v3_params_validates_private_key_and_raise(self):
         enable_flow = CiscoEnableSnmpFlow(cli_handler=MagicMock(), logger=MagicMock())
         snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user=self.SNMP_USER,
             snmp_password=self.SNMP_PASSWORD,
             snmp_private_key="",
-            auth_protocol=SNMPV3Parameters.AUTH_MD5,
-            private_key_protocol=SNMPV3Parameters.PRIV_DES,
+            snmp_auth_protocol=SNMPV3Parameters.AUTH_MD5,
+            snmp_private_key_protocol=SNMPV3Parameters.PRIV_DES,
         )
 
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             Exception, "SNMPv3 Private key has to be specified"
         ):
             enable_flow.enable_flow(snmp_v3_parameters)
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_firmware_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_firmware_flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
+from cloudshell.networking.cisco.cisco_constants import DEFAULT_FILE_SYSTEM
 from cloudshell.networking.cisco.flows.cisco_load_firmware_flow import (
     CiscoLoadFirmwareFlow,
 )
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoLoadFirmwareFlow(TestCase):
     def setUp(self):
-        self.firmware_flow = CiscoLoadFirmwareFlow(MagicMock(), MagicMock())
+        self.firmware_flow = CiscoLoadFirmwareFlow(
+            MagicMock(), MagicMock(), MagicMock()
+        )
 
     @patch("cloudshell.networking.cisco.flows.cisco_load_firmware_flow.SystemActions")
     def test_execute_flow(self, sys_actions_mock):
         sys_actions_mock.return_value.get_current_boot_config.side_effect = [
             "filename.bin",
             "filename.bin",
         ]
-        self.firmware_flow.load_firmware("filename.bin", "")
+        self.firmware_flow.load_firmware(f"{DEFAULT_FILE_SYSTEM}filename.bin", "")
 
         sys_actions_mock.return_value.get_flash_folders_list.assert_called_once()
         sys_actions_mock.return_value.get_current_boot_image.assert_called()
         sys_actions_mock.return_value.copy.assert_called_once()
         sys_actions_mock.return_value.get_current_boot_config.assert_called_once()
 
     @patch("cloudshell.networking.cisco.flows.cisco_load_firmware_flow.FirmwareActions")
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_save_configuration_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_save_configuration_flow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from unittest import TestCase
 
+from cloudshell.shell.flows.configuration.basic_flow import ConfigurationType
+from cloudshell.shell.flows.utils.url import RemoteURL
+
 from cloudshell.networking.cisco.flows.cisco_configuration_flow import (
     CiscoConfigurationFlow,
 )
 
 try:
     from unittest.mock import MagicMock
 except ImportError:
-    from mock import MagicMock
+    from unittest.mock import MagicMock
 
 
 class TestCiscoSaveConfigurationFlow(TestCase):
     def _get_handler(self, output):
         cli = MagicMock()
         self.session = MagicMock()
         self.session.send_command.return_value = output
@@ -35,15 +38,16 @@
         [#                        ]         4.50KB
 
          TFTP put operation was successful
          Copy complete, now saving to disk (please wait)...
          N5K-L3-Sw1#"""
         )
 
-        save_flow._save_flow("tftp://127.0.0.1", "startup")
+        url = RemoteURL.from_str("tftp://127.0.0.1")
+        save_flow._save_flow(url, ConfigurationType.STARTUP)
         self.session.send_command.assert_called_once()
 
     def test_save_configuration_with_vrf(self):
         save_flow = self._get_handler(
             """N5K-L3-Sw1#
         N5K-L3-Sw1# copy running-config tftp:
         Enter destination filename: [N5K-L3-Sw1-running-config] N5K1
@@ -55,12 +59,12 @@
         [                         ]         0.50KB
         [#                        ]         4.50KB
 
          TFTP put operation was successful
          Copy complete, now saving to disk (please wait)...
          N5K-L3-Sw1#"""
         )
-
+        url = RemoteURL.from_str("tftp://127.0.0.1")
         save_flow._save_flow(
-            "tftp://127.0.0.1", "running", vrf_management_name="management"
+            url, ConfigurationType.RUNNING, vrf_management_name="management"
         )
         self.session.send_command.assert_called_once()
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/flows/test_disable_snmp_flow.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/flows/test_disable_snmp_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
 from cloudshell.snmp.snmp_parameters import (
     SNMPReadParameters,
     SNMPV3Parameters,
     SNMPWriteParameters,
 )
 
 from cloudshell.networking.cisco.flows.cisco_disable_snmp_flow import (
     CiscoDisableSnmpFlow,
 )
 from cloudshell.networking.cisco.flows.cisco_enable_snmp_flow import CiscoEnableSnmpFlow
 
-try:
-    from unittest.mock import MagicMock, patch
-except ImportError:
-    from mock import MagicMock, patch
-
 
 class TestCiscoDisableSNMPFlow(TestCase):
     IP = "localhost"
     SNMP_WRITE_COMMUNITY = "private"
     SNMP_READ_COMMUNITY = "public"
     SNMP_USER = "admin"
     SNMP_PASSWORD = "P@ssw0rD"
     SNMP_PRIVATE_KEY = "PrivKey"
 
-    def _get_handler(self, remove_group=True):
+    def _get_handler(self):
         self.snmp_v2_write_parameters = SNMPWriteParameters(
             ip=self.IP, snmp_community=self.SNMP_WRITE_COMMUNITY
         )
         self.snmp_v2_read_parameters = SNMPReadParameters(
             ip=self.IP, snmp_community=self.SNMP_READ_COMMUNITY
         )
         self.snmp_v3_parameters = SNMPV3Parameters(
@@ -48,21 +44,21 @@
     )
     def test_disable_snmp_v3_no_group(self, disable_actions_mock):
         disable_actions_mock.return_value.get_current_snmp_user.side_effect = [
             self.SNMP_USER,
             "",
         ]
 
-        disable_flow = self._get_handler(remove_group=False)
+        disable_flow = self._get_handler()
         self.snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user=self.SNMP_USER,
             snmp_password=self.SNMP_PASSWORD,
             snmp_private_key=self.SNMP_PRIVATE_KEY,
-            private_key_protocol="DES",
+            snmp_private_key_protocol="DES",
         )
         disable_flow.disable_flow(self.snmp_v3_parameters)
         disable_actions_mock.return_value.get_current_snmp_user.assert_called()
         disable_actions_mock.return_value.remove_snmp_user.assert_called_once_with(
             self.snmp_v3_parameters.snmp_user, CiscoEnableSnmpFlow.DEFAULT_SNMP_GROUP
         )
 
@@ -73,23 +69,23 @@
     def test_disable_snmp_v3_with_group(self, disable_actions_mock):
         disable_actions_mock.return_value.get_current_snmp_user.side_effect = [
             self.SNMP_USER,
             "",
         ]
         (
             disable_actions_mock.return_value.get_current_snmp_config.return_value
-        ) = "snmp-server view {}".format(CiscoEnableSnmpFlow.DEFAULT_SNMP_VIEW)
+        ) = f"snmp-server view {CiscoEnableSnmpFlow.DEFAULT_SNMP_VIEW}"
 
         disable_flow = self._get_handler()
         self.snmp_v3_parameters = SNMPV3Parameters(
             ip=self.IP,
             snmp_user=self.SNMP_USER,
             snmp_password=self.SNMP_PASSWORD,
             snmp_private_key=self.SNMP_PRIVATE_KEY,
-            private_key_protocol="DES",
+            snmp_private_key_protocol="DES",
         )
         disable_flow.disable_flow(self.snmp_v3_parameters)
         disable_actions_mock.return_value.get_current_snmp_user.assert_called()
         disable_actions_mock.return_value.remove_snmp_user.assert_called_once_with(
             self.snmp_v3_parameters.snmp_user, CiscoEnableSnmpFlow.DEFAULT_SNMP_GROUP
         )
         disable_actions_mock.return_value.get_current_snmp_config.assert_called_once()
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/cli/tests_cisco_cli_handler.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/cli/tests_cisco_cli_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cloudshell.networking.cisco.cli.cisco_command_modes import (
     ConfigCommandMode,
     DefaultCommandMode,
     EnableCommandMode,
 )
 
 try:
-    from mock import MagicMock, Mock, patch
+    from unittest.mock import MagicMock, Mock, patch
 except ImportError:
     from unittest.mock import MagicMock, Mock, patch
 
 
 class TestCiscoSystemActions(TestCase):
     def set_up(self):
         ConfigCommandMode.ENTER_CONFIG_RETRY_TIMEOUT = 0.5
```

## Comparing `cloudshell-networking-cisco-6.1.4/tests/networking/cisco/command_templates/test_configuration_templates.py` & `cloudshell-networking-cisco-7.0.0/tests/networking/cisco/command_templates/test_configuration_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
             [OK - 3569/4096 bytes]
             Loading CloudShell/configs/Base/3750-1_Catalyst37xxstack.cfg !
             [OK - 3569/4096 bytes]
             %The input file is not a valid config file.
             37501#
             """  # noqa: E501
         configure_replace = CONFIGURE_REPLACE.get_command(path=self.path)
-        self.assertRegexpMatches(
-            output, "|".join(configure_replace["error_map"].keys())
-        )
+        self.assertRegex(output, "|".join(configure_replace["error_map"].keys()))
 
     def test_configure_replace_with_vrf_validates_error_output(self):
         output = """Command: configure replace ftp://admin:password@10.3.3.22/CloudShell/configs/Base/3750-1_Catalyst37xxstack.cfg vrf MGMT
             This will apply all necessary additions and deletions
             to replace the current running configuration with the
             contents of the specified configuration file, which is
             assumed to be a complete configuration, not a partial
@@ -39,17 +37,15 @@
             [OK - 3569/4096 bytes]
             Loading CloudShell/configs/Base/3750-1_Catalyst37xxstack.cfg !
             [OK - 3569/4096 bytes]
             %The input file is not a valid config file.
             37501#
             """  # noqa: E501
         configure_replace = CONFIGURE_REPLACE.get_command(path=self.path, vrf="MGMT")
-        self.assertRegexpMatches(
-            output, "|".join(configure_replace["error_map"].keys())
-        )
+        self.assertRegex(output, "|".join(configure_replace["error_map"].keys()))
 
     def test_configure_replace_ignores_rollback_done_output(self):
         output = """configure replace ftp://admin:password@10.33.3.22/CloudShell/config
             This will apply all necessary additions and deletions
             to replace the current running configuration with the
             contents of the specified configuration file, which is
             assumed to be a complete configuration, not a partial
@@ -58,17 +54,15 @@
             [OK - 8973/4096 bytes]
             Loading CloudShell/configs/3750.cfg !
             Total number of passes: 0
             Rollback Done
             37501#
             """
         configure_replace = CONFIGURE_REPLACE.get_command(path=self.path)
-        self.assertNotRegexpMatches(
-            output, "|".join(configure_replace["error_map"].keys())
-        )
+        self.assertNotRegex(output, "|".join(configure_replace["error_map"].keys()))
 
     def test_configure_replace_validates_rollback_aborted_output(self):
         output = """configure replace flash:candidate_config.txt force
             The rollback configlet from the last pass is listed below:
             ********
             !List of Rollback Commands:
             adfjasdfadfa
@@ -77,23 +71,19 @@
             Rollback aborted after 5 passes
             The following commands are failed to apply to the IOS image.
             ********
             adfjasdfadfa
             ********
             """
         configure_replace = CONFIGURE_REPLACE.get_command(path=self.path)
-        self.assertRegexpMatches(
-            output, "|".join(configure_replace["error_map"].keys())
-        )
+        self.assertRegex(output, "|".join(configure_replace["error_map"].keys()))
 
     def test_configure_replace_validates_aborting_rollback_output(self):
         output = """configure replace flash:candidate_config.txt force revert trigger error
             Failed to apply command adfjasdfadfa
             Aborting Rollback.
             Rollback failed.Reverting back to the original configuration: flash:pynet-rtr1-cfgJan--6-12-49-44.412-PST-0
             Total number of passes: 1
             Rollback Done
             """  # noqa: E501
         configure_replace = CONFIGURE_REPLACE.get_command(path=self.path)
-        self.assertRegexpMatches(
-            output, "|".join(configure_replace["error_map"].keys())
-        )
+        self.assertRegex(output, "|".join(configure_replace["error_map"].keys()))
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell_networking_cisco.egg-info/SOURCES.txt` & `cloudshell-networking-cisco-7.0.0/cloudshell_networking_cisco.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 MANIFEST.in
 README.md
 dev_requirements.txt
-pyproject.toml
 requirements.txt
 setup.py
 test_requirements.txt
 tox.ini
 version.txt
 cloudshell/__init__.py
 cloudshell/networking/__init__.py
 cloudshell/networking/cisco/__init__.py
 cloudshell/networking/cisco/cisco_constants.py
 cloudshell/networking/cisco/autoload/__init__.py
 cloudshell/networking/cisco/autoload/cisco_generic_snmp_autoload.py
-cloudshell/networking/cisco/autoload/cisco_if_table.py
-cloudshell/networking/cisco/autoload/cisco_port_attrs_service.py
 cloudshell/networking/cisco/autoload/cisco_snmp_if_port.py
-cloudshell/networking/cisco/autoload/cisco_snmp_if_port_channel.py
+cloudshell/networking/cisco/autoload/constants/__init__.py
+cloudshell/networking/cisco/autoload/constants/snmp_constants.py
+cloudshell/networking/cisco/autoload/snmp_tables/__init__.py
+cloudshell/networking/cisco/autoload/snmp_tables/cisco_duplex_table.py
+cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_auto_neg.py
+cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_duplex.py
+cloudshell/networking/cisco/autoload/snmp_tables/cisco_ports_neighbours.py
+cloudshell/networking/cisco/autoload/snmp_tables/cisco_snmp_port_table.py
+cloudshell/networking/cisco/autoload/table_services/__init__.py
+cloudshell/networking/cisco/autoload/table_services/cisco_ports_table.py
+cloudshell/networking/cisco/autoload/table_services/cisco_sys_info_table.py
 cloudshell/networking/cisco/cli/__init__.py
 cloudshell/networking/cisco/cli/cisco_cli_handler.py
 cloudshell/networking/cisco/cli/cisco_command_modes.py
 cloudshell/networking/cisco/command_actions/__init__.py
 cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py
 cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py
 cloudshell/networking/cisco/command_actions/iface_actions.py
 cloudshell/networking/cisco/command_actions/system_actions.py
 cloudshell/networking/cisco/command_templates/__init__.py
 cloudshell/networking/cisco/command_templates/add_remove_vlan.py
 cloudshell/networking/cisco/command_templates/configuration.py
 cloudshell/networking/cisco/command_templates/enable_disable_snmp.py
 cloudshell/networking/cisco/command_templates/firmware.py
 cloudshell/networking/cisco/command_templates/iface.py
+cloudshell/networking/cisco/errors/__init__.py
+cloudshell/networking/cisco/errors/cisco_errors.py
 cloudshell/networking/cisco/flows/__init__.py
 cloudshell/networking/cisco/flows/cisco_autoload_flow.py
 cloudshell/networking/cisco/flows/cisco_configuration_flow.py
 cloudshell/networking/cisco/flows/cisco_connectivity_flow.py
 cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py
 cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py
 cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py
 cloudshell/networking/cisco/flows/cisco_run_command_flow.py
 cloudshell/networking/cisco/flows/cisco_state_flow.py
-cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.py
-cloudshell/networking/cisco/mibs/CISCO-CONFIG-COPY-MIB.py
-cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.py
-cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.py
-cloudshell/networking/cisco/mibs/CISCO-SMI.py
-cloudshell/networking/cisco/mibs/CISCO-ST-TC.py
-cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.py
-cloudshell/networking/cisco/mibs/CISCO-TC.py
-cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.py
-cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.py
+cloudshell/networking/cisco/mibs/CISCO-CDP-MIB.json
+cloudshell/networking/cisco/mibs/CISCO-ENTITY-VENDORTYPE-OID-MIB.json
+cloudshell/networking/cisco/mibs/CISCO-PRODUCTS-MIB.json
+cloudshell/networking/cisco/mibs/CISCO-SMI.json
+cloudshell/networking/cisco/mibs/CISCO-STACK-MIB.json
+cloudshell/networking/cisco/mibs/CISCO-TC.json
+cloudshell/networking/cisco/mibs/CISCO-VTP-MIB.json
+cloudshell/networking/cisco/mibs/FDDI-SMT73-MIB.json
 cloudshell/networking/cisco/mibs/__init__.py
 cloudshell/networking/cisco/mibs/device_names_map.csv
 cloudshell/networking/cisco/sessions/__init__.py
-cloudshell/networking/cisco/sessions/console_ssh_session.py
-cloudshell/networking/cisco/sessions/console_telnet_session.py
 cloudshell/networking/cisco/snmp/__init__.py
 cloudshell/networking/cisco/snmp/cisco_snmp_handler.py
 cloudshell_networking_cisco.egg-info/PKG-INFO
 cloudshell_networking_cisco.egg-info/SOURCES.txt
 cloudshell_networking_cisco.egg-info/dependency_links.txt
 cloudshell_networking_cisco.egg-info/requires.txt
 cloudshell_networking_cisco.egg-info/top_level.txt
-integration-tests/__init__.py
-integration-tests/test_cisco_autoload.py
-integration-tests/test_cisco_structure_data.py
 tests/__init__.py
 tests/networking/__init__.py
 tests/networking/cisco/__init__.py
 tests/networking/cisco/autoload/__init__.py
+tests/networking/cisco/autoload/test_cisco_if_port.py
 tests/networking/cisco/autoload/test_cisco_snmp_autoload.py
 tests/networking/cisco/cli/__init__.py
 tests/networking/cisco/cli/tests_cisco_cli_handler.py
 tests/networking/cisco/command_actions/__init__.py
 tests/networking/cisco/command_actions/test_enable_disable_snmp_actions.py
 tests/networking/cisco/command_actions/test_iface_actions.py
 tests/networking/cisco/command_actions/test_vlan_actions.py
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/system_actions.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/system_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 import re
 import time
 from collections import OrderedDict
 
 from cloudshell.cli.command_template.command_template_executor import (
     CommandTemplateExecutor,
 )
 from cloudshell.cli.session.session_exceptions import (
     CommandExecutionException,
     ExpectedSessionException,
 )
-from cloudshell.shell.flows.utils.networking_utils import UrlParser
 
 from cloudshell.networking.cisco.command_templates import configuration, firmware
+from cloudshell.networking.cisco.errors.cisco_errors import CiscoConfigurationError
+
 
+class SystemActions:
+    USERNAME_PATTERN = r"(?!/)\b[Uu]ser(name)?\b"
+    PASSWORD_PATTERN = r"((?:(?!:).)|^)\b[Pp]assword\b"
+    HOSTNAME_PATTERN = r"(?!/){host}(?!/)\D*\s*$"
+    DST_FILE_NAME_PATTERN = r"[\[\(].*{dst_file_name}[\)\]]"
+    SRC_FILE_NAME_PATTERN = r"[\[\(]{src_file_name}[\)\]]"
+
+    SUCCESS_COPY_PATTERN = (
+        r"\d+ bytes copied|copied.*[\[\(].*[1-9][0-9]* bytes.*[\)\]]|"
+        r"[Cc]opy complete|[\(\[]OK[\]\)]|updated\s*commit\s*database\s*\S*\s*\d+\s*sec"
+    )
 
-class SystemActions(object):
     def __init__(self, cli_service, logger):
         """Reboot actions.
 
         :param cli_service: default mode cli_service
         :type cli_service: CliService
         :param logger:
         :type logger: Logger
         :return:
         """
         self._cli_service = cli_service
         self._logger = logger
 
     @staticmethod
-    def prepare_action_map(source_file, destination_file):
+    def prepare_action_map(source_url_obj, destination_url_obj):
+        dst_file_name = destination_url_obj.filename
+        source_file_name = source_url_obj.filename
         action_map = OrderedDict()
-        if "://" in destination_file:
-            url = UrlParser.parse_url(destination_file)
-            dst_file_name = url.get(UrlParser.FILENAME)
-            source_file_name = UrlParser.parse_url(source_file).get(UrlParser.FILENAME)
-            action_map[
-                r"[\[\(].*{}[\)\]]".format(dst_file_name)
-            ] = lambda session, logger: session.send_line("", logger)
+        host = None
 
-            action_map[
-                r"[\[\(]{}[\)\]]".format(source_file_name)
-            ] = lambda session, logger: session.send_line("", logger)
-        else:
-            destination_file_name = UrlParser.parse_url(destination_file).get(
-                UrlParser.FILENAME
-            )
-            url = UrlParser.parse_url(source_file)
+        action_map[
+            SystemActions.DST_FILE_NAME_PATTERN.format(dst_file_name=dst_file_name)
+        ] = lambda session, logger: session.send_line("", logger)
+
+        action_map[
+            SystemActions.SRC_FILE_NAME_PATTERN.format(src_file_name=source_file_name)
+        ] = lambda session, logger: session.send_line("", logger)
+
+        if hasattr(source_url_obj, "host"):
+            host = source_url_obj.host
+        elif hasattr(destination_url_obj, "host"):
+            host = destination_url_obj.host
+        password = source_url_obj.password or destination_url_obj.password
+        username = source_url_obj.username or destination_url_obj.username
 
-            source_file_name = url.get(UrlParser.FILENAME)
-            action_map[
-                r"(?!/)[\[\(]{}[\)\]]".format(destination_file_name)
-            ] = lambda session, logger: session.send_line("", logger)
+        if host:
             action_map[
-                r"(?!/)[\[\(]{}[\)\]]".format(source_file_name)
+                SystemActions.HOSTNAME_PATTERN.format(host=host)
             ] = lambda session, logger: session.send_line("", logger)
-        host = url.get(UrlParser.HOSTNAME)
-        password = url.get(UrlParser.PASSWORD)
-        username = url.get(UrlParser.USERNAME)
         if username:
-            action_map[r"[Uu]ser(name)?"] = lambda session, logger: session.send_line(
-                username, logger
-            )
-        if password:
-            action_map[r"[Pp]assword"] = lambda session, logger: session.send_line(
-                password, logger
-            )
-        if host:
             action_map[
-                r"(?!/){}(?!/)\D*\s*$".format(host)
-            ] = lambda session, logger: session.send_line("", logger)
+                SystemActions.USERNAME_PATTERN
+            ] = lambda session, logger: session.send_line(username, logger)
 
+        if password:
+            action_map[
+                SystemActions.PASSWORD_PATTERN
+            ] = lambda session, logger: session.send_line(password, logger)
         return action_map
 
     def copy(
         self,
         source,
         destination,
         vrf=None,
@@ -104,19 +104,16 @@
             self._cli_service,
             configuration.COPY,
             action_map=action_map,
             error_map=error_map,
             timeout=timeout,
         ).execute_command(src=source, dst=destination, vrf=vrf)
 
-        copy_ok_pattern = (
-            r"\d+ bytes copied|copied.*[\[\(].*[1-9][0-9]* bytes.*[\)\]]|"
-            r"[Cc]opy complete|[\(\[]OK[\]\)]"
-        )
-        status_match = re.search(copy_ok_pattern, output, re.IGNORECASE)
+        status_match = re.search(self.SUCCESS_COPY_PATTERN, output, re.IGNORECASE)
+
         if not status_match:
             match_error = re.search(
                 r"%.*|TFTP put operation failed.*|sysmgr.*not supported.*\n",
                 output,
                 re.IGNORECASE,
             )
             message = "Copy Command failed. "
@@ -124,15 +121,15 @@
                 self._logger.error(message)
                 message += re.sub(r"^%\s+|\\n|\s*at.*marker.*", "", match_error.group())
             else:
                 error_match = re.search(r"error.*\n|fail.*\n", output, re.IGNORECASE)
                 if error_match:
                     self._logger.error(message)
                     message += error_match.group()
-            raise Exception("Copy", message)
+            raise CiscoConfigurationError("Copy", message)
 
     def delete_file(self, path, action_map=None, error_map=None):
         """Delete file on the device.
 
         :param path: path to file
         :param action_map: actions will be taken during executing commands,
             i.e. handles yes/no prompts
@@ -298,15 +295,15 @@
         return current_firmware
 
     def shutdown(self):
         """Shutdown the system."""
         pass
 
 
-class FirmwareActions(object):
+class FirmwareActions:
     def __init__(self, cli_service, logger):
         """Reboot actions.
 
         :param cli_service: default mode cli_service
         :type cli_service: CliService
         :param logger:
         :type logger: Logger
@@ -347,17 +344,15 @@
         :param action_map: actions will be taken during executing commands,
             i.e. handles yes/no prompts
         :param error_map: errors will be raised during executing commands,
             i.e. handles Invalid Commands errors
         """
         self._logger.debug("Start cleaning boot configuration")
 
-        self._logger.info(
-            "Removing '{}' boot config line".format(config_line_to_remove)
-        )
+        self._logger.info(f"Removing '{config_line_to_remove}' boot config line")
         CommandTemplateExecutor(
             self._cli_service,
             configuration.NO,
             action_map=action_map,
             error_map=error_map,
         ).execute_command(command=config_line_to_remove.strip(" "))
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/add_remove_vlan_actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 import re
 
 from cloudshell.cli.command_template.command_template_executor import (
     CommandTemplateExecutor,
 )
 from cloudshell.cli.session.session_exceptions import SessionException
-from cloudshell.shell.flows.connectivity.helpers.vlan_handler import VLANHandler
+from cloudshell.shell.flows.connectivity.helpers.vlan_helper import get_vlan_list
 
 from cloudshell.networking.cisco.command_templates import add_remove_vlan, iface
 
 
-class AddRemoveVlanActions(object):
+class AddRemoveVlanActions:
     CREATE_VLAN_VALIDATION_PATTERN = re.compile(
         r"[Ii]nvalid\s*([Ii]nput|[Cc]ommand)|[Cc]ommand rejected", re.IGNORECASE
     )
     CHECK_VLAN_MODE_NOT_REJECTED = re.compile(
         r"^command\s*rejected.*encapsulation\s*is\s*\S*Auto", re.IGNORECASE
     )
     CREATE_VLAN_ERROR_PATTERN = re.compile(r"%.*\\.", re.IGNORECASE)
@@ -51,17 +50,17 @@
         """Verify interface configuration.
 
         :param vlan_range:
         :param current_config:
         :return: True or False
         """
         success = True
-        vlans_list = VLANHandler(
-            is_vlan_range_supported=True, is_multi_vlan_supported=False
-        ).get_vlan_list(vlan_range)
+        vlans_list = get_vlan_list(
+            vlan_range, is_vlan_range_supported=True, is_multi_vlan_supported=False
+        )
         vlan_range_list = [v for v in vlans_list if "-" in v]
         for vlan_range in vlan_range_list:
             str_vlan_range_ls = vlan_range.split("-")
 
             vlan_range_ls = list(map(int, str_vlan_range_ls))
             vlan_min = min(vlan_range_ls)
             vlan_max = max(vlan_range_ls)
@@ -71,21 +70,38 @@
                 if vlan not in vlan_range_list and int(vlan) in vlans_range:
                     vlans_list.remove(vlan)
             if len(range(vlan_min, vlan_max)) == 1:
                 vlans_list.remove(vlan_range)
                 vlans_list.extend(str_vlan_range_ls)
         for vlan in vlans_list:
             if not re.search(
-                r"switchport.*vlan.*\b{vlan}\b".format(vlan=vlan),
+                rf"switchport.*vlan.*\b{vlan}\b",
                 current_config,
                 re.IGNORECASE,
             ):
                 success = False
         return success
 
+    @staticmethod
+    def verify_interface_has_no_vlan_assigned(current_config):
+        """Verify interface configuration.
+
+        :param vlan_range:
+        :param current_config:
+        :return: True or False
+        """
+        success = True
+        if re.search(
+            r"switchport.*vlan",
+            current_config,
+            re.IGNORECASE,
+        ):
+            success = False
+        return success
+
     def create_vlan(self, vlan_range, action_map=None, error_map=None):
         """Create vlan entity on the device.
 
         :param vlan_range: range of vlans to be created
         :param action_map: actions will be taken during executing commands,
             i.e. handles yes/no prompts
         :param error_map: errors will be raised during executing commands,
@@ -177,15 +193,15 @@
                 add_remove_vlan.SWITCHPORT_MODE,
                 action_map=action_map,
                 error_map=error_map,
             ).execute_command(port_mode=port_mode)
         if qnq:
             self._get_l2_protocol_tunnel_cmd(action_map, error_map).execute_command()
 
-        if "trunk" not in port_mode:
+        if "trunk" not in port_mode.lower():
             CommandTemplateExecutor(
                 self._cli_service,
                 add_remove_vlan.SWITCHPORT_ALLOW_VLAN,
                 action_map=action_map,
                 error_map=error_map,
             ).execute_command(port_mode_access="", vlan_range=vlan_range)
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/enable_disable_snmp_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 from cloudshell.cli.command_template.command_template_executor import (
     CommandTemplateExecutor,
 )
 from cloudshell.cli.session.session_exceptions import CommandExecutionException
 
 from cloudshell.networking.cisco.command_templates import enable_disable_snmp
 
 
-class EnableDisableSnmpActions(object):
+class EnableDisableSnmpActions:
     READ_ONLY = "ro"
     READ_WRITE = "rw"
 
     def __init__(self, cli_service, logger):
         """Reboot actions.
 
         :param cli_service: config mode cli service
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_actions/iface_actions.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_actions/iface_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 import re
 
 from cloudshell.cli.command_template.command_template_executor import (
     CommandTemplateExecutor,
 )
 
 from cloudshell.networking.cisco.command_templates import (
     add_remove_vlan,
     configuration,
     iface,
 )
 
 
-class IFaceActions(object):
+class IFaceActions:
     def __init__(self, cli_service, logger):
         """Add remove vlan.
 
         :param cli_service: config mode cli_service
         :type cli_service: cloudshell.cli.service.cli_service_impl.CliServiceImpl
         :param logger:
         :type logger: Logger
@@ -41,15 +40,15 @@
             raise Exception("get_port_name", err_msg)
 
         temp_port_name = port.split("/")[-1]
         if "port-channel" not in temp_port_name.lower():
             temp_port_name = temp_port_name.replace("-", "/")
 
             self._logger.info(
-                "Interface name validation OK, portname = {0}".format(temp_port_name)
+                f"Interface name validation OK, portname = {temp_port_name}"
             )
         return temp_port_name
 
     def get_current_interface_config(self, port_name, action_map=None, error_map=None):
         """Retrieve current interface configuration.
 
         :param port_name:
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_connectivity_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 from cloudshell.cli.session.session_exceptions import CommandExecutionException
 from cloudshell.shell.flows.connectivity.basic_flow import AbstractConnectivityFlow
+from cloudshell.shell.flows.connectivity.models.connectivity_model import (
+    ConnectivityActionModel,
+)
+from cloudshell.shell.flows.connectivity.models.driver_response import (
+    ConnectivityActionResult,
+)
+from cloudshell.shell.flows.connectivity.parse_request_service import (
+    ParseConnectivityRequestService,
+)
 
 from cloudshell.networking.cisco.command_actions.add_remove_vlan_actions import (
     AddRemoveVlanActions,
 )
 from cloudshell.networking.cisco.command_actions.iface_actions import IFaceActions
 
 
@@ -16,39 +24,50 @@
         self,
         cli_handler,
         logger,
         support_vlan_range_str=False,
         support_multi_vlan_str=False,
         is_switch=False,
     ):
-        super(CiscoConnectivityFlow, self).__init__(logger)
+        con_service = ParseConnectivityRequestService(
+            is_vlan_range_supported=support_vlan_range_str,
+            is_multi_vlan_supported=support_multi_vlan_str,
+        )
+        super().__init__(con_service, logger)
         self._cli_handler = cli_handler
-        self.IS_VLAN_RANGE_SUPPORTED = support_vlan_range_str
-        self.IS_MULTI_VLAN_SUPPORTED = support_multi_vlan_str
         self.is_switch = is_switch
 
     def _get_vlan_actions(self, config_session):
         return AddRemoveVlanActions(config_session, self._logger)
 
     def _get_iface_actions(self, config_session):
         return IFaceActions(config_session, self._logger)
 
-    def _add_vlan_flow(self, vlan_range, port_mode, full_name, qnq, c_tag, vm_uid=None):
+    def _set_vlan(self, action: ConnectivityActionModel):
+        vlan_range = action.connection_params.vlan_id
+        full_name = action.action_target.name
+        port_mode = action.connection_params.mode.value
+        qnq = action.connection_params.vlan_service_attrs.qnq
+        c_tag = action.connection_params.vlan_service_attrs.ctag
+        msg = self._add_vlan_flow(vlan_range, port_mode, full_name, qnq, c_tag)
+        return ConnectivityActionResult.success_result(action, msg)
+
+    def _add_vlan_flow(self, vlan_range, port_mode, full_name, qnq, c_tag):
         """Configures VLANs on multiple ports or port-channels.
 
         :param vlan_range: VLAN or VLAN range
         :param port_mode: mode which will be configured on port.
             Possible Values are trunk and access
-        :param port_name: full port name
+        :param full_name: full port name
         :param qnq:
         :param c_tag:
         :return:
         """
         success = False
-        self._logger.info("Add VLAN(s) {} configuration started".format(vlan_range))
+        self._logger.info(f"Add VLAN(s) {vlan_range} configuration started")
 
         with self._cli_handler.get_cli_service(
             self._cli_handler.config_mode
         ) as config_session:
             iface_action = self._get_iface_actions(config_session)
             vlan_actions = self._get_vlan_actions(config_session)
             port_name = iface_action.get_port_name(full_name)
@@ -76,25 +95,23 @@
                         vlan_range,
                         port_name,
                         port_mode,
                         qnq,
                         c_tag,
                     )
 
-                    if "{}.{}".format(port_name, vlan_range) in current_config:
+                    if f"{port_name}.{vlan_range}" in current_config:
                         success = True
             if not success:
                 raise Exception(
                     self.__class__.__name__,
-                    "[FAIL] VLAN(s) {} configuration failed".format(vlan_range),
+                    f"[FAIL] VLAN(s) {vlan_range} configuration failed",
                 )
 
-        self._logger.info(
-            "VLAN(s) {} configuration completed successfully".format(vlan_range)
-        )
+        self._logger.info(f"VLAN(s) {vlan_range} configuration completed successfully")
         return "[ OK ] VLAN(s) {} configuration completed successfully".format(
             vlan_range
         )
 
     def _add_switchport_vlan(
         self, vlan_actions, iface_actions, vlan_range, port_name, port_mode, qnq, c_tag
     ):
@@ -103,116 +120,104 @@
         current_config = iface_actions.get_current_interface_config(port_name)
         return current_config
 
     def _add_sub_interface_vlan(
         self, vlan_actions, iface_actions, vlan_range, port_name, port_mode, qnq, c_tag
     ):
         if port_name and "-" not in vlan_range:
-            sub_port_name = "{}.{}".format(port_name, vlan_range)
+            sub_port_name = f"{port_name}.{vlan_range}"
         else:
             raise Exception(self.__class__.__name__, self.CISCO_SUB_INTERFACE_ERROR)
 
         iface_actions.enter_iface_config_mode(sub_port_name)
         vlan_actions.set_vlan_to_sub_interface(
             vlan_range, port_mode, sub_port_name, qnq, c_tag
         )
         current_config = iface_actions.get_current_interface_config(sub_port_name)
         return current_config
 
-    def _remove_all_vlan_flow(self, full_name, vm_uid=None):
-        """Remove configuration of VLANs on multiple ports or port-channels.
-
-        :param port_name: full port name
-            Possible Values are trunk and access
-        :return:
-        """
-        self._logger.info(
-            "Interface {} configuration cleanup started".format(full_name)
-        )
-        with self._cli_handler.get_cli_service(
-            self._cli_handler.config_mode
-        ) as config_session:
-            iface_action = self._get_iface_actions(config_session)
-            vlan_actions = self._get_vlan_actions(config_session)
-            port_name = iface_action.get_port_name(full_name)
-
-            current_config = iface_action.get_current_interface_config(port_name)
-            if "switchport" not in current_config:
-                self._remove_vlan_from_sub_interface(port_name, iface_action)
-                sub_interfaces_list = iface_action.get_sub_interfaces_config(port_name)
-                for interface in sub_interfaces_list:
-                    if iface_action.check_sub_interface_has_vlan(interface):
-                        self._logger.error(
-                            "[FAIL] Unable to clean sub interface: {}".format(interface)
-                        )
-            else:
-                iface_action.enter_iface_config_mode(port_name)
-                iface_action.clean_interface_switchport_config(current_config)
-                current_config = iface_action.get_current_interface_config(port_name)
-                if vlan_actions.verify_interface_configured(current_config):
-                    self._logger.error(
-                        "[FAIL] VLAN(s) cleanup failed for {}".format(port_name)
-                    )
+    def _remove_vlan(self, action: ConnectivityActionModel):
+        vlan_range = action.connection_params.vlan_id
+        full_name = action.action_target.name
+        msg = self._remove_vlan_flow(vlan_range, full_name)
+        return ConnectivityActionResult.success_result(action, msg)
 
-        self._logger.info(
-            "[ OK ] All VLAN(s) were removed successfully from {}".format(port_name)
-        )
-
-    def _remove_vlan_flow(self, vlan_range, full_name, port_mode, vm_uid=None):
+    def _remove_vlan_flow(self, vlan_range, full_name):
         """Remove configuration of VLANs on multiple ports or port-channels.
 
         :param vlan_range: VLAN or VLAN range
         :param full_name: full port name
         :param port_mode: mode which will be configured on port.
             Possible Values are trunk and access
         :return:
         """
-        self._logger.info("Remove Vlan {} configuration started".format(vlan_range))
+        vlan_range = vlan_range if vlan_range else "ALL"
+        self._logger.info(f"Remove {vlan_range} Vlan(s) configuration started")
         is_failed = False
         with self._cli_handler.get_cli_service(
             self._cli_handler.config_mode
         ) as config_session:
             iface_action = self._get_iface_actions(config_session)
             vlan_actions = self._get_vlan_actions(config_session)
             port_name = iface_action.get_port_name(full_name)
 
             current_config = iface_action.get_current_interface_config(port_name)
             if "switchport" not in current_config:
                 if not self.is_switch:
-                    sub_interface_name = "{}.{}".format(port_name, vlan_range)
-                    self._remove_sub_interface(sub_interface_name, iface_action)
-                    sub_interfaces_list = iface_action.get_current_interface_config(
-                        sub_interface_name
-                    )
-                    if sub_interface_name in sub_interfaces_list:
-                        is_failed = True
-                        self._logger.error(
-                            "Failed to remove sub interface: {}".format(
-                                sub_interface_name
+                    if vlan_range != "ALL":
+                        sub_interface_name = f"{port_name}.{vlan_range}"
+                        self._remove_sub_interface(sub_interface_name, iface_action)
+                        sub_interfaces_list = iface_action.get_current_interface_config(
+                            sub_interface_name
+                        )
+                        if sub_interface_name in sub_interfaces_list:
+                            is_failed = True
+                            self._logger.error(
+                                "Failed to remove sub interface: {}".format(
+                                    sub_interface_name
+                                )
                             )
+                    else:
+                        self._remove_vlan_from_sub_interface(port_name, iface_action)
+                        sub_interfaces_list = iface_action.get_sub_interfaces_config(
+                            port_name
                         )
+                        for interface in sub_interfaces_list:
+                            if iface_action.check_sub_interface_has_vlan(interface):
+                                self._logger.error(
+                                    "[FAIL] Unable to clean sub interface: {}".format(
+                                        interface
+                                    )
+                                )
+
             else:
                 iface_action.enter_iface_config_mode(port_name)
                 iface_action.clean_interface_switchport_config(current_config)
                 current_config = iface_action.get_current_interface_config(port_name)
-                if vlan_actions.verify_interface_has_vlan_assigned(
-                    vlan_range, current_config
+                if (
+                    vlan_range == "ALL"
+                    and not vlan_actions.verify_interface_has_no_vlan_assigned(
+                        current_config
+                    )
+                ) or (
+                    vlan_range != "ALL"
+                    and vlan_actions.verify_interface_has_vlan_assigned(
+                        vlan_range, current_config
+                    )
                 ):
                     is_failed = True
 
             if is_failed:
                 raise Exception(
                     self.__class__.__name__,
-                    "[FAIL] VLAN(s) {} removal failed".format(vlan_range),
+                    f"[FAIL] VLAN(s) {vlan_range} removal failed",
                 )
 
-        self._logger.info(
-            "VLAN(s) {} removal completed successfully".format(vlan_range)
-        )
-        return "[ OK ] VLAN(s) {} removal completed successfully".format(vlan_range)
+        self._logger.info(f"VLAN(s) {vlan_range} removal completed successfully")
+        return f"[ OK ] VLAN(s) {vlan_range} removal completed successfully"
 
     def _remove_vlan_from_sub_interface(self, port_name, iface_actions):
         sub_interfaces_list = iface_actions.get_sub_interfaces_config(port_name)
         for sub_int in sub_interfaces_list:
             iface_actions.clean_vlan_sub_iface_config(sub_int)
 
     def _remove_sub_interface(self, port_name, iface_actions):
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_configuration_flow.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_configuration_flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
-from cloudshell.shell.flows.configuration.basic_flow import AbstractConfigurationFlow
+from cloudshell.shell.flows.configuration.basic_flow import (
+    AbstractConfigurationFlow,
+    RestoreMethod,
+)
+from cloudshell.shell.flows.utils.url import BasicLocalUrl
 
 from cloudshell.networking.cisco.cisco_constants import DEFAULT_FILE_SYSTEM
 from cloudshell.networking.cisco.command_actions.system_actions import SystemActions
 
 
 class CiscoConfigurationFlow(AbstractConfigurationFlow):
     STARTUP_CONFIG_NAME = "startup_config"
     STARTUP_LOCATION = "nvram:startup_config"
 
     def __init__(self, cli_handler, resource_config, logger):
-        super(CiscoConfigurationFlow, self).__init__(logger, resource_config)
+        super().__init__(logger, resource_config)
         self._cli_handler = cli_handler
 
+    def _get_system_actions(self, enable_session):
+        return SystemActions(enable_session, self._logger)
+
     @property
-    def _file_system(self):
+    def file_system(self):
         return DEFAULT_FILE_SYSTEM
 
     def _save_flow(self, folder_path, configuration_type, vrf_management_name=None):
         """Execute flow which save selected file to the provided destination.
 
         :param folder_path: destination path where file will be saved
         :param configuration_type: source file, which will be saved
         :param vrf_management_name: Virtual Routing and Forwarding Name
         :return: saved configuration file name
         """
         with self._cli_handler.get_cli_service(
             self._cli_handler.enable_mode
         ) as enable_session:
             save_action = SystemActions(enable_session, self._logger)
-            action_map = save_action.prepare_action_map(configuration_type, folder_path)
+            config_type = configuration_type.value
+            if "-config" not in config_type:
+                config_type += "-config"
+            source_file = BasicLocalUrl.from_str(config_type, "/")
+            action_map = save_action.prepare_action_map(source_file, folder_path)
             save_action.copy(
-                configuration_type,
+                config_type,
                 folder_path,
                 vrf=vrf_management_name,
                 action_map=action_map,
             )
 
     def _restore_flow(
         self, path, configuration_type, restore_method, vrf_management_name
@@ -47,52 +57,51 @@
             file name
         :param restore_method: the restore method to use when restoring the
             configuration file. Possible Values are append and override
         :param configuration_type: the configuration type to restore.
             Possible values are startup and running
         :param vrf_management_name: Virtual Routing and Forwarding Name
         """
-        if "-config" not in configuration_type:
-            configuration_type += "-config"
-
+        config_type = configuration_type.value
+        if "-config" not in config_type:
+            config_type += "-config"
+        dst_file = BasicLocalUrl.from_str(config_type, "/")
         with self._cli_handler.get_cli_service(
             self._cli_handler.enable_mode
         ) as enable_session:
             restore_action = SystemActions(enable_session, self._logger)
-            copy_action_map = restore_action.prepare_action_map(
-                path, configuration_type
-            )
+            copy_action_map = restore_action.prepare_action_map(path, dst_file)
 
-            if "startup" in configuration_type:
-                if restore_method == "override":
+            if "startup" in config_type:
+                if restore_method == RestoreMethod.OVERRIDE:
                     del_action_map = {
                         "[Dd]elete [Ff]ilename ": lambda s, l: s.send_line(
                             self.STARTUP_CONFIG_NAME, l
                         )
                     }
                     restore_action.delete_file(
                         path=self.STARTUP_LOCATION, action_map=del_action_map
                     )
                     restore_action.copy(
                         path,
-                        configuration_type,
+                        config_type,
                         vrf=vrf_management_name,
                         action_map=copy_action_map,
                     )
                 else:
                     restore_action.copy(
                         path,
-                        configuration_type,
+                        config_type,
                         vrf=vrf_management_name,
                         action_map=copy_action_map,
                     )
 
-            elif "running" in configuration_type:
-                if restore_method == "override":
+            elif "running" in config_type:
+                if restore_method == RestoreMethod.OVERRIDE:
                     restore_action.override_running(path)
                 else:
                     restore_action.copy(
                         path,
-                        configuration_type,
+                        config_type,
                         vrf=vrf_management_name,
                         action_map=copy_action_map,
                     )
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_disable_snmp_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 import re
 
 from cloudshell.snmp.snmp_parameters import SNMPV3Parameters
 
 from cloudshell.networking.cisco.command_actions.enable_disable_snmp_actions import (
     EnableDisableSnmpActions,
 )
 from cloudshell.networking.cisco.flows.cisco_enable_snmp_flow import CiscoEnableSnmpFlow
 
 
-class CiscoDisableSnmpFlow(object):
+class CiscoDisableSnmpFlow:
     def __init__(self, cli_handler, logger):
         """Enable snmp flow.
 
         :param cli_handler:
         :type cli_handler: CiscoCliHandler
         :param logger:
         :return:
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_enable_snmp_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 import re
 
 from cloudshell.snmp.snmp_parameters import SNMPV3Parameters
 
 from cloudshell.networking.cisco.command_actions.enable_disable_snmp_actions import (
     EnableDisableSnmpActions,
 )
 
 
-class CiscoEnableSnmpFlow(object):
+class CiscoEnableSnmpFlow:
     DEFAULT_SNMP_VIEW = "quali_snmp_view"
     DEFAULT_SNMP_GROUP = "quali_snmp_group"
 
     def __init__(self, cli_handler, logger):
         """Enable snmp flow.
 
         :param cli_handler:
@@ -36,22 +35,22 @@
                 snmp_actions = EnableDisableSnmpActions(config_session, self._logger)
                 if "3" in snmp_parameters.version:
                     current_snmp_user = snmp_actions.get_current_snmp_user()
                     if snmp_parameters.snmp_user not in current_snmp_user:
                         snmp_parameters.validate()
                         current_snmp_config = snmp_actions.get_current_snmp_config()
                         if (
-                            "snmp-server view {}".format(self.DEFAULT_SNMP_VIEW)
+                            f"snmp-server view {self.DEFAULT_SNMP_VIEW}"
                             not in current_snmp_config
                         ):
                             snmp_actions.enable_snmp_view(
                                 snmp_view=self.DEFAULT_SNMP_VIEW
                             )
                         if (
-                            "snmp-server group {}".format(self.DEFAULT_SNMP_GROUP)
+                            f"snmp-server group {self.DEFAULT_SNMP_GROUP}"
                             not in current_snmp_config
                         ):
                             snmp_actions.enable_snmp_group(
                                 snmp_group=self.DEFAULT_SNMP_GROUP,
                                 snmp_view=self.DEFAULT_SNMP_VIEW,
                             )
                         priv_protocol = (
@@ -90,26 +89,24 @@
                 updated_snmp_actions = EnableDisableSnmpActions(
                     config_session, self._logger
                 )
                 if isinstance(snmp_parameters, SNMPV3Parameters):
                     updated_snmp_user = updated_snmp_actions.get_current_snmp_user()
                     if snmp_parameters.snmp_user not in updated_snmp_user:
                         raise Exception(
-                            self.__class__.__name__,
                             "Failed to create SNMP v3 Configuration."
-                            + " Please check Logs for details",
+                            + " Please check Logs for details"
                         )
                 else:
                     updated_snmp_communities = (
                         updated_snmp_actions.get_current_snmp_config()
                     )
                     if not re.search(
                         "snmp-server community {}".format(
                             re.escape(snmp_parameters.snmp_community)
                         ),
                         updated_snmp_communities,
                     ):
                         raise Exception(
-                            self.__class__.__name__,
                             "Failed to create SNMP community."
-                            + " Please check Logs for details",
+                            + " Please check Logs for details"
                         )
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/flows/cisco_load_firmware_flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,127 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 import re
 
 from cloudshell.shell.flows.firmware.basic_flow import AbstractFirmwareFlow
-from cloudshell.shell.flows.utils.networking_utils import UrlParser
+from cloudshell.shell.flows.utils.url import BasicLocalUrl
 
 from cloudshell.networking.cisco.cisco_constants import DEFAULT_FILE_SYSTEM
 from cloudshell.networking.cisco.command_actions.system_actions import (
     FirmwareActions,
     SystemActions,
 )
 
 
 class CiscoLoadFirmwareFlow(AbstractFirmwareFlow):
     RUNNING_CONFIG = "running-config"
     STARTUP_CONFIG = "startup-config"
     BOOTFOLDER = ["bootflash:", "bootdisk:"]
     KICKSTART_IMAGE = "kickstart"
 
-    def __init__(self, cli_handler, logger, default_file_system=DEFAULT_FILE_SYSTEM):
-        super(CiscoLoadFirmwareFlow, self).__init__(logger)
+    def __init__(
+        self,
+        cli_handler,
+        logger,
+        resource_config,
+        default_file_system=DEFAULT_FILE_SYSTEM,
+    ):
+        super().__init__(logger, resource_config)
         self._cli_handler = cli_handler
         self._file_system = default_file_system
 
     def _load_firmware_flow(self, path, vrf_management_name, timeout):
         """Load a firmware onto the device.
 
         :param path: The path to the firmware file, including the firmware file name
         :param vrf_management_name: Virtual Routing and Forwarding Name
         :param timeout:
         :return:
         """
-        full_path_dict = UrlParser().parse_url(path)
-        firmware_file_name = full_path_dict.get(UrlParser.FILENAME)
+        firmware_file_name = path.filename
         if not firmware_file_name:
             raise Exception(self.__class__.__name__, "Unable to find firmware file")
 
         with self._cli_handler.get_cli_service(
             self._cli_handler.enable_mode
         ) as enable_session:
             system_action = SystemActions(enable_session, self._logger)
             dst_file_system = self._file_system
 
-            firmware_dst_path = "{0}/{1}".format(dst_file_system, firmware_file_name)
-
+            firmware_dst_path = f"{dst_file_system}/{firmware_file_name}"
+            firmware_dst_path_url = BasicLocalUrl.from_str(firmware_dst_path)
             device_file_system = system_action.get_flash_folders_list()
-            self._logger.info("Discovered folders: {}".format(device_file_system))
+            self._logger.info(f"Discovered folders: {device_file_system}")
             if device_file_system:
                 device_file_system.sort()
                 for flash in device_file_system:
                     if flash in self.BOOTFOLDER:
-                        self._logger.info("Device has a {} folder".format(flash))
-                        firmware_dst_path = "{0}/{1}".format(flash, firmware_file_name)
-                        self._logger.info("Copying {} image".format(firmware_dst_path))
+                        self._logger.info(f"Device has a {flash} folder")
+                        firmware_dst_path = f"{flash}/{firmware_file_name}"
+                        self._logger.info(f"Copying {firmware_dst_path} image")
                         system_action.copy(
-                            path,
+                            path.url,
                             firmware_dst_path,
                             vrf=vrf_management_name,
                             action_map=system_action.prepare_action_map(
-                                path, firmware_dst_path
+                                path, firmware_dst_path_url
                             ),
                         )
                         break
                     if "flash-" in flash:
-                        firmware_dst_file_path = "{0}/{1}".format(
+                        firmware_dst_file_path = "{}/{}".format(
                             flash, firmware_file_name
                         )
-                        self._logger.info(
-                            "Copying {} image".format(firmware_dst_file_path)
+                        firmware_dst_file_url = BasicLocalUrl.from_str(
+                            firmware_dst_file_path
                         )
+                        self._logger.info(f"Copying {firmware_dst_file_path} image")
                         system_action.copy(
-                            path,
+                            path.url,
                             firmware_dst_file_path,
                             vrf=vrf_management_name,
                             action_map=system_action.prepare_action_map(
-                                path, firmware_dst_file_path
+                                path, firmware_dst_file_url
                             ),
                         )
             else:
-                self._logger.info("Copying {} image".format(firmware_dst_path))
+                self._logger.info(f"Copying {firmware_dst_path} image")
                 system_action.copy(
-                    path,
+                    path.url,
                     firmware_dst_path,
                     vrf=vrf_management_name,
                     action_map=system_action.prepare_action_map(
-                        path, firmware_dst_path
+                        path, firmware_dst_path_url
                     ),
                 )
 
             self._logger.info("Get current boot configuration")
             current_boot = system_action.get_current_boot_image()
             self._logger.info("Modifying boot configuration")
             self._apply_firmware(enable_session, current_boot, firmware_dst_path)
 
             output = system_action.get_current_boot_config()
             new_boot_settings = re.sub(
                 "^.*boot-start-marker|boot-end-marker.*", "", output
             )
-            self._logger.info(
-                "Boot config lines updated: {0}".format(new_boot_settings)
-            )
+            self._logger.info(f"Boot config lines updated: {new_boot_settings}")
 
             if output.find(firmware_file_name) == -1:
                 raise Exception(
                     self.__class__.__name__,
-                    "Can't add firmware '{}' for boot!".format(firmware_file_name),
+                    f"Can't add firmware '{firmware_file_name}' for boot!",
                 )
-
+            running_config = BasicLocalUrl.from_str(self.RUNNING_CONFIG, "/")
+            startup_config = BasicLocalUrl.from_str(self.STARTUP_CONFIG, "/")
             system_action.copy(
                 self.RUNNING_CONFIG,
                 self.STARTUP_CONFIG,
                 vrf=vrf_management_name,
                 action_map=system_action.prepare_action_map(
-                    self.RUNNING_CONFIG, self.STARTUP_CONFIG
+                    running_config, startup_config
                 ),
             )
             if "CONSOLE" in enable_session.session.SESSION_TYPE:
                 system_action.reload_device_via_console(timeout)
             else:
                 system_action.reload_device(timeout)
 
@@ -135,26 +139,20 @@
         )
 
         with enable_session.enter_mode(self._cli_handler.config_mode) as config_session:
             firmware_action = FirmwareActions(config_session, self._logger)
             for boot_conf in current_boot:
                 if is_kickstart_image:
                     if self.KICKSTART_IMAGE in boot_conf.lower():
-                        self._logger.info(
-                            "Removing '{}' boot config line".format(boot_conf)
-                        )
+                        self._logger.info(f"Removing '{boot_conf}' boot config line")
                         firmware_action.clean_boot_config(boot_conf)
                         firmware_config_to_append.append(boot_conf)
                 else:
-                    self._logger.info(
-                        "Removing '{}' boot config line".format(boot_conf)
-                    )
+                    self._logger.info(f"Removing '{boot_conf}' boot config line")
                     firmware_action.clean_boot_config(boot_conf)
                     firmware_config_to_append.append(boot_conf)
-            self._logger.info("Adding '{}' boot config line".format(firmware_dst_path))
+            self._logger.info(f"Adding '{firmware_dst_path}' boot config line")
             firmware_action.add_boot_config_file(firmware_dst_path)
             for append_boot in firmware_config_to_append:
                 if firmware_dst_path not in append_boot:
-                    self._logger.info(
-                        "Adding '{}' boot config line".format(append_boot)
-                    )
+                    self._logger.info(f"Adding '{append_boot}' boot config line")
                     firmware_action.add_boot_config(append_boot)
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/snmp/cisco_snmp_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 from cloudshell.snmp.snmp_configurator import (
     EnableDisableSnmpConfigurator,
     EnableDisableSnmpFlowInterface,
 )
 
 from cloudshell.networking.cisco.flows.cisco_disable_snmp_flow import (
     CiscoDisableSnmpFlow,
@@ -34,13 +31,8 @@
     def disable_snmp(self, snmp_parameters):
         CiscoDisableSnmpFlow(self._cli_handler, self._logger).disable_flow(
             snmp_parameters
         )
 
 
 class CiscoSnmpHandler(EnableDisableSnmpConfigurator):
-    def __init__(self, resource_config, logger, cli_handler):
-        self.cli_handler = cli_handler
-        enable_disable_snmp_flow = CiscoEnableDisableSnmpFlow(self.cli_handler, logger)
-        super(CiscoSnmpHandler, self).__init__(
-            enable_disable_snmp_flow, resource_config, logger
-        )
+    pass
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_cli_handler.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_cli_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from typing import ClassVar
+
+from attrs import define, field
+
 from cloudshell.cli.configurator import AbstractModeConfigurator
+from cloudshell.cli.factory.session_factory import (
+    ConsoleSessionFactory,
+    GenericSessionFactory,
+    SessionFactory,
+)
 from cloudshell.cli.service.cli import CLI
 from cloudshell.cli.service.cli_service_impl import CliServiceImpl
 from cloudshell.cli.service.command_mode_helper import CommandModeHelper
 from cloudshell.cli.service.session_pool_manager import SessionPoolManager
+from cloudshell.cli.session.console_ssh import ConsoleSSHSession
+from cloudshell.cli.session.console_telnet import ConsoleTelnetSession
 from cloudshell.cli.session.ssh_session import SSHSession
 from cloudshell.cli.session.telnet_session import TelnetSession
+from cloudshell.cli.types import T_COMMAND_MODE_RELATIONS
 
 from cloudshell.networking.cisco.cisco_constants import DEFAULT_SESSION_POOL_TIMEOUT
 from cloudshell.networking.cisco.cli.cisco_command_modes import (
     ConfigCommandMode,
     DefaultCommandMode,
     EnableCommandMode,
 )
-from cloudshell.networking.cisco.sessions.console_ssh_session import ConsoleSSHSession
-from cloudshell.networking.cisco.sessions.console_telnet_session import (
-    ConsoleTelnetSession,
-)
 
 
-class CiscoCli(object):
+class CiscoCli:
     def __init__(self, resource_config, pool_timeout=DEFAULT_SESSION_POOL_TIMEOUT):
         session_pool_size = int(resource_config.sessions_concurrency_limit)
         session_pool = SessionPoolManager(
             max_pool_size=session_pool_size, pool_timeout=pool_timeout
         )
         self.cli = CLI(session_pool=session_pool)
 
     def get_cli_handler(self, resource_config, logger):
-        return CiscoCliHandler(self.cli, resource_config, logger)
+        return CiscoCliHandler.from_config(resource_config, logger, self.cli)
 
 
+@define
 class CiscoCliHandler(AbstractModeConfigurator):
-    REGISTERED_SESSIONS = (
-        SSHSession,
-        TelnetSession,
-        ConsoleSSHSession,
-        ConsoleTelnetSession,
+    REGISTERED_SESSIONS: ClassVar[tuple[SessionFactory]] = (
+        GenericSessionFactory(SSHSession),
+        GenericSessionFactory(TelnetSession),
+        ConsoleSessionFactory(ConsoleSSHSession),
+        ConsoleSessionFactory(
+            ConsoleTelnetSession, session_kwargs={"start_with_new_line": False}
+        ),
+        ConsoleSessionFactory(
+            ConsoleTelnetSession, session_kwargs={"start_with_new_line": True}
+        ),
     )
+    modes: T_COMMAND_MODE_RELATIONS = field(init=False)
 
-    def __init__(self, cli, resource_config, logger):
-        super(CiscoCliHandler, self).__init__(resource_config, logger, cli)
-        self.modes = CommandModeHelper.create_command_mode(resource_config)
+    def __attrs_post_init__(self):
+        super().__attrs_post_init__()
+        self.modes = CommandModeHelper.create_command_mode(self._auth.enable_password)
 
     @property
     def default_mode(self):
         return self.modes[DefaultCommandMode]
 
     @property
     def enable_mode(self):
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/cli/cisco_command_modes.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/cli/cisco_command_modes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 import re
 import time
 from collections import OrderedDict
 
 from cloudshell.cli.service.command_mode import CommandMode
 
 
 class DefaultCommandMode(CommandMode):
     PROMPT = r">\s*$"
     ENTER_COMMAND = ""
     EXIT_COMMAND = ""
 
-    def __init__(self, resource_config):
+    def __init__(self, enable_password: str):
         """Initialize Default command mode.
 
         Only for cases when session started not in enable mode
-
-        :param resource_config:
         """
-        self.resource_config = resource_config
+        self.enable_password = enable_password
 
         CommandMode.__init__(
             self,
             DefaultCommandMode.PROMPT,
             DefaultCommandMode.ENTER_COMMAND,
             DefaultCommandMode.EXIT_COMMAND,
             enter_action_map=self.enter_action_map(),
@@ -47,20 +44,17 @@
 
 
 class EnableCommandMode(CommandMode):
     PROMPT = r"(?:(?!\)).)#\s*$"
     ENTER_COMMAND = "enable"
     EXIT_COMMAND = ""
 
-    def __init__(self, resource_config):
-        """Initialize Enable command mode - default command mode for Cisco Shells.
-
-        :param resource_config:
-        """
-        self.resource_config = resource_config
+    def __init__(self, enable_password: str):
+        """Initialize Enable command mode - default command mode for Cisco Shells."""
+        self.enable_password = enable_password
 
         CommandMode.__init__(
             self,
             EnableCommandMode.PROMPT,
             EnableCommandMode.ENTER_COMMAND,
             EnableCommandMode.EXIT_COMMAND,
             enter_action_map=self.enter_action_map(),
@@ -68,15 +62,15 @@
             enter_error_map=self.enter_error_map(),
             exit_error_map=self.exit_error_map(),
         )
 
     def enter_action_map(self):
         return {
             "[Pp]assword": lambda session, logger: session.send_line(
-                self.resource_config.enable_password, logger
+                self.enable_password, logger
             )
         }
 
     def enter_error_map(self):
         return OrderedDict()
 
     def exit_action_map(self):
@@ -90,34 +84,31 @@
     MAX_ENTER_CONFIG_MODE_RETRIES = 5
     ENTER_CONFIG_RETRY_TIMEOUT = 5
     PROMPT = r"\(config.*\)#\s*$"
     ENTER_COMMAND = "configure terminal"
     EXIT_COMMAND = "exit"
     ENTER_ACTION_COMMANDS = []
 
-    def __init__(self, resource_config):
-        """Initialize Config command mode.
-
-        :param resource_config:
-        """
-        self.resource_config = resource_config
+    def __init__(self, enable_password: str):
+        """Initialize Config command mode."""
+        self.enable_password = enable_password
 
         CommandMode.__init__(
             self,
             ConfigCommandMode.PROMPT,
             ConfigCommandMode.ENTER_COMMAND,
             ConfigCommandMode.EXIT_COMMAND,
             enter_action_map=self.enter_action_map(),
             exit_action_map=self.exit_action_map(),
             enter_error_map=self.enter_error_map(),
             exit_error_map=self.exit_error_map(),
         )
 
     def enter_action_map(self):
-        return {r"{}.*$".format(EnableCommandMode.PROMPT): self._check_config_mode}
+        return {rf"{EnableCommandMode.PROMPT}.*$": self._check_config_mode}
 
     def enter_error_map(self):
         return OrderedDict()
 
     def exit_error_map(self):
         return OrderedDict()
 
@@ -128,26 +119,26 @@
         for cmd in self.ENTER_ACTION_COMMANDS:
             cli_service.send_command(cmd)
 
     def _check_config_mode(self, session, logger):
         error_message = "Failed to enter config mode, please check logs, for details"
         output = session.hardware_expect(
             "",
-            expected_string="{0}|{1}".format(
+            expected_string="{}|{}".format(
                 EnableCommandMode.PROMPT, ConfigCommandMode.PROMPT
             ),
             logger=logger,
         )
         retry = 0
         while (
             not re.search(ConfigCommandMode.PROMPT, output)
         ) and retry < self.MAX_ENTER_CONFIG_MODE_RETRIES:
             output = session.hardware_expect(
                 ConfigCommandMode.ENTER_COMMAND,
-                expected_string="{0}|{1}".format(
+                expected_string="{}|{}".format(
                     EnableCommandMode.PROMPT, ConfigCommandMode.PROMPT
                 ),
                 logger=logger,
             )
             time.sleep(self.ENTER_CONFIG_RETRY_TIMEOUT)
             retry += 1
         if not re.search(ConfigCommandMode.PROMPT, output):
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/mibs/device_names_map.csv` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/mibs/device_names_map.csv`

 * *Files identical despite different names*

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/iface.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/iface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 from collections import OrderedDict
 
 from cloudshell.cli.command_template.command_template import CommandTemplate
 
 ACTION_MAP = OrderedDict(
     {
         r"[\[\(][Yy]es/[Nn]o[\)\]]|\[confirm\]": lambda session: session.send_line(
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/enable_disable_snmp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 from collections import OrderedDict
 
 from cloudshell.cli.command_template.command_template import CommandTemplate
 
 ERROR_MAP = OrderedDict(
     {
         (
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/configuration.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # !/usr/bin/python
-# -*- coding: utf-8 -*-
 
 from collections import OrderedDict
 
 from cloudshell.cli.command_template.command_template import CommandTemplate
 
 COPY = CommandTemplate(
     "copy {src} {dst} [vrf {vrf}]",
@@ -16,17 +15,19 @@
                 "yes", logger
             ),
             r"\s+[Vv][Rr][Ff]\s+": lambda session, logger: session.send_line(
                 "", logger
             ),
         }
     ),
-    error_map=OrderedDict(
-        [(r"permission\s*denied", "Failed to save configuration: Permission Denied")]
-    ),
+    error_map={
+        r"permission\s*denied": "Failed to save configuration: Permission " "Denied",
+        r"invalid\s*input": "Failed to save configuration: Invalid input",
+        r"\S+isk\d+://scp://": "SCP is no longer supported by IOS-XR",
+    },
 )
 
 DEL = CommandTemplate(
     "del {target}",
     action_map=OrderedDict(
         {
             "[confirm]": lambda session, logger: session.send_line("", logger),
```

## Comparing `cloudshell-networking-cisco-6.1.4/cloudshell/networking/cisco/command_templates/add_remove_vlan.py` & `cloudshell-networking-cisco-7.0.0/cloudshell/networking/cisco/command_templates/add_remove_vlan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 
 from collections import OrderedDict
 from copy import copy
 
 from cloudshell.cli.command_template.command_template import CommandTemplate
 
 ACTION_MAP = OrderedDict(
```

