# Comparing `tmp/agentops-0.1.5.tar.gz` & `tmp/agentops-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.5.tar", last modified: Sat Apr 20 01:56:18 2024, max compression
+gzip compressed data, was "agentops-0.1.6.tar", last modified: Sat Apr 20 03:48:53 2024, max compression
```

## Comparing `agentops-0.1.5.tar` & `agentops-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 01:56:14.000000 agentops-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-20 01:56:18.529813 agentops-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-20 01:56:14.000000 agentops-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.525813 agentops-0.1.5/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-20 01:56:14.000000 agentops-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:56:18.529813 agentops-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.968020 agentops-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 03:48:49.000000 agentops-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-20 03:48:53.968020 agentops-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-20 03:48:49.000000 agentops-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3373 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-20 03:48:49.000000 agentops-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:48:53.968020 agentops-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_teardown.py
```

### Comparing `agentops-0.1.5/LICENSE` & `agentops-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/PKG-INFO` & `agentops-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
-AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
+You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
 <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
@@ -67,24 +67,24 @@
 ### Session replays in 3 lines of code
 Initialize the AgentOps client, and automatically get analytics on every LLM call.
 
 ```python python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
-ao_client = agentops.Client(<INSERT YOUR API KEY HERE>)
+agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
-@record_function('sample function being record')
+@agentops.record_function('sample function being record')
 def sample_function(...):
     ...
 
 # End of program
-ao_client.end_session('Success')
+agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
 ## Time travel debugging 🔮
 (coming soon!)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.6 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
@@ -15,28 +15,27 @@
                                     [Logo]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps Build your next agent with benchmarks, observability, and replay
 analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
-(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
-(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+reliable AI agents. You can sign up for AgentOps [here](https://
+app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
+img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
-_#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_o___c_l_i_e_n_t_._e_n_d___s_e_s_s_i_o_n
+_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
+_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
+_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
 _(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
 _(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
 _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
 _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
 _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
 _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
 _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
```

### Comparing `agentops-0.1.5/README.md` & `agentops-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
-AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
+You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
 <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
@@ -45,24 +45,24 @@
 ### Session replays in 3 lines of code
 Initialize the AgentOps client, and automatically get analytics on every LLM call.
 
 ```python python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
-ao_client = agentops.Client(<INSERT YOUR API KEY HERE>)
+agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
-@record_function('sample function being record')
+@agentops.record_function('sample function being record')
 def sample_function(...):
     ...
 
 # End of program
-ao_client.end_session('Success')
+agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
 ## Time travel debugging 🔮
 (coming soon!)
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
                                     [Logo]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps Build your next agent with benchmarks, observability, and replay
 analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
-(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
-(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+reliable AI agents. You can sign up for AgentOps [here](https://
+app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
+img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
-_#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_o___c_l_i_e_n_t_._e_n_d___s_e_s_s_i_o_n
+_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
+_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
+_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
 _(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
 _(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
 _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
 _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
 _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
 _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
 _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
```

### Comparing `agentops-0.1.5/agentops/__init__.py` & `agentops-0.1.6/agentops/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from .client import Client
 from .config import Configuration
 from .event import Event, ActionEvent, LLMEvent, ToolEvent, ErrorEvent
 from .enums import Models
 from .decorators import record_function
 from .agent import track_agent
