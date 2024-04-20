# Comparing `tmp/redco-0.4.8.tar.gz` & `tmp/redco-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.8.tar", last modified: Tue Oct 24 05:14:04 2023, max compression
+gzip compressed data, was "redco-0.4.9.tar", last modified: Sat Nov  4 21:30:27 2023, max compression
```

## Comparing `redco-0.4.8.tar` & `redco-0.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.480000 redco-0.4.8/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.8/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4697 2023-10-24 05:14:04.480000 redco-0.4.8/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4444 2023-10-24 05:09:30.000000 redco-0.4.8/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.460000 redco-0.4.8/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.8/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.470000 redco-0.4.8/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.8/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-06-20 03:18:51.000000 redco-0.4.8/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1196 2023-07-26 05:08:40.000000 redco-0.4.8/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.470000 redco-0.4.8/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.8/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2064 2023-06-22 04:36:30.000000 redco-0.4.8/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     9403 2023-10-15 00:47:06.000000 redco-0.4.8/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2700 2023-07-21 14:47:48.000000 redco-0.4.8/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.470000 redco-0.4.8/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.8/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5669 2023-07-04 02:05:17.000000 redco-0.4.8/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.8/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1683 2023-07-04 04:06:34.000000 redco-0.4.8/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.470000 redco-0.4.8/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.8/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4503 2023-10-24 04:20:53.000000 redco-0.4.8/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1878 2023-07-26 04:43:53.000000 redco-0.4.8/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.480000 redco-0.4.8/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.8/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    13953 2023-10-24 04:20:53.000000 redco-0.4.8/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2096 2023-07-26 18:39:31.000000 redco-0.4.8/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-10-24 05:14:04.470000 redco-0.4.8/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4697 2023-10-24 05:14:03.000000 redco-0.4.8/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-10-24 05:14:04.000000 redco-0.4.8/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-10-24 05:14:04.000000 redco-0.4.8/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-10-24 05:14:04.000000 redco-0.4.8/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-10-24 05:14:04.000000 redco-0.4.8/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-10-24 05:14:04.480000 redco-0.4.8/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-10-24 04:26:17.000000 redco-0.4.8/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.060000 redco-0.4.9/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.9/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4644 2023-11-04 21:30:27.060000 redco-0.4.9/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4444 2023-10-24 20:56:35.000000 redco-0.4.9/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.050000 redco-0.4.9/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.9/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.050000 redco-0.4.9/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.9/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-06-20 03:18:51.000000 redco-0.4.9/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1196 2023-07-26 05:08:40.000000 redco-0.4.9/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.060000 redco-0.4.9/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.9/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2064 2023-06-22 04:36:30.000000 redco-0.4.9/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11668 2023-10-31 04:37:34.000000 redco-0.4.9/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2700 2023-07-21 14:47:48.000000 redco-0.4.9/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.060000 redco-0.4.9/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.9/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5669 2023-07-04 02:05:17.000000 redco-0.4.9/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.9/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1683 2023-07-04 04:06:34.000000 redco-0.4.9/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.060000 redco-0.4.9/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.9/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4503 2023-10-24 04:20:53.000000 redco-0.4.9/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1878 2023-07-26 04:43:53.000000 redco-0.4.9/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.060000 redco-0.4.9/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.9/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    14565 2023-10-30 01:18:45.000000 redco-0.4.9/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2096 2023-07-26 18:39:31.000000 redco-0.4.9/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-11-04 21:30:27.050000 redco-0.4.9/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4644 2023-11-04 21:30:26.000000 redco-0.4.9/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-11-04 21:30:27.000000 redco-0.4.9/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-11-04 21:30:26.000000 redco-0.4.9/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-11-04 21:30:26.000000 redco-0.4.9/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-11-04 21:30:26.000000 redco-0.4.9/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-11-04 21:30:27.060000 redco-0.4.9/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-10-31 03:00:58.000000 redco-0.4.9/setup.py
```

### Comparing `redco-0.4.8/LICENSE` & `redco-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/PKG-INFO` & `redco-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.8
-Summary: UNKNOWN
+Version: 0.4.9
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Redco: A Lightweight Tool to Automate Distributed Training
 
 Redco is a lightweight and user-friendly tool designed to automate distributed training and inference for large models while simplifying the ML pipeline development process without necessitating MLSys expertise from users.
