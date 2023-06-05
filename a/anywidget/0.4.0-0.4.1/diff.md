# Comparing `tmp/anywidget-0.4.0.tar.gz` & `tmp/anywidget-0.4.1.tar.gz`

## Comparing `anywidget-0.4.0.tar` & `anywidget-0.4.1.tar`

### file list

```diff
@@ -1,100 +1,103 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.4.0/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.4.0/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.0/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.0/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/__init__.py
--rw-r--r--   0        0        0    25080 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/138.c787b75870b3f713865b.js
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/326.3de5744b11f9f83e61f3.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/remoteEntry.53667379a2ee93d6fe11.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.0/examples/Counter.ipynb
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.4.0/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.0/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.0/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.4.1/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.4.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.1/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/__init__.py
+-rw-r--r--   0        0        0    25080 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/138.da9bcb3835f584489120.js
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/326.00a9c40e24b6392a7970.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/remoteEntry.68d0702ea589c32d2c52.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.1/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.1/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_descriptor.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.1/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.1/PKG-INFO
```

### Comparing `anywidget-0.4.0/.pre-commit-config.yaml` & `anywidget-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/package.json` & `anywidget-0.4.1/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/pnpm-lock.yaml` & `anywidget-0.4.1/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/_descriptor.py` & `anywidget-0.4.1/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/_file_contents.py` & `anywidget-0.4.1/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/_protocols.py` & `anywidget-0.4.1/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/_util.py` & `anywidget-0.4.1/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/widget.py` & `anywidget-0.4.1/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/anywidget/labextension/package.json` & `anywidget-0.4.1/anywidget/labextension/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.68d0702ea589c32d2c52.js'}}",*

 * * "'version'": "'0.4.1'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.53667379a2ee93d6fe11.js"
+            "load": "static/remoteEntry.68d0702ea589c32d2c52.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `anywidget-0.4.0/anywidget/labextension/static/138.c787b75870b3f713865b.js` & `anywidget-0.4.1/anywidget/labextension/static/138.da9bcb3835f584489120.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -92,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.0/anywidget/labextension/static/326.3de5744b11f9f83e61f3.js` & `anywidget-0.4.1/anywidget/labextension/static/326.00a9c40e24b6392a7970.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -110,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.0/anywidget/labextension/static/remoteEntry.53667379a2ee93d6fe11.js` & `anywidget-0.4.1/anywidget/labextension/static/remoteEntry.68d0702ea589c32d2c52.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, f, l, s, d, c, p, h, v = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -22,109 +22,109 @@
                     get: () => o,
                     init: () => a
                 })
             }
         },
         g = {};
 
-    function b(e) {
+    function m(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, b), t.exports
+        return v[e](t, t.exports, m), t.exports
     }
