# Comparing `tmp/ghstack-0.7.1.tar.gz` & `tmp/ghstack-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghstack-0.7.1.tar", max compression
+gzip compressed data, was "ghstack-0.8.0.tar", max compression
```

## Comparing `ghstack-0.7.1.tar` & `ghstack-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1070 2022-04-07 02:23:24.929636 ghstack-0.7.1/LICENSE
--rw-r--r--   0        0        0     6021 2022-04-07 02:23:24.929880 ghstack-0.7.1/README.md
--rw-r--r--   0        0        0      136 2022-04-07 02:23:24.930435 ghstack-0.7.1/ghstack/__init__.py
--rwxr-xr-x   0        0        0     5735 2022-04-07 02:23:24.930555 ghstack-0.7.1/ghstack/__main__.py
--rw-r--r--   0        0        0     1095 2022-04-07 02:23:24.930665 ghstack-0.7.1/ghstack/action.py
--rw-r--r--   0        0        0     1973 2022-04-07 02:23:24.930781 ghstack-0.7.1/ghstack/cache.py
--rw-r--r--   0        0        0     1055 2022-04-07 02:23:24.930889 ghstack-0.7.1/ghstack/checkout.py
--rw-r--r--   0        0        0     1024 2022-04-07 02:23:24.931023 ghstack-0.7.1/ghstack/circleci.py
--rw-r--r--   0        0        0     2738 2022-04-07 02:23:24.931145 ghstack-0.7.1/ghstack/circleci_real.py
--rw-r--r--   0        0        0     5894 2022-04-07 02:23:24.931281 ghstack-0.7.1/ghstack/config.py
--rw-r--r--   0        0        0     3957 2022-08-29 13:55:24.099022 ghstack-0.7.1/ghstack/diff.py
--rw-r--r--   0        0        0     4162 2022-04-07 02:23:24.931572 ghstack-0.7.1/ghstack/forensics.py
--rw-r--r--   0        0        0     3334 2022-04-07 03:20:36.909501 ghstack-0.7.1/ghstack/git.py
--rw-r--r--   0        0        0     2128 2022-08-29 13:55:24.099587 ghstack-0.7.1/ghstack/github.py
--rw-r--r--   0        0        0    13675 2022-08-29 13:55:24.100128 ghstack-0.7.1/ghstack/github_fake.py
--rw-r--r--   0        0        0     5219 2022-08-26 16:58:04.351715 ghstack-0.7.1/ghstack/github_real.py
--rw-r--r--   0        0        0   239993 2022-04-07 02:23:24.933305 ghstack-0.7.1/ghstack/github_schema.graphql
--rw-r--r--   0        0        0     3223 2022-08-26 16:58:04.353149 ghstack-0.7.1/ghstack/github_utils.py
--rw-r--r--   0        0        0     1193 2022-04-07 02:23:24.933623 ghstack-0.7.1/ghstack/gpg_sign.py
--rw-r--r--   0        0        0     5960 2022-08-29 13:55:24.100605 ghstack-0.7.1/ghstack/land.py
--rw-r--r--   0        0        0     5808 2022-04-07 02:23:24.933909 ghstack-0.7.1/ghstack/logs.py
--rw-r--r--   0        0        0        0 2022-04-07 02:23:24.933973 ghstack-0.7.1/ghstack/py.typed
--rw-r--r--   0        0        0     3629 2022-04-07 02:23:24.934107 ghstack-0.7.1/ghstack/rage.py
--rw-r--r--   0        0        0    11860 2022-04-07 03:20:36.910130 ghstack-0.7.1/ghstack/shell.py
--rw-r--r--   0        0        0     4572 2022-04-07 02:23:24.934407 ghstack-0.7.1/ghstack/status.py
--rw-r--r--   0        0        0    42114 2022-08-29 13:55:24.101210 ghstack-0.7.1/ghstack/submit.py
--rw-r--r--   0        0        0      852 2022-04-07 02:23:24.934899 ghstack-0.7.1/ghstack/types.py
--rw-r--r--   0        0        0     3474 2022-04-07 02:23:24.935094 ghstack-0.7.1/ghstack/unlink.py
--rw-r--r--   0        0        0      885 2022-08-29 13:56:11.953467 ghstack-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7131 2022-08-29 13:56:26.982858 ghstack-0.7.1/setup.py
--rw-r--r--   0        0        0     6961 2022-08-29 13:56:26.983240 ghstack-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-04-07 02:23:24.929636 ghstack-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6021 2023-03-30 12:55:39.619261 ghstack-0.8.0/README.md
+-rw-r--r--   0        0        0      241 2022-12-09 19:26:51.951885 ghstack-0.8.0/ghstack/__init__.py
+-rwxr-xr-x   0        0        0       92 2023-03-30 12:55:39.620566 ghstack-0.8.0/ghstack/__main__.py
+-rw-r--r--   0        0        0     1133 2022-12-20 00:38:37.431599 ghstack-0.8.0/ghstack/action.py
+-rw-r--r--   0        0        0     2049 2022-12-20 00:38:37.432105 ghstack-0.8.0/ghstack/cache.py
+-rw-r--r--   0        0        0     1080 2022-12-20 00:38:37.432964 ghstack-0.8.0/ghstack/checkout.py
+-rw-r--r--   0        0        0     1024 2022-12-20 00:38:37.433490 ghstack-0.8.0/ghstack/circleci.py
+-rw-r--r--   0        0        0     2677 2022-12-20 00:38:37.433950 ghstack-0.8.0/ghstack/circleci_real.py
+-rw-r--r--   0        0        0     6229 2023-03-30 12:55:46.242630 ghstack-0.8.0/ghstack/cli.py
+-rw-r--r--   0        0        0     5927 2023-03-30 12:55:39.629442 ghstack-0.8.0/ghstack/config.py
+-rw-r--r--   0        0        0     3987 2022-12-20 00:38:37.435323 ghstack-0.8.0/ghstack/diff.py
+-rw-r--r--   0        0        0     4301 2022-12-20 00:38:37.436988 ghstack-0.8.0/ghstack/forensics.py
+-rw-r--r--   0        0        0     3390 2022-12-20 00:38:37.437698 ghstack-0.8.0/ghstack/git.py
+-rw-r--r--   0        0        0     2128 2022-12-20 00:38:37.438381 ghstack-0.8.0/ghstack/github.py
+-rw-r--r--   0        0        0    13740 2023-03-30 12:55:39.630926 ghstack-0.8.0/ghstack/github_fake.py
+-rw-r--r--   0        0        0     5186 2022-12-20 00:38:37.440403 ghstack-0.8.0/ghstack/github_real.py
+-rw-r--r--   0        0        0   239993 2022-04-07 02:23:24.933305 ghstack-0.8.0/ghstack/github_schema.graphql
+-rw-r--r--   0        0        0     3289 2022-12-20 00:38:37.441217 ghstack-0.8.0/ghstack/github_utils.py
+-rw-r--r--   0        0        0     1273 2022-12-20 00:38:37.442048 ghstack-0.8.0/ghstack/gpg_sign.py
+-rw-r--r--   0        0        0     6156 2022-12-20 00:38:37.442832 ghstack-0.8.0/ghstack/land.py
+-rw-r--r--   0        0        0     5505 2023-03-30 12:55:39.632116 ghstack-0.8.0/ghstack/logs.py
+-rw-r--r--   0        0        0        0 2022-04-07 02:23:24.933973 ghstack-0.8.0/ghstack/py.typed
+-rw-r--r--   0        0        0     3708 2022-12-20 00:38:37.445762 ghstack-0.8.0/ghstack/rage.py
+-rw-r--r--   0        0        0    11709 2023-03-30 12:55:39.633351 ghstack-0.8.0/ghstack/shell.py
+-rw-r--r--   0        0        0     4837 2022-12-20 00:38:37.447406 ghstack-0.8.0/ghstack/status.py
+-rw-r--r--   0        0        0    43290 2022-12-20 00:38:37.450355 ghstack-0.8.0/ghstack/submit.py
+-rw-r--r--   0        0        0      852 2022-12-20 00:38:37.450990 ghstack-0.8.0/ghstack/types.py
+-rw-r--r--   0        0        0     3659 2022-12-20 00:38:37.451911 ghstack-0.8.0/ghstack/unlink.py
+-rw-r--r--   0        0        0      902 2023-04-14 02:17:56.432910 ghstack-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7112 2023-04-14 02:19:07.574920 ghstack-0.8.0/setup.py
+-rw-r--r--   0        0        0     6850 2023-04-14 02:19:07.575383 ghstack-0.8.0/PKG-INFO
```

### Comparing `ghstack-0.7.1/LICENSE` & `ghstack-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghstack-0.7.1/README.md` & `ghstack-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Conveniently submit stacks of diffs to GitHub as separate pull requests.
 
 ```
 pip3 install ghstack
 ```
 
-Python 3.6 and greater only.
+Python 3.8 and greater only.
 
 ## How to setup
 
 Go to github.com `Settings→Developer Settings→Personal Access Tokens` and
 generate a token with `public_repo` access only.
 Create a `~/.ghstackrc` as shown below:
 ```
```

### Comparing `ghstack-0.7.1/ghstack/__main__.py` & `ghstack-0.8.0/ghstack/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,165 +1,235 @@
-#!/usr/bin/env python3
-
-import argparse
 import asyncio
+import contextlib
+from typing import Generator, List, Tuple
+
+import click
 
 import ghstack
 import ghstack.action
 import ghstack.checkout
 import ghstack.circleci_real
 import ghstack.config
 import ghstack.github_real
 import ghstack.land
 import ghstack.logs
 import ghstack.rage
 import ghstack.status
 import ghstack.submit
 import ghstack.unlink
 
+EXIT_STACK = contextlib.ExitStack()
 
-def main() -> None:
-    parser = argparse.ArgumentParser(
-        description='Submit stack of diffs to GitHub.')
-    parser.add_argument(
-        '--version', action='version',
-        version="ghstack {}".format(ghstack.__version__),
-        help='Print version')
-    parser.add_argument(
-        '--debug', action='store_true',
-        help='Log debug information to stderr')
-
-    subparsers = parser.add_subparsers(dest='cmd')
-
-    submit = subparsers.add_parser('submit')
-    for subparser in (submit, parser):
-        subparser.add_argument(
-            '--message', '-m',
-            default='Update',
-            help='Description of change you made')
-        subparser.add_argument(
-            '--update-fields', '-u', action='store_true',
-            help='Update GitHub pull request summary from the local commit')
-        subparser.add_argument(
-            '--short', action='store_true',
-            help='Print only the URL of the latest opened PR to stdout')
-        subparser.add_argument(
-            '--force', action='store_true',
-            help='force push the branch even if your local branch is stale')
-        subparser.add_argument(
-            '--no-skip', action='store_true',
-            help='Never skip pushing commits, even if the contents didn\'t change '
-                 '(use this if you\'ve only updated the commit message).')
-        subparser.add_argument(
-            '--draft', action='store_true',
-            help='Create the pull request in draft mode (only if it has not already been created)')
-
-    unlink = subparsers.add_parser('unlink')
-    unlink.add_argument('COMMITS', nargs='*')
-
-    rage = subparsers.add_parser('rage')
-    rage.add_argument('--latest', action='store_true',
-        help='Select the last command (not including rage commands) to report')
-
-    land = subparsers.add_parser('land')
-    land.add_argument('pull_request', metavar='PR',
-        help='GitHub pull request URL of stack to land')
-
-    checkout = subparsers.add_parser('checkout')
-    checkout.add_argument('pull_request', metavar='PR',
-        help='GitHub pull request URL to checkout')
-
-    action = subparsers.add_parser('action')
-    # TODO: support number as well
-    action.add_argument('pull_request', metavar='PR',
-        help='GitHub pull request URL to perform action on')
-    action.add_argument('--close', action='store_true',
-        help='Close the specified pull request')
-
-    status = subparsers.add_parser('status')
-    # TODO: support number as well
-    status.add_argument('pull_request', metavar='PR',
-        help='GitHub pull request URL to perform action on')
-
-    args = parser.parse_args()
+GhstackContext = Tuple[
+    ghstack.shell.Shell,
+    ghstack.config.Config,
+    ghstack.github_real.RealGitHubEndpoint,
+]
+
+
+@contextlib.contextmanager
+def cli_context(
+    request_circle_token: bool = False,
+) -> Generator[GhstackContext, None, None]:
+    with EXIT_STACK:
+        shell = ghstack.shell.Shell()
+        config = ghstack.config.read_config(request_circle_token=request_circle_token)
+        github = ghstack.github_real.RealGitHubEndpoint(
+            oauth_token=config.github_oauth,
+            proxy=config.proxy,
+            github_url=config.github_url,
+        )
+        yield shell, config, github
 
-    if args.cmd is None:
-        args.cmd = 'submit'
 
-    with ghstack.logs.manager(debug=args.debug):
+@click.group(invoke_without_command=True)
+@click.pass_context
+@click.version_option(ghstack.__version__, "--version", "-V")
+@click.option("--debug", is_flag=True, help="Log debug information to stderr")
+# hidden arguments that we'll pass along to submit if no other command given
+@click.option("--message", "-m", default="Update", hidden=True)
+@click.option("--update-fields", "-u", is_flag=True, hidden=True)
+@click.option("--short", is_flag=True, hidden=True)
+@click.option("--force", is_flag=True, hidden=True)
+@click.option("--no-skip", is_flag=True, hidden=True)
+@click.option("--draft", is_flag=True, hidden=True)
+def main(
+    ctx: click.Context,
+    debug: bool,
+    message: str,
+    update_fields: bool,
+    short: bool,
+    force: bool,
+    no_skip: bool,
+    draft: bool,
+) -> None:
+    """
+    Submit stacks of diffs to Github
+    """
+    EXIT_STACK.enter_context(ghstack.logs.manager(debug=debug))
+
+    if not ctx.invoked_subcommand:
+        return ctx.invoke(
+            submit,
+            message=message,
+            update_fields=update_fields,
+            short=short,
+            force=force,
+            no_skip=no_skip,
+            draft=draft,
+        )
 
-        sh = ghstack.shell.Shell()
-        conf = ghstack.config.read_config()
-        github = ghstack.github_real.RealGitHubEndpoint(
-            oauth_token=conf.github_oauth,
-            proxy=conf.proxy,
-            github_url=conf.github_url,
-        )
-
-        if args.cmd == 'rage':
-            ghstack.rage.main(latest=args.latest)
-        elif args.cmd == 'submit':
-            ghstack.submit.main(
-                msg=args.message,
-                username=conf.github_username,
-                sh=sh,
-                github=github,
-                update_fields=args.update_fields,
-                short=args.short,
-                force=args.force,
-                no_skip=args.no_skip,
-                draft=args.draft,
-                github_url=conf.github_url,
-                remote_name=conf.remote_name,
-            )
-        elif args.cmd == 'unlink':
-            ghstack.unlink.main(
-                commits=args.COMMITS,
-                github=github,
-                sh=sh,
-                github_url=conf.github_url,
-                remote_name=conf.remote_name,
-            )
-        elif args.cmd == 'land':
-            ghstack.land.main(
-                pull_request=args.pull_request,
-                github=github,
-                sh=sh,
-                github_url=conf.github_url,
-                remote_name=conf.remote_name,
-            )
-        elif args.cmd == 'action':
-            ghstack.action.main(
-                pull_request=args.pull_request,
-                github=github,
-                sh=sh,
-                close=args.close,
-            )
-        elif args.cmd == 'status':
-            # Re-read conf and request circle token if not available
-            # TODO: Restructure this so that we just request
-            # configurations "on-demand" rather than all upfront
-            conf = ghstack.config.read_config(request_circle_token=True)
-            circleci = ghstack.circleci_real.RealCircleCIEndpoint(
-                circle_token=conf.circle_token
-            )
-            # Blegh
-            loop = asyncio.get_event_loop()
-            loop.run_until_complete(ghstack.status.main(
-                pull_request=args.pull_request,
-                github=github,
-                circleci=circleci
-            ))
-            loop.close()
-        elif args.cmd == 'checkout':
-            ghstack.checkout.main(
-                pull_request=args.pull_request,
-                github=github,
-                sh=sh,
-                remote_name=conf.remote_name,
-            )
-        else:
-            raise RuntimeError("Unrecognized command {}".format(args.cmd))
+
+@main.command("action")
+@click.option("--close", is_flag=True, help="Close the specified pull request")
+@click.argument("pull_request", metavar="PR")
+def action(close: bool, pull_request: str) -> None:
+    """
+    Perform actions on a PR
+    """
+    with cli_context() as (shell, _, github):
+        ghstack.action.main(
+            pull_request=pull_request,
+            github=github,
+            sh=shell,
+            close=close,
+        )
+
+
+@main.command("checkout")
+@click.argument("pull_request", metavar="PR")
+def checkout(pull_request: str) -> None:
+    """
+    Checkout a PR
+    """
+    with cli_context() as (shell, config, github):
+        ghstack.checkout.main(
+            pull_request=pull_request,
+            github=github,
+            sh=shell,
+            remote_name=config.remote_name,
+        )
 
 
-if __name__ == "__main__":
-    main()
+@main.command("land")
+@click.option("--force", is_flag=True, help="force land even if the PR is closed")
+@click.argument("pull_request", metavar="PR")
+def land(force: bool, pull_request: str) -> None:
+    """
+    Land a PR stack
+    """
+    with cli_context() as (shell, config, github):
+        ghstack.land.main(
+            pull_request=pull_request,
+            github=github,
+            sh=shell,
+            github_url=config.github_url,
+            remote_name=config.remote_name,
+            force=force,
+        )
+
+
+@main.command("rage")
+@click.option(
+    "--latest",
+    is_flag=True,
+    help="Select the last command (not including rage commands) to report",
+)
+def rage(latest: bool) -> None:
+    with cli_context():
+        ghstack.rage.main(latest)
+
+
+@main.command("status")
+@click.argument("pull_request", metavar="PR")
+def status(pull_request: str):
+    """
+    Check status of a PR
+    """
+    with cli_context(request_circle_token=True) as (shell, config, github):
+        circleci = ghstack.circleci_real.RealCircleCIEndpoint(
+            circle_token=config.circle_token
+        )
+
+        fut = ghstack.status.main(
+            pull_request=pull_request,
+            github=github,
+            circleci=circleci,
+        )
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(fut)
+        loop.close()
+
+
+@main.command("submit")
+@click.option(
+    "--message",
+    "-m",
+    default="Update",
+    help="Description of change you made",
+)
+@click.option(
+    "--update-fields",
+    "-u",
+    is_flag=True,
+    help="Update GitHub pull request summary from the local commit",
+)
+@click.option(
+    "--short", is_flag=True, help="Print only the URL of the latest opened PR to stdout"
+)
+@click.option(
+    "--force",
+    is_flag=True,
+    help="force push the branch even if your local branch is stale",
+)
+@click.option(
+    "--no-skip",
+    is_flag=True,
+    help="Never skip pushing commits, even if the contents didn't change "
+    "(use this if you've only updated the commit message).",
+)
+@click.option(
+    "--draft",
+    is_flag=True,
+    help="Create the pull request in draft mode (only if it has not already been created)",
+)
+def submit(
+    message: str,
+    update_fields: bool,
+    short: bool,
+    force: bool,
+    no_skip: bool,
+    draft: bool,
+) -> None:
+    """
+    Submit or update a PR stack
+    """
+    with cli_context() as (shell, config, github):
+        ghstack.submit.main(
+            msg=message,
+            username=config.github_username,
+            sh=shell,
+            github=github,
+            update_fields=update_fields,
+            short=short,
+            force=force,
+            no_skip=no_skip,
+            draft=draft,
+            github_url=config.github_url,
+            remote_name=config.remote_name,
+        )
+
+
+@main.command("unlink")
+@click.argument("commits", nargs=-1, metavar="COMMIT")
+def unlink(commits: List[str]) -> None:
+    """
+    Unlink commits from PRs
+    """
+    with cli_context() as (shell, config, github):
+        ghstack.unlink.main(
+            commits=commits,
+            github=github,
+            sh=shell,
+            github_url=config.github_url,
+            remote_name=config.remote_name,
+        )
```

### Comparing `ghstack-0.7.1/ghstack/action.py` & `ghstack-0.8.0/ghstack/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,41 @@
 from typing import Optional
 
 import ghstack.github
 import ghstack.github_utils
 import ghstack.shell
 
 
