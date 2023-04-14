# Comparing `tmp/antsibull_docs_parser-0.2.0.tar.gz` & `tmp/antsibull_docs_parser-0.3.0.tar.gz`

## Comparing `antsibull_docs_parser-0.2.0.tar` & `antsibull_docs_parser-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.flake8
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.pylintrc.automated
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/codecov.yml
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/noxfile.py
--rw-r--r--   0        0        0   117408 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/test-vectors.yaml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.reuse/dep5
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/__init__.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/_parser_impl.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/ansible_doc_text.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/dom.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/format.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/html.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/md.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/py.typed
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/rst.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/__init__.py
--rwxr-xr-x   0        0        0     2485 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/create-vectors.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_ansible_doc_text.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_dom.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_format.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_html.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_md.py
--rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_parser.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_parser_impl.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_rst.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/test_vectors.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/tests/unit/vectors.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/.gitignore
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/README.md
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.flake8
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.pylintrc.automated
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/codecov.yml
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/noxfile.py
+-rw-r--r--   0        0        0   139609 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/test-vectors.yaml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.reuse/dep5
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/__init__.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/_parser_impl.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/ansible_doc_text.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/dom.py
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/format.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/html.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/md.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/py.typed
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/rst.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/__init__.py
+-rwxr-xr-x   0        0        0     2586 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/create-vectors.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_ansible_doc_text.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_dom.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_format.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_html.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_md.py
+-rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_parser.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_parser_impl.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_rst.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_vectors.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/vectors.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/PKG-INFO
```

### Comparing `antsibull_docs_parser-0.2.0/.pylintrc.automated` & `antsibull_docs_parser-0.3.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/CHANGELOG.rst` & `antsibull_docs_parser-0.3.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 =================================================================================================
 antsibull-docs-parser -- Python library for processing Ansible documentation markup Release Notes
 =================================================================================================
 
 .. contents:: Topics
 
 
+v0.3.0
+======
+
+Release Summary
+---------------
+
+Feature release.
+
+Minor Changes
+-------------
+
+- Add support for plain RST rendering (https://github.com/ansible-community/antsibull-docs-parser/pull/20).
+
 v0.2.0
 ======
 
 Release Summary
 ---------------
 
 New major release that increases compatibility with the `TypeScript code in antsibull-docs-ts <https://github.com/ansible-community/antsibull-docs-ts>`__.
```

### Comparing `antsibull_docs_parser-0.2.0/LICENSE` & `antsibull_docs_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/noxfile.py` & `antsibull_docs_parser-0.3.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 def codeqa(session: nox.Session):
     install(session, ".[codeqa]", editable=True)
     session.run("flake8", "src/antsibull_docs_parser", *session.posargs)
     session.run(
         "pylint", "--rcfile", ".pylintrc.automated", "src/antsibull_docs_parser"
     )
     session.run("reuse", "lint")
+    session.run("antsibull-changelog", "lint")
 
 
 @nox.session
 def typing(session: nox.Session):
     install(session, ".[typing]", editable=True)
     session.run("mypy", "src/antsibull_docs_parser")
     session.run("pyre", "--source-directory", "src")
@@ -181,15 +182,15 @@
         "-a",
         "-m",
         f"antsibull-docs-parser {version}",
         "--edit",
         version,
         external=True,
     )
-    session.run("hatch", "build")
+    session.run("hatch", "build", "--clean")
 
 
 @nox.session
 def publish(session: nox.Session):
     check_no_modifications(session)
     install(session, "hatch")
     session.run("hatch", "publish", *session.posargs)
```

### Comparing `antsibull_docs_parser-0.2.0/test-vectors.yaml` & `antsibull_docs_parser-0.3.0/test-vectors.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -7,33 +7,37 @@
   empty:
     source: []
     html: ''
     html_plain: ''
     rst: ''
     md: ''
     ansible_doc_text: ''
+    rst_plain: ''
   empty_content:
     source: ['']
     html: <p></p>
     html_plain: <p></p>
     md: ' '
     rst: '\ '
     ansible_doc_text: ''
+    rst_plain: '\ '
   simple:
     source: |-
       This is a C(test) I(module) B(markup).
     html: |-
       <p>This is a <code class='docutils literal notranslate'>test</code> <em>module</em> <b>markup</b>.</p>
     html_plain: |-
       <p>This is a <code>test</code> <em>module</em> <b>markup</b>.</p>
     md: |-
       This is a <code>test</code> <em>module</em> <b>markup</b>.
     rst: |-
       This is a \ :literal:`test`\  \ :emphasis:`module`\  \ :strong:`markup`\ .
     ansible_doc_text: This is a `test' `module' *markup*.
+    rst_plain: This is a \ :literal:`test`\  \ :emphasis:`module`\  \ :strong:`markup`\
+      .
   module:
     source: |-
       The M(a.b.c) module.
     html: |-
       <p>The <a href='https://docs.ansible.com/ansible/devel/collections/a/b/c_module.html' class='module'>a.b.c</a> module.</p>
     html_opts:
       pluginLink.js: |-
@@ -48,26 +52,28 @@
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
     ansible_doc_text: The [a.b.c] module.
