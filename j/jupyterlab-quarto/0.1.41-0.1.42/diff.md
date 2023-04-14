# Comparing `tmp/jupyterlab_quarto-0.1.41.tar.gz` & `tmp/jupyterlab_quarto-0.1.42.tar.gz`

## Comparing `jupyterlab_quarto-0.1.41.tar` & `jupyterlab_quarto-0.1.42.tar`

### file list

```diff
@@ -1,112 +1,138 @@
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/install.json
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jest.config.js
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/setup.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/tsconfig.json
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/.turbo/turbo-build.log
--rw-r--r--   0        0        0    99224 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/example/example.ipynb
--rw-r--r--   0        0        0   212480 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/example/penguins.ipynb
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/example/working.jpeg
--rw-r--r--   0        0        0    99258 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/example/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/_version.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/package.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/package.json.orig
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/plugin.json
--rw-r--r--   0        0        0    19399 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/149.801306413a3cfdd81f86.js
--rw-r--r--   0        0        0    39516 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/195.c842d2e614de28bfe165.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/195.c842d2e614de28bfe165.js.LICENSE.txt
--rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/289.bde50d91891a2c5d7f26.js
--rw-r--r--   0        0        0  1402418 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/306.28f62749175a96b6ee44.js
--rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/327.de030d8658ea8d025a4a.js
--rw-r--r--   0        0        0    28056 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/337.4080fbd1086e93f41b68.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/388.25da03e62f316adece62.js
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/530.beae53e3765e960d1624.js
--rw-r--r--   0        0        0    55305 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/54.1f6a6902b285bc14280c.js
--rw-r--r--   0        0        0   855230 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/556.0beb834b3fdb7fd7ec23.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/556.0beb834b3fdb7fd7ec23.js.LICENSE.txt
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/643.6128b4348ee378bfa578.js
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/736.8e56987f52d319dd9fb1.js
--rw-r--r--   0        0        0   457207 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/744.1350087357e5daf67432.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/744.1350087357e5daf67432.js.LICENSE.txt
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/756.d250a8db06cb4ff6e3a7.js
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/788.9169e895a35225ca8ef7.js
--rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/899.b8925c5400d893ccc523.js
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/975.68ac33a18baded01f9fc.js
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/remoteEntry.36176211157a09c0eb44.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/style.js
--rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/schema/plugin.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/const.ts
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/index.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/manager.ts
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/types.ts
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/widgets.ts
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-deflist.d.ts
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-footnote.d.ts
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-gridtables.d.ts
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-implicit-figures.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-sub.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-sup.d.ts
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/@types/markdown-it-task-lists.d.ts
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/__tests__/myextension.spec.ts
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/ast/ast.ts
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/hooks/codemirror.ts
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/callouts.ts
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/cites.ts
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/decorator.ts
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/divs.ts
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/figure-divs.ts
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/figures.ts
--rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/math.ts
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/shortcodes.ts
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/spans.ts
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/table-captions.ts
--rw-r--r--   0        0        0    11604 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/yaml.ts
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/index.ts
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/gridtables/GetCells.ts
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/EmitTable.ts
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/GetLine.ts
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/ParseTable.ts
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/interfaces/markdown-it/IState.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/gridtables/rules/gridtable.ts
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/plugins/mermaid/index.ts
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/attrs.ts
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/callouts.ts
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/cites.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/decorator.ts
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/deflist.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/divs.ts
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/figure-divs.ts
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/figures.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/footnotes.ts
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/gridtables.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/math.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/mermaid.ts
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/provider.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/shortcodes.ts
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/spans.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/sub.ts
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/sup.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/table-captions.ts
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/tasklists.ts
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/providers/yaml.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/utils/html.ts
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/utils/markdownit.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/src/utils/tok.ts
--rw-r--r--   0        0        0    12921 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/style/index.js
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/LICENSE
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/README.md
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/pyproject.toml
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.41/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/.DS_Store
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/Untitled.ipynb
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/install.json
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jest.config.js
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/setup.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/tsconfig.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/.turbo/turbo-build.log
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/apa.csl
+-rw-r--r--   0        0        0    99224 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/example.ipynb
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/palmer-biblio.bib
+-rw-r--r--   0        0        0   212480 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/penguins.ipynb
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/working.jpeg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/.ipynb_checkpoints/callouts-checkpoint.ipynb
+-rw-r--r--   0        0        0    99258 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0   212499 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/example/.ipynb_checkpoints/penguins-checkpoint.ipynb
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/_version.py
+-rw-r--r--   0        0        0    21847 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/build_log.json
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/package.json
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/schemas/@quarto/jupyterlab-quarto/package.json.orig
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/schemas/@quarto/jupyterlab-quarto/plugin.json
+-rw-r--r--   0        0        0   141341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/lib_index_js.2f3c2800757da4bf48d0.js
+-rw-r--r--   0        0        0   172451 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/lib_index_js.2f3c2800757da4bf48d0.js.map
+-rw-r--r--   0        0        0    30936 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_css-loader_dist_cjs_js_style_base_css.063e9f27169f2b20a055.js
+-rw-r--r--   0        0        0    33801 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_css-loader_dist_cjs_js_style_base_css.063e9f27169f2b20a055.js.map
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-deflist_index_js.e1706800a4396962c792.js
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-deflist_index_js.e1706800a4396962c792.js.map
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sub_index_js.2ac274eb3a38b60b8ab8.js
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sub_index_js.2ac274eb3a38b60b8ab8.js.map
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sup_index_js.ead4bbcdce2c7f1bfd0a.js
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sup_index_js.ead4bbcdce2c7f1bfd0a.js.map
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-task-lists_index_js.44d456ca4d35bbb4a9e0.js
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/node_modules_markdown-it-task-lists_index_js.44d456ca4d35bbb4a9e0.js.map
+-rw-r--r--   0        0        0    41012 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/remoteEntry.656d03911c9973a126a4.js
+-rw-r--r--   0        0        0    39959 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/remoteEntry.656d03911c9973a126a4.js.map
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/style.js
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/style_index_js.45b7a42be02fe193f132.js
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/style_index_js.45b7a42be02fe193f132.js.map
+-rw-r--r--   0        0        0    12128 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.28e98368204cfba1aa42.js
+-rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.28e98368204cfba1aa42.js.map
+-rw-r--r--   0        0        0   109175 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_js-yaml_dist_js-yaml_mjs.03af40b7cb1ed37e8d2c.js
+-rw-r--r--   0        0        0   130310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_js-yaml_dist_js-yaml_mjs.03af40b7cb1ed37e8d2c.js.map
+-rw-r--r--   0        0        0    22942 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-attrs_index_js.dfeed9348eb8277d5327.js
+-rw-r--r--   0        0        0    27508 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-attrs_index_js.dfeed9348eb8277d5327.js.map
+-rw-r--r--   0        0        0    12059 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-footnote_index_js.c67c4493a317e10619e6.js
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-footnote_index_js.c67c4493a317e10619e6.js.map
+-rw-r--r--   0        0        0   212973 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_index_js.8ece910fc237f14b0ba0.js
+-rw-r--r--   0        0        0   237842 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_index_js.8ece910fc237f14b0ba0.js.map
+-rw-r--r--   0        0        0    69747 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_lib_common_utils_js-node_modules_markdown-it_lib_token_js.cbe723d662753c03bdbf.js
+-rw-r--r--   0        0        0    40268 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_lib_common_utils_js-node_modules_markdown-it_lib_token_js.cbe723d662753c03bdbf.js.map
+-rw-r--r--   0        0        0  1554457 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.8b405bc41d428f2fb802.js
+-rw-r--r--   0        0        0  2029574 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.8b405bc41d428f2fb802.js.map
+-rw-r--r--   0        0        0  3481129 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mermaid_core_mjs.33cfe50e46b258ca24e5.js
+-rw-r--r--   0        0        0  3620263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mermaid_core_mjs.33cfe50e46b258ca24e5.js.map
+-rw-r--r--   0        0        0  1216192 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.ec6dd8eadd9d45e7c586.js
+-rw-r--r--   0        0        0  1473044 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.ec6dd8eadd9d45e7c586.js.map
+-rw-r--r--   0        0        0    55557 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_timeline-definition-8e5a9bc6_js.062c230044eb1ae11cf3.js
+-rw-r--r--   0        0        0    68997 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_timeline-definition-8e5a9bc6_js.062c230044eb1ae11cf3.js.map
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_wcwidth_index_js.45b4a90834ea855c7519.js
+-rw-r--r--   0        0        0    13341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/static/vendors-node_modules_wcwidth_index_js.45b4a90834ea855c7519.js.map
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/schema/plugin.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/const.ts
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/index.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/manager.ts
+-rw-r--r--   0        0        0    61581 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/test.log
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/types.ts
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/widgets.ts
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-deflist.d.ts
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-footnote.d.ts
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-gridtables.d.ts
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-implicit-figures.d.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-sub.d.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-sup.d.ts
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/@types/markdown-it-task-lists.d.ts
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/__tests__/myextension.spec.ts
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/ast/ast.ts
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/hooks/codemirror.ts
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/callouts.ts
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/cites.ts
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/decorator.ts
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/divs.ts
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/figure-divs.ts
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/figures.ts
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/math.ts
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/shortcodes.ts
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/spans.ts
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/table-captions.ts
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/yaml.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/index.ts
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/gridtables/GetCells.ts
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/EmitTable.ts
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/GetLine.ts
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/ParseTable.ts
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/interfaces/markdown-it/IState.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/gridtables/rules/gridtable.ts
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/mermaid/index.ts
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/utils/html.ts
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/utils/markdownit.ts
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/plugins/utils/tok.ts
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/attrs.ts
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/callouts.ts
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/cites.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/decorator.ts
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/deflist.ts
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/divs.ts
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/figure-divs.ts
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/figures.ts
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/footnotes.ts
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/gridtables.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/math.ts
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/mermaid.ts
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/provider.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/shortcodes.ts
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/spans.ts
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/sub.ts
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/sup.ts
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/table-captions.ts
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/tasklists.ts
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/src/providers/yaml.ts
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/style/index.js
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/LICENSE
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/README.md
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/pyproject.toml
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.42/PKG-INFO
```

