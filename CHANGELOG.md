# 更新日志

## 7.6.10

- 机型模拟正式目录扩展到 121 款；本轮在公网机型 Release 中完成 15 款新增和 3 款原位更新。
- CPU/GPU 页面接入 `cpuwz v1.9-exp`：25 个 profile 全部开放，其中 7 个 CPU/GPU 联动，18 个 GPU-only 仅切换 GPU 并保持当前 CPU。
- GPU-only 模式保留真实 `cpuinfoReady=false` 诊断，不生成或拼接缺失的 `.cpuinfo`，切换前后强制校验 CPU SHA 不变。
- 指定真机完成 `V2403A / iQOO Neo9S Pro+ / QTI SM8650 / Qualcomm Adreno 750` 组合验收，并通过 WDF loader、local verify、SUSFS 与延迟复验。

## 7.6.6

- 修复高级防误判的BUG。

## 7.6.5

- 修复高级设备标识的原生二进制执行方式，手动更换不再被 shell 当作脚本解析。
- 无 OAID 载体的设备会自动禁用或跳过 OAID，其它序列号、Android ID、Wi-Fi MAC、蓝牙 MAC 可继续正常更换，不再误报整组失败。
- 高级防误判新增游戏场景预设、多用户应用状态、masking 操作快照与单步撤销等功能。
- 完善 ReSukiSU SUSFS、Zygisk Next、隐藏 SELinux 修改的自动配置与统一运行日志。

## 7.6.4

- 更新高级功能，修复BUG

## 7.6.2

隐藏应用和游戏防标记拆成了两个独立功能，各用各的：

- 应用隐藏：勾选要藏的 App，点“保存并隐藏”马上冻结并从桌面隐藏，点“立即恢复”再放出来。不用先开游戏防标记。
- 游戏防标记：只管游戏，和应用隐藏互不影响。

已经装了旧版本的，在管理器里直接点更新就能升到 7.6.2。
