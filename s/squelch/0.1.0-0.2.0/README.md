# Comparing `tmp/squelch-0.1.0.tar.gz` & `tmp/squelch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squelch-0.1.0.tar", max compression
+gzip compressed data, was "squelch-0.2.0.tar", max compression
```

## Comparing `squelch-0.1.0.tar` & `squelch-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.1.0/LICENSE
--rw-r--r--   0        0        0      442 2024-04-15 13:11:18.877847 squelch-0.1.0/README.md
--rw-r--r--   0        0        0      541 2024-04-16 08:57:15.899053 squelch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11392 2024-04-17 14:40:44.136032 squelch-0.1.0/squelch/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-15 12:20:52.730110 squelch-0.1.0/squelch/__main__.py
--rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 squelch-0.1.0/setup.py
--rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 squelch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2607 2024-04-17 18:59:58.698301 squelch-0.2.0/README.md
+-rw-r--r--   0        0        0      721 2024-04-20 10:42:03.743440 squelch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19166 2024-04-20 10:42:31.867731 squelch-0.2.0/squelch/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-15 12:20:52.730110 squelch-0.2.0/squelch/__main__.py
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 squelch-0.2.0/setup.py
+-rw-r--r--   0        0        0     3435 1970-01-01 00:00:00.000000 squelch-0.2.0/PKG-INFO
```

### Comparing `squelch-0.1.0/LICENSE` & `squelch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squelch-0.1.0/squelch/__init__.py` & `squelch-0.2.0/squelch/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 
 import sys
 import logging
 from pathlib import Path
 import atexit
 import traceback
 import re
@@ -16,20 +16,21 @@
 from tabulate import tabulate
 
 PROGNAME = __name__
 
 DEF_CONF_FILE = './squelch.json'
 DEF_HISTORY_FILE = Path('~/.squelch_history').expanduser()
 DEF_CONF = {}
-DEF_STATE = {'pager': True}
+DEF_STATE = {'pager': True, 'footer': True, 'AUTOCOMMIT': True}
+DEF_MIN_FOOTER = '\n'             # Blank line to separate table from prompt
 
 URL_CRED_PATTERN = r'://(.+)@'
 URL_CRED_REPLACE = r'://***@'
 
-SQL_COMPLETIONS = ['select', 'insert', 'update', 'delete', 'create', 'drop', 'from', 'where', 'and', 'or', 'not', 'like', 'order by', 'group by', 'into', 'values']
+SQL_COMPLETIONS = ['select', 'insert', 'update', 'delete', 'create', 'drop', 'from', 'where', 'and', 'or', 'not', 'like', 'order by', 'group by', 'into', 'values','begin', 'transaction', 'commit', 'rollback']
 
 logger = logging.getLogger(__name__)
 
 class Squelch(object):
     """
     Class providing a Simple SQL REPL Command Handler
     """
@@ -37,20 +38,22 @@
     DEFAULTS = {
         'conf_file': DEF_CONF_FILE,
         'history_file': DEF_HISTORY_FILE,
         'query_quoted_string_pattern': r"'[^']+'",
         'query_params_pattern': r':([a-z0-9_.]+)',
         'repl_commands': {
             'quit': [r'\q'],
-            'state': [r'\set', r'\pset']
+            'state': [r'\set', r'\pset'],
+            'help': [r'help', r'\?'],
+            'dist': [r'\copyright']
         },
         'table_opts': {
             # Unfortunately, tabulate doesn't recognise a sqlalchemy result
             # as having keys(), so we can't set 'headers': 'keys' here
-            'tablefmt': 'presto', 'showindex': False
+            'tablefmt': 'presto', 'showindex': False, 'disable_numparse': True
         }
     }
  
     def __init__(self, conf=DEF_CONF, state=DEF_STATE):
         """
         Constructor
 
@@ -133,21 +136,139 @@
         """
         Set the progam's runtime state according to the given command
 
         The state variable in self.state is updated according to command
 
         :param cmd: The command to update the program's state
         :type cmd: str
