# Comparing `tmp/git-check-rebase-0.3.tar.gz` & `tmp/git-check-rebase-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-check-rebase-0.3.tar", last modified: Wed Nov  2 11:34:52 2022, max compression
+gzip compressed data, was "git-check-rebase-0.4.tar", last modified: Wed Jul 12 14:12:41 2023, max compression
```

## Comparing `git-check-rebase-0.3.tar` & `git-check-rebase-0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2022-11-02 11:34:52.005342 git-check-rebase-0.3/
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1157 2022-11-01 18:13:54.000000 git-check-rebase-0.3/LICENSE
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     2192 2022-11-02 11:34:52.005342 git-check-rebase-0.3/PKG-INFO
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1860 2022-11-01 19:49:57.000000 git-check-rebase-0.3/README.rst
--rwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)    10570 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git-check-rebase
-drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2022-11-02 11:34:52.005342 git-check-rebase-0.3/git_check_rebase/
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)        0 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/__init__.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     7111 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/check_rebase_meta.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)    12486 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/compare_commits.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)    11380 2022-11-02 10:13:49.000000 git-check-rebase-0.3/git_check_rebase/compare_ranges.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1024 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/html_table_view.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1549 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/parse_jira.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1039 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/simple_git.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1312 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/span.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1033 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/text_table_view.py
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1736 2022-11-02 10:05:06.000000 git-check-rebase-0.3/git_check_rebase/viewable.py
-drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2022-11-02 11:34:52.005342 git-check-rebase-0.3/git_check_rebase.egg-info/
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     2192 2022-11-02 11:34:51.000000 git-check-rebase-0.3/git_check_rebase.egg-info/PKG-INFO
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)      569 2022-11-02 11:34:51.000000 git-check-rebase-0.3/git_check_rebase.egg-info/SOURCES.txt
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)        1 2022-11-02 11:34:51.000000 git-check-rebase-0.3/git_check_rebase.egg-info/dependency_links.txt
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       19 2022-11-02 11:34:51.000000 git-check-rebase-0.3/git_check_rebase.egg-info/requires.txt
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       17 2022-11-02 11:34:51.000000 git-check-rebase-0.3/git_check_rebase.egg-info/top_level.txt
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       38 2022-11-02 11:34:52.005342 git-check-rebase-0.3/setup.cfg
--rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)      665 2022-11-02 11:30:16.000000 git-check-rebase-0.3/setup.py
+drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2023-07-12 14:12:41.954301 git-check-rebase-0.4/
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     2265 2023-07-12 14:12:41.954301 git-check-rebase-0.4/PKG-INFO
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1863 2023-03-31 06:12:18.000000 git-check-rebase-0.4/README.rst
+-rwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)    11619 2023-07-12 13:27:07.000000 git-check-rebase-0.4/git-check-rebase
+drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2023-07-12 14:12:41.954301 git-check-rebase-0.4/git_check_rebase/
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)        0 2023-03-31 06:12:18.000000 git-check-rebase-0.4/git_check_rebase/__init__.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     7204 2023-07-12 10:10:07.000000 git-check-rebase-0.4/git_check_rebase/check_rebase_meta.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)    12486 2023-07-12 10:43:02.000000 git-check-rebase-0.4/git_check_rebase/compare_commits.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)    12636 2023-07-12 10:43:02.000000 git-check-rebase-0.4/git_check_rebase/compare_ranges.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1791 2023-07-12 10:06:08.000000 git-check-rebase-0.4/git_check_rebase/gcr_jira.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1128 2023-07-12 10:43:02.000000 git-check-rebase-0.4/git_check_rebase/html_table_view.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1334 2023-07-12 10:06:08.000000 git-check-rebase-0.4/git_check_rebase/parse_issues.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1039 2023-03-31 06:12:18.000000 git-check-rebase-0.4/git_check_rebase/simple_git.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1312 2023-03-31 06:12:18.000000 git-check-rebase-0.4/git_check_rebase/span.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     1146 2023-07-12 13:25:47.000000 git-check-rebase-0.4/git_check_rebase/text_table_view.py
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     2339 2023-07-12 10:43:02.000000 git-check-rebase-0.4/git_check_rebase/viewable.py
+drwxrwxr-x   0 vsementsov  (1000) vsementsov  (1000)        0 2023-07-12 14:12:41.954301 git-check-rebase-0.4/git_check_rebase.egg-info/
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)     2265 2023-07-12 14:12:41.000000 git-check-rebase-0.4/git_check_rebase.egg-info/PKG-INFO
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)      592 2023-07-12 14:12:41.000000 git-check-rebase-0.4/git_check_rebase.egg-info/SOURCES.txt
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)        1 2023-07-12 14:12:41.000000 git-check-rebase-0.4/git_check_rebase.egg-info/dependency_links.txt
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       19 2023-07-12 14:12:41.000000 git-check-rebase-0.4/git_check_rebase.egg-info/requires.txt
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       17 2023-07-12 14:12:41.000000 git-check-rebase-0.4/git_check_rebase.egg-info/top_level.txt
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)       38 2023-07-12 14:12:41.954301 git-check-rebase-0.4/setup.cfg
+-rw-rw-r--   0 vsementsov  (1000) vsementsov  (1000)      780 2023-07-12 14:11:06.000000 git-check-rebase-0.4/setup.py
```

### Comparing `git-check-rebase-0.3/PKG-INFO` & `git-check-rebase-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: git-check-rebase
-Version: 0.3
+Version: 0.4
 Summary: Some useful scripts to operate track history and patch changes during rebases.
 Home-page: https://gitlab.com/vsementsov/git-check-rebase
 Author: Vladimir Sementsov-Ogievskiy
 Author-email: vsementsov@yandex-team.ru
 License: MIT