@@ -27,17 +24,17 @@
 * **Automatic model/data parallelism**: No need to concern your large models and large datasets. *Redco* distributes your models and datasets to all your devices automatically. 
 * **No need to know JAX**: *Redco* only needs a couple of numpy-like functions as your pipeline design. 
 
 ### Installation
 
 #### Install Jax
 ```
-pip install --upgrade jax[cuda11_pip]==0.4.16 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade jax[cuda11_pip]==0.4.13 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
-Jax version (`==0.4.16`) can be flexible, as long as it matches your CUDA/CUDNN version.
+Jax version (`==0.4.13`) can be flexible, as long as it matches your CUDA/CUDNN version.
 
 If you are using TPU/CPU/AMD/Apple, see [here](https://github.com/google/jax#installation) for corresponding installation commands.
 
 #### Install Redco
 ```
 pip install redco
 ```
@@ -71,8 +68,7 @@
 ## Acknowledgement
 
 
 The name of this package, *Redco*, is inspired by *Red Coast Base*, a key location in the story of Three-Body. From Red Coast Base, humanity broadcasts its first message into the vast universe. We thank Cixin Liu for such a masterpiece!
 
 ![](https://preview.redd.it/vonp0gvw6sd61.jpg?width=1680&format=pjpg&auto=webp&s=ec76245e86fe1cdc70bad33adddb6794b5176051)
 (image: https://nhz123.lofter.com/post/1d7b3012_1c711d54c)
-
```

### Comparing `redco-0.4.8/README.md` & `redco-0.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 * **Automatic model/data parallelism**: No need to concern your large models and large datasets. *Redco* distributes your models and datasets to all your devices automatically. 
 * **No need to know JAX**: *Redco* only needs a couple of numpy-like functions as your pipeline design. 
 
 ### Installation
 
 #### Install Jax
 ```
-pip install --upgrade jax[cuda11_pip]==0.4.16 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade jax[cuda11_pip]==0.4.13 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
-Jax version (`==0.4.16`) can be flexible, as long as it matches your CUDA/CUDNN version.
+Jax version (`==0.4.13`) can be flexible, as long as it matches your CUDA/CUDNN version.
 
 If you are using TPU/CPU/AMD/Apple, see [here](https://github.com/google/jax#installation) for corresponding installation commands.
 
 #### Install Redco
 ```
 pip install redco
 ```
```

### Comparing `redco-0.4.8/redco/__init__.py` & `redco-0.4.9/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/datasets/__init__.py` & `redco-0.4.9/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/datasets/dataset.py` & `redco-0.4.9/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/datasets/jsonl_dataset.py` & `redco-0.4.9/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/__init__.py` & `redco-0.4.9/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/data_utils.py` & `redco-0.4.9/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/deployer.py` & `redco-0.4.9/redco/deployers/deployer.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
-import os
 import json
+import os
 import jax
 import jax.numpy as jnp
-import wandb
 from flax.jax_utils import replicate, unreplicate
 from flax.training.common_utils import shard_prng_key
 from flax.core.frozen_dict import unfreeze
-from flax.serialization import msgpack_serialize, msgpack_restore
+from flax.serialization import (
+    msgpack_serialize, msgpack_restore, from_state_dict, to_state_dict)
 
 from .data_utils import get_host_examples, get_data_batches
 from .opt_utils import get_lr_schedule_fn
 from .log_utils import get_logger, log_info, save_outputs
 from .model_parallel_utils.mesh_utils import (
     get_mesh,
     shard_params_and_opt_state,
@@ -36,26 +35,41 @@
 
 class Deployer:
     def __init__(self,
                  jax_seed,
                  n_model_shards=1,
                  verbose=True,
                  workdir=None,
+                 n_processes=1,
+                 host0_address=None,
+                 host0_port=None,
+                 process_id=None,
                  run_tensorboard=False,
                  run_wandb=False):
+        if n_processes > 1:
+            jax.distributed.initialize(
+                coordinator_address=f'{host0_address}:{host0_port}',
+                num_processes=n_processes,
+                process_id=process_id)
+
+            print(f'process_id: {jax.process_index()} / {jax.process_count()}')
+            print(f'devices: {jax.local_device_count()} / {jax.device_count()}')
+
         if workdir is not None:
             os.makedirs(workdir, exist_ok=True)
 
         self._verbose = verbose
         self._workdir = workdir
         self._logger = get_logger(verbose=verbose, workdir=workdir)
-        self._run_wandb = run_wandb
 
         if run_wandb:
             import wandb
+            self._wandb_log_fn = wandb.log
+        else:
+            self._wandb_log_fn = None
 
         if run_tensorboard and jax.process_index() == 0:
             from flax.metrics import tensorboard
             self._summary_writer = tensorboard.SummaryWriter(workdir)
         else:
             self._summary_writer = None
 
@@ -204,16 +218,16 @@
                 step=step)
 
     def log_metrics(self, metrics, step):
         if self._summary_writer is not None:
             for metric_name, value in metrics.items():
                 self._summary_writer.scalar(metric_name, value, step=step)
 
