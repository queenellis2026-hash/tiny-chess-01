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
