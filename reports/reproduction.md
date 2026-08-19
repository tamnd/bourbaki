# Reproducing the corpus from the PDFs

Written by hand. This is the record of a clean checkout run: both repositories cloned fresh, the volumes copied in, and the pipeline run from the PDFs to see whether it produces what is committed. It was done on 20 August 2026 against tamnd/bourbaki 882cc411 and tamnd/bourbaki-solver 7290536.

The corpus does not distribute the volumes, so a reproduction starts with somebody putting the same PDFs in `pdf/`. `bourbaki books verify` is what says they are the same ones: it checks the byte count and the SHA-256 of every file against `manifests/books.yaml`. All six volumes here verified before anything else was run, so what follows is about the code and not about the input.

## What was run

Six volumes were re-extracted. They are the six with a usable text layer that have been read all the way through, which is what makes a deterministic reproduction possible at all: no model is involved and the same PDF gives the same text every time.

```sh
git clone https://github.com/tamnd/bourbaki /tmp/repro
git clone https://github.com/tamnd/bourbaki-solver /tmp/repro-solver
cd /tmp/repro-solver && go build -o /tmp/repro-bk ./cmd/bourbaki
export BOURBAKI_CORPUS=/tmp/repro
# put the PDFs in /tmp/repro/pdf, then
/tmp/repro-bk books verify
/tmp/repro-bk pagemap build -book alg-viii
/tmp/repro-bk extract run   -book alg-viii
```

## Pages, PDF in and Markdown out

| volume | pages | identical | differ | repaired by hand | read by a model | drift |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| alg-viii | 505 | 465 | 40 | 40 | 0 | 0 |
| alg-viii-fr | 487 | 473 | 14 | 14 | 0 | 0 |
| lie-vii-ix | 439 | 420 | 19 | 7 | 12 | 0 |
| ta-i-iv-fr | 512 | 508 | 4 | 4 | 0 | 0 |
| ts-i-ii-fr | 346 | 336 | 10 | 5 | 0 | 5 |
| ts-iii-v-fr | 579 | 573 | 6 | 1 | 0 | 5 |
| **all** | **2868** | **2775** | **93** | **71** | **12** | **10** |

2775 of 2868 pages came back byte for byte identical, 96.8 per cent. So did every page map and every extraction report, which are not in the table because there is nothing to say about a file that did not change.

The 93 that differ are three different things and only one of them is a problem.

71 are pages somebody repaired by hand. They carry `manual: true` and extraction is forbidden to write over them, so the difference between the fresh run and the corpus is exactly the human edit. On page 38 of Algebra VIII the machine writes `\sigma '_i` and the corpus says `\sigma_i'`, which is the same repair M09 in the audit asks for. These are not reproducible and they are not supposed to be. A hand repair that a machine could reproduce would not need a hand.

12 are pages of Lie 7 to 9 that a model read because the text layer had lost a display there. They say `method: ocr` and a native re-extraction cannot produce them by definition. A model asked the same question twice does not give the same answer, which is the reason the OCR path writes what it got and records the model and the prompt hash rather than pretending to be a function.

10 are drift, and drift is the finding. Nine of them are #71: the corpus has `page_label: A II.285` where the current code produces `page_label: TS II.285`, with the folio stuck on the front of the running head in the committed copy and not in the fresh one. The fix for that is already in the extractor. Those nine pages were written before it and have never been extracted again, so the corpus is carrying the old answer on pages nobody has touched since. The tenth is `ts-i-ii-fr/0283`, where the corpus has a repaired bracket that the fresh run puts back the way it was, and unlike the other 71 repairs it does not say `manual: true`. A re-extraction of that volume would silently undo it. That one is #168.

## Everything downstream

With the committed pages back in place, the whole derived half of the corpus was rebuilt on the clean checkout:

```sh
/tmp/repro-bk assemble -book <each of the seven> -check
/tmp/repro-bk tags assign && /tmp/repro-bk tags merge
/tmp/repro-bk refs build
/tmp/repro-bk report coverage -write-readme
/tmp/repro-bk audit -validate-tex -report reports/audit.md
```

`git status` was empty afterwards. Every section file, every exercise file, both tag manifests, all the reference manifests, the coverage table in the README and the audit report came back identical to what is committed. The audit exits non zero because of the 40 hard findings it is supposed to report, not because anything moved.

That is the part of the claim that is now a fact rather than an intention. Given the pages, everything else in the corpus is a pure function of them and of the code, and it does not depend on the machine, on the order things were run in, or on anything left over in a working directory from an earlier run.

## What this does not show

`ens-i-iv` and `alg-x-fr`, 464 pages between them, were read by a model and cannot be reproduced this way at all. That is 14 per cent of the pages the corpus holds. The most that can be said about them is that the pages on disk pass the rules, which `reports/extraction-quality.md` says, and that the sections assembled from them are what the assembler produces, which the run above says.

The 35 volumes that have not been read are not in this at all.

The binary was built from a clean clone and the corpus from a clean clone, and the run was done on the same machine that did the original extraction. A different machine with a different pdftotext could still disagree, and nobody has tried it.
