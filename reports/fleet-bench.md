# Fleet bench, first OCR pilot

Twenty pages of Algebra I, pages 41 to 60 of the PDF, read on 10 August 2026. This is the first run of the OCR stage against real hardware and a real book, and the numbers below are what it did, not what it was meant to do.

## What the fleet is

Three rented Linux boxes, each running a pool of ChatGPT web sessions under Xvfb. A lane is one Chrome profile, and a lane wants about a gigabyte, so the lane count follows the free memory on the box and not the core count.

| host | cores | free memory | OCR lanes |
| --- | --- | --- | --- |
| server3 | 8 | 15378 MB | 4 |
| server2 | 6 | 7363 MB | 3 |
| server1 | 4 | 1334 MB | 0 |

server1 does no OCR. It has the cores for it and not the memory, and a box that cannot open a browser is worse than one that is idle, because it accepts the work and then fails every page of it.

## The baseline

A nine token text round trip to server3 takes 151 seconds. That is the number every page has to beat, and it is the reason the per page timeout was raised to fifteen minutes: the tool ships with a 120 second default, which is under the baseline, so it would have timed out on work that was going fine.

## What the pilot measured

server3, four lanes, in the order the batches ran:

| batch | pages read | elapsed | seconds a page |
| --- | --- | --- | --- |
| 1 | 5 of 5 | 5m16s | 63 |
| 2 | 5 of 5 | 8m21s | 100 |
| 3 | 3 of 5 | 21m25s | 428 |
| 4 | 1 of 4 | 23m1s | 1381 |
| 5 | 0 of 3 | 17m36s | none returned |

server2, three lanes:

| batch | pages read | elapsed | seconds a page |
| --- | --- | --- | --- |
| 1 | 4 of 5 | 31m41s | 475 |
| 2 | 1 of 3 | 18m47s | 1127 |
| 3 | 0 of 2 | 22m56s | none returned |

Over the whole run server3 read 12 pages in 1h15m39s, which is 10 pages an hour, and server2 read 3 pages in 1h13m23s, which is 2 pages an hour.

The first batch is the honest measure of what the fleet can do. Sixty three seconds a page on four lanes is 57 pages an hour, and it beats the 151 second baseline by a factor of two and a half. Nothing after the second batch is a measure of the fleet at all.

## Why it decayed

The driver starts a batch detached, so a dropped ssh tunnel cannot kill hours of reading. It also gave up on a batch that ran past its deadline without killing it, and nothing else was ever going to.

Ten minutes after the run ended, batch alg-i-iii-0055-232dcb was still running on server2 at 27 minutes elapsed. The driver had written it off at 22m56s. Under it were two live Chrome instances, and the box was at load 11.27 on six cores. Killing that one process group took the load to 6.08 and the Chrome process count from 22 to 1, within seconds.

So every abandoned batch made the next one slower, and a slower batch is more likely to be abandoned, and it leaves another one behind it when it is. The decay in the two tables above is that feedback loop, and it was self inflicted. The fix is in the driver: a batch the driver gives up on is now killed by process group, which reaches Chrome and its renderers as well as the tool.

## What the pages came to

Fifteen of the twenty pages were accepted, five are dead after three attempts. That is 75 percent, and the milestone asks for 95, so this does not pass.

The five dead pages are 44, 45, 51, 55 and 59. Their first attempts failed on real rules: two on unbalanced mathematics, one on length, two with no answer at all. Every one of their second and third attempts returned no answer, which is the decay above and not anything about those pages. They are worth re-reading on a rested fleet before anyone concludes there is something hard about them.

Retrying into a degrading fleet is wasted work. Fifteen retries went out over this run and not one of them returned a page.

## What was wrong with the pages that were accepted

Two of the fifteen, pages 50 and 53, carry a formula that opens with a dollar and never closes it. Both are the same shape, `$x\in E.` at the end of a paragraph. They were accepted because the balance rule counted dollars over the whole page, and page 53 has two unclosed ones, and two odd counts add to an even one. The rule now counts paragraph by paragraph, which catches both and names the line. Checked against the 494 native pages of Algebra VIII it flags nothing new, so it costs no false positives on the path that produces most of the corpus.

One page, 42, has two lines where a display equation came back as plain Unicode instead of LaTeX. No rule catches that yet and one page is not enough to calibrate one on.

## The failure that is now named rather than silent

An earlier run wrote `I don't see an image attached` into the corpus as page 42 and it passed every rule. The upload to the web session had failed, the prompt went anyway, and the model answered the only question it had been given.

Two things changed. The tool now refuses to submit a prompt when the upload preview never appears, so the batch log says `never attached (no upload preview after 60s)` instead of returning fluent English about a page nobody sent it. And the guard that catches a model talking instead of transcribing now straightens the typographic apostrophe before matching, because the model writes `don’t` with U+2019 and every phrase in that list was spelled with U+0027, so none of them had ever matched.

## Where this leaves the milestone

Not passed. The exit needs 95 percent of non-blank pages accepted and this run gave 75, and the sustained rate is nowhere near the peak rate.

What is settled: the transport works, the per host lane arithmetic is right, server1 is correctly excluded, the peak rate beats the baseline comfortably, and three defects that only show up against real hardware have been found and fixed.

What is not: whether the fleet holds its peak rate once batches are killed on time. That is the next measurement, and it wants a rested fleet and a run long enough to show whether the curve is flat.
