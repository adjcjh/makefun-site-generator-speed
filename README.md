# fast-site-gen

A fast, dependency-free static site generator that produces byte-identical
output to makefun-site 1.0.0. `solve.js` exports `run(input)`; `main.ts`
reads `/input/cases.json` and writes `/output/answers.json`.

Speed comes from caching slugify results, bulk HTML escaping, a single-pass
Markdown lexer/renderer, and compiling each template once into a small JS
function that appends to an output array.