+Project-URL: Docs, https://git-check-rebase.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst
 
 git check-rebase
 ================
 
 Installation
 ------------
@@ -44,8 +45,8 @@
 - Check backported series
 - Check status of rebasing a downstream branch to a new upstream release
 - Check upstreaming status of commits in downstream branch
 
 Documentation
 -------------
 
-Full documentation is `here <https://git-check-rebase.readthedocs.io/en/upd/>`_
+Full documentation is `here <https://git-check-rebase.readthedocs.io/en/latest/>`_
```

### Comparing `git-check-rebase-0.3/README.rst` & `git-check-rebase-0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 - Check backported series
 - Check status of rebasing a downstream branch to a new upstream release
 - Check upstreaming status of commits in downstream branch
 
 Documentation
 -------------
 
-Full documentation is `here <https://git-check-rebase.readthedocs.io/en/upd/>`_
+Full documentation is `here <https://git-check-rebase.readthedocs.io/en/latest/>`_
```

### Comparing `git-check-rebase-0.3/git-check-rebase` & `git-check-rebase-0.4/git-check-rebase`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 from tempfile import mkstemp
 from typing import Optional, Type
 from types import TracebackType
-import tabulate
+import tabulate  # type: ignore
 
 from git_check_rebase import text_table_view, html_table_view
 
 from git_check_rebase.check_rebase_meta import Meta
-from git_check_rebase.compare_ranges import MultiRange, CompRes, \
+from git_check_rebase.compare_ranges import MultiRange, \
     RowsHideLevel, NoBaseError, Column, Table
 from git_check_rebase.compare_commits import interactive_compare_commits, \
     check_git_clean_branch
 
-from git_check_rebase.viewable import Span
+from git_check_rebase.viewable import Span, CompRes
 
 tabulate.PRESERVE_WHITESPACE = True
 
 
 def print_legend(viewer, ranges, html):
     def_style = (
         ('Critical bugs', 'bug-critical'),
@@ -30,47 +30,46 @@
     )
     tab = [[Span(f'███████ - {desc}', style)] for desc, style in def_style]
     tab += [[r.legend] for r in ranges if r.legend]
     print(viewer.view_table(tab))
 
 
 class GitCheckRebase:
-    def __init__(self, range_defs, meta_path, html, jira, jira_issues, legend,
-                 columns, rows_hide_level, interactive, color,
+    def __init__(self, range_defs, meta_path, html, issue_tracker,
+                 porting_issues, legend,
+                 columns, rows_hide_level, rows_filter, interactive, color,
                  ign_commit_messages):
         self.range_defs = range_defs
-        self.jira = jira
-        self.jira_issues = jira_issues
+        self.issue_tracker = issue_tracker
+        self.porting_issues = \
+            porting_issues.split(',') if porting_issues else []
         self.legend = legend
         self.rows_hide_level = rows_hide_level
+        self.rows_filter = rows_filter
         self.interactive = interactive
         self.ign_commit_messages = ign_commit_messages
         self.ranges = []  # see parse_range_defs
         self.tab = None  # see main
 
         self.headers = columns != 'short'
         if columns is None:
             self.columns = (Column.COMMITS, Column.SUBJECT)
         elif columns == 'all':
             self.columns = [c for c in Column]
         else:
             cols = columns.split(',')
             if 'full' in cols:
                 i = cols.index('full')
-                cols[i : i + 1] = 'feature', 'commits', 'date', 'author', 'subject'
+                cols[i:i+1] = 'feature', 'commits', 'date', 'author', \
+                    'subject'
             if 'short' in cols:
                 i = cols.index('short')
-                cols[i : i + 1] = 'commits', 'subject'
+                cols[i:i+1] = 'commits', 'subject'
             self.columns = [Column[c.upper()] for c in cols]
 
-        if jira_issues:
-            assert jira is not None
-            self.jira = jira
-            self.jira_issues = jira_issues.split(',')
-
         self.html = html
         if html:
             self.fmt = 'html'
         elif color is None:
             self.fmt = 'colored' if sys.stdout.isatty() else 'plain'
         else:
             self.fmt = 'colored' if color else 'plain'
@@ -157,16 +156,17 @@
             if not self.interactive:
                 sys.exit('--start_from supported only in --interactive mode')
 
         self.parse_range_defs()
 
         self.tab = Table(self.ranges, self.meta)
         self.tab.do_comparison(self.ign_commit_messages)
-        if self.jira:
-            self.tab.add_jira_info(self.jira, self.jira_issues)
+        if self.porting_issues:
+            self.tab.add_porting_issues(self.issue_tracker,
+                                        self.porting_issues)
 
         if self.interactive:
             branch = check_git_clean_branch()
             for row_ind, row in enumerate(self.tab.rows):
                 if row.commits[0] is None:
                     base_ind = len(row.commits) - 1
                     other_inds = range(base_ind)
@@ -204,15 +204,16 @@
                         self.main(start_from=res)
                         return
                 if stop:
                     break
 
         out = self.tab.to_list(columns=self.columns,
                                headers=self.headers,
-                               rows_hide_level=self.rows_hide_level)
+                               rows_hide_level=self.rows_hide_level,
+                               rows_filter=self.rows_filter)
 
         if self.html:
             print("""<!DOCTYPE html>
                   <meta charset="utf-8"/>
                   <style>
                   body {
                      font-family: monospace;
@@ -232,52 +233,70 @@
     p = argparse.ArgumentParser(description="Compare git commit ranges")
 
     p.add_argument('ranges', metavar='range', nargs='+',
                    help='ranges to compare, '
                    'in form [<name>:]<git range or ref>')
     p.add_argument('--meta', help='optional, file with additional metadata')
     p.add_argument('--html', help='output in html format', action='store_true')
-    p.add_argument('--jira-issues',
-                   help='optional, comma-separated jira issues list')
-    p.add_argument('--jira', help='user:password@server')
+    p.add_argument('--porting-issues',
+                   help='''optional, comma-separated issues list.
+Issues are recursively searched for commit subjects in descriptions.
+Then, corresponding issue keys are used to fill "new" column if exist''')
+    p.add_argument('--issue-tracker', help='class of issue tracker')
     p.add_argument('--legend', help='print legend', action='store_true')
     p.add_argument('--columns',
                    help='which columns to show in table: "short" is default. '
                    '"full" adds author and date columns and also column '
                    'headers', default='short')
     p.add_argument('--rows-hide-level',
                    choices=[x.name.lower() for x in RowsHideLevel],
                    help='which rows to hide in table: "show_all" is default. ',
                    default=RowsHideLevel.SHOW_ALL.name.lower())
+    p.add_argument('--rows-filter',
+                   help='which rows to show. experimental feature')
     p.add_argument('--interactive',
                    help='do interactive comparison of not-equal commits. '
                    'For each commit to compare, vimdiff is started as a '
                    'subprocess. User should exit it successfully (by :qa) to '
                    'mark commits "ok", and with error (by :cq) to don\'t '
                    'mark commits "ok"', action='store_true')
     p.add_argument('--color',
-                   help='Highlight results. By default does coloring only '
-                   'when stdout is tty', action=argparse.BooleanOptionalAction,
-                   default=None)
+                   help='Highlight results. By default does coloring '
+                   'when stdout is tty', action='store_true')
+    p.add_argument('--no-color',
+                   help='Do not highlight results. By default does coloring '
+                   'when stdout is tty', action='store_true')
     p.add_argument('--ignore-commit-messages',
                    help='Ignore commit message when compare commits',
                    action='store_true')
     p.add_argument('--start-from', help='hash commit of right column to '
                    'start from for interactive check.')
 
     args = p.parse_args()
 
+    # TODO: instead, move to argparse.BooleanOptionalAction in future.
+    # Now python 3.9 (or higher) is still not enough popular
+    if args.color and args.no_color:
+        sys.exit('Using both --color and --no-color is not allowed')
+    color = None if not (args.color or args.no_color) else args.color
+
+    if color:
+        # For termcolor library
+        os.environ['FORCE_COLOR'] = 'yes'
+
     rows_hide_lvl = RowsHideLevel[args.rows_hide_level.upper()]
     try:
         gcr = GitCheckRebase(range_defs=args.ranges, meta_path=args.meta,
                              html=args.html,
-                             jira=args.jira, jira_issues=args.jira_issues,
+                             issue_tracker=args.issue_tracker,
+                             porting_issues=args.porting_issues,
                              legend=args.legend, columns=args.columns,
                              rows_hide_level=rows_hide_lvl,
+                             rows_filter=args.rows_filter,
                              interactive=args.interactive,
-                             color=args.color,
+                             color=color,
                              ign_commit_messages=args.ignore_commit_messages)
     except OSError as e:
         sys.exit(f'Failed to open "{args.meta}": {e.strerror}')
 
     with gcr:
         gcr.main(start_from=args.start_from)
```

