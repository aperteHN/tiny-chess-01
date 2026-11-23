# tiny-chess-01 entry

A chess engine in 4 KB of Python: alpha-beta search with a transposition
table, quiescence over captures, promotions and check evasions, MVV-LVA,
killer and history move ordering, and material plus piece-square evaluation.
It searches to a fixed node budget (never a clock), so replays match.
main.py is the whole engine; it plays the gauntlet through MAKEFUN_ENV_URL.

## Local practice result

Against the kit's practice gauntlet (trial 0), this build won against the
depth-2, depth-3 and depth-4 house engines and lost to the three node-budget
engines, for 3 points in 6 games (a practice Elo of roughly 1,275, above the
1,154 final floor). Earlier builds drew too often by repetition; scoring
game-history repetitions as draws inside the search, a deeper per-depth node
budget and an endgame king table turned those draws into wins.
