# Comparing `tmp/dex_retargeting-0.1.1-py3-none-any.whl.zip` & `tmp/dex_retargeting-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 28566 bytes, number of entries: 13
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-21 22:01 dex_retargeting/__init__.py
--rw-r--r--  2.0 unx     1439 b- defN 24-Mar-21 22:01 dex_retargeting/constants.py
--rw-r--r--  2.0 unx    22367 b- defN 24-Mar-21 22:01 dex_retargeting/optimizer.py
--rw-r--r--  2.0 unx     4185 b- defN 24-Mar-21 22:01 dex_retargeting/optimizer_utils.py
--rw-r--r--  2.0 unx     8562 b- defN 24-Mar-21 22:01 dex_retargeting/retargeting_config.py
--rw-r--r--  2.0 unx     4952 b- defN 24-Mar-21 22:01 dex_retargeting/seq_retarget.py
--rw-r--r--  2.0 unx    76137 b- defN 24-Mar-21 22:01 dex_retargeting/yourdfpy.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2494 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1131 b- defN 24-Mar-21 22:01 dex_retargeting-0.1.1.dist-info/RECORD
-13 files, 122473 bytes uncompressed, 26654 bytes compressed:  78.2%
+Zip file size: 30219 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-19 05:25 dex_retargeting/__init__.py
+-rw-r--r--  2.0 unx     1439 b- defN 24-Apr-19 05:25 dex_retargeting/constants.py
+-rw-r--r--  2.0 unx     3940 b- defN 24-Apr-19 05:25 dex_retargeting/kinematics_adaptor.py
+-rw-r--r--  2.0 unx    20369 b- defN 24-Apr-19 05:25 dex_retargeting/optimizer.py
+-rw-r--r--  2.0 unx      420 b- defN 24-Apr-19 05:25 dex_retargeting/optimizer_utils.py
+-rw-r--r--  2.0 unx     9668 b- defN 24-Apr-19 05:25 dex_retargeting/retargeting_config.py
+-rw-r--r--  2.0 unx     2791 b- defN 24-Apr-19 05:25 dex_retargeting/robot_wrapper.py
+-rw-r--r--  2.0 unx     5044 b- defN 24-Apr-19 05:25 dex_retargeting/seq_retarget.py
+-rw-r--r--  2.0 unx    76144 b- defN 24-Apr-19 05:25 dex_retargeting/yourdfpy.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2574 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1313 b- defN 24-Apr-19 05:25 dex_retargeting-0.2.0.dist-info/RECORD
+15 files, 124908 bytes uncompressed, 28017 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -1,40 +1,46 @@
 Filename: dex_retargeting/__init__.py
 Comment: 
 
 Filename: dex_retargeting/constants.py
 Comment: 
 
+Filename: dex_retargeting/kinematics_adaptor.py
+Comment: 
+
 Filename: dex_retargeting/optimizer.py
 Comment: 
 
 Filename: dex_retargeting/optimizer_utils.py
 Comment: 
 
 Filename: dex_retargeting/retargeting_config.py
 Comment: 
 
+Filename: dex_retargeting/robot_wrapper.py
+Comment: 
+
 Filename: dex_retargeting/seq_retarget.py
 Comment: 
 
 Filename: dex_retargeting/yourdfpy.py
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/LICENSE
+Filename: dex_retargeting-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/METADATA
+Filename: dex_retargeting-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/WHEEL
+Filename: dex_retargeting-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/top_level.txt
+Filename: dex_retargeting-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/zip-safe
+Filename: dex_retargeting-0.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: dex_retargeting-0.1.1.dist-info/RECORD
+Filename: dex_retargeting-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dex_retargeting/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.1"
+__version__ = "0.2.0"
```

## dex_retargeting/optimizer.py

```diff
@@ -1,90 +1,104 @@
 from abc import abstractmethod
-from typing import List
+from typing import List, Optional
 
 import nlopt
 import numpy as np
-import sapien.core as sapien
 import torch
 
+from dex_retargeting.kinematics_adaptor import KinematicAdaptor, MimicJointKinematicAdaptor
+from dex_retargeting.robot_wrapper import RobotWrapper
+
 
 class Optimizer:
     retargeting_type = "BASE"
 
     def __init__(
         self,
-        robot: sapien.Articulation,
+        robot: RobotWrapper,
         wrist_link_name: str,
         target_joint_names: List[str],
         target_link_human_indices: np.ndarray,
     ):
         self.robot = robot
-        self.robot_dof = robot.dof
-        self.model = robot.create_pinocchio_model()
+        self.num_joints = robot.dof
         self.wrist_link_name = wrist_link_name
 
-        joint_names = [joint.get_name() for joint in robot.get_active_joints()]
-        target_joint_index = []
+        joint_names = robot.dof_joint_names
+        idx_pin2target = []
         for target_joint_name in target_joint_names:
             if target_joint_name not in joint_names:
                 raise ValueError(f"Joint {target_joint_name} given does not appear to be in robot XML.")
-            target_joint_index.append(joint_names.index(target_joint_name))
+            idx_pin2target.append(joint_names.index(target_joint_name))
         self.target_joint_names = target_joint_names
-        self.target_joint_indices = np.array(target_joint_index)
-        self.fixed_joint_indices = np.array([i for i in range(robot.dof) if i not in target_joint_index], dtype=int)
-        self.opt = nlopt.opt(nlopt.LD_SLSQP, len(target_joint_index))
-        self.dof = len(target_joint_index)
+        self.idx_pin2target = np.array(idx_pin2target)
+
+        self.idx_pin2fixed = np.array([i for i in range(robot.dof) if i not in idx_pin2target], dtype=int)
+        self.opt = nlopt.opt(nlopt.LD_SLSQP, len(idx_pin2target))
+        self.opt_dof = len(idx_pin2target)  # This dof includes the mimic joints
 
         # Target
         self.target_link_human_indices = target_link_human_indices
 
         # Free joint
-        link_names = [link.get_name() for link in self.robot.get_links()]
+        link_names = robot.link_names
         self.has_free_joint = len([name for name in link_names if "dummy" in name]) >= 6
 
+        # Kinematics adaptor
+        self.adaptor: Optional[KinematicAdaptor] = None
+
     def set_joint_limit(self, joint_limits: np.ndarray):
-        if joint_limits.shape != (self.dof, 2):
-            raise ValueError(f"Expect joint limits have shape: {(self.dof, 2)}, but get {joint_limits.shape}")
+        if joint_limits.shape != (self.opt_dof, 2):
+            raise ValueError(f"Expect joint limits have shape: {(self.opt_dof, 2)}, but get {joint_limits.shape}")
         self.opt.set_lower_bounds(joint_limits[:, 0].tolist())
         self.opt.set_upper_bounds(joint_limits[:, 1].tolist())
 
-    def get_last_result(self):
-        return self.opt.last_optimize_result()
-
-    def get_link_names(self):
-        return [link.get_name() for link in self.robot.get_links()]
-
     def get_link_indices(self, target_link_names):
