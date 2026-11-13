# 抓取物块并放入盒子：场景资源入口

**数据已发布：180 条示范轨迹；模型、标注和实机评估待补充。**

平台：SO-ARM101。基础策略计划分别采用 ACT 与微调后的 π0.5，结合 Horizon MLP 选择执行步数。

| 内容 | 上传位置 |
|---|---|
| ACT 模型 | [models/act/block_to_box/](../../models/act/block_to_box/README.md) |
| 微调后的 π0.5 模型 | [models/pi05/block_to_box/](../../models/pi05/block_to_box/README.md) |
| MLP 权重 | [models/horizon_mlp/block_to_box/](../../models/horizon_mlp/block_to_box/README.md) |
| 任务数据 | [data/block_to_box/](../../data/block_to_box/README.md) |
| 标注与数据划分 | [data/annotations/block_to_box/](../../data/annotations/block_to_box/README.md) |
| 任务配置 | [configs/adaptive_horizon/block_to_box/](../../configs/adaptive_horizon/block_to_box/README.md) |
| 演示视频 | [media/demos/block_to_box/](../../media/demos/block_to_box/README.md) |
| 实验结果 | [results/block_to_box/](../../results/block_to_box/README.md) |

MLP 共用源码预留在 [research/adaptive_horizon](../../research/adaptive_horizon/README.md)。
物块示范数据已发布至 [GitHub Release](https://github.com/NeoWang213/adaptive-horizon-so101/releases/tag/dataset-block-to-box-20261110-180)，下载与校验见[数据说明](../../data/block_to_box/README.md)。
后续补充物体/容器规格、初始摆放、成功条件、超时、控制频率与评估次数；当前没有效果结论。
