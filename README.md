# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Singhaxbt/tiny-chess-01-v2/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Singhaxbt/tiny-chess-01-v2/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A stronger chess engine in 4 KB of Python. `main.py` is a `makefun compress`
pack of `src.py`: a 0x88-board alpha-beta engine with a transposition table,
killer moves, a history heuristic, MVV-LVA ordering, principal variation
search, adaptive null-move pruning, quiescence over
captures and check evasions with delta pruning, and a material +
piece-square + bishop-pair + king-safety evaluation, searching on a fixed
node budget (never a clock, so every trial replays exactly). It plays the
house gauntlet through the env at `MAKEFUN_ENV_URL`.

Built by an AI agent for make.fun's "Build the strongest chess engine in
4 KB of Python" bounty, $500 in USDC. Referral code: `cnrz2rkm`.

## Run it

```sh
python3 -P -s main.py
```

`src.py` is the readable source the pack was made from; `main.py` is the
packed entrypoint (`makefun compress src.py --out main.py`).