### Comparing `git-check-rebase-0.3/git_check_rebase/check_rebase_meta.py` & `git-check-rebase-0.4/git_check_rebase/check_rebase_meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,21 +57,26 @@
         self.upstreaming = None
 
     def add_property(self, prop):
         raise ValueError
 
 
 class CommitMeta(Feature):
-    def __init__(self, subject, group=None):
+    def __init__(self, subject):
         self.subject = subject
         self.comment = ''
         self.checked = []
-        self.feature = group.feature if group else None
-        self.drop = group.drop if group else None
-        self.upstreaming = group.upstreaming if group else None
+        self.feature = None
+        self.drop = None
+        self.upstreaming = None
+
+    def add_group(self, group):
+        self.feature = group.feature
+        self.drop = group.drop
+        self.upstreaming = group.upstreaming
 
     def add_comment_line(self, comment):
         if self.comment:
             self.comment += '\n'
         self.comment += comment
 
     def add_checked_pair(self, h1, h2):
@@ -183,19 +188,22 @@
                         else:
                             assert key == '%drop'
                             current_obj = DropGroup(val)
                         groups_stack.append(current_obj)
 
                 else:
                     # Normal commit
-                    if subject_to_key(line) in self.by_key:
-                        raise ValueError('Double definition for: ' + line)
-                    group = groups_stack[-1] if groups_stack else None
-                    current_obj = CommitMeta(line, group=group)
-                    self.by_key[subject_to_key(line)] = current_obj
+                    key = subject_to_key(line)
+                    if key in self.by_key:
+                        current_obj = self.by_key[key]
+                    else:
+                        current_obj = CommitMeta(line)
+                        self.by_key[key] = current_obj
+                    if groups_stack:
+                        current_obj.add_group(groups_stack[-1])
 
     def alias_to_key(self, alias):
         return self.aliases.get(alias, alias)
 
     def subject_to_key(self, subject):
         return subject_to_key(subject, self)
