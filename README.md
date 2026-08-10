# bourbaki

A permanently-addressable, multilingual Markdown edition of Nicolas Bourbaki's
*Éléments de mathématique*, built from the original PDFs, organised in the
spirit of the [Stacks Project](https://stacks.math.columbia.edu/), with every
exercise solved and verified.

This repository holds the **corpus**: Markdown, tags, manifests and reports.
The **code** that produces it lives in
[`tamnd/bourbaki-solver`](https://github.com/tamnd/bourbaki-solver).

## Scope

| Book | Chapters | Edition | Pages | Source |
| --- | --- | --- | --- | --- |
| Algebra | I, II, III | 1998, Springer | 734 | scanned (JBIG2, 600 dpi) |
| Algebra | VIII | 2023, Springer Nature | 505 | born-digital |

The source PDFs are **not** in this repository and never will be. They are
copyright Springer / N. Bourbaki. This corpus exists for personal study.

## Permanent tags

Every numbered statement — definition, proposition, theorem, lemma, corollary,
remark, example, exercise — carries a four-character tag that is assigned once
and never changes, never gets reused, and survives any renumbering of the text.
This is the Stacks Project's contract, adopted verbatim.

```markdown
#### Proposition 6 {#alg-viii-s1-prop-6 .statement tag=0A3F}
```

`tags/tags` is append-only:

```
0A3F,alg-viii-s1-prop-6
```

A tag is the stable way to cite a result across the English, Vietnamese,
Chinese and Japanese editions: all four use the same tag for the same
statement.

## Layout

```
content/en/alg/<CH>/NN_sN_<slug>.md        one file per §
content/en/alg/<CH>/exercises/sN/NN.md     one file per exercise
content/{vi,zh,ja}/…                       same tree, same tags
content/solutions/<lang>/alg/<CH>/sN/NN.md verified solutions
tags/                                      the permanent tag index
manifests/                                 books, TOC, page maps, refs, glossary
figures/                                   cropped diagrams (small, committed)
reports/                                   audit, usage, coverage, scorecards
```

Ignored: `pdf/`, `images/`, `work/`.

## Coverage

<!-- BEGIN COVERAGE -->
_Not yet generated. Run `bourbaki report coverage --write-readme`._
<!-- END COVERAGE -->

## Reproducing

```sh
export BOURBAKI_CORPUS=$PWD
bourbaki books add "pdf/en/Algebra I Chapters 1-3 (1998, Springer).pdf" --id alg-i-iii
bourbaki books add "pdf/en/Algebra Chapter 8 (2023, Springer Nature).pdf"  --id alg-viii
bourbaki pagemap build --book alg-viii
bourbaki extract  --book alg-viii
bourbaki render   --book alg-i-iii --dpi 300
bourbaki ocr      --book alg-i-iii
bourbaki assemble --book alg-viii
bourbaki split    --book alg-viii --force --sync
bourbaki tags assign && bourbaki tags merge && bourbaki tags verify
bourbaki audit --report reports/audit.md
```

Full specification: `docs/spec/` in `tamnd/bourbaki-solver`.

## Licence

The transcription, translations and solutions in this repository are derived
works of copyrighted material and are here for personal study and educational
purposes only. *Éléments de mathématique* is copyright N. Bourbaki and its
publishers. No source PDF is distributed here.