-        if self._run_wandb and jax.process_index() == 0:
-            wandb.log(metrics, step)
+        if self._wandb_log_fn is not None and jax.process_index() == 0:
+            self._wandb_log_fn(metrics, step)
 
     def save_outputs(self, outputs, desc, step):
         if self._workdir is not None and jax.process_index() == 0:
             save_outputs(
                 workdir=self._workdir,
                 outputs=outputs,
                 desc=desc,
@@ -225,43 +239,76 @@
         with jax.default_device(jax.devices('cpu')[0]):
             params = msgpack_restore(open(filepath, 'rb').read())
             params = jax.tree_util.tree_map(jnp.asarray, params)
 
         self.log_info(f'params loaded from {filepath}')
         return params
 
+    def load_opt_state(self, ckpt_dir, desc, target):
+        if self._mesh is None:
+            filepath = f'{ckpt_dir}/opt_state_{desc}.msgpack'
+            opt_state = msgpack_restore(open(filepath, 'rb').read())
+            opt_state = from_state_dict(target=target, state=opt_state)
+            opt_state = replicate(opt_state)
+        else:
+            n_processes_per_model = max(
+                1, self._mesh.shape['mp'] // jax.local_device_count())
+            ckpt_process_idx = jax.process_index() % n_processes_per_model
+            filepath = (f'{ckpt_dir}/opt_state_{desc}'
+                        f'_process_{ckpt_process_idx}.msgpack')
+            opt_state = msgpack_restore(open(filepath, 'rb').read())
+            opt_state = from_state_dict(target=target, state=opt_state)
+
+        return opt_state
+
     def save_params(self,
                     params,
-                    filepath,
-                    step=0,
-                    epoch_idx=-1,
+                    ckpt_dir,
+                    desc,
                     params_sharding_rules=None):
-        if self._mesh is not None:
+        if self._mesh is None:
+            params = unreplicate(params)
+        else:
             params_spec = self.get_params_spec(
                 params=params, params_sharding_rules=params_sharding_rules)
             params = gather_params_to_cpu(
                 params=params, params_spec=params_spec, mesh=self._mesh)
 
         if jax.process_index() == 0:
-            save_dir = '/'.join(filepath.split('/')[:-1])
-            os.makedirs(save_dir, exist_ok=True)
-
+            filepath = f'{ckpt_dir}/params_{desc}.msgpack'
             open(filepath, "wb").write(msgpack_serialize(unfreeze(params)))
             self.log_info(f'params saved into {filepath}')
 
-            if self.workdir is not None:
-                last_ckpt_info = {
-                    'last_ckpt': filepath,
-                    'last_step': step,
-                    'last_epoch_idx': epoch_idx
-                }
-
-                json.dump(last_ckpt_info, open(
-                    f'{self.workdir}/last_ckpt_info.json', 'w'))
-                self.log_info(f'{self.workdir}/last_ckpt_info.json updated.')
+    def save_opt_state(self, opt_state, ckpt_dir, desc):
+        if self._mesh is None:
+            if jax.process_index() == 0:
+                opt_state = to_state_dict(unreplicate(opt_state))
+
+                filepath = f'{ckpt_dir}/opt_state_{desc}.msgpack'
+                open(filepath, "wb").write(
+                    msgpack_serialize(unfreeze(opt_state)))
+                self.log_info(f'opt_state saved into {filepath}')
+        else:
+            assert (jax.local_device_count() % self._mesh.shape['mp'] == 0 or
+                    self._mesh.shape['mp'] % jax.local_device_count() == 0)
+            n_processes_per_model = max(
+                1, self._mesh.shape['mp'] // jax.local_device_count())
+
+            if jax.process_index() < n_processes_per_model:
+                opt_state = to_state_dict(opt_state)
+
+                filepath = (f'{ckpt_dir}/opt_state_{desc}'
+                            f'_process_{jax.process_index()}.msgpack')
+                open(filepath, "wb").write(
+                    msgpack_serialize(unfreeze(opt_state)))
+                self.log_info(f'opt_state saved into {filepath}')
+
+    def save_rng(self, ckpt_dir, desc):
+        if jax.process_index() == 0:
+            jnp.save(f'{ckpt_dir}/rng_{desc}.npy', self._rng)
 
     @property
     def mesh(self):
         return self._mesh
 
     @property
     def workdir(self):
```

### Comparing `redco-0.4.8/redco/deployers/log_utils.py` & `redco-0.4.9/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.9/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.9/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.9/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/deployers/opt_utils.py` & `redco-0.4.9/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/predictors/__init__.py` & `redco-0.4.9/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/predictors/predictor.py` & `redco-0.4.9/redco/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/predictors/utils.py` & `redco-0.4.9/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/trainers/__init__.py` & `redco-0.4.9/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco/trainers/trainer.py` & `redco-0.4.9/redco/trainers/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 #  limitations under the License.
 
 import os
 from functools import partial
 import json
 import numpy as np
 import jax
+import jax.numpy as jnp
 from jax.experimental.pjit import pjit
 from jax.sharding import PartitionSpec as P
 from flax.jax_utils import replicate
 from flax.training import train_state
 from flax.traverse_util import flatten_dict
 from flax.core.frozen_dict import freeze
+
 from .utils import default_train_step, default_eval_step
 from ..predictors import Predictor
 
 
 class Trainer:
     def __init__(self,
                  deployer,
@@ -49,37 +51,45 @@
         self._state_spec = None
         self._p_train_step = None
         self._p_eval_step = None
 
         n_params = sum([param.size for param in flatten_dict(params).values()])
         self._deployer.log_info(f'{n_params:,}', title='Training parameters')
 
-        last_ckpt_info_path = f'{self._deployer.workdir}/last_ckpt_info.json'
+        last_ckpt_info_path = \
+            f'{self.workdir}/ckpts/last_ckpt_info.json'
         if os.path.exists(last_ckpt_info_path):
             self._last_ckpt_info = json.load(open(last_ckpt_info_path))
-
+            desc = self._last_ckpt_info['last_desc']
             params = self._deployer.load_params(
-                self._last_ckpt_info['last_ckpt'])
+                filepath=f'{self.workdir}/ckpts/params_{desc}.msgpack')
+
             self.create_train_state(
                 apply_fn=self._apply_fn,
                 params=params,
                 optimizer=self._optimizer,
                 step=self._last_ckpt_info['last_step'])
 
-            for _ in range(self._last_ckpt_info['last_step']):
-                self._deployer.gen_rng()
+            self._state = self._state.replace(
+                opt_state=self._deployer.load_opt_state(
+                    ckpt_dir=f'{self.workdir}/ckpts',
+                    desc=desc,
+                    target=self._state.opt_state))
+
+            self._deployer._rng = jnp.load(
+                f'{self.workdir}/ckpts/rng_{desc}.npy')
 
             self._deployer.log_info(
-                'detect last_ckpt {last_ckpt},'
+                'detect last_ckpt \"{last_desc}\",'
                 ' last_step={last_step},'
                 ' last_epoch_idx={last_epoch_idx}'.format(
                     **self._last_ckpt_info))
         else:
             self._last_ckpt_info = \
-                {'last_ckpt': None, 'last_step': 0, 'last_epoch_idx': -1}
+                {'last_desc': None, 'last_step': 0, 'last_epoch_idx': -1}
             self.create_train_state(
                 apply_fn=apply_fn, params=params, optimizer=optimizer, step=0)
 
         self._default_predictor_fn = partial(
             Predictor,
             deployer=deployer,
             collate_fn=collate_fn,
@@ -214,57 +224,36 @@
             save_last_ckpt=False):
         if save_argmax_ckpt_by_metrics is None:
             save_argmax_ckpt_by_metrics = []
         if save_argmin_ckpt_by_metrics is None:
             save_argmin_ckpt_by_metrics = []
         min_metrics, max_metrics = {}, {}
 
-        if os.path.exists(f'{self._deployer.workdir}/min_metrics.json'):
+        if os.path.exists(f'{self.workdir}/min_metrics.json'):
             min_metrics = json.load(open(
-                f'{self._deployer.workdir}/min_metrics.json'))
+                f'{self.workdir}/min_metrics.json'))
             self._deployer.log_info(min_metrics, title='Detected min_metrics')
 
-        if os.path.exists(f'{self._deployer.workdir}/max_metrics.json'):
+        if os.path.exists(f'{self.workdir}/max_metrics.json'):
             max_metrics = json.load(open(
-                f'{self._deployer.workdir}/max_metrics.json'))
+                f'{self.workdir}/max_metrics.json'))
             self._deployer.log_info(max_metrics, title='Detected max_metrics')
 
         for epoch_idx in range(
                 self._last_ckpt_info['last_epoch_idx'] + 1, n_epochs):
             if isinstance(train_examples, list):
                 epoch_train_examples = train_examples
             else:
                 epoch_train_examples = train_examples(epoch_idx=epoch_idx)
 
             self.train(
                 examples=epoch_train_examples,
                 per_device_batch_size=per_device_batch_size,
                 desc=f'epoch {epoch_idx} / {n_epochs}')
 
