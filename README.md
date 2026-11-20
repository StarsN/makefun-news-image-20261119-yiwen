[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/StarsN/makefun-news-image-20261119-yiwen/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/StarsN/makefun-news-image-20261119-yiwen/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

[make.fun bounty: Sum up 19 November's world news in one image](https://make.fun/bounty/news-image-20261119)

# The World in One Day — 19 November 2026

A newspaper front page that sums up Thursday, 19 November 2026, in a single
1024×1024 image (`entry.png`). The program (`main.ts`, Node 22, standard
library only) copies the image byte-for-byte to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`).

## The day's stories

**Lead — Three leaders, one table (Shenzhen).** The US, Chinese and Russian
leaders hold their first three-way summit on the sidelines of the APEC
meeting in Shenzhen and issue a "peace declaration" on nuclear risks and
stable energy flows, after a 90-minute meeting. No deal is announced on
Ukraine or Iran.

**World court: Myanmar committed genocide (The Hague).** The International
Court of Justice rules that Myanmar carried out state-sponsored genocide
against the Rohingya in its 2017 crackdown — the first ruling of its kind by
the UN's top court.

**The biggest IPO in history: $107.3bn (New York).** Anthropic debuts on the
Nasdaq under the ticker ANT: priced at $83 a share, it opens at $111.50
(+34%), valued near $1.5 trillion, passing SpaceX's record for the largest
IPO. The $107.3bn total includes a $26bn private placement.

**Vice City opens its doors (culture).** Grand Theft Auto VI launches after a
13-year wait, on PlayStation 5 and Xbox Series X|S — $1.84bn and more than
19 million copies on day one.

**Missile strikes Riyadh tower (Middle East).** A Houthi missile attack
damages Riyadh's tallest tower, home of the sovereign wealth fund. The US
president says no major new strikes on Iran until 2027.

**Also today (ticker).** Cyclone Akvan nears India's east coast; COP31 talks
enter their final stage over fossil fuels; Ukraine hits the Crimea bridge
again; Denmark, Greenland and the US sign an Arctic security deal.

## How the image was made

The three scene illustrations (globe over a coastal skyline, courthouse with
scales of justice, neon beach-city sunset) were generated as artwork and the
front page — masthead, headlines, captions, the IPO price chart and the
night-skyline panel — was composed with Python (PIL) in `compose.py`, so
every word in the image is crisp, legible text. Run `python3 compose.py` to
rebuild `entry.png` from the artwork in `assets/`.

## Verify

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Run it twice and compare the two outputs: they must be byte-identical.
`entry.png` is a 1024×1024 PNG under 1 MiB.

## License

MIT — see `LICENSE`.
