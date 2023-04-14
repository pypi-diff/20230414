# Comparing `tmp/anywidget-0.2.0.tar.gz` & `tmp/anywidget-0.2.1.tar.gz`

## Comparing `anywidget-0.2.0.tar` & `anywidget-0.2.1.tar`

### file list

```diff
@@ -1,100 +1,101 @@
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 anywidget-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget.json
--rw-r--r--   0        0        0   210887 2020-02-02 00:00:00.000000 anywidget-0.2.0/package-lock.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 anywidget-0.2.0/package.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.2.0/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/__init__.py
--rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/_protocols.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/widget.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/static/138.4bd7cb53737d30807601.js
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/static/326.a867e75c0560aa73b7c0.js
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/static/remoteEntry.8e9b07cc14c422c7860c.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 anywidget-0.2.0/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/astro.config.mjs
--rw-r--r--   0        0        0   231058 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/package-lock.json
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10650 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.2.0/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.2.0/examples/Counter.ipynb
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 anywidget-0.2.0/scripts/prepack.mjs
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.2.0/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.2.0/src/plugin.js
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 anywidget-0.2.0/src/types.d.ts
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 anywidget-0.2.0/src/vite-plugin.js
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 anywidget-0.2.0/src/widget.js
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.2.0/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.2.0/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.2.0/tests/test_protocols.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 anywidget-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 anywidget-0.2.0/tests/test_widget.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 anywidget-0.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.2.0/LICENSE
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 anywidget-0.2.0/README.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 anywidget-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 anywidget-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 anywidget-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.2.1/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.2.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.2.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.2.1/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/__init__.py
+-rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/138.4955823d1827e11e8ec1.js
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/326.1ce804f5af553a793872.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/remoteEntry.d443ca0ab408b6568c07.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.2.1/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.2.1/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_descriptor.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_protocols.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.2.1/README.md
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 anywidget-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 anywidget-0.2.1/PKG-INFO
```

