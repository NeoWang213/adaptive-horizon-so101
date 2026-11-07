# 新场景模板

复制本目录为 `tasks/<task_id>/`，将 `<task_id>` 替换为简短英文标识，填写任务名称、
任务说明、成功条件和资源清单，并在 `tasks/README.md` 与首页任务表中加入入口。

按需创建以下对应位置；每个目录放 README，GitHub 才能保留该目录：

```text
tasks/<task_id>/                         场景说明与资源清单
models/act/<task_id>/                    ACT 模型说明/下载链接
models/pi05/<task_id>/                   微调后的 π0.5 说明/下载链接
models/horizon_mlp/<task_id>/             MLP 权重说明/下载链接
data/<task_id>/                          数据说明/下载链接
data/annotations/<task_id>/              标注与 episode 划分
configs/adaptive_horizon/<task_id>/      任务配置
media/demos/<task_id>/                   演示说明/链接
results/<task_id>/                       对比结果与图表
```

`manifest.example.json` 中的目录是填写模板，尚未创建其他实际任务或发布任何资源。
大文件建议外部托管，填入固定 revision、许可与适配版本。
现有忽略规则允许模型/数据目录内的 README 和 manifest JSON；原始数据与权重默认忽略。
