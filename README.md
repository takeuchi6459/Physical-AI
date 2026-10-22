# Physical-AI 応用1 最終課題
## 概要
日本語の指示を LLM（Qwen2.5-3B-Instruct）が行動プランに変換し、強化学習（Brax PPO）で学習した歩行ポリシーが人型ロボット Unitree G1 を MuJoCo 上で歩かせます。

## 実行順（Google Colab, T4 GPU）

| 順番 | ファイル | 内容 |
|---|---|---|
| 1 | `01_train_g1.ipynb` | G1 の歩行を PPO で学習（追加学習も可）。パラメータを Drive に保存 |
| 2 | `03a_llm_plans.ipynb` | 日本語の指示 → プランJSON を Drive の `plans/` に保存 |
| 3 | `03b_run_plans.ipynb` | `plans/*.json` を読んで G1 を歩かせ、動画を表示（前半: v1、後半: 追加学習後の v2） |

