[English project overview](README.md)

# DIKWP MESH Worldline-12 OS

Created by Yucong Duan (段玉聪).

12-month determinacy boundaries, accident triggers, calibrated forecasts and branch-robust action.

基准日：2026-07-18；预测窗口：2026-07-18 至 2027-07-18。

本系统不把“未来”主观定义为单一路径，也不把概率包装为确定事实。它将世界议题注册为时间戳化、可结算的 Forecast Card，并通过 DIKWP×DIKWP 网状路径组织观察、区分、模型、权衡与目的修订。输出包括：日历锁定项、结构驱动项、触发信号、事故表面、分支情景、Residual、可逆行动和校准记录。

## Quick start

```bash
python src/worldline12_runtime.py list
python src/worldline12_runtime.py update --forecast F03 --lr 0.70 1.25
python src/worldline12_runtime.py demo
python src/worldline12_gateway.py --port 8792
python -m unittest discover -s src -v
```

打开 `prototype/index.html` 可离线选择 Forecast、输入 Likelihood Ratio、评估 Accident Surface、查看 DIKWP Semantic Contract，并导出 Replay Bundle。

## Main artifacts

- `docs/03_Twelve_Month_Forecast_Book.docx`: 25项未来12个月可结算预测。
- `DIKWP_Worldline12_Forecast_and_Calibration_Matrix.xlsx`: 预测、触发、更新、事故表面、校准与行动矩阵。
- `data/forecast_registry.json`: 机器可读 Forecast Registry。
- `src/worldline12_runtime.py`: 确定性参考运行时。
- `src/worldline12_gateway.py`: 本地HTTP参考网关。
- `api_openapi.yaml`: OpenAPI 3.1接口草案。
- `source_ledger.md`: 当前来源与证据边界。

## Non-claims

- 不保证偶发历史事件的精确发生方式。
- 不将“高概率”解释为必然。
- 不提供个性化投资、交易或政治操纵建议。
- 不把历史类比当作历史重复定律。
- 不把 D/I/K/W/P 写成单向本体阶梯；具体路径始终由任务、观察者、证据与目的索引。
