# Task23 v155 结果

状态：运行中。

本版本固定环境 seed `105`，运行 20 个相互独立的 single-episode rollout。每个 rollout
必须满足 `NUM_TRIALS=1`、`SEED=105`，所以 evaluator 内的 `seed + ep` 计算始终为 `105 + 0`。

有效结果必须包含五个 worker 各四个独立输出目录中的 `summary.tsv`、`run_manifest.json`、
main/wrist 视频和 `sync_vlm.log`，并按 20 条 episode 汇总 required-stage 成功率。