### Comparing `jupyterlab_quarto-0.1.41/RELEASE.md` & `jupyterlab_quarto-0.1.42/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/jest.config.js` & `jupyterlab_quarto-0.1.42/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/package.json` & `jupyterlab_quarto-0.1.42/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.42'"}*

```diff
@@ -117,9 +117,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.41"
+    "version": "0.1.42"
 }
```

### Comparing `jupyterlab_quarto-0.1.41/.turbo/turbo-build.log` & `jupyterlab_quarto-0.1.42/.turbo/turbo-build.log`

 * *Files 6% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 
 Compilation starting…
 
 
 Compilation finished
 
 assets by chunk 6.45 MiB (id hint: vendors)
-  asset vendors-node_modules_mermaid_dist_mermaid_core_mjs.33cfe50e46b258ca24e5.js 3.32 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
-  asset vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.8b405bc41d428f2fb802.js 1.48 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
-  asset vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.ec6dd8eadd9d45e7c586.js 1.16 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
-  asset vendors-node_modules_markdown-it_index_js.8ece910fc237f14b0ba0.js 208 KiB [emitted] [immutable] (id hint: vendors) 1 related asset
-  asset vendors-node_modules_js-yaml_dist_js-yaml_mjs.03af40b7cb1ed37e8d2c.js 107 KiB [emitted] [immutable] (id hint: vendors) 1 related asset
+  asset vendors-node_modules_mermaid_dist_mermaid_core_mjs.f1ecd3a98599231c8777.js 3.32 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
+  asset vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.acad147ef8a8a7f9df1f.js 1.48 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
+  asset vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.4d34ed20a5d5a3bee971.js 1.16 MiB [emitted] [immutable] (id hint: vendors) 1 related asset
+  asset vendors-node_modules_markdown-it_index_js.441a9acdab854e8f5e31.js 208 KiB [emitted] [immutable] (id hint: vendors) 1 related asset
+  asset vendors-node_modules_js-yaml_dist_js-yaml_mjs.3c6d8dda6e87bd63f8fd.js 107 KiB [emitted] [immutable] (id hint: vendors) 1 related asset
   + 6 assets