-def main(pull_request: str,
-         github: ghstack.github.GitHubEndpoint,
-         sh: Optional[ghstack.shell.Shell] = None,
-         close: bool = False,
-         ) -> None:
+def main(
+    pull_request: str,
+    github: ghstack.github.GitHubEndpoint,
+    sh: Optional[ghstack.shell.Shell] = None,
+    close: bool = False,
+) -> None:
 
     params = ghstack.github_utils.parse_pull_request(pull_request)
-    pr_result = github.graphql("""
+    pr_result = github.graphql(
+        """
         query ($owner: String!, $name: String!, $number: Int!) {
             repository(name: $name, owner: $owner) {
                 pullRequest(number: $number) {
                     id
                 }
             }
         }
-    """, **params)
+    """,
+        **params
+    )
     pr_id = pr_result["data"]["repository"]["pullRequest"]["id"]
 
     if close:
         logging.info("Closing {owner}/{name}#{number}".format(**params))
-        github.graphql("""
+        github.graphql(
+            """
             mutation ($input: ClosePullRequestInput!) {
                 closePullRequest(input: $input) {
                     clientMutationId
                 }
             }
-        """, input={"pullRequestId": pr_id, "clientMutationId": "A"})
+        """,
+            input={"pullRequestId": pr_id, "clientMutationId": "A"},
+        )
```

### Comparing `ghstack-0.7.1/ghstack/cache.py` & `ghstack-0.8.0/ghstack/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,59 +11,66 @@
 _handle: Optional[sqlite3.Connection] = None
 CACHE_SIZE = 1000
 CURRENT_VERSION = 1
 
 
 def _db_conn() -> sqlite3.Connection:
     global _handle
-    fn = os.path.expanduser('~/.ghstackcache')
+    fn = os.path.expanduser("~/.ghstackcache")
     if not _handle:
         _handle = sqlite3.connect(fn)
         user_version = _handle.execute("PRAGMA user_version").fetchone()
         if user_version is None or user_version[0] != CURRENT_VERSION:
             _handle.close()
             os.remove(fn)
             _handle = sqlite3.connect(fn)
-            _handle.execute("""
+            _handle.execute(
+                """
             CREATE TABLE ghstack_cache (
                 id INTEGER PRIMARY KEY AUTOINCREMENT,
                 domain TEXT,
                 key TEXT,
                 value TEXT
             )
-            """)
-            _handle.execute("""
+            """
+            )
+            _handle.execute(
+                """
             CREATE UNIQUE INDEX domain_key ON ghstack_cache (domain, key)
-            """)
+            """
+            )
             _handle.execute("PRAGMA user_version = {}".format(CURRENT_VERSION))
             _handle.commit()
     return _handle
 
 
 def get(domain: str, key: str) -> Optional[str]:
     conn = _db_conn()
     c = conn.execute(
-        "SELECT value FROM ghstack_cache WHERE domain = ? AND key = ?",
-        (domain, key))
+        "SELECT value FROM ghstack_cache WHERE domain = ? AND key = ?", (domain, key)
+    )
     r = c.fetchone()
     if r is None:
         return None
     r = r[0]
-    assert(isinstance(r, str))
+    assert isinstance(r, str)
     return r
 
 
 def put(domain: str, key: str, value: str) -> None:
     conn = _db_conn()
     conn.execute(
         "UPDATE ghstack_cache SET value = ? WHERE domain = ? AND key = ?",
-        (value, domain, key))
+        (value, domain, key),
+    )
     c = conn.execute(
         """
         INSERT INTO ghstack_cache (domain, key, value)
         SELECT ?, ?, ? WHERE (SELECT Changes() = 0)
         """,
-        (domain, key, value))
+        (domain, key, value),
+    )
     if c.lastrowid is not None:
         conn.execute(
-            "DELETE FROM ghstack_cache WHERE id < ?", (c.lastrowid - CACHE_SIZE, ))
+            "DELETE FROM ghstack_cache WHERE id < ?", (c.lastrowid - CACHE_SIZE,)
+        )
     conn.commit()
```

### Comparing `ghstack-0.7.1/ghstack/checkout.py` & `ghstack-0.8.0/ghstack/checkout.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 import re
 
 import ghstack.github
 import ghstack.github_utils
 import ghstack.shell
 
 
-def main(pull_request: str,
-         github: ghstack.github.GitHubEndpoint,
-         sh: ghstack.shell.Shell,
-         remote_name: str,
-         ) -> None:
+def main(
+    pull_request: str,
+    github: ghstack.github.GitHubEndpoint,
+    sh: ghstack.shell.Shell,
+    remote_name: str,
+) -> None:
 
     params = ghstack.github_utils.parse_pull_request(pull_request)
-    pr_result = github.graphql("""
+    pr_result = github.graphql(
+        """
         query ($owner: String!, $name: String!, $number: Int!) {
             repository(name: $name, owner: $owner) {
                 pullRequest(number: $number) {
                     headRefName
                 }
             }
         }
-    """, **params)
+    """,
+        **params
+    )
     head_ref = pr_result["data"]["repository"]["pullRequest"]["headRefName"]
-    orig_ref = re.sub(r'/head$', '/orig', head_ref)
+    orig_ref = re.sub(r"/head$", "/orig", head_ref)
     if orig_ref == head_ref:
-        logging.warning("The ref {} doesn't look like a ghstack reference".format(head_ref))
+        logging.warning(
+            "The ref {} doesn't look like a ghstack reference".format(head_ref)
+        )
 
     # TODO: Handle remotes correctly too (so this subsumes hub)
 
     sh.git("fetch", "--prune", remote_name)
     sh.git("checkout", remote_name + "/" + orig_ref)
```

### Comparing `ghstack-0.7.1/ghstack/circleci.py` & `ghstack-0.8.0/ghstack/circleci.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 class CircleCIEndpoint(metaclass=ABCMeta):
     async def get(self, path: str, **kwargs: Any) -> Any:
         """
         Send a GET request to endpoint 'path'.
 
         Returns: parsed JSON response
         """
-        return await self.rest('get', path, **kwargs)
+        return await self.rest("get", path, **kwargs)
 
     async def post(self, path: str, **kwargs: Any) -> Any:
         """
         Send a POST request to endpoint 'path'.
 
         Returns: parsed JSON response
         """
-        return await self.rest('post', path, **kwargs)
+        return await self.rest("post", path, **kwargs)
 
     @abstractmethod
     async def rest(self, method: str, path: str, **kwargs: Any) -> Any:
         """
         Send a 'method' request to endpoint 'path'.
 
         Args:
```

### Comparing `ghstack-0.7.1/ghstack/circleci_real.py` & `ghstack-0.8.0/ghstack/circleci_real.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,65 +6,64 @@
 from typing import Any, Optional
 
 import aiohttp
 
 import ghstack.cache
 import ghstack.circleci
 
-RE_BUILD_PATH = re.compile(r'^project/github/[^/]+/[^/]+/[0-9]+$')
+RE_BUILD_PATH = re.compile(r"^project/github/[^/]+/[^/]+/[0-9]+$")
 
 
 class RealCircleCIEndpoint(ghstack.circleci.CircleCIEndpoint):
-    rest_endpoint: str = 'https://circleci.com/api/v1.1'
+    rest_endpoint: str = "https://circleci.com/api/v1.1"
 
     # The API token to authenticate to CircleCI with
     # https://circleci.com/account/api
     circle_token: Optional[str]
 
     # The URL of a proxy to use for these connections (for
     # Facebook users, this is typically 'http://fwdproxy:8080')
     proxy: Optional[str]
 
-    def __init__(self,
-                 *,
-                 circle_token: Optional[str] = None,
-                 proxy: Optional[str] = None):
+    def __init__(
+        self, *, circle_token: Optional[str] = None, proxy: Optional[str] = None
+    ):
         self.circle_token = circle_token
         self.proxy = proxy
 
     async def rest(self, method: str, path: str, **kwargs: Any) -> Any:
         headers = {
-            'Content-Type': 'application/json',
-            'User-Agent': 'ghstack',
+            "Content-Type": "application/json",
+            "User-Agent": "ghstack",
         }
 
-        url = self.rest_endpoint + '/' + path
+        url = self.rest_endpoint + "/" + path
         logging.debug("# {} {}".format(method, url))
         logging.debug("Request body:\n{}".format(json.dumps(kwargs, indent=1)))
 
         params = {}
         if self.circle_token:
-            params['circle-token'] = self.circle_token
+            params["circle-token"] = self.circle_token
 
-        is_get_build = method == 'get' and RE_BUILD_PATH.match(path)
+        is_get_build = method == "get" and RE_BUILD_PATH.match(path)
 
         if is_get_build:
             # consult cache
-            cache_result = ghstack.cache.get('circleci', path)
+            cache_result = ghstack.cache.get("circleci", path)
             if cache_result is not None:
                 logging.debug("Retrieved result from cache")
                 return json.loads(cache_result)
 
         async with aiohttp.request(
-                method.upper(),
-                url,
-                params=params,
-                json=kwargs,
-                headers=headers,
-                proxy=self.proxy,
+            method.upper(),
+            url,
+            params=params,
+            json=kwargs,
+            headers=headers,
+            proxy=self.proxy,
         ) as resp:
             logging.debug("Response status: {}".format(resp.status))
 
             r_text = await resp.text()
 
             try:
                 r = json.loads(r_text)
@@ -79,10 +78,10 @@
                 resp.raise_for_status()
             except aiohttp.ClientResponseError:
                 raise RuntimeError(pretty_json)
 
             # NB: Don't save to cache if it's still running
             if is_get_build and r["outcome"] is not None:
                 logging.debug("Saving result to cache")
-                ghstack.cache.put('circleci', path, r_text)
+                ghstack.cache.put("circleci", path, r_text)
 
             return r
```

### Comparing `ghstack-0.7.1/ghstack/diff.py` & `ghstack-0.8.0/ghstack/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,43 +5,47 @@
 from dataclasses import dataclass
 from typing import Optional, Pattern
 
 import ghstack.shell
 from ghstack.types import GitHubNumber, GitTreeHash
 
 RE_GH_METADATA = re.compile(
-    r'gh-metadata: (?P<owner>[^/]+) (?P<repo>[^/]+) (?P<number>[0-9]+) '
-    r'gh/(?P<username>[a-zA-Z0-9-]+)/(?P<ghnum>[0-9]+)/head', re.MULTILINE)
+    r"gh-metadata: (?P<owner>[^/]+) (?P<repo>[^/]+) (?P<number>[0-9]+) "
+    r"gh/(?P<username>[a-zA-Z0-9-]+)/(?P<ghnum>[0-9]+)/head",
+    re.MULTILINE,
+)
 
 
 RAW_PULL_REQUEST_RESOLVED = (
-    r'Pull Request resolved: '
-    r'https://{github_url}/(?P<owner>[^/]+)/(?P<repo>[^/]+)/pull/(?P<number>[0-9]+)'
+    r"Pull Request resolved: "
+    r"https://{github_url}/(?P<owner>[^/]+)/(?P<repo>[^/]+)/pull/(?P<number>[0-9]+)"
 )
 
 
 def re_pull_request_resolved(github_url: str) -> Pattern[str]:
     return re.compile(RAW_PULL_REQUEST_RESOLVED.format(github_url=github_url))
 
 
 def re_pull_request_resolved_w_sp(github_url: str) -> Pattern[str]:
-    return re.compile(r'\n*' + RAW_PULL_REQUEST_RESOLVED.format(github_url=github_url))
+    return re.compile(r"\n*" + RAW_PULL_REQUEST_RESOLVED.format(github_url=github_url))
 
 
 @dataclass
 class PullRequestResolved:
     owner: str
     repo: str
     number: GitHubNumber
 
     def url(self, github_url: str) -> str:
-        return "https://{}/{}/{}/pull/{}".format(github_url, self.owner, self.repo, self.number)
+        return "https://{}/{}/{}/pull/{}".format(
+            github_url, self.owner, self.repo, self.number
+        )
 
     @staticmethod
-    def search(s: str, github_url: str) -> Optional['PullRequestResolved']:
+    def search(s: str, github_url: str) -> Optional["PullRequestResolved"]:
         m = re_pull_request_resolved(github_url).search(s)
         if m is not None:
             return PullRequestResolved(
                 owner=m.group("owner"),
                 repo=m.group("repo"),
                 number=GitHubNumber(int(m.group("number"))),
             )
@@ -56,25 +60,27 @@
 
 
 class Patch(metaclass=ABCMeta):
     """
     Abstract representation of a patch, i.e., some actual
     change between two trees.
     """
+
     @abstractmethod
     def apply(self, sh: ghstack.shell.Shell, h: GitTreeHash) -> GitTreeHash:
         pass
 
 
 @dataclass
 class Diff:
     """
     An abstract representation of a diff.  Diffs can come from
     git or hg.
     """
+
     # Title of the diff
     title: str
 
     # Detailed description of the diff.  Includes the title.
     summary: str
 
     # Unique identifier representing the commit in question (may be a
```

### Comparing `ghstack-0.7.1/ghstack/forensics.py` & `ghstack-0.8.0/ghstack/forensics.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 
 import aiohttp
 
 import ghstack.circleci
 import ghstack.github
 import ghstack.github_utils
 
-RE_CIRCLECI_URL = re.compile(r'^https://circleci.com/gh/pytorch/pytorch/([0-9]+)')
+RE_CIRCLECI_URL = re.compile(r"^https://circleci.com/gh/pytorch/pytorch/([0-9]+)")
 
 
 def strip_sccache(x: str) -> str:
     sccache_marker = "=================== sccache compilation log ==================="
     marker_pos = x.rfind(sccache_marker)
-    newline_before_marker_pos = x.rfind('\n', 0, marker_pos)
+    newline_before_marker_pos = x.rfind("\n", 0, marker_pos)
     return x[:newline_before_marker_pos]
 
 
-async def main(pull_request: str,
-         github: ghstack.github.GitHubEndpoint,
-         circleci: ghstack.circleci.CircleCIEndpoint) -> None:
+async def main(
+    pull_request: str,
+    github: ghstack.github.GitHubEndpoint,
+    circleci: ghstack.circleci.CircleCIEndpoint,
+) -> None:
 
     # Game plan:
     # 1. Query GitHub to find out what the current statuses are
     #       (TODO: if we got rate limited we'll miss stuff)
     # 2. For each status in parallel:
     #   a. Query CircleCI for job status
     #   b. (Future work) Query output_url to get log information
@@ -43,15 +45,16 @@
     #         to see if there were other options, there did not appear
     #         to be any indication that a halt was called.  So we'll
     #         have to rely on the (OS X jobs, take note!)
 
     params = ghstack.github_utils.parse_pull_request(pull_request)
 
     # TODO: stop hard-coding number of commits
-    r = github.graphql("""
+    r = github.graphql(
+        """
     query ($name: String!, $owner: String!, $number: Int!) {
         repository(name: $name, owner: $owner) {
             pullRequest(number: $number) {
                 commits(last: 100) {
                     nodes {
                         commit {
                             oid
@@ -65,52 +68,62 @@
                             }
                         }
                     }
                 }
             }
         }
     }
-    """, **params)
-    nodes = r['data']['repository']['pullRequest']['commits']['nodes']
+    """,
+        **params
+    )
+    nodes = r["data"]["repository"]["pullRequest"]["commits"]["nodes"]
 
     async def process_node(n: Dict[str, Any]) -> str:
-        commit = n['commit']
-        status = commit['status']
+        commit = n["commit"]
+        status = commit["status"]
         icon = "❔"
         text = ""
         buildid_text = ""
         if status is not None:
-            contexts = status['contexts']
+            contexts = status["contexts"]
         else:
             contexts = []
         for c in contexts:
             # TODO: Stop hard-coding me
-            if c['context'] != 'ci/circleci: pytorch_linux_xenial_py3_clang5_asan_test':
+            if c["context"] != "ci/circleci: pytorch_linux_xenial_py3_clang5_asan_test":
                 continue
-            m = RE_CIRCLECI_URL.match(c['targetUrl'])
+            m = RE_CIRCLECI_URL.match(c["targetUrl"])
             if not m:
                 icon = "🍆"
                 break
-            if c['state'] == 'SUCCESS':
+            if c["state"] == "SUCCESS":
                 icon = "✅"
                 break
             buildid = m.group(1)
             buildid_text = " ({})".format(buildid)
-            r = await circleci.get("project/github/{name}/{owner}/{buildid}".format(buildid=buildid, **params))
+            r = await circleci.get(
+                "project/github/{name}/{owner}/{buildid}".format(
+                    buildid=buildid, **params
+                )
+            )
             if not r["failed"]:
                 # It was just cancelled (don't check "cancelled"; that's
                 # true even if the job failed otherwise; it just means
                 # workflow got cancelled)
                 icon = "❔"
                 break
             icon = "❌"
-            async with aiohttp.request('get', r['steps'][-1]['actions'][-1]['output_url']) as resp:
+            async with aiohttp.request(
+                "get", r["steps"][-1]["actions"][-1]["output_url"]
+            ) as resp:
                 log_json = await resp.json()
                 buf = []
                 for e in log_json:
                     buf.append(e["message"])
                 text = "\n" + strip_sccache("\n".join(buf))
                 text = text[-1500:]
-        return "{} {} {}{}{}".format(icon, commit['oid'][:8], commit['messageHeadline'], buildid_text, text)
+        return "{} {} {}{}{}".format(
+            icon, commit["oid"][:8], commit["messageHeadline"], buildid_text, text
+        )
 
     for n in nodes:
         print(await process_node(n))
```

### Comparing `ghstack-0.7.1/ghstack/git.py` & `ghstack-0.8.0/ghstack/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import re
 from typing import List, Pattern
 
 import ghstack.diff
 import ghstack.shell
 from ghstack.types import GitCommitHash, GitTreeHash
 
-RE_RAW_COMMIT_ID = re.compile(r'^(?P<commit>[a-f0-9]+)$', re.MULTILINE)
-RE_RAW_AUTHOR = re.compile(r'^author (?P<author>(?P<name>[^<]+?) <(?P<email>[^>]+)>)',
-                           re.MULTILINE)
-RE_RAW_PARENT = re.compile(r'^parent (?P<commit>[a-f0-9]+)$', re.MULTILINE)
-RE_RAW_TREE = re.compile(r'^tree (?P<tree>.+)$', re.MULTILINE)
-RE_RAW_COMMIT_MSG_LINE = re.compile(r'^    (?P<line>.*)$', re.MULTILINE)
+RE_RAW_COMMIT_ID = re.compile(r"^(?P<commit>[a-f0-9]+)$", re.MULTILINE)
+RE_RAW_AUTHOR = re.compile(
+    r"^author (?P<author>(?P<name>[^<]+?) <(?P<email>[^>]+)>)", re.MULTILINE
+)
+RE_RAW_PARENT = re.compile(r"^parent (?P<commit>[a-f0-9]+)$", re.MULTILINE)
+RE_RAW_TREE = re.compile(r"^tree (?P<tree>.+)$", re.MULTILINE)
+RE_RAW_COMMIT_MSG_LINE = re.compile(r"^    (?P<line>.*)$", re.MULTILINE)
 
 
 class CommitHeader(object):
     """
     Represents the information extracted from `git rev-list --header`
     """
+
     # The unparsed output from git rev-list --header
     raw_header: str
 
     def __init__(self, raw_header: str):
         self.raw_header = raw_header
 
     def _search_group(self, regex: Pattern[str], group: str) -> str:
@@ -33,65 +35,72 @@
     def tree(self) -> GitTreeHash:
         return GitTreeHash(self._search_group(RE_RAW_TREE, "tree"))
 
     def title(self) -> str:
         return self._search_group(RE_RAW_COMMIT_MSG_LINE, "line")
 
     def commit_id(self) -> GitCommitHash:
-        return GitCommitHash(
-            self._search_group(RE_RAW_COMMIT_ID, "commit"))
+        return GitCommitHash(self._search_group(RE_RAW_COMMIT_ID, "commit"))
 
     def parents(self) -> List[GitCommitHash]:
-        return [GitCommitHash(m.group("commit"))
-                for m in RE_RAW_PARENT.finditer(self.raw_header)]
+        return [
+            GitCommitHash(m.group("commit"))
+            for m in RE_RAW_PARENT.finditer(self.raw_header)
+        ]
 
     def author(self) -> str:
         return self._search_group(RE_RAW_AUTHOR, "author")
 
     def author_name(self) -> str:
         return self._search_group(RE_RAW_AUTHOR, "name")
 
     def author_email(self) -> str:
         return self._search_group(RE_RAW_AUTHOR, "email")
 
     def commit_msg(self) -> str:
-        return '\n'.join(
-            m.group("line")
-            for m in RE_RAW_COMMIT_MSG_LINE.finditer(self.raw_header))
+        return "\n".join(
+            m.group("line") for m in RE_RAW_COMMIT_MSG_LINE.finditer(self.raw_header)
+        )
 
 
 def split_header(s: str) -> List[CommitHeader]:
     return list(map(CommitHeader, s.split("\0")[:-1]))
 
 
 class GitPatch(ghstack.diff.Patch):
     h: CommitHeader
 
     def __init__(self, h: CommitHeader):
         self.h = h
 
     def apply(self, sh: ghstack.shell.Shell, base_tree: GitTreeHash) -> GitTreeHash:
         expected_tree = sh.git("rev-parse", self.h.commit_id() + "~^{tree}")
-        assert expected_tree == base_tree, \
-            "expected_tree = {}, base_tree = {}".format(expected_tree, base_tree)
+        assert expected_tree == base_tree, "expected_tree = {}, base_tree = {}".format(
+            expected_tree, base_tree
+        )
         return self.h.tree()
 
 
 def parse_header(s: str, github_url: str) -> List[ghstack.diff.Diff]:
     def convert(h: CommitHeader) -> ghstack.diff.Diff:
         parents = h.parents()
         if len(parents) != 1:
             raise RuntimeError(
                 "The commit {} has {} parents, which makes my head explode.  "
-                "`git rebase -i` your diffs into a stack, then try again."
-                .format(h.commit_id(), len(parents)))
+                "`git rebase -i` your diffs into a stack, then try again.".format(
+                    h.commit_id(), len(parents)
+                )
+            )
         return ghstack.diff.Diff(
             title=h.title(),
             summary=h.commit_msg(),
             oid=h.commit_id(),
             source_id=h.tree(),
-            pull_request_resolved=ghstack.diff.PullRequestResolved.search(h.raw_header, github_url),
+            pull_request_resolved=ghstack.diff.PullRequestResolved.search(
+                h.raw_header, github_url
+            ),
             patch=GitPatch(h),
             author_name=h.author_name(),
-            author_email=h.author_email()
+            author_email=h.author_email(),
         )
+
     return list(map(convert, split_header(s)))
```

### Comparing `ghstack-0.7.1/ghstack/github.py` & `ghstack-0.8.0/ghstack/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,31 +38,31 @@
 
     def get(self, path: str, **kwargs: Any) -> Any:
         """
         Send a GET request to endpoint 'path'.
 
         Returns: parsed JSON response
         """
-        return self.rest('get', path, **kwargs)
+        return self.rest("get", path, **kwargs)
 
     def post(self, path: str, **kwargs: Any) -> Any:
         """
         Send a POST request to endpoint 'path'.
 
         Returns: parsed JSON response
         """
-        return self.rest('post', path, **kwargs)
+        return self.rest("post", path, **kwargs)
 
     def patch(self, path: str, **kwargs: Any) -> Any:
         """
         Send a PATCH request to endpoint 'path'.
 
         Returns: parsed JSON response
         """
-        return self.rest('patch', path, **kwargs)
+        return self.rest("patch", path, **kwargs)
 
     @abstractmethod
     def rest(self, method: str, path: str, **kwargs: Any) -> Any:
         """
         Send a 'method' request to endpoint 'path'.
 
         Args:
```

### Comparing `ghstack-0.7.1/ghstack/github_fake.py` & `ghstack-0.8.0/ghstack/github_fake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,87 @@
 #!/usr/bin/env python3
 
 import os.path
 import re
-from dataclasses import dataclass  # Oof! Python 3.7 only!!
-from typing import Any, Dict, List, NewType, Optional, Sequence, cast
+from dataclasses import dataclass
+from typing import Any, cast, Dict, List, NewType, Optional, Sequence
 
 import graphql
 from typing_extensions import TypedDict
 
 import ghstack.diff
 import ghstack.github
 import ghstack.shell
 
-GraphQLId = NewType('GraphQLId', str)
-GitHubNumber = NewType('GitHubNumber', int)
-GitObjectID = NewType('GitObjectID', str)
+GraphQLId = NewType("GraphQLId", str)
+GitHubNumber = NewType("GitHubNumber", int)
+GitObjectID = NewType("GitObjectID", str)
 
 # https://stackoverflow.com/a/55250601
-SetDefaultBranchInput = TypedDict('SetDefaultBranchInput', {
-    'name': str,
-    'default_branch': str,
-})
-
-UpdatePullRequestInput = TypedDict('UpdatePullRequestInput', {
-    'base': Optional[str],
-    'title': Optional[str],
-    'body': Optional[str],
-})
-
-CreatePullRequestInput = TypedDict('CreatePullRequestInput', {
-    'base': str,
-    'head': str,
-    'title': str,
-    'body': str,
-    'maintainer_can_modify': bool,
-})
-
-CreatePullRequestPayload = TypedDict('CreatePullRequestPayload', {
-    'number': int,
-})
+SetDefaultBranchInput = TypedDict(
+    "SetDefaultBranchInput",
+    {
+        "name": str,
+        "default_branch": str,
+    },
+)
+
+UpdatePullRequestInput = TypedDict(
+    "UpdatePullRequestInput",
+    {
+        "base": Optional[str],
+        "title": Optional[str],
+        "body": Optional[str],
+    },
+)
+
+CreatePullRequestInput = TypedDict(
+    "CreatePullRequestInput",
+    {
+        "base": str,
+        "head": str,
+        "title": str,
+        "body": str,
+        "maintainer_can_modify": bool,
+    },
+)
+
+CreatePullRequestPayload = TypedDict(
+    "CreatePullRequestPayload",
+    {
+        "number": int,
+    },
+)
 
 
 # The "database" for our mock instance
 class GitHubState:
-    repositories: Dict[GraphQLId, 'Repository']
-    pull_requests: Dict[GraphQLId, 'PullRequest']
+    repositories: Dict[GraphQLId, "Repository"]
+    pull_requests: Dict[GraphQLId, "PullRequest"]
     _next_id: int
     _next_pull_request_number: Dict[GraphQLId, int]
-    root: 'Root'
+    root: "Root"
     upstream_sh: Optional[ghstack.shell.Shell]
 
-    def repository(self, owner: str, name: str) -> 'Repository':
+    def repository(self, owner: str, name: str) -> "Repository":
         nameWithOwner = "{}/{}".format(owner, name)
         for r in self.repositories.values():
             if r.nameWithOwner == nameWithOwner:
                 return r
         raise RuntimeError("unknown repository {}".format(nameWithOwner))
 
-    def pull_request(self, repo: 'Repository', number: GitHubNumber
-                     ) -> 'PullRequest':
+    def pull_request(self, repo: "Repository", number: GitHubNumber) -> "PullRequest":
         for pr in self.pull_requests.values():
             if repo.id == pr._repository and pr.number == number:
                 return pr
         raise RuntimeError(
-            "unrecognized pull request #{} in repository {}"
-            .format(number, repo.nameWithOwner))
+            "unrecognized pull request #{} in repository {}".format(
+                number, repo.nameWithOwner
+            )
+        )
 
     def next_id(self) -> GraphQLId:
         r = GraphQLId(str(self._next_id))
         self._next_id += 1
         return r
 
     def next_pull_request_number(self, repo_id: GraphQLId) -> GitHubNumber:
@@ -115,18 +128,15 @@
             # pytorch/pytorch repository in the directory specified
             # by upstream_sh.  This is useful because some GitHub API
             # operations depend on repository state (e.g., what
             # the headRef is at the time a PR is created), so
             # we need this information
             self.upstream_sh.git("init", "--bare", "-b", "master")
             tree = self.upstream_sh.git("write-tree")
-            commit = self.upstream_sh.git(
-                "commit-tree",
-                tree,
-                input="Initial commit")
+            commit = self.upstream_sh.git("commit-tree", tree, input="Initial commit")
             self.upstream_sh.git("branch", "-f", "master", commit)
 
             # We only update this when a PATCH changes the default
             # branch; hopefully that's fine?  In any case, it should
             # work for now since currently we only ever access the name
             # of the default branch rather than other parts of its ref.
             repo.defaultBranchRef = repo._make_ref(self, "master")
@@ -147,38 +157,42 @@
 
 
 @dataclass
 class Repository(Node):
     name: str
     nameWithOwner: str
     isFork: bool
-    defaultBranchRef: Optional['Ref']
+    defaultBranchRef: Optional["Ref"]
 
-    def pullRequest(self,
-                    info: GraphQLResolveInfo,
-                    number: GitHubNumber) -> 'PullRequest':
+    def pullRequest(
+        self, info: GraphQLResolveInfo, number: GitHubNumber
+    ) -> "PullRequest":
         return github_state(info).pull_request(self, number)
 
-    def pullRequests(self, info: GraphQLResolveInfo
-                     ) -> 'PullRequestConnection':
-        return PullRequestConnection(nodes=list(filter(
-            lambda pr: self == pr.repository(info),
-            github_state(info).pull_requests.values())))
+    def pullRequests(self, info: GraphQLResolveInfo) -> "PullRequestConnection":
+        return PullRequestConnection(
+            nodes=list(
+                filter(
+                    lambda pr: self == pr.repository(info),
+                    github_state(info).pull_requests.values(),
+                )
+            )
+        )
 
     # TODO: This should take which repository the ref is in
     # This only works if you have upstream_sh
-    def _make_ref(self, state: GitHubState, refName: str) -> 'Ref':
+    def _make_ref(self, state: GitHubState, refName: str) -> "Ref":
         # TODO: Probably should preserve object identity here when
         # you call this with refName/oid that are the same
         assert state.upstream_sh
         gitObject = GitObject(
             id=state.next_id(),
             # TODO: this upstream_sh hardcode wrong, but ok for now
             # because we only have one repo
-            oid=GitObjectID(state.upstream_sh.git('rev-parse', refName)),
+            oid=GitObjectID(state.upstream_sh.git("rev-parse", refName)),
             _repository=self.id,
         )
         ref = Ref(
             id=state.next_id(),
             name=refName,
             _repository=self.id,
             target=gitObject,
@@ -227,29 +241,29 @@
 
 @dataclass
 class PullRequestConnection:
     nodes: List[PullRequest]
 
 
 class Root:
-    def repository(self, info: GraphQLResolveInfo, owner: str,
-                   name: str) -> Repository:
+    def repository(self, info: GraphQLResolveInfo, owner: str, name: str) -> Repository:
         return github_state(info).repository(owner, name)
 
     def node(self, info: GraphQLResolveInfo, id: GraphQLId) -> Node:
         if id in github_state(info).repositories:
             return github_state(info).repositories[id]
         elif id in github_state(info).pull_requests:
             return github_state(info).pull_requests[id]
         else:
             raise RuntimeError("unknown id {}".format(id))
 
 
-with open(os.path.join(os.path.dirname(__file__),
-          'github_schema.graphql'), encoding='utf-8') as f:
+with open(
+    os.path.join(os.path.dirname(__file__), "github_schema.graphql"), encoding="utf-8"
+) as f:
     GITHUB_SCHEMA = graphql.build_schema(f.read())
 
 
 # Ummm.  I thought there would be a way to stick these on the objects
 # themselves (in the same way resolvers can be put on resolvers) but
 # after a quick read of default_resolve_type_fn it doesn't look like
 # we ever actually look to value for type of information.  This is
@@ -257,131 +271,138 @@
 def set_is_type_of(name: str, cls: Any) -> None:
     # Can't use a type ignore on the next line because fbcode
     # and us don't agree that it's necessary hmm.
     o: Any = GITHUB_SCHEMA.get_type(name)
     o.is_type_of = lambda obj, info: isinstance(obj, cls)
 
 
-set_is_type_of('Repository', Repository)
-set_is_type_of('PullRequest', PullRequest)
+set_is_type_of("Repository", Repository)
+set_is_type_of("PullRequest", PullRequest)
 
 
 class FakeGitHubEndpoint(ghstack.github.GitHubEndpoint):
     state: GitHubState
 
-    def __init__(self,
-                 upstream_sh: Optional[ghstack.shell.Shell] = None
-                 ) -> None:
+    def __init__(self, upstream_sh: Optional[ghstack.shell.Shell] = None) -> None:
         self.state = GitHubState(upstream_sh)
 
     def graphql(self, query: str, **kwargs: Any) -> Any:
         r = graphql.graphql_sync(
             schema=GITHUB_SCHEMA,
             source=query,
             root_value=self.state.root,
             context_value=self.state,
-            variable_values=kwargs)
+            variable_values=kwargs,
+        )
         if r.errors:
             # The GraphQL implementation loses all the stack traces!!!
             # D:  You can 'recover' them by deleting the
             # 'except Exception as error' from GraphQL-core-next; need
             # to file a bug report
-            raise RuntimeError("GraphQL query failed with errors:\n\n{}"
-                               .format("\n".join(str(e) for e in r.errors)))
+            raise RuntimeError(
+                "GraphQL query failed with errors:\n\n{}".format(
+                    "\n".join(str(e) for e in r.errors)
+                )
+            )
         # The top-level object isn't indexable by strings, but
         # everything underneath is, oddly enough
-        return {'data': r.data}
+        return {"data": r.data}
 
     def push_hook(self, refNames: Sequence[str]) -> None:
         self.state.push_hook(refNames)
 
     def notify_merged(self, pr_resolved: ghstack.diff.PullRequestResolved) -> None:
         self.state.notify_merged(pr_resolved)
 
-    def _create_pull(self, owner: str, name: str,
-                     input: CreatePullRequestInput) -> CreatePullRequestPayload:
+    def _create_pull(
+        self, owner: str, name: str, input: CreatePullRequestInput
+    ) -> CreatePullRequestPayload:
         state = self.state
         id = state.next_id()
         repo = state.repository(owner, name)
         number = state.next_pull_request_number(repo.id)
         baseRef = None
         headRef = None
         # TODO: When we support forks, this needs rewriting to stop
         # hard coded the repo we opened the pull request on
         if state.upstream_sh:
-            baseRef = repo._make_ref(state, input['base'])
-            headRef = repo._make_ref(state, input['head'])
+            baseRef = repo._make_ref(state, input["base"])
+            headRef = repo._make_ref(state, input["head"])
         pr = PullRequest(
             id=id,
             _repository=repo.id,
             number=number,
             closed=False,
-            url="https://github.com/{}/pull/{}"
-                .format(repo.nameWithOwner, number),
+            url="https://github.com/{}/pull/{}".format(repo.nameWithOwner, number),
             baseRef=baseRef,
-            baseRefName=input['base'],
+            baseRefName=input["base"],
             headRef=headRef,
-            headRefName=input['head'],
-            title=input['title'],
-            body=input['body'],
+            headRefName=input["head"],
+            title=input["title"],
+            body=input["body"],
         )
         # TODO: compute files changed
         state.pull_requests[id] = pr
         # This is only a subset of what the actual REST endpoint
         # returns.
         return {
-            'number': number,
+            "number": number,
         }
 
     # NB: This technically does have a payload, but we don't
     # use it so I didn't bother constructing it.
-    def _update_pull(self, owner: str, name: str, number: GitHubNumber,
-                     input: UpdatePullRequestInput) -> None:
+    def _update_pull(
+        self, owner: str, name: str, number: GitHubNumber, input: UpdatePullRequestInput
+    ) -> None:
         state = self.state
         repo = state.repository(owner, name)
         pr = state.pull_request(repo, number)
         # If I say input.get('title') is not None, mypy
         # is unable to infer input['title'] is not None
-        if 'title' in input and input['title'] is not None:
-            pr.title = input['title']
-        if 'base' in input and input['base'] is not None:
-            pr.baseRefName = input['base']
+        if "title" in input and input["title"] is not None:
+            pr.title = input["title"]
+        if "base" in input and input["base"] is not None:
+            pr.baseRefName = input["base"]
             pr.baseRef = repo._make_ref(state, pr.baseRefName)
-        if 'body' in input and input['body'] is not None:
-            pr.body = input['body']
+        if "body" in input and input["body"] is not None:
+            pr.body = input["body"]
 
     # NB: This may have a payload, but we don't
     # use it so I didn't bother constructing it.
-    def _set_default_branch(self, owner: str, name: str,
-                            input: SetDefaultBranchInput) -> None:
+    def _set_default_branch(
+        self, owner: str, name: str, input: SetDefaultBranchInput
+    ) -> None:
         state = self.state
         repo = state.repository(owner, name)
-        repo.defaultBranchRef = repo._make_ref(state, input['default_branch'])
+        repo.defaultBranchRef = repo._make_ref(state, input["default_branch"])
 
     def rest(self, method: str, path: str, **kwargs: Any) -> Any:
-        if method == 'get':
-            m = re.match(r'^repos/([^/]+)/([^/]+)/branches/([^/]+)/protection', path)
+        if method == "get":
+            m = re.match(r"^repos/([^/]+)/([^/]+)/branches/([^/]+)/protection", path)
             if m:
                 # For now, pretend all branches are not protected
                 raise ghstack.github.NotFoundError()
 
-        elif method == 'post':
-            m = re.match(r'^repos/([^/]+)/([^/]+)/pulls$', path)
+        elif method == "post":
+            m = re.match(r"^repos/([^/]+)/([^/]+)/pulls$", path)
             if m:
-                return self._create_pull(m.group(1), m.group(2),
-                                         cast(CreatePullRequestInput, kwargs))
-        elif method == 'patch':
-            m = re.match(r'^repos/([^/]+)/([^/]+)(?:/pulls/([^/]+))?$', path)
+                return self._create_pull(
+                    m.group(1), m.group(2), cast(CreatePullRequestInput, kwargs)
+                )
+        elif method == "patch":
+            m = re.match(r"^repos/([^/]+)/([^/]+)(?:/pulls/([^/]+))?$", path)
             if m:
                 owner, name, number = m.groups()
                 if number is not None:
                     return self._update_pull(
-                        owner, name, GitHubNumber(int(number)),
-                        cast(UpdatePullRequestInput, kwargs))
-                elif 'default_branch' in kwargs:
+                        owner,
+                        name,
+                        GitHubNumber(int(number)),
+                        cast(UpdatePullRequestInput, kwargs),
+                    )
+                elif "default_branch" in kwargs:
                     return self._set_default_branch(
-                        owner, name,
-                        cast(SetDefaultBranchInput, kwargs))
+                        owner, name, cast(SetDefaultBranchInput, kwargs)
+                    )
         raise NotImplementedError(
-            "FakeGitHubEndpoint REST {} {} not implemented"
-            .format(method.upper(), path)
+            "FakeGitHubEndpoint REST {} {} not implemented".format(method.upper(), path)
         )
```

### Comparing `ghstack-0.7.1/ghstack/github_real.py` & `ghstack-0.8.0/ghstack/github_real.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 class RealGitHubEndpoint(ghstack.github.GitHubEndpoint):
     """
     A class representing a GitHub endpoint we can send queries to.
     It supports both GraphQL and REST interfaces.
     """
 
     # The URL of the GraphQL endpoint to connect to
-    graphql_endpoint: str = 'https://api.{github_url}/graphql'
+    graphql_endpoint: str = "https://api.{github_url}/graphql"
 
     # The base URL of the REST endpoint to connect to (all REST requests
     # will be subpaths of this URL)
-    rest_endpoint: str = 'https://api.{github_url}'
+    rest_endpoint: str = "https://api.{github_url}"
 
     # The string OAuth token to authenticate to the GraphQL server with
     oauth_token: str
 
     # The URL of a proxy to use for these connections (for
     # Facebook users, this is typically 'http://fwdproxy:8080')
     proxy: Optional[str]
@@ -33,46 +33,48 @@
     # Passed to requests as 'verify'.
     verify: Optional[str]
 
     # Client side certificate to use when connecitng.
     # Passed to requests as 'cert'.
     cert: Optional[Union[str, Tuple[str, str]]]
 
