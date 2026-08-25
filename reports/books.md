# Assembling the books back out of the corpus

This is what happens when every volume the manifest names is built back out of `content/` into TeX, a PDF and an EPUB, in every language that has content for it. It is milestone 13, and the point of it is not that one book builds. The point is that the corpus as a whole still assembles, because nothing that reads one file at a time can see a chapter missing from the middle of a volume or a § that goes from 1 to 3.

Every number here comes from one run of `bourbaki book` per volume per language, on the corpus at the commit this file went in on. The run is reproducible: the PDF is set by tectonic against a pinned bundle, the EPUB is written with a fixed epoch, and two builds of the same content come out as the same bytes.

## What it comes to

| | |
| --- | --- |
| volumes | 40 |
| builds | 107 |
| builds that reached a PDF | 107 |
| pages set | 23000 |
| formulae set | 1267619 |
| covers that came out the printing's yellow | 107 of 107 |
| builds in the language the volume was printed in | 37 |

The audit runs 21 checks on a build. No build passes all 21 and that is expected: eight of the checks are about the corpus rather than about the build, and they are the backlog. Ten builds pass 20, twenty eight pass 19, forty four pass 18, seventeen pass 17, six pass 16 and two pass 15.

## The checks, and how many builds each one fails

| check | builds failing |
| --- | --- |
| the volume is about the length of the printing | 85 |
| no array had to be widened to hold its own rows | 40 |
| the sections manifest knows this volume | 36 |
| no TeX control sequence is loose in the prose | 33 |
| every cross reference has something to point at | 29 |
| the chapters the manifest names are all here | 24 |
| every character reached the page | 20 |
| the §§ of every chapter run without a gap | 17 |
| every character has a glyph the build can set | 16 |
| the numbered subsections run without a gap | 4 |

The length check is the coverage measure rather than a fault in the build. A volume set at 71% of the printing's page count is a volume with a chapter still to extract, and the check exists so that the shortfall is a number somebody can watch rather than something you notice on the page.

## The four faults the sweep found in the writer

The first full run of this sweep had seventeen builds stop inside the typesetter with no PDF at all. Every one of them was the writer's doing rather than the corpus's, and none of them had shown up in the years of building single volumes, because each needs a shape the corpus has in one place.

An alignment was split through a `\left` whose `\right` was on the line below, which puts the two in different cells and stops TeX with "Extra }, or forgotten \right". A `\tag` the corpus wrote inside a display ended up inside the `aligned` the build puts around a calculation, and amsmath will not set a tag in a box. A `\footnote` in a subsection title travelled into the contents line and the running head, and a footnote read a second time is "Use of \@xfootnote doesn't match its definition". A degree sign was written as a superscript even when there was a superscript open already, which is a double superscript and stops TeX.

Fixing a fifth, an environment that sets its own display ending up inside `\[ \]`, took the last two builds. All 107 now reach a PDF.

## The thirteen volumes the sections manifest does not know

These build, and what they build is a title page, a contents page with nothing on it and a cover. Four pages against the several hundred the printing has. The content is in `content/fr/` for most of them, and what is missing is the entry in `manifests/sections.yaml` that says which files belong to which chapter of which volume.

ac-i-iv-fr, ac-x-fr, alg-i-iii-fr, alg-iv-vii-fr, alg-ix-fr, alg-x-fr, fvr-i-vii-fr, int-i-iv-fr, int-ix-fr, int-vii-viii-fr, lie-vii-viii-fr, top-i-iv-fr, top-v-x-fr.

## The three volumes with no build in their own language

fvr-i-vii-fr, top-i-iv-fr and top-v-x-fr have no `content/fr/` tree at all. There is no `content/fr/top` and no `content/fr/fvr`. The English of both books is complete, so what these three want is extraction from the French printing rather than anything to do with the build.

## Every build

The columns are the volume, the language it was built in, whether that is the language it was printed in, the pages this build set, the pages the printing has, the first as a percentage of the second, the files that went into it, the formulae in it, whether the cover came out the printing's yellow, and the audit score.

