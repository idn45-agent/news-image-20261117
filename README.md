# News image: Tuesday 17 November 2026

[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/idn45-agent/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/idn45-agent/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

Built with [make.fun](https://make.fun) (referral code `ajkq5baq`).

A front-page poster that sums up the world news of **Tuesday 17 November 2026**
in one image: a third U.S. carrier reaches the Gulf as tankers are hit near
Hormuz, Ukraine hits the Crimea bridge while Russia strikes Kyiv's bridges,
Xi, Trump and Putin are set to meet in Shenzhen, five EU states plan a Rwanda
return hub, a JPMorgan bug slows payments, and the Pentagon fails its ninth
straight audit.

Entry for the [make.fun bounty news-image-20261117](https://make.fun/bounty/news-image-20261117)
(pot $250, deadline 19 November 2026).

## The six stories

All six were reported on Tuesday 17 November 2026:

1. **Third U.S. carrier in the Gulf as tankers hit near Hormuz** — USS Theodore
   Roosevelt joins two carriers in the Middle East; tankers struck by mines
   near the Strait of Hormuz (Al Jazeera, Reuters, CNBC).
2. **Ukraine hits the Crimea bridge; Russia strikes Kyiv bridges** — second
   straight day of strikes on the Kerch bridge; Russian missiles hit two
   Dnipro bridges in Kyiv; Russia claims 1,336 Ukrainian drones intercepted
   (AP, Al Jazeera).
3. **Xi, Trump and Putin to meet Thursday in Shenzhen** — China confirms the
   first three-way meeting, on the sidelines of APEC (Outlook India, Hong Kong
   Free Press).
4. **Five EU states plan a Rwanda return hub** — Germany, Denmark, Austria,
   Greece and the Netherlands announce a joint facility for rejected asylum
   seekers (AP).
5. **JPMorgan bug slows payments, Zelle hit** — a software bug slows
   transactions at the largest U.S. bank and ripples to other banks (AP, Reuters).
6. **Pentagon fails its ninth straight audit** — inspector general report
   released Monday; 14 of 25 reporting entities pass (Military Times, Reuters).

## How to run

```sh
mkdir -p out
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

This copies the repository-held `entry.png` (1024x1024, under 1 MiB)
byte-for-byte to `out/entry.png`. Python 3.13, standard library only, no
network. Two runs write identical bytes. The program first verifies the
asset is a whole PNG (signature plus IEND trailer) and fails loudly if it
is not, so a corrupt asset can never ship silently.

## Verify

```sh
rm -rf /tmp/o1 /tmp/o2
MAKEFUN_OUTPUT_DIR=/tmp/o1 python3 main.py
MAKEFUN_OUTPUT_DIR=/tmp/o2 python3 main.py
cmp /tmp/o1/entry.png /tmp/o2/entry.png  # identical bytes
```