-            save_ckpt_kwargs = {
-                'params': self.params,
-                'params_sharding_rules': self._params_sharding_rules,
-                'step': self.step,
-                'epoch_idx': epoch_idx
-            }
-
-            if save_every_ckpt:
-                assert self._deployer.workdir is not None
-                path_to_save = f'{self._deployer.workdir}/ckpts/' \
-                               f'epoch_{epoch_idx}.msgpack'
-                self._deployer.save_params(
-                    filepath=path_to_save, **save_ckpt_kwargs)
-
-            if save_last_ckpt:
-                assert self._deployer.workdir is not None
-                path_to_save = f'{self._deployer.workdir}/ckpts/' \
-                               f'last.msgpack'
-                self._deployer.save_params(
-                    filepath=path_to_save, **save_ckpt_kwargs)
-
             if eval_examples is None:
                 self._deployer.log_info(
                     'No evaluation cuz \'eval_examples\' is None.')
             else:
                 eval_metrics = {}
 
                 if eval_per_device_batch_size is None:
@@ -304,50 +293,87 @@
                     step=self.step)
                 self._deployer.log_metrics(metrics={
                     f'eval_{key}': value
                     for key, value in eval_metrics.items()
                 }, step=self.step)
 
                 for key in save_argmin_ckpt_by_metrics:
