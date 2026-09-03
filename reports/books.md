# Assembling the books back out of the corpus

Every volume the manifest names, built back out of `content/` into TeX, a PDF and an EPUB, in every language that has enough of it. It is milestone 13, and the point is not that one book builds: it is that the corpus as a whole still assembles, because nothing that reads one file at a time can see a chapter missing from the middle of a volume or a § that goes from 1 to 3.

Written by `bourbaki book check -write`. Every number here is one run of the same build `bourbaki book` makes, so a row of this table and a run of that command on that volume are the same numbers.

## What it comes to

| | |
| --- | --- |
| volumes | 44 |
| builds | 140 |
| builds that reached a PDF | 140 |
| pages set | 47906 |
| formulae set | 2348386 |
| languages refused under the 10% floor | 3 |
| builds that could not be assembled | 0 |

## The checks, and how many builds each one fails

| check | builds failing |
| --- | --- |
| the volume holds the text the printing has | 26 |
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
| ens-i-iv | en | 100% | 32 | 374 | 418 | 31 of 32 |
| ens-i-iv | fr | 100% | 32 | 362 | 418 | 31 of 32 |
| ens-i-iv | vi | 100% | 30 | 349 | 418 | 31 of 32 |
| ens-i-iv-fr | en | 100% | 32 | 374 | 349 | 31 of 32 |
| ens-i-iv-fr | fr | 100% | 32 | 362 | 349 | 31 of 32 |
| ens-i-iv-fr | vi | 100% | 30 | 349 | 349 | 31 of 32 |
| alg-i-iii | en | 100% | 43 | 755 | 734 | 32 of 32 |
| alg-i-iii | fr | 100% | 43 | 756 | 734 | 32 of 32 |
| alg-i-iii | vi | 100% | 41 | 775 | 734 | 32 of 32 |
| alg-iv-vii | en | 100% | 39 | 494 | 460 | 32 of 32 |
| alg-iv-vii | fr | 94% | 37 | 506 | 460 | 32 of 32 |
| alg-iv-vii | vi | 100% | 37 | 491 | 460 | 32 of 32 |
| alg-viii | en | 100% | 31 | 449 | 505 | 32 of 32 |
| alg-viii | fr | 100% | 31 | 455 | 505 | 32 of 32 |
| alg-viii | vi | 100% | 29 | 427 | 505 | 32 of 32 |
| alg-i-iii-fr | en | 100% | 43 | 757 | 645 | 32 of 32 |
| alg-i-iii-fr | fr | 100% | 43 | 758 | 645 | 32 of 32 |
| alg-i-iii-fr | vi | 100% | 41 | 775 | 645 | 32 of 32 |
| alg-iv-vii-fr | en | 100% | 39 | 494 | 426 | 32 of 32 |
| alg-iv-vii-fr | fr | 100% | 37 | 506 | 426 | 32 of 32 |
| alg-iv-vii-fr | vi | 100% | 37 | 491 | 426 | 32 of 32 |
| alg-viii-fr | en | 100% | 31 | 449 | 487 | 32 of 32 |
| alg-viii-fr | fr | 100% | 31 | 455 | 487 | 32 of 32 |
| alg-viii-fr | vi | 100% | 29 | 427 | 487 | 31 of 32 |
| alg-ix-fr | en | 100% | 12 | 192 | 211 | 32 of 32 |
| alg-ix-fr | en-mt | 100% | 12 | 192 | 211 | 32 of 32 |
| alg-ix-fr | fr | 100% | 14 | 200 | 211 | 32 of 32 |
| alg-ix-fr | vi | 100% | 12 | 193 | 211 | 32 of 32 |
| alg-x-fr | en | 90% | 10 | 263 | 222 | 32 of 32 |
| alg-x-fr | en-mt | 90% | 10 | 263 | 222 | 32 of 32 |
| alg-x-fr | fr | 100% | 13 | 270 | 222 | 32 of 32 |
| alg-x-fr | vi | 90% | 10 | 216 | 222 | 31 of 32 |
| top-i-iv | en | 100% | 42 | 427 | 443 | 32 of 32 |
| top-i-iv | fr | 100% | 42 | 434 | 443 | 32 of 32 |
| top-i-iv | vi | 100% | 40 | 426 | 443 | 32 of 32 |
| top-v-x | en | 100% | 40 | 353 | 372 | 32 of 32 |
| top-v-x | fr | 97% | 41 | 385 | 372 | 32 of 32 |
| top-v-x | vi | 100% | 40 | 373 | 372 | 32 of 32 |
| top-i-iv-fr | en | 100% | 42 | 429 | 367 | 32 of 32 |
| top-i-iv-fr | fr | 100% | 42 | 434 | 367 | 32 of 32 |
| top-i-iv-fr | vi | 100% | 40 | 426 | 367 | 31 of 32 |
| top-v-x-fr | en | 94% | 40 | 355 | 329 | 31 of 32 |
| top-v-x-fr | en-mt | 5% | | | 329 | refused under the floor |
| top-v-x-fr | fr | 100% | 41 | 385 | 329 | 32 of 32 |
| top-v-x-fr | vi | 100% | 40 | 373 | 329 | 31 of 32 |
| fvr-i-vii | en | 100% | 36 | 366 | 354 | 32 of 32 |
| fvr-i-vii | fr | 100% | 36 | 372 | 354 | 32 of 32 |
| fvr-i-vii | vi | 100% | 34 | 367 | 354 | 32 of 32 |
| fvr-i-vii-fr | en | 100% | 36 | 368 | 329 | 32 of 32 |
| fvr-i-vii-fr | fr | 100% | 36 | 372 | 329 | 32 of 32 |
| fvr-i-vii-fr | vi | 100% | 34 | 367 | 329 | 32 of 32 |
| evt-i-v | en | 100% | 36 | 441 | 368 | 32 of 32 |
| evt-i-v | fr | 100% | 36 | 457 | 368 | 32 of 32 |
| evt-i-v | vi | 100% | 34 | 458 | 368 | 32 of 32 |
| evt-i-v-fr | en | 100% | 36 | 441 | 372 | 32 of 32 |
| evt-i-v-fr | fr | 100% | 36 | 457 | 372 | 32 of 32 |
| evt-i-v-fr | vi | 100% | 34 | 458 | 372 | 32 of 32 |
| int-i-vi | en | 100% | 38 | 500 | 487 | 32 of 32 |
| int-i-vi | fr | 97% | 35 | 492 | 487 | 32 of 32 |
| int-i-vi | vi | 100% | 36 | 499 | 487 | 32 of 32 |
| int-vii-ix | en | 100% | 25 | 329 | 332 | 32 of 32 |
| int-vii-ix | fr | 95% | 22 | 321 | 332 | 32 of 32 |
| int-vii-ix | vi | 100% | 23 | 332 | 332 | 32 of 32 |
| int-i-iv-fr | en | 100% | 19 | 262 | 293 | 32 of 32 |
| int-i-iv-fr | fr | 100% | 21 | 275 | 293 | 32 of 32 |
| int-i-iv-fr | vi | 100% | 19 | 261 | 293 | 31 of 32 |
| int-v-fr | en | 100% | 10 | 144 | 159 | 32 of 32 |
| int-v-fr | fr | 100% | 11 | 151 | 159 | 32 of 32 |
| int-v-fr | vi | 100% | 10 | 140 | 159 | 31 of 32 |
| int-vi-fr | en | 100% | 6 | 84 | 106 | 32 of 32 |
| int-vi-fr | fr | 100% | 8 | 90 | 106 | 32 of 32 |
| int-vi-fr | vi | 100% | 6 | 101 | 106 | 32 of 32 |
| int-vii-viii-fr | en | 100% | 13 | 181 | 224 | 32 of 32 |
| int-vii-viii-fr | fr | 100% | 15 | 190 | 224 | 32 of 32 |
| int-vii-viii-fr | vi | 100% | 13 | 185 | 224 | 32 of 32 |
| int-ix-fr | en | 100% | 9 | 138 | 131 | 32 of 32 |
| int-ix-fr | fr | 100% | 11 | 146 | 131 | 32 of 32 |
| int-ix-fr | vi | 100% | 9 | 146 | 131 | 32 of 32 |
| ac-i-vii | en | 100% | 46 | 647 | 642 | 32 of 32 |
| ac-i-vii | fr | 97% | 43 | 628 | 642 | 32 of 32 |
| ac-i-vii | vi | 100% | 44 | 667 | 642 | 32 of 32 |
| ac-i-iv-fr | en | 100% | 22 | 317 | 361 | 32 of 32 |
| ac-i-iv-fr | fr | 100% | 24 | 325 | 361 | 32 of 32 |
| ac-i-iv-fr | vi | 100% | 22 | 330 | 361 | 32 of 32 |
| ac-v-vii-fr | en | 100% | 21 | 320 | 346 | 32 of 32 |
| ac-v-vii-fr | fr | 100% | 23 | 325 | 346 | 32 of 32 |
| ac-v-vii-fr | vi | 100% | 21 | 339 | 346 | 32 of 32 |
| ac-viii-ix-fr | en | 100% | 14 | 239 | 204 | 32 of 32 |
| ac-viii-ix-fr | en-mt | 100% | 14 | 239 | 204 | 32 of 32 |
| ac-viii-ix-fr | fr | 100% | 16 | 243 | 204 | 32 of 32 |
| ac-viii-ix-fr | vi | 100% | 14 | 236 | 204 | 32 of 32 |
| ac-x-fr | en | 100% | 11 | 201 | 180 | 32 of 32 |
| ac-x-fr | en-mt | 100% | 11 | 201 | 180 | 32 of 32 |
| ac-x-fr | fr | 100% | 11 | 202 | 180 | 32 of 32 |
| ac-x-fr | vi | 100% | 11 | 193 | 180 | 32 of 32 |
| var-fr | en | 100% | 10 | 85 | 190 | 31 of 32 |
| var-fr | en-mt | 100% | 10 | 85 | 190 | 31 of 32 |
| var-fr | fr | 100% | 12 | 96 | 190 | 31 of 32 |
| var-fr | vi | 100% | 10 | 84 | 190 | 31 of 32 |
| lie-i-iii | en | 100% | 33 | 488 | 481 | 32 of 32 |
| lie-i-iii | fr | 96% | 31 | 465 | 481 | 32 of 32 |
| lie-i-iii | vi | 100% | 32 | 514 | 481 | 32 of 32 |
| lie-iv-vi | en | 100% | 21 | 271 | 314 | 32 of 32 |
| lie-iv-vi | fr | 100% | 21 | 277 | 314 | 32 of 32 |
| lie-iv-vi | vi | 100% | 19 | 282 | 314 | 32 of 32 |
| lie-vii-ix | en | 100% | 36 | 446 | 439 | 32 of 32 |
| lie-vii-ix | fr | 55% | 19 | 226 | 439 | 30 of 32 |
| lie-vii-ix | vi | 100% | 34 | 437 | 439 | 32 of 32 |
| lie-i-fr | en | 100% | 8 | 126 | 144 | 32 of 32 |
| lie-i-fr | fr | 100% | 10 | 129 | 144 | 32 of 32 |
| lie-i-fr | vi | 100% | 8 | 122 | 144 | 32 of 32 |
| lie-ii-iii-fr | en | 95% | 22 | 352 | 318 | 32 of 32 |
| lie-ii-iii-fr | en-mt | 4% | | | 318 | refused under the floor |
| lie-ii-iii-fr | fr | 100% | 25 | 356 | 318 | 32 of 32 |
| lie-ii-iii-fr | vi | 100% | 23 | 392 | 318 | 32 of 32 |
| lie-iv-vi-fr | en | 100% | 21 | 271 | 284 | 31 of 32 |
| lie-iv-vi-fr | fr | 100% | 21 | 277 | 284 | 32 of 32 |
| lie-iv-vi-fr | vi | 100% | 19 | 282 | 284 | 31 of 32 |
| lie-vii-viii-fr | en | 100% | 8 | 74 | 61 | 32 of 32 |
| lie-vii-viii-fr | fr | 100% | 7 | 74 | 61 | 32 of 32 |
| lie-vii-viii-fr | vi | 100% | 8 | 74 | 61 | 32 of 32 |
| lie-ix-fr | en | 100% | 12 | 159 | 141 | 32 of 32 |
| lie-ix-fr | fr | 100% | 14 | 162 | 141 | 32 of 32 |
| lie-ix-fr | vi | 100% | 12 | 157 | 141 | 32 of 32 |
| ts-i-ii-fr | en | 100% | 15 | 295 | 346 | 32 of 32 |
| ts-i-ii-fr | en-mt | 100% | 15 | 295 | 346 | 32 of 32 |
| ts-i-ii-fr | fr | 100% | 17 | 311 | 346 | 32 of 32 |
| ts-i-ii-fr | vi | 100% | 15 | 249 | 346 | 31 of 32 |
| ts-iii-v-fr | en | 100% | 21 | 500 | 579 | 32 of 32 |
| ts-iii-v-fr | en-mt | 100% | 21 | 500 | 579 | 32 of 32 |
| ts-iii-v-fr | fr | 100% | 23 | 525 | 579 | 32 of 32 |
| ts-iii-v-fr | vi | 100% | 21 | 452 | 579 | 31 of 32 |
| ta-i-iv-fr | en | 100% | 28 | 433 | 512 | 32 of 32 |
| ta-i-iv-fr | en-mt | 100% | 28 | 433 | 512 | 32 of 32 |
| ta-i-iv-fr | fr | 100% | 30 | 456 | 512 | 32 of 32 |
| ta-i-iv-fr | vi | 100% | 28 | 424 | 512 | 31 of 32 |
| hist | en | 100% | 26 | 285 | 299 | 32 of 32 |
| hist | fr | 100% | 26 | 295 | 299 | 32 of 32 |
| hist | vi | 100% | 26 | 291 | 299 | 31 of 32 |
| hist-fr | en | 100% | 27 | 287 | 374 | 31 of 32 |
| hist-fr | en-mt | 3% | | | 374 | refused under the floor |
| hist-fr | fr | 100% | 27 | 297 | 374 | 32 of 32 |
| hist-fr | vi | 100% | 27 | 293 | 374 | 31 of 32 |
