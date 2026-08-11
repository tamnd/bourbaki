# bourbaki

Bourbaki's *Éléments de mathématique* as Markdown, with permanent tags, translations, and worked exercises.

The source PDFs go in, Markdown comes out. Every numbered statement gets a four-character tag that never changes, so you can cite a result and have the citation still work after the text is re-extracted, re-split, or renumbered. That idea is lifted straight from the [Stacks Project](https://stacks.math.columbia.edu/).

This repo is the corpus only. The code that builds it lives in [tamnd/bourbaki-solver](https://github.com/tamnd/bourbaki-solver).

## What is in scope

All twelve Books of the *Éléments*, in the English translation where one was printed and in the French original everywhere else. 43 volumes, 14989 pages, of which 15 volumes and 6648 pages are English and 28 volumes and 8341 pages are French.

| Book | English | French | Volumes | Pages |
| --- | --- | --- | --- | --- |
| Theory of Sets | I to IV | none held | 1 | 418 |
| Algebra | I to VIII | I to X | 8 | 3690 |
| General Topology | I to X | I to X | 4 | 1511 |
| Functions of a Real Variable | I to VII | I to VII | 2 | 683 |
| Topological Vector Spaces | I to V | I to V | 2 | 740 |
| Integration | I to IX | I to IX | 7 | 1732 |
| Commutative Algebra | I to VII | I to X | 5 | 1733 |
| Variétés différentielles et analytiques | never translated | fascicule de résultats | 1 | 190 |
| Lie Groups and Lie Algebras | I to IX | I to IX | 8 | 2182 |
| Théories spectrales | never translated | I to V | 2 | 925 |
| Topologie algébrique | never translated | I to IV | 1 | 512 |
| Elements of the History of Mathematics | whole | whole | 2 | 673 |

The French is not a fallback for the English. Three Books were never translated, Algèbre chapters IX and X and Algèbre commutative chapters VIII, IX and X exist in French only, and where both printings are held the French is the original a disputed English sentence gets checked against. So both are in scope and both carry the same tags.

Two gaps worth stating plainly. There is no French Théorie des ensembles here, only the English translation of it. And *Groupes et algèbres de Lie, Chapitres 7 et 8* is a partial file: 61 pages that open at Chapitre VII and stop in the middle of the exercises around printed page 65, so the English *Chapters 7-9* is the only complete copy of that material.

`bourbaki books list` prints the volume by volume detail, and `manifests/books.yaml` carries it as data, with the SHA-256 and page count of every file so that a swapped or re-downloaded PDF is caught rather than silently extracted.

The PDFs are not here and will not be. They are copyright Springer and N. Bourbaki. This corpus is for personal study.

## Three extraction paths, not one

What a volume costs to read depends entirely on what its own text layer is worth, and the library splits three ways. `bourbaki books add` measures this rather than guessing it, by sampling the images and the text of a band of body pages, and records the answer as `text_layer` in the manifest.

| Text layer | Volumes | What it means |
| --- | --- | --- |
| native | 6 | Born digital. `pdftotext -layout` gives real text and real mathematics. |
| ocr | 34 | A scan somebody has already run OCR over. Good enough to read a running head off, useless for mathematics. |
| none | 3 | A scan with no text at all. Even the page map has to come out of vision OCR. |

The six native volumes are *Algebra, Chapter 8* and *Lie Groups and Lie Algebras, Chapters 7-9* in English, and *Algèbre chapitre 8*, *Théories spectrales chapitres 1 et 2*, *Théories spectrales chapitres 3 à 5* and *Topologie algébrique chapitres 1 à 4* in French. They are cheap and they go first. The three with no text at all are *Commutative Algebra* at 642 pages, *General Topology Chapters 5-10* at 372 pages and *Algèbre chapitre 10* at 222 pages, and they are the most expensive volumes in the library.

The 34 in the middle are the ordinary case. Their OCR layer renders a pair of braces in *Theory of Sets* as `R! x, y I`, so nothing in it can be trusted as mathematics, but it is legible enough to build the page map from before a single page goes to vision OCR, which saves the expensive pass on all 34.

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

## Layout

```
content/en/<book>/<CH>/NN_sN_<slug>.md         one file per §
content/en/<book>/<CH>/exercises/sN/NN.md      one file per exercise
content/fr/...                                 same tree, extracted from the French printing
content/{vi,zh,ja}/...                         same tree, translated
content/solutions/<lang>/<book>/<CH>/sN/NN.md  verified solutions
tags/                                          permanent tag index
manifests/                                     books, TOC, page maps, refs, glossary
figures/                                       cropped diagrams, small, committed
reports/                                       audit, usage, coverage, scorecards
imports/<book>/chapter_<n>/<n>.<m>.md          read off share links, not yet checked
```

`content/fr` is not a translation and is never generated from `content/en`. It is what the French volume prints, extracted the same way the English is, which is why it carries no `translated_from` and is exempt from the translation rules.

`pdf/`, `images/` and `work/` are gitignored. Nothing large or copyrighted is committed.

`imports/` is deliberately outside `content/`. It holds sections read off public ChatGPT share links, which cost an HTTP GET rather than 150 seconds of a browser per page, and which nobody has yet held against the printed book. The audit runs over `content/`, so anything dropped in there would pass all 56 rules by default. See [imports/README.md](imports/README.md).

## Coverage

<!-- BEGIN COVERAGE -->
| Book | Chapter | Sections | Statements | Exercises | Tagged | Pages |
| --- | --- | --- | --- | --- | --- | --- |
| Algebra | I | 0 of 10 | 0 | 0 | 0 | 3 |
| Algebra | II | 0 of 12 | 0 | 0 | 0 | 0 |
| Algebra | III | 0 of 12 | 0 | 0 | 0 | 0 |
| Algebra | IV | 0 of 6 | 0 | 0 | 0 | 0 |
| Algebra | V | 0 of 17 | 0 | 0 | 0 | 0 |
| Algebra | VI | 0 of 2 | 0 | 0 | 0 | 1 |
| Algebra | VII | 0 of 5 | 0 | 0 | 0 | 1 |
| Algebra | VIII | 25 of 25 | 709 | 317 | 1026 | 964 |
| Theory of Sets | I | 0 of 6 | 0 | 0 | 0 | 0 |
| Theory of Sets | II | 0 of 6 | 0 | 0 | 0 | 0 |
| Theory of Sets | III | 0 of 7 | 0 | 0 | 0 | 0 |
| Theory of Sets | IV | 0 of 3 | 0 | 0 | 0 | 0 |
| Lie Groups and Lie Algebras | VII | 0 of 7 | 0 | 0 | 0 | 0 |
| Lie Groups and Lie Algebras | VIII | 0 of 13 | 0 | 0 | 0 | 0 |
| Lie Groups and Lie Algebras | IX | 0 of 11 | 0 | 0 | 0 | 0 |
| Topologie algébrique | I | 0 of 6 | 0 | 0 | 0 | 0 |
| Topologie algébrique | II | 0 of 5 | 0 | 0 | 0 | 0 |
| Topologie algébrique | III | 0 of 5 | 0 | 0 | 0 | 0 |
| Topologie algébrique | IV | 0 of 6 | 0 | 0 | 0 | 0 |
| Théories spectrales | I | 0 of 8 | 0 | 0 | 0 | 0 |
| Théories spectrales | II | 0 of 3 | 0 | 0 | 0 | 0 |
| Théories spectrales | III | 0 of 6 | 0 | 0 | 0 | 0 |
| Théories spectrales | IV | 0 of 5 | 0 | 0 | 0 | 0 |
| Théories spectrales | V | 0 of 4 | 0 | 0 | 0 | 0 |

25 of 190 sections are in the corpus, 13 per cent. 709 statements and 317 exercises, 1026 of them carrying a permanent tag.

The table is one row per chapter of the volumes that have a table of contents. 34 further volumes and 10509 pages are registered in `manifests/books.yaml` with no table of contents read off them yet, so none of their chapters are counted above.
<!-- END COVERAGE -->

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
bourbaki report coverage --write-readme
bourbaki audit --report reports/audit.md
```

`assemble` writes the section files, the exercise files and the two manifests in one pass, and sweeps whatever an earlier split left behind. `assemble --check` is the same run with the writing taken out and a diff put in its place, which is what CI runs.

OCR runs against a small fleet of hosts over SSH. Round trips are slow, roughly 150 seconds a call, so every long stage is resumable and safe to interrupt.

## Licence

Transcriptions, translations and solutions here are derived from copyrighted material and exist for personal study only. *Éléments de mathématique* is copyright N. Bourbaki and its publishers. No source PDF is distributed.