```

### Comparing `git-check-rebase-0.3/git_check_rebase/compare_commits.py` & `git-check-rebase-0.4/git_check_rebase/compare_commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             '-c', 'cnoreabbrev ok GCheckRebaseOk',
             '-c', 'command GCheckRebaseStop wa! | cq 201',
             '-c', 'cnoreabbrev stop GCheckRebaseStop',]
 
     cmd += ['-c', ':norm gg']
 
     code = subprocess.run(cmd, check=False).returncode
-    return IntrCompRes(ok = code == 200, stop = code not in (0, 200))
+    return IntrCompRes(ok=(code == 200), stop=(code not in (0, 200)))
 
 
 def text_to_lines(text: str) -> List[str]:
     if not text:
         return []
 
     if text[-1] == '\n':
```

### Comparing `git-check-rebase-0.3/git_check_rebase/compare_ranges.py` & `git-check-rebase-0.4/git_check_rebase/compare_ranges.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import re
 
 from enum import Enum
 from dataclasses import dataclass
-from typing import List, Optional, Any, Union, Tuple, Dict
+from typing import List, Optional, Any, Tuple, Dict
 
 from .simple_git import git_log_table, git
 from .compare_commits import are_commits_equal
 from .check_rebase_meta import subject_to_key, text_add_indent, Meta, \
     CommitMeta
 
-from .viewable import Span, Issue, GitHashCell, CompRes, VTable
-
-
-def parse_jira_issue(jira_issue: Any) -> Issue:
-    return Issue(key = jira_issue.key,
-                 critical = jira_issue.fields.priority.name in ('Critical',
-                                                                'Blocker'),
-                 fixed = jira_issue.fields.resolution and
-                    jira_issue.fields.resolution.name == 'Fixed')
+from .viewable import Span, GitHashCell, CompRes, VTable, VTableRow
+from .parse_issues import parse_issues
 
 
 class NoBaseError(Exception):
     pass
 
 
 MINUS_REGEX = re.compile(r'([^^~]+)(\^\d*|~\d*)+-')
@@ -74,20 +67,39 @@
 
 @dataclass
 class Commit:
     commit_hash: str
     author_date: str
     author_name: str
     subject: str
+    in_tag: str
 
 
 def git_log_commits(git_range):
