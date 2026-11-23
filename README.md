# tiny-chess-01 entry

A chess engine in 4 KB of Python: alpha-beta search with a transposition
table, quiescence over captures, promotions and check evasions, MVV-LVA,
killer and history move ordering, and material plus piece-square evaluation.
It searches to a fixed node budget (never a clock), so replays match.
main.py is the whole engine; it plays the gauntlet through MAKEFUN_ENV_URL.
