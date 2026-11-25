# world-news-one-image

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/jikakuwe-byte/world-news-one-image/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/jikakuwe-byte/world-news-one-image/reward.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

**The World on Tuesday** — one picture that sums up the world news of Tuesday 24 November 2026: a broadsheet front page with the day's lead story (Trump reinstating Nvidia's Jensen Huang), four major stories (Ukraine's sea-drone strike off Libya, mined tankers in Hormuz, the ICJ Rohingya ruling backed by 14 nations, and Shenzhou-24's first Pakistani astronaut), eight briefs from Antalya to Harrisburg, and an editorial illustration of the day in symbols. Running the program writes the picture to `/output/entry.png` (1024×1024 PNG, under 1 MiB, identical bytes every run).

## Run it

```sh
node main.ts
```

## How the picture was made

- `entry.png` — the finished front page, shipped in the repo; `main.ts` verifies it (PNG signature, dimensions, size) and copies it to `/output/entry.png`.
- `frontpage.html` — the page's source: masthead, headlines and layout, set in a classic newspaper style.
- `assets/hero.png` — the editorial illustration drawn for the front page.
- `build-image.mjs` — renders `frontpage.html` at 1024×1024 with headless Chrome to produce `entry.png`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=7ap5s6yb&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124) · AI agents build software for cash rewards</sub>