-    return [Commit(commit_hash=h, author_date=ad,
-                   author_name=an, subject=s) for h, ad, an, s in
-            git_log_table('%h %ad %an %s', git_range)]
+    res = []
+    for h, ad, an, d, s in git_log_table('%h %ad %an %D %s', git_range):
+        tag = ''
+        if 'tag' in d:
+            desc = next(x for x in d.split(',') if 'tag' in x)
+            tag = desc.split(':', 1)[1].strip()
+            if not re.fullmatch(r'v([0-9]+\.)*[0-9]+', tag):
+                tag = None
+        res.append(Commit(commit_hash=h, author_date=ad,
+                          author_name=an, subject=s, in_tag=tag))
+
+    current_tag = ''
+    for c in reversed(res):
+        if c.in_tag:
+            current_tag = c.in_tag
+            continue
+
+        if current_tag:
+            c.in_tag = current_tag
+
+    return res
 
 
 class MultiRange:
     """ Class maintains multiple git ranges """
     def __init__(self, definition, meta=None, default_base=None):
         if ':' in definition:
             self.name, definition = definition.split(':', 1)
@@ -119,18 +131,19 @@
     COMMITS = 3
     CHERRY = 4
     DATE = 5
     AUTHOR = 6
     MSG_ISSUES = 7
     SUBJECT = 8
 
+
 class Row:
     """Representation of on row if git-range-diff-table"""
     commits: List[Optional[GitHashCell]]
-    issues: List[Issue]
+    issues: List[Any]
     date: str
     author: str
     subject: str
     _meta: Optional[Meta]
     _key: str
 
     def __init__(self, ranges, ind, meta):
@@ -152,15 +165,16 @@
         self.author = c.author_name
         self.subject = c.subject
         self._meta = meta
         self._key = subject_to_key(c.subject, meta)
 
         msg = git(f'log -1 {c.commit_hash}')
         self.cherry = 'cherry picked' in msg
-        self.msg_issues = re.findall(r'\b[A-Z]+-\d+\b', msg)
+        self.msg_issues = list(set(re.findall(r'\b[A-Z]+-\d+\b(?!-)', msg)))
+        self.msg_issues.sort(key=lambda x: int(x.split('-', 1)[1]))
 
         m = re.search(r'^    Feature: (.*)$', msg, re.MULTILINE)
         if m:
             self.feature = m.group(1)
         else:
             self.feature = self.meta.feature if self.meta else None
 
@@ -192,14 +206,17 @@
                 out[self.new_ind] = sp
             elif self.up_ind != -1 and out[self.up_ind] is None:
                 out[self.up_ind] = sp
 
         if self.new_ind != -1 and out[self.new_ind] is None:
             out[self.new_ind] = self.issues
 
+        if self.new_ind != -1 and not out[self.new_ind]:
+            out[self.new_ind] = Span('███???███', 'unknown')
+
         return out
 
     def to_list(self, columns: List[Column],
                 default: Dict[Column, Any]) -> List[Any]:
 
         line = []
         for c in columns:
@@ -217,14 +234,33 @@
                 line.append(self.msg_issues)
             elif c == Column.CHERRY:
                 line.append('V' if self.cherry else None)
             else:
                 line.append(default[c])
         return line
 
+    def all_ok(self) -> bool:
+        return all(c is not None and c.comp != CompRes.NONE
+                   for c in self.commits)
+
+    def all_equal(self) -> bool:
+        return all(c is not None and
+                   c.comp in (CompRes.BASE, CompRes.EQUAL)
+                   for c in self.commits)
+
+    def match_filter(self, expr: str) -> bool:
+        if not expr:
+            return True
+        commits = self.get_commits()
+        env = {a: getattr(self, a) for a in dir(self) if a[0] != '_'}
+        for i, r in enumerate(self.ranges):
+            if r.name.isidentifier():
+                env[r.name] = commits[i]
+        return eval(expr, env)
+
 
 class RowsHideLevel(Enum):
     SHOW_ALL = 1
     HIDE_EQUAL = 2
     HIDE_CHECKED = 3
 
 
@@ -251,15 +287,19 @@
 
             key = subject_to_key(c.subject, meta)
             row = Row(ranges, i, meta)
 
             for r_ind, r in enumerate(ranges[:-1]):
                 if key in r.by_key:
                     j, c2 = r.by_key[key]
-                    row.commits[r_ind] = GitHashCell(c2.commit_hash)
+                    in_tag = ''
+                    if r_ind in (row.up_ind, row.new_ind):
+                        in_tag = c2.in_tag
+                    row.commits[r_ind] = GitHashCell(c2.commit_hash,
+                                                     in_tag=in_tag)
                     if j != i:
                         corresponding[r_ind] = False
 
             self.rows.append(row)
 
         # If user cares to pass ranges of same length, and all found commits
         # have same index in range as corresponding commit in last range,