-    def __init__(self,
-                 oauth_token: str,
-                 github_url: str,
-                 proxy: Optional[str] = None,
-                 verify: Optional[str] = None,
-                 cert: Optional[Union[str, Tuple[str, str]]] = None):
+    def __init__(
+        self,
+        oauth_token: str,
+        github_url: str,
+        proxy: Optional[str] = None,
+        verify: Optional[str] = None,
+        cert: Optional[Union[str, Tuple[str, str]]] = None,
+    ):
         self.oauth_token = oauth_token
         self.proxy = proxy
         self.github_url = github_url
         self.verify = verify
         self.cert = cert
 
     def push_hook(self, refName: Sequence[str]) -> None:
         pass
 
     def graphql(self, query: str, **kwargs: Any) -> Any:
         headers = {}
         if self.oauth_token:
-            headers['Authorization'] = 'bearer {}'.format(self.oauth_token)
+            headers["Authorization"] = "bearer {}".format(self.oauth_token)
 
         if self.proxy:
-            proxies = {
-                'http': self.proxy,
-                'https': self.proxy
-            }
+            proxies = {"http": self.proxy, "https": self.proxy}
         else:
             proxies = {}
 
-        logging.debug("# POST {}".format(self.graphql_endpoint.format(github_url=self.github_url)))
+        logging.debug(
+            "# POST {}".format(self.graphql_endpoint.format(github_url=self.github_url))
+        )
         logging.debug("Request GraphQL query:\n{}".format(query))
-        logging.debug("Request GraphQL variables:\n{}"
-                      .format(json.dumps(kwargs, indent=1)))
+        logging.debug(
+            "Request GraphQL variables:\n{}".format(json.dumps(kwargs, indent=1))
+        )
 
         resp = requests.post(
             self.graphql_endpoint.format(github_url=self.github_url),
             json={"query": query, "variables": kwargs},
             headers=headers,
             proxies=proxies,
             verify=self.verify,
@@ -94,36 +96,33 @@
         # they seem to always return 200, even in error case (as of
         # 11/5/2018)
         try:
             resp.raise_for_status()
         except requests.HTTPError:
             raise RuntimeError(pretty_json)
 
-        if 'errors' in r:
+        if "errors" in r:
             raise RuntimeError(pretty_json)
 
         return r
 
     def rest(self, method: str, path: str, **kwargs: Any) -> Any:
         if self.proxy:
-            proxies = {
-                'http': self.proxy,
-                'https': self.proxy
-            }
+            proxies = {"http": self.proxy, "https": self.proxy}
         else:
             proxies = {}
 
         headers = {
-            'Authorization': 'token ' + self.oauth_token,
-            'Content-Type': 'application/json',
-            'User-Agent': 'ghstack',
-            'Accept': 'application/vnd.github.v3+json',
+            "Authorization": "token " + self.oauth_token,
+            "Content-Type": "application/json",
+            "User-Agent": "ghstack",
+            "Accept": "application/vnd.github.v3+json",
         }
 
-        url = self.rest_endpoint.format(github_url=self.github_url) + '/' + path
+        url = self.rest_endpoint.format(github_url=self.github_url) + "/" + path
         logging.debug("# {} {}".format(method, url))
         logging.debug("Request body:\n{}".format(json.dumps(kwargs, indent=1)))
 
         resp: requests.Response = getattr(requests, method)(
             url,
             json=kwargs,
             headers=headers,
@@ -140,24 +139,28 @@
             logging.debug("Response body:\n{}".format(r.text))
             raise
         else:
             pretty_json = json.dumps(r, indent=1)
             logging.debug("Response JSON:\n{}".format(pretty_json))
 
         if resp.status_code == 404:
-            raise ghstack.github.NotFoundError("""\
+            raise ghstack.github.NotFoundError(
+                """\
 GitHub raised a 404 error on the request for
 {url}.
 Usually, this doesn't actually mean the page doesn't exist; instead, it
 usually means that you didn't configure your OAuth token with enough
 permissions.  Please create a new OAuth token at
 https://{github_url}/settings/tokens and DOUBLE CHECK that you checked
 "public_repo" for permissions, and update ~/.ghstackrc with your new
 value.
-""".format(url=url, github_url=self.github_url))
+""".format(
+                    url=url, github_url=self.github_url
+                )
+            )
 
         try:
             resp.raise_for_status()
         except requests.HTTPError:
             raise RuntimeError(pretty_json)
 
         return r
```

### Comparing `ghstack-0.7.1/ghstack/github_schema.graphql` & `ghstack-0.8.0/ghstack/github_schema.graphql`

 * *Files identical despite different names*

### Comparing `ghstack-0.7.1/ghstack/github_utils.py` & `ghstack-0.8.0/ghstack/github_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,57 +5,61 @@
 
 from typing_extensions import TypedDict
 
 import ghstack.github
 import ghstack.shell
 from ghstack.types import GitHubRepositoryId
 
-GitHubRepoNameWithOwner = TypedDict('GitHubRepoNameWithOwner', {
-    'owner': str,
-    'name': str,
-})
+GitHubRepoNameWithOwner = TypedDict(
+    "GitHubRepoNameWithOwner",
+    {
+        "owner": str,
+        "name": str,
+    },
+)
 
 
 def get_github_repo_name_with_owner(
     *,
     sh: ghstack.shell.Shell,
     github_url: str,
     remote_name: str,
 ) -> GitHubRepoNameWithOwner:
     # Grovel in remotes to figure it out
     remote_url = sh.git("remote", "get-url", remote_name)
     while True:
-        match = r'^git@{github_url}:([^/]+)/(.+?)(?:\.git)?$'.format(
+        match = r"^git@{github_url}:([^/]+)/(.+?)(?:\.git)?$".format(
             github_url=github_url
         )
         m = re.match(match, remote_url)
         if m:
             owner = m.group(1)
             name = m.group(2)
             break
-        search = r'{github_url}/([^/]+)/(.+?)(?:\.git)?$'.format(
-            github_url=github_url
-        )
+        search = r"{github_url}/([^/]+)/(.+?)(?:\.git)?$".format(github_url=github_url)
         m = re.search(search, remote_url)
         if m:
             owner = m.group(1)
             name = m.group(2)
             break
         raise RuntimeError(
-            "Couldn't determine repo owner and name from url: {}"
-            .format(remote_url))
-    return {'owner': owner, 'name': name}
+            "Couldn't determine repo owner and name from url: {}".format(remote_url)
+        )
+    return {"owner": owner, "name": name}
 
 
-GitHubRepoInfo = TypedDict('GitHubRepoInfo', {
-    'name_with_owner': GitHubRepoNameWithOwner,
-    'id': GitHubRepositoryId,
-    'is_fork': bool,
-    'default_branch': str,
-})
+GitHubRepoInfo = TypedDict(
+    "GitHubRepoInfo",
+    {
+        "name_with_owner": GitHubRepoNameWithOwner,
+        "id": GitHubRepositoryId,
+        "is_fork": bool,
+        "default_branch": str,
+    },
+)
 
 
 def get_github_repo_info(
     *,
     github: ghstack.github.GitHubEndpoint,
     sh: ghstack.shell.Shell,
     repo_owner: Optional[str] = None,
@@ -81,38 +85,43 @@
                 isFork
                 defaultBranchRef {
                     name
                 }
             }
         }""",
         owner=name_with_owner["owner"],
-        name=name_with_owner["name"])["data"]["repository"]
+        name=name_with_owner["name"],
+    )["data"]["repository"]
 
     return {
         "name_with_owner": name_with_owner,
         "id": repo["id"],
         "is_fork": repo["isFork"],
         "default_branch": repo["defaultBranchRef"]["name"],
     }
 
 
 RE_PR_URL = re.compile(
-    r'^https://(?P<github_url>[^/]+)/(?P<owner>[^/]+)/(?P<name>[^/]+)/pull/(?P<number>[0-9]+)/?$')
+    r"^https://(?P<github_url>[^/]+)/(?P<owner>[^/]+)/(?P<name>[^/]+)/pull/(?P<number>[0-9]+)/?$"
+)
 
-GitHubPullRequestParams = TypedDict('GitHubPullRequestParams', {
-    'github_url': str,
-    'owner': str,
-    'name': str,
-    'number': int,
-})
+GitHubPullRequestParams = TypedDict(
+    "GitHubPullRequestParams",
+    {
+        "github_url": str,
+        "owner": str,
+        "name": str,
+        "number": int,
+    },
+)
 
 
 def parse_pull_request(pull_request: str) -> GitHubPullRequestParams:
     m = RE_PR_URL.match(pull_request)
     if not m:
         raise RuntimeError("Did not understand PR argument.  PR must be URL")
 
     github_url = m.group("github_url")
     owner = m.group("owner")
     name = m.group("name")
     number = int(m.group("number"))
-    return {'github_url': github_url, 'owner': owner, 'name': name, 'number': number}
+    return {"github_url": github_url, "owner": owner, "name": name, "number": number}
```

### Comparing `ghstack-0.7.1/ghstack/gpg_sign.py` & `ghstack-0.8.0/ghstack/gpg_sign.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,21 +15,26 @@
 
 import ghstack.shell
 
 _should_sign = None
 
 
 def gpg_args_if_necessary(
-    shell: ghstack.shell.Shell = ghstack.shell.Shell()
+    shell: ghstack.shell.Shell = ghstack.shell.Shell(),
 ) -> Union[Tuple[str], Tuple[()]]:
     global _should_sign
     # cache the config result
     if _should_sign is None:
         # If the config is not set, we get exit 1
         try:
             # Why the complicated compare
             # https://git-scm.com/docs/git-config#Documentation/git-config.txt-boolean
-            _should_sign = shell.git("config", "--get", "commit.gpgsign") in ("yes", "on", "true", "1")
+            _should_sign = shell.git("config", "--get", "commit.gpgsign") in (
+                "yes",
+                "on",
+                "true",
+                "1",
+            )
         except:
             _should_sign = False
 
     return ("-S",) if _should_sign else ()
```

### Comparing `ghstack-0.7.1/ghstack/land.py` & `ghstack-0.8.0/ghstack/land.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,50 @@
 from ghstack.diff import PullRequestResolved
 from ghstack.types import GitCommitHash
 
 
 def lookup_pr_to_orig_ref_and_closed(
     github: ghstack.github.GitHubEndpoint, *, owner: str, name: str, number: int
 ) -> Tuple[str, bool]:
-    pr_result = github.graphql("""
+    pr_result = github.graphql(
+        """
         query ($owner: String!, $name: String!, $number: Int!) {
             repository(name: $name, owner: $owner) {
                 pullRequest(number: $number) {
                     headRefName
                     closed
                 }
             }
         }
-    """, owner=owner, name=name, number=number)
+    """,
+        owner=owner,
+        name=name,
+        number=number,
+    )
     pr = pr_result["data"]["repository"]["pullRequest"]
     head_ref = pr["headRefName"]
     closed = pr["closed"]
     assert isinstance(head_ref, str)
-    orig_ref = re.sub(r'/head$', '/orig', head_ref)
+    orig_ref = re.sub(r"/head$", "/orig", head_ref)
     if orig_ref == head_ref:
-        raise RuntimeError("The ref {} doesn't look like a ghstack reference".format(head_ref))
+        raise RuntimeError(
+            "The ref {} doesn't look like a ghstack reference".format(head_ref)
+        )
     return orig_ref, closed
 
 
-def main(pull_request: str,
-         remote_name: str,
-         github: ghstack.github.GitHubEndpoint,
-         sh: ghstack.shell.Shell,
-         github_url: str) -> None:
+def main(
+    pull_request: str,
+    remote_name: str,
+    github: ghstack.github.GitHubEndpoint,
+    sh: ghstack.shell.Shell,
+    github_url: str,
+    *,
+    force: bool = False,
+) -> None:
 
     # We land the entire stack pointed to by a URL.
     # Local state is ignored; PR is source of truth
     # Furthermore, the parent commits of PR are ignored: we always
     # take the canonical version of the patch from any given pr
 
     params = ghstack.github_utils.parse_pull_request(pull_request)
@@ -53,23 +64,27 @@
         repo_name=params["name"],
         github_url=github_url,
         remote_name=remote_name,
     )["default_branch"]
 
     needs_force = False
     try:
-        protection = github.get(f"repos/{params['owner']}/{params['name']}/branches/{default_branch}/protection")
+        protection = github.get(
+            f"repos/{params['owner']}/{params['name']}/branches/{default_branch}/protection"
+        )
         if not protection["allow_force_pushes"]["enabled"]:
-            raise RuntimeError("""\
+            raise RuntimeError(
+                """\
 Default branch {default_branch} is protected, and doesn't allow force pushes.
 ghstack land does not work.  You will not be able to land your ghstack; please
 resubmit your PRs using the normal pull request flow.
 
 See https://github.com/ezyang/ghstack/issues/50 for more details, or
-to complain to the ghstack authors.""")
+to complain to the ghstack authors."""
+            )
         else:
             needs_force = True
     except ghstack.github.NotFoundError:
         pass
 
     orig_ref, _ = lookup_pr_to_orig_ref_and_closed(
         github,
@@ -81,15 +96,17 @@
     if sh is None:
         # Use CWD
         sh = ghstack.shell.Shell()
 
     # Get up-to-date
     sh.git("fetch", "--prune", remote_name)
     remote_orig_ref = remote_name + "/" + orig_ref
-    base = GitCommitHash(sh.git("merge-base", f"{remote_name}/{default_branch}", remote_orig_ref))
+    base = GitCommitHash(
+        sh.git("merge-base", f"{remote_name}/{default_branch}", remote_orig_ref)
+    )
 
     # compute the stack of commits in chronological order (does not
     # include base)
     stack = ghstack.git.parse_header(
         sh.git("rev-list", "--reverse", "--header", "^" + base, remote_orig_ref),
         github_url=github_url,
     )
@@ -111,16 +128,17 @@
             # We got this from GitHub, this better not be corrupted
             assert pr_resolved is not None
 
             ref, closed = lookup_pr_to_orig_ref_and_closed(
                 github,
                 owner=pr_resolved.owner,
                 name=pr_resolved.repo,
-                number=pr_resolved.number)
-            if closed:
+                number=pr_resolved.number,
+            )
+            if closed and not force:
                 continue
             stack_orig_refs.append((ref, pr_resolved))
 
         # OK, actually do the land now
         for orig_ref, _ in stack_orig_refs:
             try:
                 sh.git("cherry-pick", f"{remote_name}/{orig_ref}")
@@ -138,27 +156,29 @@
         # directly *merge* head into base, so that the PR accurately
         # reflects what we ACTUALLY merged to master, as opposed to
         # this synthetic thing I'm doing right now just to make it look
         # like the PR got closed
 
         for orig_ref, pr_resolved in stack_orig_refs:
             # TODO: regex here so janky
-            base_ref = re.sub(r'/orig$', '/base', orig_ref)
-            head_ref = re.sub(r'/orig$', '/head', orig_ref)
+            base_ref = re.sub(r"/orig$", "/base", orig_ref)
+            head_ref = re.sub(r"/orig$", "/head", orig_ref)
             sh.git("push", remote_name, f"{remote_name}/{head_ref}:{base_ref}")
             github.notify_merged(pr_resolved)
 
         # All good! Push!
         maybe_force_arg = []
         if needs_force:
             maybe_force_arg = ["--force-with-lease"]
-        sh.git("push", *maybe_force_arg, remote_name, f"HEAD:refs/heads/{default_branch}")
+        sh.git(
+            "push", *maybe_force_arg, remote_name, f"HEAD:refs/heads/{default_branch}"
+        )
 
         # Delete the branches
         for orig_ref, _ in stack_orig_refs:
             # TODO: regex here so janky
-            base_ref = re.sub(r'/orig$', '/base', orig_ref)
-            head_ref = re.sub(r'/orig$', '/head', orig_ref)
+            base_ref = re.sub(r"/orig$", "/base", orig_ref)
+            head_ref = re.sub(r"/orig$", "/head", orig_ref)
             sh.git("push", remote_name, "--delete", orig_ref, base_ref, head_ref)
 
     finally:
         sh.git("checkout", prev_ref)
```

### Comparing `ghstack-0.7.1/ghstack/logs.py` & `ghstack-0.8.0/ghstack/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 import re
 import shutil
 import subprocess
 import sys
 import uuid
 from typing import Dict, Iterator, Optional
 
-DATETIME_FORMAT = '%Y-%m-%d_%Hh%Mm%Ss'
+DATETIME_FORMAT = "%Y-%m-%d_%Hh%Mm%Ss"
 
 
 RE_LOG_DIRNAME = re.compile(
-    r'(\d{4}-\d\d-\d\d_\d\dh\d\dm\d\ds)_'
-    r'[0-9a-f]{8}-(?:[0-9a-f]{4}-){3}[0-9a-f]{12}')
+    r"(\d{4}-\d\d-\d\d_\d\dh\d\dm\d\ds)_" r"[0-9a-f]{8}-(?:[0-9a-f]{4}-){3}[0-9a-f]{12}"
+)
 
 
 class Formatter(logging.Formatter):
     redactions: Dict[str, str]
 
-    def __init__(self, fmt: Optional[str] = None,
-                 datefmt: Optional[str] = None):
+    def __init__(self, fmt: Optional[str] = None, datefmt: Optional[str] = None):
         super().__init__(fmt, datefmt)
         self.redactions = {}
 
     # Remove sensitive information from URLs
     def _filter(self, s: str) -> str:
-        s = re.sub(r':\/\/(.*?)\@', r'://<USERNAME>:<PASSWORD>@', s)
+        s = re.sub(r":\/\/(.*?)\@", r"://<USERNAME>:<PASSWORD>@", s)
         for needle, replace in self.redactions.items():
             s = s.replace(needle, replace)
         return s
 
     def formatMessage(self, record: logging.LogRecord) -> str:
         if record.levelno == logging.INFO or record.levelno == logging.DEBUG:
             # Log INFO/DEBUG without any adornment
@@ -46,24 +45,23 @@
 
     def format(self, record: logging.LogRecord) -> str:
         return self._filter(super().format(record))
 
     # Redact specific strings; e.g., authorization tokens.  This won't
     # retroactively redact stuff you've already leaked, so make sure
     # you redact things as soon as possible
-    def redact(self, needle: str, replace: str = '<REDACTED>') -> None:
+    def redact(self, needle: str, replace: str = "<REDACTED>") -> None:
         # Don't redact empty strings; this will lead to something
         # that looks like s<REDACTED>t<REDACTED>r<REDACTED>...
-        if needle == '':
+        if needle == "":
             return
         self.redactions[needle] = replace
 
 
-formatter = Formatter(
-    fmt="%(levelname)s: %(message)s", datefmt="")
+formatter = Formatter(fmt="%(levelname)s: %(message)s", datefmt="")
 
 
 @contextlib.contextmanager
 def manager(*, debug: bool = False) -> Iterator[None]:
     # TCB code to setup logging.  If a failure starts here we won't
     # be able to save the user in a reasonable way.
 
@@ -107,40 +105,33 @@
         yield
 
     except Exception as e:
         logging.exception("Fatal exception")
         record_exception(e)
         sys.exit(1)
 
-    except BaseException as e:
-        # You could logging.debug here to suppress the backtrace
-        # entirely, but there is no reason to hide it from technically
-        # savvy users.
-        logging.info("", exc_info=True)
-        record_exception(e)
-        sys.exit(1)
-
 
 @functools.lru_cache()
 def base_dir() -> str:
     # Don't use shell here as we are not allowed to log yet!
     try:
         meta_dir = subprocess.run(
             ("git", "rev-parse", "--git-dir"),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             check=True,
-            encoding='utf-8'
+            encoding="utf-8",
         ).stdout.rstrip()
     except subprocess.CalledProcessError:
-        meta_dir = os.path.join(subprocess.run(
-            ("hg", "root"), stdout=subprocess.PIPE,
-            encoding='utf-8',
-            check=True
-        ).stdout.rstrip(), '.hg')
+        meta_dir = os.path.join(
+            subprocess.run(
+                ("hg", "root"), stdout=subprocess.PIPE, encoding="utf-8", check=True
+            ).stdout.rstrip(),
+            ".hg",
+        )
 
     base_dir = os.path.join(meta_dir, "ghstack", "log")
 
     try:
         os.makedirs(base_dir)
     except FileExistsError:
         pass
@@ -150,39 +141,38 @@
 
 # Naughty, "run it once and save" memoizing
 @functools.lru_cache()
 def run_dir() -> str:
     # NB: respects timezone
     cur_dir = os.path.join(
         base_dir(),
-        "{}_{}"
-        .format(datetime.datetime.now().strftime(DATETIME_FORMAT),
-                uuid.uuid1()))
+        "{}_{}".format(datetime.datetime.now().strftime(DATETIME_FORMAT), uuid.uuid1()),
+    )
 
     try:
         os.makedirs(cur_dir)
     except FileExistsError:
         pass
 
     return cur_dir
 
 
 def record_exception(e: BaseException) -> None:
-    with open(os.path.join(run_dir(), "exception"), 'w') as f:
+    with open(os.path.join(run_dir(), "exception"), "w") as f:
         f.write(type(e).__name__)
 
 
 @functools.lru_cache()
 def record_argv() -> None:
-    with open(os.path.join(run_dir(), "argv"), 'w') as f:
+    with open(os.path.join(run_dir(), "argv"), "w") as f:
         f.write(subprocess.list2cmdline(sys.argv))
 
 
 def record_status(status: str) -> None:
-    with open(os.path.join(run_dir(), "status"), 'w') as f:
+    with open(os.path.join(run_dir(), "status"), "w") as f:
         f.write(status)
 
 
 def rotate() -> None:
     log_base = base_dir()
     old_logs = os.listdir(log_base)
     old_logs.sort(reverse=True)
```

### Comparing `ghstack-0.7.1/ghstack/rage.py` & `ghstack-0.8.0/ghstack/rage.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import os
 import tempfile
 from typing import Dict, NewType
 
 import ghstack
 import ghstack.logs
 
-RawIndex = NewType('RawIndex', int)
-FilteredIndex = NewType('FilteredIndex', int)
+RawIndex = NewType("RawIndex", int)
+FilteredIndex = NewType("FilteredIndex", int)
 
 
 def get_argv(log_dir: str) -> str:
     argv = "Unknown"
-    argv_fn = os.path.join(log_dir, 'argv')
+    argv_fn = os.path.join(log_dir, "argv")
     if os.path.exists(argv_fn):
-        with open(argv_fn, 'r') as f:
+        with open(argv_fn, "r") as f:
             argv = f.read().rstrip()
     return argv
 
 
 def get_status(log_dir: str) -> str:
     status = ""
-    status_fn = os.path.join(log_dir, 'status')
+    status_fn = os.path.join(log_dir, "status")
     if os.path.exists(status_fn):
-        with open(status_fn, 'r') as f:
+        with open(status_fn, "r") as f:
             status = f.read().rstrip()
     return status
 
 
 def main(latest: bool = False) -> None:
 
     log_base = ghstack.logs.base_dir()
@@ -58,52 +58,59 @@
 
             if len(argv_list) >= 2 and argv_list[1] == "rage":
                 continue
 
             if len(argv_list) >= 1:
                 argv_list[0] = os.path.basename(argv_list[0])
 
-            argv = ' '.join(argv_list)
+            argv = " ".join(argv_list)
 
             status = get_status(log_dir)
             if status:
                 at_status = " at {}".format(status)
             else:
                 at_status = ""
 
             cur_index = next_index
             next_index = FilteredIndex(next_index + 1)
 
             filtered_mapping[cur_index] = raw_index
 
             m = ghstack.logs.RE_LOG_DIRNAME.fullmatch(fn)
             if m:
-                date = datetime.datetime.strptime(
-                    m.group(1), ghstack.logs.DATETIME_FORMAT
-                ).astimezone(tz=None).strftime("%a %b %d %H:%M:%S %Z")
+                date = (
+                    datetime.datetime.strptime(m.group(1), ghstack.logs.DATETIME_FORMAT)
+                    .astimezone(tz=None)
+                    .strftime("%a %b %d %H:%M:%S %Z")
+                )
             else:
                 date = "Unknown"
             exception = "Succeeded"
-            exception_fn = os.path.join(log_base, fn, 'exception')
+            exception_fn = os.path.join(log_base, fn, "exception")
             if os.path.exists(exception_fn):
-                with open(exception_fn, 'r') as f:
+                with open(exception_fn, "r") as f:
                     exception = "Failed with: " + f.read().rstrip()
 
-            print("{:<5}  {}  [{}]  {}{}"
-                  .format("[{}].".format(cur_index), date, argv, exception, at_status))
+            print(
+                "{:<5}  {}  [{}]  {}{}".format(
+                    "[{}].".format(cur_index), date, argv, exception, at_status
+                )
+            )
         print()
         selected_index = FilteredIndex(
-            int(input('(input individual number, for example 1 or 2)\n')))
+            int(input("(input individual number, for example 1 or 2)\n"))
+        )
 
     log_dir = os.path.join(log_base, logs[filtered_mapping[selected_index]])
 
     print()
     print("Writing report, please wait...")
-    with tempfile.NamedTemporaryFile(mode='w', suffix=".log",
-                                     prefix="ghstack", delete=False) as g:
+    with tempfile.NamedTemporaryFile(
+        mode="w", suffix=".log", prefix="ghstack", delete=False
+    ) as g:
         g.write("version: {}\n".format(ghstack.__version__))
         g.write("command: {}\n".format(get_argv(log_dir)))
         g.write("status: {}\n".format(get_status(log_dir)))
         g.write("\n")
         log_fn = os.path.join(log_dir, "ghstack.log")
         if os.path.exists(log_fn):
             with open(log_fn) as log:
```

### Comparing `ghstack-0.7.1/ghstack/shell.py` & `ghstack-0.8.0/ghstack/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import asyncio
 import logging
 import os
 import shlex
 import subprocess
 import sys
-from typing import (IO, Any, Dict, Optional, Sequence, Tuple, TypeVar, Union,
-                    overload)
+from typing import Any, Dict, IO, Optional, overload, Sequence, Tuple, TypeVar, Union
 
 # Shell commands generally return str, but with exitcode=True
 # they return a bool, and if stdout is piped straight to sys.stdout
 # they return None.
 _SHELL_RET = Union[bool, str, None]
 
 
@@ -22,22 +21,22 @@
     """
     Given a command, print it in a both machine and human readable way.
 
     Args:
         *args: the list of command line arguments you want to run
         env: the dictionary of environment variable settings for the command
     """
-    cmd = ' '.join(shlex.quote(arg) for arg in args)
+    cmd = " ".join(shlex.quote(arg) for arg in args)
     logging.info("$ " + cmd)
 
 
-K = TypeVar('K')
+K = TypeVar("K")
 
 
-V = TypeVar('V')
+V = TypeVar("V")
 
 
 def merge_dicts(x: Dict[K, V], y: Dict[K, V]) -> Dict[K, V]:
     z = x.copy()
     z.update(y)
     return z
 
@@ -58,18 +57,17 @@
     # Whether or not shell is in testing mode; some commands are made
     # more deterministic in this case.
     testing: bool
 
     # The current Unix timestamp.  Only used during testing mode.
     testing_time: int
 
-    def __init__(self,
-                 quiet: bool = False,
-                 cwd: Optional[str] = None,
-                 testing: bool = False):
+    def __init__(
+        self, quiet: bool = False, cwd: Optional[str] = None, testing: bool = False
+    ):
         """
         Args:
             cwd: Current working directory of the shell.  Pass None to
                 initialize to the current cwd of the current process.
             quiet: If True, suppress printing out the command executed
                 by the shell.  By default, we print out commands for ease
                 of debugging.  Quiet is most useful for non-mutating
@@ -80,22 +78,25 @@
                 variables for Git.
         """
         self.cwd = cwd if cwd else os.getcwd()
         self.quiet = quiet
         self.testing = testing
         self.testing_time = 1112911993
 
-    def sh(self, *args: str,  # noqa: C901
-           env: Optional[Dict[str, str]] = None,
-           stderr: _HANDLE = None,
-           # TODO: Arguably bytes should be accepted here too
-           input: Optional[str] = None,
-           stdin: _HANDLE = None,
-           stdout: _HANDLE = subprocess.PIPE,
-           exitcode: bool = False) -> _SHELL_RET:
+    def sh(
+        self,
+        *args: str,  # noqa: C901
+        env: Optional[Dict[str, str]] = None,
+        stderr: _HANDLE = None,
+        # TODO: Arguably bytes should be accepted here too
+        input: Optional[str] = None,
+        stdin: _HANDLE = None,
+        stdout: _HANDLE = subprocess.PIPE,
+        exitcode: bool = False
+    ) -> _SHELL_RET:
         """
         Run a command specified by args, and return string representing
         the stdout of the run command, raising an error if exit code
         was nonzero (unless exitcode kwarg is specified; see below).
 
         Args:
             *args: the list of command line arguments to run
@@ -130,16 +131,17 @@
         #   it's better for logging (since we get to dispense
         #   with the control codes).
         #
         # - We assume line buffering.  This is kind of silly but
         #   we need to assume *some* sort of buffering with the
         #   stream API.
 
-        async def process_stream(proc_stream: asyncio.StreamReader, setting: _HANDLE,
-                                 default_stream: IO[str]) -> bytes:
+        async def process_stream(
+            proc_stream: asyncio.StreamReader, setting: _HANDLE, default_stream: IO[str]
+        ) -> bytes:
             output = []
             while True:
                 try:
                     line = await proc_stream.readuntil()
                 except asyncio.LimitOverrunError as e:
                     line = await proc_stream.readexactly(e.consumed)
                 except asyncio.IncompleteReadError as e:
@@ -151,28 +153,28 @@
                     pass
                 elif setting == subprocess.STDOUT:
                     sys.stdout.buffer.write(line)
                 elif isinstance(setting, int):
                     os.write(setting, line)
                 elif setting is None:
                     # Sigh.  See https://stackoverflow.com/questions/55681488/python-3-write-binary-to-stdout-respecting-buffering
-                    default_stream.write(line.decode('utf-8'))
+                    default_stream.write(line.decode("utf-8"))
                 else:
                     # NB: don't use setting.write directly, that will
                     # not properly handle binary.  This gives us
                     # "parity" with the normal subprocess implementation
                     os.write(setting.fileno(), line)
-            return b''.join(output)
+            return b"".join(output)
 
         async def feed_input(stdin_writer: Optional[asyncio.StreamWriter]) -> None:
             if stdin_writer is None:
                 return
             if not input:
                 return
-            stdin_writer.write(input.encode('utf-8'))
+            stdin_writer.write(input.encode("utf-8"))
             await stdin_writer.drain()
             stdin_writer.close()
 
         async def run() -> Tuple[int, bytes, bytes]:
             proc = await asyncio.create_subprocess_exec(
                 *args,
                 stdin=stdin,
@@ -183,37 +185,37 @@
             )
             assert proc.stdout is not None
             assert proc.stderr is not None
             _, out, err, _ = await asyncio.gather(
                 feed_input(proc.stdin),
                 process_stream(proc.stdout, stdout, sys.stdout),
                 process_stream(proc.stderr, stderr, sys.stderr),
-                proc.wait()
+                proc.wait(),
             )
             assert proc.returncode is not None
             return (proc.returncode, out, err)
 
         loop = asyncio.get_event_loop()
         returncode, out, err = loop.run_until_complete(run())
 
         # NB: Not debug; we always want to show this to user.
         if err:
             logging.debug("# stderr:\n" + err.decode(errors="backslashreplace"))
         if out:
             logging.debug(
                 ("# stdout:\n" if err else "")
-                + out.decode(errors="backslashreplace").replace('\0', '\\0'))
+                + out.decode(errors="backslashreplace").replace("\0", "\\0")
+            )
 
         if exitcode:
             logging.debug("Exit code: {}".format(returncode))
             return returncode == 0
         if returncode != 0:
             raise RuntimeError(
-                "{} failed with exit code {}"
-                .format(' '.join(args), returncode)
+                "{} failed with exit code {}".format(" ".join(args), returncode)
             )
 
         if stdout == subprocess.PIPE:
             return out.decode()  # do a strict decode for actual return
         else:
             return None
 