+        :returns: Text of the state update with which to notify the user
+        :rtype: str
         """
 
-        if cmd.lower() == r'\pset pager off':
-            self.state['pager'] = False
-        elif cmd.lower() == r'\pset pager on':
-            self.state['pager'] = True
- 
+        state_text = ''
+        falsy = r'(off|false|0|no)'
+        truthy = r'(on|true|1|yes)'
+
+        if cmd.lower().startswith(r'\pset pager'):
+            if re.match(fr'\\pset pager {falsy}', cmd.lower()):
+                self.state['pager'] = False
+                state_text = 'Pager usage is off.'
+            elif re.match(fr'\\pset pager {truthy}', cmd.lower()):
+                self.state['pager'] = True
+                state_text = 'Pager usage is on.'
+        elif cmd.lower().startswith(r'\pset footer'):
+            if re.match(fr'\\pset footer {falsy}', cmd.lower()):
+                self.state['footer'] = False
+            elif re.match(fr'\\pset footer {truthy}', cmd.lower()):
+                self.state['footer'] = True
+        elif cmd.lower().startswith(r'\set AUTOCOMMIT'):
+            if re.match(fr'\\set AUTOCOMMIT {falsy}', cmd.lower()):
+                self.state['AUTOCOMMIT'] = False
+            elif re.match(fr'\\set AUTOCOMMIT {truthy}', cmd.lower()):
+                self.state['AUTOCOMMIT'] = True
+
+        return state_text
+
+    def get_welcome_text(self):
+        """
+        Get the welcome text
+
+        * Shows program information
+        * Signposts the user how to get help
+
+        :returns: The welcome text
+        :rtype: str
+        """
+
+        text = fr"""{PROGNAME} ({__version__})
+Type "help" for help.
+"""
+
+        return text
+
+    def get_help_summary_text(self):
+        """
+        Get the help summary text
+
+        Tells the user how to get:
+
+        * Distribution terms
+        * Help with the REPL commands
+        * How to quit
+
+        :returns: The help summary text
+        :rtype: str
+        """
+
+        text = fr"""You are using {PROGNAME}, a CLI to SQLAlchemy-supported database engines.
+Type:  \copyright for distribution terms
+       \? for help with {PROGNAME} commands
+       \q to quit"""
+
+        return text
+
+    def get_help_repl_cmd_text(self):
+        """
+        Get the REPL command help text
+
+        :returns: The REPL command help text
+        :rtype: str
+        """
+
+        text = fr"""General
+  \copyright             show {PROGNAME} usage and distribution terms
+  \q                     quit {PROGNAME}
+
+Help
+  \?                     show help on backslash commands
+
+Formatting
+  \pset [NAME [VALUE]]   set table output option
+                         (pager)
+
+Variables
+  \set [NAME [VALUE]]    set internal variable, or list all if no parameters
+"""
+
+        return text
+
+    def get_help(self, cmd):
+        r"""
+        Get the progam's help text according to the given command
+
+        * help: Get the help summary text
+        * \?: Get the REPL command text
+
+        :param cmd: The help command
+        :type cmd: str
+        :returns: The help text corresponding to the given command
+        :rtype: str
+        """
+
+        text = ''
+
+        if cmd.lower() == r'help':
+            text = self.get_help_summary_text()
+        elif cmd.lower() == r'\?':
+            text = self.get_help_repl_cmd_text()
+
+        return text
+
+    def get_dist_terms_text(self):
+        """
+        Get the program's distribution terms text
+
+        :returns: The program's distribution terms text
+        :rtype: str
+        """
+
+        text = f"""{PROGNAME} ({__version__}) distributed under Apache-2.0 license: https://spdx.org/licenses/Apache-2.0.html"""
+
+        return text
+
     def connect(self, url):
         """
         Connect to the database in the given connection URL
 
         :param url: The database connection URL
         :type url: str
         :returns: The database connection object
@@ -160,62 +281,143 @@
 
         return self.conn
 
     def exec_query(self, query, params):
         """
         Execute the given query and bind any given query parameters
 