### Comparing `anywidget-0.2.0/.pre-commit-config.yaml` & `anywidget-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/CHANGELOG.md` & `anywidget-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/anywidget/_descriptor.py` & `anywidget-0.2.1/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/anywidget/_file_contents.py` & `anywidget-0.2.1/anywidget/_file_contents.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,15 +63,21 @@
         Blocks indefinitely.
 
         Returns
         -------
         changes : Iterator[tuple[int, str]]
             An iterator that yields any time the file changes until the file is deleted.
         """
-        from watchfiles import Change, watch
+        try:
+            from watchfiles import Change, watch
+        except ImportError as exc:
+            raise ImportError(
+                "watchfiles is required to watch for file changes during development. "
+                "Install with `pip install watchfiles`."
+            ) from exc
 
         for changes in watch(self._path, stop_event=self._stop_event):
             for change, path in changes:
                 if change == Change.deleted:
                     self.deleted.emit()
                     return
                 # Only getting Change.added events on macOS so we listen for either
```

### Comparing `anywidget-0.2.0/anywidget/_protocols.py` & `anywidget-0.2.1/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/anywidget/_util.py` & `anywidget-0.2.1/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/anywidget/widget.py` & `anywidget-0.2.1/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/anywidget/labextension/static/138.4bd7cb53737d30807601.js` & `anywidget-0.2.1/anywidget/labextension/static/138.4955823d1827e11e8ec1.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -88,11 +88,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.0/anywidget/labextension/static/326.a867e75c0560aa73b7c0.js` & `anywidget-0.2.1/anywidget/labextension/static/326.1ce804f5af553a793872.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkanywidget = self.webpackChunkanywidget || []).push([
     [326], {
         326: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => d
             });
-            var n = i(98),
+            var n = i(395),
                 a = i(203),
                 s = i(147);
             const d = {
                 id: `${s.u2}:plugin`,
                 requires: [n.IJupyterWidgetRegistry],
                 activate: (e, t) => {
                     let i = (0, a.Z)(n);
@@ -106,11 +106,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.0/anywidget/labextension/static/remoteEntry.8e9b07cc14c422c7860c.js` & `anywidget-0.2.1/anywidget/labextension/static/remoteEntry.d443ca0ab408b6568c07.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, d, l, f, s, p, c, h, v = {
-            770: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v = {
+            408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => i
+                    init: () => a
                 })
             }
         },
         g = {};
 
     function m(e) {
         var r = g[e];
@@ -41,49 +41,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "4bd7cb53737d30807601",
-        326: "a867e75c0560aa73b7c0"
+        138: "4955823d1827e11e8ec1",
+        326: "1ce804f5af553a793872"
     } [e] + ".js?v=" + {
-        138: "4bd7cb53737d30807601",
-        326: "a867e75c0560aa73b7c0"
+        138: "4955823d1827e11e8ec1",
+        326: "1ce804f5af553a793872"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, i) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
+            var i, u;
             if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
-                    var f = d[l];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        a = f;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var s = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), u && document.head.appendChild(a)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -93,26 +93,26 @@
             r = {};
         m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 m.o(m.S, t) || (m.S[t] = {});
-                var i = m.S[t],
-                    a = "anywidget",
+                var a = m.S[t],
+                    i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = i[e] = i[e] || {},
+                    var o = a[e] = a[e] || {},
                         u = o[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
+                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
-                        from: a,
+                        from: i,
                         eager: !1
                     })
-                })("anywidget", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.2.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -127,93 +127,98 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
-            var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                u = (typeof i)[0];
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return d();
+        return l();
 
-        function d() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+        function l() {
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, d = !0;; u++, a++) {
-                var l, f, s = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (f = (typeof(l = r[a]))[0])) return !d || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == f) {
-                    if (!d || "u" != s) return !1
-                } else if (d)
-                    if (s == f)
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
+                } else if (l)
+                    if (f == d)
                         if (u <= n) {
-                            if (l != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (d = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    d = !1, u--
+                    l = !1, u--
                 } else {
-                    if (u <= n || f < s != o) return !1;
-                    d = !1
-                } else "s" != s && "n" != s && (d = !1, u--)
+                    if (u <= n || d < f != o) return !1;
+                    l = !1
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
-        var i = m.I(r);
-        return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), p = {}, c = {
-        98: () => s("default", "@jupyter-widgets/base", [1, 6, 0, 1])
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
+    }, d = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
+        395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
+            [1, 5],
+            [1, 4],
+            [1, 3],
+            [1, 2], 1, 1, 1, 1
+        ])
     }, h = {
-        326: [98]
+        326: [395]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
             if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
@@ -237,33 +242,33 @@
         m.f.j = (r, t) => {
             var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var i = m.p + m.u(r),
-                        a = new Error;
-                    m.l(i, (t => {
+                    var a = m.p + m.u(r),
+                        i = new Error;
+                    m.l(a, (t => {
                         if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
-                                i = t && t.target && t.target.src;
-                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
-                    d = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) m.o(a, n) && (m.m[n] = a[n]);
+                var n, o, [a, i, u] = t,
+                    l = 0;
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
                     u && u(m)
                 }
-                for (r && r(t); d < i.length; d++) o = i[d], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = m(770);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
+    var y = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
 })();
```

### Comparing `anywidget-0.2.0/anywidget/nbextension/index.js` & `anywidget-0.2.1/anywidget/nbextension/index.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,22 @@
 // package.json
 var name = "anywidget";
-var version = "0.2.0";
+var version = "0.2.1";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
     if (prev) {
-        let newLink = prev.cloneNode();
+        let newLink = (
+            /** @type {HTMLLinkElement} */
+            prev.cloneNode()
+        );
         newLink.href = href;
         newLink.addEventListener("load", () => prev?.remove());
         prev.after(newLink);
         return;
     }
     return new Promise((resolve) => {
         let link = Object.assign(document.createElement("link"), {
@@ -69,14 +72,15 @@
     class AnyModel extends base.DOMWidgetModel {
         static model_name = "AnyModel";
         static model_module = name;
         static model_module_version = version;
         static view_name = "AnyView";
         static view_module = name;
         static view_module_version = version;
+        /** @param {Parameters<InstanceType<base["DOMWidgetModel"]>["initialize"]>} args */
         initialize(...args) {
             super.initialize(...args);
             this.on("change:_css", () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] css hot updated: ${id}`);
@@ -85,15 +89,16 @@
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
                 for await (let view of Object.values(this.views ?? {})) {
                     let widget = await load_esm(this.get("_esm"));
-                    await view._anywidget_cached_cleanup();
+                    await /** @type {AnyView} */
+                    view._anywidget_cached_cleanup();
                     view.$el.empty();
                     view.stopListening(this);
                     let cleanup = await widget.render(view);
                     if (cleanup)
                         this._anywidget_cached_cleanup = cleanup;
                 }
             });
```

### Comparing `anywidget-0.2.0/docs/README.md` & `anywidget-0.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/astro.config.mjs` & `anywidget-0.2.1/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/package.json` & `anywidget-0.2.1/docs/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7487394957983193%*

 * *Differences: {"'dependencies'": "{'@astrojs/markdown-remark': '^2.1.0', 'gray-matter': '^4.0.3'}",*

 * * "'devDependencies'": "{'shiki': '^0.14.1', 'vite': '^4.1.4'}",*

 * * "'name'": "'@anywidget/docs'",*

 * * 'delete': "['version']"}*

```diff
@@ -1,37 +1,40 @@
 {
     "dependencies": {
         "@algolia/client-search": "^4.13.1",
+        "@astrojs/markdown-remark": "^2.1.0",
         "@astrojs/mdx": "^0.15.1",
         "@astrojs/preact": "^2.0.0",
         "@astrojs/react": "^2.0.1",
         "@astrojs/tailwind": "^3.0.0",
         "@docsearch/css": "^3.1.0",
         "@docsearch/react": "^3.1.0",
         "@types/node": "^18.0.0",
         "@types/react": "^17.0.45",
         "@types/react-dom": "^18.0.0",
         "astro": "^2.0.2",
+        "gray-matter": "^4.0.3",
         "preact": "^10.7.3",
         "react": "^18.1.0",
         "react-dom": "^18.1.0",
         "tailwindcss": "^3.2.4"
     },
     "devDependencies": {
         "html-escaper": "^3.0.3",
         "prettier": "^2.8.2",
-        "prettier-plugin-astro": "^0.7.2"
+        "prettier-plugin-astro": "^0.7.2",
+        "shiki": "^0.14.1",
+        "vite": "^4.1.4"
     },
-    "name": "@example/docs",
+    "name": "@anywidget/docs",
     "private": true,
     "scripts": {
         "astro": "astro",
         "build": "astro build",
         "check": "astro check && tsc",
         "dev": "astro dev",
         "format": "prettier --ignore-path=../.gitignore --use-tabs --write .",
         "preview": "astro preview",
         "start": "astro dev"
     },
-    "type": "module",
-    "version": "0.0.1"
+    "type": "module"
 }
```

### Comparing `anywidget-0.2.0/docs/public/anywidget-overview.png` & `anywidget-0.2.1/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/banner-dark.png` & `anywidget-0.2.1/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/banner-light.png` & `anywidget-0.2.1/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/banner-minimal.png` & `anywidget-0.2.1/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/client-js-diagram.png` & `anywidget-0.2.1/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/default-og-image.png` & `anywidget-0.2.1/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/favicon.svg` & `anywidget-0.2.1/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/public/widget-overview.png` & `anywidget-0.2.1/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/scripts/ipynb.mjs` & `anywidget-0.2.1/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/scripts/utils.mjs` & `anywidget-0.2.1/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/consts.ts` & `anywidget-0.2.1/docs/src/consts.ts`

 * *Files 1% similar despite different names*

```diff
@@ -56,11 +56,11 @@
 			{ text: "Advanced: Bundling", link: "en/bundling" },
 		],
 		Notebooks: [
 			{ text: "Build a Counter Widget", link: "en/notebooks/counter" },
 		],
 		Blog: [
 			{ text: "Introducing anywidget", link: "blog/introducing-anywidget" },
-			{ text: "Modern Web Meets Juptyer", link: "blog/anywidget-02" },
+			{ text: "Modern Web Meets Jupyter", link: "blog/anywidget-02" },
 		],
 	},
 };
```

### Comparing `anywidget-0.2.0/docs/src/components/CodeHero.astro` & `anywidget-0.2.1/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/CounterButton.astro` & `anywidget-0.2.1/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/HeadCommon.astro` & `anywidget-0.2.1/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/HeadSEO.astro` & `anywidget-0.2.1/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Hero.astro` & `anywidget-0.2.1/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.2.1/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.2.1/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.2.1/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/Header.astro` & `anywidget-0.2.1/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/HeaderButton.css` & `anywidget-0.2.1/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.2.1/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.2.1/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/Search.css` & `anywidget-0.2.1/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/Search.tsx` & `anywidget-0.2.1/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.2.1/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.2.1/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.2.1/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.2.1/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.2.1/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.2.1/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/components/examples/Counter.astro` & `anywidget-0.2.1/docs/src/components/examples/Counter.astro`

 * *Files 16% similar despite different names*

```diff
@@ -35,37 +35,54 @@
 <CodeHero
 	filename="mywidget/__init__.py"
 	lang="python"
 	code={widgetCode}
 	url={"localhost:8888/Demo.ipynb"}
 	showGrid={false}
 >
-	<div class="text-sm bg-transparent flex flex-col space-y-4">
-		<pre
-			class="bg-transparent p-2 rounded border border-gray-400 col-span-4 w-full">{notebookCode}</pre>
+	<div class="text-sm flex-col space-y-4">
 
-		<div class="col-span-4">
+		<button id="input-1" class="hover:border-gray-50 w-full rounded border border-solid border-gray-400 text-left text-sm bg-transparent">
+			<code class="py-2 text-left whitespace-pre text-gray-200 bg-transparent">{notebookCode}</code>
+			<div class="absolute text-white top-0">Run cell</div>
+		</button>
+
+		<div>
 			<button
 				class="text-xs text-white py-2 px-4 hover:bg-primary-800 bg-primary-600 rounded shadow"
-				id="btn"
+				id="output-1"
 			>
 			</button>
 		</div>
 
-		<pre
-			class="bg-transparent col-span-4 p-2 rounded border border-gray-400 w-full">counter.value</pre>
+		<button id="input-2" class="hover:border-gray-50 w-full rounded border border-solid border-gray-400 text-left text-sm bg-transparent">
+			<code class="py-2 text-left whitespace-pre text-gray-200 bg-transparent">counter.value</code>
+		</button>
 
-		<pre class="text-sm bg-transparent pl-1 py-0" id="pyoutput"></pre>
+		<pre id="output-2" class="text-xs bg-transparent pl-1 py-0"></pre>
 	</div>
 </CodeHero>
 
 <script is:inline>
 	let count = 0;
-	let btn = document.querySelector("#btn");
-	let pyoutput = document.querySelector("#pyoutput");
+	let input1 = document.querySelector("#input-1");
+	let output1 = document.querySelector("#output-1");
+	let input2 = document.querySelector("#input-2");
+	let output2 = document.querySelector("#output-2");
+
 	function setCount(value) {
-		btn.innerHTML = `count is ${value}`;
-		pyoutput.innerHTML = value;
+		output1.innerHTML = `count is ${value}`;
 	}
-	btn.addEventListener("click", () => setCount(++count));
+
+	input1.addEventListener("click", () => {
+		setCount(count = 0);
+	});
+	output1.addEventListener("click", () => {
+		setCount(++count);
+	});
+	input2.addEventListener("click", () => {
+		output2.innerHTML = count;
+	});
+
 	setCount(0);
+	output2.innerHTML = "0";
 </script>
```

### Comparing `anywidget-0.2.0/docs/src/layouts/MainLayout.astro` & `anywidget-0.2.1/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/layouts/SplashLayout.astro` & `anywidget-0.2.1/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.2.1/docs/src/pages/blog/anywidget-02.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 ## anywidget v0.2
 
 **anywidget** v0.2 is a significant update that brings new features to dramatically
 improve the widget development experience. Some of these features have been on my
 wishlist for Jupyter for a while, and I am thrilled to finally share them!
 
-### Native Hot Module Replacement (HMR):
+### Native Hot Module Replacement (HMR)
 
 Hot Module Replacement (HMR) is a powerful tool implemented in modern
 frameworks like [Vite](https://vitejs.dev/) that enables developers to see
 changes in their application user interface without requiring full page load
 or clearing state. HMR works by updating only modules that have been modified,
 rather than refreshing the entire application. After experiencing web development
 with HMR, working with frameworks that lack this capability can be frustrating.
```

### Comparing `anywidget-0.2.0/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.2.1/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/pages/en/bundling.md` & `anywidget-0.2.1/docs/src/pages/en/bundling.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,22 @@
 optimized ESM file. This merging process is called _bundling_ and is required by
 popular fontend frameworks (e.g., React, Vue, Solid, Svelte) which use
 unsupported browser syntax.
 
 If using a bundler, make sure to load the final bundled assets in your widget
 and not the original/untransformed JavaScript source files.
 
-## Example (esbuild)
+## esbuild
 
-### Setup
+[esbuild](https://esbuild.github.io/) is very fast JavaScript bundler written in Golang. 
+It can transform **TypeScript, JSX, and CSS files** and includes zero
+JavaScrit dependencies. Binaries can be [installed without `npm`](https://esbuild.github.io/getting-started/#other-ways-to-install),
+making it a great fit for **anywidget** projects.
+
+### Project Setup
 
 The following project structure contains a python package (`hello_widget`) with
 separate JS/CSS source code under `src/`:
 
 ```bash
 hello_widget/
 ├── pyproject.toml
@@ -34,20 +39,18 @@
 └── src/
    ├── index.js
    └── styles.css
 ```
 
 ### Build
 
-We can bundle these assets into `hello_widget/static` with
-[esbuild](https://esbuild.github.io/getting-started/) without any configuration
-(or install):
+We can bundle these assets into `hello_widget/static` with `esbuild`:
 
 ```bash
-npx esbuild --bundle --format=esm --outdir=hello_widget/static src/index.js
+esbuild --bundle --format=esm --outdir=hello_widget/static src/index.js
 #
 #  hello_widget/static/index.js   150b
 #  hello_widget/static/index.css   81b
 #
 # ⚡ Done in 2ms
 ```
 
@@ -59,52 +62,63 @@
 import anywidget
 import traitlets
 
 # bundler yields hello_widget/static/{index.js,styles.css}
 bundler_output_dir = pathlib.Path(__file__).parent / "static"
 
 class HelloWidget(anywidget.AnyWidget):
-  _esm = (bundler_output_dir / "index.js").read_text()
-  _css = (bundler_output_dir / "styles.css").read_text()
+  _esm = bundler_output_dir / "index.js"
+  _css = bundler_output_dir / "styles.css"
   name = traitlets.Unicode().tag(sync=True)
 ```
 
-> **Note** `esbuild` is the most simple option for bundling, but it must be
-> executed manually each time changes are made to the JS or CSS source files in
-> order to see changes in Python. See the Vite example for a better developer
-> experience.
-
-## Example (Vite, recommended)
-
-We recommend using [Vite](https://vitejs.dev/) while developing your widget at
-this stage. It is simple to configure, and our custom _plugin_ allows for
-best-in-class developer experience.
+### Development
+
+The `esbuild` CLI also includes a "watch" mode, which tells esbuild to
+listen for changes on the file system and automatically rebuild whenever
+a file changes that could invalidate the build. **anywidget**'s
+[native HMR](/blog/anywidget-02#native-hot-module-replacement-hmr) will
+watch for changes to the re-bundled outputs from `esbuild`, swapping in
+the new bundle in the front end.
+
+```bash
+esbuild --bundle --format=esm --outdir=hello_widget/static src/index.js --watch
+```
+
 
-### Setup
+## Vite
+
+Our [Vite](https://vitejs.dev/) plugin offers a more fully featured development
+experience compared to **anywidget**'s builtin HMR, but at the cost of added
+project complexity and tooling. Vite is a good choice if you are want to
+use a front-end framework like Svelte or Vue or need more fine grain control
+over your bundling.
+
+### Project Setup
 
 From the root of the project structure above.
 
 ```bash
 npm install -D vite
 ```
 
 Create a `vite.config.js` file with the following configuration:
 
 ```javascript
 // vite.config.js
 import { defineConfig } from "vite";
 
 export default defineConfig({
-	build: {
-		outDir: "hello_widget/static",
-		lib: {
-			entry: ["src/index.js"],
-			formats: ["es"],
-		},
-	},
+  build: {
+    outDir: "hello_widget/static",
+    lib: {
+      entry: ["src/index.js"],
+      formats: ["es"],
+    },
+  },
 });
 ```
 
 Your project structure should now look like:
 
 ```bash
 hello_widget/
@@ -130,37 +144,19 @@
 npx vite build
 # vite v4.0.4 building for production...
 # ✓ 2 modules transformed.
 # hello_widget/static/style.css  0.05 kB │ gzip: 0.06 kB
 # hello_widget/static/index.mjs  0.13 kB │ gzip: 0.14 kB
 ```
 
-So far, this example demonstrates Vite's bundling capabilities which are similar
-to esbuild. However, Vite really shines during _development_ with its second
-major feature: a modern development server that enables extremely fast
-[Hot Module Replacement (HMR)](https://vitejs.dev/guide/features.html#hot-module-replacement).
-
 ### Development
 
-Frontend development tools have evolved rapidly in the last few years to enable
-instant, precise updates to client code without reloading the page or blowing
-away application state. Unfortunately, the cookiecutter templates for custom
-Jupyter Widgets have not caught up with the times and still require full page
-loads and re-bundles to see new changes.
-
-_This all changes with **anywidget**_
-
 The Vite plugin for **anywidget** extends its dev server with precise HMR
-support for Jupyter Widgets. During development, changes made to your widget
-view are **instantly** reflected in all active output cells without a full page
-refresh. Model state is additionally preserved so you do not need to re-run the
-Python cell to setup state.
-
-To get started with HMR for your widget, install the `anywidget` Plugin and add
-the following to your `vite.config.js`:
+support for Jupyter Widgets. To get started with HMR for your widget,
+install the `anywidget` Plugin and add the following to your `vite.config.js`:
 
 ```bash
 npm install -D anywidget
 ```
 
 ```diff
 // vite.config.js
```

### Comparing `anywidget-0.2.0/docs/src/pages/en/getting-started.mdx` & `anywidget-0.2.1/docs/src/pages/en/getting-started.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - Prototype **within** `.ipynb` or `.py` files
 - Run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
 - Develop (optionally) with [Vite](https://vitejs.dev/) for **instant HMR**
 
 ## Example
 
 ```
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 ```python
 import anywidget
 import traitlets
 
 class CounterWidget(anywidget.AnyWidget):
@@ -63,43 +63,43 @@
 counter
 ```
 
 <CounterButton size={"lg"} initialValue={42} />
 
 What's going on here:
 
-- `value` is a stateful property for that both the client JavaScript and Python have access to.
+- `count` is a stateful property for that both the client JavaScript and Python have access to.
   Shared state is defined via [traitlets](https://traitlets.readthedocs.io/en/stable/) with the `sync=True`
   keyword argument.
 
 - `_css` specifies an <u>**optional**</u> CSS stylesheet to load for the widget. It can be a full URL or plain text. Styles are loaded
   in the global scope if using this feature, so take care in avoid global overrides.
 
 - `_esm` specifies a <u>**required**</u> [ECMAScript module](https://nodejs.org/api/esm.html) for the widget.
   It must _must_ export a `render` custom rendering logic and initializes dynamic updates for the custom widget.
 
 ```javascript
 /** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
 export function render(view) {
-	// Render model contents and setup dynamic updates
-	// See Jupyter widgets docs for more information: https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Rendering-model-contents
+  // Render model contents and setup dynamic updates
+  // See Jupyter widgets docs for more information: https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Rendering-model-contents
 }
 ```
 
 ECMAScript modules are the offical standard format to package JavaScript code for reuse and are supported
 natively across [all major browsers](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#javascript.statements.export).
 Therefore, dependencies can be imported directly via a fully qualified URL.
 
 ```javascript
 import * as d3 from "https://esm.sh/d3@7";
 
 /** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
 export function render(view) {
-	let selection = d3.select(view.el);
-	/* ... */
+  let selection = d3.select(view.el);
+  /* ... */
 }
 ```
 
 The `render` function can also (optionally) return a callback that is executed any time the view is
 removed from the DOM. This feature is useful when dealing with complex event listeners, subscriptions,
 or third-party libraries that require proper teardwon.
```

### Comparing `anywidget-0.2.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.2.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,40 +27,38 @@
 
 Concretely, custom widgets are traditionally defined like:
 
 ```javascript
 import { DOMWidgetModel, DOMWidgetView } from "@jupyter-widgets/base";
 
 // All boilerplate, anywidget takes care of this ...
-class CustomModel extends DOMWidgetModel {
-	/* ... */
-}
+class CustomModel extends DOMWidgetModel { /* ... */ }
 
 class CustomView extends DOMWidgetView {
-	render() {
-		let view = this;
-		let el = this.el;
-		let model = this.model;
-		/* ... */
-	}
+  render() {
+    let view = this;
+    let el = this.el;
+    let model = this.model;
+    /* ... */
+  }
 }
 
 export { CustomModel, CustomView };
 ```
 
 ... which must be transformed, bundled, and installed in multiple notebook environments.
 
 In **anywidget**, the above code simplies to just:
 
 ```javascript
 /** @param view {DOMWidgetView} view */
 export function render(view) {
-	let el = view.el;
-	let model = view.model;
-	/* ... */
+  let el = view.el;
+  let model = view.model;
+  /* ... */
 }
 ```
 
 ... which explicity defines the widget view (i.e., `CustomView`) via the `render`
 function, and (implicitly) **anywidget** defines the associated widget
 model (i.e., `CustomModel`). **anywidget** front-end code is often so
 minimal that it can easily be inlined as a Python string:
@@ -88,62 +86,62 @@
    (i.e., passing callbacks to `view.model.on`)
 
 ## Connecting JavaScript with Python
 
 The Jupyter Widgets framework is build on top of the IPython Comm framework (short for communication).
 It's worth reading the [_Low Level Widget Explanation_](https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Low%20Level.html#Low-Level-Widget-Explanation)
 to understand the core of Jupyter Widget's Model, View, Controller (MVC) architecture, but in
-short the Comm framework exposes to mechanisms to send/receive data to/from the frond end:
+short the Comm framework exposes two mechanisms to send/receive data to/from the frond end:
 
 ### 1. Traitlets
 
 [`traitlets`](https://traitlets.readthedocs.io/en/stable/using_traitlets.html)
 are the easiest and most flexible way to synchronize data between the
 front end and Python. The `sync=True` keyword argument tells the widget
 framework to handle synchronizing that value to the front end. Take the following
 `CustomWidget`:
 
 ```python
-class CustomWidget(anywidget.Widget):
+class CustomWidget(anywidget.AnyWidget):
     _esm = (pathlib.Path(__file__).parent / "index.js").read_text()
     my_value = traitlets.Int(0).tag(sync=True)
 ```
 
 It defines an Integer `my_value` trait, which is synchronized with the front
 end. The `render` function now has the ability to:
 
 - **get** `my_value`
 
 ```javascript
 // index.js
 export function render(view) {
-	let my_value = view.model.get("my_value");
+  let my_value = view.model.get("my_value");
 }
 ```
 
 - **set** `my_value`
 
 ```javascript
 // index.js
 export function render(view) {
-	view.model.set("my_value", 42);
-	view.model.save_changes(); // required to send update to Python
+  view.model.set("my_value", 42);
+  view.model.save_changes(); // required to send update to Python
 }
 ```
 
 - **listen for changes to** `my_value` (and register event handlers)
 
 ```javascript
 // index.js
 export function render(view) {
-	function on_change() {
-		let new_my_value = view.model.get("my_value");
-		console.log(`The 'my_value' changed to: ${new_my_value}`);
-	}
-	view.model.on("change:my_value", on_change);
+  function on_change() {
+    let new_my_value = view.model.get("my_value");
+    console.log(`The 'my_value' changed to: ${new_my_value}`);
+  }
+  view.model.on("change:my_value", on_change);
 }
 ```
 
 > **Note**: In the snippet above, `on_change` is called an _**event handler**_
 > because it executes any time `my_value` is updated from either Python or the
 > front-end code (i.e., a _change_ event).
```

### Comparing `anywidget-0.2.0/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.2.1/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/styles/index.css` & `anywidget-0.2.1/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/docs/src/styles/theme.css` & `anywidget-0.2.1/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/examples/Counter.ipynb` & `anywidget-0.2.1/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/scripts/prepack.mjs` & `anywidget-0.2.1/packages/anywidget/build.mjs`

 * *Files 25% similar despite different names*

```diff
@@ -3,39 +3,34 @@
 import * as path from "node:path";
 import * as url from "node:url";
 
 import * as esbuild from "esbuild";
 
 let __dirname = path.dirname(url.fileURLToPath(import.meta.url));
 
-let src = path.join(__dirname, "..", "src");
-let dist = path.join(__dirname, "..", "dist");
+let src = path.join(__dirname, "src");
+let dist = path.join(__dirname, "dist");
 
-// bundle the widget
 await esbuild.build({
 	entryPoints: [path.join(src, "index.js")],
 	bundle: true,
 	format: "esm",
 	outfile: path.join(dist, "index.js"),
 });
 
-// Just copy over the ESM
-await fs.copyFile(
-	path.join(src, "vite-plugin.js"),
+// re-export all exports from @anywidget/vite
+await fs.writeFile(
 	path.join(dist, "vite.mjs"),
+	`export * from "@anywidget/vite";`,
+);
+await fs.writeFile(
+	path.join(dist, "vite.cjs"),
+	`module.exports = require("@anywidget/vite");`,
 );
 
-// Transform the vite plugin to CJS
-await esbuild.build({
-	entryPoints: [path.join(src, "vite-plugin.js")],
-	format: "cjs",
-	outfile: path.join(dist, "vite.cjs"),
-});
-
-
-// Copy over the types and create empty files
-await fs.copyFile(
-	path.join(src, "types.d.ts"),
+// re-export all exports from @anywidget/types
+await fs.writeFile(
 	path.join(dist, "types.d.ts"),
+	`export * from "@anywidget/types";`,
 );
 await fs.writeFile(path.join(dist, "types.mjs"), "");
 await fs.writeFile(path.join(dist, "types.cjs"), "");
```

### Comparing `anywidget-0.2.0/src/widget.js` & `anywidget-0.2.1/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/tests/test_descriptor.py` & `anywidget-0.2.1/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/tests/test_file_contents.py` & `anywidget-0.2.1/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/tests/test_utils.py` & `anywidget-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/tests/test_widget.py` & `anywidget-0.2.1/tests/test_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 import pytest
 import traitlets.traitlets as t
 import watchfiles
 from anywidget._file_contents import FileContents
 from anywidget._util import _DEFAULT_ESM, _WIDGET_MIME_TYPE
 from watchfiles import Change
 
+here = pathlib.Path(__file__).parent
+
 
 def test_version():
-    with open(pathlib.Path(__file__).parent / "../package.json") as f:
+    with open(here / "../packages/anywidget/package.json") as f:
         pkg = json.load(f)
 
     assert anywidget.__version__ == pkg["version"]
 
 
 def test_basic():
     ESM = """