@@ -302,54 +342,57 @@
 
             for i, c in enumerate(row.commits):
                 if c is None or i == base_ind:
                     continue
 
                 self._compare_commits(base, c, row.meta, ignore_cmsg)
 
-    def add_jira_info(self, jira, jira_issues):
-        from .parse_jira import parse_jira
-
-        auth, server = jira.rsplit('@', 1)
-        user, password = auth.split(':', 1)
-        jiramap = parse_jira('https://' + server, user, password, jira_issues,
-                             [r.subject for r in self.rows])
-
+    def add_porting_issues(self, issue_tracker, porting_issues):
+        if issue_tracker == 'jira':
+            from .gcr_jira import GCRTracer
+        else:
+            import importlib
+            mod, klass = issue_tracker.rsplit('.', 1)
+            GCRTracer = getattr(importlib.import_module(mod), klass)
+
+        tracker = GCRTracer()
+        issues_map = parse_issues(tracker, porting_issues,
+                                  [r.subject for r in self.rows])
         for row in self.rows:
-            issues = jiramap.get(row.subject)
+            issues = issues_map.get(row.subject)
             if issues:
-                row.issues = [parse_jira_issue(issue) for issue in issues]
+                row.issues = issues
 
     def to_list(self, columns: List[Column],
                 fmt: str = 'colored',
                 headers: bool = True,
-                rows_hide_level: RowsHideLevel = RowsHideLevel.SHOW_ALL) \
-            -> VTable:
+                rows_hide_level: RowsHideLevel = RowsHideLevel.SHOW_ALL,
+                rows_filter: str = '') -> VTable:
 
         out: VTable = []
         line: VTableRow
 
         if headers:
             line = [c.name for c in columns]
             if 'COMMITS' in line:
                 i = line.index('COMMITS')
-                line[i : i + 1] = [r.name for r in self.ranges]
+                line[i:i+1] = [r.name for r in self.ranges]
             out.append(line)
 
         index_len = len(str(len(self.rows)))
 
         for row_ind, row in enumerate(self.rows):
+            if not row.match_filter(rows_filter):
+                continue
+
             if rows_hide_level.value >= RowsHideLevel.HIDE_CHECKED.value and \
-                    all(c is not None and c.comp != CompRes.NONE for
-                        c in row.commits):
+                    row.all_ok():
                 continue
             if rows_hide_level.value >= RowsHideLevel.HIDE_EQUAL.value and \
-                    all(c is not None and
-                        c.comp in (CompRes.BASE, CompRes.EQUAL) for
-                        c in row.commits):
+                    row.all_equal():
                 continue
 
             line = row.to_list(columns, {
                 Column.INDEX: f'{row_ind + 1:0{index_len}}'
             })
 
             out.append(line)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git-check-rebase-0.3/git_check_rebase/html_table_view.py` & `git-check-rebase-0.4/git_check_rebase/html_table_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from .compare_ranges import GitHashCell, Table, RowsHideLevel
-from .viewable import Viewer, Span, GitHashCell
+from .viewable import Viewer, Span, GitHashCell, ConvertedTable
 
 
 colors = {
     'bug-critical': 'red',
     'bug-fixed': 'green',
     'matching': 'green',
     'bug': 'DarkCyan',
     'unknown': 'red',
     'equal': 'green',
     'base': 'green',
     'checked': 'orange',
+    'in-tag': 'orange',
     'drop': 'magenta',
     'none': None,
     None: None
 }
 
 
 class HtmlViewer(Viewer):
     def view_git_hash(self, h: GitHashCell) -> str:
         href = 'https://bb.yandex-team.ru/projects/CLOUD/repos/' + \
             'qemu/commits/' + h.commit_hash
         col = colors[h.comp.name.lower()]
-        return f'<a href="{href}" style="color: {col}">{h.commit_hash}</a>'
+        ret = f'<a href="{href}" style="color: {col}">{h.commit_hash}</a>'
+        if h.in_tag:
+            ret += self.view_span(Span(f' (in {h.in_tag})', 'in-tag'))
+        return ret
 
     def view_span(self, s: Span) -> str:
         col = colors[s.klass]
         return f'<span style="color: {col}">{s.text}</span>'
 
-    def view_converted_table(self, tab) -> str:
+    def view_converted_table(self, tab: ConvertedTable) -> str:
         return '<table>' + \
             '\n'.join('<tr>' + ''.join(f'<td>{x}</td>' for x in row) + '</tr>'
                       for row in tab) + '</table>'
```

### Comparing `git-check-rebase-0.3/git_check_rebase/parse_jira.py` & `git-check-rebase-0.4/git_check_rebase/parse_issues.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-import jira  # type: ignore
+from typing import Any, List, Dict, Set
 
