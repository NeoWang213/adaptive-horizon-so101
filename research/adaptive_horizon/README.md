# Horizon MLP 模块：待上传

这里预留正式的自适应执行步数模块。当前只有结构与说明，没有新增训练或部署实现。

| 子目录 | 后续内容 |
|---|---|
| `features/` | MLP 输入特征及预处理 |
| `labels/` | Horizon 监督标签的定义与生成 |
| `models/` | MLP 网络结构 |
| `runtime/` | ACT 与 π0.5 的执行长度选择与接入 |

后续可以在本目录添加训练与评估入口。上传时应说明输入/输出、候选 horizon、
归一化方式、适配策略、训练数据划分和用法。权重说明放在
[models/horizon_mlp](../../models/horizon_mlp/README.md)，大文件可通过外部仓库链接提供。