-                    assert self._deployer.workdir is not None
+                    assert self.workdir is not None
                     if eval_metrics[key] < min_metrics.get(key, float('inf')):
                         min_metrics[key] = eval_metrics[key]
-                        self._deployer.log_info(
-                            f'minimal {key} updated to {min_metrics[key]}')
-
-                        path_to_save = f'{self._deployer.workdir}/ckpts/'\
-                                       f'min_{key}.msgpack'
-                        self._deployer.save_params(
-                            filepath=path_to_save, **save_ckpt_kwargs)
 
                         if jax.process_index() == 0:
+                            self._deployer.log_info(
+                                f'minimal {key} updated to {min_metrics[key]}')
                             json.dump(max_metrics, open(
-                                f'{self._deployer.workdir}/max_metrics.json',
-                                'w'))
+                                f'{self.workdir}/max_metrics.json', 'w'))
+
+                        self.save_ckpt(
+                            desc=f'min_{key}',
+                            epoch_idx=epoch_idx,
+                            ckpt_dir=f'{self.workdir}/ckpts')
 
                 for key in save_argmax_ckpt_by_metrics:
-                    assert self._deployer.workdir is not None
+                    assert self.workdir is not None
                     if eval_metrics[key] > max_metrics.get(key, float('-inf')):
                         max_metrics[key] = eval_metrics[key]
-                        self._deployer.log_info(
-                            f'maximal {key} updated to {max_metrics[key]}')
-
-                        path_to_save = f'{self._deployer.workdir}/ckpts/'\
-                                       f'max_{key}.msgpack'
-                        self._deployer.save_params(
-                            filepath=path_to_save, **save_ckpt_kwargs)
 
                         if jax.process_index() == 0:
