# 具身智能桌面机械臂 · 课设仓库

基于模仿学习的视觉抓取机械臂
（Windows 上位机 + 塔克 OpenCTR H50 下位机 + 6× 飞特 STS3215 总线舵机，SO-101 构型）

## 进来看什么

| 想看什么 | 去哪 |
|---|---|
| **现在项目到哪了、谁卡住了** | [`PROGRESS.md`](PROGRESS.md) ← 组会只看这个文件 |
| 技术方案、架构、采购清单 | [`具身智能机械臂课设方案.md`](具身智能机械臂课设方案.md) |
| 所有术语的白话解释 | [`具身智能机械臂课设·小白说明书.md`](具身智能机械臂课设·小白说明书.md) |
| 具体某件事的讨论与进展 | [Issues](../../issues)，用 `lane:` 标签和 Milestone 筛 |
| 看板视图（拖卡改状态） | [Projects 看板](https://github.com/users/mwu62665/projects/1)，五列 `Backlog / 本周 / 进行中 / 卡住 / Done` |

> 看板只是筛选器，**结论永远写在 `PROGRESS.md` 里**。投屏投那个文件，别投看板（国内访问不稳）。

## 约定

- **周次 = GitHub Milestone**（`W0` ~ `W10`），对齐方案 §8 的十周计划，自带截止日和进度条
- **泳道 = label**，五个：`lane:hw` 硬件结构 / `lane:fw` 下位机固件 / `lane:sw` 上位机算法 / `lane:ai` 数据训练 / `lane:doc` 文档答辩
- **每条泳道一个主责一个备份**，写在 `PROGRESS.md` 第 1 节
- 新建任务请走 [Issue 表单模板](../../issues/new?assignees=&labels=&projects=&template=task.yml)，不要自由写
- 发现"下一步要等别人"→ 立刻开 issue 打 `blocked`，别等组会

## 目录

```
PROGRESS.md            进度公示（单一真源，只放结论）
docs/                  协议、标定、实验记录等交付物
firmware/              H50 / STM32 端（feetech_bus / motion_ctrl / teach_mode / usb_link）
host/                  Windows 上位机 Python（camera / detect / recorder / policy / arm_link / main）
training/              数据集转换与 ACT 训练脚本
```