@@ -238,16 +240,15 @@
         ...
 
     @overload  # noqa: F811
     def git(self, *args: str, **kwargs: Any) -> _SHELL_RET:
 
         ...
 
-    def git(self, *args: str, **kwargs: Any  # noqa: F811
-            ) -> _SHELL_RET:
+    def git(self, *args: str, **kwargs: Any) -> _SHELL_RET:  # noqa: F811
         """
         Run a git command.  The returned stdout has trailing newlines stripped.
 
         Args:
             *args: Arguments to git
             **kwargs: Any valid kwargs for sh()
         """
@@ -264,20 +265,18 @@
             env.setdefault("TZ", "UTC")
             env.setdefault("TERM", "dumb")
             # These are important so we get deterministic commit times
             env.setdefault("GIT_AUTHOR_EMAIL", "author@example.com")
             env.setdefault("GIT_AUTHOR_NAME", "A U Thor")
             env.setdefault("GIT_COMMITTER_EMAIL", "committer@example.com")
             env.setdefault("GIT_COMMITTER_NAME", "C O Mitter")
-            env.setdefault("GIT_COMMITTER_DATE",
-                           "{} -0700".format(self.testing_time))
-            env.setdefault("GIT_AUTHOR_DATE",
-                           "{} -0700".format(self.testing_time))
-            if 'stderr' not in kwargs:
-                kwargs['stderr'] = subprocess.PIPE
+            env.setdefault("GIT_COMMITTER_DATE", "{} -0700".format(self.testing_time))
+            env.setdefault("GIT_AUTHOR_DATE", "{} -0700".format(self.testing_time))
+            if "stderr" not in kwargs:
+                kwargs["stderr"] = subprocess.PIPE
 
         return self._maybe_rstrip(self.sh(*(("git",) + args), **kwargs))
 
     @overload  # noqa: F811
     def hg(self, *args: str) -> str:
         ...
 
@@ -285,16 +284,15 @@
     def hg(self, *args: str, input: str) -> str:
         ...
 
     @overload  # noqa: F811
     def hg(self, *args: str, **kwargs: Any) -> _SHELL_RET:
         ...
 
-    def hg(self, *args: str, **kwargs: Any  # noqa: F811
-           ) -> _SHELL_RET:
+    def hg(self, *args: str, **kwargs: Any) -> _SHELL_RET:  # noqa: F811
         """
         Run a hg command.  The returned stdout has trailing newlines stripped.
 
         Args:
             *args: Arguments to hg
             **kwargs: Any valid kwargs for sh()
         """
