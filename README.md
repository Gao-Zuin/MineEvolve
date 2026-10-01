# MineEvolve

在具有视觉输入的 Minecraft 多智能体任务中，研究动态进化的协作与通信方式。
计划接入 TeamCraft 和 MineLand，并借鉴 DGM 的进化搜索、TrajWiki 的记忆管理、
CommCP 的消息筛选与探索决策。目前仅建立目录骨架，尚未实现算法或环境适配。

## 预期流程

视觉观测 → 记忆更新 → 协作通信 → 行动 → 任务反馈 → 协作策略进化。

## 目录规划

```text
configs/
  tasks/                    任务配置
  agents/                   agent 配置
  communication/            通信配置
  evolution/                进化配置
src/
  environments/
    teamcraft/              TeamCraft 接入
    mineland/               MineLand 接入
  perception/               视觉观测与场景理解
  agents/                   agent 决策与行动
  memory/                   记忆与协作历史
  communication/            消息生成、筛选与路由
  evolution/                协作策略变异、选择与更新
  evaluation/               成功率、通信成本与协作效率
  runners/                  任务执行与进化循环
artifacts/
  agent_archive/            agent 版本归档
  protocol_archive/         通信协议与协作策略归档
data/
  tasks/                    任务数据
  trajectories/             交互轨迹
runs/                       实验日志、结果与检查点
scripts/                    准备与运行脚本
tests/                      测试
docs/                       设计与实验说明
```

空目录通过 `.gitkeep` 保留。生成的数据、模型、实验结果和本地环境默认不提交。

## 参考项目

- [TeamCraft](https://github.com/teamcraft-bench/teamcraft)
- [MineLand](https://github.com/cocacola-lab/MineLand)
- [DGM](https://github.com/jennyzzt/dgm)
- [TrajWiki](https://github.com/JingyuSunUOE/TrajWiki)
- [CommCP](https://github.com/tasl-lab/CommCP)
