# waves

The public measurement record of the [trendkit](https://github.com/WyattAu/trendkit)
platform: weekly trend reports and the trust index, generated from raw
snapshot data and committed here so every past claim stays auditable.

Everything in this repo is **generated, not opinion**. Each number traces to
observations in the trendkit SQLite store, and the code that computes it is
public and published on crates.io. Where the data says a wave accelerated,
the report says so; where it cooled, the report says that too.

## Layout

```
2026-W43/
  weekly.md         the weekly trend report (velocity, shapes, persistence, topics)
  trust-index.md    flagged subjects, name-cluster farms, method
```

One directory per ISO week, named `YYYY-Www`, written once and never edited
after the fact. Corrections appear as new files that cite what they fix.

## Method, in one paragraph

trendkit snapshots GitHub trending/search, Hacker News, crates.io downloads,
and HuggingFace models into SQLite every morning. Velocity is the day-over-day
delta of each subject's headline counter; shape classification splits
accelerating from decelerating by comparing first-half and second-half average
velocities; trust scoring blends fork ratio, org-burst membership, velocity
outliers, and subject age. Forecasts are persisted and scored against the next
day's actuals; the verification record ships in each weekly report.

## Regenerating

```sh
cargo install trendkit
trendkit report --out weekly.md --markdown --integrity --topics 8 \
  --persistent 2 --shapes 2 --forecast 6
trendkit report --trust-page trust-index.md
```

## License

The reports are data about public repositories. Code samples in reports are
Apache-2.0 like trendkit itself.