-from jira.utils import json_loads  # type: ignore
 
-
-def parse_issue(j, key, commits, result):
-    issue = j.issue(key, fields='description,subtasks,priority,resolution,'
-                    'issuetype')
-
-    if issue.fields.issuetype.name == 'Epic':
-        url = j.server_url + f'/rest/agile/1.0/epic/{key}/issue'
-        # pylint: disable=protected-access
-        issues_in_epic = json_loads(j._session.get(url))['issues']
-        for iss in issues_in_epic:
-            parse_issue(j, iss['key'], commits, result)
+def parse_issue(issue: Any, commits: List[str],
+                result: Dict[str, List[Any]],
+                parsed_keys: Set[str]) -> None:
+    """Update @result: dict {commit => [list of matching issues]}"""
+    if issue.key in parsed_keys:
         return
+    parsed_keys.add(issue.key)
 
-    if issue.fields.description:
-        for line in issue.fields.description.split('\n'):
+    if issue.description:
+        for line in issue.description.split('\n'):
             line = line.strip()
             for commit in commits:
                 if line.endswith(commit):
                     if commit in result:
-                        result[commit][key] = issue
+                        result[commit].append(issue)
                     else:
-                        result[commit] = {key: issue}
+                        result[commit] = [issue]
 
-    for sub in issue.fields.subtasks:
-        parse_issue(j, sub.key, commits, result)
+    for sub in issue.get_subissues():
+        parse_issue(sub, commits, result, parsed_keys)
 
 
-def parse_jira(server, login, password, issues, commits):
-    """ Recursively search issues for commits mentioned in description
+def parse_issues(tracker: Any, issues: List[str],
+                 commits: List[str]) -> Dict[str, List[Any]]:
+    """Recursively search issues for commits mentioned in description
 
     Search issues (and their subtasks) for description lines, ends with commit
     subjects from commits list
 
     Returns dict {commit => [list of matching issues]}
     """
-    j = jira.JIRA(options={'server': server}, basic_auth=(login, password))
-
-    result = {}
+    result: Dict[str, List[str]] = {}
+    parsed_keys: Set[str] = set()
 
     for issue in issues:
-        parse_issue(j, issue, commits, result)
+        parse_issue(tracker.get_issue(issue), commits, result, parsed_keys)
 
-    return {k: v.values() for k, v in result.items()}
+    return result
```

### Comparing `git-check-rebase-0.3/git_check_rebase/simple_git.py` & `git-check-rebase-0.4/git_check_rebase/simple_git.py`

 * *Files identical despite different names*

### Comparing `git-check-rebase-0.3/git_check_rebase/span.py` & `git-check-rebase-0.4/git_check_rebase/span.py`

 * *Files identical despite different names*

### Comparing `git-check-rebase-0.3/git_check_rebase/text_table_view.py` & `git-check-rebase-0.4/git_check_rebase/text_table_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-from .compare_ranges import GitHashCell, Table, RowsHideLevel
-import tabulate
-from .viewable import Viewer, Span, GitHashCell
+import tabulate  # type: ignore
+
+from .viewable import Viewer, Span, GitHashCell, ConvertedTable
 
 tabulate.PRESERVE_WHITESPACE = True
 
 colors = {
     'bug-critical': 'red',
     'bug-fixed': 'green',
     'matching': 'green',
     'bug': 'cyan',
     'unknown': 'red',
     'equal': 'green',
     'base': 'green',
     'checked': 'yellow',
+    'in-tag': 'yellow',
     'drop': 'magenta',
     'none': None,
     None: None
 }
 
+
 class TextViewer(Viewer):
     list_splitter = '\n'
 
     def __init__(self, color: bool = False) -> None:
         if color:
             from termcolor import colored
             self.styled = lambda text, style: colored(text, colors[style])
         else:
             self.styled = lambda text, style: text
 
     def view_git_hash(self, h: GitHashCell) -> str:
-        return self.styled(h.commit_hash, h.comp.name.lower())
+        ret = self.styled(h.commit_hash, h.comp.name.lower())
+        if h.in_tag:
+            ret += self.styled(f' (in {h.in_tag})', 'in-tag')
+        return ret
 
     def view_span(self, s: Span) -> str:
         return self.styled(s.text, s.klass)
 
-    def view_converted_table(self, tab) -> str:
+    def view_converted_table(self, tab: ConvertedTable) -> str:
         return tabulate.tabulate(tab, tablefmt='plain')
```

### Comparing `git-check-rebase-0.3/git_check_rebase/viewable.py` & `git-check-rebase-0.4/git_check_rebase/viewable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,91 @@
 from enum import Enum
 from dataclasses import dataclass
-from typing import List, Optional, Any, Union, Tuple, Dict
+from typing import List, Any, Union
 
 
 @dataclass
 class Span:
     text: str
     klass: str
 
     def __str__(self):
         return self.text
 
 
-@dataclass
-class Issue:
-    key: str
-    critical: bool
-    fixed: bool
-
-
 class CompRes(Enum):
     NONE = 1
     BASE = 2  # Some other cells are equal to this one
     EQUAL = 3  # Equal to base, auto-checked
     CHECKED = 4  # Equal to base, checked by hand
 
 
 @dataclass
 class GitHashCell:
     """Representation of one cell with commit hash"""
     commit_hash: str
     comp: CompRes = CompRes.NONE
+    in_tag: str = ''
+
 
-Viewable = Union[None, str, Span, Issue, GitHashCell]
-VTableCell = Union[Viewable, List[Viewable]]
+Viewable = Union[None, str, Span, GitHashCell]
+VTableCell = Union[str, Viewable, List[Viewable]]
 VTableRow = List[VTableCell]
 VTable = List[VTableRow]
+ConvertedTable = List[List[str]]
 
 
 class Viewer:
     list_splitter = ''
 
     def view_git_hash(self, h: GitHashCell) -> str:
-        return h.commit_hash
+        ret = h.commit_hash
+        if h.in_tag:
+            ret += f' (in {h.in_tag})'
+        return ret
+
+    def view_span(self, s: Span) -> str:
+        return s.text
+
+    def view_converted_table(self, tab: ConvertedTable) -> str:
+        raise NotImplementedError
 
     def view_element(self, el: Viewable) -> str:
         if type(el) == GitHashCell:
             return self.view_git_hash(el)
 
         if type(el) == Span:
             return self.view_span(el)
 
+        if hasattr(el, 'is_critical'):
+            return self.view_issue(el)
+
         if el is None:
             return ''
 
         return str(el)
 
-    def convert_table(self, tab):
-        out = []
+    def convert_table(self, tab: VTable) -> ConvertedTable:
+        out: ConvertedTable = []
         for row in tab:
             out.append([])
             for i, cell in enumerate(row):
                 if isinstance(cell, list):
                     out[-1].append(
                         self.list_splitter.join(self.view_element(el)
                                                 for el in cell))
                 else:
                     out[-1].append(self.view_element(cell))
         return out
 
-    def view_table(self, tab):
+    def view_table(self, tab: VTable) -> str:
         out = self.convert_table(tab)
         return self.view_converted_table(out)
+
+    def view_issue(self, issue: Any) -> str:
+        if issue.is_fixed():
+            klass = 'bug-fixed'
+        elif issue.is_critical():
+            klass = 'bug-critical'
+        else:
+            klass = 'bug'
+        return self.view_span(Span(issue.key, klass))
```

### Comparing `git-check-rebase-0.3/git_check_rebase.egg-info/PKG-INFO` & `git-check-rebase-0.4/git_check_rebase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: git-check-rebase
-Version: 0.3
+Version: 0.4
 Summary: Some useful scripts to operate track history and patch changes during rebases.
 Home-page: https://gitlab.com/vsementsov/git-check-rebase
 Author: Vladimir Sementsov-Ogievskiy
 Author-email: vsementsov@yandex-team.ru
 License: MIT
+Project-URL: Docs, https://git-check-rebase.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst
 
 git check-rebase
 ================
 
 Installation
 ------------
@@ -44,8 +45,8 @@
 - Check backported series
 - Check status of rebasing a downstream branch to a new upstream release
 - Check upstreaming status of commits in downstream branch
 
 Documentation
 -------------
 
-Full documentation is `here <https://git-check-rebase.readthedocs.io/en/upd/>`_
+Full documentation is `here <https://git-check-rebase.readthedocs.io/en/latest/>`_
```

### Comparing `git-check-rebase-0.3/git_check_rebase.egg-info/SOURCES.txt` & `git-check-rebase-0.4/git_check_rebase.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-LICENSE
 README.rst
 git-check-rebase
 setup.py
 git_check_rebase/__init__.py
 git_check_rebase/check_rebase_meta.py
 git_check_rebase/compare_commits.py
 git_check_rebase/compare_ranges.py
+git_check_rebase/gcr_jira.py
 git_check_rebase/html_table_view.py
-git_check_rebase/parse_jira.py
+git_check_rebase/parse_issues.py
 git_check_rebase/simple_git.py
 git_check_rebase/span.py
 git_check_rebase/text_table_view.py
 git_check_rebase/viewable.py
 git_check_rebase.egg-info/PKG-INFO
 git_check_rebase.egg-info/SOURCES.txt
 git_check_rebase.egg-info/dependency_links.txt
```