```

### Comparing `anywidget-0.2.0/LICENSE` & `anywidget-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.0/README.md` & `anywidget-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 custom jupyter widgets made easy
 
 - 🛠️ create widgets **without complicated cookiecutter templates**
 - 📚 **publish to PyPI** like any other Python package
 - 🤖 prototype **within** `.ipynb` or `.py` files
 - 🚀 run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
-- ⚡ develop (optionally) with [Vite](https://vitejs.dev/) for **instant HMR**
+- ⚡ develop with **instant HMR**, like modern web frameworks
 
 Learn more in
 [the announcement](https://anywidget.dev/blog/introducing-anywidget).
 
 ## Installation
 
 > **Warning**: **anywidget** is new and under active development. It is not yet
 > ready for production as APIs are subject to change.
 
 **anywidget** is available on [PyPI](https://pypi.org/project/anywidget/) and
 may be installed with `pip`:
 
 ```bash
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 It is also available on
 [conda-forge](https://anaconda.org/conda-forge/anywidget). If you have
 [Anaconda](https://www.anaconda.com/distribution/#download-section) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your
 computer, you can install **anywidget** with the following command:
@@ -61,21 +61,50 @@
       view.el.appendChild(button);
     }
     """
     # Stateful property that can be accessed by JavaScript & Python
     count = traitlets.Int(0).tag(sync=True)
 ```
 
+Front-end code can also live in separate files (recommend):
+
+```python
+import pathlib
+import anywidget
+import traitlets
+
+class CounterWidget(anywidget.AnyWidget):
+    _esm = pathlib.Path("index.js")
+    _css = pathlib.Path("styles.css")
+
+    count = traitlets.Int(0).tag(sync=True)
+```
+
 Read [the documentation](https://anywidget.dev/en/getting-started) to learn
 more.
 
-## Development
+## Contributing
+
+This is a monorepo, meaning the repo holds multiple packages. It requires the use of [pnpm](https://pnpm.js.org/en/).
+You can [install pnpm](https://pnpm.io/installation) with:
+
+```bash
+npm i -g pnpm
+```
+
+Then, create a Python virtual environment with a complete development install:
+
+```bash
+pip install -e ".[dev,test]"
+```
+
+or alternatively use the [`hatch`](https://github.com/pypa/hatch) CLI:
 
 ```bash
-pip install -e .
+hatch shell
 ```
 
 If you are using the classic Jupyter Notebook you need to install the
 nbextension:
 
 ```bash
 jupyter nbextension install --py --symlink --sys-prefix anywidget
```

### Comparing `anywidget-0.2.0/pyproject.toml` & `anywidget-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,51 +9,50 @@
     { name = "Trevor Manz", email = "trevor.j.manz@gmail.com" }
 ]
 license = { text = "MIT" }
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "ipywidgets",
-    "importlib_metadata ; python_version < '3.8'",
-    "typing_extensions",
-    "psygnal",
+    "ipywidgets>=7.6.0",
+    "importlib-metadata ; python_version < '3.8'",
+    "typing-extensions>=4.2.0",
+    "psygnal>=0.8.1",
 ]
 
 [project.optional-dependencies]
 test = [
     "black[jupyter]",
     "pydantic",
     "pytest",
     "pytest-cov",
     "ruff",
 ]
 dev = [
     "watchfiles",
+    "ipykernel",
 ]
 
 [project.urls]
 homepage = "https://github.com/manzt/anywidget"
 
-[tool.hatch.build]
-artifacts = [
-    "anywidget/nbextension/index.*",
-    "anywidget/labextension/*.tgz",
-    "anywidget/labextension",
-]
-
 [tool.hatch.build.targets.wheel.shared-data]
 "anywidget/nbextension" = "share/jupyter/nbextensions/anywidget"
 "anywidget/labextension" = "share/jupyter/labextensions/anywidget"
-"./anywidget.json" = "etc/jupyter/nbconfig/notebook.d/anywidget.json"
+"anywidget.json" = "etc/jupyter/nbconfig/notebook.d/anywidget.json"
 
-[tool.hatch.build.targets.sdist]
+[tool.hatch.build]
 exclude = [
     ".github",
 ]
+artifacts = [
+    "anywidget/nbextension/index.*",
+    "anywidget/labextension/*.tgz",
+    "anywidget/labextension",
+]
 
 [tool.hatch.build.hooks.jupyter-builder]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
     "anywidget/nbextension/index.js",
     "anywidget/labextension/package.json",
 ]
@@ -62,18 +61,19 @@
     "anywidget/labextension/package.json",
 ]
 dependencies = [
     "hatch-jupyter-builder>=0.5.0",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
+npm = "pnpm"
 build_cmd = "build"
 
 [tool.hatch.version]
-path = "package.json"
+path = "packages/anywidget/package.json"
 pattern = "\"version\": \"(?P<version>.+?)\""
 
 [tool.hatch.envs.default]
 features = ["test", "dev"]
 
 [tool.hatch.envs.default.scripts]
 fmt = "black ."
```

### Comparing `anywidget-0.2.0/PKG-INFO` & `anywidget-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.2.0
+Version: 0.2.1
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
-Requires-Dist: ipywidgets
-Requires-Dist: psygnal
-Requires-Dist: typing-extensions
+Requires-Dist: ipywidgets>=7.6.0
+Requires-Dist: psygnal>=0.8.1
+Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: dev
+Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black[jupyter]; extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
@@ -30,29 +31,29 @@
 
 custom jupyter widgets made easy
 
 - 🛠️ create widgets **without complicated cookiecutter templates**
 - 📚 **publish to PyPI** like any other Python package
 - 🤖 prototype **within** `.ipynb` or `.py` files
 - 🚀 run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
-- ⚡ develop (optionally) with [Vite](https://vitejs.dev/) for **instant HMR**
+- ⚡ develop with **instant HMR**, like modern web frameworks
 
 Learn more in
 [the announcement](https://anywidget.dev/blog/introducing-anywidget).
 
 ## Installation
 
 > **Warning**: **anywidget** is new and under active development. It is not yet
 > ready for production as APIs are subject to change.
 
 **anywidget** is available on [PyPI](https://pypi.org/project/anywidget/) and
 may be installed with `pip`:
 
 ```bash
-pip install anywidget
+pip install "anywidget[dev]"
 ```
 
 It is also available on
 [conda-forge](https://anaconda.org/conda-forge/anywidget). If you have
 [Anaconda](https://www.anaconda.com/distribution/#download-section) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your
 computer, you can install **anywidget** with the following command:
@@ -84,21 +85,50 @@
       view.el.appendChild(button);
     }
     """
     # Stateful property that can be accessed by JavaScript & Python
     count = traitlets.Int(0).tag(sync=True)
 ```
 
+Front-end code can also live in separate files (recommend):
+
+```python
+import pathlib
+import anywidget
+import traitlets
+
+class CounterWidget(anywidget.AnyWidget):
+    _esm = pathlib.Path("index.js")
+    _css = pathlib.Path("styles.css")
+
+    count = traitlets.Int(0).tag(sync=True)
+```
+
 Read [the documentation](https://anywidget.dev/en/getting-started) to learn
 more.
 
-## Development
+## Contributing
+
+This is a monorepo, meaning the repo holds multiple packages. It requires the use of [pnpm](https://pnpm.js.org/en/).
+You can [install pnpm](https://pnpm.io/installation) with:
+
+```bash
+npm i -g pnpm
+```
+
+Then, create a Python virtual environment with a complete development install:
+
+```bash
+pip install -e ".[dev,test]"
+```
+
+or alternatively use the [`hatch`](https://github.com/pypa/hatch) CLI:
 
 ```bash
-pip install -e .
+hatch shell
 ```
 
 If you are using the classic Jupyter Notebook you need to install the
 nbextension:
 
 ```bash
 jupyter nbextension install --py --symlink --sys-prefix anywidget
```