+    rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
   module_no_link:
     source: |-
       The M(a.b.c) module.
     html: |-
       <p>The <span class='module'>a.b.c</span> module.</p>
     html_plain: |-
       <p>The <span>a.b.c</span> module.</p>
     md: |-
       The a.b.c module.
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
     ansible_doc_text: The [a.b.c] module.
+    rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
   plugin:
     source: |-
       The P(a.b.c#lookup) lookup plugin.
     html: |-
       <p>The <a href='https://docs.ansible.com/ansible/devel/collections/a/b/c_lookup.html' class='module'>a.b.c</a> lookup plugin.</p>
     html_opts:
       pluginLink.js: |-
@@ -82,50 +88,56 @@
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
     ansible_doc_text: The [a.b.c] lookup plugin.
+    rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
   plugin_no_link:
     source: |-
       The P(a.b.c#lookup) lookup plugin.
     html: |-
       <p>The <span class='module'>a.b.c</span> lookup plugin.</p>
     html_plain: |-
       <p>The <span>a.b.c</span> lookup plugin.</p>
     md: |-
       The a.b.c lookup plugin.
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
     ansible_doc_text: The [a.b.c] lookup plugin.
+    rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
   link_and_url:
     source: |-
       An URL U(https://example.com) and L(a link, https://example.org).
     html: |-
       <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.</p>
     html_plain: |-
       <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.</p>
     md: |-
       An URL [https\://example.com](https\://example.com) and [a link](https\://example.org).
     rst: |-
       An URL \ https://example.com\  and \ `a link <https://example.org>`__\ .
     ansible_doc_text: An URL https://example.com and a link <https://example.org>.
+    rst_plain: An URL \ https://example.com\  and \ `a link <https://example.org>`__\
+      .
   rst_ref:
     source: |-
       A R(RST reference, ansible_collections.community.general.ufw_module).
     html: |-
       <p>A <span class='module'>RST reference</span>.</p>
     html_plain: |-
       <p>A <span>RST reference</span>.</p>
     md: |-
       A RST reference.
     rst: |-
       A \ :ref:`RST reference <ansible_collections.community.general.ufw_module>`\ .
     ansible_doc_text: A RST reference.
+    rst_plain: A \ :ref:`RST reference <ansible_collections.community.general.ufw_module>`\
+      .
   horizontal_line:
     source: |-
       foo HORIZONTALLINE bar
     html: |-
       <p>foo <hr/> bar</p>
     html_plain: |-
       <p>foo <hr> bar</p>
@@ -139,26 +151,34 @@
         <hr>
 
        bar
     ansible_doc_text: |-
       foo 
       -------------
        bar
+    rst_plain: |-
+      foo 
+
+      ------------
+
+       bar
   semantic_markup:
     source: |-
       foo E(FOOBAR) bar P(foo.bar.baz#bam) has value V( foo\),bar\\bam ).
     html: |-
       <p>foo <code class="xref std std-envvar literal notranslate">FOOBAR</code> bar <span class='module'>foo.bar.baz</span> has value <code class="ansible-value literal notranslate"> foo),bar\bam </code>.</p>
     html_plain: |-
       <p>foo <code>FOOBAR</code> bar <span>foo.bar.baz</span> has value <code> foo),bar\bam </code>.</p>
     md: |-
       foo <code>FOOBAR</code> bar foo.bar.baz has value <code> foo\)\,bar\\bam </code>.
     rst: |-
       foo \ :envvar:`FOOBAR`\  bar \ :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_bam>`\  has value \ :ansval:`\  foo),bar\\bam \ `\ .
     ansible_doc_text: foo `FOOBAR' bar [foo.bar.baz] has value ` foo),bar\bam '.
+    rst_plain: foo \ :envvar:`FOOBAR`\  bar \ :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_bam>`\  has
+      value \ :literal:`\  foo),bar\\bam \ `\ .
   option_name_no_current_plugin:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -253,14 +273,38 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   option_name_current_plugin:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -359,14 +403,38 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   option_name_current_role:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -490,14 +558,44 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   option_name_no_current_plugin_w_links:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -602,14 +700,38 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   option_name_current_plugin_w_links:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -718,14 +840,38 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   option_name_current_role_w_links:
     source:
       - |-
         O(foo) O(bar.baz[123].bam[len(x\) - 1])
       - |-
         O(foo=) O(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -859,14 +1005,44 @@
       `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint main)\ 
