# Assembling the books back out of the corpus

Every volume the manifest names, built back out of `content/` into TeX, a PDF and an EPUB, in every language that has enough of it. It is milestone 13, and the point is not that one book builds: it is that the corpus as a whole still assembles, because nothing that reads one file at a time can see a chapter missing from the middle of a volume or a § that goes from 1 to 3.

Written by `bourbaki book check -write`. Every number here is one run of the same build `bourbaki book` makes, so a row of this table and a run of that command on that volume are the same numbers.

## What it comes to

| | |
| --- | --- |
| volumes | 44 |
| builds | 140 |
| builds that reached a PDF | 140 |
| pages set | 47763 |
| formulae set | 2361744 |
| languages refused under the 10% floor | 3 |
| builds that could not be assembled | 0 |

## The checks, and how many builds each one fails

| check | builds failing |
| --- | --- |
| no footnote is printed as its own source | 24 |
| the volume holds the text the printing has | 24 |
| no TeX control sequence is loose in the prose | 4 |
| no prose character needed the fallback face | 4 |
| the numbered subsections run without a gap | 3 |
| the chapters the manifest names are all here | 1 |

## Refused under the floor

A language that holds less than 10% of the printing's sections is not bound. The last sweep before the floor existed produced twenty one four page PDFs this way, a cover and a title page and a contents of nothing, each of them passing eighteen of twenty one checks because there was no text in them to be wrong about.

| volume | language | holds |
| --- | --- | --- |
| top-v-x-fr | en-mt | holds 2 of the printing's 39 sections, under the 10% floor; the first of what is missing is content/fr/top/00_to_the_reader_v_x.md |
| lie-ii-iii-fr | en-mt | holds 1 of the printing's 23 sections, under the 10% floor; the first of what is missing is content/fr/lie/II/00_frontmatter.md |
| hist-fr | en-mt | holds 1 of the printing's 27 sections, under the 10% floor; the first of what is missing is content/fr/hist/1/01_s1_fondements_des_mathematiques_logique.md |

## Every build

