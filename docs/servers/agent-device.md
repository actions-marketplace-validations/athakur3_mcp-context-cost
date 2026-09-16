# agent-device — context cost

**48,909 tokens** across 57 tools — *very heavy* (≥ 30K). Measured 2026-09-16 under [methodology v1.0](../METHODOLOGY.html).

An Anthropic request carries 33,319 of those tokens as tool definitions. What Claude makes of them is not published for this server: its Claude count is missing, or was taken against a capture this measurement has since replaced.

| | |
|---|---|
| server (self-reported) | agent-device v0.21.4 |
| status | measured |
| tokenizer | tiktoken / o200k_base |
| launch command | `npx -y agent-device mcp` |
| isolation | docker · public.ecr.aws/docker/library/node:22-slim · network bridge · linux/amd64 · network enabled for package fetch; clean FS, no host credentials |
| env vars supplied | none |
| canonical SHA-256 | `3405333902a4a368c930626f35a1c4cd947ab9cdc0e88e81963165028de16c55` |
| category | community |
| source | https://github.com/callstack/agent-device |

## Where the tokens are

| tool | tokens | share | description | input schema | output schema |
|---|---:|---:|---:|---:|---:|
| fill | 4,848 | 9.9% | 68 | 840 | 3,929 |
| click | 2,844 | 5.8% | 67 | 881 | 1,885 |
| press | 2,796 | 5.7% | 46 | 854 | 1,885 |
| longpress | 2,612 | 5.3% | 50 | 745 | 1,805 |
| hover | 2,605 | 5.3% | 72 | 726 | 1,796 |
| scroll | 1,535 | 3.1% | 125 | 655 | 744 |
| back | 1,208 | 2.5% | 44 | 546 | 607 |
| open | 1,029 | 2.1% | 93 | 927 | 0 |
| record | 994 | 2.0% | 46 | 502 | 435 |
| find | 993 | 2.0% | 19 | 590 | 373 |
| gesture | 852 | 1.7% | 42 | 801 | 0 |
| replay | 773 | 1.6% | 42 | 612 | 107 |
| test | 753 | 1.5% | 19 | 587 | 136 |
| doctor | 752 | 1.5% | 78 | 461 | 202 |
| batch | 746 | 1.5% | 15 | 722 | 0 |
| snapshot | 694 | 1.4% | 46 | 639 | 0 |
| get | 689 | 1.4% | 37 | 643 | 0 |
| wait | 687 | 1.4% | 64 | 535 | 77 |
| keyboard | 678 | 1.4% | 65 | 449 | 153 |
| diff | 672 | 1.4% | 31 | 484 | 146 |
| metro | 666 | 1.4% | 71 | 586 | 0 |
| is | 657 | 1.3% | 67 | 581 | 0 |
| trace | 648 | 1.3% | 41 | 457 | 139 |
| perf | 647 | 1.3% | 70 | 568 | 0 |
| tv-remote | 645 | 1.3% | 55 | 508 | 69 |
| appstate | 621 | 1.3% | 11 | 416 | 182 |
| shutdown | 621 | 1.3% | 14 | 416 | 180 |
| screenshot | 617 | 1.3% | 37 | 570 | 0 |
| push | 607 | 1.2% | 17 | 467 | 112 |
| swipe | 605 | 1.2% | 15 | 580 | 0 |

*27 smaller tools omitted (13,813 tokens combined) — all of them are in the [raw capture](https://github.com/athakur3/mcp-context-cost/blob/main/results/agent-device/measurement.json).*

Each tool is tokenized on its own, so the parts do not sum exactly to the whole: the array adds its own brackets and commas, and the tokenizer merges tokens across object boundaries. The badge number is always the count of the whole array, never a sum of parts.

## Over time

| date | tokens | tools | release | measured in | change |
|---|---:|---:|---|---|---:|
| 2026-09-04 | 53,669 | 57 | 0.20.10 | docker | — |
| 2026-09-16 | 48,909 | 57 | 0.21.4 | docker | −4,760 |

Full series: [results/history.csv](https://github.com/athakur3/mcp-context-cost/blob/main/results/history.csv).

## Re-derive it

```bash
npx -y mcp-context-cost verify results/agent-device/measurement.json
```

That re-tokenizes the [published capture](https://github.com/athakur3/mcp-context-cost/blob/main/results/agent-device/measurement.json) and checks the count and the hash. If it disagrees with the badge, the badge is wrong — [open an issue](https://github.com/athakur3/mcp-context-cost/issues) and it gets corrected.

[Badge JSON](https://github.com/athakur3/mcp-context-cost/blob/main/badges/agent-device.json) · [All servers](index.html) · [Leaderboard](https://github.com/athakur3/mcp-context-cost/blob/main/results/leaderboard.md) · [Methodology](../METHODOLOGY.html)
