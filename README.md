# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/lovedavysmith-sys/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/lovedavysmith-sys/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python (standard library only): negamax alpha-beta with PVS, late-move reductions, null-move pruning, a transposition table, killers + history ordering, and quiescence over captures, promotions and check evasions, with a material + piece-square evaluation blended between middlegame and endgame tables. It searches to a fixed budget of 47,000 nodes per move — never a clock — so every game replays move for move. On the kit's practice gauntlet it scored Elo 1451 and 1545 in two trials.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8901 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=cbeettqz&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
