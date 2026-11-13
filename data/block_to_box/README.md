# 物块放盒：180 条示范数据

数据集：`demo_20261110_180`。SO-ARM101 抓取蓝色物块并放入盒子。

| 项目 | 内容 |
|---|---|
| 格式 | LeRobot v2.1 |
| 轨迹 / 总帧数 | 180 / 58,654 |
| 相机 | handeye + front，640 × 480，30 FPS，AV1 |
| 视频数量 | 360（每条轨迹两个视角） |
| 状态 / 动作 | 6 维关节位置 |
| 任务指令 | `put the blue cube into the box` |
| 数据划分 | 原始元数据为 train `0:180`；尚未提供独立验证或测试集 |
| 数据许可 | 尚未单独指定 |

## 下载和解压

[完整数据包](https://github.com/NeoWang213/adaptive-horizon-so101/releases/download/dataset-block-to-box-20261110-180/demo_20261110_180.zip) · [SHA-256 校验文件](https://github.com/NeoWang213/adaptive-horizon-so101/releases/download/dataset-block-to-box-20261110-180/SHA256SUMS.txt)

```powershell
curl.exe -L --fail -o demo_20261110_180.zip "https://github.com/NeoWang213/adaptive-horizon-so101/releases/download/dataset-block-to-box-20261110-180/demo_20261110_180.zip"
Get-FileHash ./demo_20261110_180.zip -Algorithm SHA256
Expand-Archive -LiteralPath ./demo_20261110_180.zip -DestinationPath ./datasets
```

解压后数据根目录为 `datasets/demo_20261110_180/`，其中保留 `data/`、`meta/`、
`videos/` 和原始 `merge_report.json`；训练时将数据根路径指向此目录。
数据集已发布，完整资源信息见 [manifest.json](manifest.json)。

SHA-256：`547fcff1fcec7ac3dc04e188270b19497ab69c88d6ca31226683aed31d85e8bd`。

本次打包检查了全部 Parquet 的帧数与索引、360 个视频与原始合并报告的 SHA-256
一致性，以及 ZIP 的文件数和 CRC。原始合并报告另记录了视频解码、时间戳及
LeRobot episode 边界验证。本次未重新完整解码全部视频，也未逐条评估任务成功率。