-        The query is executed in a database transaction and the query
-        result set is stored in self.result
+        * The query result set is stored in self.result.
+        * If AUTOCOMMIT is on, the query is executed in a DB transaction
+          and automatically committed on successful execution.
 
         :param query: The query to execute
         :type query: sqlalchemy.sql.text
         :param params: Optional query parameters to bind in the query
         :type params: dict
         :returns: The query result set
         :rtype: sqlalchemy.engine.CursorResult
         """
 
         self.result = None
 
-        with self.conn.begin() as trans:
-            try:
-                self.result = self.conn.execute(query, params)
-            except DatabaseError as e:
-                if logger.isEnabledFor(logging.DEBUG):
-                    traceback.print_exc(chain=False)
-                else:
-                    print(e, file=sys.stderr)
+        try:
+            self.result = self.conn.execute(query, params)
+            self.state.get('AUTOCOMMIT') and self.conn.commit()
+        except DatabaseError as e:
+            if logger.isEnabledFor(logging.DEBUG):
+                traceback.print_exc(chain=False)
+            else:
+                print(e, file=sys.stderr)
 
         return self.result
 
+    def get_result_table_footer(self, table, table_opts):
+        """
+        Get the result table footer
+
+        The footer shows the row count of the table data
+
+        * Access to the row count is dependent on the DB engine supporting
+          this.  It should be supported for UPDATE and DELETE, but may not
+          be supported for INSERT or SELECT.
+        * If row count isn't supported by the DB engine, then a fallback is
+          to employ a heuristic to calculate the number of rows based on the
+          number of newlines found in the table.  Whilst this works for the
+          default `tablefmt` table option, it won't work for `tablefmt`
+          styles that have more or less table grid lines.
+
+        :param table: The result table text
+        :type table: str
+        :param table_opts: Options for rendering the tabulated result output
+        :type table_opts: dict
+        :returns: The result table footer text
+        :rtype: str
+        """
+
+        footer = DEF_MIN_FOOTER
+
+        if self.result.supports_sane_rowcount and self.result.rowcount != -1:
+            logger.debug(f"row count available in the result cursor")
+            nrows = self.result.rowcount
+        else:
+            try:
+                if table_opts['tablefmt'] == self.DEFAULTS['table_opts']['tablefmt']:
+                    logger.debug(f"row count calculated from lines in the table")
+                    nrows = table.count('\n') - 1
+            except KeyError:
+                nrows = -1
+
+        if nrows != -1:
+            row_text = 'row' if nrows == 1 else 'rows'
+            footer = f'\n({nrows} {row_text})\n'
+        else:
+            logger.debug(f"row count not available")
+
+        return footer
+
+    def get_command_response(self):
+        """
+        Get the non-query command response
+
+        The response shows the command name and the affected row count
+
+        * Access to the row count is dependent on the DB engine supporting
+          this.  It should be supported for UPDATE and DELETE, but may not
+          be supported for INSERT or SELECT.
+
+        :returns: The command response text
+        :rtype: str
+        """
+
+        response = ''
+
+        if self.query.text:
+            response = self.query.text.split()[0].upper()
+
+        if self.result.supports_sane_rowcount and self.result.rowcount != -1:
+            logger.debug(f"row count available in the result cursor")
+            response = f'{response} {self.result.rowcount}'
+
+        return response
+
     def present_result(self, table_opts=None):
         """
         Present the result set of the latest executed query
 
         The query result set in self.result is presented as a table
 
         * If the state variable 'pager' is True, the output is paged using the
           system pager, otherwise the whole table is printed to the output