+
+      \ :literal:`foo` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_role>`, entrypoint other\_entrypoint)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_role>`, entrypoint main)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   return_value_no_current_plugin:
     source:
       - |-
         RV(foo) RV(bar.baz[123].bam[len(x\) - 1])
       - |-
         RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -937,14 +1113,32 @@
       `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   return_value_current_plugin:
     source:
       - |-
         RV(foo) RV(bar.baz[123].bam[len(x\) - 1])
       - |-
         RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -1019,14 +1213,32 @@
       `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   return_value_no_current_plugin_w_links:
     source:
       - |-
         RV(foo) RV(bar.baz[123].bam[len(x\) - 1])
       - |-
         RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -1107,14 +1319,32 @@
       `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   return_value_current_plugin_w_links:
     source:
       - |-
         RV(foo) RV(bar.baz[123].bam[len(x\) - 1])
       - |-
         RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=)
       - |-
@@ -1199,14 +1429,32 @@
       `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
 
       `foo' `bar.baz[123].bam[len(x) - 1]'
 
       `foo=' `bar.baz[123].bam[len(x) - 1]='
 
       `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+    rst_plain: |-
+      \ :literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam <ansible_collections.foo.bar.baz.bam_boo>`)\ 
+
+      \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo <ansible_collections.bam.baz.foo_lookup>`)\ 
+
+      \ :literal:`foo`\  \ :literal:`bar.baz[123].bam[len(x) - 1]`\ 
+
+      \ :literal:`foo=`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ 
+
+      \ :literal:`foo=bar`\  \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ 
   unhelpful_errors:
     source:
       - P(foo)
       - C(foo
       - R(foo,bar
     parse_opts:
       helpfulErrors: false
@@ -1228,14 +1476,20 @@
       \ :strong:`ERROR while parsing`\ : While parsing R() at index 1 of paragraph 3: Cannot find closing ")" after last parameter\ 
     ansible_doc_text: |-
       [[ERROR while parsing: While parsing P() at index 1 of paragraph 1: Parameter "foo" is not of the form FQCN#type]]
 
       [[ERROR while parsing: While parsing C() at index 1 of paragraph 2: Cannot find closing ")" after last parameter]]
 
       [[ERROR while parsing: While parsing R() at index 1 of paragraph 3: Cannot find closing ")" after last parameter]]
+    rst_plain: |-
+      \ :strong:`ERROR while parsing`\ : While parsing P() at index 1 of paragraph 1: Parameter "foo" is not of the form FQCN#type\ 
+
+      \ :strong:`ERROR while parsing`\ : While parsing C() at index 1 of paragraph 2: Cannot find closing ")" after last parameter\ 
+
+      \ :strong:`ERROR while parsing`\ : While parsing R() at index 1 of paragraph 3: Cannot find closing ")" after last parameter\ 
   helpful_errors:
     source:
       - P(foo)
       - C(foo
       - R(foo,bar
     html: |-
       <p><span class="error">ERROR while parsing: While parsing "P(foo)" at index 1 of paragraph 1: Parameter "foo" is not of the form FQCN#type</span></p><p><span class="error">ERROR while parsing: While parsing "C(foo" at index 1 of paragraph 2: Cannot find closing ")" after last parameter</span></p><p><span class="error">ERROR while parsing: While parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find closing ")" after last parameter</span></p>
@@ -1255,7 +1509,13 @@
       \ :strong:`ERROR while parsing`\ : While parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find closing ")" after last parameter\ 
     ansible_doc_text: |-
       [[ERROR while parsing: While parsing "P(foo)" at index 1 of paragraph 1: Parameter "foo" is not of the form FQCN#type]]
 
       [[ERROR while parsing: While parsing "C(foo" at index 1 of paragraph 2: Cannot find closing ")" after last parameter]]
 
       [[ERROR while parsing: While parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find closing ")" after last parameter]]
+    rst_plain: |-
+      \ :strong:`ERROR while parsing`\ : While parsing "P(foo)" at index 1 of paragraph 1: Parameter "foo" is not of the form FQCN#type\ 
+
+      \ :strong:`ERROR while parsing`\ : While parsing "C(foo" at index 1 of paragraph 2: Cannot find closing ")" after last parameter\ 
+
+      \ :strong:`ERROR while parsing`\ : While parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find closing ")" after last parameter\
```

#### html2text {}

```diff
@@ -1,98 +1,113 @@
 --- # Simplified BSD License (see LICENSES/BSD-2-Clause.txt or https://
 opensource.org/licenses/BSD-2-Clause) # SPDX-FileCopyrightText: Ansible Project
 # SPDX-License-Identifier: BSD-2-Clause test_vectors: empty: source: [] html:
-'' html_plain: '' rst: '' md: '' ansible_doc_text: '' empty_content: source:
-[''] html:
+'' html_plain: '' rst: '' md: '' ansible_doc_text: '' rst_plain: ''
+empty_content: source: [''] html:
 html_plain:
-md: ' ' rst: '\ ' ansible_doc_text: '' simple: source: |- This is a C(test) I
-(module) B(markup). html: |-
+md: ' ' rst: '\ ' ansible_doc_text: '' rst_plain: '\ ' simple: source: |- This
+is a C(test) I(module) B(markup). html: |-
 This is a test module markup.
 html_plain: |-
 This is a test module markup.
 md: |- This is a test module markup. rst: |- This is a \ :literal:`test`\ \ :
 emphasis:`module`\ \ :strong:`markup`\ . ansible_doc_text: This is a `test'
-`module' *markup*. module: source: |- The M(a.b.c) module. html: |-
+`module' *markup*. rst_plain: This is a \ :literal:`test`\ \ :emphasis:
+`module`\ \ :strong:`markup`\ . module: source: |- The M(a.b.c) module. html:
+|-
 The a.b.c module.
 html_opts: pluginLink.js: |- (plugin_data) => `https://docs.ansible.com/
 ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_$
 {plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" html_plain: |-
 The a.b.c module.
 md: |- The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/
 c\_module.html) module. md_opts: pluginLink.js: |- (plugin_data) => `https://
 docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/
 ')}_${plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" rst: |- The \ :ref:`a.b.c