-    b.m = v, b.c = g, b.n = e => {
+    m.m = v, m.c = g, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return b.d(r, {
+        return m.d(r, {
             a: r
         }), r
-    }, b.d = (e, r) => {
-        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
+    }, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        138: "c787b75870b3f713865b",
-        326: "3de5744b11f9f83e61f3"
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
+        138: "da9bcb3835f584489120",
+        326: "00a9c40e24b6392a7970"
     } [e] + ".js?v=" + {
-        138: "c787b75870b3f713865b",
-        326: "3de5744b11f9f83e61f3"
-    } [e], b.g = function() {
+        138: "da9bcb3835f584489120",
+        326: "00a9c40e24b6392a7970"
+    } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, a) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var s = f[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, b.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        b.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        b.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                b.o(b.S, t) || (b.S[t] = {});
-                var a = b.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var a = m.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => b.e(138).then((() => () => b(138))),
+                        get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.4.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        b.g.importScripts && (e = b.g.location + "");
-        var r = b.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -147,128 +147,128 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, f = !0;; u++, i++) {
-                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == s)
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
-                            l != e[u] && (f = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    f = !1, u--
+                    l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, u--)
+                    if (u <= n || d < f != o) return !1;
+                    l = !1
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
-        var t = b.S[e];
-        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = b.I(r);
-        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, p = {
-        395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
+    }, d = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
+        395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, b.f.consumes = (e, r) => {
-        b.o(h, e) && h[e].forEach((e => {
-            if (b.o(c, e)) return r.push(c[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(h, e) && h[e].forEach((e => {
+            if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    c[e] = 0, b.m[e] = t => {
-                        delete b.c[e], t.exports = r()
+                    p[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], b.m[e] = t => {
-                        throw delete b.c[e], r
+                    delete p[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
-                var o = p[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                var o = c[e]();
+                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        b.f.j = (r, t) => {
-            var n = b.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = b.p + b.u(r),
+                    var a = m.p + m.u(r),
                         i = new Error;
-                    b.l(a, (t => {
-                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    m.l(a, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    f = 0;
+                    l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
-                    u && u(b)
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    u && u(m)
                 }
-                for (r && r(t); f < a.length; f++) o = a[f], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var m = b(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
+    var b = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
 })();
```

### Comparing `anywidget-0.4.0/anywidget/nbextension/index.js` & `anywidget-0.4.1/anywidget/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.4.0";
+var version = "0.4.1";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.4.0/docs/README.md` & `anywidget-0.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/astro.config.mjs` & `anywidget-0.4.1/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/package.json` & `anywidget-0.4.1/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/anywidget-overview.png` & `anywidget-0.4.1/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/banner-dark.png` & `anywidget-0.4.1/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/banner-light.png` & `anywidget-0.4.1/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/banner-minimal.png` & `anywidget-0.4.1/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/client-js-diagram.png` & `anywidget-0.4.1/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/default-og-image.png` & `anywidget-0.4.1/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/favicon.svg` & `anywidget-0.4.1/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/public/widget-overview.png` & `anywidget-0.4.1/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/scripts/ipynb.mjs` & `anywidget-0.4.1/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/scripts/utils.mjs` & `anywidget-0.4.1/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/consts.ts` & `anywidget-0.4.1/docs/src/consts.ts`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 		Guide: [
 			{ text: "Getting Started", link: "en/getting-started" },
 			{
 				text: "Jupyter Widgets: The Good Parts",
 				link: "en/jupyter-widgets-the-good-parts",
 			},
 			{ text: "Advanced: Bundling", link: "en/bundling" },
+			{ text: "Advanced: Experimental Features", link: "en/experimental" },
 		],
 		Notebooks: [
 			{ text: "Build a Counter Widget", link: "en/notebooks/counter" },
 		],
 		Blog: [
 			{ text: "Introducing anywidget", link: "blog/introducing-anywidget" },
 			{ text: "Modern Web Meets Jupyter", link: "blog/anywidget-02" },
```

### Comparing `anywidget-0.4.0/docs/src/components/CodeHero.astro` & `anywidget-0.4.1/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/CounterButton.astro` & `anywidget-0.4.1/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/HeadCommon.astro` & `anywidget-0.4.1/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/HeadSEO.astro` & `anywidget-0.4.1/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Hero.astro` & `anywidget-0.4.1/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.4.1/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.4.1/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.4.1/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/Header.astro` & `anywidget-0.4.1/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/HeaderButton.css` & `anywidget-0.4.1/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.4.1/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.4.1/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/Search.css` & `anywidget-0.4.1/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/Search.tsx` & `anywidget-0.4.1/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.4.1/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.4.1/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.4.1/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.4.1/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.4.1/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.4.1/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/components/examples/Counter.astro` & `anywidget-0.4.1/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/layouts/MainLayout.astro` & `anywidget-0.4.1/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/layouts/SplashLayout.astro` & `anywidget-0.4.1/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.4.1/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.4.1/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/en/bundling.md` & `anywidget-0.4.1/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/en/getting-started.mdx` & `anywidget-0.4.1/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.4.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.4.1/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/styles/index.css` & `anywidget-0.4.1/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/docs/src/styles/theme.css` & `anywidget-0.4.1/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/examples/Counter.ipynb` & `anywidget-0.4.1/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/examples/minimal_example.ipynb` & `anywidget-0.4.1/examples/minimal_example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992766203703703%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, '\\n'), (9, '\\n')]}}, 4: {'source': {insert: [(1, "*

 * *            "'\\n'), (5, '\\n')]}}}"}*

```diff
@@ -51,21 +51,23 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# +++ inline esm +++\n",
                 "\n",
+                "\n",
                 "class Widget1(anywidget.AnyWidget):\n",
                 "    _esm = \"\"\"\n",
                 "    export function render(view) {\n",
                 "        console.log(\"Hello World 1\")\n",
                 "    }\n",
                 "    \"\"\"\n",
                 "\n",
+                "\n",
                 "Widget1()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "28017701",
@@ -107,17 +109,19 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# and now in action!\n",
                 "\n",
+                "\n",
                 "class Widget2(anywidget.AnyWidget):\n",
                 "    _esm = pathlib.Path(\"index.js\")\n",
                 "\n",
+                "\n",
                 "Widget2()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6d87aaa3",
```

### Comparing `anywidget-0.4.0/packages/anywidget/CHANGELOG.md` & `anywidget-0.4.1/packages/anywidget/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # anywidget
 
+## 0.4.1
+
+### Patch Changes
+
+- feat: Add `anywidget.experimental` with simple decorator ([#126](https://github.com/manzt/anywidget/pull/126))
+
+  ```python
+  import dataclasses
+  import psygnal
+
+  from anywidget.experimental import widget
+
+  @widget(esm="index.js")
+  @psygnal.evented
+  @dataclasses.dataclass
+  class Counter:
+      value: int = 0
+  ```
+
 ## 0.4.0
 
 ### Minor Changes
 
 - feat: Add support for evented msgspec.Struct objects ([#64](https://github.com/manzt/anywidget/pull/64))
 
   Our experimental descriptor API can now work with [`msgspec`](https://jcristharif.com/msgspec/), a fast and efficient serialization library, similar to `pydantic` but with a stronger emphasis on ser/de, and less on runtime casting of Python types.
```

### Comparing `anywidget-0.4.0/packages/anywidget/build.mjs` & `anywidget-0.4.1/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/packages/anywidget/package.json` & `anywidget-0.4.1/packages/anywidget/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `anywidget-0.4.0/packages/anywidget/src/widget.js` & `anywidget-0.4.1/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/tests/test_descriptor.py` & `anywidget-0.4.1/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/tests/test_file_contents.py` & `anywidget-0.4.1/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/tests/test_utils.py` & `anywidget-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/tests/test_widget.py` & `anywidget-0.4.1/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/LICENSE` & `anywidget-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/README.md` & `anywidget-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/pyproject.toml` & `anywidget-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.0/PKG-INFO` & `anywidget-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.4.0
+Version: 0.4.1
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```