+from .log_config import set_logging_level_info, set_logging_level_critial
 
 
 def init(api_key: Optional[str] = None,
          parent_key: Optional[str] = None,
          endpoint: Optional[str] = None,
          max_wait_time: Optional[int] = None,
          max_queue_size: Optional[int] = None,
@@ -37,26 +38,26 @@
             tags (List[str], optional): Tags for the sessions that can be used for grouping or
                 sorting later (e.g. ["GPT-4"]).
             override (bool): Whether to override and LLM calls to emit as events.
             auto_start_session (bool): Whether to start a session automatically when the client is created.
             inherited_session_id (optional, str): Init Agentops with an existing Session
         Attributes:
         """
-
+    set_logging_level_info()
     c = Client(api_key=api_key,
                parent_key=parent_key,
                endpoint=endpoint,
                max_wait_time=max_wait_time,
                max_queue_size=max_queue_size,
                tags=tags,
                override=override,
                auto_start_session=auto_start_session,
                inherited_session_id=inherited_session_id
                )
-
+    
     return inherited_session_id or c.current_session_id
 
 
 def end_session(end_state: str,
                 end_state_reason: Optional[str] = None,
                 video: Optional[str] = None):
     Client().end_session(end_state, end_state_reason, video)
```

### Comparing `agentops-0.1.5/agentops/agent.py` & `agentops-0.1.6/agentops/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging
+from .log_config import logger
 from uuid import uuid4
 from agentops import Client
 from inspect import isclass, isfunction
 
 
 def track_agent(name: str | None = None):
     def decorator(obj):
@@ -14,15 +14,15 @@
 
             def new_init(self, *args, **kwargs):
                 try:
                     original_init(self, *args, **kwargs)
                     self.agent_ops_agent_id = uuid4()
                     Client().create_agent(self.agent_ops_agent_id, self.agent_ops_agent_name)
                 except AttributeError as e:
-                    logging.error("AgentOps failed to track an agent. This often happens if agentops.init() was not "
+                    logger.warning("AgentOps failed to track an agent. This often happens if agentops.init() was not "
                                   "called before initializing an agent with the @track_agent decorator.")
                     raise e
 
             obj.__init__ = new_init
 
         elif isfunction(obj):
             obj.agent_ops_agent_id = uuid4()
```

### Comparing `agentops-0.1.5/agentops/client.py` & `agentops-0.1.6/agentops/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .helpers import get_ISO_time, singleton, check_call_stack_for_agent_id
 from .session import Session
 from .worker import Worker
 from .host_env import get_host_env
 from uuid import uuid4
 from typing import Optional, List
 import traceback
-import logging
+from .log_config import logger, set_logging_level_info
 import inspect
 import atexit
 import signal
 import sys
 import threading
 
 from .meta_client import MetaClient
@@ -111,15 +111,15 @@
         Args:
             event (Event): The event to record.
         """
 
         if self._session is not None and not self._session.has_ended:
             self._worker.add_event(event.__dict__)
         else:
-            logging.warning(
+            logger.warning(
                 "🖇 AgentOps: Cannot record event - no current session")
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
         # Get default values
@@ -202,28 +202,30 @@
 
         Args:
             tags (List[str], optional): Tags that can be used for grouping or sorting later.
                 e.g. ["test_run"].
             config: (Configuration, optional): Client configuration object
             inherited_session_id (optional, str): assign session id to match existing Session
         """
+        set_logging_level_info()
+        
         if self._session is not None:
-            return logging.warning("🖇 AgentOps: Cannot start session - session already started")
+            return logger.warning("🖇 AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
-            return logging.warning("🖇 AgentOps: Cannot start session - missing configuration")
+            return logger.warning("🖇 AgentOps: Cannot start session - missing configuration")
 
         self._session = Session(inherited_session_id or uuid4(), tags or self._tags, host_env=get_host_env())
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
-            return logging.warning("🖇 AgentOps: Cannot start session")
+            return logger.warning("🖇 AgentOps: Cannot start session")
 
-        logging.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
+        logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
                      .format(self._session.session_id))
 
         return self._session.session_id
 
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
@@ -233,18 +235,18 @@
 
         Args:
             end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
             end_state_reason (str, optional): The reason for ending the session.
             video (str, optional): The video screen recording of the session
         """
         if self._session is None or self._session.has_ended:
-            return logging.warning("🖇 AgentOps: Cannot end session - no current session")
+            return logger.warning("🖇 AgentOps: Cannot end session - no current session")
 
         if not any(end_state == state.value for state in EndState):
-            return logging.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
+            return logger.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         token_cost = self._worker.end_session(self._session)
         if token_cost == 'unknown':
             print('🖇 AgentOps: Could not determine cost of run.')
         else:
@@ -268,15 +270,15 @@
             Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
 
             Args:
                 signum (int): The signal number.
                 frame: The current stack frame.
             """
             signal_name = 'SIGINT' if signum == signal.SIGINT else 'SIGTERM'
-            logging.info(
+            logger.info(
                 f'🖇 AgentOps: {signal_name} detected. Ending session...')
             self.end_session(end_state='Fail',
                              end_state_reason=f'Signal {signal_name} detected')
             sys.exit(0)
 
         def handle_exception(exc_type, exc_value, exc_traceback):
             """
```

### Comparing `agentops-0.1.5/agentops/config.py` & `agentops-0.1.6/agentops/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Classes:
     Configuration: Stores the configuration settings for AgentOps clients.
 """
 
 from typing import Optional
 from os import environ
-import logging
+from .log_config import logger
 
 
 class Configuration:
     """
     Stores the configuration settings for AgentOps clients.
 
     Args:
@@ -139,8 +139,8 @@
 
 
 class ConfigurationError(Exception):
     """Exception raised for errors related to Configuration"""
 
     def __init__(self, message: str):
         super().__init__(message)
-        logging.warning(message)
+        logger.warning(message)
```

### Comparing `agentops-0.1.5/agentops/decorators.py` & `agentops-0.1.6/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/enums.py` & `agentops-0.1.6/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/event.py` & `agentops-0.1.6/agentops/event.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/helpers.py` & `agentops-0.1.6/agentops/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pprint import pprint, pformat
 from functools import wraps
 import time
 from datetime import datetime
 import json
 import inspect
-import logging
+from .log_config import logger
 from uuid import UUID
 import os
 from importlib.metadata import version
 
 
 def singleton(class_):
     instances = {}
@@ -81,25 +81,25 @@
         # Look through the call stack for the class that called the LLM
         local_vars = frame_info.frame.f_locals
         for var in local_vars.values():
             # We stop looking up the stack at main because after that we see global variables
             if var == "__main__":
                 return
             if hasattr(var, 'agent_ops_agent_id') and getattr(var, 'agent_ops_agent_id'):
-                logging.debug('LLM call from agent named: ' + getattr(var, 'agent_ops_agent_name'))
+                logger.debug('LLM call from agent named: ' + getattr(var, 'agent_ops_agent_name'))
                 return getattr(var, 'agent_ops_agent_id')
     return None
 
 
 def get_agentops_version():
     try:
         pkg_version = version("agentops")
         return pkg_version
     except Exception as e:
-        logging.warning(f"Error reading package version: {e}")
+        logger.warning(f"Error reading package version: {e}")
         return None
 
 
 # Function decorator that prints function name and its arguments to the console for debug purposes
 # Example output:
     # <AGENTOPS_DEBUG_OUTPUT>
     # on_llm_start called with arguments:
```

### Comparing `agentops-0.1.5/agentops/host_env.py` & `agentops-0.1.6/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/http_client.py` & `agentops-0.1.6/agentops/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from typing import Optional
-import logging
+from .log_config import logger
 import requests
 from requests.adapters import Retry, HTTPAdapter
 
 JSON_HEADER = {
     "Content-Type": "application/json; charset=UTF-8",
     "Accept": "*/*"
 }
@@ -78,30 +78,30 @@
             res = request_session.post(url, data=payload,
                                        headers=JSON_HEADER, timeout=20)
 
             result.parse(res)
         except requests.exceptions.Timeout:
             result.code = 408
             result.status = HttpStatus.TIMEOUT
-            logging.warning(
+            logger.warning(
                 '🖇 AgentOps: Could not post data - connection timed out')
         except requests.exceptions.HTTPError as e:
             try:
                 result.parse(e.response)
             except:
                 result = Response()
                 result.code = e.response.status_code
                 result.status = Response.get_status(e.response.status_code)
                 result.body = {'error': str(e)}
         except requests.exceptions.RequestException as e:
             result.body = {'error': str(e)}
 
         if result.code == 401:
-            logging.warning(
+            logger.warning(
                 f'🖇 AgentOps: Could not post data - API server rejected your API key: {api_key}')
         if result.code == 400:
-            logging.warning(f'🖇 AgentOps: Could not post data - {result.body}')
+            logger.warning(f'🖇 AgentOps: Could not post data - {result.body}')
         if result.code == 500:
-            logging.warning(
+            logger.warning(
                 f'🖇 AgentOps: Could not post data - internal server error')
 
         return result
```

### Comparing `agentops-0.1.5/agentops/langchain_callback_handler.py` & `agentops-0.1.6/agentops/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/llm_tracker.py` & `agentops-0.1.6/agentops/llm_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import sys
 from importlib import import_module
 from packaging.version import parse
-import logging
+from .log_config import logger
 from .event import LLMEvent, ErrorEvent
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 import inspect
 
 
 class LlmTracker:
     SUPPORTED_APIS = {
@@ -55,16 +55,16 @@
                     self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-                # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
-                logging.warning(
+                # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+                logger.warning(
                     f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if inspect.isasyncgen(response):
             async def async_generator():
                 async for chunk in response:
                     handle_stream_chunk(chunk)
@@ -94,16 +94,16 @@
             self.llm_event.returns = {"content": response['choices'][0]['message']['content']}
             self.llm_event.model = response["model"]
             self.llm_event.end_timestamp = get_ISO_time()
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-            # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
-            logging.warning(
+            # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+            logger.warning(
                 f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def _handle_response_v1_openai(self, response, kwargs, init_timestamp):
         """Handle responses for OpenAI versions >v1.0.0"""
         from openai import Stream, AsyncStream
@@ -140,16 +140,16 @@
                                               "function_call": function_call, "tool_calls": tool_calls, "role": role}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-                # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
-                logging.warning(
+                # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+                logger.warning(
                     f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if isinstance(response, Stream):
             def generator():
                 for chunk in response:
                     handle_stream_chunk(chunk)
@@ -185,16 +185,16 @@
             self.llm_event.completion_tokens = response.usage.completion_tokens
             self.llm_event.returns = response.model_dump()
             self.llm_event.model = response.model
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-            # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
-            logging.warning(
+            # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+            logger.warning(
                 f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def override_openai_v1_completion(self):
         from openai.resources.chat import completions
```

### Comparing `agentops-0.1.5/agentops/meta_client.py` & `agentops-0.1.6/agentops/meta_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging
+from .log_config import logger
 import traceback
 
 from .host_env import get_host_env
 from .http_client import HttpClient
 from .helpers import safe_serialize, get_agentops_version
 
 from os import environ
@@ -41,14 +41,14 @@
 def handle_exceptions(method):
     """Decorator within the metaclass to wrap method execution in try-except block."""
 
     def wrapper(self, *args, **kwargs):
         try:
             return method(self, *args, **kwargs)
         except Exception as e:
-            logging.warning(f"🖇 AgentOps: Error: {e}")
+            logger.warning(f"🖇 AgentOps: Error: {e}")
             config = getattr(self, 'config', None)
             if config is not None:
                 type(self).send_exception_to_server(e, self.config._api_key)
             raise e
 
     return wrapper
```

### Comparing `agentops-0.1.5/agentops/session.py` & `agentops-0.1.6/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops/worker.py` & `agentops-0.1.6/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/agentops.egg-info/PKG-INFO` & `agentops-0.1.6/agentops.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
-AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
+You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
 <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
@@ -67,24 +67,24 @@
 ### Session replays in 3 lines of code
 Initialize the AgentOps client, and automatically get analytics on every LLM call.
 
 ```python python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
-ao_client = agentops.Client(<INSERT YOUR API KEY HERE>)
+agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
-@record_function('sample function being record')
+@agentops.record_function('sample function being record')
 def sample_function(...):
     ...
 
 # End of program
-ao_client.end_session('Success')
+agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
 ## Time travel debugging 🔮
 (coming soon!)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.6 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
@@ -15,28 +15,27 @@
                                     [Logo]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps Build your next agent with benchmarks, observability, and replay
 analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
-(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
-(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+reliable AI agents. You can sign up for AgentOps [here](https://
+app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
+img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
-_#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_o___c_l_i_e_n_t_._e_n_d___s_e_s_s_i_o_n
+_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
+_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
+_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
 _(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
 _(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
 _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
 _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
 _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
 _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
 _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
```

### Comparing `agentops-0.1.5/agentops.egg-info/SOURCES.txt` & `agentops-0.1.6/agentops.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 agentops/enums.py
 agentops/event.py
 agentops/helpers.py
 agentops/host_env.py
 agentops/http_client.py
 agentops/langchain_callback_handler.py
 agentops/llm_tracker.py
+agentops/log_config.py
 agentops/meta_client.py
 agentops/session.py
 agentops/worker.py
 agentops.egg-info/PKG-INFO
 agentops.egg-info/SOURCES.txt
 agentops.egg-info/dependency_links.txt
 agentops.egg-info/requires.txt
```

### Comparing `agentops-0.1.5/pyproject.toml` & `agentops-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
```

### Comparing `agentops-0.1.5/tests/test_canary.py` & `agentops-0.1.6/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/tests/test_patcher.py` & `agentops-0.1.6/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/tests/test_record_function.py` & `agentops-0.1.6/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/tests/test_session.py` & `agentops-0.1.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.5/tests/test_teardown.py` & `agentops-0.1.6/tests/test_teardown.py`

 * *Files identical despite different names*

