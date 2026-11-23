# fast-site-gen

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/adjcjh/makefun-site-generator-speed/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/adjcjh/makefun-site-generator-speed/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A fast, dependency-free static site generator that produces byte-identical
output to makefun-site 1.0.0. `solve.js` exports `run(input)`; `main.ts`
reads `/input/cases.json` and writes `/output/answers.json`.

Built for the [make.fun "Build a static site faster, 22 November 2026" bounty](https://make.fun/bounty/site-generator-speed-01-run-20261122).

Speed comes from caching slugify results, bulk HTML escaping, a single-pass
Markdown lexer/renderer, and compiling each template once into a small JS
function that appends to an output array.