@@ -306,15 +304,15 @@
         Run a jf command.  The returned stdout has trailing newlines stripped.
 
         Args:
             *args: Arguments to jf
             **kwargs: Any valid kwargs for sh()
         """
 
-        kwargs.setdefault('stdout', sys.stderr)
+        kwargs.setdefault("stdout", sys.stderr)
 
         return self._maybe_rstrip(self.sh(*(("jf",) + args), **kwargs))
 
     def test_tick(self) -> None:
         """
         Increase the current time.  Useful when testing is True.
         """
```

### Comparing `ghstack-0.7.1/ghstack/submit.py` & `ghstack-0.8.0/ghstack/submit.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,78 +9,85 @@
 import ghstack
 import ghstack.git
 import ghstack.github
 import ghstack.github_utils
 import ghstack.gpg_sign
 import ghstack.logs
 import ghstack.shell
-from ghstack.types import (GhNumber, GitCommitHash, GitHubNumber,
-                           GitHubRepositoryId, GitTreeHash)
+from ghstack.types import (
+    GhNumber,
+    GitCommitHash,
+    GitHubNumber,
+    GitHubRepositoryId,
+    GitTreeHash,
+)
 
 # Either "base", "head" or "orig"; which of the ghstack generated
 # branches this diff corresponds to
 BranchKind = str
 
 # Metadata describing a diff we submitted to GitHub
 # TODO: Make this directly contain a DiffWithGitHubMetadata?
-DiffMeta = NamedTuple('DiffMeta', [
-    ('title', str),
-    ('number', GitHubNumber),
-    ('body', str),
-    ('username', str),
-    ('ghnum', GhNumber),
-    # What Git commit hash we should push to what branch
-    ('push_branches', Tuple[Tuple[GitCommitHash, BranchKind], ...]),
-    # What Git commit hash corresponds to head for this
-    # (previously, we got this out of push_branches, but this is not
-    # guaranteed to be set.)  None if we didn't change it.
-    ('head_branch', Optional[GitCommitHash]),
-    # A human-readable string like 'Created' which describes what
-    # happened to this pull request
-    ('what', str),
-    ('closed', bool),
-    ('pr_url', str),
-])
+DiffMeta = NamedTuple(
+    "DiffMeta",
+    [
+        ("title", str),
+        ("number", GitHubNumber),
+        ("body", str),
+        ("username", str),
+        ("ghnum", GhNumber),
+        # What Git commit hash we should push to what branch
+        ("push_branches", Tuple[Tuple[GitCommitHash, BranchKind], ...]),
+        # What Git commit hash corresponds to head for this
+        # (previously, we got this out of push_branches, but this is not
+        # guaranteed to be set.)  None if we didn't change it.
+        ("head_branch", Optional[GitCommitHash]),
+        # A human-readable string like 'Created' which describes what
+        # happened to this pull request
+        ("what", str),
+        ("closed", bool),
+        ("pr_url", str),
+    ],
+)
 
 
 # Ya, sometimes we get carriage returns.  Crazy right?
-RE_STACK = re.compile(r'Stack.*:\r?\n(\* [^\r\n]+\r?\n)+')
+RE_STACK = re.compile(r"Stack.*:\r?\n(\* [^\r\n]+\r?\n)+")
 
 
 # NB: This regex is fuzzy because the D1234567 identifier is typically
 # linkified.
-RE_DIFF_REV = re.compile(r'^Differential Revision:.+?(D[0-9]+)', re.MULTILINE)
+RE_DIFF_REV = re.compile(r"^Differential Revision:.+?(D[0-9]+)", re.MULTILINE)
 
 
 # Suppose that you have submitted a commit to GitHub, and that commit's
 # tree was AAA.  The ghstack-source-id of your local commit after this
 # submit is AAA.  When you submit a new change on top of this, we check
 # that the source id associated with your orig commit agrees with what's
 # recorded in GitHub: this lets us know that you are "up-to-date" with
 # what was stored on GitHub.  Then, we update the commit message on your
 # local commit to record a new ghstack-source-id and push it to orig.
 #
 # We must store this in the orig commit as we have no other mechanism of
 # attaching information to a commit in question.  We don't store this in
 # the pull request body as there isn't really any need to do so.
-RE_GHSTACK_SOURCE_ID = re.compile(r'^ghstack-source-id: (.+)\n?', re.MULTILINE)
+RE_GHSTACK_SOURCE_ID = re.compile(r"^ghstack-source-id: (.+)\n?", re.MULTILINE)
 
 
 # repo layout:
 #   - gh/username/23/head -- what we think GitHub's current tip for commit is
 #   - gh/username/23/base -- what we think base commit for commit is
 #   - gh/username/23/orig -- the "clean" commit history, i.e., what we're
 #                      rebasing, what you'd like to cherry-pick (???)
 #                      (Maybe this isn't necessary, because you can
 #                      get the "whole" diff from GitHub?  What about
 #                      commit description?)
 
 
-def branch(username: str, ghnum: GhNumber, kind: BranchKind
-           ) -> GitCommitHash:
+def branch(username: str, ghnum: GhNumber, kind: BranchKind) -> GitCommitHash:
     return GitCommitHash("gh/{}/{}/{}".format(username, ghnum, kind))
 
 
 def branch_base(username: str, ghnum: GhNumber) -> GitCommitHash:
     return branch(username, ghnum, "base")
 
 
@@ -88,23 +95,25 @@
     return branch(username, ghnum, "head")
 
 
 def branch_orig(username: str, ghnum: GhNumber) -> GitCommitHash:
     return branch(username, ghnum, "orig")
 
 
-RE_MENTION = re.compile(r'@([a-z\d](?:[a-z\d]|-(?=[a-z\d])){0,38})', re.I)
+RE_MENTION = re.compile(r"@([a-z\d](?:[a-z\d]|-(?=[a-z\d])){0,38})", re.I)
 
 
 # Replace GitHub mentions with non mentions, to prevent spamming people
 def strip_mentions(body: str) -> str:
-    return RE_MENTION.sub(r'\1', body)
+    return RE_MENTION.sub(r"\1", body)
 
 
-STACK_HEADER = "Stack from [ghstack](https://github.com/ezyang/ghstack) (oldest at bottom)"
+STACK_HEADER = (
+    "Stack from [ghstack](https://github.com/ezyang/ghstack) (oldest at bottom)"
+)
 
 
 @dataclass
 class DiffWithGitHubMetadata:
     diff: ghstack.diff.Diff
     number: GitHubNumber
     username: str
@@ -113,30 +122,31 @@
     title: str
     body: str
     closed: bool
     ghnum: GhNumber
     pull_request_resolved: ghstack.diff.PullRequestResolved
 
 
-def main(*,
-         msg: Optional[str],
-         username: str,
-         github: ghstack.github.GitHubEndpoint,
-         update_fields: bool = False,
-         sh: Optional[ghstack.shell.Shell] = None,
-         stack_header: str = STACK_HEADER,
-         repo_owner: Optional[str] = None,
-         repo_name: Optional[str] = None,
-         short: bool = False,
-         force: bool = False,
-         no_skip: bool = False,
-         draft: bool = False,
-         github_url: str,
-         remote_name: str
-         ) -> List[Optional[DiffMeta]]:
+def main(
+    *,
+    msg: Optional[str],
+    username: str,
+    github: ghstack.github.GitHubEndpoint,
+    update_fields: bool = False,
+    sh: Optional[ghstack.shell.Shell] = None,
+    stack_header: str = STACK_HEADER,
+    repo_owner: Optional[str] = None,
+    repo_name: Optional[str] = None,
+    short: bool = False,
+    force: bool = False,
+    no_skip: bool = False,
+    draft: bool = False,
+    github_url: str,
+    remote_name: str,
+) -> List[Optional[DiffMeta]]:
 
     if sh is None:
         # Use CWD
         sh = ghstack.shell.Shell()
 
     repo = ghstack.github_utils.get_github_repo_info(
         github=github,
@@ -154,67 +164,75 @@
             "Cowardly refusing to upload diffs to a repository that is a "
             "fork.  ghstack expects '{}' of your Git checkout to point "
             "to the upstream repository in question.  If your checkout does "
             "not comply, please either adjust your remotes (by editing "
             ".git/config) or change the 'remote_name' field in your .ghstackrc "
             "file to point to the correct remote.  If this message is in "
             "error, please register your complaint on GitHub issues (or edit "
-            "this line to delete the check above).".format(remote_name))
+            "this line to delete the check above).".format(remote_name)
+        )
     repo_id = repo["id"]
     default_branch = repo["default_branch"]
 
     sh.git("fetch", "--prune", remote_name)
-    base = GitCommitHash(sh.git("merge-base", f"{remote_name}/{default_branch}", "HEAD"))
+    base = GitCommitHash(
+        sh.git("merge-base", f"{remote_name}/{default_branch}", "HEAD")
+    )
 
     # compute the stack of commits to process (reverse chronological order),
     stack = ghstack.git.parse_header(
         sh.git("rev-list", "--header", "^" + base, "HEAD"),
         github_url,
     )
 
     # compute the base commit
-    base_obj = ghstack.git.split_header(sh.git("rev-list", "--header", "^" + base + "^@", base))[0]
+    base_obj = ghstack.git.split_header(
+        sh.git("rev-list", "--header", "^" + base + "^@", base)
+    )[0]
 
     assert len(stack) > 0
 
     run_pre_ghstack_hook(sh, base, stack[0].oid)
 
-    ghstack.logs.record_status(
-        "{} \"{}\"".format(stack[0].oid[:9], stack[0].title))
+    ghstack.logs.record_status('{} "{}"'.format(stack[0].oid[:9], stack[0].title))
 
-    submitter = Submitter(github=github,
-                          sh=sh,
-                          username=username,
-                          repo_owner=repo_owner_nonopt,
-                          repo_name=repo_name_nonopt,
-                          repo_id=repo_id,
-                          base_commit=base,
-                          base_tree=base_obj.tree(),
-                          stack_base=base,
-                          stack_header=stack_header,
-                          update_fields=update_fields,
-                          msg=msg,
-                          short=short,
-                          force=force,
-                          no_skip=no_skip,
-                          draft=draft,
-                          stack=list(reversed(stack)),
-                          github_url=github_url,
-                          remote_name=remote_name)
+    submitter = Submitter(
+        github=github,
+        sh=sh,
+        username=username,
+        repo_owner=repo_owner_nonopt,
+        repo_name=repo_name_nonopt,
+        repo_id=repo_id,
+        base_commit=base,
+        base_tree=base_obj.tree(),
+        stack_base=base,
+        stack_header=stack_header,
+        update_fields=update_fields,
+        msg=msg,
+        short=short,
+        force=force,
+        no_skip=no_skip,
+        draft=draft,
+        stack=list(reversed(stack)),
+        github_url=github_url,
+        remote_name=remote_name,
+    )
     submitter.prepare_updates()
     submitter.push_updates()
 
     # NB: earliest first
     return submitter.stack_meta
 
 
 def all_branches(username: str, ghnum: GhNumber) -> Tuple[str, str, str]:
-    return (branch_base(username, ghnum),
-            branch_head(username, ghnum),
-            branch_orig(username, ghnum))
+    return (
+        branch_base(username, ghnum),
+        branch_head(username, ghnum),
+        branch_orig(username, ghnum),
+    )
 
 
 def push_spec(commit: GitCommitHash, branch: str) -> str:
     return "{}:refs/heads/{}".format(commit, branch)
 
 
 class Submitter(object):
@@ -311,203 +329,218 @@
     # Github url (normally github.com)
     github_url: str
 
     # Name of the upstream remote (normally origin)
     remote_name: str
 
     def __init__(
-            self,
-            github: ghstack.github.GitHubEndpoint,
-            sh: ghstack.shell.Shell,
-            username: str,
-            repo_owner: str,
-            repo_name: str,
-            repo_id: GitHubRepositoryId,
-            base_commit: GitCommitHash,
-            base_tree: GitTreeHash,
-            stack_base: GitCommitHash,
-            stack_header: str,
-            update_fields: bool,
-            msg: Optional[str],
-            stack: List[ghstack.diff.Diff],
-            short: bool,
-            force: bool,
-            no_skip: bool,
-            draft: bool,
-            github_url: str,
-            remote_name: str):
+        self,
+        github: ghstack.github.GitHubEndpoint,
+        sh: ghstack.shell.Shell,
+        username: str,
+        repo_owner: str,
+        repo_name: str,
+        repo_id: GitHubRepositoryId,
+        base_commit: GitCommitHash,
+        base_tree: GitTreeHash,
+        stack_base: GitCommitHash,
+        stack_header: str,
+        update_fields: bool,
+        msg: Optional[str],
+        stack: List[ghstack.diff.Diff],
+        short: bool,
+        force: bool,
+        no_skip: bool,
+        draft: bool,
+        github_url: str,
+        remote_name: str,
+    ):
         self.github = github
         self.sh = sh
         self.username = username
         self.repo_owner = repo_owner
         self.repo_name = repo_name
         self.repo_id = repo_id
         self.base_commit = base_commit
         self.base_orig = base_commit
         self.base_tree = base_tree
         self.stack_base = stack_base
         self.update_fields = update_fields
-        self.stack_header = None if stack_header is None else stack_header.format(github_url=github_url)
+        self.stack_header = stack_header.format(github_url=github_url)
         self.stack_meta = []
         self.ignored_diffs = []
         self.stack = stack
         self.seen_ghnums = set()
         self.msg = msg
         self.short = short
         self.force = force
         self.no_skip = no_skip
         self.draft = draft
         self.github_url = github_url
         self.remote_name = remote_name
 
-    def _default_title_and_body(self, commit: ghstack.diff.Diff,
-                                old_pr_body: Optional[str]
-                                ) -> Tuple[str, str]:
+    def _default_title_and_body(
+        self, commit: ghstack.diff.Diff, old_pr_body: Optional[str]
+    ) -> Tuple[str, str]:
         """
         Compute what the default title and body of a newly opened pull
         request would be, given the existing commit message.
 
         If you pass in the old PR body, we also preserve "Differential
         Revision" information in the PR body.  We only overwrite PR
         body if you explicitly ask for it with --update-fields, but
         it's good not to lose Phabricator diff assignment, so we special
         case this.
         """
         title = commit.title
-        extra = ''
+        extra = ""
         if old_pr_body is not None:
             # Look for tags we should preserve, and keep them
             m = RE_DIFF_REV.search(old_pr_body)
             if m:
                 extra = (
                     "\n\nDifferential Revision: "
                     "[{phabdiff}]"
                     "(https://our.internmc.facebook.com/intern/diff/{phabdiff})"
                 ).format(phabdiff=m.group(1))
-        commit_body = ''.join(commit.summary.splitlines(True)[1:]).lstrip()
+        commit_body = "".join(commit.summary.splitlines(True)[1:]).lstrip()
         # Don't store ghstack-source-id in the PR body; it will become
         # stale quickly
-        commit_body = RE_GHSTACK_SOURCE_ID.sub('', commit_body)
+        commit_body = RE_GHSTACK_SOURCE_ID.sub("", commit_body)
         # Don't store Pull request resolved in the PR body; it's
         # unnecessary
-        commit_body = ghstack.diff.re_pull_request_resolved_w_sp(self.github_url).sub('', commit_body)
-        pr_body = (
-            "{}:\n* (to be filled)\n\n{}{}"
-            .format(self.stack_header,
-                    commit_body,
-                    extra)
+        commit_body = ghstack.diff.re_pull_request_resolved_w_sp(self.github_url).sub(
+            "", commit_body
+        )
+        pr_body = "{}:\n* (to be filled)\n\n{}{}".format(
+            self.stack_header, commit_body, extra
         )
         return title, pr_body
 
     def _is_valid_ref(self, ref: str) -> bool:
-        splits = ref.split('/')
+        splits = ref.split("/")
         if len(splits) < 3:
             return False
         else:
             return splits[-2].isnumeric()
 
-    def elaborate_diff(self, commit: ghstack.diff.Diff, *,
-                       is_ghexport: bool = False) -> DiffWithGitHubMetadata:
+    def elaborate_diff(
+        self, commit: ghstack.diff.Diff, *, is_ghexport: bool = False
+    ) -> DiffWithGitHubMetadata:
         """
         Query GitHub API for the current title, body and closed? status
         of the pull request corresponding to a ghstack.diff.Diff.
         """
 
         assert commit.pull_request_resolved is not None
         assert commit.pull_request_resolved.owner == self.repo_owner
         assert commit.pull_request_resolved.repo == self.repo_name
 
         number = commit.pull_request_resolved.number
         # TODO: There is no reason to do a node query here; we can
         # just look up the repo the old fashioned way
-        r = self.github.graphql("""
+        r = self.github.graphql(
+            """
           query ($repo_id: ID!, $number: Int!) {
             node(id: $repo_id) {
               ... on Repository {
                 pullRequest(number: $number) {
                   body
                   title
                   closed
                   headRefName
                 }
               }
             }
           }
-        """, repo_id=self.repo_id, number=number)["data"]["node"]["pullRequest"]
+        """,
+            repo_id=self.repo_id,
+            number=number,
+        )["data"]["node"]["pullRequest"]
 
         # Sorry, this is a big hack to support the ghexport case
-        m = re.match(r'(refs/heads/)?export-D([0-9]+)$', r['headRefName'])
+        m = re.match(r"(refs/heads/)?export-D([0-9]+)$", r["headRefName"])
         if m is not None and is_ghexport:
-            raise RuntimeError('''\
+            raise RuntimeError(
+                """\
 This commit appears to already be associated with a pull request,
 but the pull request was previously submitted with an old version of
 ghexport.  You can continue exporting using the old style using:
 
     ghexport --legacy
 
 For future diffs, we recommend using the non-legacy version of ghexport
 as it supports bidirectional syncing.  However, there is no way to
 convert a pre-existing PR in the old style to the new format which
 supports bidirectional syncing.  If you would like to blow away the old
 PR and start anew, edit the Summary in the Phabricator diff to delete
 the line 'Pull Request resolved' and then run ghexport again.
-''')
+"""
+            )
 
         # TODO: Hmm, I'm not sure why this matches
-        m = re.match(r'gh/([^/]+)/([0-9]+)/head$', r['headRefName'])
+        m = re.match(r"gh/([^/]+)/([0-9]+)/head$", r["headRefName"])
         if m is None:
             if is_ghexport:
-                raise RuntimeError('''\
+                raise RuntimeError(
+                    """\
 This commit appears to already be associated with a pull request,
 but the pull request doesn't look like it was submitted by ghexport
 Maybe you exported it using the "Export to Open Source" button on
 the Phabricator diff page?  If so, please continue to use that button
 to export your diff.
 
 If you think this is in error, edit the Summary in the Phabricator diff
 to delete the line 'Pull Request resolved' and then run ghexport again.
-''')
+"""
+                )
             else:
-                raise RuntimeError('''\
+                raise RuntimeError(
+                    """\
 This commit appears to already be associated with a pull request,
 but the pull request doesn't look like it was submitted by ghstack.
 If you think this is in error, run:
 
     ghstack unlink {}
 
 to disassociate the commit with the pull request, and then try again.
 (This will create a new pull request!)
-'''.format(commit.oid))
+""".format(
+                        commit.oid
+                    )
+                )
         username = m.group(1)
         gh_number = GhNumber(m.group(2))
 
         # NB: Technically, we don't need to pull this information at
         # all, but it's more convenient to unconditionally edit
         # title/body when we update the pull request info
-        title = r['title']
-        pr_body = r['body']
+        title = r["title"]
+        pr_body = r["body"]
         if self.update_fields:
             title, pr_body = self._default_title_and_body(commit, pr_body)
 
         # TODO: remote summary should be done earlier so we can use
         # it to test if updates are necessary
         remote_summary = ghstack.git.split_header(
             self.sh.git(
-                "rev-list", "--max-count=1", "--header",
-                self.remote_name + "/" + branch_orig(username, gh_number)
+                "rev-list",
+                "--max-count=1",
+                "--header",
+                self.remote_name + "/" + branch_orig(username, gh_number),
             )
         )[0]
         m_remote_source_id = RE_GHSTACK_SOURCE_ID.search(remote_summary.commit_msg())
         remote_source_id = m_remote_source_id.group(1) if m_remote_source_id else None
 
         return DiffWithGitHubMetadata(
             diff=commit,
             title=title,
             body=pr_body,
-            closed=r['closed'],
+            closed=r["closed"],
             number=number,
             username=username,
             ghnum=gh_number,
             remote_source_id=remote_source_id,
             pull_request_resolved=commit.pull_request_resolved,
         )
 
@@ -518,162 +551,188 @@
         so you're still obligated to call this even if you think there's
         nothing to do.
         """
 
         ghnum = commit.ghnum
         username = commit.username
 
-        self.stack_meta.append(DiffMeta(
-            title=commit.title,
-            number=commit.number,
-            body=commit.body,
-            ghnum=ghnum,
-            username=username,
-            push_branches=(),
-            head_branch=None,
-            what='Skipped',
-            closed=commit.closed,
-            pr_url=commit.pull_request_resolved.url(self.github_url),
-        ))
-
-        self.base_commit = GitCommitHash(self.sh.git(
-            "rev-parse",
-            self.remote_name + "/" + branch_head(username, ghnum)))
-        self.base_orig = GitCommitHash(self.sh.git(
-            "rev-parse",
-            self.remote_name + "/" + branch_orig(username, ghnum)
-        ))
-        self.base_tree = GitTreeHash(self.sh.git(
-            "rev-parse", self.base_orig + "^{tree}"
-        ))
+        self.stack_meta.append(
+            DiffMeta(
+                title=commit.title,
+                number=commit.number,
+                body=commit.body,
+                ghnum=ghnum,
+                username=username,
+                push_branches=(),
+                head_branch=None,
+                what="Skipped",
+                closed=commit.closed,
+                pr_url=commit.pull_request_resolved.url(self.github_url),
+            )
+        )
+
+        self.base_commit = GitCommitHash(
+            self.sh.git(
+                "rev-parse", self.remote_name + "/" + branch_head(username, ghnum)
+            )
+        )
+        self.base_orig = GitCommitHash(
+            self.sh.git(
+                "rev-parse", self.remote_name + "/" + branch_orig(username, ghnum)
+            )
+        )
+        self.base_tree = GitTreeHash(
+            self.sh.git("rev-parse", self.base_orig + "^{tree}")
+        )
 
     def process_new_commit(self, commit: ghstack.diff.Diff) -> None:
         """
         Process a diff that has never been pushed to GitHub before.
         """
 
-        if '[ghstack-poisoned]' in commit.summary:
-            raise RuntimeError('''\
+        if "[ghstack-poisoned]" in commit.summary:
+            raise RuntimeError(
+                """\
 This commit is poisoned: it is from a head or base branch--ghstack
 cannot validly submit it.  The most common situation for this to
 happen is if you checked out the head branch of a pull request that was
 previously submitted with ghstack (e.g., by using hub checkout).
 Making modifications on the head branch is not supported; instead,
 you should fetch the original commits in question by running:
 
     ghstack checkout $PR_URL
 
 Since we cannot proceed, ghstack will abort now.
-''')
+"""
+            )
 
         title, pr_body = self._default_title_and_body(commit, None)
 
         # Determine the next available GhNumber.  We do this by
         # iterating through known branches and keeping track
         # of the max.  The next available GhNumber is the next number.
         # This is technically subject to a race, but we assume
         # end user is not running this script concurrently on
         # multiple machines (you bad bad)
         refs = self.sh.git(
             "for-each-ref",
             # Use OUR username here, since there's none attached to the
             # diff
             "refs/remotes/{}/gh/{}".format(self.remote_name, self.username),
-            "--format=%(refname)").split()
+            "--format=%(refname)",
+        ).split()
         refs = list(filter(lambda r: self._is_valid_ref(r), refs))
-        max_ref_num = max(int(ref.split('/')[-2]) for ref in refs) \
-            if refs else 0
+        max_ref_num = max(int(ref.split("/")[-2]) for ref in refs) if refs else 0
         ghnum = GhNumber(str(max_ref_num + 1))
 
         # Create the incremental pull request diff
         tree = commit.patch.apply(self.sh, self.base_tree)
 
         # Actually, if there's no change in the tree, stop processing
         if tree == self.base_tree:
             self.ignored_diffs.append((commit, None))
-            logging.warning("Skipping {} {}, as the commit has no changes"
-                         .format(commit.oid, title))
+            logging.warning(
+                "Skipping {} {}, as the commit has no changes".format(commit.oid, title)
+            )
             self.stack_meta.append(None)
             return
 
         assert ghnum not in self.seen_ghnums
         self.seen_ghnums.add(ghnum)
 
         new_pull = GitCommitHash(
-            self.sh.git("commit-tree", *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
-                        "-p", self.base_commit, tree,
-                        input=commit.summary + "\n\n[ghstack-poisoned]"))
+            self.sh.git(
+                "commit-tree",
+                *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
+                "-p",
+                self.base_commit,
+                tree,
+                input=commit.summary + "\n\n[ghstack-poisoned]",
+            )
+        )
 
         # Push the branches, so that we can create a PR for them
         new_branches = (
             push_spec(new_pull, branch_head(self.username, ghnum)),
-            push_spec(self.base_commit, branch_base(self.username, ghnum))
+            push_spec(self.base_commit, branch_base(self.username, ghnum)),
         )
         self.sh.git(
             "push",
             self.remote_name,
             *new_branches,
         )
         self.github.push_hook(new_branches)
 
         # Time to open the PR
         # NB: GraphQL API does not support opening PRs
         r = self.github.post(
-            "repos/{owner}/{repo}/pulls"
-            .format(owner=self.repo_owner, repo=self.repo_name),
+            "repos/{owner}/{repo}/pulls".format(
+                owner=self.repo_owner, repo=self.repo_name
+            ),
             title=title,
             head=branch_head(self.username, ghnum),
             base=branch_base(self.username, ghnum),
             body=pr_body,
             maintainer_can_modify=True,
             draft=self.draft,
         )
-        number = r['number']
+        number = r["number"]
 
         logging.info("Opened PR #{}".format(number))
 
         # Update the commit message of the local diff with metadata
         # so we can correlate these later
         pull_request_resolved = ghstack.diff.PullRequestResolved(
-            owner=self.repo_owner, repo=self.repo_name, number=number)
-        commit_msg = ("{commit_msg}\n\n"
-                      "ghstack-source-id: {sourceid}\n"
-                      "Pull Request resolved: "
-                      "https://{github_url}/{owner}/{repo}/pull/{number}"
-                      .format(commit_msg=strip_mentions(commit.summary.rstrip()),
-                              owner=self.repo_owner,
-                              repo=self.repo_name,
-                              number=number,
-                              sourceid=commit.source_id,
-                              github_url=self.github_url))
+            owner=self.repo_owner, repo=self.repo_name, number=number
+        )
+        commit_msg = (
+            "{commit_msg}\n\n"
+            "ghstack-source-id: {sourceid}\n"
+            "Pull Request resolved: "
+            "https://{github_url}/{owner}/{repo}/pull/{number}".format(
+                commit_msg=strip_mentions(commit.summary.rstrip()),
+                owner=self.repo_owner,
+                repo=self.repo_name,
+                number=number,
+                sourceid=commit.source_id,
+                github_url=self.github_url,
+            )
+        )
         env = {}
         if commit.author_name is not None:
-            env['GIT_AUTHOR_NAME'] = commit.author_name
+            env["GIT_AUTHOR_NAME"] = commit.author_name
         if commit.author_email is not None:
-            env['GIT_AUTHOR_EMAIL'] = commit.author_email
+            env["GIT_AUTHOR_EMAIL"] = commit.author_email
 
-        new_orig = GitCommitHash(self.sh.git(
-            "commit-tree",
-            *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
-            "-p", self.base_orig,
-            tree,
-            input=commit_msg, env=env))
+        new_orig = GitCommitHash(
+            self.sh.git(
+                "commit-tree",
+                *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
+                "-p",
+                self.base_orig,
+                tree,
+                input=commit_msg,
+                env=env,
+            )
+        )
 
-        self.stack_meta.append(DiffMeta(
-            title=title,
-            number=number,
-            body=pr_body,
-            ghnum=ghnum,
-            username=self.username,
-            push_branches=((new_orig, 'orig'), ),
-            head_branch=new_pull,
-            what='Created',
-            closed=False,
-            pr_url=pull_request_resolved.url(self.github_url),
-        ))
+        self.stack_meta.append(
+            DiffMeta(
+                title=title,
+                number=number,
+                body=pr_body,
+                ghnum=ghnum,
+                username=self.username,
+                push_branches=((new_orig, "orig"),),
+                head_branch=new_pull,
+                what="Created",
+                closed=False,
+                pr_url=pull_request_resolved.url(self.github_url),
+            )
+        )
 
         self.base_commit = new_pull
         self.base_orig = new_orig
         self.base_tree = tree
 
     def process_old_commit(self, elab_commit: DiffWithGitHubMetadata) -> None:
         """
