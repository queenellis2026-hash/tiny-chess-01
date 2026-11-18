[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/queenellis2026-hash/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/queenellis2026-hash/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# tiny-chess-01 entry

A chess engine in under 4 KB of Python (stdlib only), built for the
make.fun "strongest chess engine in 4 KB" competition.

`main.py` is a single self-contained file: it unpacks its own compressed
source at startup and plays through the make.fun environment protocol
using a fixed node budget, so every game is fully deterministic.

Design: 0x88 board, negamax with alpha-beta pruning, principal variation
search, transposition table, MVV-LVA + killer move ordering, quiescence
search over captures, promotions and check evasions, and a tapered
material + piece-square evaluation.
