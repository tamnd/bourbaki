# bourbaki

Bourbaki's *Éléments de mathématique* as Markdown, with permanent tags, translations, and worked exercises.

The source PDFs go in, Markdown comes out. Every numbered statement gets a four-character tag that never changes, so you can cite a result and have the citation still work after the text is re-extracted, re-split, or renumbered. That idea is lifted straight from the [Stacks Project](https://stacks.math.columbia.edu/).

This repo is the corpus only. The code that builds it lives in [tamnd/bourbaki-solver](https://github.com/tamnd/bourbaki-solver).

## What is in scope

<!-- BEGIN LIBRARY -->
All twelve Books of the *Éléments*, in the English translation where one was printed and in the French original everywhere else. 44 volumes, 15338 pages, of which 15 volumes and 6648 pages are English and 29 volumes and 8690 pages are French.

| Book | English | French | Volumes | Pages |
| --- | --- | --- | --- | --- |
| Theory of Sets | I to IV | I to IV | 2 | 767 |
| Algebra | I to VIII | I to X | 8 | 3690 |
| General Topology | I to X | I to X | 4 | 1511 |
| Functions of a Real Variable | I to VII | I to VII | 2 | 683 |
| Topological Vector Spaces | I to V | I to V | 2 | 740 |
| Integration | I to IX | I to IX | 7 | 1732 |
| Commutative Algebra | I to VII | I to X | 5 | 1733 |
| Variétés différentielles et analytiques | none held | 1 | 1 | 190 |
| Lie Groups and Lie Algebras | I to IX | I to VII, IX | 8 | 2182 |
| Théories spectrales | none held | I to V | 2 | 925 |
| Topologie algébrique | none held | I to IV | 1 | 512 |
| Elements of the History of Mathematics | 1 | 1 | 2 | 673 |
<!-- END LIBRARY -->

The French is not a fallback for the English. Three Books were never translated, Algèbre chapters IX and X and Algèbre commutative chapters VIII, IX and X exist in French only, and where both printings are held the French is the original a disputed English sentence gets checked against. So both are in scope and both carry the same tags.

None held in a column means one of two things, and the table cannot tell them apart. Théories spectrales, Topologie algébrique and Variétés différentielles et analytiques have no English printing because none was ever made. Théorie des ensembles has a French printing, the original one, and this corpus holds only the English translation of it.

One more gap worth stating plainly. *Groupes et algèbres de Lie, Chapitres 7 et 8* is a partial file: 61 pages that open at Chapitre VII and stop in the middle of the exercises around printed page 65, so the English *Chapters 7-9* is the only complete copy of that material.

`bourbaki books list` prints the volume by volume detail, and `manifests/books.yaml` carries it as data, with the SHA-256 and page count of every file so that a swapped or re-downloaded PDF is caught rather than silently extracted.

The PDFs are not here and will not be. They are copyright Springer and N. Bourbaki. This corpus is for personal study.

## Three extraction paths, not one

What a volume costs to read depends entirely on what its own text layer is worth, and the library splits three ways. `bourbaki books add` measures this rather than guessing it, by sampling the images and the text of a band of body pages, and records the answer as `text_layer` in the manifest.

<!-- BEGIN TEXTLAYER -->
| Text layer | Volumes | What it means |
| --- | --- | --- |
| native | 6 | Born digital. `pdftotext -layout` gives real text and real mathematics. |
| ocr | 34 | A scan somebody has already run OCR over. Good enough to read a running head off, useless for mathematics. |
| none | 4 | A scan with no text at all. Even the page map has to come out of vision OCR. |

The six native volumes are *Algebra, Chapter 8* and *Lie Groups and Lie Algebras, Chapters 7-9* in English, and *Algèbre, Chapitre 8*, *Théories spectrales, Chapitres 1 et 2*, *Théories spectrales, Chapitres 3 à 5* and *Topologie algébrique, Chapitres 1 à 4* in French. They are cheap and they go first. The four with no text at all are *Théorie des ensembles* at 349 pages, *Algèbre, Chapitre 10* at 222 pages, *General Topology, Chapters 5-10* at 372 pages and *Commutative Algebra, Chapters 1-7* at 642 pages, and they are the most expensive volumes in the library. The other 34 are the ordinary case.
<!-- END TEXTLAYER -->

Their OCR layer renders a pair of braces in *Theory of Sets* as `R! x, y I`, so nothing in it can be trusted as mathematics, but it is legible enough to build the page map from before a single page goes to vision OCR, which saves the expensive pass on every one of them.

## Running heads differ per volume

Worth knowing before you touch the page-map code, because each volume prints its locators differently:

```
1998, Ch. I     I                    ALGEBRAIC STRUCTURES
                                     p-GROUPS                         §6.5
2003, Ch. IV    A. IV. 2             POLYNOMIALS AND RATIONAL FRACTIONS   §1
                No. 2                POLYNOMIALS                      A.IV.3
2023, Ch. VIII  No 4                 POLYNOMIALS WITH ...              A VIII.13
```

Bourbaki cross-references are page based, as in `VIII, p. 3, Proposition 3`, so the page map is not decoration. It is the key the reference resolver joins on. The 1998 volume does not print a page locator in its running head at all, which is why its page map is anchored and interpolated rather than read off directly.

## Tags

```markdown
#### Proposition 6 {#alg-viii-s1-prop-6 .statement tag=0A3F}
```

`tags/tags` is append only, one line per statement:

```
0A3F,alg-viii-s1-prop-6
```

A tag is never reused and never edited. If a label has to change, the tag follows the statement and the old label goes to `tags/aliases`. Every edition uses the same tag for the same statement, the French original included, so a tag is the one identifier that works across all of them and is what lets a translation be checked against the French rather than only against the English it was made from.

`tags/runs` says where one assignment stopped and the next began, one line per merge. Tags are handed out in reading order, so the tags of a file climb on the run that assigned them, and they do not climb across runs: a statement added to the middle of a § a month later takes a tag above everything under it. The boundaries are what let the audit tell that correct edit from a heading somebody pasted the wrong tag on to.

## Layout

```
content/en/<book>/<CH>/NN_sN_<slug>.md         one file per §
content/en/<book>/<CH>/exercises/sN/NN.md      one file per exercise
content/fr/...                                 same tree, extracted from the French printing
content/{vi,zh,ja}/...                         same tree, translated
content/solutions/<lang>/<book>/<CH>/sN/NN.md  verified solutions
tags/                                          permanent tag index
manifests/                                     books, TOC, page maps, refs, glossary, errata, editions
figures/                                       cropped diagrams, small, committed
reports/                                       audit, usage, coverage, scorecards
imports/<book>/chapter_<n>/<n>.<m>.md          read off share links, not yet checked
```

`content/fr` is not a translation and is never generated from `content/en`. It is what the French volume prints, extracted the same way the English is, which is why it carries no `translated_from` and is exempt from the translation rules.

Because the two printings sit side by side, the places they disagree get noticed, and there are two manifests for what is found. `manifests/errata.yaml` is for a printing that is wrong, and it carries the words the page has and the words to read instead. `manifests/editions.yaml` is for the other case, where the printings differ and both are right: chapter VIII § 2 has twenty exercises in the 2023 English and nineteen in the 2012 French, the nineteen are the same nineteen, and the twentieth is one the later printing added. A difference like that looks exactly like a page nobody read, so the reading that settles it is written down once instead of being done again by whoever counts next.

`pdf/`, `images/` and `work/` are gitignored. Nothing large or copyrighted is committed.

`imports/` is deliberately outside `content/`. It holds sections read off public ChatGPT share links, which cost an HTTP GET rather than 150 seconds of a browser per page, and which nobody has yet held against the printed book. The audit runs over `content/`, so anything dropped in there would pass every rule in it by default. See [imports/README.md](imports/README.md).

## Coverage

<!-- BEGIN COVERAGE -->
| Book | Chapter | Sections | Statements | Exercises | Tagged | Pages |
| --- | --- | --- | --- | --- | --- | --- |
| Commutative Algebra | I | 4 of 4 | 65 | 42 | 0 | 106 |
| Commutative Algebra | II | 5 of 5 | 183 | 105 | 0 | 218 |
| Commutative Algebra | III | 5 of 5 | 143 | 59 | 0 | 230 |
| Commutative Algebra | IV | 3 of 3 | 69 | 57 | 0 | 98 |
| Commutative Algebra | V | 3 of 3 | 122 | 61 | 0 | 150 |
| Commutative Algebra | VI | 10 of 10 | 151 | 77 | 0 | 211 |
| Commutative Algebra | VII | 4 of 4 | 130 | 85 | 0 | 302 |
| Commutative Algebra | VIII | 0 of 7 | 0 | 0 | 0 | 108 |
| Commutative Algebra | IX | 0 of 5 | 0 | 0 | 0 | 85 |
| Commutative Algebra | X | 0 of 10 | 0 | 0 | 0 | 179 |
| Algebra | I | 10 of 10 | 293 | 218 | 0 | 357 |
| Algebra | II | 12 of 12 | 384 | 150 | 0 | 446 |
| Algebra | III | 12 of 12 | 273 | 97 | 0 | 542 |
| Algebra | IV | 6 of 6 | 163 | 53 | 0 | 202 |
| Algebra | V | 17 of 17 | 427 | 156 | 0 | 382 |
| Algebra | VI | 2 of 2 | 86 | 77 | 0 | 92 |
| Algebra | VII | 5 of 5 | 149 | 80 | 0 | 162 |
| Algebra | VIII | 25 of 25 | 709 | 317 | 1024 | 964 |
| Algebra | IX | 0 of 10 | 0 | 0 | 0 | 207 |
| Algebra | X | 0 of 9 | 0 | 0 | 0 | 216 |
| Theory of Sets | I | 6 of 6 | 16 | 35 | 51 | 101 |
| Theory of Sets | II | 6 of 6 | 110 | 41 | 150 | 117 |
| Theory of Sets | III | 7 of 7 | 222 | 120 | 342 | 226 |
| Theory of Sets | IV | 3 of 3 | 29 | 15 | 43 | 255 |
| Topological Vector Spaces | I | 3 of 3 | 64 | 38 | 0 | 58 |
| Topological Vector Spaces | II | 8 of 8 | 205 | 162 | 0 | 195 |
| Topological Vector Spaces | III | 6 of 6 | 123 | 78 | 0 | 101 |
| Topological Vector Spaces | IV | 6 of 6 | 114 | 118 | 0 | 152 |
| Topological Vector Spaces | V | 4 of 4 | 133 | 68 | 0 | 181 |
| Functions of a Real Variable | I | 4 of 4 | 88 | 66 | 0 | 100 |
| Functions of a Real Variable | II | 3 of 3 | 55 | 29 | 0 | 78 |
| Functions of a Real Variable | III | 2 of 2 | 10 | 48 | 0 | 141 |
| Functions of a Real Variable | IV | 2 of 2 | 54 | 28 | 0 | 94 |
| Functions of a Real Variable | V | 5 of 5 | 108 | 28 | 0 | 113 |
| Functions of a Real Variable | VI | 3 of 3 | 26 | 12 | 0 | 67 |
| Functions of a Real Variable | VII | 2 of 2 | 14 | 12 | 0 | 73 |
| Elements of the History of Mathematics | 1 | 26 of 26 | 0 | 0 | 0 | 665 |
| Integration | I | 0 of 1 | 0 | 0 | 0 | 17 |
| Integration | II | 2 of 2 | 29 | 21 | 0 | 44 |
| Integration | III | 4 of 4 | 106 | 35 | 0 | 128 |
| Integration | IV | 7 of 7 | 288 | 94 | 0 | 332 |
| Integration | V | 8 of 8 | 206 | 108 | 0 | 290 |
| Integration | VI | 4 of 4 | 98 | 57 | 0 | 173 |
| Integration | VII | 5 of 5 | 120 | 48 | 0 | 207 |
| Integration | VIII | 5 of 5 | 109 | 59 | 0 | 188 |
| Integration | IX | 7 of 7 | 188 | 56 | 0 | 259 |
| Lie Groups and Lie Algebras | I | 7 of 7 | 167 | 125 | 0 | 250 |
| Lie Groups and Lie Algebras | II | 9 of 9 | 121 | 72 | 0 | 186 |
| Lie Groups and Lie Algebras | III | 11 of 11 | 393 | 113 | 0 | 481 |
| Lie Groups and Lie Algebras | IV | 3 of 3 | 66 | 43 | 0 | 108 |
| Lie Groups and Lie Algebras | V | 7 of 7 | 139 | 44 | 0 | 179 |
| Lie Groups and Lie Algebras | VI | 4 of 4 | 130 | 47 | 0 | 291 |
| Lie Groups and Lie Algebras | VII | 7 of 7 | 139 | 66 | 205 | 127 |
| Lie Groups and Lie Algebras | VIII | 13 of 13 | 299 | 172 | 471 | 211 |
| Lie Groups and Lie Algebras | IX | 11 of 11 | 244 | 112 | 356 | 284 |
| Topologie algébrique | I | 0 of 6 | 0 | 0 | 0 | 150 |
| Topologie algébrique | II | 0 of 5 | 0 | 0 | 0 | 78 |
| Topologie algébrique | III | 0 of 5 | 0 | 0 | 0 | 110 |
| Topologie algébrique | IV | 0 of 6 | 0 | 0 | 0 | 158 |
| General Topology | I | 11 of 11 | 317 | 153 | 0 | 279 |
| General Topology | II | 4 of 4 | 113 | 41 | 0 | 94 |
| General Topology | III | 7 of 7 | 165 | 114 | 0 | 198 |
| General Topology | IV | 8 of 8 | 106 | 102 | 0 | 204 |
| General Topology | V | 4 of 4 | 24 | 8 | 0 | 21 |
| General Topology | VI | 3 of 3 | 37 | 36 | 0 | 30 |
| General Topology | VII | 3 of 3 | 38 | 24 | 0 | 28 |
| General Topology | VIII | 4 of 4 | 26 | 22 | 0 | 34 |
| General Topology | IX | 7 of 8 | 197 | 109 | 0 | 129 |
| General Topology | X | 4 of 4 | 106 | 63 | 0 | 80 |
| Théories spectrales | I | 0 of 8 | 0 | 0 | 0 | 197 |
| Théories spectrales | II | 0 of 3 | 0 | 0 | 0 | 136 |
| Théories spectrales | III | 0 of 6 | 0 | 0 | 0 | 143 |
| Théories spectrales | IV | 0 of 5 | 0 | 0 | 0 | 228 |
| Théories spectrales | V | 0 of 4 | 0 | 0 | 0 | 194 |
| Variétés différentielles et analytiques | 1 | 0 of 8 | 0 | 0 | 0 | 95 |

388 of 487 sections are in the corpus, 80 per cent. 8689 statements and 4476 exercises, 2642 of them carrying a permanent tag.
<!-- END COVERAGE -->

## What is translated

The table above is what has been read out of the printed books. This one is what has been carried into another language, which is the other half of the work and is where most of the machine time goes.

A section or an exercise is counted as translated when a file for it exists in that language, nothing more. It is not a claim about quality. The translation rules in the audit are what says whether a file that exists is any good, and `reports/audit.md` is where their findings are. Plenty of what is counted here was written by a cut down model in a hurry and is queued to be read again by a better one.

The source is the English, and the English is two directories. `content/en` is the Springer translation where one was printed. `content/en-mt` is this project's reading of the French, for the chapters no English was ever printed for, which is most of Algebra IX and X, Commutative Algebra VIII to X and Integration V to IX. They are kept apart so a reader can tell which is which, but a Vietnamese file is made from whichever of the two exists, so for this table they are one source.

The French is counted and not compared against the English. A file name carries a slug of its own title, so `02_s2_relevement_des_ideaux_premiers.md` and `02_s2_the_lift_of_prime_ideals.md` are one section under two names. Matching the two trees by path once reported 289 French sections with no English when the real answer was 41.

<!-- BEGIN TRANSLATION -->
| Book | Sections | Exercises | Vietnamese sections | Vietnamese exercises | Done | From machine English |
| --- | --- | --- | --- | --- | --- | --- |
| Theory of Sets | 32 | 214 | 30 | 211 | 98% | 3 |
| Algebra | 135 | 1302 | 130 | 1252 | 96% | 176 |
| General Topology | 84 | 788 | 82 | 739 | 94% | 118 |
| Functions of a Real Variable | 36 | 251 | 36 | 245 | 98% | 28 |
| Topological Vector Spaces | 36 | 479 | 35 | 472 | 98% | 15 |
| Integration | 63 | 511 | 61 | 504 | 98% | 33 |
| Commutative Algebra | 71 | 902 | 70 | 876 | 97% | 441 |
| Variétés différentielles et analytiques | 10 | 0 | 10 | 0 | 100% | 10, all of it |
| Lie Groups and Lie Algebras | 91 | 798 | 88 | 797 | 100% | 5 |
| Théories spectrales | 36 | 590 | 36 | 374 | 65% | 626, all of it |
| Topologie algébrique | 28 | 203 | 28 | 196 | 97% | 231, all of it |
| Elements of the History of Mathematics | 27 | 0 | 27 | 0 | 100% | 1 |
| **All** | **649** | **6038** | **633** | **5666** | **94%** | **1687** |

The source column is the English, which is 649 sections and 6038 exercises: 5000 files in `content/en` where Springer printed an English translation and 1962 in `content/en-mt` where this project read the French instead. The French originals are 651 sections and 5630 exercises in `content/fr`, and they are counted here rather than compared, because a file name carries a slug of its own title and matching the two trees by path calls every honestly translated title a missing section.

Vietnamese has 633 of the 649 sections and 5666 of the 6038 exercises. Sections here means every file that is not an exercise, so the introductions, the notes to the reader and the historical notes are counted with the §§.

The last column is the part of a Book that was never printed in English, so the only English of it is this project's own reading of the French. A translation made from one of those is a translation of a translation, and that is 1333 of the 6299 files in Vietnamese. Where the column says all of it the whole Book is in that position, and a hundred per cent in the Done column for such a Book is not the same claim as a hundred per cent for one Springer translated.
<!-- END TRANSLATION -->

## Building it

Registering a volume probes it and writes what it measured, so this is run once per file and then the manifest is the record:

```sh
export BOURBAKI_CORPUS=$PWD
bourbaki books add "pdf/en/Algebra Chapter 8 (2023, Springer Nature).pdf" \
  --id alg-viii --book alg --lang en --chapters VIII
bourbaki books add "pdf/fr/Algèbre_ Chapitre 8 (2012, Springer).pdf" \
  --id alg-viii-fr --book alg --lang fr --chapters VIII
bourbaki books list
bourbaki books verify
```

Then per volume. A native volume is three commands and a few minutes:

```sh
bourbaki pagemap build --book alg-viii
bourbaki extract       --book alg-viii
bourbaki assemble      --book alg-viii
```

A scan is four, and the middle two are the ones that take days:

```sh
bourbaki pagemap build --book alg-i-iii
bourbaki render        --book alg-i-iii --dpi 300
bourbaki ocr           --book alg-i-iii
bourbaki assemble      --book alg-i-iii
```

A volume with no text layer at all cannot have its page map read off the file, so on those three `pagemap build` runs after `render` and `ocr` rather than before. That is the third path and it is why *Commutative Algebra*, *General Topology Chapters 5-10* and *Algèbre chapitre 10* are the last volumes anybody should pick up.

The rest is corpus wide and runs after any volume changes:

```sh
bourbaki tags assign && bourbaki tags merge && bourbaki tags verify
bourbaki refs build
bourbaki report readme --write
bourbaki audit --report reports/audit.md
```

`assemble` writes the section files, the exercise files and the two manifests in one pass, and sweeps whatever an earlier split left behind. `assemble --check` is the same run with the writing taken out and a diff put in its place, which is what CI runs.

OCR runs against a small fleet of hosts over SSH. Round trips are slow, roughly 150 seconds a call, so every long stage is resumable and safe to interrupt.

## Where the numbers are

`reports/` is generated and checked by CI, so it is the state of the corpus rather than a snapshot somebody remembered to update. `audit.md` lists every finding by file and line. `extraction-quality.md` says how much of each volume has been read and how much of that passes the rules. `refs-unresolved.md` and `out-of-corpus.md` are the references that resolve to nothing and the ones that point outside the corpus.

<!-- BEGIN RULES -->
The audit is 73 rules in nine groups: 12 structure, 9 tags, 13 mathematics, 6 figures, 3 references, 16 translation, 6 solutions, 1 publication and 7 hygiene. 59 of them are hard, which means a finding fails the build, and 14 are soft.
<!-- END RULES -->

`what-it-cost.md` and `reproduction.md` are the two written by hand. The first says what the transport cost, which checks caught what, and what is still wrong, including the numbers that do not flatter the project. The second is the record of cloning both repositories fresh and running the pipeline from the PDFs to see whether it produces what is committed: 2775 of 2868 pages of the six deterministic volumes came back byte for byte, and everything derived from the pages came back identical.

## Licence

Transcriptions, translations and solutions here are derived from copyrighted material and exist for personal study only. *Éléments de mathématique* is copyright N. Bourbaki and its publishers. No source PDF is distributed.