-a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. module_no_link:
-source: |- The M(a.b.c) module. html: |-
+a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. rst_plain: The \
+:ref:`a.b.c
+a.b.c_module>`\ module. module_no_link: source: |- The M(a.b.c) module. html:
+|-
 The a.b.c module.
 html_plain: |-
 The a.b.c module.
 md: |- The a.b.c module. rst: |- The \ :ref:`a.b.c
-a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. plugin: source:
-|- The P(a.b.c#lookup) lookup plugin. html: |-
+a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. rst_plain: The \
+:ref:`a.b.c
+a.b.c_module>`\ module. plugin: source: |- The P(a.b.c#lookup) lookup plugin.
+html: |-
 The a.b.c lookup plugin.
 html_opts: pluginLink.js: |- (plugin_data) => `https://docs.ansible.com/
 ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_$
 {plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" html_plain: |-
 The a.b.c lookup plugin.
 md: |- The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/
 c\_lookup.html) lookup plugin. md_opts: pluginLink.js: |- (plugin_data) =>
 `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace
 (/\./g, '/')}_${plugin_data.type}.html` pluginLink.py: |- lambda plugin_data:
 f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace
 ('.', '/')}_{plugin_data.type}.html" rst: |- The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. ansible_doc_text: The [a.b.c] lookup plugin.