@@ -687,55 +746,61 @@
 
         if ghnum in self.seen_ghnums:
             raise RuntimeError(
                 "Something very strange has happened: a commit for "
                 "the pull request #{} occurs twice in your local "
                 "commit stack.  This is usually because of a botched "
                 "rebase.  Please take a look at your git log and seek "
-                "help from your local Git expert.".format(number))
+                "help from your local Git expert.".format(number)
+            )
         self.seen_ghnums.add(ghnum)
 
         logging.info("Pushing to #{}".format(number))
 
         # Compute the local and remote source IDs
         summary = commit.summary
         m_local_source_id = RE_GHSTACK_SOURCE_ID.search(summary)
         if m_local_source_id is None:
             # For BC, just slap on a source ID.  After BC is no longer
             # needed, we can just error in this case; however, this
             # situation is extremely likely to happen for preexisting
             # stacks.
             logging.warning(
                 "Local commit has no ghstack-source-id; assuming that it is "
-                "up-to-date with remote.")
+                "up-to-date with remote."
+            )
             summary = "{}\nghstack-source-id: {}".format(summary, commit.source_id)
         else:
             local_source_id = m_local_source_id.group(1)
             if elab_commit.remote_source_id is None:
                 # This should also be an error condition, but I suppose
                 # it can happen in the wild if a user had an aborted
                 # ghstack run, where they updated their head pointer to
                 # a copy with source IDs, but then we failed to push to
                 # orig.  We should just go ahead and push in that case.
                 logging.warning(
                     "Remote commit has no ghstack-source-id; assuming that we are "
-                    "up-to-date with remote.")
+                    "up-to-date with remote."
+                )
             else:
                 if local_source_id != elab_commit.remote_source_id and not self.force:
-                    logging.debug(f"elab_commit.remote_source_id = {elab_commit.remote_source_id}")
+                    logging.debug(
+                        f"elab_commit.remote_source_id = {elab_commit.remote_source_id}"
+                    )
                     raise RuntimeError(
                         "Cowardly refusing to push an update to GitHub, since it "
                         "looks another source has updated GitHub since you last "
                         "pushed.  If you want to push anyway, rerun this command "
                         "with --force.  Otherwise, diff your changes against "
                         "{} and reapply them on top of an up-to-date commit from "
-                        "GitHub.".format(local_source_id))
+                        "GitHub.".format(local_source_id)
+                    )
                 summary = RE_GHSTACK_SOURCE_ID.sub(
-                    'ghstack-source-id: {}\n'.format(commit.source_id),
-                    summary)
+                    "ghstack-source-id: {}\n".format(commit.source_id), summary
+                )
 
         # We've got an update to do!  But what exactly should we
         # do?
         #
         # Here are a number of situations which may have
         # occurred.
         #
@@ -776,24 +841,24 @@
         # as the gh/ezyang/X/base commit.
         #
         # In this case, we don't need to include the base as a
         # parent at all; just construct our new diff as a plain,
         # non-merge commit.
         base_args: Tuple[str, ...]
         orig_base_hash = self.sh.git(
-            "rev-parse",
-            self.remote_name + "/" + branch_base(username, ghnum))
+            "rev-parse", self.remote_name + "/" + branch_base(username, ghnum)
+        )
 
         # I vacillated between whether or not we should use the PR
         # body or the literal commit message here.  Right now we use
         # the PR body, because after initial commit the original
         # commit message is not supposed to "matter" anymore.  orig
         # still uses the original commit message, however, because
         # it's supposed to be the "original".
-        non_orig_commit_msg = strip_mentions(RE_STACK.sub('', elab_commit.body))
+        non_orig_commit_msg = strip_mentions(RE_STACK.sub("", elab_commit.body))
 
         if orig_base_hash == self.base_commit:
 
             new_base = self.base_commit
             base_args = ()
 
         else:
@@ -801,110 +866,134 @@
             # the old base. If not, we need to include the local stack
             # base as a parent of the new commit base.
             same_stack_base = self.sh.git(
                 "merge-base",
                 "--is-ancestor",
                 self.stack_base,
                 self.remote_name + "/" + branch_base(username, ghnum),
-                exitcode=True)
+                exitcode=True,
+            )
 
             # Make a fake commit that
             # "resets" the tree back to something that makes
             # sense and merge with that.  This doesn't fix
             # the fact that we still incorrectly report
             # the old base as an ancestor of our commit, but
             # it's better than nothing.
-            new_base = GitCommitHash(self.sh.git(
-                "commit-tree", *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
-                "-p",
-                self.remote_name + "/" + branch_base(username, ghnum),
-                *(() if same_stack_base else ("-p", self.stack_base)),
-                self.base_tree,
-                input='Update base for {} on "{}"\n\n{}\n\n[ghstack-poisoned]'
-                      .format(self.msg, elab_commit.title,
-                              non_orig_commit_msg)))
+            new_base = GitCommitHash(
+                self.sh.git(
+                    "commit-tree",
+                    *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
+                    "-p",
+                    self.remote_name + "/" + branch_base(username, ghnum),
+                    *(() if same_stack_base else ("-p", self.stack_base)),
+                    self.base_tree,
+                    input='Update base for {} on "{}"\n\n{}\n\n[ghstack-poisoned]'.format(
+                        self.msg, elab_commit.title, non_orig_commit_msg
+                    ),
+                )
+            )
 
             base_args = ("-p", new_base)
 
         # Blast our current tree as the newest commit, merging
         # against the previous pull entry, and the newest base.
 
         tree = commit.patch.apply(self.sh, self.base_tree)
 
         # Nothing to do, just ignore the diff
         if tree == self.base_tree:
             self.ignored_diffs.append((commit, number))
-            logging.warning("Skipping PR #{} {}, as the commit now has no changes"
-                         .format(number, elab_commit.title))
+            logging.warning(
+                "Skipping PR #{} {}, as the commit now has no changes".format(
+                    number, elab_commit.title
+                )
+            )
             return
 
-        new_pull = GitCommitHash(self.sh.git(
-            "commit-tree", *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
-            "-p", self.remote_name + "/" + branch_head(username, ghnum),
-            *base_args,
-            tree,
-            input='{} on "{}"\n\n{}\n\n[ghstack-poisoned]'.format(self.msg, elab_commit.title, non_orig_commit_msg)))
+        new_pull = GitCommitHash(
+            self.sh.git(
+                "commit-tree",
+                *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
+                "-p",
+                self.remote_name + "/" + branch_head(username, ghnum),
+                *base_args,
+                tree,
+                input='{} on "{}"\n\n{}\n\n[ghstack-poisoned]'.format(
+                    self.msg, elab_commit.title, non_orig_commit_msg
+                ),
+            )
+        )
 
         # Perform what is effectively an interactive rebase
         # on the orig branch.
         #
         # Hypothetically, there could be a case when this isn't
         # necessary, but it's INCREDIBLY unlikely (because we'd
         # have to look EXACTLY like the original orig, and since
         # we're in the branch that says "hey we changed
         # something" that's probably not what happened.
 
         logging.info("Restacking commit on {}".format(self.base_orig))
-        new_orig = GitCommitHash(self.sh.git(
-            "commit-tree", *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
-            "-p", self.base_orig, tree, input=summary))
+        new_orig = GitCommitHash(
+            self.sh.git(
+                "commit-tree",
+                *ghstack.gpg_sign.gpg_args_if_necessary(self.sh),
+                "-p",
+                self.base_orig,
+                tree,
+                input=summary,
+            )
+        )
 
         push_branches = (
             (new_base, "base"),
             (new_pull, "head"),
             (new_orig, "orig"),
         )
 
         if elab_commit.closed:
-            what = 'Skipped closed'
+            what = "Skipped closed"
         else:
-            what = 'Updated'
+            what = "Updated"
 
-        self.stack_meta.append(DiffMeta(
-            title=elab_commit.title,
-            number=number,
-            # NB: Ignore the commit message, and just reuse the old commit
-            # message.  This is consistent with 'jf submit' default
-            # behavior.  The idea is that people may have edited the
-            # PR description on GitHub and you don't want to clobber
-            # it.
-            body=elab_commit.body,
-            ghnum=ghnum,
-            username=username,
-            push_branches=push_branches,
-            head_branch=new_pull,
-            what=what,
-            closed=elab_commit.closed,
-            pr_url=elab_commit.pull_request_resolved.url(self.github_url),
-        ))
+        self.stack_meta.append(
+            DiffMeta(
+                title=elab_commit.title,
+                number=number,
+                # NB: Ignore the commit message, and just reuse the old commit
+                # message.  This is consistent with 'jf submit' default
+                # behavior.  The idea is that people may have edited the
+                # PR description on GitHub and you don't want to clobber
+                # it.
+                body=elab_commit.body,
+                ghnum=ghnum,
+                username=username,
+                push_branches=push_branches,
+                head_branch=new_pull,
+                what=what,
+                closed=elab_commit.closed,
+                pr_url=elab_commit.pull_request_resolved.url(self.github_url),
+            )
+        )
 
         self.base_commit = new_pull
         self.base_orig = new_orig
         self.base_tree = tree
 
     def _format_stack(self, index: int) -> str:
         rows = []
         for i, s in reversed(list(enumerate(self.stack_meta))):
             if s is None:
                 continue
             if index == i:
-                rows.append(f'* __->__ #{s.number}')
+                rows.append(f"* __->__ #{s.number}")
             else:
