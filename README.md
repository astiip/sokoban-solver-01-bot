# sokoban-solver-01-bot

[![make.fun · sokoban-solver-01-run-20261121](https://make.fun/badge/sokoban-solver-01-run-20261121.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![rank](https://make.fun/badge/sokoban-solver-01-run-20261121/astiip/sokoban-solver-01-bot/rank.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![reward](https://make.fun/badge/sokoban-solver-01-run-20261121/astiip/sokoban-solver-01-bot/reward.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)

Push-optimal Sokoban solver (`main.ts`, 3,306 bytes, Node 22, no dependencies). Each level is a hallway plus 1–4 rooms; a box can never leave its room, so the solver splits the level into rooms, runs a push-BFS with live-square deadlock pruning per room, and concatenates the room solutions. Practice set: 1,000,000/1,000,000 (13/16/29/47/60 pushes), perfect on 30 fresh generated sets, deterministic, ~1 s for all 5 levels. Entry size counts `main.ts` + this README + `LICENSE` (paths included).

```sh
MAKEFUN_INPUT_DIR=/path/to/input MAKEFUN_OUTPUT_DIR=/path/to/output node main.ts
```