| volume | language | of the printing | files | pages | printing's pages | checks passed |
| --- | --- | --- | --- | --- | --- | --- |
| ens-i-iv | en | 100% | 30 | 347 | 418 | 27 of 28 |
| ens-i-iv | fr | 100% | 30 | 339 | 418 | 26 of 28 |
| ens-i-iv | vi | 100% | 30 | 349 | 418 | 27 of 28 |
| ens-i-iv-fr | en | 100% | 30 | 347 | 349 | 27 of 28 |
| ens-i-iv-fr | fr | 100% | 30 | 339 | 349 | 26 of 28 |
| ens-i-iv-fr | vi | 100% | 30 | 349 | 349 | 27 of 28 |
| alg-i-iii | en | 100% | 41 | 743 | 734 | 27 of 28 |
| alg-i-iii | fr | 100% | 41 | 749 | 734 | 28 of 28 |
| alg-i-iii | vi | 100% | 41 | 775 | 734 | 28 of 28 |
| alg-iv-vii | en | 100% | 37 | 493 | 460 | 28 of 28 |
| alg-iv-vii | fr | 94% | 35 | 504 | 460 | 28 of 28 |
| alg-iv-vii | vi | 100% | 37 | 491 | 460 | 28 of 28 |
| alg-viii | en | 100% | 29 | 433 | 505 | 27 of 28 |
| alg-viii | fr | 100% | 29 | 439 | 505 | 27 of 28 |
| alg-viii | vi | 100% | 29 | 427 | 505 | 27 of 28 |
| alg-i-iii-fr | en | 100% | 41 | 745 | 645 | 27 of 28 |
| alg-i-iii-fr | fr | 100% | 41 | 749 | 645 | 28 of 28 |
| alg-i-iii-fr | vi | 100% | 41 | 775 | 645 | 28 of 28 |
| alg-iv-vii-fr | en | 100% | 37 | 493 | 426 | 28 of 28 |
| alg-iv-vii-fr | fr | 100% | 35 | 504 | 426 | 28 of 28 |
| alg-iv-vii-fr | vi | 100% | 37 | 491 | 426 | 28 of 28 |
| alg-viii-fr | en | 100% | 29 | 433 | 487 | 27 of 28 |
| alg-viii-fr | fr | 100% | 29 | 439 | 487 | 27 of 28 |
| alg-viii-fr | vi | 100% | 29 | 427 | 487 | 26 of 28 |
| alg-ix-fr | en | 100% | 12 | 192 | 211 | 28 of 28 |
| alg-ix-fr | en-mt | 100% | 12 | 192 | 211 | 28 of 28 |
| alg-ix-fr | fr | 100% | 12 | 197 | 211 | 28 of 28 |
| alg-ix-fr | vi | 100% | 12 | 193 | 211 | 28 of 28 |
| alg-x-fr | en | 90% | 10 | 263 | 222 | 27 of 28 |
| alg-x-fr | en-mt | 90% | 10 | 263 | 222 | 27 of 28 |
| alg-x-fr | fr | 100% | 11 | 269 | 222 | 28 of 28 |
| alg-x-fr | vi | 90% | 10 | 216 | 222 | 26 of 28 |
| top-i-iv | en | 100% | 40 | 417 | 443 | 28 of 28 |
| top-i-iv | fr | 100% | 40 | 432 | 443 | 28 of 28 |
| top-i-iv | vi | 100% | 40 | 426 | 443 | 28 of 28 |
| top-v-x | en | 100% | 38 | 347 | 372 | 28 of 28 |
| top-v-x | fr | 97% | 39 | 387 | 372 | 28 of 28 |
| top-v-x | vi | 100% | 40 | 373 | 372 | 28 of 28 |
| top-i-iv-fr | en | 100% | 40 | 419 | 367 | 28 of 28 |
| top-i-iv-fr | fr | 100% | 40 | 432 | 367 | 28 of 28 |
| top-i-iv-fr | vi | 100% | 40 | 426 | 367 | 27 of 28 |
| top-v-x-fr | en | 94% | 38 | 349 | 329 | 28 of 28 |
| top-v-x-fr | en-mt | 5% | | | 329 | refused under the floor |
| top-v-x-fr | fr | 100% | 39 | 387 | 329 | 28 of 28 |
| top-v-x-fr | vi | 100% | 40 | 373 | 329 | 27 of 28 |
| fvr-i-vii | en | 100% | 34 | 359 | 354 | 28 of 28 |
| fvr-i-vii | fr | 100% | 34 | 371 | 354 | 28 of 28 |
| fvr-i-vii | vi | 100% | 34 | 367 | 354 | 27 of 28 |
| fvr-i-vii-fr | en | 100% | 34 | 361 | 329 | 28 of 28 |
| fvr-i-vii-fr | fr | 100% | 34 | 371 | 329 | 28 of 28 |
| fvr-i-vii-fr | vi | 100% | 34 | 367 | 329 | 27 of 28 |
| evt-i-v | en | 100% | 34 | 445 | 368 | 28 of 28 |
| evt-i-v | fr | 100% | 34 | 461 | 368 | 28 of 28 |
| evt-i-v | vi | 100% | 34 | 458 | 368 | 28 of 28 |
| evt-i-v-fr | en | 100% | 34 | 445 | 372 | 28 of 28 |
| evt-i-v-fr | fr | 100% | 34 | 461 | 372 | 28 of 28 |
| evt-i-v-fr | vi | 100% | 34 | 458 | 372 | 28 of 28 |
| int-i-vi | en | 100% | 36 | 499 | 487 | 28 of 28 |
| int-i-vi | fr | 97% | 35 | 510 | 487 | 28 of 28 |
| int-i-vi | vi | 100% | 36 | 499 | 487 | 28 of 28 |
| int-vii-ix | en | 100% | 23 | 331 | 332 | 28 of 28 |
| int-vii-ix | fr | 95% | 22 | 331 | 332 | 28 of 28 |
| int-vii-ix | vi | 100% | 23 | 332 | 332 | 28 of 28 |
| int-i-iv-fr | en | 100% | 19 | 262 | 293 | 28 of 28 |
| int-i-iv-fr | fr | 100% | 19 | 279 | 293 | 28 of 28 |
| int-i-iv-fr | vi | 100% | 19 | 261 | 293 | 27 of 28 |
| int-v-fr | en | 100% | 10 | 144 | 159 | 28 of 28 |
| int-v-fr | fr | 100% | 10 | 151 | 159 | 28 of 28 |
| int-v-fr | vi | 100% | 10 | 140 | 159 | 27 of 28 |
| int-vi-fr | en | 100% | 6 | 97 | 106 | 28 of 28 |
| int-vi-fr | fr | 100% | 6 | 88 | 106 | 28 of 28 |
| int-vi-fr | vi | 100% | 6 | 101 | 106 | 28 of 28 |
| int-vii-viii-fr | en | 100% | 13 | 181 | 224 | 28 of 28 |
| int-vii-viii-fr | fr | 100% | 13 | 191 | 224 | 28 of 28 |
| int-vii-viii-fr | vi | 100% | 13 | 185 | 224 | 28 of 28 |
| int-ix-fr | en | 100% | 9 | 149 | 131 | 28 of 28 |
| int-ix-fr | fr | 100% | 9 | 143 | 131 | 28 of 28 |
| int-ix-fr | vi | 100% | 9 | 146 | 131 | 28 of 28 |
| ac-i-vii | en | 100% | 44 | 642 | 642 | 28 of 28 |
| ac-i-vii | fr | 97% | 43 | 646 | 642 | 28 of 28 |
| ac-i-vii | vi | 100% | 44 | 667 | 642 | 28 of 28 |
| ac-i-iv-fr | en | 100% | 22 | 317 | 361 | 28 of 28 |
| ac-i-iv-fr | fr | 100% | 22 | 323 | 361 | 28 of 28 |
| ac-i-iv-fr | vi | 100% | 22 | 330 | 361 | 28 of 28 |
| ac-v-vii-fr | en | 100% | 21 | 328 | 346 | 28 of 28 |
| ac-v-vii-fr | fr | 100% | 21 | 328 | 346 | 28 of 28 |
| ac-v-vii-fr | vi | 100% | 21 | 339 | 346 | 28 of 28 |
| ac-viii-ix-fr | en | 100% | 14 | 239 | 204 | 28 of 28 |
| ac-viii-ix-fr | en-mt | 100% | 14 | 239 | 204 | 28 of 28 |
| ac-viii-ix-fr | fr | 100% | 14 | 242 | 204 | 28 of 28 |
| ac-viii-ix-fr | vi | 100% | 14 | 236 | 204 | 28 of 28 |
| ac-x-fr | en | 100% | 11 | 201 | 180 | 28 of 28 |
| ac-x-fr | en-mt | 100% | 11 | 201 | 180 | 28 of 28 |
| ac-x-fr | fr | 100% | 11 | 202 | 180 | 28 of 28 |
| ac-x-fr | vi | 100% | 11 | 193 | 180 | 28 of 28 |
| var-fr | en | 100% | 10 | 85 | 190 | 27 of 28 |
| var-fr | en-mt | 100% | 10 | 85 | 190 | 27 of 28 |
| var-fr | fr | 100% | 10 | 87 | 190 | 27 of 28 |
| var-fr | vi | 100% | 10 | 84 | 190 | 27 of 28 |
| lie-i-iii | en | 100% | 31 | 485 | 481 | 27 of 28 |
| lie-i-iii | fr | 96% | 31 | 477 | 481 | 28 of 28 |
| lie-i-iii | vi | 100% | 32 | 514 | 481 | 27 of 28 |
| lie-iv-vi | en | 100% | 19 | 290 | 314 | 28 of 28 |
| lie-iv-vi | fr | 100% | 19 | 300 | 314 | 27 of 28 |
| lie-iv-vi | vi | 100% | 19 | 282 | 314 | 28 of 28 |
| lie-vii-ix | en | 100% | 34 | 437 | 439 | 27 of 28 |
| lie-vii-ix | fr | 55% | 19 | 229 | 439 | 26 of 28 |
| lie-vii-ix | vi | 100% | 34 | 437 | 439 | 27 of 28 |
| lie-i-fr | en | 100% | 8 | 126 | 144 | 27 of 28 |
| lie-i-fr | fr | 100% | 8 | 127 | 144 | 28 of 28 |
| lie-i-fr | vi | 100% | 8 | 122 | 144 | 27 of 28 |
| lie-ii-iii-fr | en | 95% | 22 | 361 | 318 | 28 of 28 |
| lie-ii-iii-fr | en-mt | 4% | | | 318 | refused under the floor |
| lie-ii-iii-fr | fr | 100% | 23 | 353 | 318 | 28 of 28 |
| lie-ii-iii-fr | vi | 100% | 23 | 392 | 318 | 28 of 28 |
| lie-iv-vi-fr | en | 100% | 19 | 290 | 284 | 28 of 28 |
| lie-iv-vi-fr | fr | 100% | 19 | 300 | 284 | 27 of 28 |
| lie-iv-vi-fr | vi | 100% | 19 | 282 | 284 | 27 of 28 |
| lie-vii-viii-fr | en | 100% | 8 | 74 | 61 | 28 of 28 |
| lie-vii-viii-fr | fr | 100% | 7 | 74 | 61 | 28 of 28 |
| lie-vii-viii-fr | vi | 100% | 8 | 74 | 61 | 28 of 28 |
| lie-ix-fr | en | 100% | 12 | 159 | 141 | 28 of 28 |
| lie-ix-fr | fr | 100% | 12 | 161 | 141 | 28 of 28 |
| lie-ix-fr | vi | 100% | 12 | 157 | 141 | 28 of 28 |
| ts-i-ii-fr | en | 100% | 15 | 295 | 346 | 28 of 28 |
| ts-i-ii-fr | en-mt | 100% | 15 | 295 | 346 | 28 of 28 |
| ts-i-ii-fr | fr | 100% | 15 | 297 | 346 | 28 of 28 |
| ts-i-ii-fr | vi | 100% | 15 | 249 | 346 | 27 of 28 |
| ts-iii-v-fr | en | 100% | 21 | 500 | 579 | 27 of 28 |
| ts-iii-v-fr | en-mt | 100% | 21 | 500 | 579 | 27 of 28 |
| ts-iii-v-fr | fr | 100% | 21 | 504 | 579 | 27 of 28 |
| ts-iii-v-fr | vi | 100% | 21 | 452 | 579 | 26 of 28 |
| ta-i-iv-fr | en | 100% | 28 | 433 | 512 | 27 of 28 |
| ta-i-iv-fr | en-mt | 100% | 28 | 433 | 512 | 27 of 28 |
| ta-i-iv-fr | fr | 100% | 28 | 437 | 512 | 27 of 28 |
| ta-i-iv-fr | vi | 100% | 28 | 424 | 512 | 26 of 28 |
| hist | en | 100% | 26 | 286 | 299 | 27 of 28 |
| hist | fr | 100% | 26 | 295 | 299 | 28 of 28 |
| hist | vi | 100% | 26 | 291 | 299 | 26 of 28 |
| hist-fr | en | 100% | 27 | 288 | 374 | 26 of 28 |
| hist-fr | en-mt | 3% | | | 374 | refused under the floor |
| hist-fr | fr | 100% | 27 | 297 | 374 | 28 of 28 |
| hist-fr | vi | 100% | 27 | 293 | 374 | 26 of 28 |