-asset lib_index_js.b3a74e8f05040a5d95d5.js 138 KiB [emitted] [immutable] 1 related asset
-asset remoteEntry.e700caf34f0b7d8d9785.js 40.1 KiB [emitted] [immutable] (name: @quarto/jupyterlab-quarto) 1 related asset
-asset node_modules_css-loader_dist_cjs_js_style_base_css.ab21c49f137ea1607a7a.js 33.8 KiB [emitted] [immutable] 1 related asset
-asset node_modules_markdown-it-deflist_index_js.e1706800a4396962c792.js 6.52 KiB [emitted] [immutable] 1 related asset
-asset node_modules_markdown-it-task-lists_index_js.44d456ca4d35bbb4a9e0.js 3.55 KiB [emitted] [immutable] 1 related asset
-asset style_index_js.45b7a42be02fe193f132.js 2.24 KiB [emitted] [immutable] 1 related asset
-asset node_modules_markdown-it-sup_index_js.ead4bbcdce2c7f1bfd0a.js 1.97 KiB [emitted] [immutable] 1 related asset
-asset node_modules_markdown-it-sub_index_js.2ac274eb3a38b60b8ab8.js 1.96 KiB [emitted] [immutable] 1 related asset
+asset lib_index_js.3e8361751aff357b997d.js 138 KiB [emitted] [immutable] 1 related asset
+asset remoteEntry.43a03e7e5520efc15951.js 40 KiB [emitted] [immutable] (name: jupyterlab-quarto) 1 related asset
+asset node_modules_css-loader_dist_cjs_js_style_base_css.e41702efb19623bed476.js 30 KiB [emitted] [immutable] 1 related asset
+asset node_modules_markdown-it-deflist_index_js.0e6b0ffcf597c54b059b.js 6.51 KiB [emitted] [immutable] 1 related asset
+asset node_modules_markdown-it-task-lists_index_js.63b640ba78c0f89e4ad7.js 3.53 KiB [emitted] [immutable] 1 related asset
+asset style_index_js.04d68d4fb5e2cadc4acc.js 2.23 KiB [emitted] [immutable] 1 related asset
+asset node_modules_markdown-it-sup_index_js.a6cc7c1dd25e9485619c.js 1.95 KiB [emitted] [immutable] 1 related asset
+asset node_modules_markdown-it-sub_index_js.1fff94f55b4e2916234e.js 1.95 KiB [emitted] [immutable] 1 related asset
 orphan modules 487 KiB [orphan] 491 modules
 runtime modules 29 KiB 15 modules
 modules by path ../../node_modules/ 5.31 MiB 1013 modules
-modules by path ./ 124 KiB
+modules by path ./ 120 KiB
   modules by path ./lib/ 90.8 KiB 50 modules
-  modules by path ./style/ 33.4 KiB 5 modules
+  modules by path ./style/ 29.6 KiB 5 modules
 consume-shared-module modules 546 bytes
-  modules by path consume shared module (default) @jupyterlab/*.2 (singleton) 84 bytes 2 modules
+  modules by path consume shared module (default) @jupyterlab/*.3 (singleton) 84 bytes 2 modules
   + 11 modules
 provide-module modules 462 bytes
-  provide shared module (default) @quarto/jupyterlab-quarto@0.1.40 = ./lib/index.js 42 bytes [built] [code generated]
   provide shared module (default) js-yaml@4.1.0 = ../../node_modules/js-yaml/dist/js-yaml.mjs 42 bytes [built] [code generated]
+  provide shared module (default) jupyterlab-quarto@0.1.41 = ./lib/index.js 42 bytes [built] [code generated]
   + 9 modules
 container entry 42 bytes [built] [code generated]
-webpack 5.76.3 compiled successfully in 6826 ms
+webpack 5.76.3 compiled successfully in 4013 ms
```

### Comparing `jupyterlab_quarto-0.1.41/example/example.ipynb` & `jupyterlab_quarto-0.1.42/example/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/example/penguins.ipynb` & `jupyterlab_quarto-0.1.42/example/penguins.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/example/working.jpeg` & `jupyterlab_quarto-0.1.42/example/working.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/example/.ipynb_checkpoints/example-checkpoint.ipynb` & `jupyterlab_quarto-0.1.42/example/.ipynb_checkpoints/example-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/package.json` & `jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9495833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.656d03911c9973a126a4.js'}}",*

 * * "'name'": "'@quarto/jupyterlab-quarto'",*

 * * "'version'": "'0.1.42'"}*

```diff
@@ -61,15 +61,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/quarto-dev/quarto",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.36176211157a09c0eb44.js",
+            "load": "static/remoteEntry.656d03911c9973a126a4.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
@@ -80,15 +80,15 @@
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-quarto",
+    "name": "@quarto/jupyterlab-quarto",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/quarto-dev/quarto/quarto.git"
     },
@@ -122,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.41"
+    "version": "0.1.42"
 }
```

### Comparing `jupyterlab_quarto-0.1.41/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/package.json.orig` & `jupyterlab_quarto-0.1.42/jupyterlab-quarto/labextension/schemas/@quarto/jupyterlab-quarto/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'name'": "'@quarto/jupyterlab-quarto'", "'version'": "'0.1.42'"}*

```diff
@@ -75,15 +75,15 @@
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-quarto",
+    "name": "@quarto/jupyterlab-quarto",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/quarto-dev/quarto/quarto.git"
     },
@@ -117,9 +117,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.41"
+    "version": "0.1.42"
 }
```

### Comparing `jupyterlab_quarto-0.1.41/src/index.ts` & `jupyterlab_quarto-0.1.42/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     console.log('JupyterLab extension jupyterlab-quarto is activated!');
 
     // Create a markdown rendering manager 
     return markdownItManager();
   }
 };
 
-
 // Markdown It Extensions which provide base Pandoc behavior
 const kPandocExtensions = [
   footnotes, // footnote seriously render in the cell in which they appear in :(
   spans,
   attrs,
   deflist,
   figures,
```

### Comparing `jupyterlab_quarto-0.1.41/src/manager.ts` & `jupyterlab_quarto-0.1.42/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/types.ts` & `jupyterlab_quarto-0.1.42/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/widgets.ts` & `jupyterlab_quarto-0.1.42/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/__tests__/index.spec.ts` & `jupyterlab_quarto-0.1.42/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/ast/ast.ts` & `jupyterlab_quarto-0.1.42/src/ast/ast.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/hooks/codemirror.ts` & `jupyterlab_quarto-0.1.42/src/hooks/codemirror.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/callouts.ts` & `jupyterlab_quarto-0.1.42/src/plugins/callouts.ts`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 *
 * Copyright (C) 2020-2023 Posit Software, PBC
 *
 */
 import type MarkdownIt from "markdown-it/lib"
 import Renderer from "markdown-it/lib/renderer";
 import Token from "markdown-it/lib/token";
