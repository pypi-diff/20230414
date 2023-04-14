# Comparing `tmp/kintree-1.0.0b2.tar.gz` & `tmp/kintree-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kintree-1.0.0b2.tar", max compression
+gzip compressed data, was "kintree-1.0.0rc0.tar", max compression
```

## Comparing `kintree-1.0.0b2.tar` & `kintree-1.0.0rc0.tar`

### file list

```diff
@@ -1,81 +1,79 @@
--rw-r--r--   0        0        0    35149 2023-03-23 22:01:27.824862 kintree-1.0.0b2/LICENSE
--rw-r--r--   0        0        0    15652 2023-03-23 22:01:27.828862 kintree-1.0.0b2/README.md
--rw-r--r--   0        0        0       24 2023-03-23 22:01:27.940862 kintree-1.0.0b2/kintree/__init__.py
--rw-r--r--   0        0        0     5304 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/common/part_tools.py
--rw-r--r--   0        0        0     1214 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/common/progress.py
--rw-r--r--   0        0        0     4852 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/common/tools.py
--rw-r--r--   0        0        0    15164 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/config_interface.py
--rw-r--r--   0        0        0       47 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/digikey/digikey_api.yaml
--rw-r--r--   0        0        0     2745 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/digikey/digikey_categories.yaml
--rw-r--r--   0        0        0      229 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/digikey/digikey_config.yaml
--rw-r--r--   0        0        0     5604 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/digikey/digikey_parameters.yaml
--rw-r--r--   0        0        0       99 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/element14/element14_api.yaml
--rw-r--r--   0        0        0      225 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/element14/element14_config.yaml
--rw-r--r--   0        0        0     1633 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/categories.yaml
--rw-r--r--   0        0        0       57 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/inventree_dev.yaml
--rw-r--r--   0        0        0       57 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/inventree_prod.yaml
--rw-r--r--   0        0        0     1019 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/parameters.yaml
--rw-r--r--   0        0        0      553 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/parameters_filters.yaml
--rw-r--r--   0        0        0     5710 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/supplier_parameters.yaml
--rw-r--r--   0        0        0      235 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/inventree/suppliers.yaml
--rw-r--r--   0        0        0       95 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/kicad/kicad.yaml
--rw-r--r--   0        0        0     1161 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/kicad/kicad_map.yaml
--rw-r--r--   0        0        0       68 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/lcsc/lcsc_api.yaml
--rw-r--r--   0        0        0      237 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/lcsc/lcsc_config.yaml
--rw-r--r--   0        0        0       25 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/mouser/mouser_api.yaml
--rw-r--r--   0        0        0      239 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/mouser/mouser_config.yaml
--rw-r--r--   0        0        0    11228 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/settings.py
--rw-r--r--   0        0        0      199 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/user/general.yaml
--rw-r--r--   0        0        0      183 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/user/internal_part_number.yaml
--rw-r--r--   0        0        0       73 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/config/user/search_api.yaml
--rw-r--r--   0        0        0    21057 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/database/inventree_api.py
--rw-r--r--   0        0        0    32674 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/database/inventree_interface.py
--rw-r--r--   0        0        0     3276 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/gui/gui.py
--rw-r--r--   0        0        0    14401 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/gui/views/common.py
--rw-r--r--   0        0        0    50105 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/gui/views/main.py
--rw-r--r--   0        0        0    31898 2023-03-23 22:01:27.832862 kintree-1.0.0b2/kintree/gui/views/settings.py
--rw-r--r--   0        0        0        0 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/__init__.py
--rw-r--r--   0        0        0      569 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/kicad_interface.py
--rw-r--r--   0        0        0     4752 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/kicad_symbol.py
--rw-r--r--   0        0        0    37839 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/lib_utils/kicad_sym.py
--rw-r--r--   0        0        0     6794 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/lib_utils/sexpr.py
--rw-r--r--   0        0        0     7048 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/LICENSE
--rw-r--r--   0        0        0     3275 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/capacitor-polarized.kicad_sym
--rw-r--r--   0        0        0     2960 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/capacitor.kicad_sym
--rw-r--r--   0        0        0     1152 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/connector.kicad_sym
--rw-r--r--   0        0        0     2698 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/crystal-2p.kicad_sym
--rw-r--r--   0        0        0     1154 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/default.kicad_sym
--rw-r--r--   0        0        0     2789 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/diode-led.kicad_sym
--rw-r--r--   0        0        0     2587 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/diode-schottky.kicad_sym
--rw-r--r--   0        0        0     2369 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/diode-standard.kicad_sym
--rw-r--r--   0        0        0     2579 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/diode-zener.kicad_sym
--rw-r--r--   0        0        0     2195 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/eeprom-sot23.kicad_sym
--rw-r--r--   0        0        0     2587 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/ferrite-bead.kicad_sym
--rw-r--r--   0        0        0     2389 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/fuse.kicad_sym
--rw-r--r--   0        0        0     2400 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/inductor.kicad_sym
--rw-r--r--   0        0        0     1152 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/integrated-circuit.kicad_sym
--rw-r--r--   0        0        0       65 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/library_template.kicad_sym
--rw-r--r--   0        0        0     2234 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/oscillator-4p.kicad_sym
--rw-r--r--   0        0        0     2585 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/protection-unidir.kicad_sym
--rw-r--r--   0        0        0     2335 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/resistor-sm.kicad_sym
--rw-r--r--   0        0        0     2335 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/resistor.kicad_sym
--rw-r--r--   0        0        0     4993 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/transistor-nfet.kicad_sym
--rw-r--r--   0        0        0     2945 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/transistor-npn.kicad_sym
--rw-r--r--   0        0        0     5328 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/transistor-pfet.kicad_sym
--rw-r--r--   0        0        0     2950 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates/transistor-pnp.kicad_sym
--rw-r--r--   0        0        0       51 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates_project/templates_project.kicad_pcb
--rw-r--r--   0        0        0     1151 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates_project/templates_project.kicad_prl
--rw-r--r--   0        0        0     1903 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates_project/templates_project.kicad_pro
--rw-r--r--   0        0        0      105 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kicad/templates_project/templates_project.kicad_sch
--rw-r--r--   0        0        0      227 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kintree_gui.py
--rw-r--r--   0        0        0    67605 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/kintree_gui_0.6.x.py
--rw-r--r--   0        0        0    38788 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/logo.png
--rw-r--r--   0        0        0     5988 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/digikey_api.py
--rw-r--r--   0        0        0     9274 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/element14_api.py
--rw-r--r--   0        0        0     3165 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/lcsc_api.py
--rw-r--r--   0        0        0     3383 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/mouser_api.py
--rw-r--r--   0        0        0     1243 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/search_api.py
--rw-r--r--   0        0        0     4013 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/search/snapeda_api.py
--rw-r--r--   0        0        0     2028 2023-03-23 22:01:27.836862 kintree-1.0.0b2/kintree/setup_inventree.py
--rw-r--r--   0        0        0      984 2023-03-23 22:01:27.940862 kintree-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    16843 1970-01-01 00:00:00.000000 kintree-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-29 19:46:31.216390 kintree-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0    14494 2023-03-29 19:46:31.216390 kintree-1.0.0rc0/README.md
+-rw-r--r--   0        0        0       24 2023-03-29 19:46:31.324392 kintree-1.0.0rc0/kintree/__init__.py
+-rw-r--r--   0        0        0     5304 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/part_tools.py
+-rw-r--r--   0        0        0     1214 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/progress.py
+-rw-r--r--   0        0        0     4852 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/tools.py
+-rw-r--r--   0        0        0    15164 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/config_interface.py
+-rw-r--r--   0        0        0       47 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_api.yaml
+-rw-r--r--   0        0        0     2745 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_categories.yaml
+-rw-r--r--   0        0        0      229 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_config.yaml
+-rw-r--r--   0        0        0     5604 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_parameters.yaml
+-rw-r--r--   0        0        0       99 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/element14/element14_api.yaml
+-rw-r--r--   0        0        0      225 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/element14/element14_config.yaml
+-rw-r--r--   0        0        0     1633 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/categories.yaml
+-rw-r--r--   0        0        0       57 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/inventree_dev.yaml
+-rw-r--r--   0        0        0       57 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/inventree_prod.yaml
+-rw-r--r--   0        0        0     1019 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/parameters.yaml
+-rw-r--r--   0        0        0      553 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/parameters_filters.yaml
+-rw-r--r--   0        0        0     5710 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/supplier_parameters.yaml
+-rw-r--r--   0        0        0      235 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/suppliers.yaml
+-rw-r--r--   0        0        0       95 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/kicad/kicad.yaml
+-rw-r--r--   0        0        0     1161 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/kicad/kicad_map.yaml
+-rw-r--r--   0        0        0       68 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/lcsc/lcsc_api.yaml
+-rw-r--r--   0        0        0      237 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/lcsc/lcsc_config.yaml
+-rw-r--r--   0        0        0       25 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/mouser/mouser_api.yaml
+-rw-r--r--   0        0        0      239 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/mouser/mouser_config.yaml
+-rw-r--r--   0        0        0    11228 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/settings.py
+-rw-r--r--   0        0        0      199 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/general.yaml
+-rw-r--r--   0        0        0      183 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/internal_part_number.yaml
+-rw-r--r--   0        0        0       73 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/search_api.yaml
+-rw-r--r--   0        0        0    21057 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/database/inventree_api.py
+-rw-r--r--   0        0        0    32757 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/database/inventree_interface.py
+-rw-r--r--   0        0        0     3276 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/gui.py
+-rw-r--r--   0        0        0    14401 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/common.py
+-rw-r--r--   0        0        0    50767 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/main.py
+-rw-r--r--   0        0        0    31898 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/settings.py
+-rw-r--r--   0        0        0        0 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/__init__.py
+-rw-r--r--   0        0        0      569 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/kicad_interface.py
+-rw-r--r--   0        0        0     4752 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/kicad_symbol.py
+-rw-r--r--   0        0        0     7048 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/LICENSE
+-rw-r--r--   0        0        0     3077 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/capacitor-polarized.kicad_sym
+-rw-r--r--   0        0        0     2786 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/capacitor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/connector.kicad_sym
+-rw-r--r--   0        0        0     2540 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/crystal-2p.kicad_sym
+-rw-r--r--   0        0        0     1091 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/default.kicad_sym
+-rw-r--r--   0        0        0     2647 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-led.kicad_sym
+-rw-r--r--   0        0        0     2453 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-schottky.kicad_sym
+-rw-r--r--   0        0        0     2251 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-standard.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-zener.kicad_sym
+-rw-r--r--   0        0        0     2116 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/eeprom-sot23.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/ferrite-bead.kicad_sym
+-rw-r--r--   0        0        0     2249 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/fuse.kicad_sym
+-rw-r--r--   0        0        0     2258 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/inductor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/integrated-circuit.kicad_sym
+-rw-r--r--   0        0        0       65 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/library_template.kicad_sym
+-rw-r--r--   0        0        0     2140 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/oscillator-4p.kicad_sym
+-rw-r--r--   0        0        0     2451 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/protection-unidir.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/resistor-sm.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/resistor.kicad_sym
+-rw-r--r--   0        0        0     4683 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-nfet.kicad_sym
+-rw-r--r--   0        0        0     2795 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-npn.kicad_sym
+-rw-r--r--   0        0        0     4986 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-pfet.kicad_sym
+-rw-r--r--   0        0        0     2800 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-pnp.kicad_sym
+-rw-r--r--   0        0        0     1981 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pcb
+-rw-r--r--   0        0        0     1201 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_prl
+-rw-r--r--   0        0        0     6077 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pro
+-rw-r--r--   0        0        0      187 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_sch
+-rw-r--r--   0        0        0      227 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kintree_gui.py
+-rw-r--r--   0        0        0    67605 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kintree_gui_0.6.x.py
+-rw-r--r--   0        0        0    38788 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/logo.png
+-rw-r--r--   0        0        0     5988 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/digikey_api.py
+-rw-r--r--   0        0        0     9274 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/element14_api.py
+-rw-r--r--   0        0        0     3165 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/lcsc_api.py
+-rw-r--r--   0        0        0     3383 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/mouser_api.py
+-rw-r--r--   0        0        0     1243 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/search_api.py
+-rw-r--r--   0        0        0     4013 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/snapeda_api.py
+-rw-r--r--   0        0        0     2028 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/setup_inventree.py
+-rw-r--r--   0        0        0      985 2023-03-29 19:46:31.324392 kintree-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    15687 1970-01-01 00:00:00.000000 kintree-1.0.0rc0/PKG-INFO
```

### Comparing `kintree-1.0.0b2/LICENSE` & `kintree-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/README.md` & `kintree-1.0.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# Ki-nTree
-### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.readthedocs.io/) 
+# <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
+### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
 ## New version (1.0) is coming soon!
 
-To install the beta release:
+To install the release candidate:
 ``` shell
 pip install --pre -U kintree
 ```
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_preview.png" width="auto" height="auto">
+<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
 ## Demo Videos :fast_forward: [Full Demo](https://youtu.be/haSAu926BOI) :fast_forward: [KiCad Demo](https://youtu.be/NSMfCCD0uVw)
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_example.png"  width="auto" height="auto">
-
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
 * automate part creation of InvenTree parts
 * synchronize parts data between KiCad and InvenTree
 
 Ki-nTree works with:
 - [Digi-Key](https://developer.digikey.com/), [Mouser](https://www.mouser.com/api-hub/), [Element14](https://partner.element14.com/docs) and [LCSC](https://lcsc.com/) **enormous** part databases and free APIs
-- the awesome open-source [Digi-Key API python library](https://github.com/peeter123/digikey-api) built and maintained by [@peeter123](https://github.com/peeter123)
+- the awesome open-source [InvenTree Inventory Management System](https://github.com/inventree/inventree) built and maintained by [@SchrodingersGat](https://github.com/SchrodingersGat) and [@matmair](https://github.com/matmair)
+- the reliable and SCM-friendly KiCad file parser [KiUtils](https://github.com/mvnmgrx/kiutils) built and maintained by [@mvnmgrx](https://github.com/mvnmgrx)
+- the amazing [Digi-Key API python library](https://github.com/peeter123/digikey-api) built and maintained by [@peeter123](https://github.com/peeter123)
 - the [Mouser Python API](https://github.com/sparkmicro/mouser-api/) built and maintained by [@eeintech](https://github.com/eeintech)
-- the awesome open-source [InvenTree Inventory Management System](https://github.com/inventree/inventree) built and maintained by [@SchrodingersGat](https://github.com/SchrodingersGat)
-- [KiCad](https://www.kicad.org/) (of course!) and their open-source [library utils](https://gitlab.com/kicad/libraries/kicad-library-utils)
 
-> **Important Note**
+> :warning: **Important Note**
+>
+> Ki-nTree version `1.0.x` and forward support KiCad versions **6 and up**.
+>
+> Ki-nTree versions `0.5.x` and `0.6.x` only support KiCad version **6** (`pip install kintree==0.6.6`).
 >
-> Because of limited maintenance bandwidth, Ki-nTree versions `0.5.x` and newer will only support KiCad version **6**.
-> To keep using Ki-nTree with KiCad version **5**, use older `0.4.x` versions (`pip install kintree==0.4.8`).
+> To use with KiCad version **5**, use older Ki-nTree `0.4.x` versions (`pip install kintree==0.4.8`).
 
 Ki-nTree was developped by [@eeintech](https://github.com/eeintech) for [SPARK Microsystems](https://www.sparkmicro.com/), who generously accepted to make it open-source!
 
 ## Get Started
 
 ### Requirements
 
@@ -88,16 +89,14 @@
 ### Packages
 #### Arch Linux
 
 Ki-nTree is [available on Arch Linux's AUR](https://aur.archlinux.org/packages/python-kintree/) as `python-kintree`.
 
 ### Usage Instructions
 
-> :warning: Warning: **KiCad library writer is still in development**: Make sure to open KiCad libraries inside the symbol editor and save them after adding symbols.
-
 #### Before Starting
 
 If you intend to use Ki-nTree with InvenTree, this tool offers to setup the InvenTree category tree with a simple script that you can run as follow:
 
 > :warning: Warning: Before running it, make sure you have setup your category tree in your `categories.yaml` configuration file according to your own preferences, else it will use the [default setup](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/categories.yaml).
 
 ``` bash
@@ -106,42 +105,42 @@
 
 If the InvenTree category tree is **not setup** before starting to use Ki-nTree, you **won't be able to add parts** to InvenTree.
 
 #### Advanced Configuration
 
 Configuration files are stored in the folder pointed by the `Configuration Files Folder` path in the "User Settings" window:
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/settings_user_cache.png" width="600" height="auto">
+<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_settings_user.png" width="600" height="auto">
 
 
 <details>
 <summary><b>Click here to read about configuration files</b></summary>
 <p>
 
 Ki-nTree uses a number of YAML configuration files to function. New users shouldn't need to worry about them to try out Ki-nTree (except for `categories.yaml` as mentioned in the previous section), however they can be modified to customize behavior and workflow.
 
 Below is a summary table of the different configuration files, their function and if they are updated by the GUI:
 | Filename | Function | GUI Update? |
 | --- | --- | --- |
 | `categories.yaml` | InvenTree categories hierarchy tree and category codes for IPN generation (see [Before Starting section](#before-starting)) | :x: |
-| `general.yaml` | General user settings | _Partial_ |
-| `internal_part_number.yaml` | Controls for IPN generation | :x: |
+| `general.yaml` | General user settings | :heavy_check_mark: |
+| `internal_part_number.yaml` | Controls for IPN generation | :heavy_check_mark: |
 | `inventree_<env>.yaml` | InvenTree login credentials, per environment (`<env>=['dev', 'prod']`) | :heavy_check_mark: |
 | `kicad.yaml` | KiCad symbol, footprint and library paths | :heavy_check_mark: |
 | `kicad_map.yaml` | Mapping between InvenTree parent categories and KiCad symbol/footprint libraries and templates | :x: |
 | `parameters.yaml` | List of InvenTree parameters templates (see [InvenTree Part Parameters documentation](https://docs.inventree.org/en/latest/part/parameter/)) | :x: |
 | `parameters_filters.yaml` | Mapping between InvenTree parent categories and InvenTree parameters templates | :x: |
-| `search_api.yaml` | Generic controls for Supplier search APIs like cache validity and category matching ratio | :x: |
+| `search_api.yaml` | Generic controls for Supplier search APIs like cache validity | :heavy_check_mark: |
 | `supplier_parameters.yaml` | Mapping between InvenTree parameters templates and suppliers parameters/attributes, sorted by InvenTree parent categories (see [Part Parameters section](#part-parameters)) | :x: |
 | `<supplier>_config.yaml` | Mapping for supplier name and search results fields, to overwrite defaults (`<supplier>=['digikey', 'element14', 'lcsc', 'mouser']`) | :x: |
 | `<supplier>_api.yaml` | Required supplier API fields, custom to each supplier (`<supplier>=['digikey', 'element14', 'lcsc', 'mouser']`) | :heavy_check_mark: |
-| `digikey_categories.yaml` | Mapping between InvenTree categories and Digi-Key categories | :heavy_check_mark: |
+| `digikey_categories.yaml` | Mapping between InvenTree categories and Digi-Key categories | :x: |
 | `digikey_parameters.yaml` | Mapping between InvenTree parameters and Digi-Key parameters/attributes | :x: |
 
-> In versions `0.6.x` and older, Ki-nTree only supports matching between InvenTree and Digi-Key categories and parameters/attibutes (help wanted!)
+> Ki-nTree only supports matching between InvenTree and Digi-Key categories and parameters/attibutes (help wanted!)
 
 </p>
 </details>
 
 #### InvenTree Permissions
 
 Each InvenTree user has a set of permissions associated to them.
@@ -226,15 +225,15 @@
 ```
 
 2. Install the requirements into a `poetry`-managed virtual environment
 ``` bash
 poetry install
 Installing dependencies from lock file
 ...
-Installing the current project: kintree (0.4.99)
+Installing the current project: kintree (1.0.99)
 ```
 > Note: the version is not accurate (placeholder only)
 
 3. Run Ki-nTree in the virtual environment
 ```bash
 poetry run python -m kintree_gui
 ```
@@ -245,53 +244,32 @@
 $ python -m kintree_gui
 ```
 
 #### Build
 1. Make sure you followed the previous installation steps, then run:
 ``` bash
 $ poetry build
-Building kintree (0.6.99)
+Building kintree (1.0.99)
   - Building sdist
-  - Built kintree-0.6.99.tar.gz
+  - Built kintree-1.0.99.tar.gz
   - Building wheel
-  - Built kintree-0.6.99-py3-none-any.whl
+  - Built kintree-1.0.99-py3-none-any.whl
 ```
 2. Exit the virtual environment (`Ctrl + D` on Linux; you can also close the
    terminal and reopen it in the same folder).
 
    Run `pip install dist/<wheel_file>.whl` with the file name from the previous
    step. For example:
 
 ```bash
-pip install dist/kintree-0.6.99-py3-none-any.whl
+pip install dist/kintree-1.0.99-py3-none-any.whl
 ```
 
 3. You can now start Ki-nTree by typing `kintree` in the terminal, provided
    that your python dist path is a part of your `$PATH`.
 
-## Roadmap
-
-> Priority goes to implementing new features over GUI improvements  
-> Open to new ideas and pull requests :smiley:
-
-#### Versions 1.0.x or later
-(Strikethrough items are supported in V1.0.0 beta1 release)
-
-##### New Features
-~~- Revamp category selection based on hierarchical structure from InvenTree ([reference](https://github.com/sparkmicro/Ki-nTree/issues/87))~~  
-~~- Allow user to decide the category code to use for IPN~~  
-~~- Enable option to download and save PDF files locally/to internal server storage~~
-
-##### Improvements
-~~- Optimize the category search ([reference](https://github.com/sparkmicro/Ki-nTree/issues/104))~~  
-~~- Migrate KiCad library management to [KiUtils](https://github.com/mvnmgrx/kiutils) ([reference](https://github.com/sparkmicro/Ki-nTree/issues/119))~~  
-- Add support for KiCad V7 ([reference](https://github.com/sparkmicro/Ki-nTree/issues/120))
-
-##### GUI
-~~- Migrate to [Flet](https://github.com/flet-dev/flet) ([reference](https://github.com/sparkmicro/Ki-nTree/issues/37))~~
-
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
-* https://gitlab.com/kicad/libraries/kicad-library-utils
+* https://github.com/mvnmgrx/kiutils
 * https://github.com/peeter123/digikey-api
 
 The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
```

### Comparing `kintree-1.0.0b2/kintree/common/part_tools.py` & `kintree-1.0.0rc0/kintree/common/part_tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/common/progress.py` & `kintree-1.0.0rc0/kintree/common/progress.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/common/tools.py` & `kintree-1.0.0rc0/kintree/common/tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/config_interface.py` & `kintree-1.0.0rc0/kintree/config/config_interface.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/digikey/digikey_categories.yaml` & `kintree-1.0.0rc0/kintree/config/digikey/digikey_categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/digikey/digikey_parameters.yaml` & `kintree-1.0.0rc0/kintree/config/digikey/digikey_parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/inventree/categories.yaml` & `kintree-1.0.0rc0/kintree/config/inventree/categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/inventree/parameters.yaml` & `kintree-1.0.0rc0/kintree/config/inventree/parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/inventree/parameters_filters.yaml` & `kintree-1.0.0rc0/kintree/config/inventree/parameters_filters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/inventree/supplier_parameters.yaml` & `kintree-1.0.0rc0/kintree/config/inventree/supplier_parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/kicad/kicad_map.yaml` & `kintree-1.0.0rc0/kintree/config/kicad/kicad_map.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/config/settings.py` & `kintree-1.0.0rc0/kintree/config/settings.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/database/inventree_api.py` & `kintree-1.0.0rc0/kintree/database/inventree_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/database/inventree_interface.py` & `kintree-1.0.0rc0/kintree/database/inventree_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,28 +255,35 @@
     # Replace whitespaces in URL
     inventree_part['supplier_link'] = part_info['supplier_link'].replace(' ', '%20')
     inventree_part['datasheet'] = part_info['datasheet'].replace(' ', '%20')
     # Image URL is not shown to user so force default key/value
     inventree_part['image'] = part_info['image'].replace(' ', '%20')
 
     # Load parameters map
-    parameter_map = config_interface.load_category_parameters(category=category_tree[0],
-                                                              supplier_config_path=settings.CONFIG_SUPPLIER_PARAMETERS, )
+    if category_tree:
+        parameter_map = config_interface.load_category_parameters(
+            category=category_tree[0],
+            supplier_config_path=settings.CONFIG_SUPPLIER_PARAMETERS,
+        )
+    else:
+        cprint('[INFO]\tWarning: Parameter map not loaded (no category selected)', silent=settings.SILENT)
 
     if not is_custom:
         # Add Parameters
         if parameter_map:
             for supplier_param, inventree_param in parameter_map.items():
                 # Some parameters may not be mapped
                 if inventree_param not in inventree_part['parameters'].keys():
                     if supplier_param != 'Manufacturer Part Number':
                         try:
-                            parameter_value = part_tools.clean_parameter_value(category=category_tree[0],
-                                                                               name=supplier_param,
-                                                                               value=part_info['parameters'][supplier_param])
+                            parameter_value = part_tools.clean_parameter_value(
+                                category=category_tree[0],
+                                name=supplier_param,
+                                value=part_info['parameters'][supplier_param],
+                            )
                             inventree_part['parameters'][inventree_param] = parameter_value
                         except:
                             cprint(f'[INFO]\tWarning: Parameter "{supplier_param}" not found in supplier data', silent=settings.SILENT)
                     else:
                         inventree_part['parameters'][inventree_param] = part_info['manufacturer_part_number']
 
             # Check for missing parameters and fill value with dash
```

### Comparing `kintree-1.0.0b2/kintree/gui/gui.py` & `kintree-1.0.0rc0/kintree/gui/gui.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/gui/views/common.py` & `kintree-1.0.0rc0/kintree/gui/views/common.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/gui/views/main.py` & `kintree-1.0.0rc0/kintree/gui/views/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1234,26 +1234,38 @@
             self.fields['inventree_progress'].update()
 
         if not self.create_continue:
             return self.process_cancel()
 
         # KiCad data processing
         if settings.ENABLE_KICAD and not settings.ENABLE_ALTERNATE:
+            # Store "pseudo-category" as re-used in multiple places
+            pseudo_category = symbol.split(':')[0]
+            # Translate part info if InvenTree not enabled
+            if not settings.ENABLE_INVENTREE:
+                part_info = inventree_interface.translate_form_to_inventree(
+                    part_info=part_info,
+                    category_tree=[pseudo_category],
+                    is_custom=custom,
+                )
+                # Also add datasheet URL as part page URL
+                part_info['inventree_url'] = part_info['datasheet']
             part_info['Symbol'] = symbol
             part_info['Template'] = template.split('/')
             part_info['Footprint'] = footprint
 
             symbol_library_path = os.path.join(
                 settings.KICAD_SETTINGS['KICAD_SYMBOLS_PATH'],
-                f'{symbol.split(":")[0]}.kicad_sym',
+                f'{pseudo_category}.kicad_sym',
             )
 
             # Reset progress
             progress.CREATE_PART_PROGRESS = 0
-            # Create part
+            # Add part symbol to KiCAD
+            cprint('\n[MAIN]\tAdding part to KiCad', silent=settings.SILENT)
             kicad_success, kicad_new_part = kicad_interface.inventree_to_kicad(
                 part_data=part_info,
                 library_path=symbol_library_path,
                 show_progress=self.fields['kicad_progress'],
             )
             # print(kicad_success, kicad_new_part)
```

### Comparing `kintree-1.0.0b2/kintree/gui/views/settings.py` & `kintree-1.0.0rc0/kintree/gui/views/settings.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/kicad/kicad_interface.py` & `kintree-1.0.0rc0/kintree/kicad/kicad_interface.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/kicad/kicad_symbol.py` & `kintree-1.0.0rc0/kintree/kicad/kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/LICENSE` & `kintree-1.0.0rc0/kintree/kicad/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/capacitor-polarized.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/protection-unidir.kicad_sym`

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,154 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2243 2220 2869  eference" "C" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 312e 3433   1) (at 0 -11.43
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d31 392e 3035   2) (at 0 -19.05
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 312e 3539 2030 290a 2020 2020 2020 2865  1.59 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 332e 3937 2030 290a 2020  t 0 -13.97 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3136  (id 5) (at 0 -16
-00000300: 2e35 3120 3029 0a20 2020 2020 2028 6566  .51 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2243 6170 6163 6974  roperty "Capacit
-00000350: 616e 6365 2028 4661 7261 6429 2220 2256  ance (Farad)" "V
-00000360: 616c 7565 2220 2869 6420 3629 2028 6174  alue" (id 6) (at
-00000370: 2030 202d 332e 3831 2030 290a 2020 2020   0 -3.81 0).    
-00000380: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000390: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-000003a0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
-000003b0: 726f 7065 7274 7920 2254 6f6c 6572 616e  roperty "Toleran
-000003c0: 6365 2028 2529 2220 2254 6f6c 6572 616e  ce (%)" "Toleran
-000003d0: 6365 2220 2869 6420 3729 2028 6174 2035  ce" (id 7) (at 5
-000003e0: 2e30 3820 2d33 2e38 3120 3029 0a20 2020  .08 -3.81 0).   
-000003f0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-00000400: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000410: 3729 2920 286a 7573 7469 6679 206c 6566  7)) (justify lef
-00000420: 7429 2068 6964 6529 0a20 2020 2029 0a20  t) hide).    ). 
-00000430: 2020 2028 7072 6f70 6572 7479 2022 566f     (property "Vo
-00000440: 6c74 6167 6520 5261 7465 6420 2856 6f6c  ltage Rated (Vol
-00000450: 7429 2220 2252 6174 6564 2056 6f6c 7461  t)" "Rated Volta
-00000460: 6765 2220 2869 6420 3829 2028 6174 2030  ge" (id 8) (at 0
-00000470: 202d 362e 3335 2030 290a 2020 2020 2020   -6.35 0).      
-00000480: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000490: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-000004a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000004b0: 7065 7274 7920 2250 6163 6b61 6765 2054  perty "Package T
-000004c0: 7970 6522 2022 5061 636b 6167 6520 5479  ype" "Package Ty
-000004d0: 7065 2220 2869 6420 3929 2028 6174 2030  pe" (id 9) (at 0
-000004e0: 202d 382e 3839 2030 290a 2020 2020 2020   -8.89 0).      
-000004f0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000500: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000510: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000520: 7065 7274 7920 2250 6163 6b61 6765 2053  perty "Package S
-00000530: 697a 6522 2022 5061 636b 6167 6520 5369  ize" "Package Si
-00000540: 7a65 2220 2869 6420 3130 2920 2861 7420  ze" (id 10) (at 
-00000550: 3020 2d38 2e38 3920 3029 0a20 2020 2020  0 -8.89 0).     
-00000560: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000570: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000580: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
-00000590: 2020 2870 726f 7065 7274 7920 2245 5352    (property "ESR
-000005a0: 2028 4f68 6d29 2220 2245 5352 2220 2869   (Ohm)" "ESR" (i
-000005b0: 6420 3131 2920 2861 7420 352e 3038 202d  d 11) (at 5.08 -
-000005c0: 362e 3335 2030 290a 2020 2020 2020 2865  6.35 0).      (e
-000005d0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-000005e0: 7a65 2031 2e32 3720 312e 3237 2929 2028  ze 1.27 1.27)) (
-000005f0: 6a75 7374 6966 7920 6c65 6674 2920 6869  justify left) hi
-00000600: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000610: 726f 7065 7274 7920 226b 695f 6b65 7977  roperty "ki_keyw
-00000620: 6f72 6473 2220 226b 6579 776f 7264 7322  ords" "keywords"
-00000630: 2028 6964 2031 3229 2028 6174 2030 2030   (id 12) (at 0 0
-00000640: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000650: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000660: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000670: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000680: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
-00000690: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
-000006a0: 6f6e 2220 2869 6420 3133 2920 2861 7420  on" (id 13) (at 
-000006b0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-000006c0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000006d0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-000006e0: 6465 290a 2020 2020 290a 2020 2020 2873  de).    ).    (s
-000006f0: 796d 626f 6c20 2249 504e 5f30 5f31 220a  ymbol "IPN_0_1".
-00000700: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000710: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-00000720: 2020 2020 2020 2028 7879 202d 312e 3737         (xy -1.77
-00000730: 3820 2d30 2e33 3831 290a 2020 2020 2020  8 -0.381).      
-00000740: 2020 2020 2878 7920 2d31 2e37 3738 202d      (xy -1.778 -
-00000750: 312e 3635 3129 0a20 2020 2020 2020 2029  1.651).        )
-00000760: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
-00000770: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
-00000780: 2064 6566 6175 6c74 2920 2863 6f6c 6f72   default) (color
-00000790: 2030 2030 2030 2030 2929 0a20 2020 2020   0 0 0 0)).     
-000007a0: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
-000007b0: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
-000007c0: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
-000007d0: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
-000007e0: 2020 2020 2028 7879 202d 312e 3237 2030       (xy -1.27 0
-000007f0: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
-00000800: 2d30 2e36 3335 2030 290a 2020 2020 2020  -0.635 0).      
-00000810: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
-00000820: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
-00000830: 7970 6520 6465 6661 756c 7429 2028 636f  ype default) (co
-00000840: 6c6f 7220 3020 3020 3020 3029 290a 2020  lor 0 0 0 0)).  
-00000850: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
-00000860: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
-00000870: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-00000880: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-00000890: 2020 2020 2020 2020 2878 7920 2d31 2e31          (xy -1.1
-000008a0: 3433 202d 312e 3031 3629 0a20 2020 2020  43 -1.016).     
-000008b0: 2020 2020 2028 7879 202d 322e 3431 3320       (xy -2.413 
-000008c0: 2d31 2e30 3136 290a 2020 2020 2020 2020  -1.016).        
-000008d0: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
-000008e0: 6520 2877 6964 7468 2030 2920 2874 7970  e (width 0) (typ
-000008f0: 6520 6465 6661 756c 7429 2028 636f 6c6f  e default) (colo
-00000900: 7220 3020 3020 3020 3029 290a 2020 2020  r 0 0 0 0)).    
-00000910: 2020 2020 2866 696c 6c20 2874 7970 6520      (fill (type 
-00000920: 6e6f 6e65 2929 0a20 2020 2020 2029 0a20  none)).      ). 
-00000930: 2020 2020 2028 706f 6c79 6c69 6e65 0a20       (polyline. 
-00000940: 2020 2020 2020 2028 7074 730a 2020 2020         (pts.    
-00000950: 2020 2020 2020 2878 7920 2d30 2e36 3335        (xy -0.635
-00000960: 202d 312e 3930 3529 0a20 2020 2020 2020   -1.905).       
-00000970: 2020 2028 7879 202d 302e 3633 3520 312e     (xy -0.635 1.
-00000980: 3930 3529 0a20 2020 2020 2020 2029 0a20  905).        ). 
-00000990: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-000009a0: 7769 6474 6820 302e 3235 3429 2028 7479  width 0.254) (ty
-000009b0: 7065 2064 6566 6175 6c74 2920 2863 6f6c  pe default) (col
-000009c0: 6f72 2030 2030 2030 2030 2929 0a20 2020  or 0 0 0 0)).   
-000009d0: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
-000009e0: 206e 6f6e 6529 290a 2020 2020 2020 290a   none)).      ).
-000009f0: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000a00: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-00000a10: 2020 2020 2020 2028 7879 2031 2e35 3234         (xy 1.524
-00000a20: 2030 290a 2020 2020 2020 2020 2020 2878   0).          (x
-00000a30: 7920 302e 3633 3520 3029 0a20 2020 2020  y 0.635 0).     
-00000a40: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
-00000a50: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
-00000a60: 7479 7065 2064 6566 6175 6c74 2920 2863  type default) (c
-00000a70: 6f6c 6f72 2030 2030 2030 2030 2929 0a20  olor 0 0 0 0)). 
-00000a80: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
-00000a90: 7065 206e 6f6e 6529 290a 2020 2020 2020  pe none)).      
-00000aa0: 290a 2020 2020 2020 2861 7263 2028 7374  ).      (arc (st
-00000ab0: 6172 7420 312e 3532 3420 312e 3930 3529  art 1.524 1.905)
-00000ac0: 2028 6d69 6420 302e 3833 3433 2030 2920   (mid 0.8343 0) 
-00000ad0: 2865 6e64 2031 2e35 3234 202d 312e 3930  (end 1.524 -1.90
-00000ae0: 3529 0a20 2020 2020 2020 2028 7374 726f  5).        (stro
-00000af0: 6b65 2028 7769 6474 6820 302e 3235 3429  ke (width 0.254)
-00000b00: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00000b10: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000b20: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000b30: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-00000b40: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
-00000b50: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
-00000b60: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
-00000b70: 7665 206c 696e 6520 2861 7420 2d33 2e38  ve line (at -3.8
-00000b80: 3120 3020 3029 2028 6c65 6e67 7468 2032  1 0 0) (length 2
-00000b90: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
-00000ba0: 6d65 2022 506f 7369 7469 6622 2028 6566  me "Positif" (ef
-00000bb0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000bc0: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-00000bd0: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-00000be0: 2231 2220 2865 6666 6563 7473 2028 666f  "1" (effects (fo
-00000bf0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000c00: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-00000c10: 2020 2020 2028 7069 6e20 7061 7373 6976       (pin passiv
-00000c20: 6520 6c69 6e65 2028 6174 2033 2e38 3120  e line (at 3.81 
-00000c30: 3020 3138 3029 2028 6c65 6e67 7468 2032  0 180) (length 2
-00000c40: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
-00000c50: 6d65 2022 4e65 6761 7469 6622 2028 6566  me "Negatif" (ef
-00000c60: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000c70: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-00000c80: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-00000c90: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
-00000ca0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000cb0: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-00000cc0: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2244 2220 2861  eference" "D" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 332e  "IPN" (at 0 -13.
+00000120: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3231 2e35 3920 3029 0a20  at 0 -21.59 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 342e 3133 2030 290a 2020 2020  0 -24.13 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3136 2e35 3120 3029 0a20 2020 2020   -16.51 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3139 2e30 3520 3029 0a20 2020   0 -19.05 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 3020 2d33 2e38 3120  ue" (at 0 -3.81 
+00000340: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000350: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000360: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
+00000370: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000380: 5374 616e 646f 6666 2056 6f6c 7461 6765  Standoff Voltage
+00000390: 2220 2253 7461 6e64 6f66 6620 566f 6c74  " "Standoff Volt
+000003a0: 6167 6522 2028 6174 2030 202d 362e 3335  age" (at 0 -6.35
+000003b0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
+000003c0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000003d0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
+000003e0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000003f0: 2242 7265 616b 646f 776e 2056 6f6c 7461  "Breakdown Volta
+00000400: 6765 2220 2242 7265 616b 646f 776e 2056  ge" "Breakdown V
+00000410: 6f6c 7461 6765 2220 2861 7420 3020 2d38  oltage" (at 0 -8
+00000420: 2e38 3920 3029 0a20 2020 2020 2028 6566  .89 0).      (ef
+00000430: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000440: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000450: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000460: 726f 7065 7274 7920 2250 6561 6b20 506f  roperty "Peak Po
+00000470: 7765 7220 2857 6174 7473 2922 2022 5261  wer (Watts)" "Ra
+00000480: 7465 6420 506f 7765 7222 2028 6174 2030  ted Power" (at 0
+00000490: 202d 3131 2e34 3320 3029 0a20 2020 2020   -11.43 0).     
+000004a0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000004b0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000004c0: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000004d0: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
+000004e0: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
+000004f0: 7264 7322 2028 6174 2030 2030 2030 290a  rds" (at 0 0 0).
+00000500: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000510: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000520: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000530: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+00000540: 2022 6b69 5f64 6573 6372 6970 7469 6f6e   "ki_description
+00000550: 2220 2264 6573 6372 6970 7469 6f6e 2220  " "description" 
+00000560: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
+00000570: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000580: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000590: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000005a0: 2020 2873 796d 626f 6c20 2249 504e 5f30    (symbol "IPN_0
+000005b0: 5f31 220a 2020 2020 2020 2870 6f6c 796c  _1".      (polyl
+000005c0: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
+000005d0: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
+000005e0: 2e32 3720 2d31 2e33 3937 290a 2020 2020  .27 -1.397).    
+000005f0: 2020 2020 2020 2878 7920 322e 3135 3920        (xy 2.159 
+00000600: 2d31 2e37 3738 290a 2020 2020 2020 2020  -1.778).        
+00000610: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
+00000620: 6520 2877 6964 7468 2030 2e32 3534 2920  e (width 0.254) 
+00000630: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+00000640: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+00000650: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+00000660: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+00000670: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+00000680: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
+00000690: 3237 202d 312e 3339 3729 0a20 2020 2020  27 -1.397).     
+000006a0: 2020 2020 2028 7879 2031 2e32 3720 312e       (xy 1.27 1.
+000006b0: 3339 3729 0a20 2020 2020 2020 2020 2028  397).          (
+000006c0: 7879 2030 2e33 3831 2031 2e37 3738 290a  xy 0.381 1.778).
+000006d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000006e0: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+000006f0: 2030 2e32 3534 2920 2874 7970 6520 6465   0.254) (type de
+00000700: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+00000710: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
+00000720: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+00000730: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
+00000740: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
+00000750: 2020 2878 7920 2d31 2e32 3720 312e 3237    (xy -1.27 1.27
+00000760: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000770: 2d31 2e32 3720 2d31 2e32 3729 0a20 2020  -1.27 -1.27).   
+00000780: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
+00000790: 3029 0a20 2020 2020 2020 2020 2028 7879  0).          (xy
+000007a0: 202d 312e 3237 2031 2e32 3729 0a20 2020   -1.27 1.27).   
+000007b0: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
+000007c0: 7374 726f 6b65 2028 7769 6474 6820 302e  stroke (width 0.
+000007d0: 3235 3429 2028 7479 7065 2064 6566 6175  254) (type defau
+000007e0: 6c74 2929 0a20 2020 2020 2020 2028 6669  lt)).        (fi
+000007f0: 6c6c 2028 7479 7065 2062 6163 6b67 726f  ll (type backgro
+00000800: 756e 6429 290a 2020 2020 2020 290a 2020  und)).      ).  
+00000810: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+00000820: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
+00000830: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+00000840: 6520 2861 7420 332e 3831 2030 2031 3830  e (at 3.81 0 180
+00000850: 2920 286c 656e 6774 6820 322e 3534 290a  ) (length 2.54).
+00000860: 2020 2020 2020 2020 286e 616d 6520 2243          (name "C
+00000870: 6174 686f 6465 2220 2865 6666 6563 7473  athode" (effects
+00000880: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000890: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+000008a0: 2020 2028 6e75 6d62 6572 2022 3122 2028     (number "1" (
+000008b0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000008c0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+000008d0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
+000008e0: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+000008f0: 6520 2861 7420 2d33 2e38 3120 3020 3029  e (at -3.81 0 0)
+00000900: 2028 6c65 6e67 7468 2032 2e35 3429 0a20   (length 2.54). 
+00000910: 2020 2020 2020 2028 6e61 6d65 2022 416e         (name "An
+00000920: 6f64 6522 2028 6566 6665 6374 7320 2866  ode" (effects (f
+00000930: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+00000940: 2e32 3729 2929 290a 2020 2020 2020 2020  .27)))).        
+00000950: 286e 756d 6265 7220 2232 2220 2865 6666  (number "2" (eff
+00000960: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000970: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
+00000980: 2020 2020 2029 0a20 2020 2029 0a20 2029       ).    ).  )
+00000990: 0a29 0a                                  .).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/capacitor.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/capacitor.kicad_sym`

 * *Files 10% similar despite different names*

```diff
@@ -1,185 +1,175 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2243 2220 2869  eference" "C" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 332e 3937   1) (at 0 -13.97
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 312e 3539   2) (at 0 -21.59
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 342e 3133 2030 290a 2020 2020 2020 2865  4.13 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3139  (id 5) (at 0 -19
-00000300: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2243 6170 6163 6974  roperty "Capacit
-00000350: 616e 6365 2028 4661 7261 6429 2220 2256  ance (Farad)" "V
-00000360: 616c 7565 2220 2869 6420 3629 2028 6174  alue" (id 6) (at
-00000370: 2030 202d 332e 3831 2030 290a 2020 2020   0 -3.81 0).    
-00000380: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000390: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-000003a0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
-000003b0: 726f 7065 7274 7920 2254 6f6c 6572 616e  roperty "Toleran
-000003c0: 6365 2028 2529 2220 2254 6f6c 6572 616e  ce (%)" "Toleran
-000003d0: 6365 2220 2869 6420 3729 2028 6174 2037  ce" (id 7) (at 7
-000003e0: 2e36 3220 2d33 2e38 3120 3029 0a20 2020  .62 -3.81 0).   
-000003f0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-00000400: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000410: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
-00000420: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-00000430: 6174 6564 2056 6f6c 7461 6765 2028 566f  ated Voltage (Vo
-00000440: 6c74 2922 2022 5261 7465 6420 566f 6c74  lt)" "Rated Volt
-00000450: 6167 6522 2028 6964 2038 2920 2861 7420  age" (id 8) (at 
-00000460: 3020 2d36 2e33 3520 3029 0a20 2020 2020  0 -6.35 0).     
-00000470: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000480: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000490: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
-000004a0: 6f70 6572 7479 2022 5465 6d70 6572 6174  operty "Temperat
-000004b0: 7572 6520 4772 6164 6522 2022 5465 6d70  ure Grade" "Temp
-000004c0: 6572 6174 7572 6520 4772 6164 6522 2028  erature Grade" (
-000004d0: 6964 2039 2920 2861 7420 3020 2d31 312e  id 9) (at 0 -11.
-000004e0: 3433 2030 290a 2020 2020 2020 2865 6666  43 0).      (eff
-000004f0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000500: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
-00000510: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
-00000520: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
-00000530: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
-00000540: 7970 6522 2028 6964 2031 3029 2028 6174  ype" (id 10) (at
-00000550: 2030 202d 382e 3839 2030 290a 2020 2020   0 -8.89 0).    
-00000560: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000570: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000580: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
-00000590: 726f 7065 7274 7920 226b 695f 6b65 7977  roperty "ki_keyw
-000005a0: 6f72 6473 2220 226b 6579 776f 7264 7322  ords" "keywords"
-000005b0: 2028 6964 2031 3129 2028 6174 2030 2030   (id 11) (at 0 0
-000005c0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000005d0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000005e0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000005f0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000600: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
-00000610: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
-00000620: 6f6e 2220 2869 6420 3132 2920 2861 7420  on" (id 12) (at 
-00000630: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000640: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000650: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000660: 6465 290a 2020 2020 290a 2020 2020 2873  de).    ).    (s
-00000670: 796d 626f 6c20 2249 504e 5f30 5f31 220a  ymbol "IPN_0_1".
-00000680: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000690: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-000006a0: 2020 2020 2020 2028 7879 202d 312e 3237         (xy -1.27
-000006b0: 2030 290a 2020 2020 2020 2020 2020 2878   0).          (x
-000006c0: 7920 2d31 2e30 3136 2030 290a 2020 2020  y -1.016 0).    
-000006d0: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
-000006e0: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
-000006f0: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000700: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-00000710: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-00000720: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-00000730: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-00000740: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-00000750: 2020 2020 2020 2020 2020 2878 7920 2d30            (xy -0
-00000760: 2e38 3839 2031 2e39 3035 290a 2020 2020  .889 1.905).    
-00000770: 2020 2020 2020 2878 7920 2d30 2e38 3839        (xy -0.889
-00000780: 202d 312e 3930 3529 0a20 2020 2020 2020   -1.905).       
-00000790: 2029 0a20 2020 2020 2020 2028 7374 726f   ).        (stro
-000007a0: 6b65 2028 7769 6474 6820 302e 3235 3429  ke (width 0.254)
-000007b0: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000007c0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-000007d0: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-000007e0: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000007f0: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-00000800: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000810: 0a20 2020 2020 2020 2020 2028 7879 2030  .          (xy 0
-00000820: 2e38 3839 2031 2e39 3035 290a 2020 2020  .889 1.905).    
-00000830: 2020 2020 2020 2878 7920 302e 3838 3920        (xy 0.889 
-00000840: 2d31 2e39 3035 290a 2020 2020 2020 2020  -1.905).        
-00000850: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
-00000860: 6520 2877 6964 7468 2030 2e32 3534 2920  e (width 0.254) 
-00000870: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000880: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-00000890: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-000008a0: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-000008b0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-000008c0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-000008d0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-000008e0: 3237 2030 290a 2020 2020 2020 2020 2020  27 0).          
-000008f0: 2878 7920 312e 3031 3620 3029 0a20 2020  (xy 1.016 0).   
-00000900: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00000910: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00000920: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00000930: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000940: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000950: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-00000960: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-00000970: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000980: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
-00000990: 2e39 3035 2030 290a 2020 2020 2020 2020  .905 0).        
-000009a0: 2020 2878 7920 322e 3534 2030 290a 2020    (xy 2.54 0).  
-000009b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000009c0: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-000009d0: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
-000009e0: 2028 636f 6c6f 7220 3020 3020 3020 3029   (color 0 0 0 0)
-000009f0: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
-00000a00: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
-00000a10: 2020 2029 0a20 2020 2029 0a20 2020 2028     ).    ).    (
-00000a20: 7379 6d62 6f6c 2022 4950 4e5f 315f 3122  symbol "IPN_1_1"
-00000a30: 0a20 2020 2020 2028 7069 6e20 7061 7373  .      (pin pass
-00000a40: 6976 6520 6c69 6e65 2028 6174 202d 332e  ive line (at -3.
-00000a50: 3831 2030 2030 2920 286c 656e 6774 6820  81 0 0) (length 
-00000a60: 322e 3534 290a 2020 2020 2020 2020 286e  2.54).        (n
-00000a70: 616d 6520 2231 2220 2865 6666 6563 7473  ame "1" (effects
-00000a80: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000a90: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000aa0: 2020 2028 6e75 6d62 6572 2022 3122 2028     (number "1" (
-00000ab0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000ac0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00000ad0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000ae0: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
-00000af0: 6520 2861 7420 332e 3831 2030 2031 3830  e (at 3.81 0 180
-00000b00: 2920 286c 656e 6774 6820 322e 3534 290a  ) (length 2.54).
-00000b10: 2020 2020 2020 2020 286e 616d 6520 2232          (name "2
-00000b20: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
-00000b30: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000b40: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
-00000b50: 6d62 6572 2022 3222 2028 6566 6665 6374  mber "2" (effect
-00000b60: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000b70: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-00000b80: 2020 290a 2020 2020 290a 2020 290a 290a    ).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2243 2220 2861  eference" "C" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 332e  "IPN" (at 0 -13.
+00000120: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3231 2e35 3920 3029 0a20  at 0 -21.59 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 342e 3133 2030 290a 2020 2020  0 -24.13 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3136 2e35 3120 3029 0a20 2020 2020   -16.51 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3139 2e30 3520 3029 0a20 2020   0 -19.05 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2243      (property "C
+00000320: 6170 6163 6974 616e 6365 2028 4661 7261  apacitance (Fara
+00000330: 6429 2220 2256 616c 7565 2220 2861 7420  d)" "Value" (at 
+00000340: 3020 2d33 2e38 3120 3029 0a20 2020 2020  0 -3.81 0).     
+00000350: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000360: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000370: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000380: 6f70 6572 7479 2022 546f 6c65 7261 6e63  operty "Toleranc
+00000390: 6520 2825 2922 2022 546f 6c65 7261 6e63  e (%)" "Toleranc
+000003a0: 6522 2028 6174 2037 2e36 3220 2d33 2e38  e" (at 7.62 -3.8
+000003b0: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+000003c0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+000003d0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+000003e0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000003f0: 7065 7274 7920 2252 6174 6564 2056 6f6c  perty "Rated Vol
+00000400: 7461 6765 2028 566f 6c74 2922 2022 5261  tage (Volt)" "Ra
+00000410: 7465 6420 566f 6c74 6167 6522 2028 6174  ted Voltage" (at
+00000420: 2030 202d 362e 3335 2030 290a 2020 2020   0 -6.35 0).    
+00000430: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000440: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000450: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000460: 726f 7065 7274 7920 2254 656d 7065 7261  roperty "Tempera
+00000470: 7475 7265 2047 7261 6465 2220 2254 656d  ture Grade" "Tem
+00000480: 7065 7261 7475 7265 2047 7261 6465 2220  perature Grade" 
+00000490: 2861 7420 3020 2d31 312e 3433 2030 290a  (at 0 -11.43 0).
+000004a0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000004b0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000004c0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000004d0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000004e0: 2022 5061 636b 6167 6520 5479 7065 2220   "Package Type" 
+000004f0: 2250 6163 6b61 6765 2054 7970 6522 2028  "Package Type" (
+00000500: 6174 2030 202d 382e 3839 2030 290a 2020  at 0 -8.89 0).  
+00000510: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+00000520: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000530: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
+00000540: 2870 726f 7065 7274 7920 226b 695f 6b65  (property "ki_ke
+00000550: 7977 6f72 6473 2220 226b 6579 776f 7264  ywords" "keyword
+00000560: 7322 2028 6174 2030 2030 2030 290a 2020  s" (at 0 0 0).  
+00000570: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+00000580: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000590: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+000005a0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+000005b0: 6b69 5f64 6573 6372 6970 7469 6f6e 2220  ki_description" 
+000005c0: 2264 6573 6372 6970 7469 6f6e 2220 2861  "description" (a
+000005d0: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
+000005e0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000005f0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+00000600: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+00000610: 2873 796d 626f 6c20 2249 504e 5f30 5f31  (symbol "IPN_0_1
+00000620: 220a 2020 2020 2020 2870 6f6c 796c 696e  ".      (polylin
+00000630: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+00000640: 2020 2020 2020 2020 2028 7879 202d 312e           (xy -1.
+00000650: 3237 2030 290a 2020 2020 2020 2020 2020  27 0).          
+00000660: 2878 7920 2d31 2e30 3136 2030 290a 2020  (xy -1.016 0).  
+00000670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000680: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
+00000690: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+000006a0: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+000006b0: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+000006c0: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+000006d0: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+000006e0: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+000006f0: 2d30 2e38 3839 2031 2e39 3035 290a 2020  -0.889 1.905).  
+00000700: 2020 2020 2020 2020 2878 7920 2d30 2e38          (xy -0.8
+00000710: 3839 202d 312e 3930 3529 0a20 2020 2020  89 -1.905).     
+00000720: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
+00000730: 726f 6b65 2028 7769 6474 6820 302e 3235  roke (width 0.25
+00000740: 3429 2028 7479 7065 2064 6566 6175 6c74  4) (type default
+00000750: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+00000760: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+00000770: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+00000780: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+00000790: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000007a0: 2030 2e38 3839 2031 2e39 3035 290a 2020   0.889 1.905).  
+000007b0: 2020 2020 2020 2020 2878 7920 302e 3838          (xy 0.88
+000007c0: 3920 2d31 2e39 3035 290a 2020 2020 2020  9 -1.905).      
+000007d0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+000007e0: 6f6b 6520 2877 6964 7468 2030 2e32 3534  oke (width 0.254
+000007f0: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+00000800: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+00000810: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+00000820: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+00000830: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000840: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000850: 312e 3237 2030 290a 2020 2020 2020 2020  1.27 0).        
+00000860: 2020 2878 7920 312e 3031 3620 3029 0a20    (xy 1.016 0). 
+00000870: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000880: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000890: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
+000008a0: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+000008b0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+000008c0: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+000008d0: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000008e0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000008f0: 2031 2e39 3035 2030 290a 2020 2020 2020   1.905 0).      
+00000900: 2020 2020 2878 7920 322e 3534 2030 290a      (xy 2.54 0).
+00000910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000920: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+00000930: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
+00000940: 7429 290a 2020 2020 2020 2020 2866 696c  t)).        (fil
+00000950: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
+00000960: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
+00000970: 2028 7379 6d62 6f6c 2022 4950 4e5f 315f   (symbol "IPN_1_
+00000980: 3122 0a20 2020 2020 2028 7069 6e20 7061  1".      (pin pa
+00000990: 7373 6976 6520 6c69 6e65 2028 6174 202d  ssive line (at -
+000009a0: 332e 3831 2030 2030 2920 286c 656e 6774  3.81 0 0) (lengt
+000009b0: 6820 322e 3534 290a 2020 2020 2020 2020  h 2.54).        
+000009c0: 286e 616d 6520 2231 2220 2865 6666 6563  (name "1" (effec
+000009d0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000009e0: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+000009f0: 2020 2020 2028 6e75 6d62 6572 2022 3122       (number "1"
+00000a00: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000a10: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000a20: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
+00000a30: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
+00000a40: 696e 6520 2861 7420 332e 3831 2030 2031  ine (at 3.81 0 1
+00000a50: 3830 2920 286c 656e 6774 6820 322e 3534  80) (length 2.54
+00000a60: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
+00000a70: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
+00000a80: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000a90: 3237 2929 2929 0a20 2020 2020 2020 2028  27)))).        (
+00000aa0: 6e75 6d62 6572 2022 3222 2028 6566 6665  number "2" (effe
+00000ab0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000ac0: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000ad0: 2020 2020 290a 2020 2020 290a 2020 290a      ).    ).  ).
+00000ae0: 290a                                     ).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/connector.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/connector.kicad_sym`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 224a 2220 2869  eference" "J" (i
-000000c0: 6420 3029 2028 6174 2030 2030 2030 290a  d 0) (at 0 0 0).
-000000d0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-000000e0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-000000f0: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
-00000100: 2020 2870 726f 7065 7274 7920 2256 616c    (property "Val
-00000110: 7565 2220 2249 504e 2220 2869 6420 3129  ue" "IPN" (id 1)
-00000120: 2028 6174 2030 202d 352e 3038 2030 290a   (at 0 -5.08 0).
-00000130: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000140: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000150: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
-00000160: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-00000170: 2022 466f 6f74 7072 696e 7422 2022 466f   "Footprint" "Fo
-00000180: 6f74 7072 696e 7422 2028 6964 2032 2920  otprint" (id 2) 
-00000190: 2861 7420 3020 2d31 322e 3720 3029 0a20  (at 0 -12.7 0). 
-000001a0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000001b0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-000001c0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-000001d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000001e0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
-000001f0: 656e 7472 6565 5f75 726c 2220 2869 6420  entree_url" (id 
-00000200: 3329 2028 6174 2030 202d 3135 2e32 3420  3) (at 0 -15.24 
-00000210: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000220: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000230: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000240: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000250: 7274 7920 224d 616e 7566 6163 7475 7265  rty "Manufacture
-00000260: 7222 2022 4d61 6e75 6661 6374 7572 6572  r" "Manufacturer
-00000270: 2220 2869 6420 3429 2028 6174 2030 202d  " (id 4) (at 0 -
-00000280: 372e 3632 2030 290a 2020 2020 2020 2865  7.62 0).      (e
-00000290: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-000002a0: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-000002b0: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-000002c0: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-000002d0: 6374 7572 6572 2050 6172 7420 4e75 6d62  cturer Part Numb
-000002e0: 6572 2220 224d 504e 2220 2869 6420 3529  er" "MPN" (id 5)
-000002f0: 2028 6174 2030 202d 3130 2e31 3620 3029   (at 0 -10.16 0)
-00000300: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-00000310: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000320: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000330: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000340: 7920 2250 6172 7420 4e75 6d62 6572 2220  y "Part Number" 
-00000350: 2256 616c 7565 2220 2869 6420 3629 2028  "Value" (id 6) (
-00000360: 6174 2030 202d 322e 3534 2030 290a 2020  at 0 -2.54 0).  
-00000370: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000380: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000390: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
-000003a0: 2870 726f 7065 7274 7920 226b 695f 6b65  (property "ki_ke
-000003b0: 7977 6f72 6473 2220 226b 6579 776f 7264  ywords" "keyword
-000003c0: 7322 2028 6964 2037 2920 2861 7420 3020  s" (id 7) (at 0 
-000003d0: 3020 3029 0a20 2020 2020 2028 6566 6665  0 0).      (effe
-000003e0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000003f0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000400: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000410: 7065 7274 7920 226b 695f 6465 7363 7269  perty "ki_descri
-00000420: 7074 696f 6e22 2022 6465 7363 7269 7074  ption" "descript
-00000430: 696f 6e22 2028 6964 2038 2920 2861 7420  ion" (id 8) (at 
-00000440: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000450: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000460: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000470: 6465 290a 2020 2020 290a 2020 290a 290a  de).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 224a 2220 2861  eference" "J" (a
+000000c0: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
+000000d0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000000e0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+000000f0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000100: 6572 7479 2022 5661 6c75 6522 2022 4950  erty "Value" "IP
+00000110: 4e22 2028 6174 2030 202d 352e 3038 2030  N" (at 0 -5.08 0
+00000120: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000130: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000140: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
+00000150: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000160: 7479 2022 466f 6f74 7072 696e 7422 2022  ty "Footprint" "
+00000170: 466f 6f74 7072 696e 7422 2028 6174 2030  Footprint" (at 0
+00000180: 202d 3132 2e37 2030 290a 2020 2020 2020   -12.7 0).      
+00000190: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000001a0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000001b0: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+000001c0: 2028 7072 6f70 6572 7479 2022 4461 7461   (property "Data
+000001d0: 7368 6565 7422 2022 696e 7665 6e74 7265  sheet" "inventre
+000001e0: 655f 7572 6c22 2028 6174 2030 202d 3135  e_url" (at 0 -15
+000001f0: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
+00000200: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000210: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000220: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000230: 726f 7065 7274 7920 224d 616e 7566 6163  roperty "Manufac
+00000240: 7475 7265 7222 2022 4d61 6e75 6661 6374  turer" "Manufact
+00000250: 7572 6572 2220 2861 7420 3020 2d37 2e36  urer" (at 0 -7.6
+00000260: 3220 3029 0a20 2020 2020 2028 6566 6665  2 0).      (effe
+00000270: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000280: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000290: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000002a0: 7065 7274 7920 224d 616e 7566 6163 7475  perty "Manufactu
+000002b0: 7265 7220 5061 7274 204e 756d 6265 7222  rer Part Number"
+000002c0: 2022 4d50 4e22 2028 6174 2030 202d 3130   "MPN" (at 0 -10
+000002d0: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+000002e0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000002f0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000300: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000310: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
+00000320: 6d62 6572 2220 2256 616c 7565 2220 2861  mber" "Value" (a
+00000330: 7420 3020 2d32 2e35 3420 3029 0a20 2020  t 0 -2.54 0).   
+00000340: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000350: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000360: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000370: 7072 6f70 6572 7479 2022 6b69 5f6b 6579  property "ki_key
+00000380: 776f 7264 7322 2022 6b65 7977 6f72 6473  words" "keywords
+00000390: 2220 2861 7420 3020 3020 3029 0a20 2020  " (at 0 0 0).   
+000003a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000003b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000003c0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000003d0: 2020 2020 2870 726f 7065 7274 7920 226b      (property "k
+000003e0: 695f 6465 7363 7269 7074 696f 6e22 2022  i_description" "
+000003f0: 6465 7363 7269 7074 696f 6e22 2028 6174  description" (at
+00000400: 2030 2030 2030 290a 2020 2020 2020 2865   0 0 0).      (e
+00000410: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000420: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
+00000430: 6964 6529 0a20 2020 2029 0a20 2029 0a29  ide).    ).  ).)
+00000440: 0a                                       .
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/crystal-2p.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/diode-standard.kicad_sym`

 * *Files 11% similar despite different names*

```diff
@@ -1,169 +1,141 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2259 2220 2869  eference" "Y" (i
-000000c0: 6420 3029 2028 6174 2030 2035 2e30 3820  d 0) (at 0 5.08 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 352e 3234   1) (at 0 -15.24
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 302e 3332   2) (at 0 -20.32
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 322e 3836 2030 290a 2020 2020 2020 2865  2.86 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 372e 3738 2030 290a 2020  t 0 -17.78 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 372e  (id 5) (at 0 -7.
-00000300: 3632 2030 290a 2020 2020 2020 2865 6666  62 0).      (eff
-00000310: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000320: 2031 2e32 3720 312e 3237 2929 290a 2020   1.27 1.27))).  
-00000330: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000340: 7920 2246 7265 7175 656e 6379 2220 2256  y "Frequency" "V
-00000350: 616c 7565 2220 2869 6420 3629 2028 6174  alue" (id 6) (at
-00000360: 2030 202d 352e 3038 2030 290a 2020 2020   0 -5.08 0).    
-00000370: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000380: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000390: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
-000003a0: 726f 7065 7274 7920 224c 6f61 6420 4361  roperty "Load Ca
-000003b0: 7061 6369 7461 6e63 6520 2846 6172 6164  pacitance (Farad
-000003c0: 2922 2022 4c6f 6164 2043 6170 6163 6974  )" "Load Capacit
-000003d0: 616e 6365 2220 2869 6420 3729 2028 6174  ance" (id 7) (at
-000003e0: 2030 202d 3130 2e31 3620 3029 0a20 2020   0 -10.16 0).   
-000003f0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-00000400: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000410: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
-00000420: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
-00000430: 6163 6b61 6765 2053 697a 6522 2022 5061  ackage Size" "Pa
-00000440: 636b 6167 6520 5369 7a65 2220 2869 6420  ckage Size" (id 
-00000450: 3829 2028 6174 2030 202d 3132 2e37 2030  8) (at 0 -12.7 0
-00000460: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
-00000470: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000480: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
-00000490: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-000004a0: 7479 2022 6b69 5f6b 6579 776f 7264 7322  ty "ki_keywords"
-000004b0: 2022 6b65 7977 6f72 6473 2220 2869 6420   "keywords" (id 
-000004c0: 3929 2028 6174 2030 2030 2030 290a 2020  9) (at 0 0 0).  
-000004d0: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000004e0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000004f0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-00000500: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000510: 6b69 5f64 6573 6372 6970 7469 6f6e 2220  ki_description" 
-00000520: 2264 6573 6372 6970 7469 6f6e 2220 2869  "description" (i
-00000530: 6420 3130 2920 2861 7420 3020 3020 3029  d 10) (at 0 0 0)
-00000540: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-00000550: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000560: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000570: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
-00000580: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
-00000590: 2872 6563 7461 6e67 6c65 2028 7374 6172  (rectangle (star
-000005a0: 7420 2d31 2e30 3136 2033 2e30 3438 2920  t -1.016 3.048) 
-000005b0: 2865 6e64 2031 2e30 3136 202d 332e 3034  (end 1.016 -3.04
-000005c0: 3829 0a20 2020 2020 2020 2028 7374 726f  8).        (stro
-000005d0: 6b65 2028 7769 6474 6820 302e 3235 3429  ke (width 0.254)
-000005e0: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000005f0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000600: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000610: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-00000620: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-00000630: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000640: 0a20 2020 2020 2020 2020 2028 7879 202d  .          (xy -
-00000650: 322e 3534 2030 290a 2020 2020 2020 2020  2.54 0).        
-00000660: 2020 2878 7920 2d31 2e37 3738 2030 290a    (xy -1.778 0).
-00000670: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000680: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000690: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
-000006a0: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-000006b0: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
-000006c0: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
-000006d0: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
-000006e0: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
-000006f0: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-00000700: 7920 322e 3534 2030 290a 2020 2020 2020  y 2.54 0).      
-00000710: 2020 2020 2878 7920 312e 3737 3820 3029      (xy 1.778 0)
-00000720: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00000730: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-00000740: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-00000750: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00000760: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00000770: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
-00000780: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-00000790: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-000007a0: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-000007b0: 7879 202d 312e 3737 3820 322e 3534 290a  xy -1.778 2.54).
-000007c0: 2020 2020 2020 2020 2020 2878 7920 2d31            (xy -1
-000007d0: 2e37 3738 2030 290a 2020 2020 2020 2020  .778 0).        
-000007e0: 2020 2878 7920 2d31 2e37 3738 202d 322e    (xy -1.778 -2.
-000007f0: 3534 290a 2020 2020 2020 2020 290a 2020  54).        ).  
-00000800: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
-00000810: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
-00000820: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000830: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000840: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-00000850: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00000860: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
-00000870: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
-00000880: 2020 2878 7920 312e 3737 3820 322e 3534    (xy 1.778 2.54
-00000890: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
-000008a0: 312e 3737 3820 3029 0a20 2020 2020 2020  1.778 0).       
-000008b0: 2020 2028 7879 2031 2e37 3738 202d 322e     (xy 1.778 -2.
-000008c0: 3534 290a 2020 2020 2020 2020 290a 2020  54).        ).  
-000008d0: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
-000008e0: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
-000008f0: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000900: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000910: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-00000920: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00000930: 2028 7069 6e20 7061 7373 6976 6520 6c69   (pin passive li
-00000940: 6e65 2028 6174 202d 352e 3038 2030 2030  ne (at -5.08 0 0
-00000950: 2920 286c 656e 6774 6820 322e 3534 290a  ) (length 2.54).
-00000960: 2020 2020 2020 2020 286e 616d 6520 2231          (name "1
-00000970: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
-00000980: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000990: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
-000009a0: 6d62 6572 2022 3122 2028 6566 6665 6374  mber "1" (effect
-000009b0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000009c0: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-000009d0: 2020 290a 2020 2020 2020 2870 696e 2070    ).      (pin p
-000009e0: 6173 7369 7665 206c 696e 6520 2861 7420  assive line (at 
-000009f0: 352e 3038 2030 2031 3830 2920 286c 656e  5.08 0 180) (len
-00000a00: 6774 6820 322e 3534 290a 2020 2020 2020  gth 2.54).      
-00000a10: 2020 286e 616d 6520 2232 2220 2865 6666    (name "2" (eff
-00000a20: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000a30: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-00000a40: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
-00000a50: 3222 2028 6566 6665 6374 7320 2866 6f6e  2" (effects (fon
-00000a60: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000a70: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
-00000a80: 2020 290a 2020 290a 290a                   ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2244 2220 2861  eference" "D" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 332e  "IPN" (at 0 -13.
+00000120: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3231 2e35 3920 3029 0a20  at 0 -21.59 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 342e 3133 2030 290a 2020 2020  0 -24.13 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3136 2e35 3120 3029 0a20 2020 2020   -16.51 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3139 2e30 3520 3029 0a20 2020   0 -19.05 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 3020 2d33 2e38 3120  ue" (at 0 -3.81 
+00000340: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000350: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000360: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
+00000370: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000380: 466f 7277 6172 6420 566f 6c74 6167 6520  Forward Voltage 
+00000390: 2856 6f6c 7429 2220 2246 6f72 7761 7264  (Volt)" "Forward
+000003a0: 2056 6f6c 7461 6765 2220 2861 7420 3020   Voltage" (at 0 
+000003b0: 2d38 2e38 3920 3029 0a20 2020 2020 2028  -8.89 0).      (
+000003c0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000003d0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+000003e0: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000003f0: 2870 726f 7065 7274 7920 2243 7572 7265  (property "Curre
+00000400: 6e74 2028 416d 7073 2922 2022 5261 7465  nt (Amps)" "Rate
+00000410: 6420 4375 7272 656e 7422 2028 6174 2030  d Current" (at 0
+00000420: 202d 362e 3335 2030 290a 2020 2020 2020   -6.35 0).      
+00000430: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000440: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000450: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+00000460: 7065 7274 7920 2252 6174 6564 2056 6f6c  perty "Rated Vol
+00000470: 7461 6765 2028 566f 6c74 2922 2022 5261  tage (Volt)" "Ra
+00000480: 7465 6420 566f 6c74 6167 6522 2028 6174  ted Voltage" (at
+00000490: 2030 202d 3131 2e34 3320 3029 0a20 2020   0 -11.43 0).   
+000004a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000004b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000004c0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000004d0: 2020 2020 2870 726f 7065 7274 7920 226b      (property "k
+000004e0: 695f 6b65 7977 6f72 6473 2220 226b 6579  i_keywords" "key
+000004f0: 776f 7264 7322 2028 6174 2030 2030 2030  words" (at 0 0 0
+00000500: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000510: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000520: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
+00000530: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000540: 7479 2022 6b69 5f64 6573 6372 6970 7469  ty "ki_descripti
+00000550: 6f6e 2220 2264 6573 6372 6970 7469 6f6e  on" "description
+00000560: 2220 2861 7420 3020 3020 3029 0a20 2020  " (at 0 0 0).   
+00000570: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000580: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000590: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000005a0: 2020 2020 2873 796d 626f 6c20 2249 504e      (symbol "IPN
+000005b0: 5f30 5f31 220a 2020 2020 2020 2870 6f6c  _0_1".      (pol
+000005c0: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000005d0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000005e0: 2031 2e32 3720 2d31 2e33 3937 290a 2020   1.27 -1.397).  
+000005f0: 2020 2020 2020 2020 2878 7920 312e 3237          (xy 1.27
+00000600: 2031 2e33 3937 290a 2020 2020 2020 2020   1.397).        
+00000610: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
+00000620: 6520 2877 6964 7468 2030 2e32 3534 2920  e (width 0.254) 
+00000630: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+00000640: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+00000650: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+00000660: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+00000670: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+00000680: 2020 2020 2020 2020 2020 2878 7920 2d31            (xy -1
+00000690: 2e32 3720 312e 3237 290a 2020 2020 2020  .27 1.27).      
+000006a0: 2020 2020 2878 7920 2d31 2e32 3720 2d31      (xy -1.27 -1
+000006b0: 2e32 3729 0a20 2020 2020 2020 2020 2028  .27).          (
+000006c0: 7879 2031 2e32 3720 3029 0a20 2020 2020  xy 1.27 0).     
+000006d0: 2020 2020 2028 7879 202d 312e 3237 2031       (xy -1.27 1
+000006e0: 2e32 3729 0a20 2020 2020 2020 2029 0a20  .27).        ). 
+000006f0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+00000700: 7769 6474 6820 302e 3235 3429 2028 7479  width 0.254) (ty
+00000710: 7065 2064 6566 6175 6c74 2929 0a20 2020  pe default)).   
+00000720: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
+00000730: 2062 6163 6b67 726f 756e 6429 290a 2020   background)).  
+00000740: 2020 2020 290a 2020 2020 290a 2020 2020      ).    ).    
+00000750: 2873 796d 626f 6c20 2249 504e 5f31 5f31  (symbol "IPN_1_1
+00000760: 220a 2020 2020 2020 2870 696e 2070 6173  ".      (pin pas
+00000770: 7369 7665 206c 696e 6520 2861 7420 332e  sive line (at 3.
+00000780: 3831 2030 2031 3830 2920 286c 656e 6774  81 0 180) (lengt
+00000790: 6820 322e 3534 290a 2020 2020 2020 2020  h 2.54).        
+000007a0: 286e 616d 6520 2243 6174 686f 6465 2220  (name "Cathode" 
+000007b0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000007c0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000007d0: 2929 0a20 2020 2020 2020 2028 6e75 6d62  )).        (numb
+000007e0: 6572 2022 3122 2028 6566 6665 6374 7320  er "1" (effects 
+000007f0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000800: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
+00000810: 290a 2020 2020 2020 2870 696e 2070 6173  ).      (pin pas
+00000820: 7369 7665 206c 696e 6520 2861 7420 2d33  sive line (at -3
+00000830: 2e38 3120 3020 3029 2028 6c65 6e67 7468  .81 0 0) (length
+00000840: 2032 2e35 3429 0a20 2020 2020 2020 2028   2.54).        (
+00000850: 6e61 6d65 2022 416e 6f64 6522 2028 6566  name "Anode" (ef
+00000860: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000870: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
+00000880: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
+00000890: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
+000008a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000008b0: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
+000008c0: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/default.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/default.kicad_sym`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
 000000b0: 6566 6572 656e 6365 2220 2244 4553 2220  eference" "DES" 
-000000c0: 2869 6420 3029 2028 6174 2030 2030 2030  (id 0) (at 0 0 0
-000000d0: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
-000000e0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-000000f0: 3720 312e 3237 2929 290a 2020 2020 290a  7 1.27))).    ).
-00000100: 2020 2020 2870 726f 7065 7274 7920 2256      (property "V
-00000110: 616c 7565 2220 2249 504e 2220 2869 6420  alue" "IPN" (id 
-00000120: 3129 2028 6174 2030 202d 352e 3038 2030  1) (at 0 -5.08 0
-00000130: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
-00000140: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000150: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
-00000160: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-00000170: 7479 2022 466f 6f74 7072 696e 7422 2022  ty "Footprint" "
-00000180: 466f 6f74 7072 696e 7422 2028 6964 2032  Footprint" (id 2
-00000190: 2920 2861 7420 3020 2d31 322e 3720 3029  ) (at 0 -12.7 0)
-000001a0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-000001b0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-000001c0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-000001d0: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-000001e0: 7920 2244 6174 6173 6865 6574 2220 2269  y "Datasheet" "i
-000001f0: 6e76 656e 7472 6565 5f75 726c 2220 2869  nventree_url" (i
-00000200: 6420 3329 2028 6174 2030 202d 3135 2e32  d 3) (at 0 -15.2
-00000210: 3420 3029 0a20 2020 2020 2028 6566 6665  4 0).      (effe
-00000220: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000230: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000240: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000250: 7065 7274 7920 224d 616e 7566 6163 7475  perty "Manufactu
-00000260: 7265 7222 2022 4d61 6e75 6661 6374 7572  rer" "Manufactur
-00000270: 6572 2220 2869 6420 3429 2028 6174 2030  er" (id 4) (at 0
-00000280: 202d 372e 3632 2030 290a 2020 2020 2020   -7.62 0).      
-00000290: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-000002a0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-000002b0: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-000002c0: 2028 7072 6f70 6572 7479 2022 4d61 6e75   (property "Manu
-000002d0: 6661 6374 7572 6572 2050 6172 7420 4e75  facturer Part Nu
-000002e0: 6d62 6572 2220 224d 504e 2220 2869 6420  mber" "MPN" (id 
-000002f0: 3529 2028 6174 2030 202d 3130 2e31 3620  5) (at 0 -10.16 
-00000300: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000310: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000320: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000330: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000340: 7274 7920 2250 6172 7420 4e75 6d62 6572  rty "Part Number
-00000350: 2220 2256 616c 7565 2220 2869 6420 3629  " "Value" (id 6)
-00000360: 2028 6174 2030 202d 322e 3534 2030 290a   (at 0 -2.54 0).
-00000370: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000380: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000390: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
-000003a0: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-000003b0: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
-000003c0: 7264 7322 2028 6964 2037 2920 2861 7420  rds" (id 7) (at 
-000003d0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-000003e0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000003f0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000400: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000410: 726f 7065 7274 7920 226b 695f 6465 7363  roperty "ki_desc
-00000420: 7269 7074 696f 6e22 2022 6465 7363 7269  ription" "descri
-00000430: 7074 696f 6e22 2028 6964 2038 2920 2861  ption" (id 8) (a
-00000440: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
-00000450: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000460: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000470: 6869 6465 290a 2020 2020 290a 2020 290a  hide).    ).  ).
-00000480: 290a                                     ).
+000000c0: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
+000000d0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000000e0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000000f0: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000100: 6f70 6572 7479 2022 5661 6c75 6522 2022  operty "Value" "
+00000110: 4950 4e22 2028 6174 2030 202d 352e 3038  IPN" (at 0 -5.08
+00000120: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
+00000130: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+00000140: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
+00000150: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000160: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
+00000170: 2022 466f 6f74 7072 696e 7422 2028 6174   "Footprint" (at
+00000180: 2030 202d 3132 2e37 2030 290a 2020 2020   0 -12.7 0).    
+00000190: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000001a0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000001b0: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+000001c0: 2020 2028 7072 6f70 6572 7479 2022 4461     (property "Da
+000001d0: 7461 7368 6565 7422 2022 696e 7665 6e74  tasheet" "invent
+000001e0: 7265 655f 7572 6c22 2028 6174 2030 202d  ree_url" (at 0 -
+000001f0: 3135 2e32 3420 3029 0a20 2020 2020 2028  15.24 0).      (
+00000200: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000210: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+00000220: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+00000230: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
+00000240: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
+00000250: 6374 7572 6572 2220 2861 7420 3020 2d37  cturer" (at 0 -7
+00000260: 2e36 3220 3029 0a20 2020 2020 2028 6566  .62 0).      (ef
+00000270: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000280: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000290: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+000002a0: 726f 7065 7274 7920 224d 616e 7566 6163  roperty "Manufac
+000002b0: 7475 7265 7220 5061 7274 204e 756d 6265  turer Part Numbe
+000002c0: 7222 2022 4d50 4e22 2028 6174 2030 202d  r" "MPN" (at 0 -
+000002d0: 3130 2e31 3620 3029 0a20 2020 2020 2028  10.16 0).      (
+000002e0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000002f0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+00000300: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+00000310: 2870 726f 7065 7274 7920 2250 6172 7420  (property "Part 
+00000320: 4e75 6d62 6572 2220 2256 616c 7565 2220  Number" "Value" 
+00000330: 2861 7420 3020 2d32 2e35 3420 3029 0a20  (at 0 -2.54 0). 
+00000340: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+00000350: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+00000360: 2e32 3729 2929 0a20 2020 2029 0a20 2020  .27))).    ).   
+00000370: 2028 7072 6f70 6572 7479 2022 6b69 5f6b   (property "ki_k
+00000380: 6579 776f 7264 7322 2022 6b65 7977 6f72  eywords" "keywor
+00000390: 6473 2220 2861 7420 3020 3020 3029 0a20  ds" (at 0 0 0). 
+000003a0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000003b0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000003c0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000003d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000003e0: 226b 695f 6465 7363 7269 7074 696f 6e22  "ki_description"
+000003f0: 2022 6465 7363 7269 7074 696f 6e22 2028   "description" (
+00000400: 6174 2030 2030 2030 290a 2020 2020 2020  at 0 0 0).      
+00000410: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000420: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000430: 2068 6964 6529 0a20 2020 2029 0a20 2029   hide).    ).  )
+00000440: 0a29 0a                                  .).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/diode-led.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/diode-led.kicad_sym`

 * *Files 4% similar despite different names*

```diff
@@ -1,175 +1,166 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2244 2220 2869  eference" "D" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 322e 3720   1) (at 0 -12.7 
-00000130: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000140: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000150: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000160: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000170: 7274 7920 2246 6f6f 7470 7269 6e74 2220  rty "Footprint" 
-00000180: 2246 6f6f 7470 7269 6e74 2220 2869 6420  "Footprint" (id 
-00000190: 3229 2028 6174 2030 202d 3230 2e33 3220  2) (at 0 -20.32 
-000001a0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000001b0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000001c0: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-000001d0: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-000001e0: 7274 7920 2244 6174 6173 6865 6574 2220  rty "Datasheet" 
-000001f0: 2269 6e76 656e 7472 6565 5f75 726c 2220  "inventree_url" 
-00000200: 2869 6420 3329 2028 6174 2030 202d 3232  (id 3) (at 0 -22
-00000210: 2e38 3620 3029 0a20 2020 2020 2028 6566  .86 0).      (ef
-00000220: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000230: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000240: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000250: 726f 7065 7274 7920 224d 616e 7566 6163  roperty "Manufac
-00000260: 7475 7265 7222 2022 4d61 6e75 6661 6374  turer" "Manufact
-00000270: 7572 6572 2220 2869 6420 3429 2028 6174  urer" (id 4) (at
-00000280: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
-00000290: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-000002a0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-000002b0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
-000002c0: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
-000002d0: 616e 7566 6163 7475 7265 7220 5061 7274  anufacturer Part
-000002e0: 204e 756d 6265 7222 2022 4d50 4e22 2028   Number" "MPN" (
-000002f0: 6964 2035 2920 2861 7420 3020 2d31 372e  id 5) (at 0 -17.
-00000300: 3738 2030 290a 2020 2020 2020 2865 6666  78 0).      (eff
-00000310: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000320: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
-00000330: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
-00000340: 6f70 6572 7479 2022 5061 7274 204e 756d  operty "Part Num
-00000350: 6265 7222 2022 5661 6c75 6522 2028 6964  ber" "Value" (id
-00000360: 2036 2920 2861 7420 3020 2d31 302e 3136   6) (at 0 -10.16
-00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000390: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000003a0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000003b0: 6572 7479 2022 466f 7277 6172 6420 566f  erty "Forward Vo
-000003c0: 6c74 6167 6520 2856 6f6c 7429 2220 2246  ltage (Volt)" "F
-000003d0: 6f72 7761 7264 2056 6f6c 7461 6765 2220  orward Voltage" 
-000003e0: 2869 6420 3729 2028 6174 2030 202d 372e  (id 7) (at 0 -7.
-000003f0: 3632 2030 290a 2020 2020 2020 2865 6666  62 0).      (eff
-00000400: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000410: 2031 2e32 3720 312e 3237 2929 290a 2020   1.27 1.27))).  
-00000420: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000430: 7920 224c 4544 2043 6f6c 6f72 2220 224c  y "LED Color" "L
-00000440: 4544 2043 6f6c 6f72 2220 2869 6420 3829  ED Color" (id 8)
-00000450: 2028 6174 2030 202d 352e 3038 2030 290a   (at 0 -5.08 0).
-00000460: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000470: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000480: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
-00000490: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-000004a0: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
-000004b0: 7264 7322 2028 6964 2039 2920 2861 7420  rds" (id 9) (at 
-000004c0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000004e0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-000004f0: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000500: 726f 7065 7274 7920 226b 695f 6465 7363  roperty "ki_desc
-00000510: 7269 7074 696f 6e22 2022 6465 7363 7269  ription" "descri
-00000520: 7074 696f 6e22 2028 6964 2031 3029 2028  ption" (id 10) (
-00000530: 6174 2030 2030 2030 290a 2020 2020 2020  at 0 0 0).      
-00000540: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000550: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000560: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000570: 2028 7379 6d62 6f6c 2022 4950 4e5f 305f   (symbol "IPN_0_
-00000580: 3122 0a20 2020 2020 2028 706f 6c79 6c69  1".      (polyli
-00000590: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-000005a0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-000005b0: 3237 202d 312e 3237 290a 2020 2020 2020  27 -1.27).      
-000005c0: 2020 2020 2878 7920 312e 3237 2031 2e32      (xy 1.27 1.2
-000005d0: 3729 0a20 2020 2020 2020 2029 0a20 2020  7).        ).   
-000005e0: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
-000005f0: 6474 6820 302e 3338 3129 2028 7479 7065  dth 0.381) (type
-00000600: 2064 6566 6175 6c74 2920 2863 6f6c 6f72   default) (color
-00000610: 2030 2030 2030 2030 2929 0a20 2020 2020   0 0 0 0)).     
-00000620: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
-00000630: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
-00000640: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
-00000650: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
-00000660: 2020 2020 2028 7879 202d 312e 3237 2031       (xy -1.27 1
-00000670: 2e32 3729 0a20 2020 2020 2020 2020 2028  .27).          (
-00000680: 7879 202d 312e 3237 202d 312e 3237 290a  xy -1.27 -1.27).
-00000690: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-000006a0: 3237 2030 290a 2020 2020 2020 2020 2020  27 0).          
-000006b0: 2878 7920 2d31 2e32 3720 312e 3237 290a  (xy -1.27 1.27).
-000006c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000006d0: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-000006e0: 2030 2e32 3534 2920 2874 7970 6520 6465   0.254) (type de
-000006f0: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000700: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000710: 2866 696c 6c20 2874 7970 6520 6261 636b  (fill (type back
-00000720: 6772 6f75 6e64 2929 0a20 2020 2020 2029  ground)).      )
-00000730: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-00000740: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-00000750: 2020 2020 2020 2020 2878 7920 2d30 2e38          (xy -0.8
-00000760: 3839 202d 312e 3737 3829 0a20 2020 2020  89 -1.778).     
-00000770: 2020 2020 2028 7879 2030 2e35 3038 202d       (xy 0.508 -
-00000780: 332e 3137 3529 0a20 2020 2020 2020 2020  3.175).         
-00000790: 2028 7879 2030 2e32 3534 202d 322e 3431   (xy 0.254 -2.41
-000007a0: 3329 0a20 2020 2020 2020 2020 2028 7879  3).          (xy
-000007b0: 202d 302e 3235 3420 2d32 2e39 3231 290a   -0.254 -2.921).
-000007c0: 2020 2020 2020 2020 2020 2878 7920 302e            (xy 0.
-000007d0: 3530 3820 2d33 2e31 3735 290a 2020 2020  508 -3.175).    
-000007e0: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
-000007f0: 7472 6f6b 6520 2877 6964 7468 2030 2e32  troke (width 0.2
-00000800: 3534 2920 2874 7970 6520 6465 6661 756c  54) (type defaul
-00000810: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-00000820: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
-00000830: 6c20 2874 7970 6520 6f75 746c 696e 6529  l (type outline)
-00000840: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000850: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
-00000860: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
-00000870: 2028 7879 2030 2e36 3335 202d 312e 3635   (xy 0.635 -1.65
-00000880: 3129 0a20 2020 2020 2020 2020 2028 7879  1).          (xy
-00000890: 2032 2e30 3332 202d 332e 3034 3829 0a20   2.032 -3.048). 
-000008a0: 2020 2020 2020 2020 2028 7879 2031 2e32           (xy 1.2
-000008b0: 3720 2d32 2e37 3934 290a 2020 2020 2020  7 -2.794).      
-000008c0: 2020 2020 2878 7920 312e 3737 3820 2d32      (xy 1.778 -2
-000008d0: 2e32 3836 290a 2020 2020 2020 2020 2020  .286).          
-000008e0: 2878 7920 322e 3033 3220 2d33 2e30 3438  (xy 2.032 -3.048
-000008f0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00000900: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-00000910: 7468 2030 2e32 3534 2920 2874 7970 6520  th 0.254) (type 
-00000920: 6465 6661 756c 7429 2028 636f 6c6f 7220  default) (color 
-00000930: 3020 3020 3020 3029 290a 2020 2020 2020  0 0 0 0)).      
-00000940: 2020 2866 696c 6c20 2874 7970 6520 6f75    (fill (type ou
-00000950: 746c 696e 6529 290a 2020 2020 2020 290a  tline)).      ).
-00000960: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
-00000970: 6c20 2249 504e 5f31 5f31 220a 2020 2020  l "IPN_1_1".    
-00000980: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
-00000990: 696e 6520 2861 7420 332e 3831 2030 2031  ine (at 3.81 0 1
-000009a0: 3830 2920 286c 656e 6774 6820 322e 3534  80) (length 2.54
-000009b0: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
-000009c0: 2243 6174 686f 6465 2220 2865 6666 6563  "Cathode" (effec
-000009d0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000009e0: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-000009f0: 2020 2020 2028 6e75 6d62 6572 2022 3122       (number "1"
-00000a00: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000a10: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000a20: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
-00000a30: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
-00000a40: 696e 6520 2861 7420 2d33 2e38 3120 3020  ine (at -3.81 0 
-00000a50: 3029 2028 6c65 6e67 7468 2032 2e35 3429  0) (length 2.54)
-00000a60: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
-00000a70: 416e 6f64 6522 2028 6566 6665 6374 7320  Anode" (effects 
-00000a80: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000a90: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000aa0: 2020 286e 756d 6265 7220 2232 2220 2865    (number "2" (e
-00000ab0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000ac0: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000ad0: 0a20 2020 2020 2029 0a20 2020 2029 0a20  .      ).    ). 
-00000ae0: 2029 0a29 0a                              ).).
+000000b0: 6566 6572 656e 6365 2220 2244 2220 2861  eference" "D" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 322e  "IPN" (at 0 -12.
+00000120: 3720 3029 0a20 2020 2020 2028 6566 6665  7 0).      (effe
+00000130: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000140: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000150: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+00000160: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
+00000170: 2220 2246 6f6f 7470 7269 6e74 2220 2861  " "Footprint" (a
+00000180: 7420 3020 2d32 302e 3332 2030 290a 2020  t 0 -20.32 0).  
+00000190: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+000001a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000001b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+000001c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+000001d0: 4461 7461 7368 6565 7422 2022 696e 7665  Datasheet" "inve
+000001e0: 6e74 7265 655f 7572 6c22 2028 6174 2030  ntree_url" (at 0
+000001f0: 202d 3232 2e38 3620 3029 0a20 2020 2020   -22.86 0).     
+00000200: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000210: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000220: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+00000230: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+00000240: 7566 6163 7475 7265 7222 2022 4d61 6e75  ufacturer" "Manu
+00000250: 6661 6374 7572 6572 2220 2861 7420 3020  facturer" (at 0 
+00000260: 2d31 352e 3234 2030 290a 2020 2020 2020  -15.24 0).      
+00000270: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000280: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000290: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+000002a0: 2028 7072 6f70 6572 7479 2022 4d61 6e75   (property "Manu
+000002b0: 6661 6374 7572 6572 2050 6172 7420 4e75  facturer Part Nu
+000002c0: 6d62 6572 2220 224d 504e 2220 2861 7420  mber" "MPN" (at 
+000002d0: 3020 2d31 372e 3738 2030 290a 2020 2020  0 -17.78 0).    
+000002e0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000002f0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000300: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000310: 2020 2028 7072 6f70 6572 7479 2022 5061     (property "Pa
+00000320: 7274 204e 756d 6265 7222 2022 5661 6c75  rt Number" "Valu
+00000330: 6522 2028 6174 2030 202d 3130 2e31 3620  e" (at 0 -10.16 
+00000340: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000350: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000360: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
+00000370: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
+00000380: 7274 7920 2246 6f72 7761 7264 2056 6f6c  rty "Forward Vol
+00000390: 7461 6765 2028 566f 6c74 2922 2022 466f  tage (Volt)" "Fo
+000003a0: 7277 6172 6420 566f 6c74 6167 6522 2028  rward Voltage" (
+000003b0: 6174 2030 202d 372e 3632 2030 290a 2020  at 0 -7.62 0).  
+000003c0: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+000003d0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000003e0: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
+000003f0: 2870 726f 7065 7274 7920 224c 4544 2043  (property "LED C
+00000400: 6f6c 6f72 2220 224c 4544 2043 6f6c 6f72  olor" "LED Color
+00000410: 2220 2861 7420 3020 2d35 2e30 3820 3029  " (at 0 -5.08 0)
+00000420: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+00000430: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000440: 2031 2e32 3729 2929 0a20 2020 2029 0a20   1.27))).    ). 
+00000450: 2020 2028 7072 6f70 6572 7479 2022 6b69     (property "ki
+00000460: 5f6b 6579 776f 7264 7322 2022 6b65 7977  _keywords" "keyw
+00000470: 6f72 6473 2220 2861 7420 3020 3020 3029  ords" (at 0 0 0)
+00000480: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+00000490: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000004a0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000004b0: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+000004c0: 7920 226b 695f 6465 7363 7269 7074 696f  y "ki_descriptio
+000004d0: 6e22 2022 6465 7363 7269 7074 696f 6e22  n" "description"
+000004e0: 2028 6174 2030 2030 2030 290a 2020 2020   (at 0 0 0).    
+000004f0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000500: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000510: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000520: 2020 2028 7379 6d62 6f6c 2022 4950 4e5f     (symbol "IPN_
+00000530: 305f 3122 0a20 2020 2020 2028 706f 6c79  0_1".      (poly
+00000540: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000550: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000560: 312e 3237 202d 312e 3237 290a 2020 2020  1.27 -1.27).    
+00000570: 2020 2020 2020 2878 7920 312e 3237 2031        (xy 1.27 1
+00000580: 2e32 3729 0a20 2020 2020 2020 2029 0a20  .27).        ). 
+00000590: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+000005a0: 7769 6474 6820 302e 3338 3129 2028 7479  width 0.381) (ty
+000005b0: 7065 2064 6566 6175 6c74 2929 0a20 2020  pe default)).   
+000005c0: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
+000005d0: 206e 6f6e 6529 290a 2020 2020 2020 290a   none)).      ).
+000005e0: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
+000005f0: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
+00000600: 2020 2020 2020 2028 7879 202d 312e 3237         (xy -1.27
+00000610: 2031 2e32 3729 0a20 2020 2020 2020 2020   1.27).         
+00000620: 2028 7879 202d 312e 3237 202d 312e 3237   (xy -1.27 -1.27
+00000630: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000640: 312e 3237 2030 290a 2020 2020 2020 2020  1.27 0).        
+00000650: 2020 2878 7920 2d31 2e32 3720 312e 3237    (xy -1.27 1.27
+00000660: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00000670: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+00000680: 7468 2030 2e32 3534 2920 2874 7970 6520  th 0.254) (type 
+00000690: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+000006a0: 2020 2866 696c 6c20 2874 7970 6520 6261    (fill (type ba
+000006b0: 636b 6772 6f75 6e64 2929 0a20 2020 2020  ckground)).     
+000006c0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000006d0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+000006e0: 2020 2020 2020 2020 2020 2878 7920 2d30            (xy -0
+000006f0: 2e38 3839 202d 312e 3737 3829 0a20 2020  .889 -1.778).   
+00000700: 2020 2020 2020 2028 7879 2030 2e35 3038         (xy 0.508
+00000710: 202d 332e 3137 3529 0a20 2020 2020 2020   -3.175).       
+00000720: 2020 2028 7879 2030 2e32 3534 202d 322e     (xy 0.254 -2.
+00000730: 3431 3329 0a20 2020 2020 2020 2020 2028  413).          (
+00000740: 7879 202d 302e 3235 3420 2d32 2e39 3231  xy -0.254 -2.921
+00000750: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000760: 302e 3530 3820 2d33 2e31 3735 290a 2020  0.508 -3.175).  
+00000770: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000780: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
+00000790: 2e32 3534 2920 2874 7970 6520 6465 6661  .254) (type defa
+000007a0: 756c 7429 290a 2020 2020 2020 2020 2866  ult)).        (f
+000007b0: 696c 6c20 2874 7970 6520 6f75 746c 696e  ill (type outlin
+000007c0: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+000007d0: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
+000007e0: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
+000007f0: 2020 2028 7879 2030 2e36 3335 202d 312e     (xy 0.635 -1.
+00000800: 3635 3129 0a20 2020 2020 2020 2020 2028  651).          (
+00000810: 7879 2032 2e30 3332 202d 332e 3034 3829  xy 2.032 -3.048)
+00000820: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
+00000830: 2e32 3720 2d32 2e37 3934 290a 2020 2020  .27 -2.794).    
+00000840: 2020 2020 2020 2878 7920 312e 3737 3820        (xy 1.778 
+00000850: 2d32 2e32 3836 290a 2020 2020 2020 2020  -2.286).        
+00000860: 2020 2878 7920 322e 3033 3220 2d33 2e30    (xy 2.032 -3.0
+00000870: 3438 290a 2020 2020 2020 2020 290a 2020  48).        ).  
+00000880: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+00000890: 6964 7468 2030 2e32 3534 2920 2874 7970  idth 0.254) (typ
+000008a0: 6520 6465 6661 756c 7429 290a 2020 2020  e default)).    
+000008b0: 2020 2020 2866 696c 6c20 2874 7970 6520      (fill (type 
+000008c0: 6f75 746c 696e 6529 290a 2020 2020 2020  outline)).      
+000008d0: 290a 2020 2020 290a 2020 2020 2873 796d  ).    ).    (sym
+000008e0: 626f 6c20 2249 504e 5f31 5f31 220a 2020  bol "IPN_1_1".  
+000008f0: 2020 2020 2870 696e 2070 6173 7369 7665      (pin passive
+00000900: 206c 696e 6520 2861 7420 332e 3831 2030   line (at 3.81 0
+00000910: 2031 3830 2920 286c 656e 6774 6820 322e   180) (length 2.
+00000920: 3534 290a 2020 2020 2020 2020 286e 616d  54).        (nam
+00000930: 6520 2243 6174 686f 6465 2220 2865 6666  e "Cathode" (eff
+00000940: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000950: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
+00000960: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
+00000970: 3122 2028 6566 6665 6374 7320 2866 6f6e  1" (effects (fon
+00000980: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000990: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
+000009a0: 2020 2020 2870 696e 2070 6173 7369 7665      (pin passive
+000009b0: 206c 696e 6520 2861 7420 2d33 2e38 3120   line (at -3.81 
+000009c0: 3020 3029 2028 6c65 6e67 7468 2032 2e35  0 0) (length 2.5
+000009d0: 3429 0a20 2020 2020 2020 2028 6e61 6d65  4).        (name
+000009e0: 2022 416e 6f64 6522 2028 6566 6665 6374   "Anode" (effect
+000009f0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000a00: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+00000a10: 2020 2020 286e 756d 6265 7220 2232 2220      (number "2" 
+00000a20: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000a30: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000a40: 2929 0a20 2020 2020 2029 0a20 2020 2029  )).      ).    )
+00000a50: 0a20 2029 0a29 0a                        .  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/diode-schottky.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/diode-schottky.kicad_sym`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,154 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2244 2220 2869  eference" "D" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 332e 3937   1) (at 0 -13.97
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 312e 3539   2) (at 0 -21.59
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 342e 3133 2030 290a 2020 2020 2020 2865  4.13 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3139  (id 5) (at 0 -19
-00000300: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2030 202d 332e 3831  d 6) (at 0 -3.81
-00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000390: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000003a0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000003b0: 2246 6f72 7761 7264 2056 6f6c 7461 6765  "Forward Voltage
-000003c0: 2028 566f 6c74 2922 2022 466f 7277 6172   (Volt)" "Forwar
-000003d0: 6420 566f 6c74 6167 6522 2028 6964 2037  d Voltage" (id 7
-000003e0: 2920 2861 7420 3020 2d38 2e38 3920 3029  ) (at 0 -8.89 0)
-000003f0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-00000400: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000410: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000420: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000430: 7920 2243 7572 7265 6e74 2028 416d 7073  y "Current (Amps
-00000440: 2922 2022 5261 7465 6420 4375 7272 656e  )" "Rated Curren
-00000450: 7422 2028 6964 2038 2920 2861 7420 3020  t" (id 8) (at 0 
-00000460: 2d36 2e33 3520 3029 0a20 2020 2020 2028  -6.35 0).      (
-00000470: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000480: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00000490: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000004a0: 6572 7479 2022 5261 7465 6420 566f 6c74  erty "Rated Volt
-000004b0: 6167 6520 2856 6f6c 7429 2220 2252 6174  age (Volt)" "Rat
-000004c0: 6564 2056 6f6c 7461 6765 2220 2869 6420  ed Voltage" (id 
-000004d0: 3929 2028 6174 2030 202d 3131 2e34 3320  9) (at 0 -11.43 
-000004e0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000004f0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000500: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000510: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000520: 7274 7920 226b 695f 6b65 7977 6f72 6473  rty "ki_keywords
-00000530: 2220 226b 6579 776f 7264 7322 2028 6964  " "keywords" (id
-00000540: 2031 3029 2028 6174 2030 2030 2030 290a   10) (at 0 0 0).
-00000550: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000560: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000570: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
-00000580: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-00000590: 2022 6b69 5f64 6573 6372 6970 7469 6f6e   "ki_description
-000005a0: 2220 2264 6573 6372 6970 7469 6f6e 2220  " "description" 
-000005b0: 2869 6420 3131 2920 2861 7420 3020 3020  (id 11) (at 0 0 
-000005c0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000005d0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000005e0: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-000005f0: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
-00000600: 6c20 2249 504e 5f30 5f31 220a 2020 2020  l "IPN_0_1".    
-00000610: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
-00000620: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
-00000630: 2020 2028 7879 2031 2e32 3720 2d31 2e33     (xy 1.27 -1.3
-00000640: 3937 290a 2020 2020 2020 2020 2020 2878  97).          (x
-00000650: 7920 322e 3135 3920 2d31 2e33 3937 290a  y 2.159 -1.397).
-00000660: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000670: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000680: 2030 2e32 3534 2920 2874 7970 6520 6465   0.254) (type de
-00000690: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-000006a0: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-000006b0: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-000006c0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-000006d0: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
-000006e0: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
-000006f0: 2020 2878 7920 312e 3237 202d 312e 3339    (xy 1.27 -1.39
-00000700: 3729 0a20 2020 2020 2020 2020 2028 7879  7).          (xy
-00000710: 2031 2e32 3720 312e 3339 3729 0a20 2020   1.27 1.397).   
-00000720: 2020 2020 2020 2028 7879 2030 2e33 3831         (xy 0.381
-00000730: 2031 2e33 3937 290a 2020 2020 2020 2020   1.397).        
-00000740: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
-00000750: 6520 2877 6964 7468 2030 2e32 3534 2920  e (width 0.254) 
-00000760: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000770: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-00000780: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-00000790: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-000007a0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-000007b0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-000007c0: 2020 2020 2020 2020 2020 2878 7920 2d31            (xy -1
-000007d0: 2e32 3720 312e 3237 290a 2020 2020 2020  .27 1.27).      
-000007e0: 2020 2020 2878 7920 2d31 2e32 3720 2d31      (xy -1.27 -1
-000007f0: 2e32 3729 0a20 2020 2020 2020 2020 2028  .27).          (
-00000800: 7879 2031 2e32 3720 3029 0a20 2020 2020  xy 1.27 0).     
-00000810: 2020 2020 2028 7879 202d 312e 3237 2031       (xy -1.27 1
-00000820: 2e32 3729 0a20 2020 2020 2020 2029 0a20  .27).        ). 
-00000830: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-00000840: 7769 6474 6820 302e 3235 3429 2028 7479  width 0.254) (ty
-00000850: 7065 2064 6566 6175 6c74 2920 2863 6f6c  pe default) (col
-00000860: 6f72 2030 2030 2030 2030 2929 0a20 2020  or 0 0 0 0)).   
-00000870: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
-00000880: 2062 6163 6b67 726f 756e 6429 290a 2020   background)).  
-00000890: 2020 2020 290a 2020 2020 290a 2020 2020      ).    ).    
-000008a0: 2873 796d 626f 6c20 2249 504e 5f31 5f31  (symbol "IPN_1_1
-000008b0: 220a 2020 2020 2020 2870 696e 2070 6173  ".      (pin pas
-000008c0: 7369 7665 206c 696e 6520 2861 7420 332e  sive line (at 3.
-000008d0: 3831 2030 2031 3830 2920 286c 656e 6774  81 0 180) (lengt
-000008e0: 6820 322e 3534 290a 2020 2020 2020 2020  h 2.54).        
-000008f0: 286e 616d 6520 2243 6174 686f 6465 2220  (name "Cathode" 
-00000900: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000910: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000920: 2929 0a20 2020 2020 2020 2028 6e75 6d62  )).        (numb
-00000930: 6572 2022 3122 2028 6566 6665 6374 7320  er "1" (effects 
-00000940: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000950: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000960: 290a 2020 2020 2020 2870 696e 2070 6173  ).      (pin pas
-00000970: 7369 7665 206c 696e 6520 2861 7420 2d33  sive line (at -3
-00000980: 2e38 3120 3020 3029 2028 6c65 6e67 7468  .81 0 0) (length
-00000990: 2032 2e35 3429 0a20 2020 2020 2020 2028   2.54).        (
-000009a0: 6e61 6d65 2022 416e 6f64 6522 2028 6566  name "Anode" (ef
-000009b0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000009c0: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-000009d0: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-000009e0: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
-000009f0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000a00: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-00000a10: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2244 2220 2861  eference" "D" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 332e  "IPN" (at 0 -13.
+00000120: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3231 2e35 3920 3029 0a20  at 0 -21.59 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 342e 3133 2030 290a 2020 2020  0 -24.13 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3136 2e35 3120 3029 0a20 2020 2020   -16.51 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3139 2e30 3520 3029 0a20 2020   0 -19.05 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 3020 2d33 2e38 3120  ue" (at 0 -3.81 
+00000340: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000350: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000360: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
+00000370: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000380: 466f 7277 6172 6420 566f 6c74 6167 6520  Forward Voltage 
+00000390: 2856 6f6c 7429 2220 2246 6f72 7761 7264  (Volt)" "Forward
+000003a0: 2056 6f6c 7461 6765 2220 2861 7420 3020   Voltage" (at 0 
+000003b0: 2d38 2e38 3920 3029 0a20 2020 2020 2028  -8.89 0).      (
+000003c0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000003d0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+000003e0: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000003f0: 2870 726f 7065 7274 7920 2243 7572 7265  (property "Curre
+00000400: 6e74 2028 416d 7073 2922 2022 5261 7465  nt (Amps)" "Rate
+00000410: 6420 4375 7272 656e 7422 2028 6174 2030  d Current" (at 0
+00000420: 202d 362e 3335 2030 290a 2020 2020 2020   -6.35 0).      
+00000430: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000440: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000450: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+00000460: 7065 7274 7920 2252 6174 6564 2056 6f6c  perty "Rated Vol
+00000470: 7461 6765 2028 566f 6c74 2922 2022 5261  tage (Volt)" "Ra
+00000480: 7465 6420 566f 6c74 6167 6522 2028 6174  ted Voltage" (at
+00000490: 2030 202d 3131 2e34 3320 3029 0a20 2020   0 -11.43 0).   
+000004a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000004b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000004c0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000004d0: 2020 2020 2870 726f 7065 7274 7920 226b      (property "k
+000004e0: 695f 6b65 7977 6f72 6473 2220 226b 6579  i_keywords" "key
+000004f0: 776f 7264 7322 2028 6174 2030 2030 2030  words" (at 0 0 0
+00000500: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000510: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000520: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
+00000530: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000540: 7479 2022 6b69 5f64 6573 6372 6970 7469  ty "ki_descripti
+00000550: 6f6e 2220 2264 6573 6372 6970 7469 6f6e  on" "description
+00000560: 2220 2861 7420 3020 3020 3029 0a20 2020  " (at 0 0 0).   
+00000570: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000580: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000590: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000005a0: 2020 2020 2873 796d 626f 6c20 2249 504e      (symbol "IPN
+000005b0: 5f30 5f31 220a 2020 2020 2020 2870 6f6c  _0_1".      (pol
+000005c0: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000005d0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000005e0: 2031 2e32 3720 2d31 2e33 3937 290a 2020   1.27 -1.397).  
+000005f0: 2020 2020 2020 2020 2878 7920 322e 3135          (xy 2.15
+00000600: 3920 2d31 2e33 3937 290a 2020 2020 2020  9 -1.397).      
+00000610: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+00000620: 6f6b 6520 2877 6964 7468 2030 2e32 3534  oke (width 0.254
+00000630: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+00000640: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+00000650: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+00000660: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+00000670: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000680: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000690: 312e 3237 202d 312e 3339 3729 0a20 2020  1.27 -1.397).   
+000006a0: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
+000006b0: 312e 3339 3729 0a20 2020 2020 2020 2020  1.397).         
+000006c0: 2028 7879 2030 2e33 3831 2031 2e33 3937   (xy 0.381 1.397
+000006d0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+000006e0: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+000006f0: 7468 2030 2e32 3534 2920 2874 7970 6520  th 0.254) (type 
+00000700: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00000710: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+00000720: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+00000730: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
+00000740: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
+00000750: 2020 2020 2878 7920 2d31 2e32 3720 312e      (xy -1.27 1.
+00000760: 3237 290a 2020 2020 2020 2020 2020 2878  27).          (x
+00000770: 7920 2d31 2e32 3720 2d31 2e32 3729 0a20  y -1.27 -1.27). 
+00000780: 2020 2020 2020 2020 2028 7879 2031 2e32           (xy 1.2
+00000790: 3720 3029 0a20 2020 2020 2020 2020 2028  7 0).          (
+000007a0: 7879 202d 312e 3237 2031 2e32 3729 0a20  xy -1.27 1.27). 
+000007b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000007c0: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+000007d0: 302e 3235 3429 2028 7479 7065 2064 6566  0.254) (type def
+000007e0: 6175 6c74 2929 0a20 2020 2020 2020 2028  ault)).        (
+000007f0: 6669 6c6c 2028 7479 7065 2062 6163 6b67  fill (type backg
+00000800: 726f 756e 6429 290a 2020 2020 2020 290a  round)).      ).
+00000810: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
+00000820: 6c20 2249 504e 5f31 5f31 220a 2020 2020  l "IPN_1_1".    
+00000830: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
+00000840: 696e 6520 2861 7420 332e 3831 2030 2031  ine (at 3.81 0 1
+00000850: 3830 2920 286c 656e 6774 6820 322e 3534  80) (length 2.54
+00000860: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
+00000870: 2243 6174 686f 6465 2220 2865 6666 6563  "Cathode" (effec
+00000880: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+00000890: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+000008a0: 2020 2020 2028 6e75 6d62 6572 2022 3122       (number "1"
+000008b0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000008c0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000008d0: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
+000008e0: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
+000008f0: 696e 6520 2861 7420 2d33 2e38 3120 3020  ine (at -3.81 0 
+00000900: 3029 2028 6c65 6e67 7468 2032 2e35 3429  0) (length 2.54)
+00000910: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
+00000920: 416e 6f64 6522 2028 6566 6665 6374 7320  Anode" (effects 
+00000930: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000940: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
+00000950: 2020 286e 756d 6265 7220 2232 2220 2865    (number "2" (e
+00000960: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000970: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000980: 0a20 2020 2020 2029 0a20 2020 2029 0a20  .      ).    ). 
+00000990: 2029 0a29 0a                              ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/diode-standard.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/diode-zener.kicad_sym`

 * *Files 5% similar despite different names*

```diff
@@ -1,149 +1,153 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2244 2220 2869  eference" "D" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 332e 3937   1) (at 0 -13.97
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 312e 3539   2) (at 0 -21.59
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 342e 3133 2030 290a 2020 2020 2020 2865  4.13 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3139  (id 5) (at 0 -19
-00000300: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2030 202d 332e 3831  d 6) (at 0 -3.81
-00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000390: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000003a0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000003b0: 2246 6f72 7761 7264 2056 6f6c 7461 6765  "Forward Voltage
-000003c0: 2028 566f 6c74 2922 2022 466f 7277 6172   (Volt)" "Forwar
-000003d0: 6420 566f 6c74 6167 6522 2028 6964 2037  d Voltage" (id 7
-000003e0: 2920 2861 7420 3020 2d38 2e38 3920 3029  ) (at 0 -8.89 0)
-000003f0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-00000400: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000410: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000420: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000430: 7920 2243 7572 7265 6e74 2028 416d 7073  y "Current (Amps
-00000440: 2922 2022 5261 7465 6420 4375 7272 656e  )" "Rated Curren
-00000450: 7422 2028 6964 2038 2920 2861 7420 3020  t" (id 8) (at 0 
-00000460: 2d36 2e33 3520 3029 0a20 2020 2020 2028  -6.35 0).      (
-00000470: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000480: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00000490: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000004a0: 6572 7479 2022 5261 7465 6420 566f 6c74  erty "Rated Volt
-000004b0: 6167 6520 2856 6f6c 7429 2220 2252 6174  age (Volt)" "Rat
-000004c0: 6564 2056 6f6c 7461 6765 2220 2869 6420  ed Voltage" (id 
-000004d0: 3929 2028 6174 2030 202d 3131 2e34 3320  9) (at 0 -11.43 
-000004e0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000004f0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000500: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000510: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000520: 7274 7920 226b 695f 6b65 7977 6f72 6473  rty "ki_keywords
-00000530: 2220 226b 6579 776f 7264 7322 2028 6964  " "keywords" (id
-00000540: 2031 3029 2028 6174 2030 2030 2030 290a   10) (at 0 0 0).
-00000550: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000560: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000570: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
-00000580: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-00000590: 2022 6b69 5f64 6573 6372 6970 7469 6f6e   "ki_description
-000005a0: 2220 2264 6573 6372 6970 7469 6f6e 2220  " "description" 
-000005b0: 2869 6420 3131 2920 2861 7420 3020 3020  (id 11) (at 0 0 
-000005c0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000005d0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000005e0: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-000005f0: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
-00000600: 6c20 2249 504e 5f30 5f31 220a 2020 2020  l "IPN_0_1".    
-00000610: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
-00000620: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
-00000630: 2020 2028 7879 2031 2e32 3720 2d31 2e33     (xy 1.27 -1.3
-00000640: 3937 290a 2020 2020 2020 2020 2020 2878  97).          (x
-00000650: 7920 312e 3237 2031 2e33 3937 290a 2020  y 1.27 1.397).  
-00000660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000670: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-00000680: 2e32 3534 2920 2874 7970 6520 6465 6661  .254) (type defa
-00000690: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-000006a0: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-000006b0: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-000006c0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-000006d0: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
-000006e0: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
-000006f0: 2878 7920 2d31 2e32 3720 312e 3237 290a  (xy -1.27 1.27).
-00000700: 2020 2020 2020 2020 2020 2878 7920 2d31            (xy -1
-00000710: 2e32 3720 2d31 2e32 3729 0a20 2020 2020  .27 -1.27).     
-00000720: 2020 2020 2028 7879 2031 2e32 3720 3029       (xy 1.27 0)
-00000730: 0a20 2020 2020 2020 2020 2028 7879 202d  .          (xy -
-00000740: 312e 3237 2031 2e32 3729 0a20 2020 2020  1.27 1.27).     
-00000750: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
-00000760: 726f 6b65 2028 7769 6474 6820 302e 3235  roke (width 0.25
-00000770: 3429 2028 7479 7065 2064 6566 6175 6c74  4) (type default
-00000780: 2920 2863 6f6c 6f72 2030 2030 2030 2030  ) (color 0 0 0 0
-00000790: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
-000007a0: 2028 7479 7065 2062 6163 6b67 726f 756e   (type backgroun
-000007b0: 6429 290a 2020 2020 2020 290a 2020 2020  d)).      ).    
-000007c0: 290a 2020 2020 2873 796d 626f 6c20 2249  ).    (symbol "I
-000007d0: 504e 5f31 5f31 220a 2020 2020 2020 2870  PN_1_1".      (p
-000007e0: 696e 2070 6173 7369 7665 206c 696e 6520  in passive line 
-000007f0: 2861 7420 332e 3831 2030 2031 3830 2920  (at 3.81 0 180) 
-00000800: 286c 656e 6774 6820 322e 3534 290a 2020  (length 2.54).  
-00000810: 2020 2020 2020 286e 616d 6520 2243 6174        (name "Cat
-00000820: 686f 6465 2220 2865 6666 6563 7473 2028  hode" (effects (
-00000830: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000840: 312e 3237 2929 2929 0a20 2020 2020 2020  1.27)))).       
-00000850: 2028 6e75 6d62 6572 2022 3122 2028 6566   (number "1" (ef
-00000860: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000870: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-00000880: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-00000890: 696e 2070 6173 7369 7665 206c 696e 6520  in passive line 
-000008a0: 2861 7420 2d33 2e38 3120 3020 3029 2028  (at -3.81 0 0) (
-000008b0: 6c65 6e67 7468 2032 2e35 3429 0a20 2020  length 2.54).   
-000008c0: 2020 2020 2028 6e61 6d65 2022 416e 6f64       (name "Anod
-000008d0: 6522 2028 6566 6665 6374 7320 2866 6f6e  e" (effects (fon
-000008e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-000008f0: 3729 2929 290a 2020 2020 2020 2020 286e  7)))).        (n
-00000900: 756d 6265 7220 2232 2220 2865 6666 6563  umber "2" (effec
-00000910: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000920: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-00000930: 2020 2029 0a20 2020 2029 0a20 2029 0a29     ).    ).  ).)
-00000940: 0a                                       .
+000000b0: 6566 6572 656e 6365 2220 2244 2220 2861  eference" "D" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 332e  "IPN" (at 0 -13.
+00000120: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3231 2e35 3920 3029 0a20  at 0 -21.59 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 342e 3133 2030 290a 2020 2020  0 -24.13 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3136 2e35 3120 3029 0a20 2020 2020   -16.51 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3139 2e30 3520 3029 0a20 2020   0 -19.05 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 3020 2d33 2e38 3120  ue" (at 0 -3.81 
+00000340: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000350: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000360: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
+00000370: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000380: 466f 7277 6172 6420 566f 6c74 6167 6520  Forward Voltage 
+00000390: 2856 6f6c 7429 2220 2246 6f72 7761 7264  (Volt)" "Forward
+000003a0: 2056 6f6c 7461 6765 2220 2861 7420 3020   Voltage" (at 0 
+000003b0: 2d31 312e 3433 2030 290a 2020 2020 2020  -11.43 0).      
+000003c0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000003d0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000003e0: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+000003f0: 2028 7072 6f70 6572 7479 2022 506f 7765   (property "Powe
+00000400: 7220 2857 6174 7473 2922 2022 5261 7465  r (Watts)" "Rate
+00000410: 6420 506f 7765 7222 2028 6174 2030 202d  d Power" (at 0 -
+00000420: 362e 3335 2030 290a 2020 2020 2020 2865  6.35 0).      (e
+00000430: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000440: 7a65 2031 2e32 3720 312e 3237 2929 290a  ze 1.27 1.27))).
+00000450: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
+00000460: 7274 7920 2252 6174 6564 2056 6f6c 7461  rty "Rated Volta
+00000470: 6765 2028 566f 6c74 2922 2022 5261 7465  ge (Volt)" "Rate
+00000480: 6420 566f 6c74 6167 6522 2028 6174 2030  d Voltage" (at 0
+00000490: 202d 382e 3839 2030 290a 2020 2020 2020   -8.89 0).      
+000004a0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000004b0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000004c0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000004d0: 7065 7274 7920 226b 695f 6b65 7977 6f72  perty "ki_keywor
+000004e0: 6473 2220 226b 6579 776f 7264 7322 2028  ds" "keywords" (
+000004f0: 6174 2030 2030 2030 290a 2020 2020 2020  at 0 0 0).      
+00000500: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000510: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000520: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+00000530: 2028 7072 6f70 6572 7479 2022 6b69 5f64   (property "ki_d
+00000540: 6573 6372 6970 7469 6f6e 2220 2264 6573  escription" "des
+00000550: 6372 6970 7469 6f6e 2220 2861 7420 3020  cription" (at 0 
+00000560: 3020 3029 0a20 2020 2020 2028 6566 6665  0 0).      (effe
+00000570: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000580: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000590: 290a 2020 2020 290a 2020 2020 2873 796d  ).    ).    (sym
+000005a0: 626f 6c20 2249 504e 5f30 5f31 220a 2020  bol "IPN_0_1".  
+000005b0: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
+000005c0: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
+000005d0: 2020 2020 2028 7879 2031 2e32 3720 2d31       (xy 1.27 -1
+000005e0: 2e33 3937 290a 2020 2020 2020 2020 2020  .397).          
+000005f0: 2878 7920 322e 3135 3920 2d31 2e37 3738  (xy 2.159 -1.778
+00000600: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00000610: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+00000620: 7468 2030 2e32 3534 2920 2874 7970 6520  th 0.254) (type 
+00000630: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00000640: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+00000650: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+00000660: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
+00000670: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
+00000680: 2020 2020 2878 7920 312e 3237 202d 312e      (xy 1.27 -1.
+00000690: 3339 3729 0a20 2020 2020 2020 2020 2028  397).          (
+000006a0: 7879 2031 2e32 3720 312e 3339 3729 0a20  xy 1.27 1.397). 
+000006b0: 2020 2020 2020 2020 2028 7879 2030 2e33           (xy 0.3
+000006c0: 3831 2031 2e37 3738 290a 2020 2020 2020  81 1.778).      
+000006d0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+000006e0: 6f6b 6520 2877 6964 7468 2030 2e32 3534  oke (width 0.254
+000006f0: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+00000700: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+00000710: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+00000720: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+00000730: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000740: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000750: 2d31 2e32 3720 312e 3237 290a 2020 2020  -1.27 1.27).    
+00000760: 2020 2020 2020 2878 7920 2d31 2e32 3720        (xy -1.27 
+00000770: 2d31 2e32 3729 0a20 2020 2020 2020 2020  -1.27).         
+00000780: 2028 7879 2031 2e32 3720 3029 0a20 2020   (xy 1.27 0).   
+00000790: 2020 2020 2020 2028 7879 202d 312e 3237         (xy -1.27
+000007a0: 2031 2e32 3729 0a20 2020 2020 2020 2029   1.27).        )
+000007b0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+000007c0: 2028 7769 6474 6820 302e 3235 3429 2028   (width 0.254) (
+000007d0: 7479 7065 2064 6566 6175 6c74 2929 0a20  type default)). 
+000007e0: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
+000007f0: 7065 2062 6163 6b67 726f 756e 6429 290a  pe background)).
+00000800: 2020 2020 2020 290a 2020 2020 290a 2020        ).    ).  
+00000810: 2020 2873 796d 626f 6c20 2249 504e 5f31    (symbol "IPN_1
+00000820: 5f31 220a 2020 2020 2020 2870 696e 2070  _1".      (pin p
+00000830: 6173 7369 7665 206c 696e 6520 2861 7420  assive line (at 
+00000840: 332e 3831 2030 2031 3830 2920 286c 656e  3.81 0 180) (len
+00000850: 6774 6820 322e 3534 290a 2020 2020 2020  gth 2.54).      
+00000860: 2020 286e 616d 6520 2243 6174 686f 6465    (name "Cathode
+00000870: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+00000880: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000890: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
+000008a0: 6d62 6572 2022 3122 2028 6566 6665 6374  mber "1" (effect
+000008b0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+000008c0: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+000008d0: 2020 290a 2020 2020 2020 2870 696e 2070    ).      (pin p
+000008e0: 6173 7369 7665 206c 696e 6520 2861 7420  assive line (at 
+000008f0: 2d33 2e38 3120 3020 3029 2028 6c65 6e67  -3.81 0 0) (leng
+00000900: 7468 2032 2e35 3429 0a20 2020 2020 2020  th 2.54).       
+00000910: 2028 6e61 6d65 2022 416e 6f64 6522 2028   (name "Anode" (
+00000920: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000930: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+00000940: 290a 2020 2020 2020 2020 286e 756d 6265  ).        (numbe
+00000950: 7220 2232 2220 2865 6666 6563 7473 2028  r "2" (effects (
+00000960: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000970: 312e 3237 2929 2929 0a20 2020 2020 2029  1.27)))).      )
+00000980: 0a20 2020 2029 0a20 2029 0a29 0a         .    ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/diode-zener.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/fuse.kicad_sym`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,141 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2244 2220 2869  eference" "D" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 332e 3937   1) (at 0 -13.97
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 312e 3539   2) (at 0 -21.59
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 342e 3133 2030 290a 2020 2020 2020 2865  4.13 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3139  (id 5) (at 0 -19
-00000300: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2030 202d 332e 3831  d 6) (at 0 -3.81
-00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000390: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000003a0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000003b0: 2246 6f72 7761 7264 2056 6f6c 7461 6765  "Forward Voltage
-000003c0: 2028 566f 6c74 2922 2022 466f 7277 6172   (Volt)" "Forwar
-000003d0: 6420 566f 6c74 6167 6522 2028 6964 2037  d Voltage" (id 7
-000003e0: 2920 2861 7420 3020 2d31 312e 3433 2030  ) (at 0 -11.43 0
-000003f0: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
-00000400: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000410: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
-00000420: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-00000430: 7479 2022 506f 7765 7220 2857 6174 7473  ty "Power (Watts
-00000440: 2922 2022 5261 7465 6420 506f 7765 7222  )" "Rated Power"
-00000450: 2028 6964 2038 2920 2861 7420 3020 2d36   (id 8) (at 0 -6
-00000460: 2e33 3520 3029 0a20 2020 2020 2028 6566  .35 0).      (ef
-00000470: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000480: 6520 312e 3237 2031 2e32 3729 2929 0a20  e 1.27 1.27))). 
-00000490: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-000004a0: 7479 2022 5261 7465 6420 566f 6c74 6167  ty "Rated Voltag
-000004b0: 6520 2856 6f6c 7429 2220 2252 6174 6564  e (Volt)" "Rated
-000004c0: 2056 6f6c 7461 6765 2220 2869 6420 3929   Voltage" (id 9)
-000004d0: 2028 6174 2030 202d 382e 3839 2030 290a   (at 0 -8.89 0).
-000004e0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-000004f0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000500: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
-00000510: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-00000520: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
-00000530: 7264 7322 2028 6964 2031 3029 2028 6174  rds" (id 10) (at
-00000540: 2030 2030 2030 290a 2020 2020 2020 2865   0 0 0).      (e
-00000550: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000560: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000570: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000580: 7072 6f70 6572 7479 2022 6b69 5f64 6573  property "ki_des
-00000590: 6372 6970 7469 6f6e 2220 2264 6573 6372  cription" "descr
-000005a0: 6970 7469 6f6e 2220 2869 6420 3131 2920  iption" (id 11) 
-000005b0: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
-000005c0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000005d0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000005e0: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
-000005f0: 2020 2873 796d 626f 6c20 2249 504e 5f30    (symbol "IPN_0
-00000600: 5f31 220a 2020 2020 2020 2870 6f6c 796c  _1".      (polyl
-00000610: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000620: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
-00000630: 2e32 3720 2d31 2e33 3937 290a 2020 2020  .27 -1.397).    
-00000640: 2020 2020 2020 2878 7920 322e 3135 3920        (xy 2.159 
-00000650: 2d31 2e37 3738 290a 2020 2020 2020 2020  -1.778).        
-00000660: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
-00000670: 6520 2877 6964 7468 2030 2e32 3534 2920  e (width 0.254) 
-00000680: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000690: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-000006a0: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-000006b0: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-000006c0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-000006d0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-000006e0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-000006f0: 3237 202d 312e 3339 3729 0a20 2020 2020  27 -1.397).     
-00000700: 2020 2020 2028 7879 2031 2e32 3720 312e       (xy 1.27 1.
-00000710: 3339 3729 0a20 2020 2020 2020 2020 2028  397).          (
-00000720: 7879 2030 2e33 3831 2031 2e37 3738 290a  xy 0.381 1.778).
-00000730: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000740: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000750: 2030 2e32 3534 2920 2874 7970 6520 6465   0.254) (type de
-00000760: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000770: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000780: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-00000790: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-000007a0: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
-000007b0: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
-000007c0: 2020 2878 7920 2d31 2e32 3720 312e 3237    (xy -1.27 1.27
-000007d0: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
-000007e0: 2d31 2e32 3720 2d31 2e32 3729 0a20 2020  -1.27 -1.27).   
-000007f0: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
-00000800: 3029 0a20 2020 2020 2020 2020 2028 7879  0).          (xy
-00000810: 202d 312e 3237 2031 2e32 3729 0a20 2020   -1.27 1.27).   
-00000820: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00000830: 7374 726f 6b65 2028 7769 6474 6820 302e  stroke (width 0.
-00000840: 3235 3429 2028 7479 7065 2064 6566 6175  254) (type defau
-00000850: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00000860: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00000870: 6c6c 2028 7479 7065 2062 6163 6b67 726f  ll (type backgro
-00000880: 756e 6429 290a 2020 2020 2020 290a 2020  und)).      ).  
-00000890: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
-000008a0: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
-000008b0: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
-000008c0: 6520 2861 7420 332e 3831 2030 2031 3830  e (at 3.81 0 180
-000008d0: 2920 286c 656e 6774 6820 322e 3534 290a  ) (length 2.54).
-000008e0: 2020 2020 2020 2020 286e 616d 6520 2243          (name "C
-000008f0: 6174 686f 6465 2220 2865 6666 6563 7473  athode" (effects
-00000900: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000910: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000920: 2020 2028 6e75 6d62 6572 2022 3122 2028     (number "1" (
-00000930: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000940: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00000950: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000960: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
-00000970: 6520 2861 7420 2d33 2e38 3120 3020 3029  e (at -3.81 0 0)
-00000980: 2028 6c65 6e67 7468 2032 2e35 3429 0a20   (length 2.54). 
-00000990: 2020 2020 2020 2028 6e61 6d65 2022 416e         (name "An
-000009a0: 6f64 6522 2028 6566 6665 6374 7320 2866  ode" (effects (f
-000009b0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-000009c0: 2e32 3729 2929 290a 2020 2020 2020 2020  .27)))).        
-000009d0: 286e 756d 6265 7220 2232 2220 2865 6666  (number "2" (eff
-000009e0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-000009f0: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-00000a00: 2020 2020 2029 0a20 2020 2029 0a20 2029       ).    ).  )
-00000a10: 0a29 0a                                  .).
+000000b0: 6566 6572 656e 6365 2220 2246 2220 2861  eference" "F" (a
+000000c0: 7420 3020 322e 3739 3420 3029 0a20 2020  t 0 2.794 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2243      (property "C
+00000320: 7572 7265 6e74 2052 6174 696e 6720 2841  urrent Rating (A
+00000330: 2922 2022 5261 7465 6420 4375 7272 656e  )" "Rated Curren
+00000340: 7422 2028 6174 2030 202d 322e 3534 2030  t" (at 0 -2.54 0
+00000350: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000360: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000370: 3720 312e 3237 2929 290a 2020 2020 290a  7 1.27))).    ).
+00000380: 2020 2020 2870 726f 7065 7274 7920 2256      (property "V
+00000390: 6f6c 7461 6765 2052 6174 696e 6720 2856  oltage Rating (V
+000003a0: 2922 2022 5261 7465 6420 566f 6c74 6167  )" "Rated Voltag
+000003b0: 6522 2028 6174 2030 202d 352e 3038 2030  e" (at 0 -5.08 0
+000003c0: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+000003d0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+000003e0: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
+000003f0: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000400: 7479 2022 5061 636b 6167 6520 5479 7065  ty "Package Type
+00000410: 2220 2250 6163 6b61 6765 2054 7970 6522  " "Package Type"
+00000420: 2028 6174 2030 202d 372e 3632 2030 290a   (at 0 -7.62 0).
+00000430: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000440: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000450: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000460: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+00000470: 2022 6b69 5f6b 6579 776f 7264 7322 2022   "ki_keywords" "
+00000480: 6b65 7977 6f72 6473 2220 2861 7420 3020  keywords" (at 0 
+00000490: 3020 3029 0a20 2020 2020 2028 6566 6665  0 0).      (effe
+000004a0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+000004b0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+000004c0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000004d0: 7065 7274 7920 226b 695f 6465 7363 7269  perty "ki_descri
+000004e0: 7074 696f 6e22 2022 6465 7363 7269 7074  ption" "descript
+000004f0: 696f 6e22 2028 6174 2030 2030 2030 290a  ion" (at 0 0 0).
+00000500: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000510: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000520: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000530: 2029 0a20 2020 2028 7379 6d62 6f6c 2022   ).    (symbol "
+00000540: 4950 4e5f 305f 3122 0a20 2020 2020 2028  IPN_0_1".      (
+00000550: 7265 6374 616e 676c 6520 2873 7461 7274  rectangle (start
+00000560: 202d 332e 3831 2030 2920 2865 6e64 202d   -3.81 0) (end -
+00000570: 332e 3034 3820 3029 0a20 2020 2020 2020  3.048 0).       
+00000580: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000590: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
+000005a0: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+000005b0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+000005c0: 2020 2020 290a 2020 2020 2020 2861 7263      ).      (arc
+000005d0: 2028 7374 6172 7420 3020 3029 2028 6d69   (start 0 0) (mi
+000005e0: 6420 312e 3532 3420 2d31 2e35 3137 3429  d 1.524 -1.5174)
+000005f0: 2028 656e 6420 332e 3034 3820 3029 0a20   (end 3.048 0). 
+00000600: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+00000610: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
+00000620: 6566 6175 6c74 2929 0a20 2020 2020 2020  efault)).       
+00000630: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
+00000640: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+00000650: 2020 2872 6563 7461 6e67 6c65 2028 7374    (rectangle (st
+00000660: 6172 7420 332e 3034 3820 3029 2028 656e  art 3.048 0) (en
+00000670: 6420 332e 3831 2030 290a 2020 2020 2020  d 3.81 0).      
+00000680: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+00000690: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
+000006a0: 7429 290a 2020 2020 2020 2020 2866 696c  t)).        (fil
+000006b0: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
+000006c0: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
+000006d0: 2028 7379 6d62 6f6c 2022 4950 4e5f 315f   (symbol "IPN_1_
+000006e0: 3122 0a20 2020 2020 2028 6172 6320 2873  1".      (arc (s
+000006f0: 7461 7274 2030 2030 2920 286d 6964 202d  tart 0 0) (mid -
+00000700: 312e 3532 3420 312e 3531 3734 2920 2865  1.524 1.5174) (e
+00000710: 6e64 202d 332e 3034 3820 3029 0a20 2020  nd -3.048 0).   
+00000720: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
+00000730: 6474 6820 3029 2028 7479 7065 2064 6566  dth 0) (type def
+00000740: 6175 6c74 2929 0a20 2020 2020 2020 2028  ault)).        (
+00000750: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
+00000760: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
+00000770: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+00000780: 6520 2861 7420 2d35 2e30 3820 3020 3029  e (at -5.08 0 0)
+00000790: 2028 6c65 6e67 7468 2031 2e32 3729 0a20   (length 1.27). 
+000007a0: 2020 2020 2020 2028 6e61 6d65 2022 3122         (name "1"
+000007b0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000007c0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000007d0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
+000007e0: 6265 7220 2231 2220 2865 6666 6563 7473  ber "1" (effects
+000007f0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000800: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+00000810: 2029 0a20 2020 2020 2028 7069 6e20 7061   ).      (pin pa
+00000820: 7373 6976 6520 6c69 6e65 2028 6174 2035  ssive line (at 5
+00000830: 2e30 3820 3020 3138 3029 2028 6c65 6e67  .08 0 180) (leng
+00000840: 7468 2031 2e32 3729 0a20 2020 2020 2020  th 1.27).       
+00000850: 2028 6e61 6d65 2022 3222 2028 6566 6665   (name "2" (effe
+00000860: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000870: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000880: 2020 2020 2020 286e 756d 6265 7220 2232        (number "2
+00000890: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+000008a0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000008b0: 2929 2929 0a20 2020 2020 2029 0a20 2020  )))).      ).   
+000008c0: 2029 0a20 2029 0a29 0a                    ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/eeprom-sot23.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/eeprom-sot23.kicad_sym`

 * *Files 6% similar despite different names*

```diff
@@ -1,138 +1,133 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 696e 5f62 6f6d 2079 6573  IPN" (in_bom yes
 00000060: 2920 286f 6e5f 626f 6172 6420 7965 7329  ) (on_board yes)
 00000070: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
 00000080: 5265 6665 7265 6e63 6522 2022 5522 2028  Reference" "U" (
-00000090: 6964 2030 2920 2861 7420 3020 382e 3839  id 0) (at 0 8.89
-000000a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000c0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000000d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000000e0: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-000000f0: 6420 3129 2028 6174 2030 202d 3131 2e34  d 1) (at 0 -11.4
-00000100: 3320 3029 0a20 2020 2020 2028 6566 6665  3 0).      (effe
-00000110: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000120: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000130: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000140: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000150: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000160: 6420 3229 2028 6174 2030 202d 3139 2e30  d 2) (at 0 -19.0
-00000170: 3520 3029 0a20 2020 2020 2028 6566 6665  5 0).      (effe
-00000180: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000190: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001b0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001c0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-000001d0: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-000001e0: 3231 2e35 3920 3029 0a20 2020 2020 2028  21.59 0).      (
-000001f0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000200: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000210: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000220: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000230: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000240: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000250: 6174 2030 202d 3133 2e39 3720 3029 0a20  at 0 -13.97 0). 
-00000260: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000270: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000280: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-00000290: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000002a0: 224d 616e 7566 6163 7475 7265 7220 5061  "Manufacturer Pa
-000002b0: 7274 204e 756d 6265 7222 2022 4d50 4e22  rt Number" "MPN"
-000002c0: 2028 6964 2035 2920 2861 7420 3020 2d31   (id 5) (at 0 -1
-000002d0: 362e 3531 2030 290a 2020 2020 2020 2865  6.51 0).      (e
-000002e0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-000002f0: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000300: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000310: 7072 6f70 6572 7479 2022 5061 7274 204e  property "Part N
-00000320: 756d 6265 7222 2022 5661 6c75 6522 2028  umber" "Value" (
-00000330: 6964 2036 2920 2861 7420 3020 2d38 2e38  id 6) (at 0 -8.8
-00000340: 3920 3029 0a20 2020 2020 2028 6566 6665  9 0).      (effe
-00000350: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000360: 312e 3237 2031 2e32 3729 2929 0a20 2020  1.27 1.27))).   
-00000370: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-00000380: 2022 6b69 5f6b 6579 776f 7264 7322 2022   "ki_keywords" "
-00000390: 6b65 7977 6f72 6473 2220 2869 6420 3729  keywords" (id 7)
-000003a0: 2028 6174 2030 2030 2030 290a 2020 2020   (at 0 0 0).    
-000003b0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-000003c0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-000003d0: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
-000003e0: 2020 2028 7072 6f70 6572 7479 2022 6b69     (property "ki
-000003f0: 5f64 6573 6372 6970 7469 6f6e 2220 2264  _description" "d
-00000400: 6573 6372 6970 7469 6f6e 2220 2869 6420  escription" (id 
-00000410: 3829 2028 6174 2030 2030 2030 290a 2020  8) (at 0 0 0).  
-00000420: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000430: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000440: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-00000450: 0a20 2020 2028 7379 6d62 6f6c 2022 4950  .    (symbol "IP
-00000460: 4e5f 305f 3122 0a20 2020 2020 2028 7265  N_0_1".      (re
-00000470: 6374 616e 676c 6520 2873 7461 7274 202d  ctangle (start -
-00000480: 352e 3038 2037 2e36 3229 2028 656e 6420  5.08 7.62) (end 
-00000490: 352e 3038 202d 372e 3632 290a 2020 2020  5.08 -7.62).    
-000004a0: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-000004b0: 7468 2030 2e32 3534 2920 2874 7970 6520  th 0.254) (type 
-000004c0: 6465 6661 756c 7429 2028 636f 6c6f 7220  default) (color 
-000004d0: 3020 3020 3020 3029 290a 2020 2020 2020  0 0 0 0)).      
-000004e0: 2020 2866 696c 6c20 2874 7970 6520 6261    (fill (type ba
-000004f0: 636b 6772 6f75 6e64 2929 0a20 2020 2020  ckground)).     
-00000500: 2029 0a20 2020 2029 0a20 2020 2028 7379   ).    ).    (sy
-00000510: 6d62 6f6c 2022 4950 4e5f 315f 3122 0a20  mbol "IPN_1_1". 
-00000520: 2020 2020 2028 7069 6e20 7061 7373 6976       (pin passiv
-00000530: 6520 6c69 6e65 2028 6174 202d 372e 3632  e line (at -7.62
-00000540: 2030 2030 2920 286c 656e 6774 6820 322e   0 0) (length 2.
-00000550: 3534 290a 2020 2020 2020 2020 286e 616d  54).        (nam
-00000560: 6520 2253 434c 2220 2865 6666 6563 7473  e "SCL" (effects
-00000570: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000580: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000590: 2020 2028 6e75 6d62 6572 2022 3122 2028     (number "1" (
-000005a0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-000005b0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-000005c0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-000005d0: 2870 696e 2070 6f77 6572 5f69 6e20 6c69  (pin power_in li
-000005e0: 6e65 2028 6174 2037 2e36 3220 2d35 2e30  ne (at 7.62 -5.0
-000005f0: 3820 3138 3029 2028 6c65 6e67 7468 2032  8 180) (length 2
-00000600: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
-00000610: 6d65 2022 5653 5322 2028 6566 6665 6374  me "VSS" (effect
-00000620: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000630: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-00000640: 2020 2020 286e 756d 6265 7220 2232 2220      (number "2" 
-00000650: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000660: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000670: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00000680: 2028 7069 6e20 7061 7373 6976 6520 6c69   (pin passive li
-00000690: 6e65 2028 6174 202d 372e 3632 202d 352e  ne (at -7.62 -5.
-000006a0: 3038 2030 2920 286c 656e 6774 6820 322e  08 0) (length 2.
-000006b0: 3534 290a 2020 2020 2020 2020 286e 616d  54).        (nam
-000006c0: 6520 2253 4441 2220 2865 6666 6563 7473  e "SDA" (effects
-000006d0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-000006e0: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-000006f0: 2020 2028 6e75 6d62 6572 2022 3322 2028     (number "3" (
-00000700: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000710: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00000720: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000730: 2870 696e 2070 6f77 6572 5f69 6e20 6c69  (pin power_in li
-00000740: 6e65 2028 6174 202d 372e 3632 2035 2e30  ne (at -7.62 5.0
-00000750: 3820 3029 2028 6c65 6e67 7468 2032 2e35  8 0) (length 2.5
-00000760: 3429 0a20 2020 2020 2020 2028 6e61 6d65  4).        (name
-00000770: 2022 5643 4322 2028 6566 6665 6374 7320   "VCC" (effects 
-00000780: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000790: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-000007a0: 2020 286e 756d 6265 7220 2234 2220 2865    (number "4" (e
-000007b0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-000007c0: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-000007d0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-000007e0: 7069 6e20 7061 7373 6976 6520 6c69 6e65  pin passive line
-000007f0: 2028 6174 2037 2e36 3220 352e 3038 2031   (at 7.62 5.08 1
-00000800: 3830 2920 286c 656e 6774 6820 322e 3534  80) (length 2.54
-00000810: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
-00000820: 2257 5022 2028 6566 6665 6374 7320 2866  "WP" (effects (f
-00000830: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000840: 2e32 3729 2929 290a 2020 2020 2020 2020  .27)))).        
-00000850: 286e 756d 6265 7220 2235 2220 2865 6666  (number "5" (eff
-00000860: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000870: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-00000880: 2020 2020 2029 0a20 2020 2029 0a20 2029       ).    ).  )
-00000890: 0a29 0a                                  .).
+00000090: 6174 2030 2038 2e38 3920 3029 0a20 2020  at 0 8.89 0).   
+000000a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000c0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+000000d0: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+000000e0: 2022 4950 4e22 2028 6174 2030 202d 3131   "IPN" (at 0 -11
+000000f0: 2e34 3320 3029 0a20 2020 2020 2028 6566  .43 0).      (ef
+00000100: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000110: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000120: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000130: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000140: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000150: 2861 7420 3020 2d31 392e 3035 2030 290a  (at 0 -19.05 0).
+00000160: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000170: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000180: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000190: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001a0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001b0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001c0: 2030 202d 3231 2e35 3920 3029 0a20 2020   0 -21.59 0).   
+000001d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000001e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000001f0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000200: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000210: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000220: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000230: 3020 2d31 332e 3937 2030 290a 2020 2020  0 -13.97 0).    
+00000240: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000250: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000260: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000270: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000280: 6e75 6661 6374 7572 6572 2050 6172 7420  nufacturer Part 
+00000290: 4e75 6d62 6572 2220 224d 504e 2220 2861  Number" "MPN" (a
+000002a0: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
+000002b0: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+000002c0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000002d0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+000002e0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+000002f0: 5061 7274 204e 756d 6265 7222 2022 5661  Part Number" "Va
+00000300: 6c75 6522 2028 6174 2030 202d 382e 3839  lue" (at 0 -8.89
+00000310: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
+00000320: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+00000330: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
+00000340: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+00000350: 226b 695f 6b65 7977 6f72 6473 2220 226b  "ki_keywords" "k
+00000360: 6579 776f 7264 7322 2028 6174 2030 2030  eywords" (at 0 0
+00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
+00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+00000390: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
+000003a0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+000003b0: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
+000003c0: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
+000003d0: 6f6e 2220 2861 7420 3020 3020 3029 0a20  on" (at 0 0 0). 
+000003e0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000003f0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+00000400: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+00000410: 290a 2020 2020 2873 796d 626f 6c20 2249  ).    (symbol "I
+00000420: 504e 5f30 5f31 220a 2020 2020 2020 2872  PN_0_1".      (r
+00000430: 6563 7461 6e67 6c65 2028 7374 6172 7420  ectangle (start 
+00000440: 2d35 2e30 3820 372e 3632 2920 2865 6e64  -5.08 7.62) (end
+00000450: 2035 2e30 3820 2d37 2e36 3229 0a20 2020   5.08 -7.62).   
+00000460: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
+00000470: 6474 6820 302e 3235 3429 2028 7479 7065  dth 0.254) (type
+00000480: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000490: 2020 2028 6669 6c6c 2028 7479 7065 2062     (fill (type b
+000004a0: 6163 6b67 726f 756e 6429 290a 2020 2020  ackground)).    
+000004b0: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
+000004c0: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
+000004d0: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
+000004e0: 7665 206c 696e 6520 2861 7420 2d37 2e36  ve line (at -7.6
+000004f0: 3220 3020 3029 2028 6c65 6e67 7468 2032  2 0 0) (length 2
+00000500: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
+00000510: 6d65 2022 5343 4c22 2028 6566 6665 6374  me "SCL" (effect
+00000520: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000530: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+00000540: 2020 2020 286e 756d 6265 7220 2231 2220      (number "1" 
+00000550: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000560: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000570: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+00000580: 2028 7069 6e20 706f 7765 725f 696e 206c   (pin power_in l
+00000590: 696e 6520 2861 7420 372e 3632 202d 352e  ine (at 7.62 -5.
+000005a0: 3038 2031 3830 2920 286c 656e 6774 6820  08 180) (length 
+000005b0: 322e 3534 290a 2020 2020 2020 2020 286e  2.54).        (n
+000005c0: 616d 6520 2256 5353 2220 2865 6666 6563  ame "VSS" (effec
+000005d0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000005e0: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+000005f0: 2020 2020 2028 6e75 6d62 6572 2022 3222       (number "2"
+00000600: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000610: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000620: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
+00000630: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
+00000640: 696e 6520 2861 7420 2d37 2e36 3220 2d35  ine (at -7.62 -5
+00000650: 2e30 3820 3029 2028 6c65 6e67 7468 2032  .08 0) (length 2
+00000660: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
+00000670: 6d65 2022 5344 4122 2028 6566 6665 6374  me "SDA" (effect
+00000680: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000690: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+000006a0: 2020 2020 286e 756d 6265 7220 2233 2220      (number "3" 
+000006b0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000006c0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000006d0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+000006e0: 2028 7069 6e20 706f 7765 725f 696e 206c   (pin power_in l
+000006f0: 696e 6520 2861 7420 2d37 2e36 3220 352e  ine (at -7.62 5.
+00000700: 3038 2030 2920 286c 656e 6774 6820 322e  08 0) (length 2.
+00000710: 3534 290a 2020 2020 2020 2020 286e 616d  54).        (nam
+00000720: 6520 2256 4343 2220 2865 6666 6563 7473  e "VCC" (effects
+00000730: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000740: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+00000750: 2020 2028 6e75 6d62 6572 2022 3422 2028     (number "4" (
+00000760: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000770: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+00000780: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
+00000790: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+000007a0: 6520 2861 7420 372e 3632 2035 2e30 3820  e (at 7.62 5.08 
+000007b0: 3138 3029 2028 6c65 6e67 7468 2032 2e35  180) (length 2.5
+000007c0: 3429 0a20 2020 2020 2020 2028 6e61 6d65  4).        (name
+000007d0: 2022 5750 2220 2865 6666 6563 7473 2028   "WP" (effects (
+000007e0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000007f0: 312e 3237 2929 2929 0a20 2020 2020 2020  1.27)))).       
+00000800: 2028 6e75 6d62 6572 2022 3522 2028 6566   (number "5" (ef
+00000810: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000820: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
+00000830: 2020 2020 2020 290a 2020 2020 290a 2020        ).    ).  
+00000840: 290a 290a                                ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/ferrite-bead.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/crystal-2p.kicad_sym`

 * *Files 8% similar despite different names*

```diff
@@ -1,162 +1,159 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2246 4222 2028  eference" "FB" (
-000000c0: 6964 2030 2920 2861 7420 3020 322e 3534  id 0) (at 0 2.54
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2249 6e64 7563 7461  roperty "Inducta
-00000350: 6e63 6520 2848 656e 7279 2922 2022 5661  nce (Henry)" "Va
-00000360: 6c75 6522 2028 6964 2036 2920 2861 7420  lue" (id 6) (at 
-00000370: 3020 2d32 2e35 3420 3029 0a20 2020 2020  0 -2.54 0).     
-00000380: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000390: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000003a0: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
-000003b0: 6f70 6572 7479 2022 4375 7272 656e 7420  operty "Current 
-000003c0: 5261 7469 6e67 2028 416d 7065 7265 2922  Rating (Ampere)"
-000003d0: 2022 5261 7465 6420 4375 7272 656e 7422   "Rated Current"
-000003e0: 2028 6964 2037 2920 2861 7420 3020 2d35   (id 7) (at 0 -5
-000003f0: 2e30 3820 3029 0a20 2020 2020 2028 6566  .08 0).      (ef
-00000400: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000410: 6520 312e 3237 2031 2e32 3729 2929 0a20  e 1.27 1.27))). 
-00000420: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-00000430: 7479 2022 4553 5220 284f 686d 2922 2022  ty "ESR (Ohm)" "
-00000440: 4553 5222 2028 6964 2038 2920 2861 7420  ESR" (id 8) (at 
-00000450: 3020 2d37 2e36 3220 3029 0a20 2020 2020  0 -7.62 0).     
-00000460: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000470: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000480: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
-00000490: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-000004a0: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
-000004b0: 7264 7322 2028 6964 2039 2920 2861 7420  rds" (id 9) (at 
-000004c0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000004e0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-000004f0: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000500: 726f 7065 7274 7920 226b 695f 6465 7363  roperty "ki_desc
-00000510: 7269 7074 696f 6e22 2022 6465 7363 7269  ription" "descri
-00000520: 7074 696f 6e22 2028 6964 2031 3029 2028  ption" (id 10) (
-00000530: 6174 2030 2030 2030 290a 2020 2020 2020  at 0 0 0).      
-00000540: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000550: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000560: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000570: 2028 7379 6d62 6f6c 2022 4950 4e5f 305f   (symbol "IPN_0_
-00000580: 3122 0a20 2020 2020 2028 706f 6c79 6c69  1".      (polyli
-00000590: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-000005a0: 2020 2020 2020 2020 2020 2878 7920 2d34            (xy -4
-000005b0: 2e33 3138 2030 290a 2020 2020 2020 2020  .318 0).        
-000005c0: 2020 2878 7920 2d34 2e30 3634 2030 290a    (xy -4.064 0).
-000005d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000005e0: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-000005f0: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
-00000600: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-00000610: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
-00000620: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
-00000630: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
-00000640: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
-00000650: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-00000660: 7920 2d31 2e32 3720 3029 0a20 2020 2020  y -1.27 0).     
-00000670: 2020 2020 2028 7879 2031 2e32 3720 3029       (xy 1.27 0)
-00000680: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00000690: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-000006a0: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-000006b0: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-000006c0: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-000006d0: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
-000006e0: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-000006f0: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-00000700: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-00000710: 7879 2034 2e30 3634 2030 290a 2020 2020  xy 4.064 0).    
-00000720: 2020 2020 2020 2878 7920 342e 3331 3820        (xy 4.318 
-00000730: 3029 0a20 2020 2020 2020 2029 0a20 2020  0).        ).   
-00000740: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
-00000750: 6474 6820 3029 2028 7479 7065 2064 6566  dth 0) (type def
-00000760: 6175 6c74 2920 2863 6f6c 6f72 2030 2030  ault) (color 0 0
-00000770: 2030 2030 2929 0a20 2020 2020 2020 2028   0 0)).        (
-00000780: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
-00000790: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-000007a0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
-000007b0: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
-000007c0: 2028 7879 202d 322e 3534 2031 2e32 3729   (xy -2.54 1.27)
-000007d0: 0a20 2020 2020 2020 2020 2028 7879 202d  .          (xy -
-000007e0: 322e 3534 202d 312e 3237 290a 2020 2020  2.54 -1.27).    
-000007f0: 2020 2020 2020 2878 7920 322e 3534 202d        (xy 2.54 -
-00000800: 312e 3237 290a 2020 2020 2020 2020 2020  1.27).          
-00000810: 2878 7920 322e 3534 2031 2e32 3729 0a20  (xy 2.54 1.27). 
-00000820: 2020 2020 2020 2020 2028 7879 202d 322e           (xy -2.
-00000830: 3534 2031 2e32 3729 0a20 2020 2020 2020  54 1.27).       
-00000840: 2029 0a20 2020 2020 2020 2028 7374 726f   ).        (stro
-00000850: 6b65 2028 7769 6474 6820 3029 2028 7479  ke (width 0) (ty
-00000860: 7065 2064 6566 6175 6c74 2920 2863 6f6c  pe default) (col
-00000870: 6f72 2030 2030 2030 2030 2929 0a20 2020  or 0 0 0 0)).   
-00000880: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
-00000890: 206e 6f6e 6529 290a 2020 2020 2020 290a   none)).      ).
-000008a0: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
-000008b0: 6c20 2249 504e 5f31 5f31 220a 2020 2020  l "IPN_1_1".    
-000008c0: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
-000008d0: 696e 6520 2861 7420 2d35 2e30 3820 3020  ine (at -5.08 0 
-000008e0: 3029 2028 6c65 6e67 7468 2032 2e35 3429  0) (length 2.54)
-000008f0: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
-00000900: 3122 2028 6566 6665 6374 7320 2866 6f6e  1" (effects (fon
-00000910: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000920: 3729 2929 290a 2020 2020 2020 2020 286e  7)))).        (n
-00000930: 756d 6265 7220 2231 2220 2865 6666 6563  umber "1" (effec
-00000940: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000950: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-00000960: 2020 2029 0a20 2020 2020 2028 7069 6e20     ).      (pin 
-00000970: 7061 7373 6976 6520 6c69 6e65 2028 6174  passive line (at
-00000980: 2035 2e30 3820 3020 3138 3029 2028 6c65   5.08 0 180) (le
-00000990: 6e67 7468 2032 2e35 3429 0a20 2020 2020  ngth 2.54).     
-000009a0: 2020 2028 6e61 6d65 2022 3222 2028 6566     (name "2" (ef
-000009b0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000009c0: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-000009d0: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-000009e0: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
-000009f0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000a00: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-00000a10: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2259 2220 2861  eference" "Y" (a
+000000c0: 7420 3020 352e 3038 2030 290a 2020 2020  t 0 5.08 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 352e  "IPN" (at 0 -15.
+00000120: 3234 2030 290a 2020 2020 2020 2865 6666  24 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3230 2e33 3220 3029 0a20  at 0 -20.32 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 322e 3836 2030 290a 2020 2020  0 -22.86 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3137 2e37 3820 3029 0a20 2020 2020   -17.78 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 372e 3632 2030 290a 2020 2020   0 -7.62 0).    
+000002e0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000002f0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000300: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000310: 726f 7065 7274 7920 2246 7265 7175 656e  roperty "Frequen
+00000320: 6379 2220 2256 616c 7565 2220 2861 7420  cy" "Value" (at 
+00000330: 3020 2d35 2e30 3820 3029 0a20 2020 2020  0 -5.08 0).     
+00000340: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000350: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000360: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000370: 6f70 6572 7479 2022 4c6f 6164 2043 6170  operty "Load Cap
+00000380: 6163 6974 616e 6365 2028 4661 7261 6429  acitance (Farad)
+00000390: 2220 224c 6f61 6420 4361 7061 6369 7461  " "Load Capacita
+000003a0: 6e63 6522 2028 6174 2030 202d 3130 2e31  nce" (at 0 -10.1
+000003b0: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
+000003c0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+000003d0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+000003e0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000003f0: 7065 7274 7920 2250 6163 6b61 6765 2053  perty "Package S
+00000400: 697a 6522 2022 5061 636b 6167 6520 5369  ize" "Package Si
+00000410: 7a65 2220 2861 7420 3020 2d31 322e 3720  ze" (at 0 -12.7 
+00000420: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000430: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000440: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
+00000450: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
+00000460: 7274 7920 226b 695f 6b65 7977 6f72 6473  rty "ki_keywords
+00000470: 2220 226b 6579 776f 7264 7322 2028 6174  " "keywords" (at
+00000480: 2030 2030 2030 290a 2020 2020 2020 2865   0 0 0).      (e
+00000490: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+000004a0: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
+000004b0: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
+000004c0: 7072 6f70 6572 7479 2022 6b69 5f64 6573  property "ki_des
+000004d0: 6372 6970 7469 6f6e 2220 2264 6573 6372  cription" "descr
+000004e0: 6970 7469 6f6e 2220 2861 7420 3020 3020  iption" (at 0 0 
+000004f0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+00000500: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000510: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
+00000520: 2020 2020 290a 2020 2020 2873 796d 626f      ).    (symbo
+00000530: 6c20 2249 504e 5f31 5f31 220a 2020 2020  l "IPN_1_1".    
+00000540: 2020 2872 6563 7461 6e67 6c65 2028 7374    (rectangle (st
+00000550: 6172 7420 2d31 2e30 3136 2033 2e30 3438  art -1.016 3.048
+00000560: 2920 2865 6e64 2031 2e30 3136 202d 332e  ) (end 1.016 -3.
+00000570: 3034 3829 0a20 2020 2020 2020 2028 7374  048).        (st
+00000580: 726f 6b65 2028 7769 6474 6820 302e 3235  roke (width 0.25
+00000590: 3429 2028 7479 7065 2064 6566 6175 6c74  4) (type default
+000005a0: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+000005b0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+000005c0: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+000005d0: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000005e0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000005f0: 202d 322e 3534 2030 290a 2020 2020 2020   -2.54 0).      
+00000600: 2020 2020 2878 7920 2d31 2e37 3738 2030      (xy -1.778 0
+00000610: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00000620: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+00000630: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
+00000640: 756c 7429 290a 2020 2020 2020 2020 2866  ult)).        (f
+00000650: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
+00000660: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
+00000670: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
+00000680: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
+00000690: 2878 7920 322e 3534 2030 290a 2020 2020  (xy 2.54 0).    
+000006a0: 2020 2020 2020 2878 7920 312e 3737 3820        (xy 1.778 
+000006b0: 3029 0a20 2020 2020 2020 2029 0a20 2020  0).        ).   
+000006c0: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
+000006d0: 6474 6820 3029 2028 7479 7065 2064 6566  dth 0) (type def
+000006e0: 6175 6c74 2929 0a20 2020 2020 2020 2028  ault)).        (
+000006f0: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
+00000700: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
+00000710: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000720: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000730: 2028 7879 202d 312e 3737 3820 322e 3534   (xy -1.778 2.54
+00000740: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000750: 2d31 2e37 3738 2030 290a 2020 2020 2020  -1.778 0).      
+00000760: 2020 2020 2878 7920 2d31 2e37 3738 202d      (xy -1.778 -
+00000770: 322e 3534 290a 2020 2020 2020 2020 290a  2.54).        ).
+00000780: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
+00000790: 2877 6964 7468 2030 2920 2874 7970 6520  (width 0) (type 
+000007a0: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+000007b0: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+000007c0: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+000007d0: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
+000007e0: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
+000007f0: 2020 2020 2878 7920 312e 3737 3820 322e      (xy 1.778 2.
+00000800: 3534 290a 2020 2020 2020 2020 2020 2878  54).          (x
+00000810: 7920 312e 3737 3820 3029 0a20 2020 2020  y 1.778 0).     
+00000820: 2020 2020 2028 7879 2031 2e37 3738 202d       (xy 1.778 -
+00000830: 322e 3534 290a 2020 2020 2020 2020 290a  2.54).        ).
+00000840: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
+00000850: 2877 6964 7468 2030 2920 2874 7970 6520  (width 0) (type 
+00000860: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00000870: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+00000880: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+00000890: 2020 2028 7069 6e20 7061 7373 6976 6520     (pin passive 
+000008a0: 6c69 6e65 2028 6174 202d 352e 3038 2030  line (at -5.08 0
+000008b0: 2030 2920 286c 656e 6774 6820 322e 3534   0) (length 2.54
+000008c0: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
+000008d0: 2231 2220 2865 6666 6563 7473 2028 666f  "1" (effects (fo
+000008e0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000008f0: 3237 2929 2929 0a20 2020 2020 2020 2028  27)))).        (
+00000900: 6e75 6d62 6572 2022 3122 2028 6566 6665  number "1" (effe
+00000910: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000920: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000930: 2020 2020 290a 2020 2020 2020 2870 696e      ).      (pin
+00000940: 2070 6173 7369 7665 206c 696e 6520 2861   passive line (a
+00000950: 7420 352e 3038 2030 2031 3830 2920 286c  t 5.08 0 180) (l
+00000960: 656e 6774 6820 322e 3534 290a 2020 2020  ength 2.54).    
+00000970: 2020 2020 286e 616d 6520 2232 2220 2865      (name "2" (e
+00000980: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000990: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+000009a0: 0a20 2020 2020 2020 2028 6e75 6d62 6572  .        (number
+000009b0: 2022 3222 2028 6566 6665 6374 7320 2866   "2" (effects (f
+000009c0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000009d0: 2e32 3729 2929 290a 2020 2020 2020 290a  .27)))).      ).
+000009e0: 2020 2020 290a 2020 290a 290a                ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/fuse.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/inductor.kicad_sym`

 * *Files 12% similar despite different names*

```diff
@@ -1,150 +1,142 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2246 2220 2869  eference" "F" (i
-000000c0: 6420 3029 2028 6174 2030 2032 2e37 3934  d 0) (at 0 2.794
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2243 7572 7265 6e74  roperty "Current
-00000350: 2052 6174 696e 6720 2841 2922 2022 5261   Rating (A)" "Ra
-00000360: 7465 6420 4375 7272 656e 7422 2028 6964  ted Current" (id
-00000370: 2036 2920 2861 7420 3020 2d32 2e35 3420   6) (at 0 -2.54 
-00000380: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000390: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000003a0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-000003b0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000003c0: 566f 6c74 6167 6520 5261 7469 6e67 2028  Voltage Rating (
-000003d0: 5629 2220 2252 6174 6564 2056 6f6c 7461  V)" "Rated Volta
-000003e0: 6765 2220 2869 6420 3729 2028 6174 2030  ge" (id 7) (at 0
-000003f0: 202d 352e 3038 2030 290a 2020 2020 2020   -5.08 0).      
-00000400: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000410: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000420: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000430: 2028 7072 6f70 6572 7479 2022 5061 636b   (property "Pack
-00000440: 6167 6520 5479 7065 2220 2250 6163 6b61  age Type" "Packa
-00000450: 6765 2054 7970 6522 2028 6964 2038 2920  ge Type" (id 8) 
-00000460: 2861 7420 3020 2d37 2e36 3220 3029 0a20  (at 0 -7.62 0). 
-00000470: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000480: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000490: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-000004a0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000004b0: 226b 695f 6b65 7977 6f72 6473 2220 226b  "ki_keywords" "k
-000004c0: 6579 776f 7264 7322 2028 6964 2039 2920  eywords" (id 9) 
-000004d0: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
-000004e0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000004f0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000500: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
-00000510: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-00000520: 6465 7363 7269 7074 696f 6e22 2022 6465  description" "de
-00000530: 7363 7269 7074 696f 6e22 2028 6964 2031  scription" (id 1
-00000540: 3029 2028 6174 2030 2030 2030 290a 2020  0) (at 0 0 0).  
-00000550: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000560: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000570: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-00000580: 0a20 2020 2028 7379 6d62 6f6c 2022 4950  .    (symbol "IP
-00000590: 4e5f 305f 3122 0a20 2020 2020 2028 7265  N_0_1".      (re
-000005a0: 6374 616e 676c 6520 2873 7461 7274 202d  ctangle (start -
-000005b0: 332e 3831 2030 2920 2865 6e64 202d 332e  3.81 0) (end -3.
-000005c0: 3034 3820 3029 0a20 2020 2020 2020 2028  048 0).        (
-000005d0: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-000005e0: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000005f0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000600: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000610: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-00000620: 2020 290a 2020 2020 2020 2861 7263 2028    ).      (arc (
-00000630: 7374 6172 7420 3020 3029 2028 6d69 6420  start 0 0) (mid 
-00000640: 312e 3532 3420 2d31 2e35 3234 2920 2865  1.524 -1.524) (e
-00000650: 6e64 2033 2e30 3438 2030 290a 2020 2020  nd 3.048 0).    
-00000660: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-00000670: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-00000680: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-00000690: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-000006a0: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-000006b0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-000006c0: 7265 6374 616e 676c 6520 2873 7461 7274  rectangle (start
-000006d0: 2033 2e30 3438 2030 2920 2865 6e64 2033   3.048 0) (end 3
-000006e0: 2e38 3120 3029 0a20 2020 2020 2020 2028  .81 0).        (
-000006f0: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00000700: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00000710: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000720: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000730: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-00000740: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
-00000750: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
-00000760: 2020 2020 2020 2861 7263 2028 7374 6172        (arc (star
-00000770: 7420 3020 3029 2028 6d69 6420 2d31 2e35  t 0 0) (mid -1.5
-00000780: 3234 2031 2e35 3234 2920 2865 6e64 202d  24 1.524) (end -
-00000790: 332e 3034 3820 3029 0a20 2020 2020 2020  3.048 0).       
-000007a0: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
-000007b0: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
-000007c0: 2920 2863 6f6c 6f72 2030 2030 2030 2030  ) (color 0 0 0 0
-000007d0: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
-000007e0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
-000007f0: 2020 2020 290a 2020 2020 2020 2870 696e      ).      (pin
-00000800: 2070 6173 7369 7665 206c 696e 6520 2861   passive line (a
-00000810: 7420 2d35 2e30 3820 3020 3029 2028 6c65  t -5.08 0 0) (le
-00000820: 6e67 7468 2031 2e32 3729 0a20 2020 2020  ngth 1.27).     
-00000830: 2020 2028 6e61 6d65 2022 3122 2028 6566     (name "1" (ef
-00000840: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000850: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-00000860: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-00000870: 2231 2220 2865 6666 6563 7473 2028 666f  "1" (effects (fo
-00000880: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000890: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-000008a0: 2020 2020 2028 7069 6e20 7061 7373 6976       (pin passiv
-000008b0: 6520 6c69 6e65 2028 6174 2035 2e30 3820  e line (at 5.08 
-000008c0: 3020 3138 3029 2028 6c65 6e67 7468 2031  0 180) (length 1
-000008d0: 2e32 3729 0a20 2020 2020 2020 2028 6e61  .27).        (na
-000008e0: 6d65 2022 3222 2028 6566 6665 6374 7320  me "2" (effects 
-000008f0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000900: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000910: 2020 286e 756d 6265 7220 2232 2220 2865    (number "2" (e
-00000920: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000930: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000940: 0a20 2020 2020 2029 0a20 2020 2029 0a20  .      ).    ). 
-00000950: 2029 0a29 0a                              ).).
+000000b0: 6566 6572 656e 6365 2220 224c 2220 2861  eference" "L" (a
+000000c0: 7420 3020 322e 3534 2030 290a 2020 2020  t 0 2.54 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d38 2e38  "IPN" (at 0 -8.8
+00000120: 3920 3029 0a20 2020 2020 2028 6566 6665  9 0).      (effe
+00000130: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000140: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000150: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+00000160: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
+00000170: 2220 2246 6f6f 7470 7269 6e74 2220 2861  " "Footprint" (a
+00000180: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
+00000190: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+000001a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000001b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+000001c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+000001d0: 4461 7461 7368 6565 7422 2022 696e 7665  Datasheet" "inve
+000001e0: 6e74 7265 655f 7572 6c22 2028 6174 2030  ntree_url" (at 0
+000001f0: 202d 3139 2e30 3520 3029 0a20 2020 2020   -19.05 0).     
+00000200: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000210: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000220: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+00000230: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+00000240: 7566 6163 7475 7265 7222 2022 4d61 6e75  ufacturer" "Manu
+00000250: 6661 6374 7572 6572 2220 2861 7420 3020  facturer" (at 0 
+00000260: 2d31 312e 3433 2030 290a 2020 2020 2020  -11.43 0).      
+00000270: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+00000280: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+00000290: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+000002a0: 2028 7072 6f70 6572 7479 2022 4d61 6e75   (property "Manu
+000002b0: 6661 6374 7572 6572 2050 6172 7420 4e75  facturer Part Nu
+000002c0: 6d62 6572 2220 224d 504e 2220 2861 7420  mber" "MPN" (at 
+000002d0: 3020 2d31 332e 3937 2030 290a 2020 2020  0 -13.97 0).    
+000002e0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000002f0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000300: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000310: 2020 2028 7072 6f70 6572 7479 2022 496e     (property "In
+00000320: 6475 6374 616e 6365 2028 4865 6e72 7929  ductance (Henry)
+00000330: 2220 2256 616c 7565 2220 2861 7420 3020  " "Value" (at 0 
+00000340: 2d31 2e32 3720 3029 0a20 2020 2020 2028  -1.27 0).      (
+00000350: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000360: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+00000370: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000380: 6572 7479 2022 4375 7272 656e 7420 5261  erty "Current Ra
+00000390: 7469 6e67 2028 416d 7065 7265 2922 2022  ting (Ampere)" "
+000003a0: 5261 7465 6420 4375 7272 656e 7422 2028  Rated Current" (
+000003b0: 6174 2030 202d 332e 3831 2030 290a 2020  at 0 -3.81 0).  
+000003c0: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+000003d0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+000003e0: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
+000003f0: 2870 726f 7065 7274 7920 2245 5352 2028  (property "ESR (
+00000400: 4f68 6d29 2220 2245 5352 2220 2861 7420  Ohm)" "ESR" (at 
+00000410: 3020 2d36 2e33 3520 3029 0a20 2020 2020  0 -6.35 0).     
+00000420: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000430: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000440: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+00000450: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
+00000460: 6b65 7977 6f72 6473 2220 226b 6579 776f  keywords" "keywo
+00000470: 7264 7322 2028 6174 2030 2030 2030 290a  rds" (at 0 0 0).
+00000480: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000490: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000004a0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000004b0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000004c0: 2022 6b69 5f64 6573 6372 6970 7469 6f6e   "ki_description
+000004d0: 2220 2264 6573 6372 6970 7469 6f6e 2220  " "description" 
+000004e0: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
+000004f0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000500: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000510: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+00000520: 2020 2873 796d 626f 6c20 2249 504e 5f30    (symbol "IPN_0
+00000530: 5f31 220a 2020 2020 2020 2861 7263 2028  _1".      (arc (
+00000540: 7374 6172 7420 2d31 2e39 3035 2030 2920  start -1.905 0) 
+00000550: 286d 6964 202d 322e 3835 3735 2030 2e39  (mid -2.8575 0.9
+00000560: 3339 3929 2028 656e 6420 2d33 2e38 3120  399) (end -3.81 
+00000570: 3029 0a20 2020 2020 2020 2028 7374 726f  0).        (stro
+00000580: 6b65 2028 7769 6474 6820 3029 2028 7479  ke (width 0) (ty
+00000590: 7065 2064 6566 6175 6c74 2929 0a20 2020  pe default)).   
+000005a0: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
+000005b0: 206e 6f6e 6529 290a 2020 2020 2020 290a   none)).      ).
+000005c0: 2020 2020 2020 2861 7263 2028 7374 6172        (arc (star
+000005d0: 7420 3020 3029 2028 6d69 6420 2d30 2e39  t 0 0) (mid -0.9
+000005e0: 3532 3520 302e 3933 3939 2920 2865 6e64  525 0.9399) (end
+000005f0: 202d 312e 3930 3520 3029 0a20 2020 2020   -1.905 0).     
+00000600: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
+00000610: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
+00000620: 6c74 2929 0a20 2020 2020 2020 2028 6669  lt)).        (fi
+00000630: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
+00000640: 2020 2020 2020 290a 2020 2020 2020 2861        ).      (a
+00000650: 7263 2028 7374 6172 7420 312e 3930 3520  rc (start 1.905 
+00000660: 3029 2028 6d69 6420 302e 3935 3235 2030  0) (mid 0.9525 0
+00000670: 2e39 3339 3929 2028 656e 6420 3020 3029  .9399) (end 0 0)
+00000680: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000690: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+000006a0: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+000006b0: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+000006c0: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+000006d0: 2020 2020 2861 7263 2028 7374 6172 7420      (arc (start 
+000006e0: 332e 3831 2030 2920 286d 6964 2032 2e38  3.81 0) (mid 2.8
+000006f0: 3537 3520 302e 3933 3939 2920 2865 6e64  575 0.9399) (end
+00000700: 2031 2e39 3035 2030 290a 2020 2020 2020   1.905 0).      
+00000710: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+00000720: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
+00000730: 7429 290a 2020 2020 2020 2020 2866 696c  t)).        (fil
+00000740: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
+00000750: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
+00000760: 2028 7379 6d62 6f6c 2022 4950 4e5f 315f   (symbol "IPN_1_
+00000770: 3122 0a20 2020 2020 2028 7069 6e20 7061  1".      (pin pa
+00000780: 7373 6976 6520 6c69 6e65 2028 6174 202d  ssive line (at -
+00000790: 362e 3335 2030 2030 2920 286c 656e 6774  6.35 0 0) (lengt
+000007a0: 6820 322e 3534 290a 2020 2020 2020 2020  h 2.54).        
+000007b0: 286e 616d 6520 2231 2220 2865 6666 6563  (name "1" (effec
+000007c0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000007d0: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+000007e0: 2020 2020 2028 6e75 6d62 6572 2022 3122       (number "1"
+000007f0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000800: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000810: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
+00000820: 2020 2870 696e 2070 6173 7369 7665 206c    (pin passive l
+00000830: 696e 6520 2861 7420 362e 3335 2030 2031  ine (at 6.35 0 1
+00000840: 3830 2920 286c 656e 6774 6820 322e 3534  80) (length 2.54
+00000850: 290a 2020 2020 2020 2020 286e 616d 6520  ).        (name 
+00000860: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
+00000870: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000880: 3237 2929 2929 0a20 2020 2020 2020 2028  27)))).        (
+00000890: 6e75 6d62 6572 2022 3222 2028 6566 6665  number "2" (effe
+000008a0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+000008b0: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+000008c0: 2020 2020 290a 2020 2020 290a 2020 290a      ).    ).  ).
+000008d0: 290a                                     ).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/inductor.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/resistor-sm.kicad_sym`

 * *Files 11% similar despite different names*

```diff
@@ -1,150 +1,140 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 224c 2220 2869  eference" "L" (i
-000000c0: 6420 3029 2028 6174 2030 2032 2e35 3420  d 0) (at 0 2.54 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d38 2e38 3920   1) (at 0 -8.89 
-00000130: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000140: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000150: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000160: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000170: 7274 7920 2246 6f6f 7470 7269 6e74 2220  rty "Footprint" 
-00000180: 2246 6f6f 7470 7269 6e74 2220 2869 6420  "Footprint" (id 
-00000190: 3229 2028 6174 2030 202d 3136 2e35 3120  2) (at 0 -16.51 
-000001a0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000001b0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000001c0: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-000001d0: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-000001e0: 7274 7920 2244 6174 6173 6865 6574 2220  rty "Datasheet" 
-000001f0: 2269 6e76 656e 7472 6565 5f75 726c 2220  "inventree_url" 
-00000200: 2869 6420 3329 2028 6174 2030 202d 3139  (id 3) (at 0 -19
-00000210: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000220: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000230: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000240: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000250: 726f 7065 7274 7920 224d 616e 7566 6163  roperty "Manufac
-00000260: 7475 7265 7222 2022 4d61 6e75 6661 6374  turer" "Manufact
-00000270: 7572 6572 2220 2869 6420 3429 2028 6174  urer" (id 4) (at
-00000280: 2030 202d 3131 2e34 3320 3029 0a20 2020   0 -11.43 0).   
-00000290: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-000002a0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-000002b0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
-000002c0: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
-000002d0: 616e 7566 6163 7475 7265 7220 5061 7274  anufacturer Part
-000002e0: 204e 756d 6265 7222 2022 4d50 4e22 2028   Number" "MPN" (
-000002f0: 6964 2035 2920 2861 7420 3020 2d31 332e  id 5) (at 0 -13.
-00000300: 3937 2030 290a 2020 2020 2020 2865 6666  97 0).      (eff
-00000310: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000320: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
-00000330: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
-00000340: 6f70 6572 7479 2022 496e 6475 6374 616e  operty "Inductan
-00000350: 6365 2028 4865 6e72 7929 2220 2256 616c  ce (Henry)" "Val
-00000360: 7565 2220 2869 6420 3629 2028 6174 2030  ue" (id 6) (at 0
-00000370: 202d 312e 3237 2030 290a 2020 2020 2020   -1.27 0).      
-00000380: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000390: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-000003a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000003b0: 7065 7274 7920 2243 7572 7265 6e74 2052  perty "Current R
-000003c0: 6174 696e 6720 2841 6d70 6572 6529 2220  ating (Ampere)" 
-000003d0: 2252 6174 6564 2043 7572 7265 6e74 2220  "Rated Current" 
-000003e0: 2869 6420 3729 2028 6174 2030 202d 332e  (id 7) (at 0 -3.
-000003f0: 3831 2030 290a 2020 2020 2020 2865 6666  81 0).      (eff
-00000400: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000410: 2031 2e32 3720 312e 3237 2929 290a 2020   1.27 1.27))).  
-00000420: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000430: 7920 2245 5352 2028 4f68 6d29 2220 2245  y "ESR (Ohm)" "E
-00000440: 5352 2220 2869 6420 3829 2028 6174 2030  SR" (id 8) (at 0
-00000450: 202d 362e 3335 2030 290a 2020 2020 2020   -6.35 0).      
-00000460: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000470: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00000480: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000490: 2028 7072 6f70 6572 7479 2022 6b69 5f6b   (property "ki_k
-000004a0: 6579 776f 7264 7322 2022 6b65 7977 6f72  eywords" "keywor
-000004b0: 6473 2220 2869 6420 3929 2028 6174 2030  ds" (id 9) (at 0
-000004c0: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
-000004d0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-000004e0: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
-000004f0: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
-00000500: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
-00000510: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
-00000520: 7469 6f6e 2220 2869 6420 3130 2920 2861  tion" (id 10) (a
-00000530: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
-00000540: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000550: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000560: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000570: 2873 796d 626f 6c20 2249 504e 5f30 5f31  (symbol "IPN_0_1
-00000580: 220a 2020 2020 2020 2861 7263 2028 7374  ".      (arc (st
-00000590: 6172 7420 2d31 2e39 3035 2030 2920 286d  art -1.905 0) (m
-000005a0: 6964 202d 322e 3835 3735 2030 2e39 3339  id -2.8575 0.939
-000005b0: 3929 2028 656e 6420 2d33 2e38 3120 3029  9) (end -3.81 0)
-000005c0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
-000005d0: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
-000005e0: 2064 6566 6175 6c74 2920 2863 6f6c 6f72   default) (color
-000005f0: 2030 2030 2030 2030 2929 0a20 2020 2020   0 0 0 0)).     
-00000600: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
-00000610: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
-00000620: 2020 2020 2861 7263 2028 7374 6172 7420      (arc (start 
-00000630: 3020 3029 2028 6d69 6420 2d30 2e39 3532  0 0) (mid -0.952
-00000640: 3520 302e 3933 3939 2920 2865 6e64 202d  5 0.9399) (end -
-00000650: 312e 3930 3520 3029 0a20 2020 2020 2020  1.905 0).       
-00000660: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
-00000670: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
-00000680: 2920 2863 6f6c 6f72 2030 2030 2030 2030  ) (color 0 0 0 0
-00000690: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
-000006a0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
-000006b0: 2020 2020 290a 2020 2020 2020 2861 7263      ).      (arc
-000006c0: 2028 7374 6172 7420 312e 3930 3520 3029   (start 1.905 0)
-000006d0: 2028 6d69 6420 302e 3935 3235 2030 2e39   (mid 0.9525 0.9
-000006e0: 3339 3929 2028 656e 6420 3020 3029 0a20  399) (end 0 0). 
-000006f0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-00000700: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
-00000710: 6566 6175 6c74 2920 2863 6f6c 6f72 2030  efault) (color 0
-00000720: 2030 2030 2030 2929 0a20 2020 2020 2020   0 0 0)).       
-00000730: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
-00000740: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
-00000750: 2020 2861 7263 2028 7374 6172 7420 332e    (arc (start 3.
-00000760: 3831 2030 2920 286d 6964 2032 2e38 3537  81 0) (mid 2.857
-00000770: 3520 302e 3933 3939 2920 2865 6e64 2031  5 0.9399) (end 1
-00000780: 2e39 3035 2030 290a 2020 2020 2020 2020  .905 0).        
-00000790: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-000007a0: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
-000007b0: 2028 636f 6c6f 7220 3020 3020 3020 3029   (color 0 0 0 0)
-000007c0: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
-000007d0: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
-000007e0: 2020 2029 0a20 2020 2029 0a20 2020 2028     ).    ).    (
-000007f0: 7379 6d62 6f6c 2022 4950 4e5f 315f 3122  symbol "IPN_1_1"
-00000800: 0a20 2020 2020 2028 7069 6e20 7061 7373  .      (pin pass
-00000810: 6976 6520 6c69 6e65 2028 6174 202d 362e  ive line (at -6.
-00000820: 3335 2030 2030 2920 286c 656e 6774 6820  35 0 0) (length 
-00000830: 322e 3534 290a 2020 2020 2020 2020 286e  2.54).        (n
-00000840: 616d 6520 2231 2220 2865 6666 6563 7473  ame "1" (effects
-00000850: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000860: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000870: 2020 2028 6e75 6d62 6572 2022 3122 2028     (number "1" (
-00000880: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000890: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-000008a0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-000008b0: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
-000008c0: 6520 2861 7420 362e 3335 2030 2031 3830  e (at 6.35 0 180
-000008d0: 2920 286c 656e 6774 6820 322e 3534 290a  ) (length 2.54).
-000008e0: 2020 2020 2020 2020 286e 616d 6520 2232          (name "2
-000008f0: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
-00000900: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000910: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
-00000920: 6d62 6572 2022 3222 2028 6566 6665 6374  mber "2" (effect
-00000930: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000940: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-00000950: 2020 290a 2020 2020 290a 2020 290a 290a    ).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2252 2220 2861  eference" "R" (a
+000000c0: 7420 3020 322e 3033 3220 3029 0a20 2020  t 0 2.032 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
+00000320: 6573 6973 7461 6e63 6520 284f 686d 7329  esistance (Ohms)
+00000330: 2220 2256 616c 7565 2220 2861 7420 3020  " "Value" (at 0 
+00000340: 2d32 2e35 3420 3029 0a20 2020 2020 2028  -2.54 0).      (
+00000350: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000360: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+00000370: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000380: 6572 7479 2022 546f 6c65 7261 6e63 6520  erty "Tolerance 
+00000390: 2825 2922 2022 546f 6c65 7261 6e63 6522  (%)" "Tolerance"
+000003a0: 2028 6174 2033 2e38 3120 2d32 2e35 3420   (at 3.81 -2.54 
+000003b0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+000003c0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+000003d0: 3237 2031 2e32 3729 2920 286a 7573 7469  27 1.27)) (justi
+000003e0: 6679 206c 6566 7429 2068 6964 6529 0a20  fy left) hide). 
+000003f0: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000400: 7479 2022 5061 636b 6167 6520 5479 7065  ty "Package Type
+00000410: 2220 2250 6163 6b61 6765 2054 7970 6522  " "Package Type"
+00000420: 2028 6174 2030 202d 352e 3038 2030 290a   (at 0 -5.08 0).
+00000430: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000440: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000450: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
+00000460: 2020 2870 726f 7065 7274 7920 2250 6f77    (property "Pow
+00000470: 6572 2028 5761 7474 7329 2220 2252 6174  er (Watts)" "Rat
+00000480: 6564 2050 6f77 6572 2220 2861 7420 3020  ed Power" (at 0 
+00000490: 2d37 2e36 3220 3029 0a20 2020 2020 2028  -7.62 0).      (
+000004a0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000004b0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+000004c0: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000004d0: 2870 726f 7065 7274 7920 226b 695f 6b65  (property "ki_ke
+000004e0: 7977 6f72 6473 2220 226b 6579 776f 7264  ywords" "keyword
+000004f0: 7322 2028 6174 2030 2030 2030 290a 2020  s" (at 0 0 0).  
+00000500: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+00000510: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000520: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+00000530: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000540: 6b69 5f64 6573 6372 6970 7469 6f6e 2220  ki_description" 
+00000550: 2264 6573 6372 6970 7469 6f6e 2220 2861  "description" (a
+00000560: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
+00000570: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000580: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+00000590: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000005a0: 2873 796d 626f 6c20 2249 504e 5f30 5f31  (symbol "IPN_0_1
+000005b0: 220a 2020 2020 2020 2870 6f6c 796c 696e  ".      (polylin
+000005c0: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+000005d0: 2020 2020 2020 2020 2028 7879 202d 332e           (xy -3.
+000005e0: 3831 2030 290a 2020 2020 2020 2020 2020  81 0).          
+000005f0: 2878 7920 2d33 2e30 3438 2030 290a 2020  (xy -3.048 0).  
+00000600: 2020 2020 2020 2020 2878 7920 2d32 2e35          (xy -2.5
+00000610: 3420 302e 3736 3229 0a20 2020 2020 2020  4 0.762).       
+00000620: 2020 2028 7879 202d 312e 3532 3420 2d30     (xy -1.524 -0
+00000630: 2e37 3632 290a 2020 2020 2020 2020 2020  .762).          
+00000640: 2878 7920 2d30 2e35 3038 2030 2e37 3632  (xy -0.508 0.762
+00000650: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000660: 302e 3530 3820 2d30 2e37 3632 290a 2020  0.508 -0.762).  
+00000670: 2020 2020 2020 2020 2878 7920 312e 3532          (xy 1.52
+00000680: 3420 302e 3736 3229 0a20 2020 2020 2020  4 0.762).       
+00000690: 2020 2028 7879 2032 2e35 3420 2d30 2e37     (xy 2.54 -0.7
+000006a0: 3632 290a 2020 2020 2020 2020 2020 2878  62).          (x
+000006b0: 7920 332e 3034 3820 3029 0a20 2020 2020  y 3.048 0).     
+000006c0: 2020 2020 2028 7879 2033 2e38 3120 3029       (xy 3.81 0)
+000006d0: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
+000006e0: 2e38 3120 3029 0a20 2020 2020 2020 2029  .81 0).        )
+000006f0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000700: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000710: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000720: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000730: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000740: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+00000750: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
+00000760: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+00000770: 6520 2861 7420 2d35 2e30 3820 3020 3029  e (at -5.08 0 0)
+00000780: 2028 6c65 6e67 7468 2031 2e32 3729 0a20   (length 1.27). 
+00000790: 2020 2020 2020 2028 6e61 6d65 2022 3122         (name "1"
+000007a0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000007b0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000007c0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
+000007d0: 6265 7220 2231 2220 2865 6666 6563 7473  ber "1" (effects
+000007e0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+000007f0: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+00000800: 2029 0a20 2020 2020 2028 7069 6e20 7061   ).      (pin pa
+00000810: 7373 6976 6520 6c69 6e65 2028 6174 2035  ssive line (at 5
+00000820: 2e30 3820 3020 3138 3029 2028 6c65 6e67  .08 0 180) (leng
+00000830: 7468 2031 2e32 3729 0a20 2020 2020 2020  th 1.27).       
+00000840: 2028 6e61 6d65 2022 3222 2028 6566 6665   (name "2" (effe
+00000850: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000860: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000870: 2020 2020 2020 286e 756d 6265 7220 2232        (number "2
+00000880: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+00000890: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000008a0: 2929 2929 0a20 2020 2020 2029 0a20 2020  )))).      ).   
+000008b0: 2029 0a20 2029 0a29 0a                    ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/integrated-circuit.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/integrated-circuit.kicad_sym`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2255 2220 2869  eference" "U" (i
-000000c0: 6420 3029 2028 6174 2030 2030 2030 290a  d 0) (at 0 0 0).
-000000d0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-000000e0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-000000f0: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
-00000100: 2020 2870 726f 7065 7274 7920 2256 616c    (property "Val
-00000110: 7565 2220 2249 504e 2220 2869 6420 3129  ue" "IPN" (id 1)
-00000120: 2028 6174 2030 202d 352e 3038 2030 290a   (at 0 -5.08 0).
-00000130: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000140: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000150: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
-00000160: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-00000170: 2022 466f 6f74 7072 696e 7422 2022 466f   "Footprint" "Fo
-00000180: 6f74 7072 696e 7422 2028 6964 2032 2920  otprint" (id 2) 
-00000190: 2861 7420 3020 2d31 322e 3720 3029 0a20  (at 0 -12.7 0). 
-000001a0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000001b0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-000001c0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-000001d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000001e0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
-000001f0: 656e 7472 6565 5f75 726c 2220 2869 6420  entree_url" (id 
-00000200: 3329 2028 6174 2030 202d 3135 2e32 3420  3) (at 0 -15.24 
-00000210: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-00000220: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-00000230: 3237 2031 2e32 3729 2920 6869 6465 290a  27 1.27)) hide).
-00000240: 2020 2020 290a 2020 2020 2870 726f 7065      ).    (prope
-00000250: 7274 7920 224d 616e 7566 6163 7475 7265  rty "Manufacture
-00000260: 7222 2022 4d61 6e75 6661 6374 7572 6572  r" "Manufacturer
-00000270: 2220 2869 6420 3429 2028 6174 2030 202d  " (id 4) (at 0 -
-00000280: 372e 3632 2030 290a 2020 2020 2020 2865  7.62 0).      (e
-00000290: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-000002a0: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-000002b0: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-000002c0: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-000002d0: 6374 7572 6572 2050 6172 7420 4e75 6d62  cturer Part Numb
-000002e0: 6572 2220 224d 504e 2220 2869 6420 3529  er" "MPN" (id 5)
-000002f0: 2028 6174 2030 202d 3130 2e31 3620 3029   (at 0 -10.16 0)
-00000300: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-00000310: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000320: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000330: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000340: 7920 2250 6172 7420 4e75 6d62 6572 2220  y "Part Number" 
-00000350: 2256 616c 7565 2220 2869 6420 3629 2028  "Value" (id 6) (
-00000360: 6174 2030 202d 322e 3534 2030 290a 2020  at 0 -2.54 0).  
-00000370: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000380: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000390: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
-000003a0: 2870 726f 7065 7274 7920 226b 695f 6b65  (property "ki_ke
-000003b0: 7977 6f72 6473 2220 226b 6579 776f 7264  ywords" "keyword
-000003c0: 7322 2028 6964 2037 2920 2861 7420 3020  s" (id 7) (at 0 
-000003d0: 3020 3029 0a20 2020 2020 2028 6566 6665  0 0).      (effe
-000003e0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000003f0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000400: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000410: 7065 7274 7920 226b 695f 6465 7363 7269  perty "ki_descri
-00000420: 7074 696f 6e22 2022 6465 7363 7269 7074  ption" "descript
-00000430: 696f 6e22 2028 6964 2038 2920 2861 7420  ion" (id 8) (at 
-00000440: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000450: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000460: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000470: 6465 290a 2020 2020 290a 2020 290a 290a  de).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2255 2220 2861  eference" "U" (a
+000000c0: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
+000000d0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000000e0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+000000f0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000100: 6572 7479 2022 5661 6c75 6522 2022 4950  erty "Value" "IP
+00000110: 4e22 2028 6174 2030 202d 352e 3038 2030  N" (at 0 -5.08 0
+00000120: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000130: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000140: 3720 312e 3237 2929 2068 6964 6529 0a20  7 1.27)) hide). 
+00000150: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000160: 7479 2022 466f 6f74 7072 696e 7422 2022  ty "Footprint" "
+00000170: 466f 6f74 7072 696e 7422 2028 6174 2030  Footprint" (at 0
+00000180: 202d 3132 2e37 2030 290a 2020 2020 2020   -12.7 0).      
+00000190: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000001a0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000001b0: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
+000001c0: 2028 7072 6f70 6572 7479 2022 4461 7461   (property "Data
+000001d0: 7368 6565 7422 2022 696e 7665 6e74 7265  sheet" "inventre
+000001e0: 655f 7572 6c22 2028 6174 2030 202d 3135  e_url" (at 0 -15
+000001f0: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
+00000200: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000210: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000220: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000230: 726f 7065 7274 7920 224d 616e 7566 6163  roperty "Manufac
+00000240: 7475 7265 7222 2022 4d61 6e75 6661 6374  turer" "Manufact
+00000250: 7572 6572 2220 2861 7420 3020 2d37 2e36  urer" (at 0 -7.6
+00000260: 3220 3029 0a20 2020 2020 2028 6566 6665  2 0).      (effe
+00000270: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000280: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000290: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+000002a0: 7065 7274 7920 224d 616e 7566 6163 7475  perty "Manufactu
+000002b0: 7265 7220 5061 7274 204e 756d 6265 7222  rer Part Number"
+000002c0: 2022 4d50 4e22 2028 6174 2030 202d 3130   "MPN" (at 0 -10
+000002d0: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+000002e0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000002f0: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000300: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000310: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
+00000320: 6d62 6572 2220 2256 616c 7565 2220 2861  mber" "Value" (a
+00000330: 7420 3020 2d32 2e35 3420 3029 0a20 2020  t 0 -2.54 0).   
+00000340: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000350: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000360: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000370: 7072 6f70 6572 7479 2022 6b69 5f6b 6579  property "ki_key
+00000380: 776f 7264 7322 2022 6b65 7977 6f72 6473  words" "keywords
+00000390: 2220 2861 7420 3020 3020 3029 0a20 2020  " (at 0 0 0).   
+000003a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000003b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000003c0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+000003d0: 2020 2020 2870 726f 7065 7274 7920 226b      (property "k
+000003e0: 695f 6465 7363 7269 7074 696f 6e22 2022  i_description" "
+000003f0: 6465 7363 7269 7074 696f 6e22 2028 6174  description" (at
+00000400: 2030 2030 2030 290a 2020 2020 2020 2865   0 0 0).      (e
+00000410: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000420: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
+00000430: 6964 6529 0a20 2020 2029 0a20 2029 0a29  ide).    ).  ).)
+00000440: 0a                                       .
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/oscillator-4p.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/oscillator-4p.kicad_sym`

 * *Files 8% similar despite different names*

```diff
@@ -1,140 +1,134 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 696e 5f62 6f6d 2079 6573  IPN" (in_bom yes
 00000060: 2920 286f 6e5f 626f 6172 6420 7965 7329  ) (on_board yes)
 00000070: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
 00000080: 5265 6665 7265 6e63 6522 2022 5922 2028  Reference" "Y" (
-00000090: 6964 2030 2920 2861 7420 3020 362e 3335  id 0) (at 0 6.35
-000000a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000c0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000000d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000000e0: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-000000f0: 6420 3129 2028 6174 2030 202d 3136 2e35  d 1) (at 0 -16.5
-00000100: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
-00000110: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000120: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000130: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000140: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000150: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000160: 6420 3229 2028 6174 2030 202d 3231 2e35  d 2) (at 0 -21.5
-00000170: 3920 3029 0a20 2020 2020 2028 6566 6665  9 0).      (effe
-00000180: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000190: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001b0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001c0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-000001d0: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-000001e0: 3234 2e31 3320 3029 0a20 2020 2020 2028  24.13 0).      (
-000001f0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000200: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000210: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000220: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000230: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000240: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000250: 6174 2030 202d 3139 2e30 3520 3029 0a20  at 0 -19.05 0). 
-00000260: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000270: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000280: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-00000290: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000002a0: 224d 616e 7566 6163 7475 7265 7220 5061  "Manufacturer Pa
-000002b0: 7274 204e 756d 6265 7222 2022 4d50 4e22  rt Number" "MPN"
-000002c0: 2028 6964 2035 2920 2861 7420 3020 2d38   (id 5) (at 0 -8
-000002d0: 2e38 3920 3029 0a20 2020 2020 2028 6566  .89 0).      (ef
-000002e0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-000002f0: 6520 312e 3237 2031 2e32 3729 2929 0a20  e 1.27 1.27))). 
-00000300: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
-00000310: 7479 2022 5061 7274 204e 756d 6265 7222  ty "Part Number"
-00000320: 2022 5661 6c75 6522 2028 6964 2036 2920   "Value" (id 6) 
-00000330: 2861 7420 3020 2d36 2e33 3520 3029 0a20  (at 0 -6.35 0). 
-00000340: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000350: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000360: 2e32 3729 2929 0a20 2020 2029 0a20 2020  .27))).    ).   
-00000370: 2028 7072 6f70 6572 7479 2022 5261 7465   (property "Rate
-00000380: 6420 566f 6c74 6167 6520 2856 6f6c 7429  d Voltage (Volt)
-00000390: 2220 2252 6174 6564 2056 6f6c 7461 6765  " "Rated Voltage
-000003a0: 2220 2869 6420 3729 2028 6174 2030 202d  " (id 7) (at 0 -
-000003b0: 3131 2e34 3320 3029 0a20 2020 2020 2028  11.43 0).      (
-000003c0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-000003d0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-000003e0: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-000003f0: 2870 726f 7065 7274 7920 2250 6163 6b61  (property "Packa
-00000400: 6765 2053 697a 6522 2022 5061 636b 6167  ge Size" "Packag
-00000410: 6520 5369 7a65 2220 2869 6420 3829 2028  e Size" (id 8) (
-00000420: 6174 2030 202d 3133 2e39 3720 3029 0a20  at 0 -13.97 0). 
-00000430: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000440: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000450: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-00000460: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000470: 226b 695f 6b65 7977 6f72 6473 2220 226b  "ki_keywords" "k
-00000480: 6579 776f 7264 7322 2028 6964 2039 2920  eywords" (id 9) 
-00000490: 2861 7420 3020 3020 3029 0a20 2020 2020  (at 0 0 0).     
-000004a0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000004b0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000004c0: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
-000004d0: 2020 2870 726f 7065 7274 7920 226b 695f    (property "ki_
-000004e0: 6465 7363 7269 7074 696f 6e22 2022 6465  description" "de
-000004f0: 7363 7269 7074 696f 6e22 2028 6964 2031  scription" (id 1
-00000500: 3029 2028 6174 2030 2030 2030 290a 2020  0) (at 0 0 0).  
-00000510: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000520: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000530: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-00000540: 0a20 2020 2028 7379 6d62 6f6c 2022 4950  .    (symbol "IP
-00000550: 4e5f 315f 3122 0a20 2020 2020 2028 7265  N_1_1".      (re
-00000560: 6374 616e 676c 6520 2873 7461 7274 202d  ctangle (start -
-00000570: 352e 3038 2035 2e30 3829 2028 656e 6420  5.08 5.08) (end 
-00000580: 352e 3038 202d 352e 3038 290a 2020 2020  5.08 -5.08).    
-00000590: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-000005a0: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-000005b0: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-000005c0: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-000005d0: 696c 6c20 2874 7970 6520 6261 636b 6772  ill (type backgr
-000005e0: 6f75 6e64 2929 0a20 2020 2020 2029 0a20  ound)).      ). 
-000005f0: 2020 2020 2028 7069 6e20 696e 7075 7420       (pin input 
-00000600: 6c69 6e65 2028 6174 202d 3130 2e31 3620  line (at -10.16 
-00000610: 2d32 2e35 3420 3029 2028 6c65 6e67 7468  -2.54 0) (length
-00000620: 2035 2e30 3829 0a20 2020 2020 2020 2028   5.08).        (
-00000630: 6e61 6d65 2022 4f45 2220 2865 6666 6563  name "OE" (effec
-00000640: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000650: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-00000660: 2020 2020 2028 6e75 6d62 6572 2022 3122       (number "1"
-00000670: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000680: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000690: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
-000006a0: 2020 2870 696e 2070 6f77 6572 5f6f 7574    (pin power_out
-000006b0: 206c 696e 6520 2861 7420 3130 2e31 3620   line (at 10.16 
-000006c0: 2d32 2e35 3420 3138 3029 2028 6c65 6e67  -2.54 180) (leng
-000006d0: 7468 2035 2e30 3829 0a20 2020 2020 2020  th 5.08).       
-000006e0: 2028 6e61 6d65 2022 474e 4422 2028 6566   (name "GND" (ef
-000006f0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000700: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
-00000710: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
-00000720: 2232 2220 2865 6666 6563 7473 2028 666f  "2" (effects (fo
-00000730: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000740: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
-00000750: 2020 2020 2028 7069 6e20 6f75 7470 7574       (pin output
-00000760: 206c 696e 6520 2861 7420 3130 2e31 3620   line (at 10.16 
-00000770: 322e 3534 2031 3830 2920 286c 656e 6774  2.54 180) (lengt
-00000780: 6820 352e 3038 290a 2020 2020 2020 2020  h 5.08).        
-00000790: 286e 616d 6520 224f 5554 2220 2865 6666  (name "OUT" (eff
-000007a0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-000007b0: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-000007c0: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
-000007d0: 3322 2028 6566 6665 6374 7320 2866 6f6e  3" (effects (fon
-000007e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-000007f0: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
-00000800: 2020 2020 2870 696e 2070 6f77 6572 5f69      (pin power_i
-00000810: 6e20 6c69 6e65 2028 6174 202d 3130 2e31  n line (at -10.1
-00000820: 3620 322e 3534 2030 2920 286c 656e 6774  6 2.54 0) (lengt
-00000830: 6820 352e 3038 290a 2020 2020 2020 2020  h 5.08).        
-00000840: 286e 616d 6520 2256 4444 2220 2865 6666  (name "VDD" (eff
-00000850: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000860: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-00000870: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
-00000880: 3422 2028 6566 6665 6374 7320 2866 6f6e  4" (effects (fon
-00000890: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-000008a0: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
-000008b0: 2020 290a 2020 290a 290a                   ).  ).).
+00000090: 6174 2030 2036 2e33 3520 3029 0a20 2020  at 0 6.35 0).   
+000000a0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000b0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000c0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+000000d0: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+000000e0: 2022 4950 4e22 2028 6174 2030 202d 3136   "IPN" (at 0 -16
+000000f0: 2e35 3120 3029 0a20 2020 2020 2028 6566  .51 0).      (ef
+00000100: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000110: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000120: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000130: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000140: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000150: 2861 7420 3020 2d32 312e 3539 2030 290a  (at 0 -21.59 0).
+00000160: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000170: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000180: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000190: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001a0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001b0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001c0: 2030 202d 3234 2e31 3320 3029 0a20 2020   0 -24.13 0).   
+000001d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000001e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000001f0: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000200: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000210: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000220: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000230: 3020 2d31 392e 3035 2030 290a 2020 2020  0 -19.05 0).    
+00000240: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000250: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000260: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000270: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000280: 6e75 6661 6374 7572 6572 2050 6172 7420  nufacturer Part 
+00000290: 4e75 6d62 6572 2220 224d 504e 2220 2861  Number" "MPN" (a
+000002a0: 7420 3020 2d38 2e38 3920 3029 0a20 2020  t 0 -8.89 0).   
+000002b0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002c0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000002d0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+000002e0: 7072 6f70 6572 7479 2022 5061 7274 204e  property "Part N
+000002f0: 756d 6265 7222 2022 5661 6c75 6522 2028  umber" "Value" (
+00000300: 6174 2030 202d 362e 3335 2030 290a 2020  at 0 -6.35 0).  
+00000310: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+00000320: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000330: 3237 2929 290a 2020 2020 290a 2020 2020  27))).    ).    
+00000340: 2870 726f 7065 7274 7920 2252 6174 6564  (property "Rated
+00000350: 2056 6f6c 7461 6765 2028 566f 6c74 2922   Voltage (Volt)"
+00000360: 2022 5261 7465 6420 566f 6c74 6167 6522   "Rated Voltage"
+00000370: 2028 6174 2030 202d 3131 2e34 3320 3029   (at 0 -11.43 0)
+00000380: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+00000390: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000003a0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000003b0: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+000003c0: 7920 2250 6163 6b61 6765 2053 697a 6522  y "Package Size"
+000003d0: 2022 5061 636b 6167 6520 5369 7a65 2220   "Package Size" 
+000003e0: 2861 7420 3020 2d31 332e 3937 2030 290a  (at 0 -13.97 0).
+000003f0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000400: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000410: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+00000420: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+00000430: 2022 6b69 5f6b 6579 776f 7264 7322 2022   "ki_keywords" "
+00000440: 6b65 7977 6f72 6473 2220 2861 7420 3020  keywords" (at 0 
+00000450: 3020 3029 0a20 2020 2020 2028 6566 6665  0 0).      (effe
+00000460: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000470: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
+00000480: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
+00000490: 7065 7274 7920 226b 695f 6465 7363 7269  perty "ki_descri
+000004a0: 7074 696f 6e22 2022 6465 7363 7269 7074  ption" "descript
+000004b0: 696f 6e22 2028 6174 2030 2030 2030 290a  ion" (at 0 0 0).
+000004c0: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000004d0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000004e0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000004f0: 2029 0a20 2020 2028 7379 6d62 6f6c 2022   ).    (symbol "
+00000500: 4950 4e5f 315f 3122 0a20 2020 2020 2028  IPN_1_1".      (
+00000510: 7265 6374 616e 676c 6520 2873 7461 7274  rectangle (start
+00000520: 202d 352e 3038 2035 2e30 3829 2028 656e   -5.08 5.08) (en
+00000530: 6420 352e 3038 202d 352e 3038 290a 2020  d 5.08 -5.08).  
+00000540: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+00000550: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
+00000560: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+00000570: 2866 696c 6c20 2874 7970 6520 6261 636b  (fill (type back
+00000580: 6772 6f75 6e64 2929 0a20 2020 2020 2029  ground)).      )
+00000590: 0a20 2020 2020 2028 7069 6e20 696e 7075  .      (pin inpu
+000005a0: 7420 6c69 6e65 2028 6174 202d 3130 2e31  t line (at -10.1
+000005b0: 3620 2d32 2e35 3420 3029 2028 6c65 6e67  6 -2.54 0) (leng
+000005c0: 7468 2035 2e30 3829 0a20 2020 2020 2020  th 5.08).       
+000005d0: 2028 6e61 6d65 2022 4f45 2220 2865 6666   (name "OE" (eff
+000005e0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+000005f0: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
+00000600: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
+00000610: 3122 2028 6566 6665 6374 7320 2866 6f6e  1" (effects (fon
+00000620: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000630: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
+00000640: 2020 2020 2870 696e 2070 6f77 6572 5f6f      (pin power_o
+00000650: 7574 206c 696e 6520 2861 7420 3130 2e31  ut line (at 10.1
+00000660: 3620 2d32 2e35 3420 3138 3029 2028 6c65  6 -2.54 180) (le
+00000670: 6e67 7468 2035 2e30 3829 0a20 2020 2020  ngth 5.08).     
+00000680: 2020 2028 6e61 6d65 2022 474e 4422 2028     (name "GND" (
+00000690: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000006a0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+000006b0: 290a 2020 2020 2020 2020 286e 756d 6265  ).        (numbe
+000006c0: 7220 2232 2220 2865 6666 6563 7473 2028  r "2" (effects (
+000006d0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000006e0: 312e 3237 2929 2929 0a20 2020 2020 2029  1.27)))).      )
+000006f0: 0a20 2020 2020 2028 7069 6e20 6f75 7470  .      (pin outp
+00000700: 7574 206c 696e 6520 2861 7420 3130 2e31  ut line (at 10.1
+00000710: 3620 322e 3534 2031 3830 2920 286c 656e  6 2.54 180) (len
+00000720: 6774 6820 352e 3038 290a 2020 2020 2020  gth 5.08).      
+00000730: 2020 286e 616d 6520 224f 5554 2220 2865    (name "OUT" (e
+00000740: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000750: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000760: 0a20 2020 2020 2020 2028 6e75 6d62 6572  .        (number
+00000770: 2022 3322 2028 6566 6665 6374 7320 2866   "3" (effects (f
+00000780: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+00000790: 2e32 3729 2929 290a 2020 2020 2020 290a  .27)))).      ).
+000007a0: 2020 2020 2020 2870 696e 2070 6f77 6572        (pin power
+000007b0: 5f69 6e20 6c69 6e65 2028 6174 202d 3130  _in line (at -10
+000007c0: 2e31 3620 322e 3534 2030 2920 286c 656e  .16 2.54 0) (len
+000007d0: 6774 6820 352e 3038 290a 2020 2020 2020  gth 5.08).      
+000007e0: 2020 286e 616d 6520 2256 4444 2220 2865    (name "VDD" (e
+000007f0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000800: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000810: 0a20 2020 2020 2020 2028 6e75 6d62 6572  .        (number
+00000820: 2022 3422 2028 6566 6665 6374 7320 2866   "4" (effects (f
+00000830: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+00000840: 2e32 3729 2929 290a 2020 2020 2020 290a  .27)))).      ).
+00000850: 2020 2020 290a 2020 290a 290a                ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/protection-unidir.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/transistor-npn.kicad_sym`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,175 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2244 2220 2869  eference" "D" (i
-000000c0: 6420 3029 2028 6174 2030 2033 2e38 3120  d 0) (at 0 3.81 
-000000d0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
-000000e0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000000f0: 3237 2031 2e32 3729 2929 0a20 2020 2029  27 1.27))).    )
-00000100: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000110: 5661 6c75 6522 2022 4950 4e22 2028 6964  Value" "IPN" (id
-00000120: 2031 2920 2861 7420 3020 2d31 332e 3937   1) (at 0 -13.97
-00000130: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000140: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000150: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-00000160: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-00000170: 6572 7479 2022 466f 6f74 7072 696e 7422  erty "Footprint"
-00000180: 2022 466f 6f74 7072 696e 7422 2028 6964   "Footprint" (id
-00000190: 2032 2920 2861 7420 3020 2d32 312e 3539   2) (at 0 -21.59
-000001a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000001b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000001c0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000001d0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000001e0: 6572 7479 2022 4461 7461 7368 6565 7422  erty "Datasheet"
-000001f0: 2022 696e 7665 6e74 7265 655f 7572 6c22   "inventree_url"
-00000200: 2028 6964 2033 2920 2861 7420 3020 2d32   (id 3) (at 0 -2
-00000210: 342e 3133 2030 290a 2020 2020 2020 2865  4.13 0).      (e
-00000220: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000230: 7a65 2031 2e32 3720 312e 3237 2929 2068  ze 1.27 1.27)) h
-00000240: 6964 6529 0a20 2020 2029 0a20 2020 2028  ide).    ).    (
-00000250: 7072 6f70 6572 7479 2022 4d61 6e75 6661  property "Manufa
-00000260: 6374 7572 6572 2220 224d 616e 7566 6163  cturer" "Manufac
-00000270: 7475 7265 7222 2028 6964 2034 2920 2861  turer" (id 4) (a
-00000280: 7420 3020 2d31 362e 3531 2030 290a 2020  t 0 -16.51 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3139  (id 5) (at 0 -19
-00000300: 2e30 3520 3029 0a20 2020 2020 2028 6566  .05 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2030 202d 332e 3831  d 6) (at 0 -3.81
-00000370: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000380: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000390: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-000003a0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-000003b0: 2253 7461 6e64 6f66 6620 566f 6c74 6167  "Standoff Voltag
-000003c0: 6522 2022 5374 616e 646f 6666 2056 6f6c  e" "Standoff Vol
-000003d0: 7461 6765 2220 2869 6420 3729 2028 6174  tage" (id 7) (at
-000003e0: 2030 202d 362e 3335 2030 290a 2020 2020   0 -6.35 0).    
-000003f0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000400: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000410: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
-00000420: 726f 7065 7274 7920 2242 7265 616b 646f  roperty "Breakdo
-00000430: 776e 2056 6f6c 7461 6765 2220 2242 7265  wn Voltage" "Bre
-00000440: 616b 646f 776e 2056 6f6c 7461 6765 2220  akdown Voltage" 
-00000450: 2869 6420 3829 2028 6174 2030 202d 382e  (id 8) (at 0 -8.
-00000460: 3839 2030 290a 2020 2020 2020 2865 6666  89 0).      (eff
-00000470: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000480: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
-00000490: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
-000004a0: 6f70 6572 7479 2022 5065 616b 2050 6f77  operty "Peak Pow
-000004b0: 6572 2028 5761 7474 7329 2220 2252 6174  er (Watts)" "Rat
-000004c0: 6564 2050 6f77 6572 2220 2869 6420 3929  ed Power" (id 9)
-000004d0: 2028 6174 2030 202d 3131 2e34 3320 3029   (at 0 -11.43 0)
-000004e0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-000004f0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000500: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-00000510: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
-00000520: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
-00000530: 226b 6579 776f 7264 7322 2028 6964 2031  "keywords" (id 1
-00000540: 3029 2028 6174 2030 2030 2030 290a 2020  0) (at 0 0 0).  
-00000550: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-00000560: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-00000570: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-00000580: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-00000590: 6b69 5f64 6573 6372 6970 7469 6f6e 2220  ki_description" 
-000005a0: 2264 6573 6372 6970 7469 6f6e 2220 2869  "description" (i
-000005b0: 6420 3131 2920 2861 7420 3020 3020 3029  d 11) (at 0 0 0)
-000005c0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
-000005d0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-000005e0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
-000005f0: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
-00000600: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
-00000610: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
-00000620: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
-00000630: 2028 7879 2031 2e32 3720 2d31 2e33 3937   (xy 1.27 -1.397
-00000640: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
-00000650: 322e 3135 3920 2d31 2e37 3738 290a 2020  2.159 -1.778).  
-00000660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000670: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-00000680: 2e32 3534 2920 2874 7970 6520 6465 6661  .254) (type defa
-00000690: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-000006a0: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-000006b0: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-000006c0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-000006d0: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
-000006e0: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
-000006f0: 2878 7920 312e 3237 202d 312e 3339 3729  (xy 1.27 -1.397)
-00000700: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
-00000710: 2e32 3720 312e 3339 3729 0a20 2020 2020  .27 1.397).     
-00000720: 2020 2020 2028 7879 2030 2e33 3831 2031       (xy 0.381 1
-00000730: 2e37 3738 290a 2020 2020 2020 2020 290a  .778).        ).
-00000740: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
-00000750: 2877 6964 7468 2030 2e32 3534 2920 2874  (width 0.254) (t
-00000760: 7970 6520 6465 6661 756c 7429 2028 636f  ype default) (co
-00000770: 6c6f 7220 3020 3020 3020 3029 290a 2020  lor 0 0 0 0)).  
-00000780: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
-00000790: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
-000007a0: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-000007b0: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-000007c0: 2020 2020 2020 2020 2878 7920 2d31 2e32          (xy -1.2
-000007d0: 3720 312e 3237 290a 2020 2020 2020 2020  7 1.27).        
-000007e0: 2020 2878 7920 2d31 2e32 3720 2d31 2e32    (xy -1.27 -1.2
-000007f0: 3729 0a20 2020 2020 2020 2020 2028 7879  7).          (xy
-00000800: 2031 2e32 3720 3029 0a20 2020 2020 2020   1.27 0).       
-00000810: 2020 2028 7879 202d 312e 3237 2031 2e32     (xy -1.27 1.2
-00000820: 3729 0a20 2020 2020 2020 2029 0a20 2020  7).        ).   
-00000830: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
-00000840: 6474 6820 302e 3235 3429 2028 7479 7065  dth 0.254) (type
-00000850: 2064 6566 6175 6c74 2920 2863 6f6c 6f72   default) (color
-00000860: 2030 2030 2030 2030 2929 0a20 2020 2020   0 0 0 0)).     
-00000870: 2020 2028 6669 6c6c 2028 7479 7065 2062     (fill (type b
-00000880: 6163 6b67 726f 756e 6429 290a 2020 2020  ackground)).    
-00000890: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
-000008a0: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
-000008b0: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
-000008c0: 7665 206c 696e 6520 2861 7420 332e 3831  ve line (at 3.81
-000008d0: 2030 2031 3830 2920 286c 656e 6774 6820   0 180) (length 
-000008e0: 322e 3534 290a 2020 2020 2020 2020 286e  2.54).        (n
-000008f0: 616d 6520 2243 6174 686f 6465 2220 2865  ame "Cathode" (e
-00000900: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000910: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000920: 0a20 2020 2020 2020 2028 6e75 6d62 6572  .        (number
-00000930: 2022 3122 2028 6566 6665 6374 7320 2866   "1" (effects (f
-00000940: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000950: 2e32 3729 2929 290a 2020 2020 2020 290a  .27)))).      ).
-00000960: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
-00000970: 7665 206c 696e 6520 2861 7420 2d33 2e38  ve line (at -3.8
-00000980: 3120 3020 3029 2028 6c65 6e67 7468 2032  1 0 0) (length 2
-00000990: 2e35 3429 0a20 2020 2020 2020 2028 6e61  .54).        (na
-000009a0: 6d65 2022 416e 6f64 6522 2028 6566 6665  me "Anode" (effe
-000009b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000009c0: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
-000009d0: 2020 2020 2020 286e 756d 6265 7220 2232        (number "2
-000009e0: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
-000009f0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000a00: 2929 2929 0a20 2020 2020 2029 0a20 2020  )))).      ).   
-00000a10: 2029 0a20 2029 0a29 0a                    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2251 2220 2861  eference" "Q" (a
+000000c0: 7420 3020 342e 3331 3820 3029 0a20 2020  t 0 4.318 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 352e 3038 2033 2e38  ue" (at 5.08 3.8
+00000340: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+00000350: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000360: 312e 3237 2031 2e32 3729 2920 286a 7573  1.27 1.27)) (jus
+00000370: 7469 6679 206c 6566 7429 290a 2020 2020  tify left)).    
+00000380: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+00000390: 2252 6174 6564 2056 6f6c 7461 6765 2028  "Rated Voltage (
+000003a0: 566f 6c74 2922 2022 5261 7465 6420 566f  Volt)" "Rated Vo
+000003b0: 6c74 6167 6522 2028 6174 2035 2e30 3820  ltage" (at 5.08 
+000003c0: 312e 3237 2030 290a 2020 2020 2020 2865  1.27 0).      (e
+000003d0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+000003e0: 7a65 2031 2e32 3720 312e 3237 2929 2028  ze 1.27 1.27)) (
+000003f0: 6a75 7374 6966 7920 6c65 6674 2929 0a20  justify left)). 
+00000400: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000410: 7479 2022 5261 7465 6420 4375 7272 656e  ty "Rated Curren
+00000420: 7420 2841 6d70 7329 2220 2252 6174 6564  t (Amps)" "Rated
+00000430: 2043 7572 7265 6e74 2220 2861 7420 352e   Current" (at 5.
+00000440: 3038 202d 312e 3237 2030 290a 2020 2020  08 -1.27 0).    
+00000450: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000460: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000470: 2929 2028 6a75 7374 6966 7920 6c65 6674  )) (justify left
+00000480: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000490: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
+000004a0: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
+000004b0: 7970 6522 2028 6174 2035 2e30 3820 2d33  ype" (at 5.08 -3
+000004c0: 2e38 3120 3029 0a20 2020 2020 2028 6566  .81 0).      (ef
+000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000004e0: 6520 312e 3237 2031 2e32 3729 2920 286a  e 1.27 1.27)) (j
+000004f0: 7573 7469 6679 206c 6566 7429 290a 2020  ustify left)).  
+00000500: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+00000510: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
+00000520: 226b 6579 776f 7264 7322 2028 6174 2030  "keywords" (at 0
+00000530: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
+00000540: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000550: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000560: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000570: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
+00000580: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
+00000590: 7469 6f6e 2220 2861 7420 3020 3020 3029  tion" (at 0 0 0)
+000005a0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+000005b0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000005c0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000005d0: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+000005e0: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
+000005f0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000600: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000610: 2028 7879 2031 2e32 3720 322e 3238 3629   (xy 1.27 2.286)
+00000620: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
+00000630: 2e32 3720 2d32 2e32 3836 290a 2020 2020  .27 -2.286).    
+00000640: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+00000650: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+00000660: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+00000670: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+00000680: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+00000690: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000006a0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+000006b0: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
+000006c0: 3831 202d 322e 3534 290a 2020 2020 2020  81 -2.54).      
+000006d0: 2020 2020 2878 7920 312e 3237 202d 312e      (xy 1.27 -1.
+000006e0: 3031 3629 0a20 2020 2020 2020 2029 0a20  016).        ). 
+000006f0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+00000700: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
+00000710: 6566 6175 6c74 2929 0a20 2020 2020 2020  efault)).       
+00000720: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
+00000730: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+00000740: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
+00000750: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
+00000760: 2020 2028 7879 2033 2e38 3120 322e 3534     (xy 3.81 2.54
+00000770: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000780: 312e 3237 2031 2e30 3136 290a 2020 2020  1.27 1.016).    
+00000790: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+000007a0: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+000007b0: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+000007c0: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+000007d0: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+000007e0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000007f0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+00000800: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
+00000810: 3831 202d 322e 3534 290a 2020 2020 2020  81 -2.54).      
+00000820: 2020 2020 2878 7920 332e 3137 3520 2d31      (xy 3.175 -1
+00000830: 2e32 3729 0a20 2020 2020 2020 2020 2028  .27).          (
+00000840: 7879 2032 2e34 3133 202d 322e 3431 3329  xy 2.413 -2.413)
+00000850: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
+00000860: 2e38 3120 2d32 2e35 3429 0a20 2020 2020  .81 -2.54).     
+00000870: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
+00000880: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
+00000890: 7479 7065 2064 6566 6175 6c74 2929 0a20  type default)). 
+000008a0: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
+000008b0: 7065 206f 7574 6c69 6e65 2929 0a20 2020  pe outline)).   
+000008c0: 2020 2029 0a20 2020 2029 0a20 2020 2028     ).    ).    (
+000008d0: 7379 6d62 6f6c 2022 4950 4e5f 315f 3122  symbol "IPN_1_1"
+000008e0: 0a20 2020 2020 2028 7069 6e20 696e 7075  .      (pin inpu
+000008f0: 7420 6c69 6e65 2028 6174 202d 332e 3831  t line (at -3.81
+00000900: 2030 2030 2920 286c 656e 6774 6820 352e   0 0) (length 5.
+00000910: 3038 290a 2020 2020 2020 2020 286e 616d  08).        (nam
+00000920: 6520 2242 2220 2865 6666 6563 7473 2028  e "B" (effects (
+00000930: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000940: 312e 3237 2929 2929 0a20 2020 2020 2020  1.27)))).       
+00000950: 2028 6e75 6d62 6572 2022 7e22 2028 6566   (number "~" (ef
+00000960: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000970: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
+00000980: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
+00000990: 696e 2069 6e70 7574 206c 696e 6520 2861  in input line (a
+000009a0: 7420 332e 3831 2037 2e36 3220 3237 3029  t 3.81 7.62 270)
+000009b0: 2028 6c65 6e67 7468 2035 2e30 3829 0a20   (length 5.08). 
+000009c0: 2020 2020 2020 2028 6e61 6d65 2022 4322         (name "C"
+000009d0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000009e0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000009f0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
+00000a00: 6265 7220 227e 2220 2865 6666 6563 7473  ber "~" (effects
+00000a10: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000a20: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+00000a30: 2029 0a20 2020 2020 2028 7069 6e20 6f75   ).      (pin ou
+00000a40: 7470 7574 206c 696e 6520 2861 7420 332e  tput line (at 3.
+00000a50: 3831 202d 372e 3632 2039 3029 2028 6c65  81 -7.62 90) (le
+00000a60: 6e67 7468 2035 2e30 3829 0a20 2020 2020  ngth 5.08).     
+00000a70: 2020 2028 6e61 6d65 2022 4522 2028 6566     (name "E" (ef
+00000a80: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000a90: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
+00000aa0: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
+00000ab0: 227e 2220 2865 6666 6563 7473 2028 666f  "~" (effects (fo
+00000ac0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000ad0: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
+00000ae0: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/resistor-sm.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/resistor.kicad_sym`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,140 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2252 2220 2869  eference" "R" (i
-000000c0: 6420 3029 2028 6174 2030 2032 2e30 3332  d 0) (at 0 2.032
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2252 6573 6973 7461  roperty "Resista
-00000350: 6e63 6520 284f 686d 7329 2220 2256 616c  nce (Ohms)" "Val
-00000360: 7565 2220 2869 6420 3629 2028 6174 2030  ue" (id 6) (at 0
-00000370: 202d 322e 3534 2030 290a 2020 2020 2020   -2.54 0).      
-00000380: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000390: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-000003a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000003b0: 7065 7274 7920 2254 6f6c 6572 616e 6365  perty "Tolerance
-000003c0: 2028 2529 2220 2254 6f6c 6572 616e 6365   (%)" "Tolerance
-000003d0: 2220 2869 6420 3729 2028 6174 2033 2e38  " (id 7) (at 3.8
-000003e0: 3120 2d32 2e35 3420 3029 0a20 2020 2020  1 -2.54 0).     
-000003f0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000400: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000410: 2920 286a 7573 7469 6679 206c 6566 7429  ) (justify left)
-00000420: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000430: 2028 7072 6f70 6572 7479 2022 5061 636b   (property "Pack
-00000440: 6167 6520 5479 7065 2220 2250 6163 6b61  age Type" "Packa
-00000450: 6765 2054 7970 6522 2028 6964 2038 2920  ge Type" (id 8) 
-00000460: 2861 7420 3020 2d35 2e30 3820 3029 0a20  (at 0 -5.08 0). 
-00000470: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000480: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000490: 2e32 3729 2929 0a20 2020 2029 0a20 2020  .27))).    ).   
-000004a0: 2028 7072 6f70 6572 7479 2022 506f 7765   (property "Powe
-000004b0: 7220 2857 6174 7473 2922 2022 5261 7465  r (Watts)" "Rate
-000004c0: 6420 506f 7765 7222 2028 6964 2039 2920  d Power" (id 9) 
-000004d0: 2861 7420 3020 2d37 2e36 3220 3029 0a20  (at 0 -7.62 0). 
-000004e0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000004f0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000500: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-00000510: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000520: 226b 695f 6b65 7977 6f72 6473 2220 226b  "ki_keywords" "k
-00000530: 6579 776f 7264 7322 2028 6964 2031 3029  eywords" (id 10)
-00000540: 2028 6174 2030 2030 2030 290a 2020 2020   (at 0 0 0).    
-00000550: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000560: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000570: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
-00000580: 2020 2028 7072 6f70 6572 7479 2022 6b69     (property "ki
-00000590: 5f64 6573 6372 6970 7469 6f6e 2220 2264  _description" "d
-000005a0: 6573 6372 6970 7469 6f6e 2220 2869 6420  escription" (id 
-000005b0: 3131 2920 2861 7420 3020 3020 3029 0a20  11) (at 0 0 0). 
-000005c0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000005d0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-000005e0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-000005f0: 290a 2020 2020 2873 796d 626f 6c20 2249  ).    (symbol "I
-00000600: 504e 5f30 5f31 220a 2020 2020 2020 2870  PN_0_1".      (p
-00000610: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-00000620: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-00000630: 7879 202d 332e 3831 2030 290a 2020 2020  xy -3.81 0).    
-00000640: 2020 2020 2020 2878 7920 2d33 2e30 3438        (xy -3.048
-00000650: 2030 290a 2020 2020 2020 2020 2020 2878   0).          (x
-00000660: 7920 2d32 2e35 3420 302e 3736 3229 0a20  y -2.54 0.762). 
-00000670: 2020 2020 2020 2020 2028 7879 202d 312e           (xy -1.
-00000680: 3532 3420 2d30 2e37 3632 290a 2020 2020  524 -0.762).    
-00000690: 2020 2020 2020 2878 7920 2d30 2e35 3038        (xy -0.508
-000006a0: 2030 2e37 3632 290a 2020 2020 2020 2020   0.762).        
-000006b0: 2020 2878 7920 302e 3530 3820 2d30 2e37    (xy 0.508 -0.7
-000006c0: 3632 290a 2020 2020 2020 2020 2020 2878  62).          (x
-000006d0: 7920 312e 3532 3420 302e 3736 3229 0a20  y 1.524 0.762). 
-000006e0: 2020 2020 2020 2020 2028 7879 2032 2e35           (xy 2.5
-000006f0: 3420 2d30 2e37 3632 290a 2020 2020 2020  4 -0.762).      
-00000700: 2020 2020 2878 7920 332e 3034 3820 3029      (xy 3.048 0)
-00000710: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
-00000720: 2e38 3120 3029 0a20 2020 2020 2020 2020  .81 0).         
-00000730: 2028 7879 2033 2e38 3120 3029 0a20 2020   (xy 3.81 0).   
-00000740: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00000750: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00000760: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00000770: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000780: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000790: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000007a0: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
-000007b0: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
-000007c0: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
-000007d0: 7665 206c 696e 6520 2861 7420 2d35 2e30  ve line (at -5.0
-000007e0: 3820 3020 3029 2028 6c65 6e67 7468 2031  8 0 0) (length 1
-000007f0: 2e32 3729 0a20 2020 2020 2020 2028 6e61  .27).        (na
-00000800: 6d65 2022 3122 2028 6566 6665 6374 7320  me "1" (effects 
-00000810: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000820: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000830: 2020 286e 756d 6265 7220 2231 2220 2865    (number "1" (e
-00000840: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000850: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000860: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000870: 7069 6e20 7061 7373 6976 6520 6c69 6e65  pin passive line
-00000880: 2028 6174 2035 2e30 3820 3020 3138 3029   (at 5.08 0 180)
-00000890: 2028 6c65 6e67 7468 2031 2e32 3729 0a20   (length 1.27). 
-000008a0: 2020 2020 2020 2028 6e61 6d65 2022 3222         (name "2"
-000008b0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000008c0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000008d0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
-000008e0: 6265 7220 2232 2220 2865 6666 6563 7473  ber "2" (effects
-000008f0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000900: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000910: 2029 0a20 2020 2029 0a20 2029 0a29 0a     ).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2252 2220 2861  eference" "R" (a
+000000c0: 7420 3020 322e 3033 3220 3029 0a20 2020  t 0 2.032 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
+00000320: 6573 6973 7461 6e63 6520 284f 686d 7329  esistance (Ohms)
+00000330: 2220 2256 616c 7565 2220 2861 7420 3020  " "Value" (at 0 
+00000340: 2d32 2e35 3420 3029 0a20 2020 2020 2028  -2.54 0).      (
+00000350: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000360: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
+00000370: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000380: 6572 7479 2022 546f 6c65 7261 6e63 6520  erty "Tolerance 
+00000390: 2825 2922 2022 546f 6c65 7261 6e63 6522  (%)" "Tolerance"
+000003a0: 2028 6174 2033 2e38 3120 2d32 2e35 3420   (at 3.81 -2.54 
+000003b0: 3029 0a20 2020 2020 2028 6566 6665 6374  0).      (effect
+000003c0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+000003d0: 3237 2031 2e32 3729 2920 286a 7573 7469  27 1.27)) (justi
+000003e0: 6679 206c 6566 7429 2068 6964 6529 0a20  fy left) hide). 
+000003f0: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000400: 7479 2022 5061 636b 6167 6520 5479 7065  ty "Package Type
+00000410: 2220 2250 6163 6b61 6765 2054 7970 6522  " "Package Type"
+00000420: 2028 6174 2030 202d 352e 3038 2030 290a   (at 0 -5.08 0).
+00000430: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+00000440: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+00000450: 312e 3237 2929 290a 2020 2020 290a 2020  1.27))).    ).  
+00000460: 2020 2870 726f 7065 7274 7920 2250 6f77    (property "Pow
+00000470: 6572 2028 5761 7474 7329 2220 2252 6174  er (Watts)" "Rat
+00000480: 6564 2050 6f77 6572 2220 2861 7420 3020  ed Power" (at 0 
+00000490: 2d37 2e36 3220 3029 0a20 2020 2020 2028  -7.62 0).      (
+000004a0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+000004b0: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+000004c0: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000004d0: 2870 726f 7065 7274 7920 226b 695f 6b65  (property "ki_ke
+000004e0: 7977 6f72 6473 2220 226b 6579 776f 7264  ywords" "keyword
+000004f0: 7322 2028 6174 2030 2030 2030 290a 2020  s" (at 0 0 0).  
+00000500: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
+00000510: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00000520: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
+00000530: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
+00000540: 6b69 5f64 6573 6372 6970 7469 6f6e 2220  ki_description" 
+00000550: 2264 6573 6372 6970 7469 6f6e 2220 2861  "description" (a
+00000560: 7420 3020 3020 3029 0a20 2020 2020 2028  t 0 0 0).      (
+00000570: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
+00000580: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
+00000590: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
+000005a0: 2873 796d 626f 6c20 2249 504e 5f30 5f31  (symbol "IPN_0_1
+000005b0: 220a 2020 2020 2020 2870 6f6c 796c 696e  ".      (polylin
+000005c0: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+000005d0: 2020 2020 2020 2020 2028 7879 202d 332e           (xy -3.
+000005e0: 3831 2030 290a 2020 2020 2020 2020 2020  81 0).          
+000005f0: 2878 7920 2d33 2e30 3438 2030 290a 2020  (xy -3.048 0).  
+00000600: 2020 2020 2020 2020 2878 7920 2d32 2e35          (xy -2.5
+00000610: 3420 302e 3736 3229 0a20 2020 2020 2020  4 0.762).       
+00000620: 2020 2028 7879 202d 312e 3532 3420 2d30     (xy -1.524 -0
+00000630: 2e37 3632 290a 2020 2020 2020 2020 2020  .762).          
+00000640: 2878 7920 2d30 2e35 3038 2030 2e37 3632  (xy -0.508 0.762
+00000650: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000660: 302e 3530 3820 2d30 2e37 3632 290a 2020  0.508 -0.762).  
+00000670: 2020 2020 2020 2020 2878 7920 312e 3532          (xy 1.52
+00000680: 3420 302e 3736 3229 0a20 2020 2020 2020  4 0.762).       
+00000690: 2020 2028 7879 2032 2e35 3420 2d30 2e37     (xy 2.54 -0.7
+000006a0: 3632 290a 2020 2020 2020 2020 2020 2878  62).          (x
+000006b0: 7920 332e 3034 3820 3029 0a20 2020 2020  y 3.048 0).     
+000006c0: 2020 2020 2028 7879 2033 2e38 3120 3029       (xy 3.81 0)
+000006d0: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
+000006e0: 2e38 3120 3029 0a20 2020 2020 2020 2029  .81 0).        )
+000006f0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000700: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000710: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000720: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000730: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000740: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+00000750: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
+00000760: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+00000770: 6520 2861 7420 2d35 2e30 3820 3020 3029  e (at -5.08 0 0)
+00000780: 2028 6c65 6e67 7468 2031 2e32 3729 0a20   (length 1.27). 
+00000790: 2020 2020 2020 2028 6e61 6d65 2022 3122         (name "1"
+000007a0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+000007b0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+000007c0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
+000007d0: 6265 7220 2231 2220 2865 6666 6563 7473  ber "1" (effects
+000007e0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+000007f0: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
+00000800: 2029 0a20 2020 2020 2028 7069 6e20 7061   ).      (pin pa
+00000810: 7373 6976 6520 6c69 6e65 2028 6174 2035  ssive line (at 5
+00000820: 2e30 3820 3020 3138 3029 2028 6c65 6e67  .08 0 180) (leng
+00000830: 7468 2031 2e32 3729 0a20 2020 2020 2020  th 1.27).       
+00000840: 2028 6e61 6d65 2022 3222 2028 6566 6665   (name "2" (effe
+00000850: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000860: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000870: 2020 2020 2020 286e 756d 6265 7220 2232        (number "2
+00000880: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+00000890: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000008a0: 2929 2929 0a20 2020 2020 2029 0a20 2020  )))).      ).   
+000008b0: 2029 0a20 2029 0a29 0a                    ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/resistor.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/transistor-pnp.kicad_sym`

 * *Files 21% similar despite different names*

```diff
@@ -1,146 +1,175 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2252 2220 2869  eference" "R" (i
-000000c0: 6420 3029 2028 6174 2030 2032 2e30 3332  d 0) (at 0 2.032
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2252 6573 6973 7461  roperty "Resista
-00000350: 6e63 6520 284f 686d 7329 2220 2256 616c  nce (Ohms)" "Val
-00000360: 7565 2220 2869 6420 3629 2028 6174 2030  ue" (id 6) (at 0
-00000370: 202d 322e 3534 2030 290a 2020 2020 2020   -2.54 0).      
-00000380: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00000390: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-000003a0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000003b0: 7065 7274 7920 2254 6f6c 6572 616e 6365  perty "Tolerance
-000003c0: 2028 2529 2220 2254 6f6c 6572 616e 6365   (%)" "Tolerance
-000003d0: 2220 2869 6420 3729 2028 6174 2033 2e38  " (id 7) (at 3.8
-000003e0: 3120 2d32 2e35 3420 3029 0a20 2020 2020  1 -2.54 0).     
-000003f0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-00000400: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-00000410: 2920 286a 7573 7469 6679 206c 6566 7429  ) (justify left)
-00000420: 2068 6964 6529 0a20 2020 2029 0a20 2020   hide).    ).   
-00000430: 2028 7072 6f70 6572 7479 2022 5061 636b   (property "Pack
-00000440: 6167 6520 5479 7065 2220 2250 6163 6b61  age Type" "Packa
-00000450: 6765 2054 7970 6522 2028 6964 2038 2920  ge Type" (id 8) 
-00000460: 2861 7420 3020 2d35 2e30 3820 3029 0a20  (at 0 -5.08 0). 
-00000470: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-00000480: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000490: 2e32 3729 2929 0a20 2020 2029 0a20 2020  .27))).    ).   
-000004a0: 2028 7072 6f70 6572 7479 2022 506f 7765   (property "Powe
-000004b0: 7220 2857 6174 7473 2922 2022 5261 7465  r (Watts)" "Rate
-000004c0: 6420 506f 7765 7222 2028 6964 2039 2920  d Power" (id 9) 
-000004d0: 2861 7420 3020 2d37 2e36 3220 3029 0a20  (at 0 -7.62 0). 
-000004e0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000004f0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-00000500: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-00000510: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000520: 226b 695f 6b65 7977 6f72 6473 2220 226b  "ki_keywords" "k
-00000530: 6579 776f 7264 7322 2028 6964 2031 3029  eywords" (id 10)
-00000540: 2028 6174 2030 2030 2030 290a 2020 2020   (at 0 0 0).    
-00000550: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
-00000560: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00000570: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
-00000580: 2020 2028 7072 6f70 6572 7479 2022 6b69     (property "ki
-00000590: 5f64 6573 6372 6970 7469 6f6e 2220 2264  _description" "d
-000005a0: 6573 6372 6970 7469 6f6e 2220 2869 6420  escription" (id 
-000005b0: 3131 2920 2861 7420 3020 3020 3029 0a20  11) (at 0 0 0). 
-000005c0: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
-000005d0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
-000005e0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
-000005f0: 290a 2020 2020 2873 796d 626f 6c20 2249  ).    (symbol "I
-00000600: 504e 5f30 5f31 220a 2020 2020 2020 2870  PN_0_1".      (p
-00000610: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-00000620: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-00000630: 7879 202d 332e 3831 2030 290a 2020 2020  xy -3.81 0).    
-00000640: 2020 2020 2020 2878 7920 2d33 2e30 3438        (xy -3.048
-00000650: 2030 290a 2020 2020 2020 2020 2020 2878   0).          (x
-00000660: 7920 2d32 2e35 3420 302e 3736 3229 0a20  y -2.54 0.762). 
-00000670: 2020 2020 2020 2020 2028 7879 202d 312e           (xy -1.
-00000680: 3532 3420 2d30 2e37 3632 290a 2020 2020  524 -0.762).    
-00000690: 2020 2020 2020 2878 7920 2d30 2e35 3038        (xy -0.508
-000006a0: 2030 2e37 3632 290a 2020 2020 2020 2020   0.762).        
-000006b0: 2020 2878 7920 302e 3530 3820 2d30 2e37    (xy 0.508 -0.7
-000006c0: 3632 290a 2020 2020 2020 2020 2020 2878  62).          (x
-000006d0: 7920 312e 3532 3420 302e 3736 3229 0a20  y 1.524 0.762). 
-000006e0: 2020 2020 2020 2020 2028 7879 2032 2e35           (xy 2.5
-000006f0: 3420 2d30 2e37 3632 290a 2020 2020 2020  4 -0.762).      
-00000700: 2020 2020 2878 7920 332e 3034 3820 3029      (xy 3.048 0)
-00000710: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
-00000720: 2e38 3120 3029 0a20 2020 2020 2020 2020  .81 0).         
-00000730: 2028 7879 2033 2e38 3120 3029 0a20 2020   (xy 3.81 0).   
-00000740: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00000750: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00000760: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00000770: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00000780: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00000790: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000007a0: 2020 290a 2020 2020 290a 2020 2020 2873    ).    ).    (s
-000007b0: 796d 626f 6c20 2249 504e 5f31 5f31 220a  ymbol "IPN_1_1".
-000007c0: 2020 2020 2020 2870 696e 2070 6173 7369        (pin passi
-000007d0: 7665 206c 696e 6520 2861 7420 2d35 2e30  ve line (at -5.0
-000007e0: 3820 3020 3029 2028 6c65 6e67 7468 2031  8 0 0) (length 1
-000007f0: 2e32 3729 0a20 2020 2020 2020 2028 6e61  .27).        (na
-00000800: 6d65 2022 3122 2028 6566 6665 6374 7320  me "1" (effects 
-00000810: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000820: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000830: 2020 286e 756d 6265 7220 2231 2220 2865    (number "1" (e
-00000840: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000850: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000860: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000870: 7069 6e20 7061 7373 6976 6520 6c69 6e65  pin passive line
-00000880: 2028 6174 2035 2e30 3820 3020 3138 3029   (at 5.08 0 180)
-00000890: 2028 6c65 6e67 7468 2031 2e32 3729 0a20   (length 1.27). 
-000008a0: 2020 2020 2020 2028 6e61 6d65 2022 3222         (name "2"
-000008b0: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000008c0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000008d0: 2929 290a 2020 2020 2020 2020 286e 756d  ))).        (num
-000008e0: 6265 7220 2232 2220 2865 6666 6563 7473  ber "2" (effects
-000008f0: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00000900: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00000910: 2029 0a20 2020 2029 0a20 2029 0a29 0a     ).    ).  ).).
+000000b0: 6566 6572 656e 6365 2220 2251 2220 2861  eference" "Q" (a
+000000c0: 7420 3020 342e 3331 3820 3029 0a20 2020  t 0 4.318 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 352e 3038 2033 2e38  ue" (at 5.08 3.8
+00000340: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+00000350: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000360: 312e 3237 2031 2e32 3729 2920 286a 7573  1.27 1.27)) (jus
+00000370: 7469 6679 206c 6566 7429 290a 2020 2020  tify left)).    
+00000380: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+00000390: 2252 6174 6564 2056 6f6c 7461 6765 2028  "Rated Voltage (
+000003a0: 566f 6c74 2922 2022 5261 7465 6420 566f  Volt)" "Rated Vo
+000003b0: 6c74 6167 6522 2028 6174 2035 2e30 3820  ltage" (at 5.08 
+000003c0: 312e 3237 2030 290a 2020 2020 2020 2865  1.27 0).      (e
+000003d0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+000003e0: 7a65 2031 2e32 3720 312e 3237 2929 2028  ze 1.27 1.27)) (
+000003f0: 6a75 7374 6966 7920 6c65 6674 2929 0a20  justify left)). 
+00000400: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000410: 7479 2022 5261 7465 6420 4375 7272 656e  ty "Rated Curren
+00000420: 7420 2841 6d70 7329 2220 2252 6174 6564  t (Amps)" "Rated
+00000430: 2043 7572 7265 6e74 2220 2861 7420 352e   Current" (at 5.
+00000440: 3038 202d 312e 3237 2030 290a 2020 2020  08 -1.27 0).    
+00000450: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000460: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000470: 2929 2028 6a75 7374 6966 7920 6c65 6674  )) (justify left
+00000480: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000490: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
+000004a0: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
+000004b0: 7970 6522 2028 6174 2035 2e30 3820 2d33  ype" (at 5.08 -3
+000004c0: 2e38 3120 3029 0a20 2020 2020 2028 6566  .81 0).      (ef
+000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000004e0: 6520 312e 3237 2031 2e32 3729 2920 286a  e 1.27 1.27)) (j
+000004f0: 7573 7469 6679 206c 6566 7429 290a 2020  ustify left)).  
+00000500: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+00000510: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
+00000520: 226b 6579 776f 7264 7322 2028 6174 2030  "keywords" (at 0
+00000530: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
+00000540: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000550: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000560: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000570: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
+00000580: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
+00000590: 7469 6f6e 2220 2861 7420 3020 3020 3029  tion" (at 0 0 0)
+000005a0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+000005b0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000005c0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000005d0: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+000005e0: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
+000005f0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000600: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000610: 2028 7879 2031 2e32 3720 2d32 2e32 3836   (xy 1.27 -2.286
+00000620: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000630: 312e 3237 2032 2e32 3836 290a 2020 2020  1.27 2.286).    
+00000640: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+00000650: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+00000660: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+00000670: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+00000680: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+00000690: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000006a0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+000006b0: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
+000006c0: 3831 202d 322e 3534 290a 2020 2020 2020  81 -2.54).      
+000006d0: 2020 2020 2878 7920 312e 3237 202d 312e      (xy 1.27 -1.
+000006e0: 3031 3629 0a20 2020 2020 2020 2029 0a20  016).        ). 
+000006f0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+00000700: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
+00000710: 6566 6175 6c74 2929 0a20 2020 2020 2020  efault)).       
+00000720: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
+00000730: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+00000740: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
+00000750: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
+00000760: 2020 2028 7879 2033 2e38 3120 322e 3534     (xy 3.81 2.54
+00000770: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000780: 312e 3237 2031 2e30 3136 290a 2020 2020  1.27 1.016).    
+00000790: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+000007a0: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+000007b0: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+000007c0: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+000007d0: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+000007e0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000007f0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+00000800: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
+00000810: 3339 3720 2d31 2e30 3136 290a 2020 2020  397 -1.016).    
+00000820: 2020 2020 2020 2878 7920 322e 3033 3220        (xy 2.032 
+00000830: 2d32 2e32 3836 290a 2020 2020 2020 2020  -2.286).        
+00000840: 2020 2878 7920 322e 3739 3420 2d31 2e31    (xy 2.794 -1.1
+00000850: 3433 290a 2020 2020 2020 2020 2020 2878  43).          (x
+00000860: 7920 312e 3339 3720 2d31 2e30 3136 290a  y 1.397 -1.016).
+00000870: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000880: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+00000890: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
+000008a0: 7429 290a 2020 2020 2020 2020 2866 696c  t)).        (fil
+000008b0: 6c20 2874 7970 6520 6f75 746c 696e 6529  l (type outline)
+000008c0: 290a 2020 2020 2020 290a 2020 2020 290a  ).      ).    ).
+000008d0: 2020 2020 2873 796d 626f 6c20 2249 504e      (symbol "IPN
+000008e0: 5f31 5f31 220a 2020 2020 2020 2870 696e  _1_1".      (pin
+000008f0: 2069 6e70 7574 206c 696e 6520 2861 7420   input line (at 
+00000900: 2d33 2e38 3120 3020 3029 2028 6c65 6e67  -3.81 0 0) (leng
+00000910: 7468 2035 2e30 3829 0a20 2020 2020 2020  th 5.08).       
+00000920: 2028 6e61 6d65 2022 4222 2028 6566 6665   (name "B" (effe
+00000930: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000940: 312e 3237 2031 2e32 3729 2929 290a 2020  1.27 1.27)))).  
+00000950: 2020 2020 2020 286e 756d 6265 7220 227e        (number "~
+00000960: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+00000970: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000980: 2929 2929 0a20 2020 2020 2029 0a20 2020  )))).      ).   
+00000990: 2020 2028 7069 6e20 6f75 7470 7574 206c     (pin output l
+000009a0: 696e 6520 2861 7420 332e 3831 2037 2e36  ine (at 3.81 7.6
+000009b0: 3220 3237 3029 2028 6c65 6e67 7468 2035  2 270) (length 5
+000009c0: 2e30 3829 0a20 2020 2020 2020 2028 6e61  .08).        (na
+000009d0: 6d65 2022 4322 2028 6566 6665 6374 7320  me "C" (effects 
+000009e0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000009f0: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
+00000a00: 2020 286e 756d 6265 7220 227e 2220 2865    (number "~" (e
+00000a10: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000a20: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000a30: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
+00000a40: 7069 6e20 696e 7075 7420 6c69 6e65 2028  pin input line (
+00000a50: 6174 2033 2e38 3120 2d37 2e36 3220 3930  at 3.81 -7.62 90
+00000a60: 2920 286c 656e 6774 6820 352e 3038 290a  ) (length 5.08).
+00000a70: 2020 2020 2020 2020 286e 616d 6520 2245          (name "E
+00000a80: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+00000a90: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000aa0: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
+00000ab0: 6d62 6572 2022 7e22 2028 6566 6665 6374  mber "~" (effect
+00000ac0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00000ad0: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+00000ae0: 2020 290a 2020 2020 290a 2020 290a 290a    ).    ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/transistor-nfet.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/transistor-pfet.kicad_sym`

 * *Files 15% similar despite different names*

```diff
@@ -1,313 +1,312 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2251 2220 2869  eference" "Q" (i
-000000c0: 6420 3029 2028 6174 2030 2034 2e33 3138  d 0) (at 0 4.318
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2037 2e36 3220 332e  d 6) (at 7.62 3.
-00000370: 3831 2030 290a 2020 2020 2020 2865 6666  81 0).      (eff
-00000380: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000390: 2031 2e32 3720 312e 3237 2929 2028 6a75   1.27 1.27)) (ju
-000003a0: 7374 6966 7920 6c65 6674 2929 0a20 2020  stify left)).   
-000003b0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-000003c0: 2022 5261 7465 6420 566f 6c74 6167 6520   "Rated Voltage 
-000003d0: 2856 6f6c 7429 2220 2252 6174 6564 2056  (Volt)" "Rated V
-000003e0: 6f6c 7461 6765 2220 2869 6420 3729 2028  oltage" (id 7) (
-000003f0: 6174 2037 2e36 3220 312e 3237 2030 290a  at 7.62 1.27 0).
-00000400: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000410: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000420: 312e 3237 2929 2028 6a75 7374 6966 7920  1.27)) (justify 
-00000430: 6c65 6674 2929 0a20 2020 2029 0a20 2020  left)).    ).   
-00000440: 2028 7072 6f70 6572 7479 2022 5261 7465   (property "Rate
-00000450: 6420 4375 7272 656e 7420 2841 6d70 7329  d Current (Amps)
-00000460: 2220 2252 6174 6564 2043 7572 7265 6e74  " "Rated Current
-00000470: 2220 2869 6420 3829 2028 6174 2037 2e36  " (id 8) (at 7.6
-00000480: 3220 2d31 2e32 3720 3029 0a20 2020 2020  2 -1.27 0).     
-00000490: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000004a0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000004b0: 2920 286a 7573 7469 6679 206c 6566 7429  ) (justify left)
-000004c0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000004d0: 7065 7274 7920 2250 6163 6b61 6765 2054  perty "Package T
-000004e0: 7970 6522 2022 5061 636b 6167 6520 5479  ype" "Package Ty
-000004f0: 7065 2220 2869 6420 3929 2028 6174 2037  pe" (id 9) (at 7
-00000500: 2e36 3220 2d33 2e38 3120 3029 0a20 2020  .62 -3.81 0).   
-00000510: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-00000520: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000530: 3729 2920 286a 7573 7469 6679 206c 6566  7)) (justify lef
-00000540: 7429 290a 2020 2020 290a 2020 2020 2870  t)).    ).    (p
-00000550: 726f 7065 7274 7920 226b 695f 6b65 7977  roperty "ki_keyw
-00000560: 6f72 6473 2220 226b 6579 776f 7264 7322  ords" "keywords"
-00000570: 2028 6964 2031 3029 2028 6174 2030 2030   (id 10) (at 0 0
-00000580: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000590: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000005a0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000005b0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000005c0: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
-000005d0: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
-000005e0: 6f6e 2220 2869 6420 3131 2920 2861 7420  on" (id 11) (at 
-000005f0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000600: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000610: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000620: 6465 290a 2020 2020 290a 2020 2020 2873  de).    ).    (s
-00000630: 796d 626f 6c20 2249 504e 5f30 5f31 220a  ymbol "IPN_0_1".
-00000640: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000650: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-00000660: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
-00000670: 3029 0a20 2020 2020 2020 2020 2028 7879  0).          (xy
-00000680: 2031 2e32 3720 2d32 2e35 3429 0a20 2020   1.27 -2.54).   
-00000690: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-000006a0: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-000006b0: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000006c0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-000006d0: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-000006e0: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000006f0: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-00000700: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000710: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
-00000720: 2e32 3720 3029 0a20 2020 2020 2020 2020  .27 0).         
-00000730: 2028 7879 2031 2e32 3720 322e 3534 290a   (xy 1.27 2.54).
-00000740: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000750: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000760: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
-00000770: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-00000780: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
-00000790: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
-000007a0: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
-000007b0: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
-000007c0: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-000007d0: 7920 312e 3737 3820 2d31 2e32 3729 0a20  y 1.778 -1.27). 
-000007e0: 2020 2020 2020 2020 2028 7879 2031 2e37           (xy 1.7
-000007f0: 3738 202d 322e 3534 290a 2020 2020 2020  78 -2.54).      
-00000800: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
-00000810: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
-00000820: 7970 6520 6465 6661 756c 7429 2028 636f  ype default) (co
-00000830: 6c6f 7220 3020 3020 3020 3029 290a 2020  lor 0 0 0 0)).  
-00000840: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
-00000850: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
-00000860: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-00000870: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-00000880: 2020 2020 2020 2020 2878 7920 312e 3737          (xy 1.77
-00000890: 3820 2d30 2e36 3335 290a 2020 2020 2020  8 -0.635).      
-000008a0: 2020 2020 2878 7920 312e 3737 3820 302e      (xy 1.778 0.
-000008b0: 3633 3529 0a20 2020 2020 2020 2029 0a20  635).        ). 
-000008c0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-000008d0: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
-000008e0: 6566 6175 6c74 2920 2863 6f6c 6f72 2030  efault) (color 0
-000008f0: 2030 2030 2030 2929 0a20 2020 2020 2020   0 0 0)).       
-00000900: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
-00000910: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
-00000920: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
-00000930: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
-00000940: 2020 2028 7879 2031 2e37 3738 2031 2e32     (xy 1.778 1.2
-00000950: 3729 0a20 2020 2020 2020 2020 2028 7879  7).          (xy
-00000960: 2031 2e37 3738 2032 2e35 3429 0a20 2020   1.778 2.54).   
-00000970: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00000980: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00000990: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000009a0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-000009b0: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-000009c0: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000009d0: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-000009e0: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-000009f0: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
-00000a00: 2e38 3120 2d32 2e35 3429 0a20 2020 2020  .81 -2.54).     
-00000a10: 2020 2020 2028 7879 2033 2e38 3120 2d31       (xy 3.81 -1
-00000a20: 2e39 3035 290a 2020 2020 2020 2020 290a  .905).        ).
-00000a30: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
-00000a40: 2877 6964 7468 2030 2920 2874 7970 6520  (width 0) (type 
-00000a50: 6465 6661 756c 7429 2028 636f 6c6f 7220  default) (color 
-00000a60: 3020 3020 3020 3029 290a 2020 2020 2020  0 0 0 0)).      
-00000a70: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
-00000a80: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
-00000a90: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
-00000aa0: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
-00000ab0: 2020 2020 2878 7920 342e 3935 3320 302e      (xy 4.953 0.
-00000ac0: 3530 3829 0a20 2020 2020 2020 2020 2028  508).          (
-00000ad0: 7879 2036 2e32 3233 2030 2e35 3038 290a  xy 6.223 0.508).
-00000ae0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000af0: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000b00: 2030 2e31 3237 2920 2874 7970 6520 6465   0.127) (type de
-00000b10: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000b20: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000b30: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-00000b40: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00000b50: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
-00000b60: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
-00000b70: 2020 2878 7920 352e 3038 202d 302e 3633    (xy 5.08 -0.63
-00000b80: 3529 0a20 2020 2020 2020 2020 2028 7879  5).          (xy
-00000b90: 2034 2e39 3533 202d 302e 3633 3529 0a20   4.953 -0.635). 
-00000ba0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000bb0: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
-00000bc0: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
-00000bd0: 2920 2863 6f6c 6f72 2030 2030 2030 2030  ) (color 0 0 0 0
-00000be0: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
-00000bf0: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
-00000c00: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
-00000c10: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
-00000c20: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
-00000c30: 2031 2e37 3738 2031 2e39 3035 290a 2020   1.778 1.905).  
-00000c40: 2020 2020 2020 2020 2878 7920 332e 3831          (xy 3.81
-00000c50: 2031 2e39 3035 290a 2020 2020 2020 2020   1.905).        
-00000c60: 2020 2878 7920 332e 3831 2032 2e35 3429    (xy 3.81 2.54)
-00000c70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00000c80: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-00000c90: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-00000ca0: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00000cb0: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00000cc0: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
-00000cd0: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-00000ce0: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-00000cf0: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-00000d00: 7879 2035 2e35 3838 202d 302e 3633 3529  xy 5.588 -0.635)
-00000d10: 0a20 2020 2020 2020 2020 2028 7879 2035  .          (xy 5
-00000d20: 2e35 3838 202d 322e 3431 3329 0a20 2020  .588 -2.413).   
-00000d30: 2020 2020 2020 2028 7879 2033 2e38 3120         (xy 3.81 
-00000d40: 2d32 2e34 3133 290a 2020 2020 2020 2020  -2.413).        
-00000d50: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
-00000d60: 6520 2877 6964 7468 2030 2920 2874 7970  e (width 0) (typ
-00000d70: 6520 6465 6661 756c 7429 2028 636f 6c6f  e default) (colo
-00000d80: 7220 3020 3020 3020 3029 290a 2020 2020  r 0 0 0 0)).    
-00000d90: 2020 2020 2866 696c 6c20 2874 7970 6520      (fill (type 
-00000da0: 6e6f 6e65 2929 0a20 2020 2020 2029 0a20  none)).      ). 
-00000db0: 2020 2020 2028 706f 6c79 6c69 6e65 0a20       (polyline. 
-00000dc0: 2020 2020 2020 2028 7074 730a 2020 2020         (pts.    
-00000dd0: 2020 2020 2020 2878 7920 352e 3538 3820        (xy 5.588 
-00000de0: 302e 3633 3529 0a20 2020 2020 2020 2020  0.635).         
-00000df0: 2028 7879 2035 2e35 3838 2032 2e32 3836   (xy 5.588 2.286
-00000e00: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
-00000e10: 332e 3831 2032 2e32 3836 290a 2020 2020  3.81 2.286).    
-00000e20: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
-00000e30: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
-00000e40: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000e50: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-00000e60: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-00000e70: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-00000e80: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-00000e90: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-00000ea0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-00000eb0: 3737 3820 2d31 2e39 3035 290a 2020 2020  778 -1.905).    
-00000ec0: 2020 2020 2020 2878 7920 332e 3831 202d        (xy 3.81 -
-00000ed0: 312e 3930 3529 0a20 2020 2020 2020 2020  1.905).         
-00000ee0: 2028 7879 2033 2e38 3120 3029 0a20 2020   (xy 3.81 0).   
-00000ef0: 2020 2020 2020 2028 7879 2033 2e30 3438         (xy 3.048
-00000f00: 2030 290a 2020 2020 2020 2020 290a 2020   0).        ).  
-00000f10: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
-00000f20: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
-00000f30: 6661 756c 7429 2028 636f 6c6f 7220 3020  fault) (color 0 
-00000f40: 3020 3020 3029 290a 2020 2020 2020 2020  0 0 0)).        
-00000f50: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
-00000f60: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00000f70: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
-00000f80: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
-00000f90: 2020 2878 7920 312e 3930 3520 3029 0a20    (xy 1.905 0). 
-00000fa0: 2020 2020 2020 2020 2028 7879 2033 2e30           (xy 3.0
-00000fb0: 3438 2030 2e36 3335 290a 2020 2020 2020  48 0.635).      
-00000fc0: 2020 2020 2878 7920 332e 3034 3820 2d30      (xy 3.048 -0
-00000fd0: 2e36 3335 290a 2020 2020 2020 2020 2020  .635).          
-00000fe0: 2878 7920 312e 3930 3520 3029 0a20 2020  (xy 1.905 0).   
-00000ff0: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-00001000: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-00001010: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-00001020: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-00001030: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-00001040: 7479 7065 206f 7574 6c69 6e65 2929 0a20  type outline)). 
-00001050: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
-00001060: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
-00001070: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-00001080: 7920 342e 3935 3320 2d30 2e36 3335 290a  y 4.953 -0.635).
-00001090: 2020 2020 2020 2020 2020 2878 7920 352e            (xy 5.
-000010a0: 3538 3820 302e 3530 3829 0a20 2020 2020  588 0.508).     
-000010b0: 2020 2020 2028 7879 2036 2e32 3233 202d       (xy 6.223 -
-000010c0: 302e 3633 3529 0a20 2020 2020 2020 2020  0.635).         
-000010d0: 2028 7879 2035 2e30 3820 2d30 2e36 3335   (xy 5.08 -0.635
-000010e0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-000010f0: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-00001100: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-00001110: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-00001120: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-00001130: 696c 6c20 2874 7970 6520 6f75 746c 696e  ill (type outlin
-00001140: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
-00001150: 290a 2020 2020 2873 796d 626f 6c20 2249  ).    (symbol "I
-00001160: 504e 5f31 5f31 220a 2020 2020 2020 2870  PN_1_1".      (p
-00001170: 696e 2062 6964 6972 6563 7469 6f6e 616c  in bidirectional
-00001180: 206c 696e 6520 2861 7420 332e 3831 2037   line (at 3.81 7
-00001190: 2e36 3220 3237 3029 2028 6c65 6e67 7468  .62 270) (length
-000011a0: 2035 2e30 3829 0a20 2020 2020 2020 2028   5.08).        (
-000011b0: 6e61 6d65 2022 4422 2028 6566 6665 6374  name "D" (effect
-000011c0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000011d0: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-000011e0: 2020 2020 286e 756d 6265 7220 227e 2220      (number "~" 
-000011f0: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00001200: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00001210: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
-00001220: 2028 7069 6e20 696e 7075 7420 6c69 6e65   (pin input line
-00001230: 2028 6174 202d 332e 3831 2030 2030 2920   (at -3.81 0 0) 
-00001240: 286c 656e 6774 6820 352e 3038 290a 2020  (length 5.08).  
-00001250: 2020 2020 2020 286e 616d 6520 2247 2220        (name "G" 
-00001260: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
-00001270: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
-00001280: 2929 0a20 2020 2020 2020 2028 6e75 6d62  )).        (numb
-00001290: 6572 2022 7e22 2028 6566 6665 6374 7320  er "~" (effects 
-000012a0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-000012b0: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-000012c0: 290a 2020 2020 2020 2870 696e 2062 6964  ).      (pin bid
-000012d0: 6972 6563 7469 6f6e 616c 206c 696e 6520  irectional line 
-000012e0: 2861 7420 332e 3831 202d 372e 3632 2039  (at 3.81 -7.62 9
-000012f0: 3029 2028 6c65 6e67 7468 2035 2e30 3829  0) (length 5.08)
-00001300: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
-00001310: 5322 2028 6566 6665 6374 7320 2866 6f6e  S" (effects (fon
-00001320: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00001330: 3729 2929 290a 2020 2020 2020 2020 286e  7)))).        (n
-00001340: 756d 6265 7220 227e 2220 2865 6666 6563  umber "~" (effec
-00001350: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00001360: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-00001370: 2020 2029 0a20 2020 2029 0a20 2029 0a29     ).    ).  ).)
-00001380: 0a                                       .
+000000b0: 6566 6572 656e 6365 2220 2251 2220 2861  eference" "Q" (a
+000000c0: 7420 3020 342e 3331 3820 3029 0a20 2020  t 0 4.318 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 372e 3632 2033 2e38  ue" (at 7.62 3.8
+00000340: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+00000350: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000360: 312e 3237 2031 2e32 3729 2920 286a 7573  1.27 1.27)) (jus
+00000370: 7469 6679 206c 6566 7429 290a 2020 2020  tify left)).    
+00000380: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+00000390: 2252 6174 6564 2056 6f6c 7461 6765 2028  "Rated Voltage (
+000003a0: 566f 6c74 2922 2022 5261 7465 6420 566f  Volt)" "Rated Vo
+000003b0: 6c74 6167 6522 2028 6174 2037 2e36 3220  ltage" (at 7.62 
+000003c0: 312e 3237 2030 290a 2020 2020 2020 2865  1.27 0).      (e
+000003d0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+000003e0: 7a65 2031 2e32 3720 312e 3237 2929 2028  ze 1.27 1.27)) (
+000003f0: 6a75 7374 6966 7920 6c65 6674 2929 0a20  justify left)). 
+00000400: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000410: 7479 2022 5261 7465 6420 4375 7272 656e  ty "Rated Curren
+00000420: 7420 2841 6d70 7329 2220 2252 6174 6564  t (Amps)" "Rated
+00000430: 2043 7572 7265 6e74 2220 2861 7420 372e   Current" (at 7.
+00000440: 3632 202d 312e 3237 2030 290a 2020 2020  62 -1.27 0).    
+00000450: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000460: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000470: 2929 2028 6a75 7374 6966 7920 6c65 6674  )) (justify left
+00000480: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000490: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
+000004a0: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
+000004b0: 7970 6522 2028 6174 2037 2e36 3220 2d33  ype" (at 7.62 -3
+000004c0: 2e38 3120 3029 0a20 2020 2020 2028 6566  .81 0).      (ef
+000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000004e0: 6520 312e 3237 2031 2e32 3729 2920 286a  e 1.27 1.27)) (j
+000004f0: 7573 7469 6679 206c 6566 7429 290a 2020  ustify left)).  
+00000500: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+00000510: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
+00000520: 226b 6579 776f 7264 7322 2028 6174 2030  "keywords" (at 0
+00000530: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
+00000540: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000550: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000560: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000570: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
+00000580: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
+00000590: 7469 6f6e 2220 2861 7420 3020 3020 3029  tion" (at 0 0 0)
+000005a0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+000005b0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000005c0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000005d0: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+000005e0: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
+000005f0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000600: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000610: 2028 7879 2031 2e32 3720 3029 0a20 2020   (xy 1.27 0).   
+00000620: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
+00000630: 2d32 2e35 3429 0a20 2020 2020 2020 2029  -2.54).        )
+00000640: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000650: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000660: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000670: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000680: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000690: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
+000006a0: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
+000006b0: 2020 2020 2028 7879 2031 2e32 3720 3029       (xy 1.27 0)
+000006c0: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
+000006d0: 2e32 3720 322e 3534 290a 2020 2020 2020  .27 2.54).      
+000006e0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+000006f0: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
+00000700: 7970 6520 6465 6661 756c 7429 290a 2020  ype default)).  
+00000710: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
+00000720: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
+00000730: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
+00000740: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
+00000750: 2020 2020 2020 2020 2878 7920 312e 3737          (xy 1.77
+00000760: 3820 2d31 2e39 3035 290a 2020 2020 2020  8 -1.905).      
+00000770: 2020 2020 2878 7920 332e 3831 202d 312e      (xy 3.81 -1.
+00000780: 3930 3529 0a20 2020 2020 2020 2029 0a20  905).        ). 
+00000790: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+000007a0: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
+000007b0: 6566 6175 6c74 2929 0a20 2020 2020 2020  efault)).       
+000007c0: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
+000007d0: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+000007e0: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
+000007f0: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
+00000800: 2020 2028 7879 2031 2e37 3738 202d 312e     (xy 1.778 -1.
+00000810: 3237 290a 2020 2020 2020 2020 2020 2878  27).          (x
+00000820: 7920 312e 3737 3820 2d32 2e35 3429 0a20  y 1.778 -2.54). 
+00000830: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000840: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000850: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
+00000860: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+00000870: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+00000880: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+00000890: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000008a0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000008b0: 2031 2e37 3738 202d 302e 3633 3529 0a20   1.778 -0.635). 
+000008c0: 2020 2020 2020 2020 2028 7879 2031 2e37           (xy 1.7
+000008d0: 3738 2030 2e36 3335 290a 2020 2020 2020  78 0.635).      
+000008e0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+000008f0: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
+00000900: 7970 6520 6465 6661 756c 7429 290a 2020  ype default)).  
+00000910: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
+00000920: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
+00000930: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
+00000940: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
+00000950: 2020 2020 2020 2020 2878 7920 312e 3737          (xy 1.77
+00000960: 3820 3029 0a20 2020 2020 2020 2020 2028  8 0).          (
+00000970: 7879 2032 2e36 3637 2030 290a 2020 2020  xy 2.667 0).    
+00000980: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+00000990: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+000009a0: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+000009b0: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+000009c0: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
+000009d0: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
+000009e0: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
+000009f0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
+00000a00: 3737 3820 312e 3237 290a 2020 2020 2020  778 1.27).      
+00000a10: 2020 2020 2878 7920 312e 3737 3820 322e      (xy 1.778 2.
+00000a20: 3534 290a 2020 2020 2020 2020 290a 2020  54).        ).  
+00000a30: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+00000a40: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
+00000a50: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+00000a60: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
+00000a70: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+00000a80: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
+00000a90: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
+00000aa0: 2020 2878 7920 332e 3831 202d 322e 3534    (xy 3.81 -2.54
+00000ab0: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000ac0: 332e 3831 202d 312e 3930 3529 0a20 2020  3.81 -1.905).   
+00000ad0: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
+00000ae0: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
+00000af0: 2028 7479 7065 2064 6566 6175 6c74 2929   (type default))
+00000b00: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
+00000b10: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
+00000b20: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
+00000b30: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
+00000b40: 0a20 2020 2020 2020 2020 2028 7879 2034  .          (xy 4
+00000b50: 2e39 3533 202d 302e 3633 3529 0a20 2020  .953 -0.635).   
+00000b60: 2020 2020 2020 2028 7879 2036 2e32 3233         (xy 6.223
+00000b70: 202d 302e 3633 3529 0a20 2020 2020 2020   -0.635).       
+00000b80: 2029 0a20 2020 2020 2020 2028 7374 726f   ).        (stro
+00000b90: 6b65 2028 7769 6474 6820 302e 3132 3729  ke (width 0.127)
+00000ba0: 2028 7479 7065 2064 6566 6175 6c74 2929   (type default))
+00000bb0: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
+00000bc0: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
+00000bd0: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
+00000be0: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
+00000bf0: 0a20 2020 2020 2020 2020 2028 7879 2035  .          (xy 5
+00000c00: 2e30 3820 302e 3530 3829 0a20 2020 2020  .08 0.508).     
+00000c10: 2020 2020 2028 7879 2034 2e39 3533 2030       (xy 4.953 0
+00000c20: 2e35 3038 290a 2020 2020 2020 2020 290a  .508).        ).
+00000c30: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
+00000c40: 2877 6964 7468 2030 2920 2874 7970 6520  (width 0) (type 
+00000c50: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00000c60: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+00000c70: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+00000c80: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
+00000c90: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
+00000ca0: 2020 2020 2878 7920 312e 3737 3820 312e      (xy 1.778 1.
+00000cb0: 3930 3529 0a20 2020 2020 2020 2020 2028  905).          (
+00000cc0: 7879 2033 2e38 3120 312e 3930 3529 0a20  xy 3.81 1.905). 
+00000cd0: 2020 2020 2020 2020 2028 7879 2033 2e38           (xy 3.8
+00000ce0: 3120 322e 3534 290a 2020 2020 2020 2020  1 2.54).        
+00000cf0: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
+00000d00: 6520 2877 6964 7468 2030 2920 2874 7970  e (width 0) (typ
+00000d10: 6520 6465 6661 756c 7429 290a 2020 2020  e default)).    
+00000d20: 2020 2020 2866 696c 6c20 2874 7970 6520      (fill (type 
+00000d30: 6e6f 6e65 2929 0a20 2020 2020 2029 0a20  none)).      ). 
+00000d40: 2020 2020 2028 706f 6c79 6c69 6e65 0a20       (polyline. 
+00000d50: 2020 2020 2020 2028 7074 730a 2020 2020         (pts.    
+00000d60: 2020 2020 2020 2878 7920 332e 3638 3320        (xy 3.683 
+00000d70: 3029 0a20 2020 2020 2020 2020 2028 7879  0).          (xy
+00000d80: 2033 2e38 3120 3029 0a20 2020 2020 2020   3.81 0).       
+00000d90: 2020 2028 7879 2033 2e38 3120 2d31 2e39     (xy 3.81 -1.9
+00000da0: 3035 290a 2020 2020 2020 2020 290a 2020  05).        ).  
+00000db0: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+00000dc0: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
+00000dd0: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+00000de0: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
+00000df0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+00000e00: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
+00000e10: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
+00000e20: 2020 2878 7920 352e 3538 3820 2d30 2e36    (xy 5.588 -0.6
+00000e30: 3335 290a 2020 2020 2020 2020 2020 2878  35).          (x
+00000e40: 7920 352e 3538 3820 2d32 2e34 3133 290a  y 5.588 -2.413).
+00000e50: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
+00000e60: 3831 202d 322e 3431 3329 0a20 2020 2020  81 -2.413).     
+00000e70: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
+00000e80: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
+00000e90: 7479 7065 2064 6566 6175 6c74 2929 0a20  type default)). 
+00000ea0: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
+00000eb0: 7065 206e 6f6e 6529 290a 2020 2020 2020  pe none)).      
+00000ec0: 290a 2020 2020 2020 2870 6f6c 796c 696e  ).      (polylin
+00000ed0: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+00000ee0: 2020 2020 2020 2020 2028 7879 2035 2e35           (xy 5.5
+00000ef0: 3838 2030 2e35 3038 290a 2020 2020 2020  88 0.508).      
+00000f00: 2020 2020 2878 7920 352e 3538 3820 322e      (xy 5.588 2.
+00000f10: 3238 3629 0a20 2020 2020 2020 2020 2028  286).          (
+00000f20: 7879 2033 2e38 3120 322e 3238 3629 0a20  xy 3.81 2.286). 
+00000f30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000f40: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000f50: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
+00000f60: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+00000f70: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+00000f80: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+00000f90: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+00000fa0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+00000fb0: 2033 2e36 3833 2030 290a 2020 2020 2020   3.683 0).      
+00000fc0: 2020 2020 2878 7920 322e 3636 3720 302e      (xy 2.667 0.
+00000fd0: 3736 3229 0a20 2020 2020 2020 2020 2028  762).          (
+00000fe0: 7879 2032 2e36 3637 202d 302e 3736 3229  xy 2.667 -0.762)
+00000ff0: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
+00001000: 2e36 3833 2030 290a 2020 2020 2020 2020  .683 0).        
+00001010: 290a 2020 2020 2020 2020 2873 7472 6f6b  ).        (strok
+00001020: 6520 2877 6964 7468 2030 2920 2874 7970  e (width 0) (typ
+00001030: 6520 6465 6661 756c 7429 290a 2020 2020  e default)).    
+00001040: 2020 2020 2866 696c 6c20 2874 7970 6520      (fill (type 
+00001050: 6f75 746c 696e 6529 290a 2020 2020 2020  outline)).      
+00001060: 290a 2020 2020 2020 2870 6f6c 796c 696e  ).      (polylin
+00001070: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+00001080: 2020 2020 2020 2020 2028 7879 2034 2e39           (xy 4.9
+00001090: 3533 2030 2e35 3038 290a 2020 2020 2020  53 0.508).      
+000010a0: 2020 2020 2878 7920 352e 3538 3820 2d30      (xy 5.588 -0
+000010b0: 2e36 3335 290a 2020 2020 2020 2020 2020  .635).          
+000010c0: 2878 7920 362e 3232 3320 302e 3530 3829  (xy 6.223 0.508)
+000010d0: 0a20 2020 2020 2020 2020 2028 7879 2035  .          (xy 5
+000010e0: 2e30 3820 302e 3530 3829 0a20 2020 2020  .08 0.508).     
+000010f0: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
+00001100: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
+00001110: 7479 7065 2064 6566 6175 6c74 2929 0a20  type default)). 
+00001120: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
+00001130: 7065 206f 7574 6c69 6e65 2929 0a20 2020  pe outline)).   
+00001140: 2020 2029 0a20 2020 2029 0a20 2020 2028     ).    ).    (
+00001150: 7379 6d62 6f6c 2022 4950 4e5f 315f 3122  symbol "IPN_1_1"
+00001160: 0a20 2020 2020 2028 7069 6e20 6269 6469  .      (pin bidi
+00001170: 7265 6374 696f 6e61 6c20 6c69 6e65 2028  rectional line (
+00001180: 6174 2033 2e38 3120 372e 3632 2032 3730  at 3.81 7.62 270
+00001190: 2920 286c 656e 6774 6820 352e 3038 290a  ) (length 5.08).
+000011a0: 2020 2020 2020 2020 286e 616d 6520 2244          (name "D
+000011b0: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
+000011c0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000011d0: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
+000011e0: 6d62 6572 2022 7e22 2028 6566 6665 6374  mber "~" (effect
+000011f0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00001200: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+00001210: 2020 290a 2020 2020 2020 2870 696e 2069    ).      (pin i
+00001220: 6e70 7574 206c 696e 6520 2861 7420 2d33  nput line (at -3
+00001230: 2e38 3120 3020 3029 2028 6c65 6e67 7468  .81 0 0) (length
+00001240: 2035 2e30 3829 0a20 2020 2020 2020 2028   5.08).        (
+00001250: 6e61 6d65 2022 4722 2028 6566 6665 6374  name "G" (effect
+00001260: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
+00001270: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
+00001280: 2020 2020 286e 756d 6265 7220 227e 2220      (number "~" 
+00001290: 2865 6666 6563 7473 2028 666f 6e74 2028  (effects (font (
+000012a0: 7369 7a65 2031 2e32 3720 312e 3237 2929  size 1.27 1.27))
+000012b0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+000012c0: 2028 7069 6e20 6269 6469 7265 6374 696f   (pin bidirectio
+000012d0: 6e61 6c20 6c69 6e65 2028 6174 2033 2e38  nal line (at 3.8
+000012e0: 3120 2d37 2e36 3220 3930 2920 286c 656e  1 -7.62 90) (len
+000012f0: 6774 6820 352e 3038 290a 2020 2020 2020  gth 5.08).      
+00001300: 2020 286e 616d 6520 2253 2220 2865 6666    (name "S" (eff
+00001310: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00001320: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
+00001330: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
+00001340: 7e22 2028 6566 6665 6374 7320 2866 6f6e  ~" (effects (fon
+00001350: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00001360: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
+00001370: 2020 290a 2020 290a 290a                   ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/transistor-npn.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/capacitor-polarized.kicad_sym`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,193 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2251 2220 2869  eference" "Q" (i
-000000c0: 6420 3029 2028 6174 2030 2034 2e33 3138  d 0) (at 0 4.318
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2035 2e30 3820 332e  d 6) (at 5.08 3.
-00000370: 3831 2030 290a 2020 2020 2020 2865 6666  81 0).      (eff
-00000380: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000390: 2031 2e32 3720 312e 3237 2929 2028 6a75   1.27 1.27)) (ju
-000003a0: 7374 6966 7920 6c65 6674 2929 0a20 2020  stify left)).   
-000003b0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-000003c0: 2022 5261 7465 6420 566f 6c74 6167 6520   "Rated Voltage 
-000003d0: 2856 6f6c 7429 2220 2252 6174 6564 2056  (Volt)" "Rated V
-000003e0: 6f6c 7461 6765 2220 2869 6420 3729 2028  oltage" (id 7) (
-000003f0: 6174 2035 2e30 3820 312e 3237 2030 290a  at 5.08 1.27 0).
-00000400: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000410: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000420: 312e 3237 2929 2028 6a75 7374 6966 7920  1.27)) (justify 
-00000430: 6c65 6674 2929 0a20 2020 2029 0a20 2020  left)).    ).   
-00000440: 2028 7072 6f70 6572 7479 2022 5261 7465   (property "Rate
-00000450: 6420 4375 7272 656e 7420 2841 6d70 7329  d Current (Amps)
-00000460: 2220 2252 6174 6564 2043 7572 7265 6e74  " "Rated Current
-00000470: 2220 2869 6420 3829 2028 6174 2035 2e30  " (id 8) (at 5.0
-00000480: 3820 2d31 2e32 3720 3029 0a20 2020 2020  8 -1.27 0).     
-00000490: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000004a0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000004b0: 2920 286a 7573 7469 6679 206c 6566 7429  ) (justify left)
-000004c0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000004d0: 7065 7274 7920 2250 6163 6b61 6765 2054  perty "Package T
-000004e0: 7970 6522 2022 5061 636b 6167 6520 5479  ype" "Package Ty
-000004f0: 7065 2220 2869 6420 3929 2028 6174 2035  pe" (id 9) (at 5
-00000500: 2e30 3820 2d33 2e38 3120 3029 0a20 2020  .08 -3.81 0).   
+000000b0: 6566 6572 656e 6365 2220 2243 2220 2861  eference" "C" (a
+000000c0: 7420 3020 332e 3831 2030 290a 2020 2020  t 0 3.81 0).    
+000000d0: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+000000e0: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+000000f0: 2929 290a 2020 2020 290a 2020 2020 2870  ))).    ).    (p
+00000100: 726f 7065 7274 7920 2256 616c 7565 2220  roperty "Value" 
+00000110: 2249 504e 2220 2861 7420 3020 2d31 312e  "IPN" (at 0 -11.
+00000120: 3433 2030 290a 2020 2020 2020 2865 6666  43 0).      (eff
+00000130: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000140: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000150: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000160: 6f70 6572 7479 2022 466f 6f74 7072 696e  operty "Footprin
+00000170: 7422 2022 466f 6f74 7072 696e 7422 2028  t" "Footprint" (
+00000180: 6174 2030 202d 3139 2e30 3520 3029 0a20  at 0 -19.05 0). 
+00000190: 2020 2020 2028 6566 6665 6374 7320 2866       (effects (f
+000001a0: 6f6e 7420 2873 697a 6520 312e 3237 2031  ont (size 1.27 1
+000001b0: 2e32 3729 2920 6869 6465 290a 2020 2020  .27)) hide).    
+000001c0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000001d0: 2244 6174 6173 6865 6574 2220 2269 6e76  "Datasheet" "inv
+000001e0: 656e 7472 6565 5f75 726c 2220 2861 7420  entree_url" (at 
+000001f0: 3020 2d32 312e 3539 2030 290a 2020 2020  0 -21.59 0).    
+00000200: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000210: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000220: 2929 2068 6964 6529 0a20 2020 2029 0a20  )) hide).    ). 
+00000230: 2020 2028 7072 6f70 6572 7479 2022 4d61     (property "Ma
+00000240: 6e75 6661 6374 7572 6572 2220 224d 616e  nufacturer" "Man
+00000250: 7566 6163 7475 7265 7222 2028 6174 2030  ufacturer" (at 0
+00000260: 202d 3133 2e39 3720 3029 0a20 2020 2020   -13.97 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3136 2e35 3120 3029 0a20 2020   0 -16.51 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2243      (property "C
+00000320: 6170 6163 6974 616e 6365 2028 4661 7261  apacitance (Fara
+00000330: 6429 2220 2256 616c 7565 2220 2861 7420  d)" "Value" (at 
+00000340: 3020 2d33 2e38 3120 3029 0a20 2020 2020  0 -3.81 0).     
+00000350: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000360: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000370: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000380: 6f70 6572 7479 2022 546f 6c65 7261 6e63  operty "Toleranc
+00000390: 6520 2825 2922 2022 546f 6c65 7261 6e63  e (%)" "Toleranc
+000003a0: 6522 2028 6174 2035 2e30 3820 2d33 2e38  e" (at 5.08 -3.8
+000003b0: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+000003c0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+000003d0: 312e 3237 2031 2e32 3729 2920 286a 7573  1.27 1.27)) (jus
+000003e0: 7469 6679 206c 6566 7429 2068 6964 6529  tify left) hide)
+000003f0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
+00000400: 6572 7479 2022 566f 6c74 6167 6520 5261  erty "Voltage Ra
+00000410: 7465 6420 2856 6f6c 7429 2220 2252 6174  ted (Volt)" "Rat
+00000420: 6564 2056 6f6c 7461 6765 2220 2861 7420  ed Voltage" (at 
+00000430: 3020 2d36 2e33 3520 3029 0a20 2020 2020  0 -6.35 0).     
+00000440: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000450: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000460: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000470: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
+00000480: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
+00000490: 7970 6522 2028 6174 2030 202d 382e 3839  ype" (at 0 -8.89
+000004a0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
+000004b0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000004c0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
+000004d0: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+000004e0: 2250 6163 6b61 6765 2053 697a 6522 2022  "Package Size" "
+000004f0: 5061 636b 6167 6520 5369 7a65 2220 2861  Package Size" (a
+00000500: 7420 3020 2d38 2e38 3920 3029 0a20 2020  t 0 -8.89 0).   
 00000510: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
 00000520: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000530: 3729 2920 286a 7573 7469 6679 206c 6566  7)) (justify lef
-00000540: 7429 290a 2020 2020 290a 2020 2020 2870  t)).    ).    (p
-00000550: 726f 7065 7274 7920 226b 695f 6b65 7977  roperty "ki_keyw
-00000560: 6f72 6473 2220 226b 6579 776f 7264 7322  ords" "keywords"
-00000570: 2028 6964 2031 3029 2028 6174 2030 2030   (id 10) (at 0 0
-00000580: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000590: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000005a0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000005b0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000005c0: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
-000005d0: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
-000005e0: 6f6e 2220 2869 6420 3131 2920 2861 7420  on" (id 11) (at 
-000005f0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000600: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000610: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000620: 6465 290a 2020 2020 290a 2020 2020 2873  de).    ).    (s
-00000630: 796d 626f 6c20 2249 504e 5f30 5f31 220a  ymbol "IPN_0_1".
-00000640: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000650: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-00000660: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
-00000670: 322e 3238 3629 0a20 2020 2020 2020 2020  2.286).         
-00000680: 2028 7879 2031 2e32 3720 2d32 2e32 3836   (xy 1.27 -2.286
-00000690: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-000006a0: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-000006b0: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-000006c0: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-000006d0: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-000006e0: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-000006f0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000700: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
-00000710: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
-00000720: 2878 7920 332e 3831 202d 322e 3534 290a  (xy 3.81 -2.54).
-00000730: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-00000740: 3237 202d 312e 3031 3629 0a20 2020 2020  27 -1.016).     
-00000750: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
-00000760: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
-00000770: 7479 7065 2064 6566 6175 6c74 2920 2863  type default) (c
-00000780: 6f6c 6f72 2030 2030 2030 2030 2929 0a20  olor 0 0 0 0)). 
-00000790: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
-000007a0: 7065 206e 6f6e 6529 290a 2020 2020 2020  pe none)).      
-000007b0: 290a 2020 2020 2020 2870 6f6c 796c 696e  ).      (polylin
-000007c0: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
-000007d0: 2020 2020 2020 2020 2028 7879 2033 2e38           (xy 3.8
-000007e0: 3120 322e 3534 290a 2020 2020 2020 2020  1 2.54).        
-000007f0: 2020 2878 7920 312e 3237 2031 2e30 3136    (xy 1.27 1.016
-00000800: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00000810: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-00000820: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-00000830: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-00000840: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-00000850: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-00000860: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000870: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
-00000880: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
-00000890: 2878 7920 332e 3831 202d 322e 3534 290a  (xy 3.81 -2.54).
-000008a0: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
-000008b0: 3137 3520 2d31 2e32 3729 0a20 2020 2020  175 -1.27).     
-000008c0: 2020 2020 2028 7879 2032 2e34 3133 202d       (xy 2.413 -
-000008d0: 322e 3431 3329 0a20 2020 2020 2020 2020  2.413).         
-000008e0: 2028 7879 2033 2e38 3120 2d32 2e35 3429   (xy 3.81 -2.54)
-000008f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00000900: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-00000910: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-00000920: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00000930: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00000940: 6c6c 2028 7479 7065 206f 7574 6c69 6e65  ll (type outline
-00000950: 2929 0a20 2020 2020 2029 0a20 2020 2029  )).      ).    )
-00000960: 0a20 2020 2028 7379 6d62 6f6c 2022 4950  .    (symbol "IP
-00000970: 4e5f 315f 3122 0a20 2020 2020 2028 7069  N_1_1".      (pi
-00000980: 6e20 696e 7075 7420 6c69 6e65 2028 6174  n input line (at
-00000990: 202d 332e 3831 2030 2030 2920 286c 656e   -3.81 0 0) (len
-000009a0: 6774 6820 352e 3038 290a 2020 2020 2020  gth 5.08).      
-000009b0: 2020 286e 616d 6520 2242 2220 2865 6666    (name "B" (eff
-000009c0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-000009d0: 2031 2e32 3720 312e 3237 2929 2929 0a20   1.27 1.27)))). 
-000009e0: 2020 2020 2020 2028 6e75 6d62 6572 2022         (number "
-000009f0: 7e22 2028 6566 6665 6374 7320 2866 6f6e  ~" (effects (fon
-00000a00: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000a10: 3729 2929 290a 2020 2020 2020 290a 2020  7)))).      ).  
-00000a20: 2020 2020 2870 696e 2069 6e70 7574 206c      (pin input l
-00000a30: 696e 6520 2861 7420 332e 3831 2037 2e36  ine (at 3.81 7.6
-00000a40: 3220 3237 3029 2028 6c65 6e67 7468 2035  2 270) (length 5
-00000a50: 2e30 3829 0a20 2020 2020 2020 2028 6e61  .08).        (na
-00000a60: 6d65 2022 4322 2028 6566 6665 6374 7320  me "C" (effects 
-00000a70: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
-00000a80: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
-00000a90: 2020 286e 756d 6265 7220 227e 2220 2865    (number "~" (e
-00000aa0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
-00000ab0: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
-00000ac0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000ad0: 7069 6e20 6f75 7470 7574 206c 696e 6520  pin output line 
-00000ae0: 2861 7420 332e 3831 202d 372e 3632 2039  (at 3.81 -7.62 9
-00000af0: 3029 2028 6c65 6e67 7468 2035 2e30 3829  0) (length 5.08)
-00000b00: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
-00000b10: 4522 2028 6566 6665 6374 7320 2866 6f6e  E" (effects (fon
-00000b20: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000b30: 3729 2929 290a 2020 2020 2020 2020 286e  7)))).        (n
-00000b40: 756d 6265 7220 227e 2220 2865 6666 6563  umber "~" (effec
-00000b50: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-00000b60: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
-00000b70: 2020 2029 0a20 2020 2029 0a20 2029 0a29     ).    ).  ).)
-00000b80: 0a                                       .
+00000530: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000540: 2020 2020 2870 726f 7065 7274 7920 2245      (property "E
+00000550: 5352 2028 4f68 6d29 2220 2245 5352 2220  SR (Ohm)" "ESR" 
+00000560: 2861 7420 352e 3038 202d 362e 3335 2030  (at 5.08 -6.35 0
+00000570: 290a 2020 2020 2020 2865 6666 6563 7473  ).      (effects
+00000580: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
+00000590: 3720 312e 3237 2929 2028 6a75 7374 6966  7 1.27)) (justif
+000005a0: 7920 6c65 6674 2920 6869 6465 290a 2020  y left) hide).  
+000005b0: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+000005c0: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
+000005d0: 226b 6579 776f 7264 7322 2028 6174 2030  "keywords" (at 0
+000005e0: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
+000005f0: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000600: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000610: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000620: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
+00000630: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
+00000640: 7469 6f6e 2220 2861 7420 3020 3020 3029  tion" (at 0 0 0)
+00000650: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+00000660: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000670: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+00000680: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+00000690: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
+000006a0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+000006b0: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+000006c0: 2028 7879 202d 312e 3737 3820 2d30 2e33   (xy -1.778 -0.3
+000006d0: 3831 290a 2020 2020 2020 2020 2020 2878  81).          (x
+000006e0: 7920 2d31 2e37 3738 202d 312e 3635 3129  y -1.778 -1.651)
+000006f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00000700: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
+00000710: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
+00000720: 6c74 2929 0a20 2020 2020 2020 2028 6669  lt)).        (fi
+00000730: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
+00000740: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
+00000750: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
+00000760: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
+00000770: 7879 202d 312e 3237 2030 290a 2020 2020  xy -1.27 0).    
+00000780: 2020 2020 2020 2878 7920 2d30 2e36 3335        (xy -0.635
+00000790: 2030 290a 2020 2020 2020 2020 290a 2020   0).        ).  
+000007a0: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+000007b0: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
+000007c0: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+000007d0: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
+000007e0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+000007f0: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
+00000800: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
+00000810: 2020 2878 7920 2d31 2e31 3433 202d 312e    (xy -1.143 -1.
+00000820: 3031 3629 0a20 2020 2020 2020 2020 2028  016).          (
+00000830: 7879 202d 322e 3431 3320 2d31 2e30 3136  xy -2.413 -1.016
+00000840: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00000850: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+00000860: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
+00000870: 756c 7429 290a 2020 2020 2020 2020 2866  ult)).        (f
+00000880: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
+00000890: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
+000008a0: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
+000008b0: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
+000008c0: 2878 7920 2d30 2e36 3335 202d 312e 3930  (xy -0.635 -1.90
+000008d0: 3529 0a20 2020 2020 2020 2020 2028 7879  5).          (xy
+000008e0: 202d 302e 3633 3520 312e 3930 3529 0a20   -0.635 1.905). 
+000008f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000900: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000910: 302e 3235 3429 2028 7479 7065 2064 6566  0.254) (type def
+00000920: 6175 6c74 2929 0a20 2020 2020 2020 2028  ault)).        (
+00000930: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
+00000940: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
+00000950: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000960: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000970: 2028 7879 2031 2e35 3234 2030 290a 2020   (xy 1.524 0).  
+00000980: 2020 2020 2020 2020 2878 7920 302e 3633          (xy 0.63
+00000990: 3520 3029 0a20 2020 2020 2020 2029 0a20  5 0).        ). 
+000009a0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
+000009b0: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
+000009c0: 6566 6175 6c74 2929 0a20 2020 2020 2020  efault)).       
+000009d0: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
+000009e0: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
+000009f0: 2020 2861 7263 2028 7374 6172 7420 312e    (arc (start 1.
+00000a00: 3532 3420 312e 3930 3529 2028 6d69 6420  524 1.905) (mid 
+00000a10: 302e 3833 3433 2030 2920 2865 6e64 2031  0.8343 0) (end 1
+00000a20: 2e35 3234 202d 312e 3930 3529 0a20 2020  .524 -1.905).   
+00000a30: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
+00000a40: 6474 6820 302e 3235 3429 2028 7479 7065  dth 0.254) (type
+00000a50: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000a60: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000a70: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000a80: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+00000a90: 2249 504e 5f31 5f31 220a 2020 2020 2020  "IPN_1_1".      
+00000aa0: 2870 696e 2070 6173 7369 7665 206c 696e  (pin passive lin
+00000ab0: 6520 2861 7420 2d33 2e38 3120 3020 3029  e (at -3.81 0 0)
+00000ac0: 2028 6c65 6e67 7468 2032 2e35 3429 0a20   (length 2.54). 
+00000ad0: 2020 2020 2020 2028 6e61 6d65 2022 506f         (name "Po
+00000ae0: 7369 7469 6622 2028 6566 6665 6374 7320  sitif" (effects 
+00000af0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000b00: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
+00000b10: 2020 286e 756d 6265 7220 2231 2220 2865    (number "1" (e
+00000b20: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000b30: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000b40: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
+00000b50: 7069 6e20 7061 7373 6976 6520 6c69 6e65  pin passive line
+00000b60: 2028 6174 2033 2e38 3120 3020 3138 3029   (at 3.81 0 180)
+00000b70: 2028 6c65 6e67 7468 2032 2e35 3429 0a20   (length 2.54). 
+00000b80: 2020 2020 2020 2028 6e61 6d65 2022 4e65         (name "Ne
+00000b90: 6761 7469 6622 2028 6566 6665 6374 7320  gatif" (effects 
+00000ba0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+00000bb0: 2031 2e32 3729 2929 290a 2020 2020 2020   1.27)))).      
+00000bc0: 2020 286e 756d 6265 7220 2232 2220 2865    (number "2" (e
+00000bd0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+00000be0: 7a65 2031 2e32 3720 312e 3237 2929 2929  ze 1.27 1.27))))
+00000bf0: 0a20 2020 2020 2029 0a20 2020 2029 0a20  .      ).    ). 
+00000c00: 2029 0a29 0a                              ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates/transistor-pfet.kicad_sym` & `kintree-1.0.0rc0/kintree/kicad/templates/transistor-nfet.kicad_sym`

 * *Files 15% similar despite different names*

```diff
@@ -1,333 +1,293 @@
 00000000: 286b 6963 6164 5f73 796d 626f 6c5f 6c69  (kicad_symbol_li
-00000010: 6220 2876 6572 7369 6f6e 2032 3032 3131  b (version 20211
-00000020: 3031 3429 2028 6765 6e65 7261 746f 7220  014) (generator 
+00000010: 6220 2876 6572 7369 6f6e 2032 3032 3230  b (version 20220
+00000020: 3931 3429 2028 6765 6e65 7261 746f 7220  914) (generator 
 00000030: 6b69 6361 645f 7379 6d62 6f6c 5f65 6469  kicad_symbol_edi
 00000040: 746f 7229 0a20 2028 7379 6d62 6f6c 2022  tor).  (symbol "
 00000050: 4950 4e22 2028 7069 6e5f 6e75 6d62 6572  IPN" (pin_number
 00000060: 7320 6869 6465 2920 2870 696e 5f6e 616d  s hide) (pin_nam
 00000070: 6573 2028 6f66 6673 6574 2030 2920 6869  es (offset 0) hi
 00000080: 6465 2920 2869 6e5f 626f 6d20 7965 7329  de) (in_bom yes)
 00000090: 2028 6f6e 5f62 6f61 7264 2079 6573 290a   (on_board yes).
 000000a0: 2020 2020 2870 726f 7065 7274 7920 2252      (property "R
-000000b0: 6566 6572 656e 6365 2220 2251 2220 2869  eference" "Q" (i
-000000c0: 6420 3029 2028 6174 2030 2034 2e33 3138  d 0) (at 0 4.318
-000000d0: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-000000e0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000000f0: 2e32 3720 312e 3237 2929 290a 2020 2020  .27 1.27))).    
-00000100: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
-00000110: 2256 616c 7565 2220 2249 504e 2220 2869  "Value" "IPN" (i
-00000120: 6420 3129 2028 6174 2030 202d 3130 2e31  d 1) (at 0 -10.1
-00000130: 3620 3029 0a20 2020 2020 2028 6566 6665  6 0).      (effe
-00000140: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-00000150: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-00000160: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-00000170: 7065 7274 7920 2246 6f6f 7470 7269 6e74  perty "Footprint
-00000180: 2220 2246 6f6f 7470 7269 6e74 2220 2869  " "Footprint" (i
-00000190: 6420 3229 2028 6174 2030 202d 3137 2e37  d 2) (at 0 -17.7
-000001a0: 3820 3029 0a20 2020 2020 2028 6566 6665  8 0).      (effe
-000001b0: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
-000001c0: 312e 3237 2031 2e32 3729 2920 6869 6465  1.27 1.27)) hide
-000001d0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000001e0: 7065 7274 7920 2244 6174 6173 6865 6574  perty "Datasheet
-000001f0: 2220 2269 6e76 656e 7472 6565 5f75 726c  " "inventree_url
-00000200: 2220 2869 6420 3329 2028 6174 2030 202d  " (id 3) (at 0 -
-00000210: 3230 2e33 3220 3029 0a20 2020 2020 2028  20.32 0).      (
-00000220: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00000230: 697a 6520 312e 3237 2031 2e32 3729 2920  ize 1.27 1.27)) 
-00000240: 6869 6465 290a 2020 2020 290a 2020 2020  hide).    ).    
-00000250: 2870 726f 7065 7274 7920 224d 616e 7566  (property "Manuf
-00000260: 6163 7475 7265 7222 2022 4d61 6e75 6661  acturer" "Manufa
-00000270: 6374 7572 6572 2220 2869 6420 3429 2028  cturer" (id 4) (
-00000280: 6174 2030 202d 3132 2e37 2030 290a 2020  at 0 -12.7 0).  
-00000290: 2020 2020 2865 6666 6563 7473 2028 666f      (effects (fo
-000002a0: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
-000002b0: 3237 2929 2068 6964 6529 0a20 2020 2029  27)) hide).    )
-000002c0: 0a20 2020 2028 7072 6f70 6572 7479 2022  .    (property "
-000002d0: 4d61 6e75 6661 6374 7572 6572 2050 6172  Manufacturer Par
-000002e0: 7420 4e75 6d62 6572 2220 224d 504e 2220  t Number" "MPN" 
-000002f0: 2869 6420 3529 2028 6174 2030 202d 3135  (id 5) (at 0 -15
-00000300: 2e32 3420 3029 0a20 2020 2020 2028 6566  .24 0).      (ef
-00000310: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000320: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000330: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
-00000340: 726f 7065 7274 7920 2250 6172 7420 4e75  roperty "Part Nu
-00000350: 6d62 6572 2220 2256 616c 7565 2220 2869  mber" "Value" (i
-00000360: 6420 3629 2028 6174 2037 2e36 3220 332e  d 6) (at 7.62 3.
-00000370: 3831 2030 290a 2020 2020 2020 2865 6666  81 0).      (eff
-00000380: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
-00000390: 2031 2e32 3720 312e 3237 2929 2028 6a75   1.27 1.27)) (ju
-000003a0: 7374 6966 7920 6c65 6674 2929 0a20 2020  stify left)).   
-000003b0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
-000003c0: 2022 5261 7465 6420 566f 6c74 6167 6520   "Rated Voltage 
-000003d0: 2856 6f6c 7429 2220 2252 6174 6564 2056  (Volt)" "Rated V
-000003e0: 6f6c 7461 6765 2220 2869 6420 3729 2028  oltage" (id 7) (
-000003f0: 6174 2037 2e36 3220 312e 3237 2030 290a  at 7.62 1.27 0).
-00000400: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
-00000410: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00000420: 312e 3237 2929 2028 6a75 7374 6966 7920  1.27)) (justify 
-00000430: 6c65 6674 2929 0a20 2020 2029 0a20 2020  left)).    ).   
-00000440: 2028 7072 6f70 6572 7479 2022 5261 7465   (property "Rate
-00000450: 6420 4375 7272 656e 7420 2841 6d70 7329  d Current (Amps)
-00000460: 2220 2252 6174 6564 2043 7572 7265 6e74  " "Rated Current
-00000470: 2220 2869 6420 3829 2028 6174 2037 2e36  " (id 8) (at 7.6
-00000480: 3220 2d31 2e32 3720 3029 0a20 2020 2020  2 -1.27 0).     
-00000490: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
-000004a0: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
-000004b0: 2920 286a 7573 7469 6679 206c 6566 7429  ) (justify left)
-000004c0: 290a 2020 2020 290a 2020 2020 2870 726f  ).    ).    (pro
-000004d0: 7065 7274 7920 2250 6163 6b61 6765 2054  perty "Package T
-000004e0: 7970 6522 2022 5061 636b 6167 6520 5479  ype" "Package Ty
-000004f0: 7065 2220 2869 6420 3929 2028 6174 2037  pe" (id 9) (at 7
-00000500: 2e36 3220 2d33 2e38 3120 3029 0a20 2020  .62 -3.81 0).   
-00000510: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
-00000520: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
-00000530: 3729 2920 286a 7573 7469 6679 206c 6566  7)) (justify lef
-00000540: 7429 290a 2020 2020 290a 2020 2020 2870  t)).    ).    (p
-00000550: 726f 7065 7274 7920 226b 695f 6b65 7977  roperty "ki_keyw
-00000560: 6f72 6473 2220 226b 6579 776f 7264 7322  ords" "keywords"
-00000570: 2028 6964 2031 3029 2028 6174 2030 2030   (id 10) (at 0 0
-00000580: 2030 290a 2020 2020 2020 2865 6666 6563   0).      (effec
-00000590: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
-000005a0: 2e32 3720 312e 3237 2929 2068 6964 6529  .27 1.27)) hide)
-000005b0: 0a20 2020 2029 0a20 2020 2028 7072 6f70  .    ).    (prop
-000005c0: 6572 7479 2022 6b69 5f64 6573 6372 6970  erty "ki_descrip
-000005d0: 7469 6f6e 2220 2264 6573 6372 6970 7469  tion" "descripti
-000005e0: 6f6e 2220 2869 6420 3131 2920 2861 7420  on" (id 11) (at 
-000005f0: 3020 3020 3029 0a20 2020 2020 2028 6566  0 0 0).      (ef
-00000600: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
-00000610: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
-00000620: 6465 290a 2020 2020 290a 2020 2020 2873  de).    ).    (s
-00000630: 796d 626f 6c20 2249 504e 5f30 5f31 220a  ymbol "IPN_0_1".
-00000640: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
-00000650: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
-00000660: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
-00000670: 3029 0a20 2020 2020 2020 2020 2028 7879  0).          (xy
-00000680: 2031 2e32 3720 2d32 2e35 3429 0a20 2020   1.27 -2.54).   
-00000690: 2020 2020 2029 0a20 2020 2020 2020 2028       ).        (
-000006a0: 7374 726f 6b65 2028 7769 6474 6820 3029  stroke (width 0)
-000006b0: 2028 7479 7065 2064 6566 6175 6c74 2920   (type default) 
-000006c0: 2863 6f6c 6f72 2030 2030 2030 2030 2929  (color 0 0 0 0))
-000006d0: 0a20 2020 2020 2020 2028 6669 6c6c 2028  .        (fill (
-000006e0: 7479 7065 206e 6f6e 6529 290a 2020 2020  type none)).    
-000006f0: 2020 290a 2020 2020 2020 2870 6f6c 796c    ).      (polyl
-00000700: 696e 650a 2020 2020 2020 2020 2870 7473  ine.        (pts
-00000710: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
-00000720: 2e32 3720 3029 0a20 2020 2020 2020 2020  .27 0).         
-00000730: 2028 7879 2031 2e32 3720 322e 3534 290a   (xy 1.27 2.54).
-00000740: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000750: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000760: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
-00000770: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-00000780: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
-00000790: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
-000007a0: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
-000007b0: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
-000007c0: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-000007d0: 7920 312e 3737 3820 2d31 2e39 3035 290a  y 1.778 -1.905).
-000007e0: 2020 2020 2020 2020 2020 2878 7920 332e            (xy 3.
-000007f0: 3831 202d 312e 3930 3529 0a20 2020 2020  81 -1.905).     
-00000800: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
-00000810: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
-00000820: 7479 7065 2064 6566 6175 6c74 2920 2863  type default) (c
-00000830: 6f6c 6f72 2030 2030 2030 2030 2929 0a20  olor 0 0 0 0)). 
-00000840: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
-00000850: 7065 206e 6f6e 6529 290a 2020 2020 2020  pe none)).      
-00000860: 290a 2020 2020 2020 2870 6f6c 796c 696e  ).      (polylin
-00000870: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
-00000880: 2020 2020 2020 2020 2028 7879 2031 2e37           (xy 1.7
-00000890: 3738 202d 312e 3237 290a 2020 2020 2020  78 -1.27).      
-000008a0: 2020 2020 2878 7920 312e 3737 3820 2d32      (xy 1.778 -2
-000008b0: 2e35 3429 0a20 2020 2020 2020 2029 0a20  .54).        ). 
-000008c0: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-000008d0: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
-000008e0: 6566 6175 6c74 2920 2863 6f6c 6f72 2030  efault) (color 0
-000008f0: 2030 2030 2030 2929 0a20 2020 2020 2020   0 0 0)).       
-00000900: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
-00000910: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
-00000920: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
-00000930: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
-00000940: 2020 2028 7879 2031 2e37 3738 202d 302e     (xy 1.778 -0.
-00000950: 3633 3529 0a20 2020 2020 2020 2020 2028  635).          (
-00000960: 7879 2031 2e37 3738 2030 2e36 3335 290a  xy 1.778 0.635).
-00000970: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000980: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
-00000990: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
-000009a0: 7429 2028 636f 6c6f 7220 3020 3020 3020  t) (color 0 0 0 
-000009b0: 3029 290a 2020 2020 2020 2020 2866 696c  0)).        (fil
+000000b0: 6566 6572 656e 6365 2220 2251 2220 2861  eference" "Q" (a
+000000c0: 7420 3020 342e 3331 3820 3029 0a20 2020  t 0 4.318 0).   
+000000d0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000000e0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000000f0: 3729 2929 0a20 2020 2029 0a20 2020 2028  7))).    ).    (
+00000100: 7072 6f70 6572 7479 2022 5661 6c75 6522  property "Value"
+00000110: 2022 4950 4e22 2028 6174 2030 202d 3130   "IPN" (at 0 -10
+00000120: 2e31 3620 3029 0a20 2020 2020 2028 6566  .16 0).      (ef
+00000130: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+00000140: 6520 312e 3237 2031 2e32 3729 2920 6869  e 1.27 1.27)) hi
+00000150: 6465 290a 2020 2020 290a 2020 2020 2870  de).    ).    (p
+00000160: 726f 7065 7274 7920 2246 6f6f 7470 7269  roperty "Footpri
+00000170: 6e74 2220 2246 6f6f 7470 7269 6e74 2220  nt" "Footprint" 
+00000180: 2861 7420 3020 2d31 372e 3738 2030 290a  (at 0 -17.78 0).
+00000190: 2020 2020 2020 2865 6666 6563 7473 2028        (effects (
+000001a0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
+000001b0: 312e 3237 2929 2068 6964 6529 0a20 2020  1.27)) hide).   
+000001c0: 2029 0a20 2020 2028 7072 6f70 6572 7479   ).    (property
+000001d0: 2022 4461 7461 7368 6565 7422 2022 696e   "Datasheet" "in
+000001e0: 7665 6e74 7265 655f 7572 6c22 2028 6174  ventree_url" (at
+000001f0: 2030 202d 3230 2e33 3220 3029 0a20 2020   0 -20.32 0).   
+00000200: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+00000210: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000220: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000230: 2020 2020 2870 726f 7065 7274 7920 224d      (property "M
+00000240: 616e 7566 6163 7475 7265 7222 2022 4d61  anufacturer" "Ma
+00000250: 6e75 6661 6374 7572 6572 2220 2861 7420  nufacturer" (at 
+00000260: 3020 2d31 322e 3720 3029 0a20 2020 2020  0 -12.7 0).     
+00000270: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00000280: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00000290: 2920 6869 6465 290a 2020 2020 290a 2020  ) hide).    ).  
+000002a0: 2020 2870 726f 7065 7274 7920 224d 616e    (property "Man
+000002b0: 7566 6163 7475 7265 7220 5061 7274 204e  ufacturer Part N
+000002c0: 756d 6265 7222 2022 4d50 4e22 2028 6174  umber" "MPN" (at
+000002d0: 2030 202d 3135 2e32 3420 3029 0a20 2020   0 -15.24 0).   
+000002e0: 2020 2028 6566 6665 6374 7320 2866 6f6e     (effects (fon
+000002f0: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+00000300: 3729 2920 6869 6465 290a 2020 2020 290a  7)) hide).    ).
+00000310: 2020 2020 2870 726f 7065 7274 7920 2250      (property "P
+00000320: 6172 7420 4e75 6d62 6572 2220 2256 616c  art Number" "Val
+00000330: 7565 2220 2861 7420 372e 3632 2033 2e38  ue" (at 7.62 3.8
+00000340: 3120 3029 0a20 2020 2020 2028 6566 6665  1 0).      (effe
+00000350: 6374 7320 2866 6f6e 7420 2873 697a 6520  cts (font (size 
+00000360: 312e 3237 2031 2e32 3729 2920 286a 7573  1.27 1.27)) (jus
+00000370: 7469 6679 206c 6566 7429 290a 2020 2020  tify left)).    
+00000380: 290a 2020 2020 2870 726f 7065 7274 7920  ).    (property 
+00000390: 2252 6174 6564 2056 6f6c 7461 6765 2028  "Rated Voltage (
+000003a0: 566f 6c74 2922 2022 5261 7465 6420 566f  Volt)" "Rated Vo
+000003b0: 6c74 6167 6522 2028 6174 2037 2e36 3220  ltage" (at 7.62 
+000003c0: 312e 3237 2030 290a 2020 2020 2020 2865  1.27 0).      (e
+000003d0: 6666 6563 7473 2028 666f 6e74 2028 7369  ffects (font (si
+000003e0: 7a65 2031 2e32 3720 312e 3237 2929 2028  ze 1.27 1.27)) (
+000003f0: 6a75 7374 6966 7920 6c65 6674 2929 0a20  justify left)). 
+00000400: 2020 2029 0a20 2020 2028 7072 6f70 6572     ).    (proper
+00000410: 7479 2022 5261 7465 6420 4375 7272 656e  ty "Rated Curren
+00000420: 7420 2841 6d70 7329 2220 2252 6174 6564  t (Amps)" "Rated
+00000430: 2043 7572 7265 6e74 2220 2861 7420 372e   Current" (at 7.
+00000440: 3632 202d 312e 3237 2030 290a 2020 2020  62 -1.27 0).    
+00000450: 2020 2865 6666 6563 7473 2028 666f 6e74    (effects (font
+00000460: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
+00000470: 2929 2028 6a75 7374 6966 7920 6c65 6674  )) (justify left
+00000480: 2929 0a20 2020 2029 0a20 2020 2028 7072  )).    ).    (pr
+00000490: 6f70 6572 7479 2022 5061 636b 6167 6520  operty "Package 
+000004a0: 5479 7065 2220 2250 6163 6b61 6765 2054  Type" "Package T
+000004b0: 7970 6522 2028 6174 2037 2e36 3220 2d33  ype" (at 7.62 -3
+000004c0: 2e38 3120 3029 0a20 2020 2020 2028 6566  .81 0).      (ef
+000004d0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000004e0: 6520 312e 3237 2031 2e32 3729 2920 286a  e 1.27 1.27)) (j
+000004f0: 7573 7469 6679 206c 6566 7429 290a 2020  ustify left)).  
+00000500: 2020 290a 2020 2020 2870 726f 7065 7274    ).    (propert
+00000510: 7920 226b 695f 6b65 7977 6f72 6473 2220  y "ki_keywords" 
+00000520: 226b 6579 776f 7264 7322 2028 6174 2030  "keywords" (at 0
+00000530: 2030 2030 290a 2020 2020 2020 2865 6666   0 0).      (eff
+00000540: 6563 7473 2028 666f 6e74 2028 7369 7a65  ects (font (size
+00000550: 2031 2e32 3720 312e 3237 2929 2068 6964   1.27 1.27)) hid
+00000560: 6529 0a20 2020 2029 0a20 2020 2028 7072  e).    ).    (pr
+00000570: 6f70 6572 7479 2022 6b69 5f64 6573 6372  operty "ki_descr
+00000580: 6970 7469 6f6e 2220 2264 6573 6372 6970  iption" "descrip
+00000590: 7469 6f6e 2220 2861 7420 3020 3020 3029  tion" (at 0 0 0)
+000005a0: 0a20 2020 2020 2028 6566 6665 6374 7320  .      (effects 
+000005b0: 2866 6f6e 7420 2873 697a 6520 312e 3237  (font (size 1.27
+000005c0: 2031 2e32 3729 2920 6869 6465 290a 2020   1.27)) hide).  
+000005d0: 2020 290a 2020 2020 2873 796d 626f 6c20    ).    (symbol 
+000005e0: 2249 504e 5f30 5f31 220a 2020 2020 2020  "IPN_0_1".      
+000005f0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
+00000600: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
+00000610: 2028 7879 2031 2e32 3720 3029 0a20 2020   (xy 1.27 0).   
+00000620: 2020 2020 2020 2028 7879 2031 2e32 3720         (xy 1.27 
+00000630: 2d32 2e35 3429 0a20 2020 2020 2020 2029  -2.54).        )
+00000640: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000650: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000660: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000670: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000680: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000690: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
+000006a0: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
+000006b0: 2020 2020 2028 7879 2031 2e32 3720 3029       (xy 1.27 0)
+000006c0: 0a20 2020 2020 2020 2020 2028 7879 2031  .          (xy 1
+000006d0: 2e32 3720 322e 3534 290a 2020 2020 2020  .27 2.54).      
+000006e0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+000006f0: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
+00000700: 7970 6520 6465 6661 756c 7429 290a 2020  ype default)).  
+00000710: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
+00000720: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
+00000730: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
+00000740: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
+00000750: 2020 2020 2020 2020 2878 7920 312e 3737          (xy 1.77
+00000760: 3820 2d31 2e32 3729 0a20 2020 2020 2020  8 -1.27).       
+00000770: 2020 2028 7879 2031 2e37 3738 202d 322e     (xy 1.778 -2.
+00000780: 3534 290a 2020 2020 2020 2020 290a 2020  54).        ).  
+00000790: 2020 2020 2020 2873 7472 6f6b 6520 2877        (stroke (w
+000007a0: 6964 7468 2030 2920 2874 7970 6520 6465  idth 0) (type de
+000007b0: 6661 756c 7429 290a 2020 2020 2020 2020  fault)).        
+000007c0: 2866 696c 6c20 2874 7970 6520 6e6f 6e65  (fill (type none
+000007d0: 2929 0a20 2020 2020 2029 0a20 2020 2020  )).      ).     
+000007e0: 2028 706f 6c79 6c69 6e65 0a20 2020 2020   (polyline.     
+000007f0: 2020 2028 7074 730a 2020 2020 2020 2020     (pts.        
+00000800: 2020 2878 7920 312e 3737 3820 2d30 2e36    (xy 1.778 -0.6
+00000810: 3335 290a 2020 2020 2020 2020 2020 2878  35).          (x
+00000820: 7920 312e 3737 3820 302e 3633 3529 0a20  y 1.778 0.635). 
+00000830: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000840: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
+00000850: 3029 2028 7479 7065 2064 6566 6175 6c74  0) (type default
+00000860: 2929 0a20 2020 2020 2020 2028 6669 6c6c  )).        (fill
+00000870: 2028 7479 7065 206e 6f6e 6529 290a 2020   (type none)).  
+00000880: 2020 2020 290a 2020 2020 2020 2870 6f6c      ).      (pol
+00000890: 796c 696e 650a 2020 2020 2020 2020 2870  yline.        (p
+000008a0: 7473 0a20 2020 2020 2020 2020 2028 7879  ts.          (xy
+000008b0: 2031 2e37 3738 2031 2e32 3729 0a20 2020   1.778 1.27).   
+000008c0: 2020 2020 2020 2028 7879 2031 2e37 3738         (xy 1.778
+000008d0: 2032 2e35 3429 0a20 2020 2020 2020 2029   2.54).        )
+000008e0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+000008f0: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000900: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000910: 2020 2028 6669 6c6c 2028 7479 7065 206e     (fill (type n
+00000920: 6f6e 6529 290a 2020 2020 2020 290a 2020  one)).      ).  
+00000930: 2020 2020 2870 6f6c 796c 696e 650a 2020      (polyline.  
+00000940: 2020 2020 2020 2870 7473 0a20 2020 2020        (pts.     
+00000950: 2020 2020 2028 7879 2033 2e38 3120 2d32       (xy 3.81 -2
+00000960: 2e35 3429 0a20 2020 2020 2020 2020 2028  .54).          (
+00000970: 7879 2033 2e38 3120 2d31 2e39 3035 290a  xy 3.81 -1.905).
+00000980: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000990: 2020 2873 7472 6f6b 6520 2877 6964 7468    (stroke (width
+000009a0: 2030 2920 2874 7970 6520 6465 6661 756c   0) (type defaul
+000009b0: 7429 290a 2020 2020 2020 2020 2866 696c  t)).        (fil
 000009c0: 6c20 2874 7970 6520 6e6f 6e65 2929 0a20  l (type none)). 
 000009d0: 2020 2020 2029 0a20 2020 2020 2028 706f       ).      (po
 000009e0: 6c79 6c69 6e65 0a20 2020 2020 2020 2028  lyline.        (
 000009f0: 7074 730a 2020 2020 2020 2020 2020 2878  pts.          (x
-00000a00: 7920 312e 3737 3820 3029 0a20 2020 2020  y 1.778 0).     
-00000a10: 2020 2020 2028 7879 2032 2e36 3637 2030       (xy 2.667 0
-00000a20: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00000a30: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
-00000a40: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
-00000a50: 756c 7429 2028 636f 6c6f 7220 3020 3020  ult) (color 0 0 
-00000a60: 3020 3029 290a 2020 2020 2020 2020 2866  0 0)).        (f
-00000a70: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
-00000a80: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
-00000a90: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
-00000aa0: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
-00000ab0: 2878 7920 312e 3737 3820 312e 3237 290a  (xy 1.778 1.27).
-00000ac0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-00000ad0: 3737 3820 322e 3534 290a 2020 2020 2020  778 2.54).      
-00000ae0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
-00000af0: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
-00000b00: 7970 6520 6465 6661 756c 7429 2028 636f  ype default) (co
-00000b10: 6c6f 7220 3020 3020 3020 3029 290a 2020  lor 0 0 0 0)).  
-00000b20: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
-00000b30: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
-00000b40: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-00000b50: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-00000b60: 2020 2020 2020 2020 2878 7920 332e 3831          (xy 3.81
-00000b70: 202d 322e 3534 290a 2020 2020 2020 2020   -2.54).        
-00000b80: 2020 2878 7920 332e 3831 202d 312e 3930    (xy 3.81 -1.90
-00000b90: 3529 0a20 2020 2020 2020 2029 0a20 2020  5).        ).   
-00000ba0: 2020 2020 2028 7374 726f 6b65 2028 7769       (stroke (wi
-00000bb0: 6474 6820 3029 2028 7479 7065 2064 6566  dth 0) (type def
-00000bc0: 6175 6c74 2920 2863 6f6c 6f72 2030 2030  ault) (color 0 0
-00000bd0: 2030 2030 2929 0a20 2020 2020 2020 2028   0 0)).        (
-00000be0: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
-00000bf0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000c00: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
-00000c10: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
-00000c20: 2028 7879 2034 2e39 3533 202d 302e 3633   (xy 4.953 -0.63
-00000c30: 3529 0a20 2020 2020 2020 2020 2028 7879  5).          (xy
-00000c40: 2036 2e32 3233 202d 302e 3633 3529 0a20   6.223 -0.635). 
-00000c50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000c60: 2028 7374 726f 6b65 2028 7769 6474 6820   (stroke (width 
-00000c70: 302e 3132 3729 2028 7479 7065 2064 6566  0.127) (type def
-00000c80: 6175 6c74 2920 2863 6f6c 6f72 2030 2030  ault) (color 0 0
-00000c90: 2030 2030 2929 0a20 2020 2020 2020 2028   0 0)).        (
-00000ca0: 6669 6c6c 2028 7479 7065 206e 6f6e 6529  fill (type none)
-00000cb0: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00000cc0: 2870 6f6c 796c 696e 650a 2020 2020 2020  (polyline.      
-00000cd0: 2020 2870 7473 0a20 2020 2020 2020 2020    (pts.         
-00000ce0: 2028 7879 2035 2e30 3820 302e 3530 3829   (xy 5.08 0.508)
-00000cf0: 0a20 2020 2020 2020 2020 2028 7879 2034  .          (xy 4
-00000d00: 2e39 3533 2030 2e35 3038 290a 2020 2020  .953 0.508).    
-00000d10: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
-00000d20: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
-00000d30: 2874 7970 6520 6465 6661 756c 7429 2028  (type default) (
-00000d40: 636f 6c6f 7220 3020 3020 3020 3029 290a  color 0 0 0 0)).
-00000d50: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
-00000d60: 7970 6520 6e6f 6e65 2929 0a20 2020 2020  ype none)).     
-00000d70: 2029 0a20 2020 2020 2028 706f 6c79 6c69   ).      (polyli
-00000d80: 6e65 0a20 2020 2020 2020 2028 7074 730a  ne.        (pts.
-00000d90: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
-00000da0: 3737 3820 312e 3930 3529 0a20 2020 2020  778 1.905).     
-00000db0: 2020 2020 2028 7879 2033 2e38 3120 312e       (xy 3.81 1.
-00000dc0: 3930 3529 0a20 2020 2020 2020 2020 2028  905).          (
-00000dd0: 7879 2033 2e38 3120 322e 3534 290a 2020  xy 3.81 2.54).  
-00000de0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000df0: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-00000e00: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
-00000e10: 2028 636f 6c6f 7220 3020 3020 3020 3029   (color 0 0 0 0)
-00000e20: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
-00000e30: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
-00000e40: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
-00000e50: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
-00000e60: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
-00000e70: 332e 3638 3320 3029 0a20 2020 2020 2020  3.683 0).       
-00000e80: 2020 2028 7879 2033 2e38 3120 3029 0a20     (xy 3.81 0). 
-00000e90: 2020 2020 2020 2020 2028 7879 2033 2e38           (xy 3.8
-00000ea0: 3120 2d31 2e39 3035 290a 2020 2020 2020  1 -1.905).      
-00000eb0: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
-00000ec0: 6f6b 6520 2877 6964 7468 2030 2920 2874  oke (width 0) (t
-00000ed0: 7970 6520 6465 6661 756c 7429 2028 636f  ype default) (co
-00000ee0: 6c6f 7220 3020 3020 3020 3029 290a 2020  lor 0 0 0 0)).  
-00000ef0: 2020 2020 2020 2866 696c 6c20 2874 7970        (fill (typ
-00000f00: 6520 6e6f 6e65 2929 0a20 2020 2020 2029  e none)).      )
-00000f10: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
-00000f20: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
-00000f30: 2020 2020 2020 2020 2878 7920 352e 3538          (xy 5.58
-00000f40: 3820 2d30 2e36 3335 290a 2020 2020 2020  8 -0.635).      
-00000f50: 2020 2020 2878 7920 352e 3538 3820 2d32      (xy 5.588 -2
-00000f60: 2e34 3133 290a 2020 2020 2020 2020 2020  .413).          
-00000f70: 2878 7920 332e 3831 202d 322e 3431 3329  (xy 3.81 -2.413)
-00000f80: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00000f90: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-00000fa0: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-00000fb0: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00000fc0: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00000fd0: 6c6c 2028 7479 7065 206e 6f6e 6529 290a  ll (type none)).
-00000fe0: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-00000ff0: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-00001000: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-00001010: 7879 2035 2e35 3838 2030 2e35 3038 290a  xy 5.588 0.508).
-00001020: 2020 2020 2020 2020 2020 2878 7920 352e            (xy 5.
-00001030: 3538 3820 322e 3238 3629 0a20 2020 2020  588 2.286).     
-00001040: 2020 2020 2028 7879 2033 2e38 3120 322e       (xy 3.81 2.
-00001050: 3238 3629 0a20 2020 2020 2020 2029 0a20  286).        ). 
-00001060: 2020 2020 2020 2028 7374 726f 6b65 2028         (stroke (
-00001070: 7769 6474 6820 3029 2028 7479 7065 2064  width 0) (type d
-00001080: 6566 6175 6c74 2920 2863 6f6c 6f72 2030  efault) (color 0
-00001090: 2030 2030 2030 2929 0a20 2020 2020 2020   0 0 0)).       
-000010a0: 2028 6669 6c6c 2028 7479 7065 206e 6f6e   (fill (type non
-000010b0: 6529 290a 2020 2020 2020 290a 2020 2020  e)).      ).    
-000010c0: 2020 2870 6f6c 796c 696e 650a 2020 2020    (polyline.    
-000010d0: 2020 2020 2870 7473 0a20 2020 2020 2020      (pts.       
-000010e0: 2020 2028 7879 2033 2e36 3833 2030 290a     (xy 3.683 0).
-000010f0: 2020 2020 2020 2020 2020 2878 7920 322e            (xy 2.
-00001100: 3636 3720 302e 3736 3229 0a20 2020 2020  667 0.762).     
-00001110: 2020 2020 2028 7879 2032 2e36 3637 202d       (xy 2.667 -
-00001120: 302e 3736 3229 0a20 2020 2020 2020 2020  0.762).         
-00001130: 2028 7879 2033 2e36 3833 2030 290a 2020   (xy 3.683 0).  
-00001140: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00001150: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
-00001160: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
-00001170: 2028 636f 6c6f 7220 3020 3020 3020 3029   (color 0 0 0 0)
-00001180: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
-00001190: 2874 7970 6520 6f75 746c 696e 6529 290a  (type outline)).
-000011a0: 2020 2020 2020 290a 2020 2020 2020 2870        ).      (p
-000011b0: 6f6c 796c 696e 650a 2020 2020 2020 2020  olyline.        
-000011c0: 2870 7473 0a20 2020 2020 2020 2020 2028  (pts.          (
-000011d0: 7879 2034 2e39 3533 2030 2e35 3038 290a  xy 4.953 0.508).
-000011e0: 2020 2020 2020 2020 2020 2878 7920 352e            (xy 5.
-000011f0: 3538 3820 2d30 2e36 3335 290a 2020 2020  588 -0.635).    
-00001200: 2020 2020 2020 2878 7920 362e 3232 3320        (xy 6.223 
-00001210: 302e 3530 3829 0a20 2020 2020 2020 2020  0.508).         
-00001220: 2028 7879 2035 2e30 3820 302e 3530 3829   (xy 5.08 0.508)
-00001230: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00001240: 2020 2028 7374 726f 6b65 2028 7769 6474     (stroke (widt
-00001250: 6820 3029 2028 7479 7065 2064 6566 6175  h 0) (type defau
-00001260: 6c74 2920 2863 6f6c 6f72 2030 2030 2030  lt) (color 0 0 0
-00001270: 2030 2929 0a20 2020 2020 2020 2028 6669   0)).        (fi
-00001280: 6c6c 2028 7479 7065 206f 7574 6c69 6e65  ll (type outline
-00001290: 2929 0a20 2020 2020 2029 0a20 2020 2029  )).      ).    )
-000012a0: 0a20 2020 2028 7379 6d62 6f6c 2022 4950  .    (symbol "IP
-000012b0: 4e5f 315f 3122 0a20 2020 2020 2028 7069  N_1_1".      (pi
-000012c0: 6e20 6269 6469 7265 6374 696f 6e61 6c20  n bidirectional 
-000012d0: 6c69 6e65 2028 6174 2033 2e38 3120 372e  line (at 3.81 7.
-000012e0: 3632 2032 3730 2920 286c 656e 6774 6820  62 270) (length 
-000012f0: 352e 3038 290a 2020 2020 2020 2020 286e  5.08).        (n
-00001300: 616d 6520 2244 2220 2865 6666 6563 7473  ame "D" (effects
-00001310: 2028 666f 6e74 2028 7369 7a65 2031 2e32   (font (size 1.2
-00001320: 3720 312e 3237 2929 2929 0a20 2020 2020  7 1.27)))).     
-00001330: 2020 2028 6e75 6d62 6572 2022 7e22 2028     (number "~" (
-00001340: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-00001350: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-00001360: 290a 2020 2020 2020 290a 2020 2020 2020  ).      ).      
-00001370: 2870 696e 2069 6e70 7574 206c 696e 6520  (pin input line 
-00001380: 2861 7420 2d33 2e38 3120 3020 3029 2028  (at -3.81 0 0) (
-00001390: 6c65 6e67 7468 2035 2e30 3829 0a20 2020  length 5.08).   
-000013a0: 2020 2020 2028 6e61 6d65 2022 4722 2028       (name "G" (
-000013b0: 6566 6665 6374 7320 2866 6f6e 7420 2873  effects (font (s
-000013c0: 697a 6520 312e 3237 2031 2e32 3729 2929  ize 1.27 1.27)))
-000013d0: 290a 2020 2020 2020 2020 286e 756d 6265  ).        (numbe
-000013e0: 7220 227e 2220 2865 6666 6563 7473 2028  r "~" (effects (
-000013f0: 666f 6e74 2028 7369 7a65 2031 2e32 3720  font (size 1.27 
-00001400: 312e 3237 2929 2929 0a20 2020 2020 2029  1.27)))).      )
-00001410: 0a20 2020 2020 2028 7069 6e20 6269 6469  .      (pin bidi
-00001420: 7265 6374 696f 6e61 6c20 6c69 6e65 2028  rectional line (
-00001430: 6174 2033 2e38 3120 2d37 2e36 3220 3930  at 3.81 -7.62 90
-00001440: 2920 286c 656e 6774 6820 352e 3038 290a  ) (length 5.08).
-00001450: 2020 2020 2020 2020 286e 616d 6520 2253          (name "S
-00001460: 2220 2865 6666 6563 7473 2028 666f 6e74  " (effects (font
-00001470: 2028 7369 7a65 2031 2e32 3720 312e 3237   (size 1.27 1.27
-00001480: 2929 2929 0a20 2020 2020 2020 2028 6e75  )))).        (nu
-00001490: 6d62 6572 2022 7e22 2028 6566 6665 6374  mber "~" (effect
-000014a0: 7320 2866 6f6e 7420 2873 697a 6520 312e  s (font (size 1.
-000014b0: 3237 2031 2e32 3729 2929 290a 2020 2020  27 1.27)))).    
-000014c0: 2020 290a 2020 2020 290a 2020 290a 290a    ).    ).  ).).
+00000a00: 7920 342e 3935 3320 302e 3530 3829 0a20  y 4.953 0.508). 
+00000a10: 2020 2020 2020 2020 2028 7879 2036 2e32           (xy 6.2
+00000a20: 3233 2030 2e35 3038 290a 2020 2020 2020  23 0.508).      
+00000a30: 2020 290a 2020 2020 2020 2020 2873 7472    ).        (str
+00000a40: 6f6b 6520 2877 6964 7468 2030 2e31 3237  oke (width 0.127
+00000a50: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+00000a60: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+00000a70: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+00000a80: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+00000a90: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000aa0: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000ab0: 352e 3038 202d 302e 3633 3529 0a20 2020  5.08 -0.635).   
+00000ac0: 2020 2020 2020 2028 7879 2034 2e39 3533         (xy 4.953
+00000ad0: 202d 302e 3633 3529 0a20 2020 2020 2020   -0.635).       
+00000ae0: 2029 0a20 2020 2020 2020 2028 7374 726f   ).        (stro
+00000af0: 6b65 2028 7769 6474 6820 3029 2028 7479  ke (width 0) (ty
+00000b00: 7065 2064 6566 6175 6c74 2929 0a20 2020  pe default)).   
+00000b10: 2020 2020 2028 6669 6c6c 2028 7479 7065       (fill (type
+00000b20: 206e 6f6e 6529 290a 2020 2020 2020 290a   none)).      ).
+00000b30: 2020 2020 2020 2870 6f6c 796c 696e 650a        (polyline.
+00000b40: 2020 2020 2020 2020 2870 7473 0a20 2020          (pts.   
+00000b50: 2020 2020 2020 2028 7879 2031 2e37 3738         (xy 1.778
+00000b60: 2031 2e39 3035 290a 2020 2020 2020 2020   1.905).        
+00000b70: 2020 2878 7920 332e 3831 2031 2e39 3035    (xy 3.81 1.905
+00000b80: 290a 2020 2020 2020 2020 2020 2878 7920  ).          (xy 
+00000b90: 332e 3831 2032 2e35 3429 0a20 2020 2020  3.81 2.54).     
+00000ba0: 2020 2029 0a20 2020 2020 2020 2028 7374     ).        (st
+00000bb0: 726f 6b65 2028 7769 6474 6820 3029 2028  roke (width 0) (
+00000bc0: 7479 7065 2064 6566 6175 6c74 2929 0a20  type default)). 
+00000bd0: 2020 2020 2020 2028 6669 6c6c 2028 7479         (fill (ty
+00000be0: 7065 206e 6f6e 6529 290a 2020 2020 2020  pe none)).      
+00000bf0: 290a 2020 2020 2020 2870 6f6c 796c 696e  ).      (polylin
+00000c00: 650a 2020 2020 2020 2020 2870 7473 0a20  e.        (pts. 
+00000c10: 2020 2020 2020 2020 2028 7879 2035 2e35           (xy 5.5
+00000c20: 3838 202d 302e 3633 3529 0a20 2020 2020  88 -0.635).     
+00000c30: 2020 2020 2028 7879 2035 2e35 3838 202d       (xy 5.588 -
+00000c40: 322e 3431 3329 0a20 2020 2020 2020 2020  2.413).         
+00000c50: 2028 7879 2033 2e38 3120 2d32 2e34 3133   (xy 3.81 -2.413
+00000c60: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00000c70: 2020 2020 2873 7472 6f6b 6520 2877 6964      (stroke (wid
+00000c80: 7468 2030 2920 2874 7970 6520 6465 6661  th 0) (type defa
+00000c90: 756c 7429 290a 2020 2020 2020 2020 2866  ult)).        (f
+00000ca0: 696c 6c20 2874 7970 6520 6e6f 6e65 2929  ill (type none))
+00000cb0: 0a20 2020 2020 2029 0a20 2020 2020 2028  .      ).      (
+00000cc0: 706f 6c79 6c69 6e65 0a20 2020 2020 2020  polyline.       
+00000cd0: 2028 7074 730a 2020 2020 2020 2020 2020   (pts.          
+00000ce0: 2878 7920 352e 3538 3820 302e 3633 3529  (xy 5.588 0.635)
+00000cf0: 0a20 2020 2020 2020 2020 2028 7879 2035  .          (xy 5
+00000d00: 2e35 3838 2032 2e32 3836 290a 2020 2020  .588 2.286).    
+00000d10: 2020 2020 2020 2878 7920 332e 3831 2032        (xy 3.81 2
+00000d20: 2e32 3836 290a 2020 2020 2020 2020 290a  .286).        ).
+00000d30: 2020 2020 2020 2020 2873 7472 6f6b 6520          (stroke 
+00000d40: 2877 6964 7468 2030 2920 2874 7970 6520  (width 0) (type 
+00000d50: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00000d60: 2020 2866 696c 6c20 2874 7970 6520 6e6f    (fill (type no
+00000d70: 6e65 2929 0a20 2020 2020 2029 0a20 2020  ne)).      ).   
+00000d80: 2020 2028 706f 6c79 6c69 6e65 0a20 2020     (polyline.   
+00000d90: 2020 2020 2028 7074 730a 2020 2020 2020       (pts.      
+00000da0: 2020 2020 2878 7920 312e 3737 3820 2d31      (xy 1.778 -1
+00000db0: 2e39 3035 290a 2020 2020 2020 2020 2020  .905).          
+00000dc0: 2878 7920 332e 3831 202d 312e 3930 3529  (xy 3.81 -1.905)
+00000dd0: 0a20 2020 2020 2020 2020 2028 7879 2033  .          (xy 3
+00000de0: 2e38 3120 3029 0a20 2020 2020 2020 2020  .81 0).         
+00000df0: 2028 7879 2033 2e30 3438 2030 290a 2020   (xy 3.048 0).  
+00000e00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000e10: 2873 7472 6f6b 6520 2877 6964 7468 2030  (stroke (width 0
+00000e20: 2920 2874 7970 6520 6465 6661 756c 7429  ) (type default)
+00000e30: 290a 2020 2020 2020 2020 2866 696c 6c20  ).        (fill 
+00000e40: 2874 7970 6520 6e6f 6e65 2929 0a20 2020  (type none)).   
+00000e50: 2020 2029 0a20 2020 2020 2028 706f 6c79     ).      (poly
+00000e60: 6c69 6e65 0a20 2020 2020 2020 2028 7074  line.        (pt
+00000e70: 730a 2020 2020 2020 2020 2020 2878 7920  s.          (xy 
+00000e80: 312e 3930 3520 3029 0a20 2020 2020 2020  1.905 0).       
+00000e90: 2020 2028 7879 2033 2e30 3438 2030 2e36     (xy 3.048 0.6
+00000ea0: 3335 290a 2020 2020 2020 2020 2020 2878  35).          (x
+00000eb0: 7920 332e 3034 3820 2d30 2e36 3335 290a  y 3.048 -0.635).
+00000ec0: 2020 2020 2020 2020 2020 2878 7920 312e            (xy 1.
+00000ed0: 3930 3520 3029 0a20 2020 2020 2020 2029  905 0).        )
+00000ee0: 0a20 2020 2020 2020 2028 7374 726f 6b65  .        (stroke
+00000ef0: 2028 7769 6474 6820 3029 2028 7479 7065   (width 0) (type
+00000f00: 2064 6566 6175 6c74 2929 0a20 2020 2020   default)).     
+00000f10: 2020 2028 6669 6c6c 2028 7479 7065 206f     (fill (type o
+00000f20: 7574 6c69 6e65 2929 0a20 2020 2020 2029  utline)).      )
+00000f30: 0a20 2020 2020 2028 706f 6c79 6c69 6e65  .      (polyline
+00000f40: 0a20 2020 2020 2020 2028 7074 730a 2020  .        (pts.  
+00000f50: 2020 2020 2020 2020 2878 7920 342e 3935          (xy 4.95
+00000f60: 3320 2d30 2e36 3335 290a 2020 2020 2020  3 -0.635).      
+00000f70: 2020 2020 2878 7920 352e 3538 3820 302e      (xy 5.588 0.
+00000f80: 3530 3829 0a20 2020 2020 2020 2020 2028  508).          (
+00000f90: 7879 2036 2e32 3233 202d 302e 3633 3529  xy 6.223 -0.635)
+00000fa0: 0a20 2020 2020 2020 2020 2028 7879 2035  .          (xy 5
+00000fb0: 2e30 3820 2d30 2e36 3335 290a 2020 2020  .08 -0.635).    
+00000fc0: 2020 2020 290a 2020 2020 2020 2020 2873      ).        (s
+00000fd0: 7472 6f6b 6520 2877 6964 7468 2030 2920  troke (width 0) 
+00000fe0: 2874 7970 6520 6465 6661 756c 7429 290a  (type default)).
+00000ff0: 2020 2020 2020 2020 2866 696c 6c20 2874          (fill (t
+00001000: 7970 6520 6f75 746c 696e 6529 290a 2020  ype outline)).  
+00001010: 2020 2020 290a 2020 2020 290a 2020 2020      ).    ).    
+00001020: 2873 796d 626f 6c20 2249 504e 5f31 5f31  (symbol "IPN_1_1
+00001030: 220a 2020 2020 2020 2870 696e 2062 6964  ".      (pin bid
+00001040: 6972 6563 7469 6f6e 616c 206c 696e 6520  irectional line 
+00001050: 2861 7420 332e 3831 2037 2e36 3220 3237  (at 3.81 7.62 27
+00001060: 3029 2028 6c65 6e67 7468 2035 2e30 3829  0) (length 5.08)
+00001070: 0a20 2020 2020 2020 2028 6e61 6d65 2022  .        (name "
+00001080: 4422 2028 6566 6665 6374 7320 2866 6f6e  D" (effects (fon
+00001090: 7420 2873 697a 6520 312e 3237 2031 2e32  t (size 1.27 1.2
+000010a0: 3729 2929 290a 2020 2020 2020 2020 286e  7)))).        (n
+000010b0: 756d 6265 7220 227e 2220 2865 6666 6563  umber "~" (effec
+000010c0: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+000010d0: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+000010e0: 2020 2029 0a20 2020 2020 2028 7069 6e20     ).      (pin 
+000010f0: 696e 7075 7420 6c69 6e65 2028 6174 202d  input line (at -
+00001100: 332e 3831 2030 2030 2920 286c 656e 6774  3.81 0 0) (lengt
+00001110: 6820 352e 3038 290a 2020 2020 2020 2020  h 5.08).        
+00001120: 286e 616d 6520 2247 2220 2865 6666 6563  (name "G" (effec
+00001130: 7473 2028 666f 6e74 2028 7369 7a65 2031  ts (font (size 1
+00001140: 2e32 3720 312e 3237 2929 2929 0a20 2020  .27 1.27)))).   
+00001150: 2020 2020 2028 6e75 6d62 6572 2022 7e22       (number "~"
+00001160: 2028 6566 6665 6374 7320 2866 6f6e 7420   (effects (font 
+00001170: 2873 697a 6520 312e 3237 2031 2e32 3729  (size 1.27 1.27)
+00001180: 2929 290a 2020 2020 2020 290a 2020 2020  ))).      ).    
+00001190: 2020 2870 696e 2062 6964 6972 6563 7469    (pin bidirecti
+000011a0: 6f6e 616c 206c 696e 6520 2861 7420 332e  onal line (at 3.
+000011b0: 3831 202d 372e 3632 2039 3029 2028 6c65  81 -7.62 90) (le
+000011c0: 6e67 7468 2035 2e30 3829 0a20 2020 2020  ngth 5.08).     
+000011d0: 2020 2028 6e61 6d65 2022 5322 2028 6566     (name "S" (ef
+000011e0: 6665 6374 7320 2866 6f6e 7420 2873 697a  fects (font (siz
+000011f0: 6520 312e 3237 2031 2e32 3729 2929 290a  e 1.27 1.27)))).
+00001200: 2020 2020 2020 2020 286e 756d 6265 7220          (number 
+00001210: 227e 2220 2865 6666 6563 7473 2028 666f  "~" (effects (fo
+00001220: 6e74 2028 7369 7a65 2031 2e32 3720 312e  nt (size 1.27 1.
+00001230: 3237 2929 2929 0a20 2020 2020 2029 0a20  27)))).      ). 
+00001240: 2020 2029 0a20 2029 0a29 0a                 ).  ).).
```

### Comparing `kintree-1.0.0b2/kintree/kicad/templates_project/templates_project.kicad_prl` & `kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_prl`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.985897435897436%*

 * *Differences: {"'board'": "{'opacity': {'images': 0.6}, 'hidden_netclasses': []}"}*

```diff
@@ -1,16 +1,18 @@
 {
     "board": {
         "active_layer": 0,
         "active_layer_preset": "",
         "auto_track_width": true,
+        "hidden_netclasses": [],
         "hidden_nets": [],
         "high_contrast_mode": 0,
         "net_color_mode": 1,
         "opacity": {
+            "images": 0.6,
             "pads": 1.0,
             "tracks": 1.0,
             "vias": 1.0,
             "zones": 0.6
         },
         "ratsnest_display_mode": 0,
         "selection_filter": {
```

### Comparing `kintree-1.0.0b2/kintree/kintree_gui_0.6.x.py` & `kintree-1.0.0rc0/kintree/kintree_gui_0.6.x.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/logo.png` & `kintree-1.0.0rc0/kintree/logo.png`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/digikey_api.py` & `kintree-1.0.0rc0/kintree/search/digikey_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/element14_api.py` & `kintree-1.0.0rc0/kintree/search/element14_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/lcsc_api.py` & `kintree-1.0.0rc0/kintree/search/lcsc_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/mouser_api.py` & `kintree-1.0.0rc0/kintree/search/mouser_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/search_api.py` & `kintree-1.0.0rc0/kintree/search/search_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/search/snapeda_api.py` & `kintree-1.0.0rc0/kintree/search/snapeda_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/kintree/setup_inventree.py` & `kintree-1.0.0rc0/kintree/setup_inventree.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0b2/pyproject.toml` & `kintree-1.0.0rc0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kintree"
-version = "1.0.0b2"
+version = "1.0.0rc"
 description = "Fast part creation in KiCad and InvenTree"
 authors = ["eeintech <eeintech@eeinte.ch>"]
 maintainers = ["eeintech <eeintech@eeinte.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/sparkmicro/Ki-nTree"
 repository = "https://github.com/sparkmicro/Ki-nTree"
 keywords = ["inventree", "kicad", "component", "part", "create"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 digikey-api = "^1.0.0"
 Flet = "^0.4.2"
 thefuzz = "^0.19.0"
-inventree = "^0.9.2"
-kiutils = "^1.3.0"
-mouser = "^0.1.2"
+inventree = "^0.10.1"
+kiutils = "^1.4.0"
+mouser = "^0.1.3"
 multiprocess = "^0.70.12"
 PyYAML = "^5.4.1"
 validators = "^0.19.0"
 wrapt_timeout_decorator = "^1.3.12"
 
 [tool.poetry.dev-dependencies]
 invoke = "^1.7.3"
```

### Comparing `kintree-1.0.0b2/PKG-INFO` & `kintree-1.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kintree
-Version: 1.0.0b2
+Version: 1.0.0rc0
 Summary: Fast part creation in KiCad and InvenTree
 Home-page: https://github.com/sparkmicro/Ki-nTree
 License: GPL-3.0-or-later
 Keywords: inventree,kicad,component,part,create
 Author: eeintech
 Author-email: eeintech@eeinte.ch
 Maintainer: eeintech
@@ -14,62 +14,63 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Flet (>=0.4.2,<0.5.0)
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: digikey-api (>=1.0.0,<2.0.0)
-Requires-Dist: inventree (>=0.9.2,<0.10.0)
-Requires-Dist: kiutils (>=1.3.0,<2.0.0)
-Requires-Dist: mouser (>=0.1.2,<0.2.0)
+Requires-Dist: inventree (>=0.10.1,<0.11.0)
+Requires-Dist: kiutils (>=1.4.0,<2.0.0)
+Requires-Dist: mouser (>=0.1.3,<0.2.0)
 Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: validators (>=0.19.0,<0.20.0)
 Requires-Dist: wrapt_timeout_decorator (>=1.3.12,<2.0.0)
 Project-URL: Repository, https://github.com/sparkmicro/Ki-nTree
 Description-Content-Type: text/markdown
 
-# Ki-nTree
-### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.readthedocs.io/) 
+# <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
+### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
 ## New version (1.0) is coming soon!
 
-To install the beta release:
+To install the release candidate:
 ``` shell
 pip install --pre -U kintree
 ```
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_preview.png" width="auto" height="auto">
+<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
 ## Demo Videos :fast_forward: [Full Demo](https://youtu.be/haSAu926BOI) :fast_forward: [KiCad Demo](https://youtu.be/NSMfCCD0uVw)
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_example.png"  width="auto" height="auto">
-
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
 * automate part creation of InvenTree parts
 * synchronize parts data between KiCad and InvenTree
 
 Ki-nTree works with:
 - [Digi-Key](https://developer.digikey.com/), [Mouser](https://www.mouser.com/api-hub/), [Element14](https://partner.element14.com/docs) and [LCSC](https://lcsc.com/) **enormous** part databases and free APIs
-- the awesome open-source [Digi-Key API python library](https://github.com/peeter123/digikey-api) built and maintained by [@peeter123](https://github.com/peeter123)
+- the awesome open-source [InvenTree Inventory Management System](https://github.com/inventree/inventree) built and maintained by [@SchrodingersGat](https://github.com/SchrodingersGat) and [@matmair](https://github.com/matmair)
+- the reliable and SCM-friendly KiCad file parser [KiUtils](https://github.com/mvnmgrx/kiutils) built and maintained by [@mvnmgrx](https://github.com/mvnmgrx)
+- the amazing [Digi-Key API python library](https://github.com/peeter123/digikey-api) built and maintained by [@peeter123](https://github.com/peeter123)
 - the [Mouser Python API](https://github.com/sparkmicro/mouser-api/) built and maintained by [@eeintech](https://github.com/eeintech)
-- the awesome open-source [InvenTree Inventory Management System](https://github.com/inventree/inventree) built and maintained by [@SchrodingersGat](https://github.com/SchrodingersGat)
-- [KiCad](https://www.kicad.org/) (of course!) and their open-source [library utils](https://gitlab.com/kicad/libraries/kicad-library-utils)
 
-> **Important Note**
+> :warning: **Important Note**
+>
+> Ki-nTree version `1.0.x` and forward support KiCad versions **6 and up**.
+>
+> Ki-nTree versions `0.5.x` and `0.6.x` only support KiCad version **6** (`pip install kintree==0.6.6`).
 >
-> Because of limited maintenance bandwidth, Ki-nTree versions `0.5.x` and newer will only support KiCad version **6**.
-> To keep using Ki-nTree with KiCad version **5**, use older `0.4.x` versions (`pip install kintree==0.4.8`).
+> To use with KiCad version **5**, use older Ki-nTree `0.4.x` versions (`pip install kintree==0.4.8`).
 
 Ki-nTree was developped by [@eeintech](https://github.com/eeintech) for [SPARK Microsystems](https://www.sparkmicro.com/), who generously accepted to make it open-source!
 
 ## Get Started
 
 ### Requirements
 
@@ -118,16 +119,14 @@
 ### Packages
 #### Arch Linux
 
 Ki-nTree is [available on Arch Linux's AUR](https://aur.archlinux.org/packages/python-kintree/) as `python-kintree`.
 
 ### Usage Instructions
 
-> :warning: Warning: **KiCad library writer is still in development**: Make sure to open KiCad libraries inside the symbol editor and save them after adding symbols.
-
 #### Before Starting
 
 If you intend to use Ki-nTree with InvenTree, this tool offers to setup the InvenTree category tree with a simple script that you can run as follow:
 
 > :warning: Warning: Before running it, make sure you have setup your category tree in your `categories.yaml` configuration file according to your own preferences, else it will use the [default setup](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/categories.yaml).
 
 ``` bash
@@ -136,42 +135,42 @@
 
 If the InvenTree category tree is **not setup** before starting to use Ki-nTree, you **won't be able to add parts** to InvenTree.
 
 #### Advanced Configuration
 
 Configuration files are stored in the folder pointed by the `Configuration Files Folder` path in the "User Settings" window:
 
-<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/settings_user_cache.png" width="600" height="auto">
+<img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_settings_user.png" width="600" height="auto">
 
 
 <details>
 <summary><b>Click here to read about configuration files</b></summary>
 <p>
 
 Ki-nTree uses a number of YAML configuration files to function. New users shouldn't need to worry about them to try out Ki-nTree (except for `categories.yaml` as mentioned in the previous section), however they can be modified to customize behavior and workflow.
 
 Below is a summary table of the different configuration files, their function and if they are updated by the GUI:
 | Filename | Function | GUI Update? |
 | --- | --- | --- |
 | `categories.yaml` | InvenTree categories hierarchy tree and category codes for IPN generation (see [Before Starting section](#before-starting)) | :x: |
-| `general.yaml` | General user settings | _Partial_ |
-| `internal_part_number.yaml` | Controls for IPN generation | :x: |
+| `general.yaml` | General user settings | :heavy_check_mark: |
+| `internal_part_number.yaml` | Controls for IPN generation | :heavy_check_mark: |
 | `inventree_<env>.yaml` | InvenTree login credentials, per environment (`<env>=['dev', 'prod']`) | :heavy_check_mark: |
 | `kicad.yaml` | KiCad symbol, footprint and library paths | :heavy_check_mark: |
 | `kicad_map.yaml` | Mapping between InvenTree parent categories and KiCad symbol/footprint libraries and templates | :x: |
 | `parameters.yaml` | List of InvenTree parameters templates (see [InvenTree Part Parameters documentation](https://docs.inventree.org/en/latest/part/parameter/)) | :x: |
 | `parameters_filters.yaml` | Mapping between InvenTree parent categories and InvenTree parameters templates | :x: |
-| `search_api.yaml` | Generic controls for Supplier search APIs like cache validity and category matching ratio | :x: |
+| `search_api.yaml` | Generic controls for Supplier search APIs like cache validity | :heavy_check_mark: |
 | `supplier_parameters.yaml` | Mapping between InvenTree parameters templates and suppliers parameters/attributes, sorted by InvenTree parent categories (see [Part Parameters section](#part-parameters)) | :x: |
 | `<supplier>_config.yaml` | Mapping for supplier name and search results fields, to overwrite defaults (`<supplier>=['digikey', 'element14', 'lcsc', 'mouser']`) | :x: |
 | `<supplier>_api.yaml` | Required supplier API fields, custom to each supplier (`<supplier>=['digikey', 'element14', 'lcsc', 'mouser']`) | :heavy_check_mark: |
-| `digikey_categories.yaml` | Mapping between InvenTree categories and Digi-Key categories | :heavy_check_mark: |
+| `digikey_categories.yaml` | Mapping between InvenTree categories and Digi-Key categories | :x: |
 | `digikey_parameters.yaml` | Mapping between InvenTree parameters and Digi-Key parameters/attributes | :x: |
 
-> In versions `0.6.x` and older, Ki-nTree only supports matching between InvenTree and Digi-Key categories and parameters/attibutes (help wanted!)
+> Ki-nTree only supports matching between InvenTree and Digi-Key categories and parameters/attibutes (help wanted!)
 
 </p>
 </details>
 
 #### InvenTree Permissions
 
 Each InvenTree user has a set of permissions associated to them.
@@ -256,15 +255,15 @@
 ```
 
 2. Install the requirements into a `poetry`-managed virtual environment
 ``` bash
 poetry install
 Installing dependencies from lock file
 ...
-Installing the current project: kintree (0.4.99)
+Installing the current project: kintree (1.0.99)
 ```
 > Note: the version is not accurate (placeholder only)
 
 3. Run Ki-nTree in the virtual environment
 ```bash
 poetry run python -m kintree_gui
 ```
@@ -275,53 +274,32 @@
 $ python -m kintree_gui
 ```
 
 #### Build
 1. Make sure you followed the previous installation steps, then run:
 ``` bash
 $ poetry build
-Building kintree (0.6.99)
+Building kintree (1.0.99)
   - Building sdist
-  - Built kintree-0.6.99.tar.gz
+  - Built kintree-1.0.99.tar.gz
   - Building wheel
-  - Built kintree-0.6.99-py3-none-any.whl
+  - Built kintree-1.0.99-py3-none-any.whl
 ```
 2. Exit the virtual environment (`Ctrl + D` on Linux; you can also close the
    terminal and reopen it in the same folder).
 
    Run `pip install dist/<wheel_file>.whl` with the file name from the previous
    step. For example:
 
 ```bash
-pip install dist/kintree-0.6.99-py3-none-any.whl
+pip install dist/kintree-1.0.99-py3-none-any.whl
 ```
 
 3. You can now start Ki-nTree by typing `kintree` in the terminal, provided
    that your python dist path is a part of your `$PATH`.
 
-## Roadmap
-
-> Priority goes to implementing new features over GUI improvements  
-> Open to new ideas and pull requests :smiley:
-
-#### Versions 1.0.x or later
-(Strikethrough items are supported in V1.0.0 beta1 release)
-
-##### New Features
-~~- Revamp category selection based on hierarchical structure from InvenTree ([reference](https://github.com/sparkmicro/Ki-nTree/issues/87))~~  
-~~- Allow user to decide the category code to use for IPN~~  
-~~- Enable option to download and save PDF files locally/to internal server storage~~
-
-##### Improvements
-~~- Optimize the category search ([reference](https://github.com/sparkmicro/Ki-nTree/issues/104))~~  
-~~- Migrate KiCad library management to [KiUtils](https://github.com/mvnmgrx/kiutils) ([reference](https://github.com/sparkmicro/Ki-nTree/issues/119))~~  
-- Add support for KiCad V7 ([reference](https://github.com/sparkmicro/Ki-nTree/issues/120))
-
-##### GUI
-~~- Migrate to [Flet](https://github.com/flet-dev/flet) ([reference](https://github.com/sparkmicro/Ki-nTree/issues/37))~~
-
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
-* https://gitlab.com/kicad/libraries/kicad-library-utils
+* https://github.com/mvnmgrx/kiutils
 * https://github.com/peeter123/digikey-api
 
 The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
```

