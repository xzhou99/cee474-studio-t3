# Team 3 - Tempe - CEE 474/574 Studio, Fall 2026

**Mission.** Tempe Streetcar carries roughly 790,000 riders a year. Can your mode-choice model explain who they are?

**This repo is a scaffold, not a solution.** The data is real and frozen; the
templates are empty; STATUS.md is almost entirely *not started*. The work is
yours. Congestion and bottleneck behaviour, in particular, are NOT handled by
anything shipped here - see Open problems.

## Layout
| Where | What |
|---|---|
| `data/` | Your network and inputs - FROZEN, never edited (see data/README.md for file-by-file meaning) |
| `derived/` | Everything you compute from data/ |
| `cards/` | Model cards - start from MODEL_CARD_M1_TEMPLATE.md |
| `fig/` | Figures for the cards |
| `log/` | The contribution log (hours + evidence) - required at M1 and M2 |
| `RUNBOOK.md` | How to reproduce every number, step by step |
| `STATUS.md` | Per-item state of the project - the only progress claim that counts |
| `CONTRIBUTING.md` | Issues, status tags, commit rules |

## Start here
1. Read `data/README.md` (which file feeds which step).
2. Run Step 0 of `RUNBOOK.md` - the known-good check.
3. Open one Issue: "M1 task split" - who takes which step, by name.

## Milestones
- **M1 - Mon Oct 26:** four-step baseline + handoff tables (ADOT mid-review).
- **M2 - Wed Nov 11:** one dynamic feedback loop through the integrated model.
- **M3 - Wed Nov 18:** land-use scenario with uncertainty bounds.
Each runs on the previous one's output; your handoff blocks the next team.

## Open problems (deliberately unsolved - this is the actual studio)
- The logit coefficients in L02/L07 are classroom values. Calibrate or at least stress-test them against the observed ridership - the 2x band is a floor, not the goal.
- Fare-free years vs fares: what does a $0 fare do in your utility function, and is that the whole story?
- The campus special generator: students do not behave like the average Tempe household. Quantify how wrong the average assumption is.
- Congestion on Mill Ave at peak is a bottleneck your static auto background does not queue - does that help or hurt the streetcar in your model vs reality?

## Tools and self-study
GMNS spec: https://github.com/zephyr-data-specs/GMNS - osm2gmns docs:
https://osm2gmns.readthedocs.io - toolchain: https://github.com/asu-trans-ai-lab
(osm2gmns, grid2demand, Path4GMNS, DTALite, NeXTA). If you do not know GMNS
yet, studying it is week-1 work. Course workbooks live on Canvas, not here.

## Structure credit
Repo conventions (frozen inputs, runbook, per-item status, known-good check
first) adapted from https://github.com/scholarhaozheng/mobility-network-lab -
a former student's research repo. That is the ceiling; aim at it.