-          stream
+          stream.
+        * If the state variable 'footer' is True, then a footer is appended to
+          the result table.
 
         :param table_opts: Options for rendering the tabulated result output
         :type table_opts: dict
         """
 
         table_opts = table_opts or self.get_conf_item('table_opts')
         logger.debug(f"table_opts: {table_opts}")
 
         if self.result:
-            table = tabulate(self.result, headers=self.result.keys(), **table_opts)
+            if self.result.returns_rows:
+                table = tabulate(self.result, headers=self.result.keys(), **table_opts)
 
-            if self.state['pager']:
-                pydoc.pager(table)
+                if table:
+                    if self.state.get('footer'):
+                        table += self.get_result_table_footer(table, table_opts)
+                    else:
+                        table += DEF_MIN_FOOTER
+
+                    if self.state.get('pager'):
+                        pydoc.pager(table)
+                    else:
+                        print(table)
             else:
-                print(table)
+                print(self.get_command_response())
 
     def prompt_for_query_params(self, raw):
         """
         Prompt for any query parameters
 
         If the raw query contains query parameter placeholders, then the user
         is prompted to provide a value for each parameter.  These parameters
@@ -254,14 +456,54 @@
 
         raw = input(prompt)
         raw = raw.strip().rstrip(terminator)
         logger.debug(f"raw stripped query: '{raw}'")
 
         return raw
 
+    def handle_state_command(self, raw):
+        """
+        Process the given state change command
+
+        :param raw: The raw stripped input (a REPL state command)
+        :type raw: str
+        """
+
+        if len(raw.split()) > 1:
+            state_text = self.set_state(raw)
+
+            if state_text:
+                print(state_text)
+        else:
+            print(self.state)
+
+    def handle_query(self, raw):
+        """
+        Process the given query
+
+        :param raw: The raw stripped input (a query)
+        :type raw: str
+        """
+
+        cmd = raw.split()[0].lower()
+
+        # Disable autocommit during an explicit transaction
+        if cmd == 'begin':
+            self.state['AUTOCOMMIT'] = False
+
+        self.query = text(raw)
+        self.params = self.prompt_for_query_params(raw)
+        self.exec_query(self.query, self.params)
+        self.present_result()
+
+        if cmd == 'rollback':
+            self.state['AUTOCOMMIT'] = True
+        elif cmd == 'commit':
+            self.state['AUTOCOMMIT'] = True
+
     def process_input(self, raw):
         """
         Process the given input
 
         * If the input is a REPL command, then the command is executed
         * If the input is a database query, then the raw query is converted
           to an sqlalchemy.sql.text prepared query and stored in self.query,
@@ -279,20 +521,21 @@
         if raw:
             cmd = raw.split()[0]
 
             if cmd in self.get_conf_item('repl_commands')['quit']:
                 logger.info('quitting')
                 sys.exit(0)
             elif cmd in self.get_conf_item('repl_commands')['state']:
-                self.set_state(raw)
+                self.handle_state_command(raw)
+            elif cmd in self.get_conf_item('repl_commands')['help']:
+                print(self.get_help(raw))
+            elif cmd in self.get_conf_item('repl_commands')['dist']:
+                print(self.get_dist_terms_text())
             else:
-                self.query = text(raw)
-                self.params = self.prompt_for_query_params(raw)
-                self.exec_query(self.query, self.params)
-                self.present_result()
+                self.handle_query(raw)
         else:
             q = input('no input, do you want to quit (yes/no)? ')
 
             if q.lower().startswith('y'):
                 logger.info('no input, so quitting')
                 sys.exit(0)
 
@@ -334,14 +577,16 @@
         logger.info(f"reading history from file {history_file}")
         readline.read_history_file(history_file)
 
         logger.info(f"setting input completions")
         readline.parse_and_bind("tab: complete")
         readline.set_completer(self.input_completions)
 
+        print(self.get_welcome_text())
+
     def complete_repl(self):
         """
         Complete the REPL
 
         The session history is written to the configured history_file
         """
```

### Comparing `squelch-0.1.0/squelch/__main__.py` & `squelch-0.2.0/squelch/__main__.py`

 * *Files identical despite different names*

