[![make.fun](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/rinoo9/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/rinoo9/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121)

# 21 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261121](https://make.fun/bounty/news-image-20261121) bounty: one image that sums up the world's news of Saturday 21 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of Kyiv's skyline at dusk:

- **Lead — US offers Ukraine NATO membership for land.** Washington
  floats NATO membership for Kyiv in return for ceding territory to
  Moscow — the boldest peace offer of the war; allies divided.
- **Overnight strikes hit Kryvyi Rih.** 2 killed, 42 hurt — four of
  them children — in fresh Russian attacks; Ukraine hits the Crimean
  bridge.
- **Poland seeks NATO backing.** Warsaw turns to its allies after
  Russian missiles and drones cross into its territory.
- **ICJ: Myanmar committed genocide.** The Hague finds Myanmar guilty
  of genocide against the Rohingya — a first for any state.
- **Houthi missile hits Riyadh tower.** Debris and material damage in
  the Saudi capital; Riyadh says it intercepted further attacks.
- **Ticker:** COP31 enters final stage, JPMorgan/Visa/Mastercard hit
  in cyberattack, Cyclone Akvan aftermath, Trump pardons Pete Rose,
  Sensex +898.

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
