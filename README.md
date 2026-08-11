# bourbaki

Bourbaki's *Éléments de mathématique* as Markdown, with permanent tags, translations, and worked exercises.

The source PDFs go in, Markdown comes out. Every numbered statement gets a four-character tag that never changes, so you can cite a result and have the citation still work after the text is re-extracted, re-split, or renumbered. That idea is lifted straight from the [Stacks Project](https://stacks.math.columbia.edu/).

This repo is the corpus only. The code that builds it lives in [tamnd/bourbaki-solver](https://github.com/tamnd/bourbaki-solver).

## What is in scope

| Book | Chapters | Edition | Pages | Sections | PDF |
| --- | --- | --- | --- | --- | --- |
| Algebra | I, II, III | 1998, Springer | 734 | 34 | scan, JBIG2 at 600 dpi |
| Algebra | IV, V, VI, VII | 2003, Springer | 460 | 30 | scan, JBIG2 at 600 dpi |
| Algebra | VIII | 2023, Springer Nature | 505 | 25 | born digital |

1699 pages, 89 sections, chapters I through VIII of the Book *Algebra*. The count is §§ and appendices together, because an appendix carries numbered statements and exercises exactly as a § does and is a file like any other. Chapters IX and X have no English translation, so they are out of scope until one exists.

The two scans need vision OCR. The 2023 volume has a real text layer and extracts natively with `pdftotext -layout`, which is why it goes first.

The PDFs are not here and will not be. They are copyright Springer and N. Bourbaki. This corpus is for personal study.

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

A tag is never reused and never edited. If a label has to change, the tag follows the statement and the old label goes to `tags/aliases`. The English, Vietnamese, Chinese and Japanese editions all use the same tag for the same statement, so a tag is the one identifier that works across all four.

## Layout

```
content/en/alg/<CH>/NN_sN_<slug>.md          one file per §
content/en/alg/<CH>/exercises/sN/NN.md       one file per exercise
content/{vi,zh,ja}/...                       same tree, same tags
content/solutions/<lang>/alg/<CH>/sN/NN.md   verified solutions
tags/                                        permanent tag index
manifests/                                   books, TOC, page maps, refs, glossary
figures/                                     cropped diagrams, small, committed
reports/                                     audit, usage, coverage, scorecards
```

`pdf/`, `images/` and `work/` are gitignored. Nothing large or copyrighted is committed.

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
| Algebra | VIII | 25 of 25 | 706 | 317 | 1023 | 488 |

25 of 89 sections are in the corpus, 28 per cent. 706 statements and 317 exercises, 1023 of them carrying a permanent tag.
<!-- END COVERAGE -->

## Building it

```sh
export BOURBAKI_CORPUS=$PWD
bourbaki books add "pdf/en/Algebra I Chapters 1-3 (1998, Springer).pdf"     --id alg-i-iii
bourbaki books add "pdf/en/Algebra II Chapters 4 - 7 (2003, Springer).pdf"  --id alg-iv-vii
bourbaki books add "pdf/en/Algebra Chapter 8 (2023, Springer Nature).pdf"   --id alg-viii
bourbaki pagemap build --book alg-viii
bourbaki extract  --book alg-viii
bourbaki render   --book alg-i-iii --dpi 300
bourbaki ocr      --book alg-i-iii
bourbaki assemble --book alg-viii
bourbaki tags assign && bourbaki tags merge && bourbaki tags verify
bourbaki refs build
bourbaki report coverage --write-readme
bourbaki audit --report reports/audit.md
```

`assemble` writes the section files, the exercise files and the two manifests in one pass, and sweeps whatever an earlier split left behind. `assemble --check` is the same run with the writing taken out and a diff put in its place, which is what CI runs.

OCR runs against a small fleet of hosts over SSH. Round trips are slow, roughly 150 seconds a call, so every long stage is resumable and safe to interrupt.

## Licence

Transcriptions, translations and solutions here are derived from copyrighted material and exist for personal study only. *Éléments de mathématique* is copyright N. Bourbaki and its publishers. No source PDF is distributed.
