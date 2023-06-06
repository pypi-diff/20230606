# Comparing `tmp/rl_games_y-0.0.1.tar.gz` & `tmp/rl_games_y-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_games_y-0.0.1.tar", max compression
+gzip compressed data, was "rl_games_y-0.0.2.tar", max compression
```

## Comparing `rl_games_y-0.0.1.tar` & `rl_games_y-0.0.2.tar`

### file list

```diff
@@ -1,208 +1,204 @@
--rw-r--r--   0        0        0     1068 2023-06-06 12:36:05.369197 rl_games_y-0.0.1/LICENSE
--rw-r--r--   0        0        0      104 2023-06-06 12:31:25.308716 rl_games_y-0.0.1/README.md
--rw-r--r--   0        0        0     1126 2023-06-06 13:03:58.916389 rl_games_y-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/HEAD
--rw-r--r--   0        0        0      264 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/config
--rw-r--r--   0        0        0       73 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/description
--rwxr-xr-x   0        0        0      478 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     3079 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1638 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1348 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     3610 2023-06-06 12:22:19.330646 rl_games_y-0.0.1/rl_games/.git/hooks/update.sample
--rw-r--r--   0        0        0    17950 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/index
--rw-r--r--   0        0        0      240 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/info/exclude
--rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/logs/HEAD
--rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/logs/refs/heads/master
--rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0    11936 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx
--rw-r--r--   0        0        0   210728 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack
--rw-r--r--   0        0        0      247 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/packed-refs
--rw-r--r--   0        0        0       41 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/refs/heads/master
--rw-r--r--   0        0        0       32 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.git/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0     1289 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/.gitignore
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/__init__.py
--rw-r--r--   0        0        0     8605 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/a2c_continuous.py
--rw-r--r--   0        0        0     7125 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/a2c_discrete.py
--rw-r--r--   0        0        0    10679 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/central_value.py
--rw-r--r--   0        0        0     1259 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/d2rl.py
--rw-r--r--   0        0        0    10830 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/flatten.py
--rw-r--r--   0        0        0     4148 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/layers.py
--rw-r--r--   0        0        0     2886 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/model_builder.py
--rw-r--r--   0        0        0    13507 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/models.py
--rw-r--r--   0        0        0     2729 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/moving_mean_std.py
--rw-r--r--   0        0        0    58864 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/network_builder.py
--rw-r--r--   0        0        0     8728 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/players.py
--rw-r--r--   0        0        0     4111 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/running_mean_std.py
--rw-r--r--   0        0        0    23967 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/sac_agent.py
--rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/sac_helper.py
--rw-r--r--   0        0        0     1332 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/self_play_manager.py
--rw-r--r--   0        0        0    12758 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/algos_torch/torch_ext.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/__init__.py
--rw-r--r--   0        0        0    55205 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/a2c_common.py
--rw-r--r--   0        0        0     5456 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/algo_observer.py
--rw-r--r--   0        0        0     1977 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/categorical.py
--rw-r--r--   0        0        0     2255 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/common_losses.py
--rw-r--r--   0        0        0     3396 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/datasets.py
--rw-r--r--   0        0        0     2284 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/diagnostics.py
--rw-r--r--   0        0        0      680 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/divergence.py
--rw-r--r--   0        0        0    15196 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/env_configurations.py
--rw-r--r--   0        0        0    17184 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/experience.py
--rw-r--r--   0        0        0     2440 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/experiment.py
--rw-r--r--   0        0        0     2750 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/interval_summary_writer.py
--rw-r--r--   0        0        0      945 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/ivecenv.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/layers/__init__.py
--rw-r--r--   0        0        0     2763 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/layers/recurrent.py
--rw-r--r--   0        0        0      414 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/object_factory.py
--rw-r--r--   0        0        0    10863 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/player.py
--rw-r--r--   0        0        0      382 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/rollouts.py
--rw-r--r--   0        0        0     1948 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/schedulers.py
--rw-r--r--   0        0        0     4888 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/segment_tree.py
--rw-r--r--   0        0        0     2260 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/tr_helpers.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/transforms/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/transforms/soft_augmentation.py
--rw-r--r--   0        0        0      746 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/transforms/transforms.py
--rw-r--r--   0        0        0     8191 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/vecenv.py
--rw-r--r--   0        0        0    23776 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/common/wrappers.py
--rw-r--r--   0        0        0     1606 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout.yaml
--rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_envpool.yaml
--rw-r--r--   0        0        0     1468 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml
--rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_torch_impala.yaml
--rw-r--r--   0        0        0     1607 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_gopher.yaml
--rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_invaders_envpool.yaml
--rw-r--r--   0        0        0     1834 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml
--rw-r--r--   0        0        0     1730 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool.yaml
--rw-r--r--   0        0        0     1518 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml
--rw-r--r--   0        0        0     1841 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml
--rw-r--r--   0        0        0     1619 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_torch.yaml
--rw-r--r--   0        0        0     1729 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml
--rw-r--r--   0        0        0     1650 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong.yaml
--rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong_envpool.yaml
--rw-r--r--   0        0        0     1434 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml
--rw-r--r--   0        0        0     1334 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_space_invaders_resnet.yaml
--rw-r--r--   0        0        0     1640 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/atari/ppo_space_invaders_torch.yaml
--rw-r--r--   0        0        0     1315 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_ant.yaml
--rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_ant_tcnn.yaml
--rw-r--r--   0        0        0     1264 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_grasp.yaml
--rw-r--r--   0        0        0     1273 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_halfcheetah.yaml
--rw-r--r--   0        0        0     1344 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_humanoid.yaml
--rw-r--r--   0        0        0     1260 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/ppo_ur5e.yaml
--rw-r--r--   0        0        0      902 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/sac_ant.yaml
--rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/brax/sac_humanoid.yaml
--rw-r--r--   0        0        0     1651 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/carracing_ppo.yaml
--rw-r--r--   0        0        0     1129 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/cartpole.yaml
--rw-r--r--   0        0        0     1339 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/fish_swim.yaml
--rw-r--r--   0        0        0     1134 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/halfcheetah_run.yaml
--rw-r--r--   0        0        0     1189 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/humanoid2.yaml
--rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/humanoid_run.yaml
--rw-r--r--   0        0        0      863 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/sac_humanoid.yaml
--rw-r--r--   0        0        0     1239 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/walker_run.yaml
--rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/walker_stand.yaml
--rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/dm_control/walker_walk.yaml
--rw-r--r--   0        0        0     1660 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ma/ppo_connect4_self_play.yaml
--rw-r--r--   0        0        0      978 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml
--rw-r--r--   0        0        0     1221 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ma/ppo_slime_self_play.yaml
--rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ma/ppo_slime_v0.yaml
--rw-r--r--   0        0        0     1744 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/minigrid/lava_rnn_img.yaml
--rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/minigrid/minigrid_rnn_img.yaml
--rw-r--r--   0        0        0     1209 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/ant.yaml
--rw-r--r--   0        0        0     1245 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/ant_envpool.yaml
--rw-r--r--   0        0        0     1276 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/halfcheetah.yaml
--rw-r--r--   0        0        0     1351 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/halfcheetah_envpool.yaml
--rw-r--r--   0        0        0     1242 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/hopper.yaml
--rw-r--r--   0        0        0     1268 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/hopper_envpool.yaml
--rw-r--r--   0        0        0     1290 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/humanoid.yaml
--rw-r--r--   0        0        0     1279 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/humanoid_envpool.yaml
--rw-r--r--   0        0        0      828 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/sac_ant_envpool.yaml
--rw-r--r--   0        0        0      913 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml
--rw-r--r--   0        0        0     1196 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/walker2d.yaml
--rw-r--r--   0        0        0     1228 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/mujoco/walker2d_envpool.yaml
--rw-r--r--   0        0        0     1223 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_ant.yaml
--rw-r--r--   0        0        0     1266 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_hand.yaml
--rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_humanoid.yaml
--rw-r--r--   0        0        0      907 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_cartpole.yaml
--rw-r--r--   0        0        0     1103 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml
--rw-r--r--   0        0        0     1251 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_continuous.yaml
--rw-r--r--   0        0        0     1190 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_continuous_lstm.yaml
--rw-r--r--   0        0        0     1234 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_lunar.yaml
--rw-r--r--   0        0        0     1178 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_lunar_continiuos_torch.yaml
--rw-r--r--   0        0        0      868 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_lunar_discrete.yaml
--rw-r--r--   0        0        0     1723 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_multiwalker.yaml
--rw-r--r--   0        0        0     1159 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_pendulum.yaml
--rw-r--r--   0        0        0     1128 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_pendulum_torch.yaml
--rw-r--r--   0        0        0     1508 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_reacher.yaml
--rw-r--r--   0        0        0      905 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_smac.yaml
--rw-r--r--   0        0        0     1303 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_walker.yaml
--rw-r--r--   0        0        0     1258 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_walker_hardcore.yaml
--rw-r--r--   0        0        0     1483 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_walker_rnn.yaml
--rw-r--r--   0        0        0     1081 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/ppo_walker_tcnn.yaml
--rw-r--r--   0        0        0     1219 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/procgen/ppo_coinrun.yaml
--rw-r--r--   0        0        0     1379 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/10m_vs_11m_torch.yaml
--rw-r--r--   0        0        0     1709 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/27m_vs_30m_cv.yaml
--rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/27m_vs_30m_torch.yaml
--rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/2m_vs_1z.yaml
--rw-r--r--   0        0        0      910 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/2m_vs_1z_torch.yaml
--rw-r--r--   0        0        0      966 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/2s_vs_1c.yaml
--rw-r--r--   0        0        0     1443 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_cnn_torch.yaml
--rw-r--r--   0        0        0      956 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch.yaml
--rw-r--r--   0        0        0     1470 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv.yaml
--rw-r--r--   0        0        0     1644 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv_joint.yaml
--rw-r--r--   0        0        0     1647 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv_rnn.yaml
--rw-r--r--   0        0        0     1037 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_rnn.yaml
--rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_sparse.yaml
--rw-r--r--   0        0        0     1516 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml
--rw-r--r--   0        0        0     1520 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml
--rw-r--r--   0        0        0      961 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_4z.yaml
--rw-r--r--   0        0        0      970 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z.yaml
--rw-r--r--   0        0        0     1473 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_cv.yaml
--rw-r--r--   0        0        0     1681 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml
--rw-r--r--   0        0        0     1047 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml
--rw-r--r--   0        0        0     1022 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml
--rw-r--r--   0        0        0     1287 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_rnn.yaml
--rw-r--r--   0        0        0     1883 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml
--rw-r--r--   0        0        0     1437 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_torch.yaml
--rw-r--r--   0        0        0     1043 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/6h_vs_8z_torch.yaml
--rw-r--r--   0        0        0     1669 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml
--rw-r--r--   0        0        0      993 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/8m_torch.yaml
--rw-r--r--   0        0        0     1509 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/8m_torch_cv.yaml
--rw-r--r--   0        0        0     1457 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/MMM2_torch.yaml
--rw-r--r--   0        0        0     1456 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/corridor_torch.yaml
--rw-r--r--   0        0        0     1515 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/smac/corridor_torch_cv.yaml
--rw-r--r--   0        0        0     1965 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_continuous.yaml
--rw-r--r--   0        0        0     1712 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete.yaml
--rw-r--r--   0        0        0     1873 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml
--rw-r--r--   0        0        0     1401 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml
--rw-r--r--   0        0        0     1146 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_discrete.yaml
--rw-r--r--   0        0        0     1162 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml
--rw-r--r--   0        0        0     1301 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_ppo_walker_truncated_time.yaml
--rw-r--r--   0        0        0     1205 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_rnn.yaml
--rw-r--r--   0        0        0     1829 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_rnn_multidiscrete.yaml
--rw-r--r--   0        0        0     1325 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/distributed/__init__.py
--rw-r--r--   0        0        0      281 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/__init__.py
--rw-r--r--   0        0        0     1941 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/brax.py
--rw-r--r--   0        0        0     2992 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/connect4_network.py
--rw-r--r--   0        0        0     4505 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/connect4_selfplay.py
--rw-r--r--   0        0        0     3496 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/diambra/diambra.py
--rw-r--r--   0        0        0     3116 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/envpool.py
--rw-r--r--   0        0        0     3195 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/multiwalker.py
--rw-r--r--   0        0        0     2148 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/slimevolley_selfplay.py
--rw-r--r--   0        0        0     3690 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/smac_env.py
--rw-r--r--   0        0        0      279 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/test/__init__.py
--rw-r--r--   0        0        0      779 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/test/example_env.py
--rw-r--r--   0        0        0     5217 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/test/rnn_env.py
--rw-r--r--   0        0        0     1715 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/test/test_asymmetric_env.py
--rw-r--r--   0        0        0     1596 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/envs/test_network.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/interfaces/__init__.py
--rw-r--r--   0        0        0      674 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/interfaces/base_algorithm.py
--rw-r--r--   0        0        0      159 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/networks/__init__.py
--rw-r--r--   0        0        0     1463 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/networks/tcnn_mlp.py
--rw-r--r--   0        0        0     4860 2023-06-06 12:22:19.334646 rl_games_y-0.0.1/rl_games/torch_runner.py
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 rl_games_y-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-06 12:36:05.369197 rl_games_y-0.0.2/LICENSE
+-rw-r--r--   0        0        0      104 2023-06-06 12:31:25.308716 rl_games_y-0.0.2/README.md
+-rw-r--r--   0        0        0     1126 2023-06-06 15:38:02.228217 rl_games_y-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/HEAD
+-rw-r--r--   0        0        0      264 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/config
+-rw-r--r--   0        0        0       73 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     3079 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1638 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1348 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     3610 2023-06-06 12:22:19.330646 rl_games_y-0.0.2/rl_games/.git/hooks/update.sample
+-rw-r--r--   0        0        0    17950 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/index
+-rw-r--r--   0        0        0      240 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/info/exclude
+-rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/logs/HEAD
+-rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/logs/refs/heads/master
+-rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0    11936 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx
+-rw-r--r--   0        0        0   210728 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack
+-rw-r--r--   0        0        0      247 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/packed-refs
+-rw-r--r--   0        0        0       41 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/refs/heads/master
+-rw-r--r--   0        0        0       32 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/__init__.py
+-rw-r--r--   0        0        0     8605 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/a2c_continuous.py
+-rw-r--r--   0        0        0     7125 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/a2c_discrete.py
+-rw-r--r--   0        0        0    10679 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/central_value.py
+-rw-r--r--   0        0        0     1259 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/d2rl.py
+-rw-r--r--   0        0        0    10830 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/flatten.py
+-rw-r--r--   0        0        0     4148 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/layers.py
+-rw-r--r--   0        0        0     2886 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/model_builder.py
+-rw-r--r--   0        0        0    13507 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/models.py
+-rw-r--r--   0        0        0     2729 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/moving_mean_std.py
+-rw-r--r--   0        0        0    58864 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/network_builder.py
+-rw-r--r--   0        0        0     8728 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/players.py
+-rw-r--r--   0        0        0     4111 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/running_mean_std.py
+-rw-r--r--   0        0        0    23967 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/sac_agent.py
+-rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/sac_helper.py
+-rw-r--r--   0        0        0     1332 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/self_play_manager.py
+-rw-r--r--   0        0        0    12758 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/algos_torch/torch_ext.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/__init__.py
+-rw-r--r--   0        0        0    55205 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/a2c_common.py
+-rw-r--r--   0        0        0     5456 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/algo_observer.py
+-rw-r--r--   0        0        0     1977 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/categorical.py
+-rw-r--r--   0        0        0     2255 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/common_losses.py
+-rw-r--r--   0        0        0     3396 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/datasets.py
+-rw-r--r--   0        0        0     2284 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/diagnostics.py
+-rw-r--r--   0        0        0      680 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/divergence.py
+-rw-r--r--   0        0        0    15196 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/env_configurations.py
+-rw-r--r--   0        0        0    17184 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/experience.py
+-rw-r--r--   0        0        0     2440 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/experiment.py
+-rw-r--r--   0        0        0     2750 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/interval_summary_writer.py
+-rw-r--r--   0        0        0      945 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/ivecenv.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/layers/__init__.py
+-rw-r--r--   0        0        0     2763 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/layers/recurrent.py
+-rw-r--r--   0        0        0      414 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/object_factory.py
+-rw-r--r--   0        0        0    10863 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/player.py
+-rw-r--r--   0        0        0      382 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/rollouts.py
+-rw-r--r--   0        0        0     1948 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/schedulers.py
+-rw-r--r--   0        0        0     4888 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/segment_tree.py
+-rw-r--r--   0        0        0     2260 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/tr_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/transforms/__init__.py
+-rw-r--r--   0        0        0     1165 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/transforms/soft_augmentation.py
+-rw-r--r--   0        0        0      746 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/transforms/transforms.py
+-rw-r--r--   0        0        0     8191 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/vecenv.py
+-rw-r--r--   0        0        0    23776 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/common/wrappers.py
+-rw-r--r--   0        0        0     1606 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout.yaml
+-rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_envpool.yaml
+-rw-r--r--   0        0        0     1468 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_torch_impala.yaml
+-rw-r--r--   0        0        0     1607 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_gopher.yaml
+-rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_invaders_envpool.yaml
+-rw-r--r--   0        0        0     1834 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml
+-rw-r--r--   0        0        0     1730 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool.yaml
+-rw-r--r--   0        0        0     1518 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1841 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml
+-rw-r--r--   0        0        0     1619 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_torch.yaml
+-rw-r--r--   0        0        0     1729 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml
+-rw-r--r--   0        0        0     1650 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong.yaml
+-rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong_envpool.yaml
+-rw-r--r--   0        0        0     1434 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1334 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_space_invaders_resnet.yaml
+-rw-r--r--   0        0        0     1640 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/atari/ppo_space_invaders_torch.yaml
+-rw-r--r--   0        0        0     1315 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_ant.yaml
+-rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_ant_tcnn.yaml
+-rw-r--r--   0        0        0     1264 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_grasp.yaml
+-rw-r--r--   0        0        0     1273 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_halfcheetah.yaml
+-rw-r--r--   0        0        0     1344 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_humanoid.yaml
+-rw-r--r--   0        0        0     1260 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/ppo_ur5e.yaml
+-rw-r--r--   0        0        0      902 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/sac_ant.yaml
+-rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/brax/sac_humanoid.yaml
+-rw-r--r--   0        0        0     1651 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/carracing_ppo.yaml
+-rw-r--r--   0        0        0     1129 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/cartpole.yaml
+-rw-r--r--   0        0        0     1339 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/fish_swim.yaml
+-rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/humanoid_run.yaml
+-rw-r--r--   0        0        0     1239 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/walker_run.yaml
+-rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/walker_stand.yaml
+-rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/dm_control/walker_walk.yaml
+-rw-r--r--   0        0        0     1660 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ma/ppo_connect4_self_play.yaml
+-rw-r--r--   0        0        0      978 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml
+-rw-r--r--   0        0        0     1221 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ma/ppo_slime_self_play.yaml
+-rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ma/ppo_slime_v0.yaml
+-rw-r--r--   0        0        0     1744 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/minigrid/lava_rnn_img.yaml
+-rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/minigrid/minigrid_rnn_img.yaml
+-rw-r--r--   0        0        0     1209 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/ant.yaml
+-rw-r--r--   0        0        0     1245 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/ant_envpool.yaml
+-rw-r--r--   0        0        0     1276 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/halfcheetah.yaml
+-rw-r--r--   0        0        0     1351 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/halfcheetah_envpool.yaml
+-rw-r--r--   0        0        0     1242 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/hopper.yaml
+-rw-r--r--   0        0        0     1268 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/hopper_envpool.yaml
+-rw-r--r--   0        0        0     1290 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/humanoid.yaml
+-rw-r--r--   0        0        0     1279 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/humanoid_envpool.yaml
+-rw-r--r--   0        0        0      828 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/sac_ant_envpool.yaml
+-rw-r--r--   0        0        0      913 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml
+-rw-r--r--   0        0        0     1196 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/walker2d.yaml
+-rw-r--r--   0        0        0     1228 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/mujoco/walker2d_envpool.yaml
+-rw-r--r--   0        0        0     1223 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_ant.yaml
+-rw-r--r--   0        0        0     1266 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_hand.yaml
+-rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_humanoid.yaml
+-rw-r--r--   0        0        0      907 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_cartpole.yaml
+-rw-r--r--   0        0        0     1103 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml
+-rw-r--r--   0        0        0     1251 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_continuous.yaml
+-rw-r--r--   0        0        0     1190 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_continuous_lstm.yaml
+-rw-r--r--   0        0        0     1234 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_lunar.yaml
+-rw-r--r--   0        0        0     1178 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_lunar_continiuos_torch.yaml
+-rw-r--r--   0        0        0      868 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_lunar_discrete.yaml
+-rw-r--r--   0        0        0     1723 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_multiwalker.yaml
+-rw-r--r--   0        0        0     1159 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_pendulum.yaml
+-rw-r--r--   0        0        0     1128 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_pendulum_torch.yaml
+-rw-r--r--   0        0        0     1508 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_reacher.yaml
+-rw-r--r--   0        0        0      905 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_smac.yaml
+-rw-r--r--   0        0        0     1303 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_walker.yaml
+-rw-r--r--   0        0        0     1258 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_walker_hardcore.yaml
+-rw-r--r--   0        0        0     1483 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_walker_rnn.yaml
+-rw-r--r--   0        0        0     1081 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/ppo_walker_tcnn.yaml
+-rw-r--r--   0        0        0     1219 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/procgen/ppo_coinrun.yaml
+-rw-r--r--   0        0        0     1379 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/10m_vs_11m_torch.yaml
+-rw-r--r--   0        0        0     1709 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/27m_vs_30m_cv.yaml
+-rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/27m_vs_30m_torch.yaml
+-rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/2m_vs_1z.yaml
+-rw-r--r--   0        0        0      910 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/2m_vs_1z_torch.yaml
+-rw-r--r--   0        0        0      966 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/2s_vs_1c.yaml
+-rw-r--r--   0        0        0     1443 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_cnn_torch.yaml
+-rw-r--r--   0        0        0      956 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch.yaml
+-rw-r--r--   0        0        0     1470 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv.yaml
+-rw-r--r--   0        0        0     1644 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv_joint.yaml
+-rw-r--r--   0        0        0     1647 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv_rnn.yaml
+-rw-r--r--   0        0        0     1037 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_rnn.yaml
+-rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_sparse.yaml
+-rw-r--r--   0        0        0     1516 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml
+-rw-r--r--   0        0        0     1520 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml
+-rw-r--r--   0        0        0      961 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_4z.yaml
+-rw-r--r--   0        0        0      970 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z.yaml
+-rw-r--r--   0        0        0     1473 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_cv.yaml
+-rw-r--r--   0        0        0     1681 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml
+-rw-r--r--   0        0        0     1047 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml
+-rw-r--r--   0        0        0     1022 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml
+-rw-r--r--   0        0        0     1287 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_rnn.yaml
+-rw-r--r--   0        0        0     1883 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml
+-rw-r--r--   0        0        0     1437 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_torch.yaml
+-rw-r--r--   0        0        0     1043 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/6h_vs_8z_torch.yaml
+-rw-r--r--   0        0        0     1669 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml
+-rw-r--r--   0        0        0      993 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/8m_torch.yaml
+-rw-r--r--   0        0        0     1509 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/8m_torch_cv.yaml
+-rw-r--r--   0        0        0     1457 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/MMM2_torch.yaml
+-rw-r--r--   0        0        0     1456 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/corridor_torch.yaml
+-rw-r--r--   0        0        0     1515 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/smac/corridor_torch_cv.yaml
+-rw-r--r--   0        0        0     1965 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_continuous.yaml
+-rw-r--r--   0        0        0     1712 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete.yaml
+-rw-r--r--   0        0        0     1873 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml
+-rw-r--r--   0        0        0     1401 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml
+-rw-r--r--   0        0        0     1146 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_discrete.yaml
+-rw-r--r--   0        0        0     1162 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml
+-rw-r--r--   0        0        0     1301 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_ppo_walker_truncated_time.yaml
+-rw-r--r--   0        0        0     1205 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_rnn.yaml
+-rw-r--r--   0        0        0     1829 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_rnn_multidiscrete.yaml
+-rw-r--r--   0        0        0     1325 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/distributed/__init__.py
+-rw-r--r--   0        0        0      281 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/__init__.py
+-rw-r--r--   0        0        0     1941 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/brax.py
+-rw-r--r--   0        0        0     2992 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/connect4_network.py
+-rw-r--r--   0        0        0     4505 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/connect4_selfplay.py
+-rw-r--r--   0        0        0     3496 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/diambra/diambra.py
+-rw-r--r--   0        0        0     3116 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/envpool.py
+-rw-r--r--   0        0        0     3195 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/multiwalker.py
+-rw-r--r--   0        0        0     2148 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/slimevolley_selfplay.py
+-rw-r--r--   0        0        0     3690 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/smac_env.py
+-rw-r--r--   0        0        0      279 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/test/example_env.py
+-rw-r--r--   0        0        0     5217 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/test/rnn_env.py
+-rw-r--r--   0        0        0     1715 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/test/test_asymmetric_env.py
+-rw-r--r--   0        0        0     1596 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/envs/test_network.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/interfaces/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/interfaces/base_algorithm.py
+-rw-r--r--   0        0        0      159 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/networks/__init__.py
+-rw-r--r--   0        0        0     1463 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/networks/tcnn_mlp.py
+-rw-r--r--   0        0        0     4860 2023-06-06 12:22:19.334646 rl_games_y-0.0.2/rl_games/torch_runner.py
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 rl_games_y-0.0.2/PKG-INFO
```

### Comparing `rl_games_y-0.0.1/LICENSE` & `rl_games_y-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/pyproject.toml` & `rl_games_y-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "rl_games_y"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 readme = "README.md"
 authors = [
     "Denys Makoviichuk <trrrrr97@gmail.com>",
     "Viktor Makoviichuk <victor.makoviychuk@gmail.com>",
     "Shengchao Yan <ysc0505@gmail.com>"
 ]
 packages = [
     {include = "rl_games"},
     {include ="rl_games/**/*.py"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
-gym = {version = "^0.23.0", extras = ["classic_control"]}
+gym = {version = "^0.24.1", extras = ["classic_control"]}
 tensorboard = "^2.8.0"
 tensorboardX = "^2.5"
 PyYAML = "^6.0"
 psutil = "^5.9.0"
 setproctitle = "^1.2.2"
 ray = "^1.11.0"
 opencv-python = "^4.5.5"
```

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/commit-msg.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/fsmonitor-watchman.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/pre-commit.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/pre-push.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/pre-rebase.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/pre-receive.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/prepare-commit-msg.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/hooks/update.sample` & `rl_games_y-0.0.2/rl_games/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/index` & `rl_games_y-0.0.2/rl_games/.git/index`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx` & `rl_games_y-0.0.2/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack` & `rl_games_y-0.0.2/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/a2c_continuous.py` & `rl_games_y-0.0.2/rl_games/algos_torch/a2c_continuous.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/a2c_discrete.py` & `rl_games_y-0.0.2/rl_games/algos_torch/a2c_discrete.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/central_value.py` & `rl_games_y-0.0.2/rl_games/algos_torch/central_value.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/d2rl.py` & `rl_games_y-0.0.2/rl_games/algos_torch/d2rl.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/flatten.py` & `rl_games_y-0.0.2/rl_games/algos_torch/flatten.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/layers.py` & `rl_games_y-0.0.2/rl_games/algos_torch/layers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/model_builder.py` & `rl_games_y-0.0.2/rl_games/algos_torch/model_builder.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/models.py` & `rl_games_y-0.0.2/rl_games/algos_torch/models.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/moving_mean_std.py` & `rl_games_y-0.0.2/rl_games/algos_torch/moving_mean_std.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/network_builder.py` & `rl_games_y-0.0.2/rl_games/algos_torch/network_builder.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/players.py` & `rl_games_y-0.0.2/rl_games/algos_torch/players.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/running_mean_std.py` & `rl_games_y-0.0.2/rl_games/algos_torch/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/sac_agent.py` & `rl_games_y-0.0.2/rl_games/algos_torch/sac_agent.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/sac_helper.py` & `rl_games_y-0.0.2/rl_games/algos_torch/sac_helper.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/self_play_manager.py` & `rl_games_y-0.0.2/rl_games/algos_torch/self_play_manager.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/algos_torch/torch_ext.py` & `rl_games_y-0.0.2/rl_games/algos_torch/torch_ext.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/a2c_common.py` & `rl_games_y-0.0.2/rl_games/common/a2c_common.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/algo_observer.py` & `rl_games_y-0.0.2/rl_games/common/algo_observer.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/categorical.py` & `rl_games_y-0.0.2/rl_games/common/categorical.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/common_losses.py` & `rl_games_y-0.0.2/rl_games/common/common_losses.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/datasets.py` & `rl_games_y-0.0.2/rl_games/common/datasets.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/diagnostics.py` & `rl_games_y-0.0.2/rl_games/common/diagnostics.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/divergence.py` & `rl_games_y-0.0.2/rl_games/common/divergence.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/env_configurations.py` & `rl_games_y-0.0.2/rl_games/common/env_configurations.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/experience.py` & `rl_games_y-0.0.2/rl_games/common/experience.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/experiment.py` & `rl_games_y-0.0.2/rl_games/common/experiment.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/interval_summary_writer.py` & `rl_games_y-0.0.2/rl_games/common/interval_summary_writer.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/ivecenv.py` & `rl_games_y-0.0.2/rl_games/common/ivecenv.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/layers/recurrent.py` & `rl_games_y-0.0.2/rl_games/common/layers/recurrent.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/player.py` & `rl_games_y-0.0.2/rl_games/common/player.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/schedulers.py` & `rl_games_y-0.0.2/rl_games/common/schedulers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/segment_tree.py` & `rl_games_y-0.0.2/rl_games/common/segment_tree.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/tr_helpers.py` & `rl_games_y-0.0.2/rl_games/common/tr_helpers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/transforms/soft_augmentation.py` & `rl_games_y-0.0.2/rl_games/common/transforms/soft_augmentation.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/transforms/transforms.py` & `rl_games_y-0.0.2/rl_games/common/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/vecenv.py` & `rl_games_y-0.0.2/rl_games/common/vecenv.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/common/wrappers.py` & `rl_games_y-0.0.2/rl_games/common/wrappers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_breakout_torch_impala.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_breakout_torch_impala.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_gopher.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_gopher.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_invaders_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_invaders_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_space_invaders_resnet.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_space_invaders_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/atari/ppo_space_invaders_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/atari/ppo_space_invaders_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_ant.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_ant_tcnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_ant_tcnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_grasp.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_grasp.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_halfcheetah.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_halfcheetah.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_humanoid.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/ppo_ur5e.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/ppo_ur5e.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/sac_ant.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/sac_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/brax/sac_humanoid.yaml` & `rl_games_y-0.0.2/rl_games/configs/brax/sac_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/carracing_ppo.yaml` & `rl_games_y-0.0.2/rl_games/configs/carracing_ppo.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/cartpole.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/cartpole.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/fish_swim.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/fish_swim.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/halfcheetah_run.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/hopper.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-params:  
+params:
+  seed: 5
   algo:
     name: a2c_continuous
 
   model:
     name: continuous_a2c_logstd
 
   network:
@@ -19,42 +20,46 @@
           val: 0
         fixed_sigma: True
     mlp:
       units: [256, 128, 64]
       activation: elu
       initializer:
         name: default
+
   config:
+    name: Hopper-v4_ray
+    env_name: openai_gym
+    score_to_win: 20000
+    normalize_input: True
+    normalize_value: True
+    value_bootstrap: True
     reward_shaper:
       scale_value: 0.1
     normalize_advantage: True
-    gamma: 0.995
+    gamma: 0.99
     tau: 0.95
 
-    learning_rate: 3e-4
-    name: HalfCheetah-v2
-    score_to_win: 10000
-
-    grad_norm: 0.5
+    learning_rate: 5e-4
+    lr_schedule: adaptive
+    kl_threshold: 0.008
+    grad_norm: 1.0
     entropy_coef: 0.0
     truncate_grads: True
-    env_name: openai_gym
     e_clip: 0.2
     clip_value: False
-    num_actors: 16
-    horizon_length: 128
-    minibatch_size: 512
-    mini_epochs: 4
-    critic_coef: 1
-    lr_schedule:  adaptive
-    kl_threshold: 0.008
-    normalize_input: True
-    normalize_value: True
-    value_bootstrap: True
-    bounds_loss_coef: 0.000
+    num_actors: 64
+    horizon_length: 64
+    minibatch_size: 2048
+    mini_epochs: 5
+    critic_coef: 2
+    use_smooth_clamp: True
+    bound_loss_type: regularisation
+    bounds_loss_coef: 0.0
+    max_epochs: 1000
 
     env_config:
-      name: HalfCheetah-v2
+      name: Hopper-v4
       seed: 5
 
     player:
-      render: True
+      render: True
+      determenistic: True
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/humanoid2.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_continuous.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -21,43 +21,44 @@
         fixed_sigma: True
     mlp:
       units: [256, 128, 64]
       activation: elu
       initializer:
         name: default
       regularizer:
-        name:  'None' #'l2_regularizer'
+        name: None #'l2_regularizer'
         #scale: 0.001
 
+  load_checkpoint: False
+  load_path: path
+
   config:
-    reward_shaper:
-      scale_value: 0.1
-    normalize_advantage: True
-    gamma: 0.99
-    tau: 0.9
-
-    learning_rate: 3e-4
-    name: dm_humanoid
-    score_to_win: 10000
-
-    grad_norm: 0.5
-    entropy_coef: 0.0
-    truncate_grads: True
-    env_name: dm_control
-    e_clip: 0.2
-    clip_value: True
-    num_actors: 4
-    horizon_length: 4096
-    minibatch_size: 4096
-    mini_epochs: 15
-    critic_coef: 1
-    lr_schedule: adaptive
-    kl_threshold: 0.008
-
-    normalize_input: False
-    seq_length: 8
-    bounds_loss_coef: 0.0
-
-    env_config:
-      name: Humanoid2Run-v0
-      flat_observation: True
-      
+      reward_shaper:
+        scale_value: 0.1
+      normalize_advantage: True
+      gamma: 0.99
+      tau: 0.9
+
+      learning_rate: 3e-4
+      name: walker
+      score_to_win: 300
+
+      grad_norm: 0.5
+      entropy_coef: 0.0
+      truncate_grads: True
+      env_name: openai_gym
+      e_clip: 0.2
+      clip_value: True
+      num_actors: 16
+      horizon_length: 256
+      minibatch_size: 1024
+      mini_epochs: 8
+      critic_coef: 1
+      lr_schedule:  adaptive
+      kl_threshold: 0.008
+
+      normalize_input: False
+      seq_length: 8
+      bounds_loss_coef: 0.001
+      env_config:
+        name: BipedalWalkerHardcore-v3
+
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/humanoid_run.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/humanoid_run.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/sac_humanoid.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-params:  
+params:
+  seed: 5
   algo:
     name: sac
 
   model:
     name: soft_actor_critic
 
   network:
     name: soft_actor_critic
     separate: True
     space:
       continuous:
-
     mlp:
-      units: [512, 256]
+      units: [256, 128, 64]
       activation: relu
+
       initializer:
         name: default
-
     log_std_bounds: [-5, 2]
 
   config:
-    name: 'humanoid_run_sac'
-    env_name : dm_control
+    name: HalfCheetah-v4_SAC
+    env_name: envpool
     normalize_input: True
     reward_shaper:
-      scale_value: 0.1
-    device: cuda
-    max_epochs: 2000000
-    num_steps_per_episode: 128
-    save_best_after: 100
-    save_frequency: 10000
+      scale_value: 1.0
+
+    max_epochs: 40000
+    num_steps_per_episode: 2
+    save_best_after: 500
+    save_frequency: 1000
     gamma: 0.99
-    init_alpha: 1
-    alpha_lr: 0.0002
-    actor_lr: 0.0003
-    critic_lr: 0.0003
+    init_alpha: 1.0
+    alpha_lr: 5e-3
+    actor_lr: 5e-4
+    critic_lr: 5e-4
     critic_tau: 0.005
-    batch_size: 1024
-    learnable_temperature: true
-    num_warmup_steps: 16
+    batch_size: 2048
+    learnable_temperature: True
+    num_warmup_steps: 50
     replay_buffer_size: 1000000
     num_actors: 32
 
     env_config:
-      name: HumanoidRun-v0
-      flat_observation: True
+      env_name: HalfCheetah-v4
+      seed: 5
+
+    player:
+      render: True
+      deterministic: True
+      games_num: 100
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/walker_run.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/walker_run.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/walker_stand.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/walker_stand.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/dm_control/walker_walk.yaml` & `rl_games_y-0.0.2/rl_games/configs/dm_control/walker_walk.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ma/ppo_connect4_self_play.yaml` & `rl_games_y-0.0.2/rl_games/configs/ma/ppo_connect4_self_play.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml` & `rl_games_y-0.0.2/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ma/ppo_slime_self_play.yaml` & `rl_games_y-0.0.2/rl_games/configs/ma/ppo_slime_self_play.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ma/ppo_slime_v0.yaml` & `rl_games_y-0.0.2/rl_games/configs/ma/ppo_slime_v0.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/minigrid/lava_rnn_img.yaml` & `rl_games_y-0.0.2/rl_games/configs/minigrid/lava_rnn_img.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/minigrid/minigrid_rnn_img.yaml` & `rl_games_y-0.0.2/rl_games/configs/minigrid/minigrid_rnn_img.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/ant.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/ant_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/ant_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/halfcheetah.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/halfcheetah.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/halfcheetah_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/halfcheetah_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/hopper.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/walker2d.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -22,44 +22,41 @@
     mlp:
       units: [256, 128, 64]
       activation: elu
       initializer:
         name: default
 
   config:
-    name: Hopper-v4_ray
+    name: Walker2d-v4_ray
     env_name: openai_gym
-    score_to_win: 20000
     normalize_input: True
     normalize_value: True
     value_bootstrap: True
     reward_shaper:
       scale_value: 0.1
     normalize_advantage: True
     gamma: 0.99
     tau: 0.95
 
-    learning_rate: 5e-4
+    learning_rate: 3e-4
     lr_schedule: adaptive
     kl_threshold: 0.008
     grad_norm: 1.0
     entropy_coef: 0.0
     truncate_grads: True
     e_clip: 0.2
     clip_value: False
     num_actors: 64
-    horizon_length: 64
+    horizon_length: 128
     minibatch_size: 2048
     mini_epochs: 5
     critic_coef: 2
     use_smooth_clamp: True
     bound_loss_type: regularisation
     bounds_loss_coef: 0.0
     max_epochs: 1000
-
     env_config:
-      name: Hopper-v4
+      name: Walker2d-v4
       seed: 5
 
     player:
-      render: True
-      determenistic: True
+      render: True
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/hopper_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/hopper_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/humanoid.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/humanoid_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/humanoid_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/sac_ant_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/sac_ant_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_pendulum_torch.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,58 @@
-params:
-  seed: 5
+params:  
   algo:
-    name: sac
+    name: a2c_continuous
 
   model:
-    name: soft_actor_critic
+    name: continuous_a2c_logstd
 
   network:
-    name: soft_actor_critic
+    name: actor_critic
     separate: True
     space:
       continuous:
+        mu_activation: None
+        sigma_activation: None
+        mu_init:
+          name: glorot_normal_initializer
+          gain: 0.01
+        sigma_init:
+          name: const_initializer
+          val: 0
+        fixed_sigma: True
     mlp:
-      units: [256, 128, 64]
-      activation: relu
-
+      units: [32, 32]
+      activation: elu
       initializer:
-        name: default
-    log_std_bounds: [-5, 2]
+        name: glorot_normal_initializer
+        gain: 2
+      regularizer:
+        name: None #'l2_regularizer'
+        #scale: 0.001
 
   config:
-    name: HalfCheetah-v4_SAC
-    env_name: envpool
-    normalize_input: True
+    env_name: Pendulum-v0
     reward_shaper:
-      scale_value: 1.0
-
-    max_epochs: 40000
-    num_steps_per_episode: 2
-    save_best_after: 500
-    save_frequency: 1000
+      scale_value: 0.01
+    normalize_advantage: True
     gamma: 0.99
-    init_alpha: 1.0
-    alpha_lr: 5e-3
-    actor_lr: 5e-4
-    critic_lr: 5e-4
-    critic_tau: 0.005
-    batch_size: 2048
-    learnable_temperature: True
-    num_warmup_steps: 50
-    replay_buffer_size: 1000000
-    num_actors: 32
-
-    env_config:
-      env_name: HalfCheetah-v4
-      seed: 5
-
-    player:
-      render: True
-      deterministic: True
-      games_num: 100
+    tau: 0.9
+
+    learning_rate: 1e-3
+    name: pendulum
+    score_to_win: 300
+
+    grad_norm: 0.5
+    entropy_coef: 0.0
+    truncate_grads: True
+    e_clip: 0.2
+    clip_value: False
+    num_actors: 16
+    horizon_length: 128
+    minibatch_size: 1024
+    mini_epochs: 4
+    critic_coef: 1
+    lr_schedule: adaptive
+    kl_threshold: 0.016
+
+    normalize_input: False
+    bounds_loss_coef: 0
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/walker2d.yaml` & `rl_games_y-0.0.2/rl_games/configs/mujoco/walker2d_envpool.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,29 @@
     mlp:
       units: [256, 128, 64]
       activation: elu
       initializer:
         name: default
 
   config:
-    name: Walker2d-v4_ray
-    env_name: openai_gym
+    name: Walker2d-v4_envpool
+    env_name: envpool
+    score_to_win: 20000
     normalize_input: True
     normalize_value: True
     value_bootstrap: True
     reward_shaper:
       scale_value: 0.1
     normalize_advantage: True
     gamma: 0.99
     tau: 0.95
 
     learning_rate: 3e-4
     lr_schedule: adaptive
-    kl_threshold: 0.008
+    kl_threshold: 0.008 
     grad_norm: 1.0
     entropy_coef: 0.0
     truncate_grads: True
     e_clip: 0.2
     clip_value: False
     num_actors: 64
     horizon_length: 128
@@ -51,12 +52,13 @@
     mini_epochs: 5
     critic_coef: 2
     use_smooth_clamp: True
     bound_loss_type: regularisation
     bounds_loss_coef: 0.0
     max_epochs: 1000
     env_config:
-      name: Walker2d-v4
+      env_name: Walker2d-v4
       seed: 5
 
     player:
-      render: True
+      render: True
+
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/mujoco/walker2d_envpool.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_continuous_lstm.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,61 @@
-params:
-  seed: 5
+params:  
   algo:
     name: a2c_continuous
 
   model:
-    name: continuous_a2c_logstd
+    name: continuous_a2c_lstm_logstd
 
   network:
     name: actor_critic
-    separate: False
+    separate: True
     space:
       continuous:
         mu_activation: None
         sigma_activation: None
         mu_init:
-          name: default
+          name: normc_initializer
+          std: 0.01
         sigma_init:
           name: const_initializer
-          val: 0
+          value: 0.0
         fixed_sigma: True
+
     mlp:
-      units: [256, 128, 64]
-      activation: elu
+      units: [256, 256, 128]
+      activation: relu
       initializer:
-        name: default
+        name: normc_initializer
+        std: 1
+      regularizer:
+        name: None
+    lstm:
+      units: 128
+      concated: False
 
   config:
-    name: Walker2d-v4_envpool
-    env_name: envpool
-    score_to_win: 20000
-    normalize_input: True
-    normalize_value: True
-    value_bootstrap: True
+    env_name:  BipedalWalkerHardcore-v2
     reward_shaper:
       scale_value: 0.1
+
     normalize_advantage: True
     gamma: 0.99
-    tau: 0.95
-
-    learning_rate: 3e-4
-    lr_schedule: adaptive
-    kl_threshold: 0.008 
-    grad_norm: 1.0
-    entropy_coef: 0.0
+    tau: 0.9
+    learning_rate: 1e-4
+    name: walker_lstm
+    score_to_win: 300
+    grad_norm: 0.5
+    entropy_coef: 0.000
     truncate_grads: True
     e_clip: 0.2
-    clip_value: False
-    num_actors: 64
-    horizon_length: 128
+    clip_value: True
+    num_actors: 16
+    horizon_length: 512
     minibatch_size: 2048
-    mini_epochs: 5
-    critic_coef: 2
-    use_smooth_clamp: True
-    bound_loss_type: regularisation
-    bounds_loss_coef: 0.0
-    max_epochs: 1000
-    env_config:
-      env_name: Walker2d-v4
-      seed: 5
-
-    player:
-      render: True
-
+    mini_epochs: 8
+    critic_coef: 1
+    lr_schedule:  None
+    kl_threshold: 0.008
+    normalize_input: False
+    seq_length: 8
+    bounds_loss_coef: 0.5
+    max_epochs: 5000
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_ant.yaml` & `rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_hand.yaml` & `rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_hand.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/openai/ppo_gym_humanoid.yaml` & `rl_games_y-0.0.2/rl_games/configs/openai/ppo_gym_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_cartpole.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_cartpole.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_continuous.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_lunar.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -9,56 +9,52 @@
     name: actor_critic
     separate: True
     space:
       continuous:
         mu_activation: None
         sigma_activation: None
         mu_init:
-          name: default
-          scale: 0.02
+          name: glorot_normal_initializer
+          #scal: 0.01
         sigma_init:
           name: const_initializer
-          val: 0
+          value: 0
         fixed_sigma: True
     mlp:
-      units: [256, 128, 64]
-      activation: elu
+      units: [64, 64]
+      activation: relu
       initializer:
-        name: default
+        name: glorot_normal_initializer
+        #gain: 2
       regularizer:
-        name: None #'l2_regularizer'
+        name:  'None' #'l2_regularizer'
         #scale: 0.001
 
   load_checkpoint: False
   load_path: path
 
   config:
       reward_shaper:
         scale_value: 0.1
       normalize_advantage: True
       gamma: 0.99
       tau: 0.9
 
-      learning_rate: 3e-4
-      name: walker
+      learning_rate: 1e-4
+      name: test
       score_to_win: 300
 
       grad_norm: 0.5
       entropy_coef: 0.0
       truncate_grads: True
-      env_name: openai_gym
+      env_name:  LunarLanderContinuous-v2
       e_clip: 0.2
       clip_value: True
       num_actors: 16
-      horizon_length: 256
+      horizon_length: 128
       minibatch_size: 1024
-      mini_epochs: 8
+      mini_epochs: 4
       critic_coef: 1
       lr_schedule:  adaptive
       kl_threshold: 0.008
-
       normalize_input: False
-      seq_length: 8
-      bounds_loss_coef: 0.001
-      env_config:
-        name: BipedalWalkerHardcore-v3
-
+      bounds_loss_coef: 0
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_continuous_lstm.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/corridor_torch_cv.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 params:  
   algo:
-    name: a2c_continuous
+    name: a2c_discrete
 
   model:
-    name: continuous_a2c_lstm_logstd
+    name: discrete_a2c
 
   network:
     name: actor_critic
-    separate: True
-    space:
-      continuous:
-        mu_activation: None
-        sigma_activation: None
-        mu_init:
-          name: normc_initializer
-          std: 0.01
-        sigma_init:
-          name: const_initializer
-          value: 0.0
-        fixed_sigma: True
-
+    separate: False
+    #normalization: layer_norm
+    space: 
+      discrete:
     mlp:
-      units: [256, 256, 128]
+      units: [512, 256, 128]
       activation: relu
       initializer:
-        name: normc_initializer
-        std: 1
+        name: default 
       regularizer:
         name: None
-    lstm:
-      units: 128
-      concated: False
 
   config:
-    env_name:  BipedalWalkerHardcore-v2
+    name: corridor_cv
     reward_shaper:
-      scale_value: 0.1
-
+      scale_value: 1
     normalize_advantage: True
-    gamma: 0.99
-    tau: 0.9
-    learning_rate: 1e-4
-    name: walker_lstm
-    score_to_win: 300
+    gamma: 0.995
+    tau: 0.95
+    learning_rate: 3e-4
+    score_to_win: 20
     grad_norm: 0.5
-    entropy_coef: 0.000
+    entropy_coef: 0.005
     truncate_grads: True
+    env_name: smac
     e_clip: 0.2
     clip_value: True
-    num_actors: 16
-    horizon_length: 512
-    minibatch_size: 2048
-    mini_epochs: 8
+    num_actors: 8
+    horizon_length: 128
+    minibatch_size: 3072 # 6 * 512
+    mini_epochs: 4
     critic_coef: 1
-    lr_schedule:  None
-    kl_threshold: 0.008
-    normalize_input: False
-    seq_length: 8
-    bounds_loss_coef: 0.5
-    max_epochs: 5000
+    lr_schedule: None
+    kl_threshold: 0.05
+    normalize_input: True
+    use_action_masks: True
+    ignore_dead_batches : False
+
+    env_config:
+      name: corridor
+      central_value: True
+      reward_only_positive: False
+      obs_last_action: True
+      frames: 1
+      reward_negative_scale: 0.05
+      #apply_agent_ids: True
+      #flatten: False
+
+    central_value_config:
+      minibatch_size: 512
+      mini_epochs: 4
+      learning_rate: 3e-4
+      clip_value: False
+      normalize_input: True
+      network:
+        name: actor_critic
+        central_value: True
+        mlp:
+          units: [512, 256, 128]
+          activation: relu
+          initializer:
+            name: default
+            scale: 2 
+          regularizer:
+            name: None
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_lunar.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_pendulum.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,52 +9,54 @@
     name: actor_critic
     separate: True
     space:
       continuous:
         mu_activation: None
         sigma_activation: None
         mu_init:
-          name: glorot_normal_initializer
-          #scal: 0.01
+          name: default
+          scale: 0.01
         sigma_init:
           name: const_initializer
           value: 0
-        fixed_sigma: True
+        fixed_sigma: False
     mlp:
-      units: [64, 64]
-      activation: relu
+      units: [32, 32]
+      activation: elu
       initializer:
-        name: glorot_normal_initializer
-        #gain: 2
+        name: default
+        scale: 1
       regularizer:
         name:  'None' #'l2_regularizer'
         #scale: 0.001
 
   load_checkpoint: False
   load_path: path
 
   config:
-      reward_shaper:
-        scale_value: 0.1
-      normalize_advantage: True
-      gamma: 0.99
-      tau: 0.9
+    env_name: Pendulum-v0
+    reward_shaper:
+      scale_value: 0.01
+    normalize_advantage: True
+    gamma: 0.99
+    tau: 0.9
 
-      learning_rate: 1e-4
-      name: test
-      score_to_win: 300
+    learning_rate: 1e-4
+    lr_schedule:  adaptive
+    kl_threshold: 0.008
+    name: test
+    score_to_win: 300
 
-      grad_norm: 0.5
-      entropy_coef: 0.0
-      truncate_grads: True
-      env_name:  LunarLanderContinuous-v2
-      e_clip: 0.2
-      clip_value: True
-      num_actors: 16
-      horizon_length: 128
-      minibatch_size: 1024
-      mini_epochs: 4
-      critic_coef: 1
-      lr_schedule:  adaptive
-      kl_threshold: 0.008
-      normalize_input: False
-      bounds_loss_coef: 0
+    grad_norm: 0.5
+    entropy_coef: 0.0
+    truncate_grads: True 
+    e_clip: 0.2
+    clip_value: True
+    num_actors: 16
+    horizon_length: 128
+    minibatch_size: 1024
+    mini_epochs: 4
+    critic_coef: 1
+
+    normalize_input: False
+    seq_length: 8
+    bounds_loss_coef: 0
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_lunar_continiuos_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_lunar_continiuos_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_lunar_discrete.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_lunar_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_multiwalker.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_multiwalker.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_pendulum.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_walker.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 params:  
+  seed: 8
   algo:
     name: a2c_continuous
 
   model:
     name: continuous_a2c_logstd
 
   network:
     name: actor_critic
-    separate: True
+    separate: False
     space:
       continuous:
         mu_activation: None
         sigma_activation: None
         mu_init:
           name: default
-          scale: 0.01
         sigma_init:
           name: const_initializer
-          value: 0
-        fixed_sigma: False
+          val: 0
+        fixed_sigma: True
     mlp:
-      units: [32, 32]
+      units: [256,128,64]
+      d2rl: False
       activation: elu
       initializer:
         name: default
-        scale: 1
-      regularizer:
-        name:  'None' #'l2_regularizer'
-        #scale: 0.001
-
-  load_checkpoint: False
-  load_path: path
-
+        scale: 2
   config:
-    env_name: Pendulum-v0
+    env_name: BipedalWalker-v3
+    name: walker
     reward_shaper:
-      scale_value: 0.01
-    normalize_advantage: True
-    gamma: 0.99
-    tau: 0.9
+      min_val: -1
+      scale_value: 0.1
 
-    learning_rate: 1e-4
-    lr_schedule:  adaptive
+    normalize_advantage: True
+    gamma: 0.995
+    tau: 0.95
+    learning_rate: 3e-4
+    lr_schedule: adaptive
     kl_threshold: 0.008
-    name: test
+    save_best_after: 10
     score_to_win: 300
-
-    grad_norm: 0.5
-    entropy_coef: 0.0
-    truncate_grads: True 
+    grad_norm: 1.5
+    entropy_coef: 0
+    truncate_grads: True
     e_clip: 0.2
-    clip_value: True
+    clip_value: False
     num_actors: 16
-    horizon_length: 128
-    minibatch_size: 1024
+    horizon_length: 4096
+    minibatch_size: 8192
     mini_epochs: 4
-    critic_coef: 1
-
-    normalize_input: False
-    seq_length: 8
-    bounds_loss_coef: 0
+    critic_coef: 2
+    normalize_input: True
+    bounds_loss_coef: 0.00
+    max_epochs: 10000
+    normalize_value: True
+    use_diagnostics: True
+    value_bootstrap: True
+    #weight_decay: 0.0001
+    use_smooth_clamp: True
+
+    player:
+      render: True
+      determenistic: True
+      games_num: 200
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_pendulum_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/8m_torch_cv.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 params:  
   algo:
-    name: a2c_continuous
+    name: a2c_discrete
 
   model:
-    name: continuous_a2c_logstd
+    name: discrete_a2c
 
   network:
     name: actor_critic
-    separate: True
-    space:
-      continuous:
-        mu_activation: None
-        sigma_activation: None
-        mu_init:
-          name: glorot_normal_initializer
-          gain: 0.01
-        sigma_init:
-          name: const_initializer
-          val: 0
-        fixed_sigma: True
+    separate: False
+    #normalization: layer_norm
+    space: 
+      discrete:
+
     mlp:
-      units: [32, 32]
-      activation: elu
+      units: [256, 128]
+      activation: relu
       initializer:
-        name: glorot_normal_initializer
-        gain: 2
+        name: default 
       regularizer:
-        name: None #'l2_regularizer'
-        #scale: 0.001
+        name: None
 
   config:
-    env_name: Pendulum-v0
+    name: 8m_cv
     reward_shaper:
-      scale_value: 0.01
+      scale_value: 1
     normalize_advantage: True
     gamma: 0.99
-    tau: 0.9
-
-    learning_rate: 1e-3
-    name: pendulum
-    score_to_win: 300
-
+    tau: 0.95
+    learning_rate: 5e-4
+    score_to_win: 20
     grad_norm: 0.5
-    entropy_coef: 0.0
+    entropy_coef: 0.001
     truncate_grads: True
+    env_name: smac
     e_clip: 0.2
-    clip_value: False
-    num_actors: 16
+    clip_value: True
+    num_actors: 8
     horizon_length: 128
-    minibatch_size: 1024
+    minibatch_size: 4096 # 3 * 512
     mini_epochs: 4
     critic_coef: 1
-    lr_schedule: adaptive
-    kl_threshold: 0.016
-
-    normalize_input: False
-    bounds_loss_coef: 0
+    lr_schedule: None
+    kl_threshold: 0.05
+    normalize_input: True
+    seq_length: 2
+    use_action_masks: True
+    ignore_dead_batches : False
+    max_epochs: 10000
+
+    central_value_config:
+      minibatch_size: 512
+      mini_epochs: 4
+      learning_rate: 5e-4
+      clip_value: False
+      normalize_input: True
+      network:
+        name: actor_critic
+        central_value: True
+        mlp:
+          units: [512, 256,128]
+          activation: relu
+          initializer:
+            name: default
+            scale: 2 
+          regularizer:
+            name: None
+
+    env_config:
+      name: 8m
+      frames: 1
+      transpose: False
+      random_invalid_step: False
+      central_value: True
+      reward_only_positive: False
+      obs_last_action: True
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_reacher.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_reacher.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_smac.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_smac.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_walker.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_walker_hardcore.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 params:  
-  seed: 8
   algo:
     name: a2c_continuous
 
   model:
     name: continuous_a2c_logstd
 
   network:
     name: actor_critic
-    separate: False
+    separate: True
     space:
       continuous:
         mu_activation: None
         sigma_activation: None
         mu_init:
           name: default
         sigma_init:
           name: const_initializer
           val: 0
         fixed_sigma: True
     mlp:
-      units: [256,128,64]
+      units: [256,128, 64]
       d2rl: False
       activation: elu
       initializer:
         name: default
-        scale: 2
+  load_checkpoint: False
+  load_path: './nn/walker_hc.pth'
+
   config:
-    env_name: BipedalWalker-v3
-    name: walker
+    env_name:  BipedalWalkerHardcore-v3
+    name: walker_hc
     reward_shaper:
       min_val: -1
       scale_value: 0.1
 
     normalize_advantage: True
     gamma: 0.995
     tau: 0.95
-    learning_rate: 3e-4
+    learning_rate: 5e-4
     lr_schedule: adaptive
     kl_threshold: 0.008
-    save_best_after: 10
     score_to_win: 300
     grad_norm: 1.5
+    save_best_after: 10
     entropy_coef: 0
     truncate_grads: True
     e_clip: 0.2
     clip_value: False
     num_actors: 16
     horizon_length: 4096
     minibatch_size: 8192
     mini_epochs: 4
-    critic_coef: 2
+    critic_coef: 1
     normalize_input: True
-    bounds_loss_coef: 0.00
-    max_epochs: 10000
-    normalize_value: True
-    use_diagnostics: True
-    value_bootstrap: True
-    #weight_decay: 0.0001
-    use_smooth_clamp: True
+    seq_length: 4
+    bounds_loss_coef: 0.0
+    max_epochs: 100000
+    weight_decay: 0
 
     player:
-      render: True
-      determenistic: True
+      render: False
       games_num: 200
+      determenistic: True 
+
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_walker_hardcore.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,54 @@
 params:  
   algo:
-    name: a2c_continuous
+    name: a2c_discrete
 
   model:
-    name: continuous_a2c_logstd
+    name: discrete_a2c_lstm
+
 
   network:
     name: actor_critic
     separate: True
-    space:
-      continuous:
-        mu_activation: None
-        sigma_activation: None
-        mu_init:
-          name: default
-        sigma_init:
-          name: const_initializer
-          val: 0
-        fixed_sigma: True
+    space: 
+      discrete:
+      
     mlp:
-      units: [256,128, 64]
-      d2rl: False
-      activation: elu
+      units: [256, 128]
+      activation: relu
       initializer:
-        name: default
-  load_checkpoint: False
-  load_path: './nn/walker_hc.pth'
-
+        name: default 
+      regularizer:
+        name: 'None'
+    lstm:
+      units: 128
+      concated: False
   config:
-    env_name:  BipedalWalkerHardcore-v3
-    name: walker_hc
+    name: 3s_vs_5z
     reward_shaper:
-      min_val: -1
-      scale_value: 0.1
-
+      scale_value: 1
     normalize_advantage: True
-    gamma: 0.995
+    gamma: 0.99
     tau: 0.95
-    learning_rate: 5e-4
-    lr_schedule: adaptive
-    kl_threshold: 0.008
-    score_to_win: 300
-    grad_norm: 1.5
-    save_best_after: 10
-    entropy_coef: 0
+    learning_rate: 1e-4
+    score_to_win: 1000
+    grad_norm: 0.5
+    entropy_coef: 0.001
     truncate_grads: True
+    env_name: smac
     e_clip: 0.2
-    clip_value: False
-    num_actors: 16
-    horizon_length: 4096
-    minibatch_size: 8192
+    clip_value: True
+    num_actors: 8
+    horizon_length: 128
+    minibatch_size: 1536 #1024
     mini_epochs: 4
     critic_coef: 1
-    normalize_input: True
+    lr_schedule: None
+    kl_threshold: 0.05
+    normalize_input: False
     seq_length: 4
-    bounds_loss_coef: 0.0
-    max_epochs: 100000
-    weight_decay: 0
-
-    player:
-      render: False
-      games_num: 200
-      determenistic: True 
+    use_action_masks: True
 
+    env_config:
+      name: 3s_vs_5z
+      frames: 1
+      random_invalid_step: False
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_walker_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_walker_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/ppo_walker_tcnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/ppo_walker_tcnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/procgen/ppo_coinrun.yaml` & `rl_games_y-0.0.2/rl_games/configs/procgen/ppo_coinrun.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/10m_vs_11m_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/10m_vs_11m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/27m_vs_30m_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/27m_vs_30m_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/27m_vs_30m_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/27m_vs_30m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/2m_vs_1z.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/2m_vs_1z_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/2m_vs_1z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/2s_vs_1c.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/2s_vs_1c.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_cnn_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_cnn_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv_joint.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv_joint.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_cv_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_cv_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3m_torch_sparse.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3m_torch_sparse.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_4z.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_4z.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/8m_torch.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 params:  
   algo:
     name: a2c_discrete
 
   model:
-    name: discrete_a2c_lstm
-
+    name: discrete_a2c
 
   network:
     name: actor_critic
     separate: True
+    #normalization: layer_norm
     space: 
       discrete:
-      
+
     mlp:
       units: [256, 128]
       activation: relu
       initializer:
         name: default 
       regularizer:
-        name: 'None'
-    lstm:
-      units: 128
-      concated: False
+        name: None
   config:
-    name: 3s_vs_5z
+    name: 8m
     reward_shaper:
       scale_value: 1
     normalize_advantage: True
     gamma: 0.99
     tau: 0.95
-    learning_rate: 1e-4
-    score_to_win: 1000
+    learning_rate: 5e-4
+    score_to_win: 20
     grad_norm: 0.5
     entropy_coef: 0.001
     truncate_grads: True
     env_name: smac
     e_clip: 0.2
     clip_value: True
     num_actors: 8
     horizon_length: 128
-    minibatch_size: 1536 #1024
+    minibatch_size: 4096
     mini_epochs: 4
     critic_coef: 1
     lr_schedule: None
     kl_threshold: 0.05
-    normalize_input: False
-    seq_length: 4
+    normalize_input: True
+    seq_length: 2
     use_action_masks: True
-
+    ignore_dead_batches : False
+    max_epochs: 10000
     env_config:
-      name: 3s_vs_5z
+      name: 8m
       frames: 1
+      transpose: False
       random_invalid_step: False
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/5m_vs_6m_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/5m_vs_6m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/6h_vs_8z_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/6h_vs_8z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/8m_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 params:  
   algo:
     name: a2c_discrete
 
   model:
-    name: discrete_a2c
+    name: multi_discrete_a2c
 
   network:
     name: actor_critic
     separate: True
-    #normalization: layer_norm
+    #normalization: 'layer_norm'
     space: 
-      discrete:
+      multi_discrete:
 
     mlp:
-      units: [256, 128]
+      units: [32,32]
       activation: relu
       initializer:
-        name: default 
+        name: default
       regularizer:
         name: None
+
   config:
-    name: 8m
     reward_shaper:
       scale_value: 1
     normalize_advantage: True
     gamma: 0.99
-    tau: 0.95
-    learning_rate: 5e-4
-    score_to_win: 20
-    grad_norm: 0.5
-    entropy_coef: 0.001
+    tau: 0.9
+    learning_rate: 2e-4
+    name: test_md_mhv
+    score_to_win: 0.95
+    grad_norm: 10.5
+    entropy_coef: 0.005
     truncate_grads: True
-    env_name: smac
+    env_name: test_env
     e_clip: 0.2
-    clip_value: True
-    num_actors: 8
-    horizon_length: 128
-    minibatch_size: 4096
+    clip_value: False
+    num_actors: 16
+    horizon_length: 512
+    minibatch_size: 2048
     mini_epochs: 4
     critic_coef: 1
     lr_schedule: None
-    kl_threshold: 0.05
-    normalize_input: True
-    seq_length: 2
-    use_action_masks: True
-    ignore_dead_batches : False
+    kl_threshold: 0.008
+    normalize_input: False
+    weight_decay: 0.0000
     max_epochs: 10000
+
     env_config:
-      name: 8m
-      frames: 1
-      transpose: False
-      random_invalid_step: False
+      name: TestRnnEnv-v0
+      hide_object: False
+      apply_dist_reward: False
+      min_dist: 2
+      max_dist: 8
+      use_central_value: False
+      multi_discrete_space: True
+      multi_head_value: False
+    player:
+        games_num: 100
+        determenistic: True
+
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/8m_torch_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/corridor_torch.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,74 +3,73 @@
     name: a2c_discrete
 
   model:
     name: discrete_a2c
 
   network:
     name: actor_critic
-    separate: False
+    separate: True
     #normalization: layer_norm
     space: 
       discrete:
-
+      
+    cnn:
+      type: conv1d
+      activation: relu
+      initializer:
+        name: glorot_uniform_initializer
+        gain: 1.4241 
+      regularizer:
+        name: None
+      convs:    
+        - filters: 64
+          kernel_size: 3
+          strides: 2
+          padding: 1
+        - filters: 128
+          kernel_size: 3
+          strides: 1
+          padding: 0
+        - filters: 256
+          kernel_size: 3
+          strides: 1
+          padding: 0
     mlp:
       units: [256, 128]
       activation: relu
       initializer:
         name: default 
       regularizer:
         name: None
 
   config:
-    name: 8m_cv
+    name: corridor_cnn
     reward_shaper:
       scale_value: 1
     normalize_advantage: True
     gamma: 0.99
     tau: 0.95
-    learning_rate: 5e-4
+    learning_rate: 1e-4
     score_to_win: 20
     grad_norm: 0.5
-    entropy_coef: 0.001
+    entropy_coef: 0.005
     truncate_grads: True
-    env_name: smac
+    env_name: smac_cnn
     e_clip: 0.2
     clip_value: True
     num_actors: 8
     horizon_length: 128
-    minibatch_size: 4096 # 3 * 512
-    mini_epochs: 4
-    critic_coef: 1
+    minibatch_size: 3072
+    mini_epochs: 1
+    critic_coef: 2
     lr_schedule: None
     kl_threshold: 0.05
-    normalize_input: True
+    normalize_input: False
     seq_length: 2
     use_action_masks: True
-    ignore_dead_batches : False
-    max_epochs: 10000
-
-    central_value_config:
-      minibatch_size: 512
-      mini_epochs: 4
-      learning_rate: 5e-4
-      clip_value: False
-      normalize_input: True
-      network:
-        name: actor_critic
-        central_value: True
-        mlp:
-          units: [512, 256,128]
-          activation: relu
-          initializer:
-            name: default
-            scale: 2 
-          regularizer:
-            name: None
+    ignore_dead_batches: False
 
     env_config:
-      name: 8m
-      frames: 1
+      name: corridor
+      frames: 4
       transpose: False
-      random_invalid_step: False
-      central_value: True
-      reward_only_positive: False
-      obs_last_action: True
+      random_invalid_step: False
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/MMM2_torch.yaml` & `rl_games_y-0.0.2/rl_games/configs/smac/MMM2_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/smac/corridor_torch_cv.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -4,71 +4,91 @@
 
   model:
     name: discrete_a2c
 
   network:
     name: actor_critic
     separate: False
-    #normalization: layer_norm
+    #normalization: 'layer_norm'
     space: 
       discrete:
+
     mlp:
-      units: [512, 256, 128]
+      units: [32]
       activation: relu
       initializer:
-        name: default 
+        name: default
       regularizer:
         name: None
+    rnn:
+      name: lstm
+      units: 32
+      layers: 1
+      layer_norm: False
+      before_mlp: False
 
   config:
-    name: corridor_cv
     reward_shaper:
-      scale_value: 1
+        scale_value: 1
     normalize_advantage: True
-    gamma: 0.995
-    tau: 0.95
-    learning_rate: 3e-4
-    score_to_win: 20
-    grad_norm: 0.5
+    gamma: 0.99
+    tau: 0.9
+    learning_rate: 2e-4
+    name: test_md
+    score_to_win: 0.95
+    grad_norm: 10.5
     entropy_coef: 0.005
     truncate_grads: True
-    env_name: smac
+    env_name: test_env
     e_clip: 0.2
-    clip_value: True
-    num_actors: 8
-    horizon_length: 128
-    minibatch_size: 3072 # 6 * 512
+    clip_value: False
+    num_actors: 16
+    horizon_length: 512
+    minibatch_size: 2048
     mini_epochs: 4
     critic_coef: 1
     lr_schedule: None
-    kl_threshold: 0.05
-    normalize_input: True
-    use_action_masks: True
-    ignore_dead_batches : False
+    kl_threshold: 0.008
+    normalize_input: False
+    normalize_value: True
+    weight_decay: 0.0000
+    max_epochs: 10000
+    seq_length: 16
+    save_best_after: 10
 
     env_config:
-      name: corridor
-      central_value: True
-      reward_only_positive: False
-      obs_last_action: True
-      frames: 1
-      reward_negative_scale: 0.05
-      #apply_agent_ids: True
-      #flatten: False
+      name: TestRnnEnv-v0
+      hide_object: True
+      apply_dist_reward: True
+      min_dist: 2
+      max_dist: 8
+      use_central_value: True
+      multi_discrete_space: False
+      multi_head_value: False
+    player:
+        games_num: 100
+        determenistic: True
 
     central_value_config:
       minibatch_size: 512
       mini_epochs: 4
-      learning_rate: 3e-4
+      learning_rate: 5e-4
       clip_value: False
       normalize_input: True
+      truncate_grads: True
+      grad_norm: 10
       network:
         name: actor_critic
         central_value: True
         mlp:
-          units: [512, 256, 128]
+          units: [64]
           activation: relu
           initializer:
             name: default
-            scale: 2 
           regularizer:
-            name: None
+            name: None
+        rnn:
+          name: lstm
+          units: 64
+          layers: 1
+          layer_norm: False
+          before_mlp: False
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_continuous.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_continuous.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-params:  
+params:
+  seed: 322  
   algo:
     name: a2c_discrete
 
   model:
-    name: discrete_a2c
+    name: multi_discrete_a2c
 
   network:
     name: actor_critic
-    separate: False
+    separate: True
     #normalization: 'layer_norm'
     space: 
-      discrete:
+      multi_discrete:
 
     mlp:
-      units: [32]
+      units: [64]
       activation: relu
       initializer:
         name: default
       regularizer:
         name: None
     rnn:
       name: lstm
-      units: 32
+      #layer_norm: True
+      units: 64
       layers: 1
-      layer_norm: False
       before_mlp: False
 
   config:
     reward_shaper:
         scale_value: 1
     normalize_advantage: True
     gamma: 0.99
     tau: 0.9
     learning_rate: 2e-4
-    name: test_md
-    score_to_win: 0.95
+    name: test_rnn_md_mhv
+    score_to_win: 0.99
     grad_norm: 10.5
     entropy_coef: 0.005
     truncate_grads: True
     env_name: test_env
     e_clip: 0.2
     clip_value: False
     num_actors: 16
@@ -46,49 +47,24 @@
     minibatch_size: 2048
     mini_epochs: 4
     critic_coef: 1
     lr_schedule: None
     kl_threshold: 0.008
     normalize_input: False
     normalize_value: True
+    seq_length: 16
     weight_decay: 0.0000
     max_epochs: 10000
-    seq_length: 16
-    save_best_after: 10
 
     env_config:
       name: TestRnnEnv-v0
       hide_object: True
       apply_dist_reward: True
       min_dist: 2
       max_dist: 8
-      use_central_value: True
-      multi_discrete_space: False
-      multi_head_value: False
+      use_central_value: False
+      multi_discrete_space: True
+      multi_head_value: True
     player:
         games_num: 100
         determenistic: True
 
-    central_value_config:
-      minibatch_size: 512
-      mini_epochs: 4
-      learning_rate: 5e-4
-      clip_value: False
-      normalize_input: True
-      truncate_grads: True
-      grad_norm: 10
-      network:
-        name: actor_critic
-        central_value: True
-        mlp:
-          units: [64]
-          activation: relu
-          initializer:
-            name: default
-          regularizer:
-            name: None
-        rnn:
-          name: lstm
-          units: 64
-          layers: 1
-          layer_norm: False
-          before_mlp: False
```

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_discrete.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_ppo_walker_truncated_time.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_ppo_walker_truncated_time.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_rnn.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/configs/test/test_rnn_multidiscrete.yaml` & `rl_games_y-0.0.2/rl_games/configs/test/test_rnn_multidiscrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/brax.py` & `rl_games_y-0.0.2/rl_games/envs/brax.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/connect4_network.py` & `rl_games_y-0.0.2/rl_games/envs/connect4_network.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/connect4_selfplay.py` & `rl_games_y-0.0.2/rl_games/envs/connect4_selfplay.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/diambra/diambra.py` & `rl_games_y-0.0.2/rl_games/envs/diambra/diambra.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/envpool.py` & `rl_games_y-0.0.2/rl_games/envs/envpool.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/multiwalker.py` & `rl_games_y-0.0.2/rl_games/envs/multiwalker.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/slimevolley_selfplay.py` & `rl_games_y-0.0.2/rl_games/envs/slimevolley_selfplay.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/smac_env.py` & `rl_games_y-0.0.2/rl_games/envs/smac_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/test/example_env.py` & `rl_games_y-0.0.2/rl_games/envs/test/example_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/test/rnn_env.py` & `rl_games_y-0.0.2/rl_games/envs/test/rnn_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/test/test_asymmetric_env.py` & `rl_games_y-0.0.2/rl_games/envs/test/test_asymmetric_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/envs/test_network.py` & `rl_games_y-0.0.2/rl_games/envs/test_network.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/interfaces/base_algorithm.py` & `rl_games_y-0.0.2/rl_games/interfaces/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/networks/tcnn_mlp.py` & `rl_games_y-0.0.2/rl_games/networks/tcnn_mlp.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/rl_games/torch_runner.py` & `rl_games_y-0.0.2/rl_games/torch_runner.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.1/PKG-INFO` & `rl_games_y-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl-games-y
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Denys Makoviichuk
 Author-email: trrrrr97@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Provides-Extra: envpool
 Provides-Extra: mujoco
 Requires-Dist: AutoROM[accept-rom-license] (>=0.4.2,<0.5.0) ; extra == "atari"
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: ale-py (>=0.7,<0.8) ; extra == "atari"
 Requires-Dist: brax (>=0.0.13,<0.0.14) ; extra == "brax"
 Requires-Dist: envpool (>=0.6.1,<0.7.0) ; extra == "envpool"
-Requires-Dist: gym[classic-control] (>=0.23.0,<0.24.0)
+Requires-Dist: gym[classic-control] (>=0.24.1,<0.25.0)
 Requires-Dist: jax (>=0.3.13,<0.4.0) ; extra == "brax"
 Requires-Dist: mujoco-py (>=2.1.2,<3.0.0) ; extra == "mujoco"
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: ray (>=1.11.0,<2.0.0)
 Requires-Dist: setproctitle (>=1.2.2,<2.0.0)
 Requires-Dist: tensorboard (>=2.8.0,<3.0.0)
```