-                rows.append(f'* #{s.number}')
-        return self.stack_header + ':\n' + '\n'.join(rows) + '\n'
+                rows.append(f"* #{s.number}")
+        return self.stack_header + ":\n" + "\n".join(rows) + "\n"
 
     def prepare_updates(self, *, is_ghexport: bool = False) -> None:
         """
         Go through each commit in the stack and construct the commits
         which we will push to GitHub shortly.  If a commit does not have
         an associated PR, push it immediately and create a PR so that we
         ensure that every diff in stack_meta has an associated pull
@@ -918,15 +1007,20 @@
                 d = self.elaborate_diff(s, is_ghexport=is_ghexport)
                 # In principle, we can still skip commits if both their
                 # trees and orig commits match; and even if the messages
                 # don't match we only really need to push an updated
                 # orig commit.  However, the code to make this happen is
                 # a bit bothersome, so I don't do it for now, to fix a
                 # very real bug.
-                if skip and d.remote_source_id == s.source_id and not self.no_skip and not self.update_fields:
+                if (
+                    skip
+                    and d.remote_source_id == s.source_id
+                    and not self.no_skip
+                    and not self.update_fields
+                ):
                     self.skip_commit(d)
                 else:
                     skip = False
                     self.process_old_commit(d)
             else:
                 skip = False
                 self.process_new_commit(s)
@@ -950,43 +1044,48 @@
         force_push_branches: List[str] = []
         for i, s in enumerate(self.stack_meta):
             # NB: GraphQL API does not support modifying PRs
             if s is None:
                 continue
             if not s.closed:
                 logging.info(
-                    "# Updating https://{github_url}/{owner}/{repo}/pull/{number}"
-                    .format(github_url=self.github_url,
-                            owner=self.repo_owner,
-                            repo=self.repo_name,
-                            number=s.number))
+                    "# Updating https://{github_url}/{owner}/{repo}/pull/{number}".format(
+                        github_url=self.github_url,
+                        owner=self.repo_owner,
+                        repo=self.repo_name,
+                        number=s.number,
+                    )
+                )
                 self.github.patch(
-                    "repos/{owner}/{repo}/pulls/{number}"
-                    .format(owner=self.repo_owner, repo=self.repo_name,
-                            number=s.number),
+                    "repos/{owner}/{repo}/pulls/{number}".format(
+                        owner=self.repo_owner, repo=self.repo_name, number=s.number
+                    ),
                     body=RE_STACK.sub(self._format_stack(i), s.body),
-                    title=s.title)
+                    title=s.title,
+                )
             else:
                 logging.info(
-                    "# Skipping closed https://{github_url}/{owner}/{repo}/pull/{number}"
-                    .format(github_url=self.github_url,
-                            owner=self.repo_owner,
-                            repo=self.repo_name,
-                            number=s.number))
+                    "# Skipping closed https://{github_url}/{owner}/{repo}/pull/{number}".format(
+                        github_url=self.github_url,
+                        owner=self.repo_owner,
+                        repo=self.repo_name,
+                        number=s.number,
+                    )
+                )
 
             # It is VERY important that we do base updates BEFORE real
             # head updates, otherwise GitHub will spuriously think that
             # the user pushed a number of patches as part of the PR,
             # when actually they were just from the (new) upstream
             # branch
 
             for commit, b in s.push_branches:
-                if b == 'orig':
+                if b == "orig":
                     q = force_push_branches
-                elif b == 'base':
+                elif b == "base":
                     q = base_push_branches
                 else:
                     q = push_branches
                 q.append(push_spec(commit, branch(s.username, s.ghnum, b)))
         # Careful!  Don't push master.
         # TODO: These pushes need to be atomic (somehow)
         if base_push_branches:
@@ -997,27 +1096,32 @@
             self.github.push_hook(push_branches)
         if force_push_branches:
             self.sh.git("push", self.remote_name, "--force", *force_push_branches)
             self.github.push_hook(force_push_branches)
 
         # Report what happened
         def format_url(s: DiffMeta) -> str:
-            return ("https://{github_url}/{owner}/{repo}/pull/{number}"
-                    .format(github_url=self.github_url,
-                            owner=self.repo_owner,
-                            repo=self.repo_name,
-                            number=s.number))
+            return "https://{github_url}/{owner}/{repo}/pull/{number}".format(
+                github_url=self.github_url,
+                owner=self.repo_owner,
+                repo=self.repo_name,
+                number=s.number,
+            )
 
         if self.short:
             # Guarantee that the FIRST PR URL is the top of the stack
-            print('\n'.join(format_url(s) for s in reversed(self.stack_meta) if s is not None))
+            print(
+                "\n".join(
+                    format_url(s) for s in reversed(self.stack_meta) if s is not None
+                )
+            )
             return
 
         print()
-        print('# Summary of changes (ghstack {})'.format(ghstack.__version__))
+        print("# Summary of changes (ghstack {})".format(ghstack.__version__))
         print()
         if self.stack_meta:
             for s in reversed(self.stack_meta):
                 if s is None:
                     continue
                 url = format_url(s)
                 print(" - {} {}".format(s.what, url))
@@ -1026,45 +1130,63 @@
             if import_help:
                 top_of_stack = None
                 for x in self.stack_meta:
                     if x is not None:
                         top_of_stack = x
                 assert top_of_stack is not None
 
-                print("Facebook employees can import your changes by running ")
-                print("(on a Facebook machine):")
+                print("Meta employees can import your changes by running ")
+                print("(on a Meta machine):")
                 print()
                 print("    ghimport -s {}".format(format_url(top_of_stack)))
                 print()
                 print("If you want to work on this diff stack on another machine:")
                 print()
                 print("    ghstack checkout {}".format(format_url(top_of_stack)))
                 print("")
         else:
-            print("No pull requests updated; all commits in your diff stack were empty!")
+            print(
+                "No pull requests updated; all commits in your diff stack were empty!"
+            )
 
         if self.ignored_diffs:
             print()
             print("FYI: I ignored the following commits, because they had no changes:")
             print()
             noop_pr = False
             for d, pr in reversed(self.ignored_diffs):
                 if pr is None:
                     print(" - {} {}".format(d.oid[:8], d.title))
                 else:
                     noop_pr = True
-                    print(" - {} {} (was previously submitted as PR #{})".format(d.oid[:8], d.title, pr))
+                    print(
+                        " - {} {} (was previously submitted as PR #{})".format(
+                            d.oid[:8], d.title, pr
+                        )
+                    )
             if noop_pr:
                 print()
-                print("I did NOT close or update PRs previously associated with these commits.")
+                print(
+                    "I did NOT close or update PRs previously associated with these commits."
+                )
 
 
-def run_pre_ghstack_hook(sh: ghstack.shell.Shell, base_commit: str, top_commit: str) -> None:
+def run_pre_ghstack_hook(
+    sh: ghstack.shell.Shell, base_commit: str, top_commit: str
+) -> None:
     """If a `pre-ghstack` git hook is configured, run it."""
-    default_hooks_path = os.path.join(sh.git("rev-parse", "--show-toplevel"), ".git/hooks")
-    hooks_path = sh.git("config", "--default", default_hooks_path, "--get", "core.hooksPath")
-    hook_file = os.path.join(hooks_path, "pre-ghstack")
+    default_hooks_path = os.path.join(
+        sh.git("rev-parse", "--show-toplevel"), ".git/hooks"
+    )
+    try:
+        hooks_path = sh.git(
+            "config", "--default", default_hooks_path, "--get", "core.hooksPath"
+        )
+        hook_file = os.path.join(hooks_path, "pre-ghstack")
+    except Exception as e:
+        logging.warning(f"Pre ghstack hook failed: {e}")
+        return
 
     if not os.path.isfile(hook_file) or not os.access(hook_file, os.X_OK):
         return
 
     sh.sh(hook_file, base_commit, top_commit, stdout=None)
```

### Comparing `ghstack-0.7.1/ghstack/types.py` & `ghstack-0.8.0/ghstack/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 
 from typing import NewType
 
 # A bunch of commonly used type definitions.
 
-PhabricatorDiffNumberWithD = \
-    NewType('PhabricatorDiffNumberWithD', str)  # aka "D1234567"
+PhabricatorDiffNumberWithD = NewType(
+    "PhabricatorDiffNumberWithD", str
+)  # aka "D1234567"
 
-GitHubNumber = NewType('GitHubNumber', int)  # aka 1234 (as in #1234)
+GitHubNumber = NewType("GitHubNumber", int)  # aka 1234 (as in #1234)
 
 # GraphQL ID that identifies Repository from GitHubb schema;
 # aka MDExOlB1bGxSZXF1ZXN0MjU2NDM3MjQw
-GitHubRepositoryId = NewType('GitHubRepositoryId', str)
+GitHubRepositoryId = NewType("GitHubRepositoryId", str)
 
 # aka 12 (as in gh/ezyang/12/base)
-GhNumber = NewType('GhNumber', str)
+GhNumber = NewType("GhNumber", str)
 
 # Actually, sometimes we smuggle revs in here.  We shouldn't.
 # We want to guarantee that they're full canonical revs so that
 # you can do equality on them without fear.
 # commit 3f72e04eeabcc7e77f127d3e7baf2f5ccdb148ee
-GitCommitHash = NewType('GitCommitHash', str)
+GitCommitHash = NewType("GitCommitHash", str)
 
 # tree 3f72e04eeabcc7e77f127d3e7baf2f5ccdb148ee
-GitTreeHash = NewType('GitTreeHash', str)
+GitTreeHash = NewType("GitTreeHash", str)
```

### Comparing `ghstack-0.7.1/ghstack/unlink.py` & `ghstack-0.8.0/ghstack/unlink.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 import ghstack.git
 import ghstack.github
 import ghstack.github_utils
 import ghstack.gpg_sign
 import ghstack.shell
 from ghstack.types import GitCommitHash
 
-RE_GHSTACK_SOURCE_ID = re.compile(r'^ghstack-source-id: (.+)\n?', re.MULTILINE)
+RE_GHSTACK_SOURCE_ID = re.compile(r"^ghstack-source-id: (.+)\n?", re.MULTILINE)
 
 
-def main(*,
-         commits: Optional[List[str]] = None,
-         github: ghstack.github.GitHubEndpoint,
-         sh: Optional[ghstack.shell.Shell] = None,
-         repo_owner: Optional[str] = None,
-         repo_name: Optional[str] = None,
-         github_url: str,
-         remote_name: str) -> GitCommitHash:
+def main(
+    *,
+    commits: Optional[List[str]] = None,
+    github: ghstack.github.GitHubEndpoint,
+    sh: Optional[ghstack.shell.Shell] = None,
+    repo_owner: Optional[str] = None,
+    repo_name: Optional[str] = None,
+    github_url: str,
+    remote_name: str,
+) -> GitCommitHash:
     # If commits is empty, we unlink the entire stack
     #
     # For now, we only process commits on our current
     # stack, because we have no way of knowing how to
     # "restack" for other commits.
 
     if sh is None:
@@ -46,32 +48,37 @@
     # Parse the commits
     parsed_commits: Optional[Set[GitCommitHash]] = None
     if commits:
         parsed_commits = set()
         for c in commits:
             parsed_commits.add(GitCommitHash(sh.git("rev-parse", c)))
 
-    base = GitCommitHash(sh.git("merge-base", f"{remote_name}/{default_branch}", "HEAD"))
+    base = GitCommitHash(
+        sh.git("merge-base", f"{remote_name}/{default_branch}", "HEAD")
+    )
 
     # compute the stack of commits in chronological order (does not
     # include base)
     stack = ghstack.git.split_header(
-        sh.git("rev-list", "--reverse", "--header", "^" + base, "HEAD"))
+        sh.git("rev-list", "--reverse", "--header", "^" + base, "HEAD")
+    )
 
     # sanity check the parsed_commits
     if parsed_commits is not None:
         stack_commits = set()
         for s in stack:
             stack_commits.add(s.commit_id())
         invalid_commits = parsed_commits - stack_commits
         if invalid_commits:
             raise RuntimeError(
                 "unlink can only process commits which are on the "
-                "current stack; these commits are not:\n{}"
-                .format("\n".join(invalid_commits)))
+                "current stack; these commits are not:\n{}".format(
+                    "\n".join(invalid_commits)
+                )
+            )
 
     # Run the interactive rebase.  Don't start rewriting until we
     # hit the first commit that needs it.
     head = base
     rewriting = False
 
     for s in stack:
@@ -80,33 +87,44 @@
         if not rewriting and not should_unlink:
             # Advance HEAD without reconstructing commit
             head = commit_id
             continue
 
         rewriting = True
         commit_msg = s.commit_msg()
-        logging.debug("-- commit_msg:\n{}".format(textwrap.indent(commit_msg, '   ')))
+        logging.debug("-- commit_msg:\n{}".format(textwrap.indent(commit_msg, "   ")))
         if should_unlink:
             commit_msg = RE_GHSTACK_SOURCE_ID.sub(
-                '',
-                ghstack.diff.re_pull_request_resolved_w_sp(github_url).sub('', commit_msg)
+                "",
+                ghstack.diff.re_pull_request_resolved_w_sp(github_url).sub(
+                    "", commit_msg
+                ),
+            )
+            logging.debug(
+                "-- edited commit_msg:\n{}".format(textwrap.indent(commit_msg, "   "))
+            )
+        head = GitCommitHash(
+            sh.git(
+                "commit-tree",
+                *ghstack.gpg_sign.gpg_args_if_necessary(sh),
+                s.tree(),
+                "-p",
+                head,
+                input=commit_msg,
             )
-            logging.debug("-- edited commit_msg:\n{}".format(
-                textwrap.indent(commit_msg, '   ')))
-        head = GitCommitHash(sh.git(
-            "commit-tree",
-            *ghstack.gpg_sign.gpg_args_if_necessary(sh),
-            s.tree(),
-            "-p", head,
-            input=commit_msg))
+        )
 
-    sh.git('reset', '--soft', head)
+    sh.git("reset", "--soft", head)
 
-    logging.info("""
+    logging.info(
+        """
 Diffs successfully unlinked!
 
 To undo this operation, run:
 
     git reset --soft {}
-""".format(s.commit_id()))
+""".format(
+            s.commit_id()
+        )
+    )
 
     return head
```

### Comparing `ghstack-0.7.1/pyproject.toml` & `ghstack-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [tool.poetry]
 name = "ghstack"
-version = "0.7.1"
+version = "0.8.0"
 authors = ["Edward Z. Yang <ezyang@mit.edu>"]
 description = "Stack diff support for GitHub"
 readme = "README.md"
 repository = "https://github.com/ezyang/ghstack"
 include = ["ghstack/py.typed"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.scripts]
-ghstack = "ghstack.__main__:main"
+ghstack = "ghstack.cli:main"
 
 [tool.poetry.dependencies]
 aiohttp = "^3"
-dataclasses = { version = "^0.8", python = "<3.7" }
-importlib-metadata = "^3"
-python = "^3.6"
+importlib-metadata = { version = ">=1.4", python = "<3.8" }
+python = "^3.8"
 requests = "^2"
 typing-extensions = ">=3 <5"
+click = "^8"
 
 [tool.poetry.dev-dependencies]
+black = "^22.12.0"
 expecttest = "^0.1"
 flake8 = "^3"
 graphql-core = "^3"
 hypothesis = "^6"
-isort = "^5"
-mypy = "^0.800"
-pytest = "^6"
+mypy = "^1"
+pytest = "^7"
+usort = "^1"
+ufmt = "^2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ghstack-0.7.1/setup.py` & `ghstack-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,35 @@
 packages = \
 ['ghstack']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3,<4',
- 'importlib-metadata>=3,<4',
- 'requests>=2,<3',
- 'typing-extensions>=3,<5']
+['aiohttp>=3,<4', 'click>=8,<9', 'requests>=2,<3', 'typing-extensions>=3,<5']
 
 extras_require = \
-{':python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
+{':python_version < "3.8"': ['importlib-metadata>=1.4']}
 
 entry_points = \
-{'console_scripts': ['ghstack = ghstack.__main__:main']}
+{'console_scripts': ['ghstack = ghstack.cli:main']}
 
 setup_kwargs = {
     'name': 'ghstack',
-    'version': '0.7.1',
+    'version': '0.8.0',
     'description': 'Stack diff support for GitHub',
-    'long_description': '# ghstack\n\nConveniently submit stacks of diffs to GitHub as separate pull requests.\n\n```\npip3 install ghstack\n```\n\nPython 3.6 and greater only.\n\n## How to setup\n\nGo to github.com `Settings→Developer Settings→Personal Access Tokens` and\ngenerate a token with `public_repo` access only.\nCreate a `~/.ghstackrc` as shown below:\n```\nλ cat ~/.ghstackrc\n[ghstack]\ngithub_url = github.com\ngithub_oauth = [your_own_token]\ngithub_username = [your_username]\nremote_name = upstream [if remote is called upstream and not origin]\n```\n\n## How to use\n\nMake sure you have write permission to the repo you\'re opening PR with.\n\nPrepare a series of commits on top of master, then run `ghstack`.  This\ntool will push and create pull requests for each commit on the stack.\n\n**How do I stack another PR on top of an existing one?** Assuming\nyou\'ve checked out the latest commit from the existing PR, just\n`git commit` a new commit on top, and then run `ghstack`.\n\n**How do I modify a PR?**  Just edit the commit in question, and then\nrun `ghstack` again.  If the commit is at the top of your stack,\nyou can edit it with `git commit --amend`; otherwise, you\'ll have\nto use `git rebase -i` to edit the commit directly.\n\n**How do I rebase?**  The obvious way: `git rebase origin/master`.\nDon\'t do a `git merge`; `ghstack` will throw a hissy fit if you\ndo that.  (There\'s also a more fundamental reason why this\nwon\'t work: since each commit is a separate PR, you have to\nresolve conflicts in *each* PR, not just for the entire stack.)\n\n**How do I start a new feature?**  Just checkout master on a new\nbranch, and start working on a fresh branch.\n\n**WARNING.**  You will NOT be able to merge these commits using the\nnormal GitHub UI, as their branch bases won\'t be master.  Use\n`ghstack land $PR_URL` to land a ghstack\'ed pull request.\n\n## Structure of submitted pull requests\n\nEvery commit in your local commit stack gets submitted into a separate\npull request and pushes commits onto three branches:\n\n* `gh/username/1/base` - think of this like "master": it\'s the base\n  branch that your commit was based upon.  It is never force pushed;\n  whenever you rebase your local stack, we add merge commits on top of\n  base from the true upstream master.\n\n* `gh/username/1/head` - this branch is your change, on top of the base\n  branch.  Like base, it is never force pushed.  We open a pull request\n  on this branch, requesting to merge into base.\n\n* `gh/username/1/orig` - this is the actual commit as per your local\n  copy.  GitHub pull requests never sees this commit, but if you want\n  to get a "clean" commit all by itself, for example, because you\n  want to work on the commits from another machine, this is the best way\n  to get it.\n\n## Developer notes\n\nThis project uses [Poetry](https://python-poetry.org/docs/#installation), so\nafter you\'ve installed Poetry itself, run this command in your clone of this\nrepo to install all the dependencies you need for working on `ghstack`:\n```\npoetry install\n```\nNote that this installs the dependencies (and `ghstack` itself) in an isolated\nPython virtual environment rather than globally. If your cwd is in your clone of\nthis repo then you can run your locally-built `ghstack` using `poetry run\nghstack $ARGS`, but if you want to run it from somewhere else, you probably want\n[`poetry shell`](https://python-poetry.org/docs/cli/#shell) instead:\n```\npoetry shell\ncd $SOMEWHERE\nghstack $ARGS\n```\n\n### Testing\n\nWe have tests, using a mock GitHub GraphQL server!  How cool is that?\n```\npoetry run python test_ghstack.py\n```\nThat runs most of the tests; you can run all tests (including lints) like this:\n```\npoetry run ./run_tests.sh\n```\n\n### Publishing\n\nYou can also [use Poetry to\npublish](https://python-poetry.org/docs/cli/#publish) to a package repository.\nFor instance, if you\'ve configured your [Poetry\nrepositories](https://python-poetry.org/docs/repositories/) like this:\n```\npoetry config repositories.testpypi https://test.pypi.org/legacy/\n```\nThen you can publish to TestPyPI like this:\n```\npoetry publish --build --repository testpypi\n```\nTo publish to PyPI itself, just omit the `--repository` argument.\n\n## Design constraints\n\nThere are some weird aspects about GitHub\'s design which lead to unusual\ndesign decisions on this tool.\n\n1. When you create a PR on GitHub, it is ALWAYS created on the\n   repository that the base branch exists on.  Thus, we MUST\n   push branches to the upstream repository that you want\n   PRs to be created on.  This can result in a lot of stale\n   branches hanging around; you\'ll need to setup some other\n   mechanism for pruning these branches.\n\n2. Branch name does not correspond to pull request number. While this\n   would be excellent, we have no way of reserving a pull request\n   number, so we have no idea what it\'s going to be until we open\n   the pull request, but we can\'t open the pull request without a\n   branch.\n\n## Ripley Cupboard\n\nChanneling Conor McBride, this section documents mistakes worth\nmentioning.\n\n**Non-stack mode.**  ghstack processes your entire stack when it\nuploads updates, but it doesn\'t have to be that way; you could\nimagine that you could ask ghstack to only process the topmost\ncommit and leave the rest alone.  An easy and attractive\nlooking way of doing this is to edit the stack selection algorithm\nto look a single commit, rather than all the commits from\nmerge-base to head.\n\nThis sounds OK but you try it and you realize two things:\n\n1. This is wrong, if you exclude the commits before your commit\n   you\'ll end up with a base commit based on the "literal"\n   commit in your Git repository.  But this has no relationship\n   with the base commit that was previously uploaded, which\n   was synthetically constructed.\n\n2. You also have do extra work to pull out an up to date stack\n   to write into the pull request body.\n\nSo, this is not impossible to do, but it will need some work.\nYou have to work out what the real base commit is, whether\nor not you need to advance it, and also rewrite the stack rendering\ncode.\n',
+    'long_description': '# ghstack\n\nConveniently submit stacks of diffs to GitHub as separate pull requests.\n\n```\npip3 install ghstack\n```\n\nPython 3.8 and greater only.\n\n## How to setup\n\nGo to github.com `Settings→Developer Settings→Personal Access Tokens` and\ngenerate a token with `public_repo` access only.\nCreate a `~/.ghstackrc` as shown below:\n```\nλ cat ~/.ghstackrc\n[ghstack]\ngithub_url = github.com\ngithub_oauth = [your_own_token]\ngithub_username = [your_username]\nremote_name = upstream [if remote is called upstream and not origin]\n```\n\n## How to use\n\nMake sure you have write permission to the repo you\'re opening PR with.\n\nPrepare a series of commits on top of master, then run `ghstack`.  This\ntool will push and create pull requests for each commit on the stack.\n\n**How do I stack another PR on top of an existing one?** Assuming\nyou\'ve checked out the latest commit from the existing PR, just\n`git commit` a new commit on top, and then run `ghstack`.\n\n**How do I modify a PR?**  Just edit the commit in question, and then\nrun `ghstack` again.  If the commit is at the top of your stack,\nyou can edit it with `git commit --amend`; otherwise, you\'ll have\nto use `git rebase -i` to edit the commit directly.\n\n**How do I rebase?**  The obvious way: `git rebase origin/master`.\nDon\'t do a `git merge`; `ghstack` will throw a hissy fit if you\ndo that.  (There\'s also a more fundamental reason why this\nwon\'t work: since each commit is a separate PR, you have to\nresolve conflicts in *each* PR, not just for the entire stack.)\n\n**How do I start a new feature?**  Just checkout master on a new\nbranch, and start working on a fresh branch.\n\n**WARNING.**  You will NOT be able to merge these commits using the\nnormal GitHub UI, as their branch bases won\'t be master.  Use\n`ghstack land $PR_URL` to land a ghstack\'ed pull request.\n\n## Structure of submitted pull requests\n\nEvery commit in your local commit stack gets submitted into a separate\npull request and pushes commits onto three branches:\n\n* `gh/username/1/base` - think of this like "master": it\'s the base\n  branch that your commit was based upon.  It is never force pushed;\n  whenever you rebase your local stack, we add merge commits on top of\n  base from the true upstream master.\n\n* `gh/username/1/head` - this branch is your change, on top of the base\n  branch.  Like base, it is never force pushed.  We open a pull request\n  on this branch, requesting to merge into base.\n\n* `gh/username/1/orig` - this is the actual commit as per your local\n  copy.  GitHub pull requests never sees this commit, but if you want\n  to get a "clean" commit all by itself, for example, because you\n  want to work on the commits from another machine, this is the best way\n  to get it.\n\n## Developer notes\n\nThis project uses [Poetry](https://python-poetry.org/docs/#installation), so\nafter you\'ve installed Poetry itself, run this command in your clone of this\nrepo to install all the dependencies you need for working on `ghstack`:\n```\npoetry install\n```\nNote that this installs the dependencies (and `ghstack` itself) in an isolated\nPython virtual environment rather than globally. If your cwd is in your clone of\nthis repo then you can run your locally-built `ghstack` using `poetry run\nghstack $ARGS`, but if you want to run it from somewhere else, you probably want\n[`poetry shell`](https://python-poetry.org/docs/cli/#shell) instead:\n```\npoetry shell\ncd $SOMEWHERE\nghstack $ARGS\n```\n\n### Testing\n\nWe have tests, using a mock GitHub GraphQL server!  How cool is that?\n```\npoetry run python test_ghstack.py\n```\nThat runs most of the tests; you can run all tests (including lints) like this:\n```\npoetry run ./run_tests.sh\n```\n\n### Publishing\n\nYou can also [use Poetry to\npublish](https://python-poetry.org/docs/cli/#publish) to a package repository.\nFor instance, if you\'ve configured your [Poetry\nrepositories](https://python-poetry.org/docs/repositories/) like this:\n```\npoetry config repositories.testpypi https://test.pypi.org/legacy/\n```\nThen you can publish to TestPyPI like this:\n```\npoetry publish --build --repository testpypi\n```\nTo publish to PyPI itself, just omit the `--repository` argument.\n\n## Design constraints\n\nThere are some weird aspects about GitHub\'s design which lead to unusual\ndesign decisions on this tool.\n\n1. When you create a PR on GitHub, it is ALWAYS created on the\n   repository that the base branch exists on.  Thus, we MUST\n   push branches to the upstream repository that you want\n   PRs to be created on.  This can result in a lot of stale\n   branches hanging around; you\'ll need to setup some other\n   mechanism for pruning these branches.\n\n2. Branch name does not correspond to pull request number. While this\n   would be excellent, we have no way of reserving a pull request\n   number, so we have no idea what it\'s going to be until we open\n   the pull request, but we can\'t open the pull request without a\n   branch.\n\n## Ripley Cupboard\n\nChanneling Conor McBride, this section documents mistakes worth\nmentioning.\n\n**Non-stack mode.**  ghstack processes your entire stack when it\nuploads updates, but it doesn\'t have to be that way; you could\nimagine that you could ask ghstack to only process the topmost\ncommit and leave the rest alone.  An easy and attractive\nlooking way of doing this is to edit the stack selection algorithm\nto look a single commit, rather than all the commits from\nmerge-base to head.\n\nThis sounds OK but you try it and you realize two things:\n\n1. This is wrong, if you exclude the commits before your commit\n   you\'ll end up with a base commit based on the "literal"\n   commit in your Git repository.  But this has no relationship\n   with the base commit that was previously uploaded, which\n   was synthetically constructed.\n\n2. You also have do extra work to pull out an up to date stack\n   to write into the pull request body.\n\nSo, this is not impossible to do, but it will need some work.\nYou have to work out what the real base commit is, whether\nor not you need to advance it, and also rewrite the stack rendering\ncode.\n',
     'author': 'Edward Z. Yang',
     'author_email': 'ezyang@mit.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ezyang/ghstack',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ghstack-0.7.1/PKG-INFO` & `ghstack-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: ghstack
-Version: 0.7.1
+Version: 0.8.0
 Summary: Stack diff support for GitHub
 Home-page: https://github.com/ezyang/ghstack
 License: MIT
 Author: Edward Z. Yang
 Author-email: ezyang@mit.edu
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3,<4)
-Requires-Dist: dataclasses (>=0.8,<0.9); python_version < "3.7"
-Requires-Dist: importlib-metadata (>=3,<4)
+Requires-Dist: click (>=8,<9)
+Requires-Dist: importlib-metadata (>=1.4); python_version < "3.8"
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: typing-extensions (>=3,<5)
 Project-URL: Repository, https://github.com/ezyang/ghstack
 Description-Content-Type: text/markdown
 
 # ghstack
 
 Conveniently submit stacks of diffs to GitHub as separate pull requests.
 
 ```
 pip3 install ghstack
 ```
 
-Python 3.6 and greater only.
+Python 3.8 and greater only.
 
 ## How to setup
 
 Go to github.com `Settings→Developer Settings→Personal Access Tokens` and
 generate a token with `public_repo` access only.
 Create a `~/.ghstackrc` as shown below:
 ```
```