-plugin_no_link: source: |- The P(a.b.c#lookup) lookup plugin. html: |-
+rst_plain: The \ :ref:`a.b.c
+a.b.c_lookup>`\ lookup plugin. plugin_no_link: source: |- The P(a.b.c#lookup)
+lookup plugin. html: |-
 The a.b.c lookup plugin.
 html_plain: |-
 The a.b.c lookup plugin.
 md: |- The a.b.c lookup plugin. rst: |- The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. ansible_doc_text: The [a.b.c] lookup plugin.
-link_and_url: source: |- An URL U(https://example.com) and L(a link, https://
-example.org). html: |-
+rst_plain: The \ :ref:`a.b.c
+a.b.c_lookup>`\ lookup plugin. link_and_url: source: |- An URL U(https://
+example.com) and L(a link, https://example.org). html: |-
 An URL https://example.com and a_link.
 html_plain: |-
 An URL https://example.com and a_link.
 md: |- An URL [https\://example.com](https\://example.com) and [a link](https\:
 //example.org). rst: |- An URL \ https://example.com\ and \ `a link
 example.org>`__\ . ansible_doc_text: An URL https://example.com and a link
-example.org>. rst_ref: source: |- A R(RST reference,
+example.org>. rst_plain: An URL \ https://example.com\ and \ `a link
+example.org>`__\ . rst_ref: source: |- A R(RST reference,
 ansible_collections.community.general.ufw_module). html: |-
 A RST reference.
 html_plain: |-
 A RST reference.
 md: |- A RST reference. rst: |- A \ :ref:`RST reference
-community.general.ufw_module>`\ . ansible_doc_text: A RST reference.
-horizontal_line: source: |- foo HORIZONTALLINE bar html: |-
+community.general.ufw_module>`\ . ansible_doc_text: A RST reference. rst_plain:
+A \ :ref:`RST reference
+community.general.ufw_module>`\ . horizontal_line: source: |- foo
+HORIZONTALLINE bar html: |-
 foo
 ===============================================================================
 bar
 html_plain: |-
 foo
 ===============================================================================
 bar
 md: |- foo
 ===============================================================================
 bar rst: |- foo .. raw:: html
 ===============================================================================
-bar ansible_doc_text: |- foo ------------- bar semantic_markup: source: |- foo
-E(FOOBAR) bar P(foo.bar.baz#bam) has value V( foo\),bar\\bam ). html: |-
+bar ansible_doc_text: |- foo ------------- bar rst_plain: |- foo -----------
+- bar semantic_markup: source: |- foo E(FOOBAR) bar P(foo.bar.baz#bam) has
+value V( foo\),bar\\bam ). html: |-
 foo FOOBAR bar foo.bar.baz has value foo),bar\bam.
 html_plain: |-
 foo FOOBAR bar foo.bar.baz has value foo),bar\bam.
 md: |- foo FOOBAR bar foo.bar.baz has value foo\)\,bar\\bam. rst: |- foo \ :
 envvar:`FOOBAR`\ bar \ :ref:`foo.bar.baz
 foo.bar.baz_bam>`\ has value \ :ansval:`\ foo),bar\\bam \ `\ .
 ansible_doc_text: foo `FOOBAR' bar [foo.bar.baz] has value ` foo),bar\bam '.
+rst_plain: foo \ :envvar:`FOOBAR`\ bar \ :ref:`foo.bar.baz
+foo.bar.baz_bam>`\ has value \ :literal:`\ foo),bar\\bam \ `\ .
 option_name_no_current_plugin: source: - |- O(foo) O(bar.baz[123].bam[len(x\) -
 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
 [123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
@@ -156,17 +171,43 @@
 [123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role
 bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role
 bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main entrypoint)
 `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) -
 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) -
 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) -
-1]=bar' option_name_current_plugin: source: - |- O(foo) O(bar.baz[123].bam[len
-(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
-(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
+1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of
+lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+option_name_current_plugin: source: - |- O(foo) O(bar.baz[123].bam[len(x\) -
+1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
+[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
 [123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:
 main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:main:foo=bar) O
 (bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O
@@ -232,30 +273,64 @@
 lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]' (of role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo,
 main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
 entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
 [len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
-`bar.baz[123].bam[len(x) - 1]=bar' option_name_current_role: source: - |- O
-(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\)
-- 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(other_entrypoint:foo) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) - |- O
-(other_entrypoint:foo=) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |-
-O(other_entrypoint:foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) -
-1]=bar) - |- O(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam
-[len(x\) - 1]) - |- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz
-[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#lookup:foo=bar) O
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:
-main:foo) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]) - |- O
-(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) -
-1]=) - |- O(bam.baz.foo#role:main:foo=bar) O(bam.baz.foo#role:main:bar.baz
-[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O(ignore:bar.baz[123].bam[len
-(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O
-(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
+`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+option_name_current_role: source: - |- O(foo) O(bar.baz[123].bam[len(x\) - 1])
+- |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
+[123].bam[len(x\) - 1]=bar) - |- O(other_entrypoint:foo) O(other_entrypoint:
+bar.baz[123].bam[len(x\) - 1]) - |- O(other_entrypoint:foo=) O
+(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |- O(other_entrypoint:
+foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
+|- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
+1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:
+bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O
+(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:
+main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O
+(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz
+[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -331,14 +406,61 @@
 - 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role bam.baz.foo, main
 entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role bam.baz.foo, main
 entrypoint) `foo=' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]=' (of role bam.baz.foo, main entrypoint) `foo=bar' (of role
 bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role
 bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) - 1]' `foo='
 `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+rst_plain: |- \ :literal:`foo` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :
+ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=bar` (of
+role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 option_name_no_current_plugin_w_links: source: - |- O(foo) O(bar.baz[123].bam
 [len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
 (bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
@@ -415,17 +537,43 @@
 [123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role
 bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role
 bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main entrypoint)
 `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) -
 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) -
 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) -
-1]=bar' option_name_current_plugin_w_links: source: - |- O(foo) O(bar.baz
-[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O
-(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
+1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of
+lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+option_name_current_plugin_w_links: source: - |- O(foo) O(bar.baz[123].bam[len
+(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
+(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
 [123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:
 main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:main:foo=bar) O
 (bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O
@@ -504,30 +652,64 @@
 lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]' (of role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo,
 main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
 entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
 [len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
-`bar.baz[123].bam[len(x) - 1]=bar' option_name_current_role_w_links: source: -
-|- O(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len
-(x\) - 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(other_entrypoint:foo) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) - |- O
-(other_entrypoint:foo=) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |-
-O(other_entrypoint:foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) -
-1]=bar) - |- O(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam
-[len(x\) - 1]) - |- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz
-[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#lookup:foo=bar) O
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:
-main:foo) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]) - |- O
-(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) -
-1]=) - |- O(bam.baz.foo#role:main:foo=bar) O(bam.baz.foo#role:main:bar.baz
-[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O(ignore:bar.baz[123].bam[len
-(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O
-(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
+`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+option_name_current_role_w_links: source: - |- O(foo) O(bar.baz[123].bam[len
+(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
+(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(other_entrypoint:foo) O
+(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) - |- O(other_entrypoint:foo=)
+O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |- O(other_entrypoint:
+foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
+|- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
+1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:
+bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O
+(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:
+main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O
+(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz
+[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
@@ -615,23 +797,71 @@
 `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of
 lookup plugin bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]' (of role bam.baz.foo, main entrypoint) `foo='
 (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role
 bam.baz.foo, main entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo'
 `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
-`bar.baz[123].bam[len(x) - 1]=bar' return_value_no_current_plugin: source: - |-
-RV(foo) RV(bar.baz[123].bam[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len
-(x\) - 1]=) - |- RV(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV
-(bam.baz.foo#lookup:foo) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
-|- RV(bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=) - |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam
-[len(x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1])
-- |- RV(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:
-foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of role :
+ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo` (of role :ref:
+`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :
+ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=bar` (of
+role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
+foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
+`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar` (of role :ref:`bam.baz.foo
+bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
+- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+return_value_no_current_plugin: source: - |- RV(foo) RV(bar.baz[123].bam[len
+(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV(foo=bar) RV
+(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo) RV
+(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV(bam.baz.foo#lookup:
+foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- RV
+(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
+1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) - |- RV
+(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:foo=bar)
+RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -665,15 +895,30 @@
 [123].bam[len(x) - 1]=bar`\ ansible_doc_text: |- `foo' `bar.baz[123].bam[len(x)
 - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x)
 - 1]=bar' `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]'
 (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo) `bar.baz
 [123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup
 plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
-(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
+literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:
+`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 return_value_current_plugin: source: - |- RV(foo) RV(bar.baz[123].bam[len(x\) -
 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV(foo=bar) RV
 (bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo) RV
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV(bam.baz.foo#lookup:
 foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- RV
 (bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) - |- RV
@@ -721,15 +966,37 @@
 [123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam) `foo=bar' (of boo
 plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=bar' (of boo plugin
 foo.bar.baz.bam) `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x)
 - 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo)
 `bar.baz[123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of
 lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
-(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
+literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
+`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 return_value_no_current_plugin_w_links: source: - |- RV(foo) RV(bar.baz
 [123].bam[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |-
 RV(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:
 foo) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
 (bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=)
 - |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len
 (x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) -
@@ -785,15 +1052,30 @@
 [123].bam[len(x) - 1]=bar`\ ansible_doc_text: |- `foo' `bar.baz[123].bam[len(x)
 - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x)
 - 1]=bar' `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]'
 (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo) `bar.baz
 [123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup
 plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
-(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
+literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:
+`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 return_value_current_plugin_w_links: source: - |- RV(foo) RV(bar.baz[123].bam
 [len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV
 (foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo)
 RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
 (bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=)
 - |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len
 (x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) -
@@ -855,16 +1137,38 @@
 foo.bar.baz.bam) `foo=bar' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam
 [len(x) - 1]=bar' (of boo plugin foo.bar.baz.bam) `foo' (of lookup plugin
 bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo)
 `foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of
 lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz
 [123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
-`bar.baz[123].bam[len(x) - 1]=bar' unhelpful_errors: source: - P(foo) - C(foo -
-R(foo,bar parse_opts: helpfulErrors: false html: |-
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
+`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
+plugin :ref:`foo.bar.baz.bam
+foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
+plugin :ref:`bam.baz.foo
+bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
+`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ unhelpful_errors:
+source: - P(foo) - C(foo - R(foo,bar parse_opts: helpfulErrors: false html: |-
 ERROR while parsing: While parsing P() at index 1 of paragraph 1: Parameter
 "foo" is not of the form FQCN#type
 ERROR while parsing: While parsing C() at index 1 of paragraph 2: Cannot find
 closing ")" after last parameter
 ERROR while parsing: While parsing R() at index 1 of paragraph 3: Cannot find
 closing ")" after last parameter
 html_plain: |-
@@ -884,16 +1188,21 @@
 index 1 of paragraph 2: Cannot find closing ")" after last parameter\ \ :
 strong:`ERROR while parsing`\ : While parsing R() at index 1 of paragraph 3:
 Cannot find closing ")" after last parameter\ ansible_doc_text: |- [[ERROR
 while parsing: While parsing P() at index 1 of paragraph 1: Parameter "foo" is
 not of the form FQCN#type]] [[ERROR while parsing: While parsing C() at index 1
 of paragraph 2: Cannot find closing ")" after last parameter]] [[ERROR while
 parsing: While parsing R() at index 1 of paragraph 3: Cannot find closing ")"
-after last parameter]] helpful_errors: source: - P(foo) - C(foo - R(foo,bar
-html: |-
+after last parameter]] rst_plain: |- \ :strong:`ERROR while parsing`\ : While
+parsing P() at index 1 of paragraph 1: Parameter "foo" is not of the form
+FQCN#type\ \ :strong:`ERROR while parsing`\ : While parsing C() at index 1 of
+paragraph 2: Cannot find closing ")" after last parameter\ \ :strong:`ERROR
+while parsing`\ : While parsing R() at index 1 of paragraph 3: Cannot find
+closing ")" after last parameter\ helpful_errors: source: - P(foo) - C(foo - R
+(foo,bar html: |-
 ERROR while parsing: While parsing "P(foo)" at index 1 of paragraph 1:
 Parameter "foo" is not of the form FQCN#type
 ERROR while parsing: While parsing "C(foo" at index 1 of paragraph 2: Cannot
 find closing ")" after last parameter
 ERROR while parsing: While parsing "R(foo,bar" at index 1 of paragraph 3:
 Cannot find closing ")" after last parameter
 html_plain: |-
@@ -914,8 +1223,13 @@
 closing ")" after last parameter\ \ :strong:`ERROR while parsing`\ : While
 parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find closing ")" after
 last parameter\ ansible_doc_text: |- [[ERROR while parsing: While parsing "P
 (foo)" at index 1 of paragraph 1: Parameter "foo" is not of the form
 FQCN#type]] [[ERROR while parsing: While parsing "C(foo" at index 1 of
 paragraph 2: Cannot find closing ")" after last parameter]] [[ERROR while
 parsing: While parsing "R(foo,bar" at index 1 of paragraph 3: Cannot find
-closing ")" after last parameter]]
+closing ")" after last parameter]] rst_plain: |- \ :strong:`ERROR while
+parsing`\ : While parsing "P(foo)" at index 1 of paragraph 1: Parameter "foo"
+is not of the form FQCN#type\ \ :strong:`ERROR while parsing`\ : While parsing
+"C(foo" at index 1 of paragraph 2: Cannot find closing ")" after last
+parameter\ \ :strong:`ERROR while parsing`\ : While parsing "R(foo,bar" at
+index 1 of paragraph 3: Cannot find closing ")" after last parameter\
```

### Comparing `antsibull_docs_parser-0.2.0/.github/workflows/nox.yml` & `antsibull_docs_parser-0.3.0/.github/workflows/nox.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/changelogs/changelog.yaml` & `antsibull_docs_parser-0.3.0/changelogs/changelog.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -32,7 +32,16 @@
     - 15-lint.yml
     - 16-create-vectors.yml
     - 17-ansible-doc-text.yml
     - 18-source.yml
     - 19-helpful-errors.yml
     - 9-semantic-markup-roles.yml
     release_date: '2023-04-02'
+  0.3.0:
+    changes:
+      minor_changes:
+      - Add support for plain RST rendering (https://github.com/ansible-community/antsibull-docs-parser/pull/20).
+      release_summary: Feature release.
+    fragments:
+    - 0.3.0.yml
+    - 20-rst-plain.yml
+    release_date: '2023-04-14'
```

### Comparing `antsibull_docs_parser-0.2.0/changelogs/config.yaml` & `antsibull_docs_parser-0.3.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/_parser_impl.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/ansible_doc_text.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/ansible_doc_text.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/dom.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/format.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/html.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/md.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/md.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/src/antsibull_docs_parser/parser.py` & `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/create-vectors.py` & `antsibull_docs_parser-0.3.0/tests/unit/create-vectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     get_rst_opts,
 )
 
 from antsibull_docs_parser.ansible_doc_text import to_ansible_doc_text
 from antsibull_docs_parser.html import to_html, to_html_plain
 from antsibull_docs_parser.md import to_md
 from antsibull_docs_parser.parser import parse
-from antsibull_docs_parser.rst import to_rst
+from antsibull_docs_parser.rst import to_rst, to_rst_plain
 
 
 def add(test_data: t.Dict[str, t.Any], key: str, value: t.Any) -> None:
     if isinstance(value, str):
         if key not in test_data and "\n" in value:
             value = LiteralScalarString(value)
     test_data[key] = value
@@ -47,14 +47,17 @@
 
     result = to_md(parsed, link_provider=md_link_provider, **md_opts)
     add(test_data, "md", result)
 
     result = to_rst(parsed, **rst_opts)
     add(test_data, "rst", result)
 
+    result = to_rst_plain(parsed, **rst_opts)
+    add(test_data, "rst_plain", result)
+
     result = to_ansible_doc_text(parsed, **ansible_doc_text_opts)
     add(test_data, "ansible_doc_text", result)
 
 
 def main() -> None:
     yaml = YAML(typ="rt")
     with open(VECTORS_FILE, "r") as stream:
```

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_dom.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_format.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_html.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_md.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_md.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_parser.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_parser_impl.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_rst.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_rst.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Author: Felix Fontein <felix@fontein.de>
 # GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or
 # https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2023, Ansible Project
 
 from antsibull_docs_parser import dom
-from antsibull_docs_parser.rst import rst_escape, to_rst
+from antsibull_docs_parser.rst import rst_escape, to_rst, to_rst_plain
 
 
 def test_rst_escape():
     assert rst_escape("") == ""
     assert rst_escape("  foo  ") == "  foo  "
     assert rst_escape("  foo  ", True) == "\\   foo  \\ "
     assert rst_escape("\\<_>`*<_>*`\\") == "\\\\\\<\\_\\>\\`\\*\\<\\_\\>\\*\\`\\\\"
 
 
 def test_to_rst():
     assert to_rst([]) == ""
     assert to_rst([[dom.TextPart(text="test")]]) == "test"
+
+
+def test_to_rst_plain():
+    assert to_rst_plain([]) == ""
+    assert to_rst_plain([[dom.TextPart(text="test")]]) == "test"
```

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/test_vectors.py` & `antsibull_docs_parser-0.3.0/tests/unit/test_vectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from antsibull_docs_parser import dom
 from antsibull_docs_parser.ansible_doc_text import to_ansible_doc_text
 from antsibull_docs_parser.format import LinkProvider
 from antsibull_docs_parser.html import to_html, to_html_plain
 from antsibull_docs_parser.md import to_md
 from antsibull_docs_parser.parser import Context, parse
-from antsibull_docs_parser.rst import to_rst
+from antsibull_docs_parser.rst import to_rst, to_rst_plain
 
 from .vectors import (
     VECTORS_FILE,
     get_ansible_doc_text_opts,
     get_context_parse_opts,
     get_html_opts_link_provider,
     get_md_opts_link_provider,
@@ -67,10 +67,14 @@
         result = to_md(parsed, link_provider=md_link_provider, **md_opts)
         assert result == test_data["md"]
 
     if "rst" in test_data:
         result = to_rst(parsed, **rst_opts)
         assert result == test_data["rst"]
 
+    if "rst_plain" in test_data:
+        result = to_rst_plain(parsed, **rst_opts)
+        assert result == test_data["rst_plain"]
+
     if "ansible_doc_text" in test_data:
         result = to_ansible_doc_text(parsed, **ansible_doc_text_opts)
         assert result == test_data["ansible_doc_text"]
```

### Comparing `antsibull_docs_parser-0.2.0/tests/unit/vectors.py` & `antsibull_docs_parser-0.3.0/tests/unit/vectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2022, Ansible Project
 
 import typing as t
 
 from antsibull_docs_parser import dom
 from antsibull_docs_parser.format import LinkProvider
-from antsibull_docs_parser.html import to_html, to_html_plain
-from antsibull_docs_parser.md import to_md
-from antsibull_docs_parser.parser import Context, parse
-from antsibull_docs_parser.rst import to_rst
+from antsibull_docs_parser.parser import Context
 
 VECTORS_FILE = "test-vectors.yaml"
 
 
 class _TestLinkProvider(LinkProvider):
     _plugin_link = None
     _plugin_option_like_link = None
```

### Comparing `antsibull_docs_parser-0.2.0/.gitignore` & `antsibull_docs_parser-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/README.md` & `antsibull_docs_parser-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
 Install and run `nox` to run all tests. `nox` will create virtual environments in `.nox` inside the checked out project and install the requirements needed to run the tests there.
 
 To run specific tests:
 1. `nox -e test` to only run unit tests;
 2. `nox -e lint` to run all linters and formatters at once;
 3. `nox -e formatters` to run `isort` and `black`;
-4. `nox -e codeqa` to run `flake8`, `pylint`, and `reuse lint`;
+4. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
 5. `nox -e typing` to run `mypy` and `pyre`;
 6. `nox -e create_vectors` to update the `test-vectors.yml` file. Please note that this file should be synchronized with the corresponding file in [the antsibull-docs-ts project](https://github.com/ansible-community/antsibull-docs-ts).
 
 ## Releasing a new version
 
 1. Run `nox -e bump -- <version> <release_summary_message>`. This:
    * Bumps the package version in `pyproject.toml`. 
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-docs-parser <version>' <version>`.
-   * Runs `hatch build`.
+   * Runs `hatch build --clean`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
    * Bumps the version to `<version>.post0`;
    * Adds the changed file to git and run `git commit -m 'Post-release version bump.'`;
 4. Run `git push --follow-tags` to the appropriate remotes and create a GitHub release.
```

### Comparing `antsibull_docs_parser-0.2.0/pyproject.toml` & `antsibull_docs_parser-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs-parser"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python library for processing Ansible documentation markup"
 readme = "README.md"
 requires-python = ">=3.6.1"
 license = "GPL-3.0-or-later AND BSD-2-Clause"
 license-files.globs = ["LICENSES/*.txt"]
 authors = [
   { name = "Felix Fontein", email = "felix@fontein.de" },
@@ -36,14 +36,15 @@
 ]
 
 [project.urls]
 "Source code" = "https://github.com/ansible-community/antsibull-docs-parser/"
 
 [project.optional-dependencies]
 codeqa = [
+    "antsibull-changelog",
     "flake8",
     "pylint",
     "reuse",
 ]
 coverage = [
     "coverage[toml]",
 ]
@@ -56,15 +57,15 @@
     "pytest",
     "pytest-cov",
     "pytest-error-for-skips",
 ]
 typing = [
     "mypy",
     # https://github.com/facebook/pyre-check/issues/398
-    "pyre-check ~= 0.9.17",
+    "pyre-check >= 0.9.17",
 ]
 dev = [
     # Used by nox sessions
     "antsibull-docs-parser[codeqa]",
     "antsibull-docs-parser[coverage]",
     "antsibull-docs-parser[formatters]",
     "antsibull-docs-parser[test]",
```

### Comparing `antsibull_docs_parser-0.2.0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs_parser-0.3.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.2.0/PKG-INFO` & `antsibull_docs_parser-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs-parser
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for processing Ansible documentation markup
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs-parser/
 Author-email: Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later AND BSD-2-Clause
 License-File: LICENSES/BSD-2-Clause.txt
 License-File: LICENSES/GPL-3.0-or-later.txt
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Provides-Extra: codeqa
+Requires-Dist: antsibull-changelog; extra == 'codeqa'
 Requires-Dist: flake8; extra == 'codeqa'
 Requires-Dist: pylint; extra == 'codeqa'
 Requires-Dist: reuse; extra == 'codeqa'
 Provides-Extra: coverage
 Requires-Dist: coverage[toml]; extra == 'coverage'
 Provides-Extra: dev
 Requires-Dist: antsibull-docs-parser[codeqa]; extra == 'dev'
@@ -39,15 +40,15 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-error-for-skips; extra == 'test'
 Requires-Dist: pyyaml; extra == 'test'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
-Requires-Dist: pyre-check~=0.9.17; extra == 'typing'
+Requires-Dist: pyre-check>=0.9.17; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 SPDX-FileCopyrightText: 2023, Ansible Project
@@ -64,25 +65,25 @@
 
 Install and run `nox` to run all tests. `nox` will create virtual environments in `.nox` inside the checked out project and install the requirements needed to run the tests there.
 
 To run specific tests:
 1. `nox -e test` to only run unit tests;
 2. `nox -e lint` to run all linters and formatters at once;
 3. `nox -e formatters` to run `isort` and `black`;
-4. `nox -e codeqa` to run `flake8`, `pylint`, and `reuse lint`;
+4. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
 5. `nox -e typing` to run `mypy` and `pyre`;
 6. `nox -e create_vectors` to update the `test-vectors.yml` file. Please note that this file should be synchronized with the corresponding file in [the antsibull-docs-ts project](https://github.com/ansible-community/antsibull-docs-ts).
 
 ## Releasing a new version
 
 1. Run `nox -e bump -- <version> <release_summary_message>`. This:
    * Bumps the package version in `pyproject.toml`. 
    * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
    * Runs `antsibull-changelog release` and adds the changed files to git.
    * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-docs-parser <version>' <version>`.
-   * Runs `hatch build`.
+   * Runs `hatch build --clean`.
 2. Run `git push` to the appropriate remotes.
 3. Once CI passes on GitHub, run `nox -e publish`. This:
    * Runs `hatch publish`;
    * Bumps the version to `<version>.post0`;
    * Adds the changed file to git and run `git commit -m 'Post-release version bump.'`;
 4. Run `git push --follow-tags` to the appropriate remotes and create a GitHub release.
```

