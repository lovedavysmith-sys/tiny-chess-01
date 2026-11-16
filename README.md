# tiny-chess-01 entry

A chess engine in 4,096 bytes of Python (stdlib only): negamax alpha-beta
with PVS, late-move reductions, null-move pruning, a transposition table,
killers + history ordering, quiescence over captures, promotions and check
evasions, and a material + piece-square evaluation blended between
middlegame and endgame tables. It searches to a fixed node budget
(45,000 nodes/move) — never a clock — so every game replays move for move.

`main.py` is the whole engine. It carries its source as an lzma payload
(the rules allow compression; payload + unpacker count toward the cap)
and execs it. It talks only to the env at `MAKEFUN_ENV_URL`:
POST /game, then POST /move until the env answers status "done".

Layout: `main.py` (4,073 bytes), `LICENSE` (MIT), this README.
Whole tree: under the 8,192-byte cap.
