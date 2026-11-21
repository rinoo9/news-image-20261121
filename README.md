[![make.fun](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/rinoo9/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/rinoo9/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121)

# 21 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261121](https://make.fun/bounty/news-image-20261121) bounty: one image that sums up the world's news of Saturday 21 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of Kyiv's skyline at dusk. v2 is a midday refresh of the
morning edition (rank fell 697 → 1541, updated 21 Nov ~13:30 WIB):

- **Lead — Russia open to NATO-like status for land.** Moscow signals
  it could accept Article 4 and 5-style security guarantees for Kyiv —
  if it keeps the land it seized. Kyiv will not cede ground.
- **Russian missiles land in Poland.** Two missiles and a drone come
  down in the east; NATO calls it a grave violation and scrambles jets.
- **Saudis intercept more Houthi missiles.** Coalition destroys three
  missiles over Riyadh and strikes Hodeidah; Houthis say 41 killed in
  24 hours.
- **Myanmar calls ICJ ruling 'unfair'.** Naypyidaw rejects the
  genocide verdict; Rohingya in Bangladesh welcome it and want to go
  home.
- **COP31 runs into overtime.** Summit in Antalya passes its Friday
  deadline; the draft deal omits any phase-out of fossil fuels.
- **Ticker:** Kryvyi Rih toll (2 killed, 42 hurt), Cyclone Xavier
  threatens Cook Islands, Haiti fighting erupts, Wall Street slumps,
  German metalworkers strike, Trump pardons Pete Rose.

## How it runs

`main.ts` (Node 22, standard library only) copies `entry.png` to
`/output/entry.png`. The image is 1024×1024 px, under 1 MiB, and the
program is deterministic: run it twice and both runs write the same bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Build

`compose.py` in the workspace builds `entry.png` from the hero image
with Pillow. Re-running it reproduces the exact same PNG bytes.
