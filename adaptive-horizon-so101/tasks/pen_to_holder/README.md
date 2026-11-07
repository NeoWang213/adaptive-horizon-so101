# 捡起笔并放入笔筒：场景资源入口

**状态：待上传、待验证。**

平台：SO-ARM101。基础策略计划分别采用 ACT 与微调后的 π0.5，结合 Horizon MLP 选择执行步数。

| 内容 | 上传位置 |
|---|---|
| ACT 模型 | [models/act/pen_to_holder/](../../models/act/pen_to_holder/README.md) |
| 微调后的 π0.5 模型 | [models/pi05/pen_to_holder/](../../models/pi05/pen_to_holder/README.md) |
| MLP 权重 | [models/horizon_mlp/pen_to_holder/](../../models/horizon_mlp/pen_to_holder/README.md) |
| 任务数据 | [data/pen_to_holder/](../../data/pen_to_holder/README.md) |
| 标注与数据划分 | [data/annotations/pen_to_holder/](../../data/annotations/pen_to_holder/README.md) |
| 任务配置 | [configs/adaptive_horizon/pen_to_holder/](../../configs/adaptive_horizon/pen_to_holder/README.md) |
| 演示视频 | [media/demos/pen_to_holder/](../../media/demos/pen_to_holder/README.md) |
| 实验结果 | [results/pen_to_holder/](../../results/pen_to_holder/README.md) |

MLP 共用源码预留在 [research/adaptive_horizon](../../research/adaptive_horizon/README.md)。
模型和原始数据可放在 Hugging Face Hub，在对应目录填写固定版本下载链接。
后续补充物体/容器规格、初始摆放、成功条件、超时、控制频率与评估次数；当前没有效果结论。
