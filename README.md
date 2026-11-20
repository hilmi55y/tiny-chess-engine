# tiny-chess-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/hilmi55y/tiny-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/hilmi55y/tiny-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact chess engine in 4 KB of Python: tapered PeSTO evaluation, PVS with null-move pruning and late-move reduction, transposition table, killer-move ordering, quiescence search over captures and check evasions, and per-opponent fixed node budgets. The entry is a single self-contained `main.py` (an LZMA-compressed payload with a tiny unpacker) that plays the make.fun tiny-chess-01 gauntlet through the env at `MAKEFUN_ENV_URL`.

## Run it

```sh
python3 main.py
```

## Practice results

Three practice trials against the house gauntlet (6 games each): trial-0 3.5/6, Elo 1364; trial-1 3/6, Elo 1279; trial-2 3/6, Elo 1279 — mean Elo about 1307, above the 1154 practice floor. The entry is built from the source in `main_minified.py` with the kit's `makefun compress`, so the packed `main.py` is byte-for-byte the kit's own compression of that source.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ky8x585w&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
