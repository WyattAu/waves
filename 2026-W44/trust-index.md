# trendkit trust index: 2026-10-29

Generated from 1935 tracked subjects and 16683 observations over a 8-day window by [trendkit](https://crates.io/crates/trendkit). Every number below is recomputed from the raw snapshot store; the code that computes it is public.

## Flagged subjects: 97 above the Elevated fork-ratio line

Trust blends four signals: fork ratio, membership in an org burst, velocity-outlier z, and subject age. Sorted worst first; `trust` runs 0-100.

| repo | stars | forks | ratio | trust |
|---|---:|---:|---:|---:|
| storytold/craft-libs | 325 | 620 | 191% | 0 |
| WoYun520/dsh-purge | 458 | 740 | 162% | 35 |
| Hinln/ARTEX | 907 | 1,392 | 153% | 39 |
| zgx949/ai-pojia | 368 | 494 | 134% | 46 |
| mmparko/dsh-purge | 2,396 | 2,896 | 121% | 42 |
| heqiangdiao-wq/AI-Cross-Border-Ecommerce-Agent-Toolkit | 680 | 711 | 105% | 58 |
| jddevtime/open-lakehouse-compute-fabric | 276 | 275 | 100% | 60 |
| val-tools/.github | 244 | 238 | 98% | 61 |
| cs-tool-s/.github | 244 | 216 | 89% | 64 |
| crhywun/gpt-subscribe-studio-1 | 253 | 210 | 83% | 67 |
| rbl-tools/.github | 242 | 197 | 81% | 67 |
| JeffKeeping/dsh-purge-plus | 525 | 421 | 80% | 68 |
| ZiChuanLan/agent-purge | 714 | 534 | 75% | 70 |
| david-silvalab1993i0/Roblox-Aimbot-Smooth-Tracking-Auto-Aim-Script-2026 | 307 | 217 | 71% | 71 |
| RuoJi6/ARTEX | 490 | 324 | 66% | 74 |
| i12bp8/decomp.wtf | 540 | 335 | 62% | 75 |
| anthropics/oss-scanner | 1,369 | 809 | 59% | 52 |
| CoolkHz/gptibo | 858 | 504 | 59% | 77 |
| dipa-studio/ios-sweet | 1,098 | 624 | 57% | 77 |
| reacher-z/Awesome-CUA | 233 | 130 | 56% | 78 |

## Name-cluster farms

Repo names ending in `/.github` with a best-known fork ratio over 20 percent, counted per day. These are template-deployed farms: one repository cloned across freshly created orgs, stars bought in batches. Sources observe members sporadically, so each day counts every member whose last known state had cleared the line.

| day | cluster size |
|---|---:|
| 2026-10-20 | 5 |
| 2026-10-21 | 5 |
| 2026-10-22 | 8 |
| 2026-10-23 | 8 |
| 2026-10-25 | 8 |
| 2026-10-26 | 8 |
| 2026-10-27 | 8 |
| 2026-10-28 | 8 |

The cluster grew from 5 to 8 orgs across this window.

## Method

- Fork ratio = forks per 100 stars at the latest snapshot; Elevated starts at 20 percent, Extreme near 100.
- Trust blends fork ratio, org-burst membership (3+ same-shape repos created within 5 days), velocity-outlier z, and subject age. Extreme fork verdicts cap the trust band at Watch.
- A high fork ratio alone is not fraud: this page only claims that the engagement pattern is farm-shaped. The named clusters' ratios (81-100 percent) are far beyond organic baselines (this store's median is ~7).
- Known limits: bought stars that stay under the ratio line are invisible here; deleted repos leave gaps.