-        target_link_index = []
-        for target_link_name in target_link_names:
-            if target_link_name not in self.get_link_names():
-                raise ValueError(f"Body {target_link_name} given does not appear to be in robot XML.")
-            target_link_index.append(self.get_link_names().index(target_link_name))
-        return target_link_index
-
-    @abstractmethod
-    def retarget(self, ref_value, fixed_qpos, last_qpos=None):
-        pass
+        return [self.robot.get_link_index(link_name) for link_name in target_link_names]
 
     def optimize(self, objective_fn, last_qpos):
         self.opt.set_min_objective(objective_fn)
         try:
             qpos = self.opt.optimize(last_qpos)
+            return np.array(qpos)
         except RuntimeError as e:
             print(e)
             return np.array(last_qpos)
-        return qpos
+
+    def set_kinematic_adaptor(self, adaptor: KinematicAdaptor):
+        self.adaptor = adaptor
+
+        # Remove mimic joints from fixed joint list
+        if isinstance(adaptor, MimicJointKinematicAdaptor):
+            fixed_idx = self.idx_pin2fixed
+            mimic_idx = adaptor.idx_pin2mimic
+            new_fixed_id = np.array([x for x in fixed_idx if x not in mimic_idx], dtype=int)
+            self.idx_pin2fixed = new_fixed_id
+
+    def retarget(self, ref_value, fixed_qpos, last_qpos=None):
+        if len(fixed_qpos) != len(self.idx_pin2fixed):
+            raise ValueError(
+                f"Optimizer has {len(self.idx_pin2fixed)} joints but non_target_qpos {fixed_qpos} is given"
+            )
+        if last_qpos is None:
+            last_qpos = self.robot.q0.copy()[self.idx_pin2target]
+        objective_fn = self.get_objective_function(ref_value, fixed_qpos, np.array(last_qpos).astype(np.float32))
+        return np.array(self.optimize(objective_fn, last_qpos))
+
+    @abstractmethod
+    def get_objective_function(self, ref_value: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
+        pass
 
 
 class PositionOptimizer(Optimizer):
     retargeting_type = "position"
 
     def __init__(
         self,
-        robot: sapien.Articulation,
+        robot: RobotWrapper,
         wrist_link_name: str,
         target_joint_names: List[str],
         target_link_names: List[str],
         target_link_human_indices: np.ndarray,
         huber_delta=0.02,
         norm_delta=4e-3,
     ):
@@ -92,94 +106,79 @@
         self.body_names = target_link_names
         self.huber_loss = torch.nn.SmoothL1Loss(beta=huber_delta)
         self.norm_delta = norm_delta
 
         # Sanity check and cache link indices
         self.target_link_indices = self.get_link_indices(target_link_names)
 
-        # Use local jacobian if target link name <= 2, otherwise first cache all jacobian and then get all
-        # This is only for the speed but will not affect the performance
-        if len(target_link_names) <= 40:
-            self.use_sparse_jacobian = True
-        else:
-            self.use_sparse_jacobian = False
         self.opt.set_ftol_abs(1e-5)
 
-    def _get_objective_function(self, target_pos: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
-        qpos = np.zeros(self.robot_dof)
-        qpos[self.fixed_joint_indices] = fixed_qpos
+    def get_objective_function(self, target_pos: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
+        qpos = np.zeros(self.num_joints)
+        qpos[self.idx_pin2fixed] = fixed_qpos
         torch_target_pos = torch.as_tensor(target_pos)
         torch_target_pos.requires_grad_(False)
 
         def objective(x: np.ndarray, grad: np.ndarray) -> float:
-            qpos[self.target_joint_indices] = x
-            self.model.compute_forward_kinematics(qpos)
-            target_link_poses = [self.model.get_link_pose(index) for index in self.target_link_indices]
-            body_pos = np.array([pose.p for pose in target_link_poses])
+            qpos[self.idx_pin2target] = x
+
+            # Kinematics forwarding for qpos
+            if self.adaptor is not None:
+                qpos[:] = self.adaptor.forward_qpos(qpos)[:]
+
+            self.robot.compute_forward_kinematics(qpos)
+            target_link_poses = [self.robot.get_link_pose(index) for index in self.target_link_indices]
+            body_pos = np.stack([pose[:3, 3] for pose in target_link_poses], axis=0)  # (n ,3)
 
             # Torch computation for accurate loss and grad
             torch_body_pos = torch.as_tensor(body_pos)
             torch_body_pos.requires_grad_()
 
             # Loss term for kinematics retargeting based on 3D position error
             huber_distance = self.huber_loss(torch_body_pos, torch_target_pos)
-            # huber_distance = torch.norm(torch_body_pos - torch_target_pos, dim=1).mean()
             result = huber_distance.cpu().detach().item()
 
             if grad.size > 0:
-                if self.use_sparse_jacobian:
-                    jacobians = []
-                    for i, index in enumerate(self.target_link_indices):
-                        link_spatial_jacobian = self.model.compute_single_link_local_jacobian(qpos, index)[
-                            :3, self.target_joint_indices
-                        ]
-                        link_rot = self.model.get_link_pose(index).to_transformation_matrix()[:3, :3]
-                        link_kinematics_jacobian = link_rot @ link_spatial_jacobian
-                        jacobians.append(link_kinematics_jacobian)
-                    jacobians = np.stack(jacobians, axis=0)
-                else:
-                    self.model.compute_full_jacobian(qpos)
-                    jacobians = [
-                        self.model.get_link_jacobian(index, local=True)[:3, self.target_joint_indices]
-                        for index in self.target_link_indices
-                    ]
+                jacobians = []
+                for i, index in enumerate(self.target_link_indices):
+                    link_body_jacobian = self.robot.compute_single_link_local_jacobian(qpos, index)[:3, ...]
+                    link_pose = target_link_poses[i]
+                    link_rot = link_pose[:3, :3]
+                    link_kinematics_jacobian = link_rot @ link_body_jacobian
+                    jacobians.append(link_kinematics_jacobian)
 
+                # Note: the joint order in this jacobian is consistent pinocchio
+                jacobians = np.stack(jacobians, axis=0)
                 huber_distance.backward()
                 grad_pos = torch_body_pos.grad.cpu().numpy()[:, None, :]
-                grad_qpos = np.matmul(grad_pos, np.array(jacobians))
-                grad_qpos = grad_qpos.mean(1).sum(0)
 
+                # Convert the jacobian from pinocchio order to target order
+                if self.adaptor is not None:
+                    jacobians = self.adaptor.backward_jacobian(jacobians)
+                else:
+                    jacobians = jacobians[..., self.idx_pin2target]
+
+                # Compute the gradient to the qpos
+                grad_qpos = np.matmul(grad_pos, jacobians)
+                grad_qpos = grad_qpos.mean(1).sum(0)
                 grad_qpos += 2 * self.norm_delta * (x - last_qpos)
 
                 grad[:] = grad_qpos[:]
 
             return result
 
         return objective
 
-    def retarget(self, ref_value, fixed_qpos, last_qpos=None):
-        if len(fixed_qpos) != len(self.fixed_joint_indices):
-            raise ValueError(
-                f"Optimizer has {len(self.fixed_joint_indices)} joints but non_target_qpos {fixed_qpos} is given"
-            )
-        if last_qpos is None:
-            last_qpos = np.zeros(self.dof)
-        if isinstance(last_qpos, np.ndarray):
-            last_qpos = last_qpos.astype(np.float32)
-        last_qpos = list(last_qpos)
-        objective_fn = self._get_objective_function(ref_value, fixed_qpos, np.array(last_qpos).astype(np.float32))
-        return self.optimize(objective_fn, last_qpos)
-
 
 class VectorOptimizer(Optimizer):
     retargeting_type = "VECTOR"
 
     def __init__(
         self,
-        robot: sapien.Articulation,
+        robot: RobotWrapper,
         wrist_link_name: str,
         target_joint_names: List[str],
         target_origin_link_names: List[str],
         target_task_link_names: List[str],
         target_link_human_indices: np.ndarray,
         huber_delta=0.02,
         norm_delta=4e-3,
@@ -196,36 +195,35 @@
         # For one link used in multiple vectors, e.g. hand palm, we do not want to compute it multiple times
         self.computed_link_names = list(set(target_origin_link_names).union(set(target_task_link_names)))
         self.origin_link_indices = torch.tensor(
             [self.computed_link_names.index(name) for name in target_origin_link_names]
         )
         self.task_link_indices = torch.tensor([self.computed_link_names.index(name) for name in target_task_link_names])
 
-        # Sanity check and cache link indices
-        self.robot_link_indices = self.get_link_indices(self.computed_link_names)
+        # Cache link indices that will involve in kinematics computation
+        self.computed_link_indices = self.get_link_indices(self.computed_link_names)
 
-        # Use local jacobian if target link name <= 2, otherwise first cache all jacobian and then get all
-        # This is only for the speed but will not affect the performance
-        if len(self.computed_link_names) <= 40:
-            self.use_sparse_jacobian = True
-        else:
-            self.use_sparse_jacobian = False
         self.opt.set_ftol_abs(1e-6)
 
-    def _get_objective_function(self, target_vector: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
-        qpos = np.zeros(self.robot_dof)
-        qpos[self.fixed_joint_indices] = fixed_qpos
+    def get_objective_function(self, target_vector: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
+        qpos = np.zeros(self.num_joints)
+        qpos[self.idx_pin2fixed] = fixed_qpos
         torch_target_vec = torch.as_tensor(target_vector) * self.scaling
         torch_target_vec.requires_grad_(False)
 
         def objective(x: np.ndarray, grad: np.ndarray) -> float:
-            qpos[self.target_joint_indices] = x
-            self.model.compute_forward_kinematics(qpos)
-            target_link_poses = [self.model.get_link_pose(index) for index in self.robot_link_indices]
-            body_pos = np.array([pose.p for pose in target_link_poses])
+            qpos[self.idx_pin2target] = x
+
+            # Kinematics forwarding for qpos
+            if self.adaptor is not None:
+                qpos[:] = self.adaptor.forward_qpos(qpos)[:]
+
+            self.robot.compute_forward_kinematics(qpos)
+            target_link_poses = [self.robot.get_link_pose(index) for index in self.computed_link_indices]
+            body_pos = np.array([pose[:3, 3] for pose in target_link_poses])
 
             # Torch computation for accurate loss and grad
             torch_body_pos = torch.as_tensor(body_pos)
             torch_body_pos.requires_grad_()
 
             # Index link for computation
             origin_link_pos = torch_body_pos[self.origin_link_indices, :]
@@ -234,55 +232,43 @@
 
             # Loss term for kinematics retargeting based on 3D position error
             vec_dist = torch.norm(robot_vec - torch_target_vec, dim=1, keepdim=False)
             huber_distance = self.huber_loss(vec_dist, torch.zeros_like(vec_dist))
             result = huber_distance.cpu().detach().item()
 
             if grad.size > 0:
-                if self.use_sparse_jacobian:
-                    jacobians = []
-                    for i, index in enumerate(self.robot_link_indices):
-                        link_spatial_jacobian = self.model.compute_single_link_local_jacobian(qpos, index)[
-                            :3, self.target_joint_indices
-                        ]
-                        link_rot = self.model.get_link_pose(index).to_transformation_matrix()[:3, :3]
-                        link_kinematics_jacobian = link_rot @ link_spatial_jacobian
-                        jacobians.append(link_kinematics_jacobian)
-                    jacobians = np.stack(jacobians, axis=0)
-                else:
-                    self.model.compute_full_jacobian(qpos)
-                    jacobians = [
-                        self.model.get_link_jacobian(index, local=True)[:3, self.target_joint_indices]
-                        for index in self.robot_link_indices
-                    ]
+                jacobians = []
+                for i, index in enumerate(self.computed_link_indices):
+                    link_body_jacobian = self.robot.compute_single_link_local_jacobian(qpos, index)[:3, ...]
+                    link_pose = target_link_poses[i]
+                    link_rot = link_pose[:3, :3]
+                    link_kinematics_jacobian = link_rot @ link_body_jacobian
+                    jacobians.append(link_kinematics_jacobian)
 
+                # Note: the joint order in this jacobian is consistent pinocchio
+                jacobians = np.stack(jacobians, axis=0)
                 huber_distance.backward()
                 grad_pos = torch_body_pos.grad.cpu().numpy()[:, None, :]
+
+                # Convert the jacobian from pinocchio order to target order
+                if self.adaptor is not None:
+                    jacobians = self.adaptor.backward_jacobian(jacobians)
+                else:
+                    jacobians = jacobians[..., self.idx_pin2target]
+
                 grad_qpos = np.matmul(grad_pos, np.array(jacobians))
                 grad_qpos = grad_qpos.mean(1).sum(0)
-
                 grad_qpos += 2 * self.norm_delta * (x - last_qpos)
 
                 grad[:] = grad_qpos[:]
 
             return result
 
         return objective
 
-    def retarget(self, ref_value, fixed_qpos, last_qpos=None):
-        if len(fixed_qpos) != len(self.fixed_joint_indices):
-            raise ValueError(
-                f"Optimizer has {len(self.fixed_joint_indices)} joints but non_target_qpos {fixed_qpos} is given"
-            )
-        if last_qpos is None:
-            last_qpos = np.zeros(self.dof)
-        last_qpos = list(last_qpos)
-        objective_fn = self._get_objective_function(ref_value, fixed_qpos, np.array(last_qpos).astype(np.float32))
-        return self.optimize(objective_fn, last_qpos)
-
 
 class DexPilotAllegroOptimizer(Optimizer):
     """Retargeting optimizer using the method proposed in DexPilot
 
     This is a broader adaptation of the original optimizer delineated in the DexPilot paper.
     While the initial DexPilot study focused solely on the four-fingered Allegro Hand, this version of the optimizer
     embraces the same principles for both four-fingered and five-fingered hands. It projects the distance between the
@@ -302,15 +288,15 @@
         scaling:
     """
 
     retargeting_type = "DEXPILOT"
 
     def __init__(
         self,
-        robot: sapien.Articulation,
+        robot: RobotWrapper,
         target_joint_names: List[str],
         finger_tip_link_names: List[str],
         wrist_link_name: str,
         huber_delta=0.03,
         norm_delta=4e-3,
         # DexPilot parameters
         # gamma=2.5e-3,
@@ -355,42 +341,33 @@
         self.computed_link_names = list(set(target_origin_link_names).union(set(target_task_link_names)))
         self.origin_link_indices = torch.tensor(
             [self.computed_link_names.index(name) for name in target_origin_link_names]
         )
         self.task_link_indices = torch.tensor([self.computed_link_names.index(name) for name in target_task_link_names])
 
         # Sanity check and cache link indices
-        self.robot_link_indices = self.get_link_indices(self.computed_link_names)
+        self.computed_link_indices = self.get_link_indices(self.computed_link_names)
 
-        # Use local jacobian if target link name <= 2, otherwise first cache all jacobian and then get all
-        # This is only for the speed but will not affect the performance
-        if len(self.computed_link_names) <= 40:
-            self.use_sparse_jacobian = True
-        else:
-            self.use_sparse_jacobian = False
         self.opt.set_ftol_abs(1e-6)
 
         # DexPilot cache
         if is_four_finger:
             self.projected = np.zeros(6, dtype=bool)
             self.s2_project_index_origin = np.array([1, 2, 2], dtype=int)
             self.s2_project_index_task = np.array([0, 0, 1], dtype=int)
             self.projected_dist = np.array([eta1] * 3 + [eta2] * 3)
         else:
             self.projected = np.zeros(10, dtype=bool)
             self.s2_project_index_origin = np.array([1, 2, 3, 2, 3, 3], dtype=int)
             self.s2_project_index_task = np.array([0, 0, 0, 1, 1, 2], dtype=int)
             self.projected_dist = np.array([eta1] * 4 + [eta2] * 6)
 
-    def _get_objective_function_four_finger(
-        self, target_vector: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray
-    ):
-        target_vector = target_vector.astype(np.float32)
-        qpos = np.zeros(self.robot_dof)
-        qpos[self.fixed_joint_indices] = fixed_qpos
+    def get_objective_function(self, target_vector: np.ndarray, fixed_qpos: np.ndarray, last_qpos: np.ndarray):
+        qpos = np.zeros(self.num_joints)
+        qpos[self.idx_pin2fixed] = fixed_qpos
 
         len_proj = len(self.projected)
         len_s2 = len(self.s2_project_index_task)
         len_s1 = len_proj - len_s2
 
         # Update projection indicator
         target_vec_dist = np.linalg.norm(target_vector[:len_proj], axis=1)
@@ -422,18 +399,23 @@
         # Compute final reference vector
         reference_vec = np.where(self.projected[:, None], projected_vec, normal_vec[:len_proj])  # (6, 3)
         reference_vec = np.concatenate([reference_vec, normal_vec[len_proj:]], axis=0)  # (10, 3)
         torch_target_vec = torch.as_tensor(reference_vec, dtype=torch.float32)
         torch_target_vec.requires_grad_(False)
 
         def objective(x: np.ndarray, grad: np.ndarray) -> float:
-            qpos[self.target_joint_indices] = x
-            self.model.compute_forward_kinematics(qpos)
-            target_link_poses = [self.model.get_link_pose(index) for index in self.robot_link_indices]
-            body_pos = np.array([pose.p for pose in target_link_poses])
+            qpos[self.idx_pin2target] = x
+
+            # Kinematics forwarding for qpos
+            if self.adaptor is not None:
+                qpos[:] = self.adaptor.forward_qpos(qpos)[:]
+
+            self.robot.compute_forward_kinematics(qpos)
+            target_link_poses = [self.robot.get_link_pose(index) for index in self.computed_link_indices]
+            body_pos = np.array([pose[:3, 3] for pose in target_link_poses])
 
             # Torch computation for accurate loss and grad
             torch_body_pos = torch.as_tensor(body_pos)
             torch_body_pos.requires_grad_()
 
             # Index link for computation
             origin_link_pos = torch_body_pos[self.origin_link_indices, :]
@@ -446,51 +428,39 @@
             huber_distance = (
                 self.huber_loss(vec_dist, torch.zeros_like(vec_dist)) * weight / (robot_vec.shape[0])
             ).sum()
             huber_distance = huber_distance.sum()
             result = huber_distance.cpu().detach().item()
 
             if grad.size > 0:
-                if self.use_sparse_jacobian:
-                    jacobians = []
-                    for i, index in enumerate(self.robot_link_indices):
-                        link_spatial_jacobian = self.model.compute_single_link_local_jacobian(qpos, index)[
-                            :3, self.target_joint_indices
-                        ]
-                        link_rot = self.model.get_link_pose(index).to_transformation_matrix()[:3, :3]
-                        link_kinematics_jacobian = link_rot @ link_spatial_jacobian
-                        jacobians.append(link_kinematics_jacobian)
-                    jacobians = np.stack(jacobians, axis=0)
-                else:
-                    self.model.compute_full_jacobian(qpos)
-                    jacobians = [
-                        self.model.get_link_jacobian(index, local=True)[:3, self.target_joint_indices]
-                        for index in self.robot_link_indices
-                    ]
+                jacobians = []
+                for i, index in enumerate(self.computed_link_indices):
+                    link_body_jacobian = self.robot.compute_single_link_local_jacobian(qpos, index)[:3, ...]
+                    link_pose = target_link_poses[i]
+                    link_rot = link_pose[:3, :3]
+                    link_kinematics_jacobian = link_rot @ link_body_jacobian
+                    jacobians.append(link_kinematics_jacobian)
 
+                # Note: the joint order in this jacobian is consistent pinocchio
+                jacobians = np.stack(jacobians, axis=0)
                 huber_distance.backward()
                 grad_pos = torch_body_pos.grad.cpu().numpy()[:, None, :]
+
+                # Convert the jacobian from pinocchio order to target order
+                if self.adaptor is not None:
+                    jacobians = self.adaptor.backward_jacobian(jacobians)
+                else:
+                    jacobians = jacobians[..., self.idx_pin2target]
+
                 grad_qpos = np.matmul(grad_pos, np.array(jacobians))
                 grad_qpos = grad_qpos.mean(1).sum(0)
 
                 # In the original DexPilot, γ = 2.5 × 10−3 is a weight on regularizing the Allegro angles to zero
                 # which is equivalent to fully opened the hand
                 # In our implementation, we regularize the joint angles to the previous joint angles
                 grad_qpos += 2 * self.norm_delta * (x - last_qpos)
 
                 grad[:] = grad_qpos[:]
 
             return result
 
         return objective
-
-    def retarget(self, ref_value, fixed_qpos, last_qpos=None):
-        if len(fixed_qpos) != len(self.fixed_joint_indices):
-            raise ValueError(
-                f"Optimizer has {len(self.fixed_joint_indices)} joints but non_target_qpos {fixed_qpos} is given"
-            )
-        if last_qpos is None:
-            last_qpos = np.zeros(self.dof)
-        objective_fn = self._get_objective_function_four_finger(
-            ref_value, fixed_qpos, np.array(last_qpos).astype(np.float32)
-        )
-        return self.optimize(objective_fn, last_qpos)
```

## dex_retargeting/optimizer_utils.py

```diff
@@ -1,15 +1,7 @@
-from typing import Optional
-
-import numpy as np
-import sapien.core as sapien
-from sapien.core import Pose
-from transforms3d.euler import euler2quat
-
-
 class LPFilter:
     def __init__(self, alpha):
         self.alpha = alpha
         self.y = None
         self.is_init = False
 
     def next(self, x):
@@ -19,101 +11,7 @@
             return self.y.copy()
         self.y = self.y + self.alpha * (x - self.y)
         return self.y.copy()
 
     def reset(self):
         self.y = None
         self.is_init = False
-
-
-def add_dummy_free_joint(
-    robot_builder: sapien.ArticulationBuilder,
-    joint_indicator=(True, True, True, True, True, True),
-    translation_range=(-1, 1),
-    rotation_range=(-np.pi, np.pi),
-):
-    assert len(joint_indicator) == 6
-    new_root = robot_builder.create_link_builder()
-    parent = new_root
-
-    # Prepare link and joint properties
-    joint_types = ["prismatic"] * 3 + ["revolute"] * 3
-    joint_limit = [translation_range] * 3 + [rotation_range] * 3
-    joint_name = [f"dummy_{name}_translation_joint" for name in "xyz"] + [
-        f"dummy_{name}_rotation_joint" for name in "xyz"
-    ]
-    link_name = [f"dummy_{name}_translation_link" for name in "xyz"] + [f"dummy_{name}_rotation_link" for name in "xyz"]
-
-    # Find root link which has no parent
-    root_link_builder = None
-    for link_builder in robot_builder.get_link_builders():
-        if link_builder.get_parent() == -1:
-            root_link_builder = link_builder
-            break
-    assert root_link_builder is not None
-
-    # Build free root
-    valid_joint_num = 0
-    for i in range(6):
-        # Joint orders are x,y,z translation and then x,y,z rotation, 6 in total
-        # If joint indicator for specific index is False, do not build this joint
-        if not joint_indicator[i]:
-            continue
-        valid_joint_num += 1
-
-        # Add small inertia property for more stable simulation
-        parent.set_mass_and_inertia(1e-4, Pose(np.zeros(3)), np.ones(3) * 1e-6)
-        parent.set_name(link_name[i])
-
-        # The last joint will connect the last dummy link to the original root link of the robot
-        if valid_joint_num < sum(joint_indicator):
-            child = robot_builder.create_link_builder(parent)
-        else:
-            child = root_link_builder
-            child.set_parent(parent.get_index())
-        child.set_joint_name(joint_name[i])
-
-        # Build joint
-        if i == 3 or i == 0:
-            child.set_joint_properties(joint_types[i], limits=np.array([joint_limit[i]]))
-        elif i == 4 or i == 1:
-            child.set_joint_properties(
-                joint_types[i],
-                limits=np.array([joint_limit[i]]),
-                pose_in_child=Pose(q=euler2quat(0, 0, np.pi / 2)),
-                pose_in_parent=Pose(q=euler2quat(0, 0, np.pi / 2)),
-            )
-        elif i == 2 or i == 5:
-            child.set_joint_properties(
-                joint_types[i],
-                limits=np.array([joint_limit[i]]),
-                pose_in_parent=Pose(q=euler2quat(0, -np.pi / 2, 0)),
-                pose_in_child=Pose(q=euler2quat(0, -np.pi / 2, 0)),
-            )
-        parent = child
-
-    return parent
-
-
-class SAPIENKinematicsModelStandalone:
-    def __init__(
-        self, urdf_path, add_dummy_translation=False, add_dummy_rotation=False, scene: Optional[sapien.Scene] = None
-    ):
-        if scene is None:
-            self.engine = sapien.Engine()
-            self.scene = self.engine.create_scene()
-        else:
-            self.scene = scene
-            self.engine = self.scene.engine
-        loader = self.scene.create_urdf_loader()
-
-        builder = loader.load_file_as_articulation_builder(urdf_path)
-        if add_dummy_rotation or add_dummy_translation:
-            dummy_joint_indicator = (add_dummy_translation,) * 3 + (add_dummy_rotation,) * 3
-            add_dummy_free_joint(builder, dummy_joint_indicator)
-        self.robot = builder.build(fix_root_link=True)
-        self.robot.set_pose(sapien.Pose())
-        self.robot.set_qpos(np.zeros(self.robot.dof))
-
-    def release(self):
-        self.scene = None
-        self.engine = None
```

## dex_retargeting/retargeting_config.py

```diff
@@ -1,18 +1,21 @@
-import sapien.core as sapien
+# import sapien.core as sapien
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict, Any, Tuple
 from typing import Union
 
 import numpy as np
 import yaml
 
 from dex_retargeting.optimizer_utils import LPFilter
+from dex_retargeting.robot_wrapper import RobotWrapper
 from dex_retargeting.seq_retarget import SeqRetargeting
+from dex_retargeting import yourdfpy as urdf
+from dex_retargeting.kinematics_adaptor import MimicJointKinematicAdaptor
 
 
 @dataclass
 class RetargetingConfig:
     type: str
     urdf_path: str
 
@@ -41,20 +44,20 @@
     # For example, Allegro is 1.6 times larger than normal human hand, then this scaling factor should be 1.6
     scaling_factor: float = 1.0
 
     # Optimization hyperparameter
     normal_delta: float = 4e-3
     huber_delta: float = 2e-2
 
-    # Constraint parameters
-    constraint_map: Optional[Dict[str, np.ndarray]] = None
-
     # Joint limit tag
     has_joint_limits: bool = True
 
+    # Mimic joint tag
+    ignore_mimic_joint: bool = False
+
     # Low pass filter
     low_pass_alpha: float = 0.1
 
     _TYPE = ["vector", "position", "dexpilot"]
     _DEFAULT_URDF_DIR = "./"
 
     def __post_init__(self):
@@ -121,43 +124,32 @@
             cfg["target_link_human_indices"] = np.array(cfg["target_link_human_indices"])
         if override is not None:
             for key, value in override.items():
                 cfg[key] = value
         config = RetargetingConfig(**cfg)
         return config
 
-    def build(self, scene: Optional[sapien.Scene] = None) -> SeqRetargeting:
+    def build(self) -> SeqRetargeting:
         from dex_retargeting.optimizer import (
             VectorOptimizer,
             PositionOptimizer,
             DexPilotAllegroOptimizer,
         )
-        from dex_retargeting.optimizer_utils import SAPIENKinematicsModelStandalone
-        from dex_retargeting import yourdfpy as urdf
         import tempfile
 
         # Process the URDF with yourdfpy to better find file path
-        robot_urdf = urdf.URDF.load(self.urdf_path)
+        robot_urdf = urdf.URDF.load(self.urdf_path, build_scene_graph=False)
         urdf_name = self.urdf_path.split("/")[-1]
         temp_dir = tempfile.mkdtemp(prefix="dex_retargeting-")
         temp_path = f"{temp_dir}/{urdf_name}"
         robot_urdf.write_xml_file(temp_path)
-        sapien_model = SAPIENKinematicsModelStandalone(
-            temp_path,
-            add_dummy_translation=self.add_dummy_free_joint,
-            add_dummy_rotation=self.add_dummy_free_joint,
-            scene=scene,
-        )
-        robot = sapien_model.robot
-        robot.set_name(Path(self.urdf_path).stem)
-        joint_names = (
-            self.target_joint_names
-            if self.target_joint_names is not None
-            else [joint.get_name() for joint in robot.get_active_joints()]
-        )
+
+        # Load pinocchio model
+        robot = RobotWrapper(temp_path)
+        joint_names = self.target_joint_names if self.target_joint_names is not None else robot.dof_joint_names
         if self.type == "position":
             optimizer = PositionOptimizer(
                 robot,
                 self.wrist_link_name,
                 joint_names,
                 target_link_names=self.target_link_names,
                 target_link_human_indices=self.target_link_human_indices,
@@ -188,29 +180,61 @@
             raise RuntimeError()
 
         if 0 <= self.low_pass_alpha <= 1:
             lp_filter = LPFilter(self.low_pass_alpha)
         else:
             lp_filter = None
 
+        # Parse mimic joints and set kinematics adaptor for optimizer
+        has_mimic_joints, source_names, mimic_names, multipliers, offsets = parse_mimic_joint(robot_urdf)
+        if has_mimic_joints and not self.ignore_mimic_joint:
+            adaptor = MimicJointKinematicAdaptor(
+                robot,
+                target_joint_names=joint_names,
+                source_joint_names=source_names,
+                mimic_joint_names=mimic_names,
+                multipliers=multipliers,
+                offsets=offsets,
+            )
+            optimizer.set_kinematic_adaptor(adaptor)
+            print(
+                "\033[34m",
+                "Mimic joint adaptor enabled. The mimic joint tags in the URDF will be considered during retargeting.\n"
+                "To disable mimic joint adaptor, consider setting ignore_mimic_joint=True in the configuration.",
+                "\033[39m",
+            )
+
         retargeting = SeqRetargeting(
             optimizer,
             has_joint_limits=self.has_joint_limits,
             lp_filter=lp_filter,
         )
-        # TODO: hack here for SAPIEN
-        retargeting.scene = sapien_model.scene
         return retargeting
 
 
 def get_retargeting_config(config_path) -> RetargetingConfig:
     config = RetargetingConfig.load_from_file(config_path)
     return config
 
 
+def parse_mimic_joint(robot_urdf: urdf.URDF) -> Tuple[bool, List[str], List[str], List[float], List[float]]:
+    mimic_joint_names = []
+    source_joint_names = []
+    multipliers = []
+    offsets = []
+    for name, joint in robot_urdf.joint_map.items():
+        if joint.mimic is not None:
+            mimic_joint_names.append(name)
+            source_joint_names.append(joint.mimic.joint)
+            multipliers.append(joint.mimic.multiplier)
+            offsets.append(joint.mimic.offset)
+
+    return len(mimic_joint_names) > 0, source_joint_names, mimic_joint_names, multipliers, offsets
+
+
 if __name__ == "__main__":
     # Path below is relative to this file
 
     test_config = get_retargeting_config(str(Path(__file__).parent / "configs/allegro_hand.yml"))
     print(test_config)
     opt = test_config.build()
     print(opt.optimizer.target_link_human_indices)
```

## dex_retargeting/seq_retarget.py

```diff
@@ -1,12 +1,12 @@
 from time import time
 from typing import Optional
 
 import numpy as np
-import transforms3d
+from pytransform3d import rotations
 
 from dex_retargeting.optimizer import Optimizer
 from dex_retargeting.optimizer_utils import LPFilter
 
 
 class SeqRetargeting:
     def __init__(
@@ -16,90 +16,91 @@
         lp_filter: Optional[LPFilter] = None,
     ):
         self.optimizer = optimizer
         robot = self.optimizer.robot
 
         # Joint limit
         self.has_joint_limits = has_joint_limits
-        joint_limits = np.ones_like(robot.get_qlimits())
+        joint_limits = np.ones_like(robot.joint_limits)
         joint_limits[:, 0] = -1e4  # a large value is equivalent to no limit
         joint_limits[:, 1] = 1e4
         if has_joint_limits:
-            joint_limits[:] = robot.get_qlimits()[:]
-            self.optimizer.set_joint_limit(joint_limits[self.optimizer.target_joint_indices])
+            joint_limits[:] = robot.joint_limits[:]
+            self.optimizer.set_joint_limit(joint_limits[self.optimizer.idx_pin2target])
         self.joint_limits = joint_limits
 
         # Temporal information
-        self.last_qpos = joint_limits.mean(1)[self.optimizer.target_joint_indices]
+        self.last_qpos = joint_limits.mean(1)[self.optimizer.idx_pin2target]
         self.accumulated_time = 0
         self.num_retargeting = 0
 
         # Filter
         self.filter = lp_filter
 
         # Warm started
         self.is_warm_started = False
 
         # TODO: hack here
         self.scene = None
 
     def warm_start(self, wrist_pos: np.ndarray, wrist_orientation: np.ndarray, global_rot: np.array):
+        """
+        Initialize the wrist joint pose using analytical computation instead of retargeting optimization.
+        This function is specifically for position retargeting with the flying robot hand, i.e. has 6D free joint
+        You are not expected to use this function for vector retargeting, e.g. when you are working on teleoperation
+        Args:
+            wrist_pos: position of the hand wrist, typically from human hand pose
+            wrist_orientation: orientation of the hand orientation, typically from human hand pose in MANO convention
+            global_rot:
+
+        Returns:
+
+        """
         # This function can only be used when the first joints of robot are free joints
         if len(wrist_pos) != 3:
             raise ValueError(f"Wrist pos:{wrist_pos} is not a 3-dim vector.")
         if len(wrist_orientation) != 3:
             raise ValueError(f"Wrist orientation:{wrist_orientation} is not a 3-dim vector.")
 
         if np.linalg.norm(wrist_orientation) < 1e-3:
             mat = np.eye(3)
         else:
-            angle = np.linalg.norm(wrist_orientation)
-            axis = wrist_orientation / angle
-            mat = transforms3d.axangles.axangle2mat(axis, angle)
-            print(transforms3d.quaternions.axangle2quat(axis, angle))
+            mat = rotations.matrix_from_compact_axis_angle(wrist_orientation)
 
         robot = self.optimizer.robot
         operator2mano = np.array([[0, 0, -1], [-1, 0, 0], [0, 1, 0]])
         mat = global_rot.T @ mat @ operator2mano
         target_wrist_pose = np.eye(4)
         target_wrist_pose[:3, :3] = mat
         target_wrist_pose[:3, 3] = wrist_pos
 
         wrist_link_name = self.optimizer.wrist_link_name
-        wrist_link = [link for link in self.optimizer.robot.get_links() if link.get_name() == wrist_link_name][0]
+        wrist_link_id = self.optimizer.robot.get_link_index(wrist_link_name)
         name_list = [
             "dummy_x_translation_joint",
             "dummy_y_translation_joint",
             "dummy_z_translation_joint",
             "dummy_x_rotation_joint",
             "dummy_y_rotation_joint",
             "dummy_z_rotation_joint",
         ]
-        old_qpos = robot.get_qpos()
+        old_qpos = robot.q0
         new_qpos = old_qpos.copy()
         for num, joint_name in enumerate(self.optimizer.target_joint_names):
             if joint_name in name_list:
                 new_qpos[num] = 0
-        robot.set_qpos(new_qpos)
-        root2wrist = (robot.get_pose().inv() * wrist_link.get_pose()).inv().to_transformation_matrix()
+
+        robot.compute_forward_kinematics(new_qpos)
+        root2wrist = robot.get_link_pose_inv(wrist_link_id)
         target_root_pose = target_wrist_pose @ root2wrist
-        robot.set_qpos(old_qpos)
 
-        euler = transforms3d.euler.mat2euler(target_root_pose[:3, :3], "rxyz")
+        euler = rotations.euler_from_matrix(target_root_pose[:3, :3], 0, 1, 2, extrinsic=False)
         pose_vec = np.concatenate([target_root_pose[:3, 3], euler])
 
         # Find the dummy joints
-        name_list = [
-            "dummy_x_translation_joint",
-            "dummy_y_translation_joint",
-            "dummy_z_translation_joint",
-            "dummy_x_rotation_joint",
-            "dummy_y_rotation_joint",
-            "dummy_z_rotation_joint",
-        ]
         for num, joint_name in enumerate(self.optimizer.target_joint_names):
             if joint_name in name_list:
                 index = name_list.index(joint_name)
                 self.last_qpos[num] = pose_vec[index]
 
         self.is_warm_started = True
 
@@ -110,21 +111,21 @@
             fixed_qpos=fixed_qpos.astype(np.float32),
             last_qpos=self.last_qpos.astype(np.float32),
         )
         self.accumulated_time += time() - tic
         self.num_retargeting += 1
         self.last_qpos = qpos
         robot_qpos = np.zeros(self.optimizer.robot.dof)
-        robot_qpos[self.optimizer.fixed_joint_indices] = fixed_qpos
-        robot_qpos[self.optimizer.target_joint_indices] = qpos
+        robot_qpos[self.optimizer.idx_pin2fixed] = fixed_qpos
+        robot_qpos[self.optimizer.idx_pin2target] = qpos
         if self.filter is not None:
             robot_qpos = self.filter.next(robot_qpos)
         return robot_qpos
 
     def verbose(self):
         min_value = self.optimizer.opt.last_optimum_value()
         print(f"Retargeting {self.num_retargeting} times takes: {self.accumulated_time}s")
         print(f"Last distance: {min_value}")
 
     def reset(self):
-        self.last_qpos = self.joint_limits.mean(1)[self.optimizer.target_joint_indices]
+        self.last_qpos = self.joint_limits.mean(1)[self.optimizer.idx_pin2target]
         self.num_retargeting = 0
```

## dex_retargeting/yourdfpy.py

```diff
@@ -1006,15 +1006,15 @@
                     f"Joint '{joint.name}' is supposed to mimic '{joint.mimic.joint}'. But this joint is not actuated - will assume (0.0 + offset)."
                 )
                 q = 0.0 + joint.mimic.offset
 
         if joint.type in ["revolute", "prismatic", "continuous"]:
             if q is None:
                 # Use internal cfg vector for forward kinematics
-                q = self.cfg[self.actuated_dof_indices[self.actuated_joint_names.index(joint.name)]]
+                q = float(self.cfg[self.actuated_dof_indices[self.actuated_joint_names.index(joint.name)]])
 
             if joint.type == "prismatic":
                 matrix = origin @ tra.translation_matrix(q * joint.axis)
             else:
                 matrix = origin @ tra.rotation_matrix(q, joint.axis)
         else:
             # this includes: floating, planar, fixed
```

## Comparing `dex_retargeting-0.1.1.dist-info/LICENSE` & `dex_retargeting-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dex_retargeting-0.1.1.dist-info/METADATA` & `dex_retargeting-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dex_retargeting
-Version: 0.1.1
+Version: 0.2.0
 Summary: Hand pose retargeting for dexterous robot hand.
 Home-page: https://github.com/dexsuite/dex-retargeting
 Author: Yuzhe Qin
 Author-email: y1qin@ucsd.edu
 Maintainer: Yuzhe Qin
 Maintainer-email: y1qin@ucsd.edu
 License: MIT
@@ -18,35 +18,37 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy <1.24
-Requires-Dist: torch
-Requires-Dist: sapien >=2.0.0
+Requires-Dist: numpy
+Requires-Dist: pytransform3d
+Requires-Dist: pin >=2.7.0
 Requires-Dist: nlopt
 Requires-Dist: trimesh
 Requires-Dist: anytree
-Requires-Dist: pycollada
 Requires-Dist: pyyaml
 Requires-Dist: lxml
+Requires-Dist: torch
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: pytest-xdist ; extra == 'dev'
 Requires-Dist: pyright ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
+Requires-Dist: mypy ; extra == 'dev'
 Provides-Extra: example
 Requires-Dist: tyro ; extra == 'example'
 Requires-Dist: tqdm ; extra == 'example'
 Requires-Dist: opencv-python ; extra == 'example'
 Requires-Dist: mediapipe ; extra == 'example'
+Requires-Dist: sapien <3.0 ; extra == 'example'
 
 Dex Retargeting
 ---
 <p align="center">
     <!-- code check badges -->
     <a href='https://github.com/dexsuite/dex-retargeting/blob/main/.github/workflows/test.yml'>
         <img src='https://github.com/dexsuite/dex-retargeting/actions/workflows/test.yml/badge.svg' alt='Test Status' />
```

### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: dex_retargeting Version: 0.1.1 Summary: Hand pose
+Metadata-Version: 2.1 Name: dex_retargeting Version: 0.2.0 Summary: Hand pose
 retargeting for dexterous robot hand. Home-page: https://github.com/dexsuite/
 dex-retargeting Author: Yuzhe Qin Author-email: y1qin@ucsd.edu Maintainer:
 Yuzhe Qin Maintainer-email: y1qin@ucsd.edu License: MIT Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7,<3.11 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: numpy <1.24 Requires-Dist: torch Requires-Dist:
-sapien >=2.0.0 Requires-Dist: nlopt Requires-Dist: trimesh Requires-Dist:
-anytree Requires-Dist: pycollada Requires-Dist: pyyaml Requires-Dist: lxml
-Provides-Extra: dev Requires-Dist: pytest ; extra == 'dev' Requires-Dist: black
-; extra == 'dev' Requires-Dist: isort ; extra == 'dev' Requires-Dist: pytest-
-xdist ; extra == 'dev' Requires-Dist: pyright ; extra == 'dev' Requires-Dist:
-ruff ; extra == 'dev' Provides-Extra: example Requires-Dist: tyro ; extra ==
-'example' Requires-Dist: tqdm ; extra == 'example' Requires-Dist: opencv-python
-; extra == 'example' Requires-Dist: mediapipe ; extra == 'example' Dex
+File: LICENSE Requires-Dist: numpy Requires-Dist: pytransform3d Requires-Dist:
+pin >=2.7.0 Requires-Dist: nlopt Requires-Dist: trimesh Requires-Dist: anytree
+Requires-Dist: pyyaml Requires-Dist: lxml Requires-Dist: torch Provides-Extra:
+dev Requires-Dist: pytest ; extra == 'dev' Requires-Dist: black ; extra ==
+'dev' Requires-Dist: isort ; extra == 'dev' Requires-Dist: pytest-xdist ; extra
+== 'dev' Requires-Dist: pyright ; extra == 'dev' Requires-Dist: ruff ; extra ==
+'dev' Requires-Dist: mypy ; extra == 'dev' Provides-Extra: example Requires-
+Dist: tyro ; extra == 'example' Requires-Dist: tqdm ; extra == 'example'
+Requires-Dist: opencv-python ; extra == 'example' Requires-Dist: mediapipe ;
+extra == 'example' Requires-Dist: sapien <3.0 ; extra == 'example' Dex
 Retargeting ---
                             _[_T_e_s_t_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
 ## Installation ```shell pip3 install -e ".[example]" # If you do not need to
 run the examples: # pip install -e . ``` ## Examples ### Retargeting from human
 hand video [Tutorial on retargeting from human hand video](example/
 vector_retargeting/README.md) ### Retarget from hand object pose dataset
 [Tutorial on retargeting from hand-object pose dataset](example/
```

## Comparing `dex_retargeting-0.1.1.dist-info/RECORD` & `dex_retargeting-0.2.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-dex_retargeting/__init__.py,sha256=rnObPjuBcEStqSO0S6gsdS_ot8ITOQjVj_-P1LUUYpg,22
+dex_retargeting/__init__.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
 dex_retargeting/constants.py,sha256=TEdIWoqI3pE3YDYqlBDQZkyTomm0A0qC1CwwK7DIU_E,1439
-dex_retargeting/optimizer.py,sha256=nkLX2HmGq-CLDkHasdsq0r9RJ2ivlPfwVyaDqsw1shs,22367
-dex_retargeting/optimizer_utils.py,sha256=3nqCjzMgOIPgWj6Ue3mcp2ympAiP5lJER1d1THT9v5s,4185
-dex_retargeting/retargeting_config.py,sha256=7_EEiJMMdaU4jDvtn23-h3ySr72_gLVcsZPPgXTrAlM,8562
-dex_retargeting/seq_retarget.py,sha256=S5r_Q95zF4ISyZJ3LAALwnCq2e-mjxN1tZxrojaUDG0,4952
-dex_retargeting/yourdfpy.py,sha256=zi0M2ALNw6-yeXESlmo_qHeptxF09my4R-Or_CSwJPc,76137
-dex_retargeting-0.1.1.dist-info/LICENSE,sha256=n-mi0aBrkdsTe19Q7k45FLC4wd9SO4G90KnZMOHOYQY,1075
-dex_retargeting-0.1.1.dist-info/METADATA,sha256=DNfYprOPebX_E80ZGSn6bjDE6li5E61JZ_u8A9DE49U,2494
-dex_retargeting-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dex_retargeting-0.1.1.dist-info/top_level.txt,sha256=k7-L97sLJXIYlYjDd-WHSRlfhjc9JF5K3Kk-zbfjjfw,16
-dex_retargeting-0.1.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-dex_retargeting-0.1.1.dist-info/RECORD,,
+dex_retargeting/kinematics_adaptor.py,sha256=O6waE4aXJ3LiUXlolIrKI38KO2DEnYPik_IZVuXQha0,3940
+dex_retargeting/optimizer.py,sha256=os5XRaNmtdUmD-HCTHIkpkqcltGAfXRX1Py7qBxEF8Y,20369
+dex_retargeting/optimizer_utils.py,sha256=qG928BVOqKE1aRhqZo6oGgiGCBlZlEhbBqD1vOL-Jvs,420
+dex_retargeting/retargeting_config.py,sha256=vNpWnvI-2Ja7Hru0EQkYSfKSjeje-eiHxgBmZWjsU8Q,9668
+dex_retargeting/robot_wrapper.py,sha256=Z6ePK3UQkrm5O5vlylNhgHVC5L3gubdshrnscbmy0Bg,2791
+dex_retargeting/seq_retarget.py,sha256=tM0kcmG1PtYuqyPJuBRSWcjvnDToczTOGuQAN4G7TzA,5044
+dex_retargeting/yourdfpy.py,sha256=h6JfnatR7kVgnG-iduQ8CB_gGPSYyiGKm5VO5CcVHiY,76144
+dex_retargeting-0.2.0.dist-info/LICENSE,sha256=n-mi0aBrkdsTe19Q7k45FLC4wd9SO4G90KnZMOHOYQY,1075
+dex_retargeting-0.2.0.dist-info/METADATA,sha256=snSQcpznFb_5LCV3XILzUvhi1rNnviwcbsx1NU5mn28,2574
+dex_retargeting-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dex_retargeting-0.2.0.dist-info/top_level.txt,sha256=k7-L97sLJXIYlYjDd-WHSRlfhjc9JF5K3Kk-zbfjjfw,16
+dex_retargeting-0.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+dex_retargeting-0.2.0.dist-info/RECORD,,
```