| volume | lang | printed in it | pages | printing | of it | files | formulae | cover | checks |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ac-i-iv-fr | en | no | 252 | 361 | 70% | 21 | 17731 | yes | 17 of 21 |
| ac-i-iv-fr | fr | yes | 4 | 361 | 1% | 0 | 0 | yes | 18 of 21 |
| ac-i-iv-fr | vi | no | 44 | 361 | 12% | 11 | 2279 | yes | 16 of 21 |
| ac-i-vii | en | yes | 742 | 642 | 116% | 42 | 36403 | yes | 19 of 21 |
| ac-i-vii | fr | no | 378 | 642 | 59% | 21 | 17785 | yes | 17 of 21 |
| ac-i-vii | vi | no | 150 | 642 | 23% | 24 | 6504 | yes | 17 of 21 |
| ac-v-vii-fr | en | no | 258 | 346 | 75% | 21 | 18672 | yes | 18 of 21 |
| ac-v-vii-fr | fr | yes | 257 | 346 | 74% | 21 | 17785 | yes | 18 of 21 |
| ac-v-vii-fr | vi | no | 65 | 346 | 19% | 13 | 4225 | yes | 18 of 21 |
| ac-viii-ix-fr | en | no | 4 | 0 | 0% | 0 | 0 | yes | 19 of 21 |
| ac-viii-ix-fr | fr | yes | 199 | 204 | 98% | 14 | 12309 | yes | 18 of 21 |
| ac-viii-ix-fr | vi | no | 4 | 0 | 0% | 0 | 0 | yes | 19 of 21 |
| ac-x-fr | en | no | 4 | 180 | 2% | 0 | 0 | yes | 18 of 21 |
| ac-x-fr | fr | yes | 4 | 180 | 2% | 0 | 0 | yes | 18 of 21 |
| ac-x-fr | vi | no | 4 | 180 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-i-iii | en | yes | 851 | 734 | 116% | 39 | 35144 | yes | 19 of 21 |
| alg-i-iii | fr | no | 4 | 0 | 0% | 0 | 0 | yes | 19 of 21 |
| alg-i-iii | vi | no | 706 | 734 | 96% | 39 | 27177 | yes | 18 of 21 |
| alg-i-iii-fr | en | no | 600 | 645 | 93% | 39 | 35144 | yes | 18 of 21 |
| alg-i-iii-fr | fr | yes | 4 | 645 | 1% | 0 | 0 | yes | 18 of 21 |
| alg-i-iii-fr | vi | no | 503 | 645 | 78% | 39 | 27177 | yes | 16 of 21 |
| alg-iv-vii | en | yes | 503 | 460 | 109% | 36 | 23480 | yes | 18 of 21 |
| alg-iv-vii | fr | no | 4 | 0 | 0% | 0 | 0 | yes | 19 of 21 |
| alg-iv-vii | vi | no | 398 | 460 | 87% | 36 | 17671 | yes | 17 of 21 |
| alg-iv-vii-fr | en | no | 353 | 426 | 83% | 36 | 23480 | yes | 17 of 21 |
| alg-iv-vii-fr | fr | yes | 4 | 426 | 1% | 0 | 0 | yes | 18 of 21 |
| alg-iv-vii-fr | vi | no | 284 | 426 | 67% | 36 | 17671 | yes | 15 of 21 |
| alg-ix-fr | en | no | 4 | 211 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-ix-fr | fr | yes | 4 | 211 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-ix-fr | vi | no | 4 | 211 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-viii | en | yes | 336 | 505 | 67% | 27 | 19834 | yes | 18 of 21 |
| alg-viii | fr | no | 340 | 505 | 67% | 27 | 19646 | yes | 18 of 21 |
| alg-viii | vi | no | 338 | 505 | 67% | 27 | 19824 | yes | 19 of 21 |
| alg-viii-fr | en | no | 344 | 487 | 71% | 27 | 19834 | yes | 19 of 21 |
| alg-viii-fr | fr | yes | 348 | 487 | 71% | 27 | 19646 | yes | 17 of 21 |
| alg-viii-fr | vi | no | 346 | 487 | 71% | 27 | 19824 | yes | 19 of 21 |
| alg-x-fr | en | no | 4 | 222 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-x-fr | fr | yes | 4 | 222 | 2% | 0 | 0 | yes | 18 of 21 |
| alg-x-fr | vi | no | 4 | 222 | 2% | 0 | 0 | yes | 18 of 21 |
| ens-i-iv | en | yes | 279 | 418 | 67% | 29 | 15359 | yes | 19 of 21 |
| ens-i-iv | vi | no | 286 | 418 | 68% | 29 | 15362 | yes | 19 of 21 |
| evt-i-v | en | yes | 347 | 368 | 94% | 32 | 21152 | yes | 19 of 21 |
| evt-i-v | fr | no | 360 | 368 | 98% | 33 | 20930 | yes | 18 of 21 |
| evt-i-v | vi | no | 225 | 368 | 61% | 32 | 12788 | yes | 18 of 21 |
| evt-i-v-fr | en | no | 306 | 372 | 82% | 32 | 21152 | yes | 18 of 21 |
| evt-i-v-fr | fr | yes | 323 | 372 | 87% | 33 | 20930 | yes | 19 of 21 |
| evt-i-v-fr | vi | no | 203 | 372 | 55% | 32 | 12788 | yes | 18 of 21 |
| fvr-i-vii | en | yes | 379 | 354 | 107% | 32 | 14673 | yes | 18 of 21 |
| fvr-i-vii | vi | no | 312 | 354 | 88% | 32 | 10689 | yes | 18 of 21 |
| fvr-i-vii-fr | en | no | 302 | 329 | 92% | 32 | 14673 | yes | 17 of 21 |
| fvr-i-vii-fr | vi | no | 242 | 329 | 74% | 32 | 10689 | yes | 16 of 21 |
| int-i-iv-fr | en | no | 208 | 293 | 71% | 18 | 14048 | yes | 19 of 21 |
| int-i-iv-fr | fr | yes | 4 | 293 | 1% | 0 | 0 | yes | 18 of 21 |
| int-i-iv-fr | vi | no | 144 | 293 | 49% | 16 | 8832 | yes | 17 of 21 |
| int-i-vi | en | yes | 397 | 487 | 82% | 34 | 26745 | yes | 20 of 21 |
| int-i-vi | fr | no | 187 | 487 | 38% | 16 | 12247 | yes | 18 of 21 |
| int-i-vi | vi | no | 276 | 487 | 57% | 31 | 17015 | yes | 17 of 21 |
| int-ix-fr | en | no | 109 | 131 | 83% | 9 | 7009 | yes | 17 of 21 |
| int-ix-fr | fr | yes | 4 | 131 | 3% | 0 | 0 | yes | 18 of 21 |
| int-ix-fr | vi | no | 85 | 131 | 65% | 8 | 4703 | yes | 16 of 21 |
| int-v-fr | en | no | 119 | 159 | 75% | 10 | 7690 | yes | 20 of 21 |
| int-v-fr | fr | yes | 119 | 159 | 75% | 10 | 7628 | yes | 20 of 21 |
| int-v-fr | vi | no | 77 | 159 | 48% | 9 | 4530 | yes | 20 of 21 |
| int-vi-fr | en | no | 75 | 106 | 71% | 6 | 5007 | yes | 19 of 21 |
| int-vi-fr | fr | yes | 69 | 106 | 65% | 6 | 4619 | yes | 18 of 21 |
| int-vi-fr | vi | no | 60 | 106 | 57% | 6 | 3653 | yes | 19 of 21 |
| int-vii-ix | en | yes | 269 | 332 | 81% | 22 | 16772 | yes | 18 of 21 |
| int-vii-ix | fr | no | 4 | 0 | 0% | 0 | 0 | yes | 19 of 21 |
| int-vii-ix | vi | no | 189 | 332 | 57% | 19 | 10130 | yes | 15 of 21 |
| int-vii-viii-fr | en | no | 149 | 224 | 67% | 13 | 9763 | yes | 19 of 21 |
| int-vii-viii-fr | fr | yes | 4 | 224 | 2% | 0 | 0 | yes | 18 of 21 |
| int-vii-viii-fr | vi | no | 96 | 224 | 43% | 11 | 5427 | yes | 16 of 21 |
| lie-i-fr | en | no | 99 | 144 | 69% | 8 | 7068 | yes | 18 of 21 |
| lie-i-fr | fr | yes | 101 | 144 | 70% | 8 | 6293 | yes | 18 of 21 |
| lie-i-fr | vi | no | 30 | 144 | 21% | 5 | 1701 | yes | 18 of 21 |
| lie-i-iii | en | yes | 962 | 481 | 200% | 30 | 23984 | yes | 17 of 21 |
| lie-i-iii | fr | no | 969 | 481 | 201% | 31 | 22424 | yes | 17 of 21 |
| lie-i-iii | vi | no | 174 | 481 | 36% | 14 | 3778 | yes | 18 of 21 |
| lie-ii-iii-fr | en | no | 297 | 318 | 93% | 22 | 16916 | yes | 17 of 21 |
| lie-ii-iii-fr | fr | yes | 291 | 318 | 92% | 23 | 16131 | yes | 18 of 21 |
| lie-ii-iii-fr | vi | no | 49 | 318 | 15% | 9 | 2077 | yes | 19 of 21 |
| lie-iv-vi | en | yes | 240 | 314 | 76% | 18 | 14408 | yes | 17 of 21 |
| lie-iv-vi | fr | no | 223 | 314 | 71% | 18 | 14508 | yes | 19 of 21 |
| lie-iv-vi | vi | no | 47 | 314 | 15% | 10 | 2652 | yes | 19 of 21 |
| lie-iv-vi-fr | en | no | 215 | 284 | 76% | 18 | 14408 | yes | 17 of 21 |
| lie-iv-vi-fr | fr | yes | 202 | 284 | 71% | 18 | 14508 | yes | 19 of 21 |
| lie-iv-vi-fr | vi | no | 44 | 284 | 15% | 10 | 2652 | yes | 20 of 21 |
| lie-ix-fr | en | no | 113 | 141 | 80% | 12 | 8724 | yes | 20 of 21 |
| lie-ix-fr | fr | yes | 115 | 141 | 82% | 12 | 8484 | yes | 20 of 21 |
| lie-ix-fr | vi | no | 30 | 141 | 21% | 6 | 1681 | yes | 20 of 21 |
| lie-vii-ix | en | yes | 357 | 439 | 81% | 34 | 27942 | yes | 20 of 21 |
| lie-vii-ix | fr | no | 128 | 439 | 29% | 12 | 8484 | yes | 18 of 21 |
| lie-vii-ix | vi | no | 107 | 439 | 24% | 19 | 7201 | yes | 19 of 21 |
| lie-vii-viii-fr | en | no | 234 | 61 | 384% | 22 | 19218 | yes | 19 of 21 |
| lie-vii-viii-fr | fr | yes | 4 | 61 | 7% | 0 | 0 | yes | 18 of 21 |
| lie-vii-viii-fr | vi | no | 76 | 61 | 125% | 13 | 5520 | yes | 18 of 21 |
| ta-i-iv-fr | fr | yes | 340 | 512 | 66% | 26 | 24278 | yes | 19 of 21 |
| top-i-iv | en | yes | 326 | 443 | 74% | 38 | 22499 | yes | 19 of 21 |
| top-i-iv | vi | no | 248 | 443 | 56% | 38 | 15430 | yes | 18 of 21 |
| top-i-iv-fr | en | no | 326 | 367 | 89% | 38 | 22499 | yes | 19 of 21 |
| top-i-iv-fr | vi | no | 248 | 367 | 68% | 38 | 15430 | yes | 17 of 21 |
| top-v-x | en | yes | 297 | 372 | 80% | 37 | 18797 | yes | 18 of 21 |
| top-v-x | vi | no | 187 | 372 | 50% | 35 | 10285 | yes | 17 of 21 |
| top-v-x-fr | en | no | 249 | 329 | 76% | 37 | 18797 | yes | 18 of 21 |
| top-v-x-fr | vi | no | 157 | 329 | 48% | 35 | 10285 | yes | 16 of 21 |
| ts-i-ii-fr | fr | yes | 240 | 346 | 69% | 13 | 15570 | yes | 20 of 21 |
| ts-iii-v-fr | fr | yes | 408 | 579 | 70% | 19 | 26739 | yes | 19 of 21 |
