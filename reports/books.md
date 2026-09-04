# Assembling the books back out of the corpus

Every volume the manifest names, built back out of `content/` into TeX, a PDF and an EPUB, in every language that has enough of it. It is milestone 13, and the point is not that one book builds: it is that the corpus as a whole still assembles, because nothing that reads one file at a time can see a chapter missing from the middle of a volume or a § that goes from 1 to 3.

Written by `bourbaki book check -write`. Every number here is one run of the same build `bourbaki book` makes, so a row of this table and a run of that command on that volume are the same numbers.

## What it comes to

| | |
| --- | --- |
| volumes | 44 |
| builds | 140 |
| builds that reached a PDF | 140 |
| pages set | 48330 |
| formulae set | 2355812 |
| languages refused under the 10% floor | 3 |
| builds that could not be assembled | 0 |

## The checks, and how many builds each one fails

| check | builds failing |
| --- | --- |
| the volume holds the text the printing has | 25 |
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
| ens-i-iv | en | 100% | 32 | 374 | 418 | 32 of 33 |
| ens-i-iv | fr | 100% | 32 | 362 | 418 | 32 of 33 |
| ens-i-iv | vi | 100% | 32 | 376 | 418 | 32 of 33 |
| ens-i-iv-fr | en | 100% | 32 | 374 | 349 | 32 of 33 |
| ens-i-iv-fr | fr | 100% | 32 | 362 | 349 | 32 of 33 |
| ens-i-iv-fr | vi | 100% | 32 | 376 | 349 | 32 of 33 |
| alg-i-iii | en | 100% | 43 | 755 | 734 | 33 of 33 |
| alg-i-iii | fr | 100% | 43 | 756 | 734 | 33 of 33 |
| alg-i-iii | vi | 100% | 43 | 822 | 734 | 33 of 33 |
| alg-iv-vii | en | 100% | 39 | 494 | 460 | 33 of 33 |
| alg-iv-vii | fr | 94% | 37 | 506 | 460 | 33 of 33 |
| alg-iv-vii | vi | 100% | 38 | 506 | 460 | 33 of 33 |
| alg-viii | en | 100% | 31 | 449 | 505 | 33 of 33 |
| alg-viii | fr | 100% | 31 | 455 | 505 | 33 of 33 |
| alg-viii | vi | 100% | 29 | 427 | 505 | 33 of 33 |
| alg-i-iii-fr | en | 100% | 43 | 757 | 645 | 33 of 33 |
| alg-i-iii-fr | fr | 100% | 43 | 758 | 645 | 33 of 33 |
| alg-i-iii-fr | vi | 100% | 43 | 822 | 645 | 33 of 33 |
| alg-iv-vii-fr | en | 100% | 39 | 494 | 426 | 33 of 33 |
| alg-iv-vii-fr | fr | 100% | 37 | 506 | 426 | 33 of 33 |
| alg-iv-vii-fr | vi | 100% | 38 | 506 | 426 | 33 of 33 |
| alg-viii-fr | en | 100% | 31 | 449 | 487 | 33 of 33 |
| alg-viii-fr | fr | 100% | 31 | 455 | 487 | 33 of 33 |
| alg-viii-fr | vi | 100% | 29 | 427 | 487 | 32 of 33 |
| alg-ix-fr | en | 100% | 12 | 192 | 211 | 33 of 33 |
| alg-ix-fr | en-mt | 100% | 12 | 192 | 211 | 33 of 33 |
| alg-ix-fr | fr | 100% | 14 | 200 | 211 | 33 of 33 |
| alg-ix-fr | vi | 100% | 12 | 193 | 211 | 33 of 33 |
| alg-x-fr | en | 90% | 10 | 263 | 222 | 33 of 33 |
| alg-x-fr | en-mt | 90% | 10 | 263 | 222 | 33 of 33 |
| alg-x-fr | fr | 100% | 13 | 270 | 222 | 33 of 33 |
| alg-x-fr | vi | 90% | 10 | 216 | 222 | 32 of 33 |
| top-i-iv | en | 100% | 42 | 427 | 443 | 33 of 33 |
| top-i-iv | fr | 100% | 42 | 434 | 443 | 33 of 33 |
| top-i-iv | vi | 100% | 42 | 445 | 443 | 33 of 33 |
| top-v-x | en | 100% | 40 | 353 | 372 | 33 of 33 |
| top-v-x | fr | 97% | 41 | 385 | 372 | 33 of 33 |
| top-v-x | vi | 100% | 42 | 413 | 372 | 33 of 33 |
| top-i-iv-fr | en | 100% | 42 | 429 | 367 | 33 of 33 |
| top-i-iv-fr | fr | 100% | 42 | 434 | 367 | 33 of 33 |
| top-i-iv-fr | vi | 100% | 42 | 445 | 367 | 32 of 33 |
| top-v-x-fr | en | 94% | 40 | 355 | 329 | 32 of 33 |
| top-v-x-fr | en-mt | 5% | | | 329 | refused under the floor |
| top-v-x-fr | fr | 100% | 41 | 385 | 329 | 33 of 33 |
| top-v-x-fr | vi | 100% | 42 | 413 | 329 | 33 of 33 |
| fvr-i-vii | en | 100% | 36 | 366 | 354 | 33 of 33 |
| fvr-i-vii | fr | 100% | 36 | 372 | 354 | 33 of 33 |
| fvr-i-vii | vi | 100% | 36 | 378 | 354 | 33 of 33 |
| fvr-i-vii-fr | en | 100% | 36 | 368 | 329 | 33 of 33 |
| fvr-i-vii-fr | fr | 100% | 36 | 372 | 329 | 33 of 33 |
| fvr-i-vii-fr | vi | 100% | 36 | 378 | 329 | 33 of 33 |
| evt-i-v | en | 100% | 36 | 441 | 368 | 33 of 33 |
| evt-i-v | fr | 100% | 36 | 457 | 368 | 33 of 33 |
| evt-i-v | vi | 100% | 36 | 471 | 368 | 33 of 33 |
| evt-i-v-fr | en | 100% | 36 | 441 | 372 | 33 of 33 |
| evt-i-v-fr | fr | 100% | 36 | 457 | 372 | 33 of 33 |
| evt-i-v-fr | vi | 100% | 36 | 471 | 372 | 33 of 33 |
| int-i-vi | en | 100% | 38 | 500 | 487 | 33 of 33 |
| int-i-vi | fr | 97% | 35 | 492 | 487 | 33 of 33 |
| int-i-vi | vi | 100% | 37 | 510 | 487 | 33 of 33 |
| int-vii-ix | en | 100% | 25 | 329 | 332 | 33 of 33 |
| int-vii-ix | fr | 95% | 22 | 321 | 332 | 33 of 33 |
| int-vii-ix | vi | 100% | 25 | 341 | 332 | 33 of 33 |
| int-i-iv-fr | en | 100% | 19 | 262 | 293 | 33 of 33 |
| int-i-iv-fr | fr | 100% | 21 | 275 | 293 | 33 of 33 |
| int-i-iv-fr | vi | 100% | 19 | 261 | 293 | 32 of 33 |
| int-v-fr | en | 100% | 10 | 144 | 159 | 33 of 33 |
| int-v-fr | fr | 100% | 11 | 151 | 159 | 33 of 33 |
| int-v-fr | vi | 100% | 10 | 140 | 159 | 32 of 33 |
| int-vi-fr | en | 100% | 6 | 84 | 106 | 33 of 33 |
| int-vi-fr | fr | 100% | 8 | 90 | 106 | 33 of 33 |
| int-vi-fr | vi | 100% | 6 | 101 | 106 | 33 of 33 |
| int-vii-viii-fr | en | 100% | 13 | 181 | 224 | 33 of 33 |
| int-vii-viii-fr | fr | 100% | 15 | 190 | 224 | 33 of 33 |
| int-vii-viii-fr | vi | 100% | 13 | 185 | 224 | 33 of 33 |
| int-ix-fr | en | 100% | 9 | 138 | 131 | 33 of 33 |
| int-ix-fr | fr | 100% | 11 | 146 | 131 | 33 of 33 |
| int-ix-fr | vi | 100% | 9 | 146 | 131 | 33 of 33 |
| ac-i-vii | en | 100% | 46 | 647 | 642 | 33 of 33 |
| ac-i-vii | fr | 97% | 43 | 628 | 642 | 33 of 33 |
| ac-i-vii | vi | 100% | 46 | 691 | 642 | 33 of 33 |
| ac-i-iv-fr | en | 100% | 22 | 317 | 361 | 33 of 33 |
| ac-i-iv-fr | fr | 100% | 24 | 325 | 361 | 33 of 33 |
| ac-i-iv-fr | vi | 100% | 22 | 340 | 361 | 33 of 33 |
| ac-v-vii-fr | en | 100% | 21 | 320 | 346 | 33 of 33 |
| ac-v-vii-fr | fr | 100% | 23 | 325 | 346 | 33 of 33 |
| ac-v-vii-fr | vi | 100% | 21 | 339 | 346 | 33 of 33 |
| ac-viii-ix-fr | en | 100% | 14 | 239 | 204 | 33 of 33 |
| ac-viii-ix-fr | en-mt | 100% | 14 | 239 | 204 | 33 of 33 |
| ac-viii-ix-fr | fr | 100% | 16 | 243 | 204 | 33 of 33 |
| ac-viii-ix-fr | vi | 100% | 14 | 236 | 204 | 33 of 33 |
| ac-x-fr | en | 100% | 11 | 201 | 180 | 33 of 33 |
| ac-x-fr | en-mt | 100% | 11 | 201 | 180 | 33 of 33 |
| ac-x-fr | fr | 100% | 11 | 202 | 180 | 33 of 33 |
| ac-x-fr | vi | 100% | 11 | 193 | 180 | 33 of 33 |
| var-fr | en | 100% | 10 | 85 | 190 | 32 of 33 |
| var-fr | en-mt | 100% | 10 | 85 | 190 | 32 of 33 |
| var-fr | fr | 100% | 12 | 96 | 190 | 32 of 33 |
| var-fr | vi | 100% | 10 | 84 | 190 | 32 of 33 |
| lie-i-iii | en | 100% | 33 | 488 | 481 | 33 of 33 |
| lie-i-iii | fr | 96% | 31 | 465 | 481 | 33 of 33 |
| lie-i-iii | vi | 100% | 34 | 526 | 481 | 33 of 33 |
| lie-iv-vi | en | 100% | 21 | 271 | 314 | 33 of 33 |
| lie-iv-vi | fr | 100% | 21 | 277 | 314 | 33 of 33 |
| lie-iv-vi | vi | 100% | 21 | 287 | 314 | 33 of 33 |
| lie-vii-ix | en | 100% | 36 | 446 | 439 | 33 of 33 |
| lie-vii-ix | fr | 55% | 19 | 226 | 439 | 31 of 33 |
| lie-vii-ix | vi | 100% | 35 | 441 | 439 | 33 of 33 |
| lie-i-fr | en | 100% | 8 | 126 | 144 | 33 of 33 |
| lie-i-fr | fr | 100% | 10 | 129 | 144 | 33 of 33 |
| lie-i-fr | vi | 100% | 8 | 122 | 144 | 33 of 33 |
| lie-ii-iii-fr | en | 95% | 22 | 352 | 318 | 33 of 33 |
| lie-ii-iii-fr | en-mt | 4% | | | 318 | refused under the floor |
| lie-ii-iii-fr | fr | 100% | 25 | 356 | 318 | 33 of 33 |
| lie-ii-iii-fr | vi | 100% | 23 | 392 | 318 | 33 of 33 |
| lie-iv-vi-fr | en | 100% | 21 | 271 | 284 | 32 of 33 |
| lie-iv-vi-fr | fr | 100% | 21 | 277 | 284 | 33 of 33 |
| lie-iv-vi-fr | vi | 100% | 21 | 287 | 284 | 32 of 33 |
| lie-vii-viii-fr | en | 100% | 8 | 74 | 61 | 33 of 33 |
| lie-vii-viii-fr | fr | 100% | 7 | 74 | 61 | 33 of 33 |
| lie-vii-viii-fr | vi | 100% | 8 | 74 | 61 | 33 of 33 |
| lie-ix-fr | en | 100% | 12 | 159 | 141 | 33 of 33 |
| lie-ix-fr | fr | 100% | 14 | 162 | 141 | 33 of 33 |
| lie-ix-fr | vi | 100% | 12 | 157 | 141 | 33 of 33 |
| ts-i-ii-fr | en | 100% | 15 | 295 | 346 | 33 of 33 |
| ts-i-ii-fr | en-mt | 100% | 15 | 295 | 346 | 33 of 33 |
| ts-i-ii-fr | fr | 100% | 17 | 311 | 346 | 33 of 33 |
| ts-i-ii-fr | vi | 100% | 15 | 249 | 346 | 32 of 33 |
| ts-iii-v-fr | en | 100% | 21 | 500 | 579 | 33 of 33 |
| ts-iii-v-fr | en-mt | 100% | 21 | 500 | 579 | 33 of 33 |
| ts-iii-v-fr | fr | 100% | 23 | 525 | 579 | 33 of 33 |
| ts-iii-v-fr | vi | 100% | 21 | 452 | 579 | 32 of 33 |
| ta-i-iv-fr | en | 100% | 28 | 433 | 512 | 33 of 33 |
| ta-i-iv-fr | en-mt | 100% | 28 | 433 | 512 | 33 of 33 |
| ta-i-iv-fr | fr | 100% | 30 | 456 | 512 | 33 of 33 |
| ta-i-iv-fr | vi | 100% | 28 | 424 | 512 | 32 of 33 |
| hist | en | 100% | 26 | 285 | 299 | 33 of 33 |
| hist | fr | 100% | 26 | 295 | 299 | 33 of 33 |
| hist | vi | 100% | 26 | 291 | 299 | 32 of 33 |
| hist-fr | en | 100% | 27 | 287 | 374 | 32 of 33 |
| hist-fr | en-mt | 3% | | | 374 | refused under the floor |
| hist-fr | fr | 100% | 27 | 297 | 374 | 33 of 33 |
| hist-fr | vi | 100% | 27 | 293 | 374 | 32 of 33 |
