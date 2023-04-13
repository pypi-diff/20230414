# Comparing `tmp/runtimepy-1.4.0.tar.gz` & `tmp/runtimepy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.4.0.tar", last modified: Thu Apr 13 22:15:58 2023, max compression
+gzip compressed data, was "runtimepy-1.4.1.tar", last modified: Thu Apr 13 23:39:06 2023, max compression
```

## Comparing `runtimepy-1.4.0.tar` & `runtimepy-1.4.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.386806 runtimepy-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 22:14:20.000000 runtimepy-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 22:15:58.382805 runtimepy-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-13 22:14:20.000000 runtimepy-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 22:14:20.000000 runtimepy-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.370804 runtimepy-1.4.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.366804 runtimepy-1.4.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.378805 runtimepy-1.4.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 22:14:20.000000 runtimepy-1.4.0/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.374805 runtimepy-1.4.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 22:15:58.000000 runtimepy-1.4.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:15:58.386806 runtimepy-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 22:14:20.000000 runtimepy-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:15:58.382805 runtimepy-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 22:14:20.000000 runtimepy-1.4.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 22:14:20.000000 runtimepy-1.4.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 22:14:20.000000 runtimepy-1.4.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 23:37:43.000000 runtimepy-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 23:39:06.059302 runtimepy-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-13 23:37:43.000000 runtimepy-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 23:37:43.000000 runtimepy-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.039302 runtimepy-1.4.1/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.031303 runtimepy-1.4.1/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/task/basic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:39:06.059302 runtimepy-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 23:37:43.000000 runtimepy-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_resources.py
```

### Comparing `runtimepy-1.4.0/LICENSE` & `runtimepy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/PKG-INFO` & `runtimepy-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=5e9b582a69bb3f7feead0f3db3466aaf
+    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
     =====================================
 -->
 
-# runtimepy ([1.4.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.0/README.md` & `runtimepy-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=5e9b582a69bb3f7feead0f3db3466aaf
+    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
     =====================================
 -->
 
-# runtimepy ([1.4.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.0/pyproject.toml` & `runtimepy-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.4.0"
+version = "1.4.1"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.4.0/runtimepy/app.py` & `runtimepy-1.4.1/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/__init__.py` & `runtimepy-1.4.1/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/__init__.py` & `runtimepy-1.4.1/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/array.py` & `runtimepy-1.4.1/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/base.py` & `runtimepy-1.4.1/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/create.py` & `runtimepy-1.4.1/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/file.py` & `runtimepy-1.4.1/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/environment/names.py` & `runtimepy-1.4.1/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/channel/registry.py` & `runtimepy-1.4.1/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/codec/protocol/base.py` & `runtimepy-1.4.1/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/codec/protocol/json.py` & `runtimepy-1.4.1/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/commands/all.py` & `runtimepy-1.4.1/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/commands/arbiter.py` & `runtimepy-1.4.1/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/commands/tui.py` & `runtimepy-1.4.1/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.4.1/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.4.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/entry.py` & `runtimepy-1.4.1/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/enum/__init__.py` & `runtimepy-1.4.1/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/enum/registry.py` & `runtimepy-1.4.1/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/enum/type.py` & `runtimepy-1.4.1/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/mapping.py` & `runtimepy-1.4.1/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/mixins/enum.py` & `runtimepy-1.4.1/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/mixins/regex.py` & `runtimepy-1.4.1/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/__init__.py` & `runtimepy-1.4.1/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/base.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/config.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,17 @@
 
         # Registier factories.
         for factory in config.factories:
             name = factory["name"]
             assert self.register_module_factory(
                 name,
                 *factory.get("namespaces", []),
-                **factory.get("kwargs", {}),
+                **dict_resolve_env_vars(
+                    factory.get("kwargs", {}), env=config.ports  # type: ignore
+                ),
             ), "Couldn't register factory '{name}'!"
 
         # Register clients.
         for client in config.clients:
             factory = client["factory"]
             name = client["name"]
```

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/factory.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/factory.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/imports.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/udp.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.4.1/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/connection.py` & `runtimepy-1.4.1/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/factories/__init__.py` & `runtimepy-1.4.1/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/manager.py` & `runtimepy-1.4.1/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/mixin.py` & `runtimepy-1.4.1/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/tcp/connection.py` & `runtimepy-1.4.1/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.4.1/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.4.1/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/udp/connection.py` & `runtimepy-1.4.1/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/util.py` & `runtimepy-1.4.1/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/net/websocket/connection.py` & `runtimepy-1.4.1/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/__init__.py` & `runtimepy-1.4.1/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/array.py` & `runtimepy-1.4.1/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/base.py` & `runtimepy-1.4.1/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/bool.py` & `runtimepy-1.4.1/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/byte_order.py` & `runtimepy-1.4.1/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/field/__init__.py` & `runtimepy-1.4.1/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/field/fields.py` & `runtimepy-1.4.1/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.4.1/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.4.1/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/float.py` & `runtimepy-1.4.1/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/int.py` & `runtimepy-1.4.1/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/string.py` & `runtimepy-1.4.1/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/type/__init__.py` & `runtimepy-1.4.1/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/type/base.py` & `runtimepy-1.4.1/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/type/float.py` & `runtimepy-1.4.1/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/primitives/type/int.py` & `runtimepy-1.4.1/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/registry/__init__.py` & `runtimepy-1.4.1/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/registry/bool.py` & `runtimepy-1.4.1/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/registry/item.py` & `runtimepy-1.4.1/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/registry/name.py` & `runtimepy-1.4.1/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/schemas.py` & `runtimepy-1.4.1/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/task/__init__.py` & `runtimepy-1.4.1/runtimepy/task/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/task/basic/__init__.py` & `runtimepy-1.4.1/runtimepy/task/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/tui/channels/__init__.py` & `runtimepy-1.4.1/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy/tui/task.py` & `runtimepy-1.4.1/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.4.1/runtimepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=5e9b582a69bb3f7feead0f3db3466aaf
+    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
     =====================================
 -->
 
-# runtimepy ([1.4.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.4.1/runtimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/setup.py` & `runtimepy-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/tests/test_entry.py` & `runtimepy-1.4.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.0/tests/test_mapping.py` & `runtimepy-1.4.1/tests/test_mapping.py`

 * *Files identical despite different names*