+                            self._deployer.log_info(
+                                f'maximal {key} updated to {max_metrics[key]}')
                             json.dump(max_metrics, open(
-                                f'{self._deployer.workdir}/max_metrics.json',
-                                'w'))
+                                f'{self.workdir}/max_metrics.json', 'w'))
+
+                        self.save_ckpt(
+                            desc=f'max_{key}',
+                            epoch_idx=epoch_idx,
+                            ckpt_dir=f'{self.workdir}/ckpts')
+
+            if save_every_ckpt:
+                self.save_ckpt(
+                    desc=f'epoch_{epoch_idx}',
+                    epoch_idx=epoch_idx,
+                    ckpt_dir=f'{self.workdir}/ckpts')
+            elif save_last_ckpt:
+                self.save_ckpt(
+                    desc=f'last',
+                    epoch_idx=epoch_idx,
+                    ckpt_dir=f'{self.workdir}/ckpts')
+
+    def save_ckpt(self, epoch_idx, desc, ckpt_dir):
+        if jax.process_index() == 0:
+            os.makedirs(ckpt_dir, exist_ok=True)
+
+        self._deployer.save_params(
+            params=self._state.params,
+            ckpt_dir=ckpt_dir,
+            desc=desc,
+            params_sharding_rules=self._params_sharding_rules)
+        self._deployer.save_opt_state(
+            opt_state=self._state.opt_state, ckpt_dir=ckpt_dir, desc=desc)
+        self._deployer.save_rng(ckpt_dir=ckpt_dir, desc=desc)
+
+        if jax.process_index() == 0:
+            last_ckpt_info = {
+                'last_desc': desc,
+                'last_step': self.step,
+                'last_epoch_idx': epoch_idx
+            }
+
+            json.dump(last_ckpt_info, open(
+                f'{ckpt_dir}/last_ckpt_info.json', 'w'), indent=4)
+            self._deployer.log_info(f'{ckpt_dir}/last_ckpt_info.json updated.')
 
     def get_default_predictor(self, pred_fn, output_fn=None):
         return self._default_predictor_fn(pred_fn=pred_fn, output_fn=output_fn)
 
     @property
     def params(self):
         return self._deployer.process_to_deliver(self._state.params)
 
     @property
     def step(self):
         return self._deployer.process_to_deliver(self._state.step).item()
+
+    @property
+    def workdir(self):
+        return self._deployer.workdir
```

### Comparing `redco-0.4.8/redco/trainers/utils.py` & `redco-0.4.9/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/redco.egg-info/PKG-INFO` & `redco-0.4.9/redco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.8
-Summary: UNKNOWN
+Version: 0.4.9
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Redco: A Lightweight Tool to Automate Distributed Training
 
 Redco is a lightweight and user-friendly tool designed to automate distributed training and inference for large models while simplifying the ML pipeline development process without necessitating MLSys expertise from users.
@@ -27,17 +24,17 @@
 * **Automatic model/data parallelism**: No need to concern your large models and large datasets. *Redco* distributes your models and datasets to all your devices automatically. 
 * **No need to know JAX**: *Redco* only needs a couple of numpy-like functions as your pipeline design. 
 
 ### Installation
 
 #### Install Jax
 ```
-pip install --upgrade jax[cuda11_pip]==0.4.16 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade jax[cuda11_pip]==0.4.13 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
-Jax version (`==0.4.16`) can be flexible, as long as it matches your CUDA/CUDNN version.
+Jax version (`==0.4.13`) can be flexible, as long as it matches your CUDA/CUDNN version.
 
 If you are using TPU/CPU/AMD/Apple, see [here](https://github.com/google/jax#installation) for corresponding installation commands.
 
 #### Install Redco
 ```
 pip install redco
 ```
@@ -71,8 +68,7 @@
 ## Acknowledgement
 
 
 The name of this package, *Redco*, is inspired by *Red Coast Base*, a key location in the story of Three-Body. From Red Coast Base, humanity broadcasts its first message into the vast universe. We thank Cixin Liu for such a masterpiece!
 
 ![](https://preview.redd.it/vonp0gvw6sd61.jpg?width=1680&format=pjpg&auto=webp&s=ec76245e86fe1cdc70bad33adddb6794b5176051)
 (image: https://nhz123.lofter.com/post/1d7b3012_1c711d54c)
-
```

### Comparing `redco-0.4.8/redco.egg-info/SOURCES.txt` & `redco-0.4.9/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.8/setup.py` & `redco-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.8",
+    version="0.4.9",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