-import { addClass, readAttrValue } from "../utils/markdownit";
-import { kDivRuleName, kTokDivClose, kTokDivOpen } from "./divs";
+import { addClass, readAttrValue } from "./utils/markdownit";
+import { kTokDivClose, kTokDivOpen } from "./divs";
 
 
 const kTokCalloutOpen = "quarto_callout_open";
 const kTokCalloutClose = "quarto_callout_close";
 
 const kTokCalloutTitleOpen = "quarto_callout_title_open";
 const kTokCalloutTitleClose = "quarto_callout_title_close";
@@ -161,46 +161,46 @@
   md.renderer.rules[kTokCalloutClose] = renderEndCallout
   md.renderer.rules[kTokCalloutTitleOpen] = renderStartCalloutTitle
   md.renderer.rules[kTokCalloutTitleClose] = renderEndCalloutTitle
 }
 
 
 // Render pandoc-style divs
-function renderStartCallout(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderStartCallout(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
   const token = tokens[idx];
   const callout = token.meta as Callout;
 
   // Add classes decorating as callout
   token.attrs = addClass(`callout ${callout.clz}`, token.attrs);
 
   // Add class that reflects the style
   token.attrs = addClass(appearanceClass(callout.appearance), token.attrs);
 
   return `<div ${self.renderAttrs(token)}>`;
 }
 
 // Render pandoc-style divs
-function renderEndCallout(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderEndCallout(): string {
   return `</div>`;
 }
 
-function renderStartCalloutTitle(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderStartCalloutTitle(tokens: Token[], idx: number): string {
   const token = tokens[idx];
   const title = readAttrValue("title", token.attrs) || "";
   const startContent = `
 <div class="callout-header">
 <div class="callout-icon-container">
   <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container">${title}
 `;
   return startContent;
 }
 
-function renderEndCalloutTitle(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderEndCalloutTitle(): string {
   return `</div>\n</div>`;
 }
 
 
 const calloutAppearance = (val: string | undefined) => {
   if (val) {
     switch(val) {
@@ -248,11 +248,11 @@
   } else {
     return undefined;
   }
 
 }
 
 const appearanceClass = (appearance?:  "default" | "minimal" | "simple") => {
-  let style = appearance || "default";
+  const style = appearance || "default";
   return `callout-style-${style}`;
 }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/cites.ts` & `jupyterlab_quarto-0.1.42/src/plugins/cites.ts`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       if (token.type === 'inline' && token.children) {
 
         // Rebuild the child list
         const children: Token[] = [];
         for (let i = 0; i < token.children.length; i++) {
           const child = token.children[i];
           if (child.type === 'text') {
-            let content = child.content;
+            const content = child.content;
 
 
             const textToken = (text: string[]) => {
               const newToken = new state.Token('text', '', 0);
               newToken.content = text.join("");
               
               return newToken;
@@ -53,15 +53,15 @@
                   style = "normal";
                 }
 
                 // The classes
                 const clz = ["cite", style];
 
                 // If the cite ends in punctuation, trim that off and make that text
-                let puncText: string[] = [];
+                const puncText: string[] = [];
 
                 // Trim off ending punctuation
                 if ([":",".","#","$","%","&","-","+","?","<",">","~","/","!"].includes(cite[cite.length - 1])) {
                   puncText.push(cite[cite.length - 1]);
                   cite = cite.slice(0, -1);
                 }
 
@@ -150,12 +150,12 @@
   });
 
   md.renderer.rules[kTokCite] = renderCite
 }
 
 
 // Render pandoc-style divs
-function renderCite(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderCite(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
   const token = tokens[idx]; 
   const citeContent =  `<code ${self.renderAttrs(token)}>${token.content}</code>`;
   return citeContent;
 }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/decorator.ts` & `jupyterlab_quarto-0.1.42/src/plugins/decorator.ts`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 * fence.ts
 *
 * Copyright (C) 2020-2023 Posit Software, PBC
 *
 */
 import type MarkdownIt from "markdown-it/lib"
 import Token from "markdown-it/lib/token"
-import Renderer from "markdown-it/lib/renderer";
-import { attributeDecorator, decorator, DecoratorOptions } from "../utils/html";
+import { attributeDecorator, decorator, DecoratorOptions } from "./utils/html";
 import { kTokDivOpen } from "./divs";
 import { kTokFigureOpen } from "./figures";
-import { kTokHeadingOpen, kTokTableOpen } from "../utils/tok";
+import { kTokHeadingOpen, kTokTableOpen } from "./utils/tok";
 import { kTokMathBlock } from "./math";
 
 
 const kTokDecorator = "quarto_decorator";
 const kQuartoDecoratorOptions = "quarto-decorator-options";
 
 
@@ -53,15 +52,15 @@
     decoratorTok.meta[kQuartoDecoratorOptions] = options;  
   }
   return decoratorTok;
 }
 
 
 // Render pandoc-style divs
-function renderDecorator(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderDecorator(tokens: Token[], idx: number): string {
   const token = tokens[idx];
   const decoratorOptions = token.meta?.[kQuartoDecoratorOptions];
   if (token.info) {
     return decorator([token.info]) ;
   } else {
     return attributeDecorator(token, decoratorOptions);
   }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/divs.ts` & `jupyterlab_quarto-0.1.42/src/plugins/divs.ts`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 *
 * Copyright (C) 2020-2023 Posit Software, PBC
 *
 */
 import type MarkdownIt from "markdown-it/lib"
 import Token from "markdown-it/lib/token"
 import Renderer from "markdown-it/lib/renderer";
-import { addClass } from "../utils/markdownit";
+import { addClass } from "./utils/markdownit";
 
 export const kDivRuleName = "pandocDiv";
 
 export const kTokDivOpen = 'pandoc_div_open';
 export const kTokDivClose = 'pandoc_div_close';
 
 export const divPlugin = (md: MarkdownIt) => {
   
   // Render pandoc-style divs
-  function renderStartDiv(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+  function renderStartDiv(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
 
     // Add a class to designate that this is a quarto dev
     const token = tokens[idx];
     token.attrs = addClass("quarto-div", token.attrs)
 
     return `<div ${self.renderAttrs(token)}>`;
   }
 
   // Render pandoc-style divs
-  function renderEndDiv(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+  function renderEndDiv(): string {
     return `</div>`;
   }
 
   // TODO Implement a better test during validation run
   // Handle pandoc-style divs
   md.block.ruler.before(
     "fence",
     kDivRuleName,
-    (state, start, end, silent) => {
+    (state, start, _end, silent) => {
 
       // This is a validation run, can ignore
       if (silent) {
         return true;
       }
       
       // Get the line for parsing
@@ -64,15 +64,15 @@
         state.env.quartoOpenDivs[fence] = Math.max(0, current - 1);
       }
 
       // Three or more colons followed by a an optional brace with attributes
       const divBraceRegex = /^(:::+)\s*(?:(\{[\s\S]+?\}))?$/;
 
       // Three or more colons followed by a string with no braces
-      const divNoBraceRegex = /^(:::+)\s*(?:([^\{\}\s]+?))?$/;
+      const divNoBraceRegex = /^(:::+)\s*(?:([^{}\s]+?))?$/;
 
       const matchers = [divBraceRegex, divNoBraceRegex];
 
       let match;
       for (const matcher of matchers) {
         match = matcher.exec(line);
         if (match) {
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/figure-divs.ts` & `jupyterlab_quarto-0.1.42/src/plugins/figure-divs.ts`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
 import MarkdownIt from "markdown-it";
 import Token from "markdown-it/lib/token";
-import { readAttrValue } from "../utils/markdownit";
-import { kTokInline, kTokParaClose, kTokParaOpen } from "../utils/tok";
+import { readAttrValue } from "./utils/markdownit";
+import { kTokInline, kTokParaClose, kTokParaOpen } from "./utils/tok";
 import { kTokDivClose, kTokDivOpen } from "./divs";
 import { kTokFigCaptionClose, kTokFigCaptionOpen, mutateToFigureTok } from "./figures";
 
 
 const kFigureDivRuleName = "quarto-figure-divs";
 const kFigurePrefix = "fig-";
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/figures.ts` & `jupyterlab_quarto-0.1.42/src/plugins/figures.ts`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
 import MarkdownIt from "markdown-it";
 import Token from "markdown-it/lib/token";
-import { kTokParaClose, kTokParaOpen } from "../utils/tok";
+import { kTokParaClose, kTokParaOpen } from "./utils/tok";
 
 export interface FigureOptions {
   dataType?: boolean;
   link?: boolean;
   figcaption?: boolean;
   copyAttrs?: boolean;
   tabindex?: boolean;
@@ -30,19 +30,19 @@
 }
 
 export function figuresPlugin(md: MarkdownIt, options: FigureOptions) {
   options = options || {};
 
   md.core.ruler.before("linkify", "implicit_figures", (state) => {
     // reset tabIndex on md.render()
-    var tabIndex = 1;
+    let tabIndex = 1;
 
     // do not process first and last token
-    for (var i = 1, l = state.tokens.length; i < l - 1; ++i) {
-      var token = state.tokens[i];
+    for (let i = 1, l = state.tokens.length; i < l - 1; ++i) {
+      const token = state.tokens[i];
 
       if (token.type !== "inline") {
         continue;
       }
 
       // children: image alone, or link_open -> image -> link_close
       if (
@@ -74,26 +74,26 @@
       }
       // next token is paragraph close
       if (i !== l - 1 && state.tokens[i + 1].type !== kTokParaClose) {
         continue;
       }
 
       // The image
-      var image = token.children.length === 1 ? token.children[0] : token.children[1];
+      const image = token.children.length === 1 ? token.children[0] : token.children[1];
       
       // The image must have a caption to count as a figure
       if (!image.children || image.children.length === 0) {
         continue;
       }
     
       // We have inline token containing an image only.
       // Previous token is paragraph open.
       // Next token is paragraph close.
       // Lets replace the paragraph tokens with figure tokens.
-      var figure = state.tokens[i - 1];
+      const figure = state.tokens[i - 1];
       mutateToFigureTok(figure, "open");
       mutateToFigureTok(state.tokens[i + 1], "close");
 
       if (options.dataType == true) {
         state.tokens[i - 1].attrPush(["data-type", "image"]);
       }
 
@@ -119,15 +119,15 @@
           );
           image.children.length = 0;
         }
       }
 
       if (options.copyAttrs && image.attrs) {
         const f = options.copyAttrs === true ? "" : options.copyAttrs;
-        figure.attrs = image.attrs.filter(([k, v]) => k.match(f));
+        figure.attrs = image.attrs.filter(([k]) => k.match(f));
       }
 
       if (options.tabindex == true) {
         // add a tabindex property
         // you could use this with css-tricks.com/expanding-images-html5
         state.tokens[i - 1].attrPush(["tabindex", String(tabIndex)]);
         tabIndex++;
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/math.ts` & `jupyterlab_quarto-0.1.42/src/plugins/math.ts`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     return `<span class='quarto-inline-math'>\\(${content}\\)</span>`;
   }
 }
 
 // Test if potential opening or closing delimieter
 // Assumes that there is a "$" at state.src[pos]
 function isValidDelim(state: StateInline, pos: number) {
-  let max = state.posMax,
-    can_open = true,
-    can_close = true;
+  const max = state.posMax;
+  let can_open = true;
+  let can_close = true;
 
   const prevChar = pos > 0 ? state.src.charCodeAt(pos - 1) : -1,
     nextChar = pos + 1 <= max ? state.src.charCodeAt(pos + 1) : -1;
 
   // Check non-whitespace conditions for opening and closing, and
   // check that closing delimeter isn't followed by a number
   if (
@@ -207,15 +207,15 @@
     state.getLines(start + 1, next, state.tShift[start], true) +
     (lastLine && lastLine.trim() ? lastLine : "");
   token.map = [start, state.line];
   token.markup = "$$";
   return true;
 }
 
-export function mathjaxPlugin(md: MarkdownIt, options: any) {
+export function mathjaxPlugin(md: MarkdownIt) {
   // Default options
 
   const convertOptions = {
     display: false
   }
 
   // set MathJax as the renderer for markdown-it-simplemath
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/shortcodes.ts` & `jupyterlab_quarto-0.1.42/src/plugins/shortcodes.ts`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 * shortcodes.ts
 *
 * Copyright (C) 2020-2023 Posit Software, PBC
 *
 */
 import type MarkdownIt from "markdown-it/lib"
 import Token from "markdown-it/lib/token"
-import Renderer from "markdown-it/lib/renderer";
-import { addClass } from "../utils/markdownit";
 
 import StateInline from "markdown-it/lib/rules_inline/state_inline";
-import StateBlock from "markdown-it/lib/rules_block/state_block";
 import { escapeHtml } from "markdown-it/lib/common/utils";
 
 export const kShortcode = "shortcode";
 
 export const shortcodePlugin = (md: MarkdownIt) => {
   const shortcode = (state: StateInline, silent: boolean): boolean => {
     // {{< shortcode >}}
@@ -36,15 +33,15 @@
       token.content = shortcodeContent;
     }
     state.pos += end + 3;
     return true;
   }
   md.inline.ruler.after("escape", kShortcode, shortcode);
 
-  const renderShortcode = (tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string => {
+  const renderShortcode = (tokens: Token[], idx: number): string => {
     const token = tokens[idx];
     const content = token.content;
     // insert shortcode braces and escape content's html entities
     return `<span class="shortcode">${escapeHtml(`{{<${content}>}}`)}</span>`;
   }
 
   md.renderer.rules[kShortcode] = renderShortcode;
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/spans.ts` & `jupyterlab_quarto-0.1.42/src/plugins/spans.ts`

 * *Files 27% similar despite different names*

```diff
@@ -5,32 +5,32 @@
  *
  */
 
 import MarkdownIt from "markdown-it";
 import StateInline from "markdown-it/lib/rules_inline/state_inline";
 
 
-export function spansPlugin(md: MarkdownIt, _options: unknown) {
-  function span(state: StateInline, silent: boolean) {
-    var max = state.posMax
+export function spansPlugin(md: MarkdownIt) {
+  function span(state: StateInline) {
+    const max = state.posMax
 
     if (state.src.charCodeAt(state.pos) !== 0x5B) {
       // opening [
       return false;
     }
 
-    var labelStart = state.pos + 1;
-    var labelEnd   = state.md.helpers.parseLinkLabel(state, state.pos, true);
+    const labelStart = state.pos + 1;
+    const labelEnd   = state.md.helpers.parseLinkLabel(state, state.pos, true);
 
     if (labelEnd < 0) {
       // parser failed to find closing ]
       return false;
     }
 
-    var pos = labelEnd + 1;
+    const pos = labelEnd + 1;
     if (pos < max && state.src.charCodeAt(pos) === 0x7B /* { */) {
       // probably found span
 
       state.pos = labelStart;
       state.posMax = labelEnd;
 
       state.push('span_open', 'span', 1);
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/table-captions.ts` & `jupyterlab_quarto-0.1.42/src/plugins/table-captions.ts`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
 import MarkdownIt from "markdown-it";
 import Token from "markdown-it/lib/token";
-import { kTokInline, kTokParaClose, kTokParaOpen, kTokTableClose, kTokTableOpen, kTokText } from "../utils/tok";
+import { kTokInline, kTokParaClose, kTokParaOpen, kTokTableClose, kTokTableOpen, kTokText } from "./utils/tok";
 
 
 const kTableCaptionRule = "quarto-table-captions";
 
 export const tableCaptionPlugin = (md: MarkdownIt) => {
   
   md.core.ruler.push(
@@ -56,15 +56,15 @@
         && tokens[tblEndPos + 2].type === kTokInline
         && tokens[tblEndPos + 3].type === kTokParaClose) {
 
           const maybeCaption = tokens[tblEndPos + 2];
           
           const isText = maybeCaption.children !== null && maybeCaption.children.length > 0 && maybeCaption.children[0].type === kTokText;
           const maybeCaptionText = isText ? maybeCaption.children![0].content : "";
-          const match = maybeCaptionText.match(/^:\s([^\{\}]*)(?:\{.*\}){0,1}$/);
+          const match = maybeCaptionText.match(/^:\s([^{}]*)(?:\{.*\}){0,1}$/);
           if (match && match[1]) {
 
             // Carve out the existing tokens
             const capTokens = tokens.splice(tblEndPos + 1, 3);
 
             // We have the caption, remove the paragraph and return
             // the caption
@@ -79,20 +79,16 @@
             capTokens[1].children![0].content = match[1];
 
             // Close the caption
             capTokens[2].type = "table_caption";
             capTokens[2].tag = "caption";
 
             tokens.splice(tblStartPos + 1, 0, ...capTokens);
-          } else {
-            return undefined;
-          }
-      }
-    } else {
-      return undefined;
-    }
+          } 
+      } 
+    } 
   }
 
   interface TablePos {
     start: number,
     end: number
   }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/yaml.ts` & `jupyterlab_quarto-0.1.42/src/plugins/yaml.ts`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,25 @@
  * ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING THOSE OF NON-INFRINGEMENT,
  * MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE. Please refer to the
  * AGPL (http://www.gnu.org/licenses/agpl-3.0.txt) for more details.
  *
  */
 
 import MarkdownIt from "markdown-it";
-import Renderer from "markdown-it/lib/renderer";
 import StateBlock from "markdown-it/lib/rules_block/state_block";
 import Token from "markdown-it/lib/token";
 import * as yaml from "js-yaml";
-import { decorator } from "../utils/html";
+import { decorator } from "./utils/html";
 
 // Typescript version of https://github.com/parksb/markdown-it-front-matter
 // TODO: Rationalize this with quarto-core/src/markdownit-yaml.ts
 //       This is a copy with rendering added - the core tokenizing function is identical (or should be)
 const kTokFrontMatter = 'front_matter';
 
-export function markdownitFrontMatterPlugin(md: MarkdownIt, cb?: (yaml: unknown) => void) {
+export function yamlPlugin(md: MarkdownIt, cb?: (yaml: unknown) => void) {
   const min_markers = 3,
     marker_str = "-",
     marker_char = marker_str.charCodeAt(0),
     marker_len = marker_str.length;
 
   function frontMatter(
     state: StateBlock,
@@ -41,14 +40,16 @@
     let pos,
       nextLine,
       start_content,
       auto_closed = false,
       start = state.bMarks[startLine] + state.tShift[startLine],
       max = state.eMarks[startLine];
 
+
+
     // Check out the first character of the first line quickly,
     // this should filter out non-front matter
     if (startLine !== 0 || marker_char !== state.src.charCodeAt(0)) {
       return false;
     }
 
     // Check out the rest of the marker string
@@ -126,14 +127,15 @@
       }
 
       // found!
       auto_closed = true;
       break;
     }
 
+
     const old_parent = state.parentType;
     const old_line_max = state.lineMax;
     state.parentType = "root";
 
     // this will prevent lazy continuations from ever going past our end marker
     state.lineMax = nextLine;
 
@@ -159,22 +161,21 @@
     alt: ["paragraph", "reference", "blockquote", "list"],
   });
 
   // Add rendering
   md.renderer.rules[kTokFrontMatter] = renderFrontMatter
 }
 
-function renderFrontMatter(tokens: Token[], idx: number, options: MarkdownIt.Options, env: any, self: Renderer): string {
+function renderFrontMatter(tokens: Token[], idx: number): string {
   const token = tokens[idx];
 
   // Parse the markup
   const frontUnknown = parseFrontMatterStr(token.markup);
 
   // Extract important content
-  
   if (typeof(frontUnknown) === "object") {
     const titleBlock: TitleBlock = {};
     const frontMatter = frontUnknown as Record<string, unknown>;
 
     const readStr = (key: string) => {
       if (frontMatter[key] === undefined) {
         return undefined;
@@ -212,18 +213,19 @@
 
       // decorator
       const decor = decorator(["Options"]);
       titleLines.push(decor);
 
       // yaml
       const yamlDump = yaml.dump(frontMatter);
-      const otherYamlRendered = `<pre><code class="cm-s-jupyter language-yaml quarto-frontmatter">${yamlDump}</code></pre>`;
+      const otherYamlRendered = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${yamlDump}</code></pre>`;
 
       titleLines.push(otherYamlRendered);
     }
+
     return titleLines.join("\n");
   } else {
     return "";
   }
 }
 
 interface Author {
@@ -382,17 +384,18 @@
 
       const affiliations: string[] = [];
       const affiliationSimple = str("affiliation");
       if (affiliationSimple) {
         affiliations.push(affiliationSimple);
       } else if (authorRaw.affiliations) {
         const affils = Array.isArray(authorRaw.affiliations) ? authorRaw.affiliations as unknown[] : [authorRaw.affiliations];
-        affils.forEach((affilRaw) => {
+        affils.forEach((affilRaw: unknown) => {
           if (typeof(affilRaw) === "string") {
             affiliations.push(affilRaw);
+          // eslint-disable-next-line no-constant-condition
           } else if (typeof(affilRaw === "object")) {
             const affilRecord = affilRaw as Record<string, unknown>;
             const name = affilRecord.name;
             if (typeof(name) === "string") {
               affiliations.push(name);
             }
           }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/index.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/index.ts`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
 import gridTableRule from "./rules/gridtable";
 
 export default function gridTableRulePlugin(
-    md: any,
-    options: any)
+    // eslint-disable-next-line @typescript-eslint/no-explicit-any
+    md: any)
 {
     md.block.ruler.before(
         "table",
         "gridtable",
         gridTableRule(md));
 }
```

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/gridtables/GetCells.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/gridtables/GetCells.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/EmitTable.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/EmitTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/GetLine.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/GetLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/ParseTable.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/ParseTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/interfaces/markdown-it/IState.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/interfaces/markdown-it/IState.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/gridtables/rules/gridtable.ts` & `jupyterlab_quarto-0.1.42/src/plugins/gridtables/rules/gridtable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/plugins/mermaid/index.ts` & `jupyterlab_quarto-0.1.42/src/plugins/mermaid/index.ts`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,50 @@
+/* eslint-disable @typescript-eslint/no-explicit-any */
 import MarkdownIt from "markdown-it";
 import Mermaid from "mermaid";
 
-export default function mermaidPlugin(md: MarkdownIt, options: any) {
+export default function mermaidPlugin(md: MarkdownIt, options: { dark?: boolean}) {
 
 
   const kLang = "mermaid";
   const kContainer = "quarto-mermaid";
 
   Mermaid.initialize({
     securityLevel: "loose",
+    theme: options.dark ? "dark" : "default",
     ...options,
   });
 
-  let defaultFenceRenderer = md.renderer.rules.fence;
+  const defaultFenceRenderer = md.renderer.rules.fence;
 
   // Render custom code types as SVGs, letting the fence parser do all the heavy lifting.
   function mermaidFenceRenderer(
     tokens: any[],
     idx: number,
     options: any,
     env: any,
     slf: any
   ) {
-    let token = tokens[idx];
+    const token = tokens[idx];
     if (token.info === kLang || (token.attrs !== null && token.attrs.length === 1 && token.attrs[0][0] === kLang))  {
-      let imageHTML: string = "";
-      let imageAttrs: string[][] = [];
+      let imageHTML = "";
+      const imageAttrs: string[][] = [];
   
       // Create element to render into
       const element = document.createElement("div");
       document.body.appendChild(element);
   
       // Render with Mermaid
       try {
         Mermaid.mermaidAPI.render(
           kContainer,
           token.content,
           (html: string) => {
             // We need to forcibly extract the max-width/height attributes to set on img tag
-            let mermaidEl = document.getElementById(kContainer);
+            const mermaidEl = document.getElementById(kContainer);
             if (mermaidEl !== null) {
               imageAttrs.push([
                 "style",
                 `max-width:${mermaidEl.style.maxWidth};max-height:${mermaidEl.style.maxHeight}`,
               ]);
             }
             // Store HTML
```

### Comparing `jupyterlab_quarto-0.1.41/src/providers/divs.ts` & `jupyterlab_quarto-0.1.42/src/providers/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/providers/math.ts` & `jupyterlab_quarto-0.1.42/src/providers/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/providers/provider.ts` & `jupyterlab_quarto-0.1.42/src/providers/provider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/utils/html.ts` & `jupyterlab_quarto-0.1.42/src/plugins/utils/html.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/src/utils/markdownit.ts` & `jupyterlab_quarto-0.1.42/src/plugins/utils/markdownit.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/style/base.css` & `jupyterlab_quarto-0.1.42/style/base.css`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,18 @@
 }
 
 .callout-title-container {
   font-size: 1em;
   font-weight: 600;
 }
 
+body[data-jp-theme-light="false"] .callout-title-container {
+  color: var(--jp-input-background);
+}
+
 .callout.callout-style-default  div.callout-title {
   border-bottom: none;
   font-weight: 600;
   opacity: 85%;
   font-size: 0.9rem;
   padding-left: 0.5em;
   padding-right: 0.5em;
```

### Comparing `jupyterlab_quarto-0.1.41/LICENSE` & `jupyterlab_quarto-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/README.md` & `jupyterlab_quarto-0.1.42/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # JupyterLab Quarto Extension
 
 [Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more. 
 
 The JupyterLab Quarto extension allows JupyterLab to render notebooks which include Quarto markdown content.
-
-&nbsp;
+<br/><br/>
 <p align="center">
-<img src="https://user-images.githubusercontent.com/261654/229227775-9b1cb1d7-36a6-4ad0-926a-bf8d3293d858.png" width="60%">
+<img src="https://user-images.githubusercontent.com/261654/230087634-d5027ebc-8508-43b4-81c9-c4b7d6cfa738.png" width="60%">
 </p>
 
 ## Requirements
 
 - JupyterLab >= 3.0
 
 ## Install
```

### Comparing `jupyterlab_quarto-0.1.41/pyproject.toml` & `jupyterlab_quarto-0.1.42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.1.41/PKG-INFO` & `jupyterlab_quarto-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-quarto
-Version: 0.1.41
+Version: 0.1.42
 Summary: Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.
 Project-URL: Homepage, https://github.com/quarto-dev/quarto
 Project-URL: Bug Tracker, https://github.com/quarto-dev/quarto/issues/
 Project-URL: Repository, https://github.com/quarto-dev/quarto/quarto.git
 Author-email: Charles Teague <charles@posit.co>
 License: BSD 3-Clause License
         
@@ -53,18 +53,17 @@
 Description-Content-Type: text/markdown
 
 # JupyterLab Quarto Extension
 
 [Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more. 
 
 The JupyterLab Quarto extension allows JupyterLab to render notebooks which include Quarto markdown content.
-
-&nbsp;
+<br/><br/>
 <p align="center">
-<img src="https://user-images.githubusercontent.com/261654/229227775-9b1cb1d7-36a6-4ad0-926a-bf8d3293d858.png" width="60%">
+<img src="https://user-images.githubusercontent.com/261654/230087634-d5027ebc-8508-43b4-81c9-c4b7d6cfa738.png" width="60%">
 </p>
 
 ## Requirements
 
 - JupyterLab >= 3.0
 
 ## Install
```

