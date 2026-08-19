# imports

Sections read off public ChatGPT share links, before anything has checked them.

This is not corpus. It is raw material, and it is kept in a tree of its own so that it cannot be mistaken for corpus by a person or by a program. Every audit rule the project has runs over `content/`, so a file dropped in there passes all 64 of them by default. Nothing in here has passed anything.

## Where it comes from

Somebody transcribed a book a page at a time in a ChatGPT conversation and made the conversation public. The share page carries the whole conversation inline in its HTML, so reading one is a plain HTTP GET with no account, no browser and no rate limit. That makes it by far the cheapest transcription this project has: the OCR path drives a browser on a server and waits about 150 seconds a page.

```sh
bourbaki share import -book sets \
  https://chatgpt.com/share/6a7af1d4-31e0-83ec-afd1-608a29c56c91 \
  https://chatgpt.com/share/6a7af1eb-3f74-83ec-9612-45e6992e80d6
```

A link goes where its conversation title says, or where a `1.1=<url>` label on the command line says. A title that does not say is an error and never a guess.

## Layout

```
imports/<book>/intro.md                 what comes before chapter 1
imports/<book>/chapter_<n>/<n>.<m>.md   one file per numbered section
```

## What the front matter records

```yaml
share_url: https://chatgpt.com/share/6a7af1eb-3f74-83ec-9612-45e6992e80d6
asks: 14
answers: 13
models: [gpt-5-6-thinking]
joined: 1 of 12
answers_sha256: cc6d2ade...
```

`asks` against `answers` is the first thing to look at. One more ask than answers is the instruction that opened the conversation; any bigger gap means a page went in and nothing came back.

`joined` is how many of the seams between one answer and the next were two halves of one paragraph. Each answer is one page of the book, so the seams are page turns, and a sentence broken across one has to be put back together. The rule is that an answer opening in lower case is finishing the sentence above rather than starting a new one, and it skips back over any footnote printed at the foot of the page. On the four sections here that is right about all 31 seams.

`answers_sha256` is the digest of the answers as they arrived, not of the file. Re-import after a change to the rendering and it still says this is the same conversation; a fetch that comes back different says so.

## What is checked, and what is not

Checked: the answers are free of refusals, narration and the provider's own markup, mathematics is balanced and closed, and the delimiters are the ones the corpus uses.

Not checked: whether any of it is what the book prints. Nobody has held these pages against the printed volume. Promoting a file into `content/` is a separate job with a person reading it, and until that happens this text should be read as a good transcription and not as the book.

## Promotion

`bourbaki share promote -book ens-i-iv -import sets` is the rule for moving a file out of here into `content/`. Four things have to hold, and every import file comes out of the command either promoted or listed with the reason it was not, because a file that appears in neither list is how an import ends up cited as the book.

It has to be a §. The introduction has no number and no place in the content layout, so it stays here.

`share audit` has to pass over it: every no. the printed contents lists, every label the pages print, and every page of the § found somewhere in the text. That says the transcription is of the whole section rather than most of it, which is the one thing that cannot be seen by reading the file on its own.

A person has to have read it against the printed volume and written that down in `manifests/imports.yaml`. No machine check stands in for this. `share audit` counts labels and looks for runs of words, and it cannot tell a correct statement from a fluent wrong one, which is the failure a model transcribing mathematics actually produces. The review is of a text and not of a filename, so it can record the digest of the body the reader had in front of them, and editing the import afterwards then breaks the sign-off rather than travelling with it.

And `content/` must not already hold a reading of that § made from the pages. This is the one that refuses everything here today. Theory of Sets was read off the rendered pages long before anyone had share links for it, so `content/en/ens` already holds every § of chapters I to IV. Those files carry `pdf_pages` and can be taken back to the page files and to the PDF. An import carries a link to a conversation. Writing the second over the first would swap a reading that has provenance for one that has none, and it would look like nothing had happened, because both are Markdown. So an import is promoted into a gap and never over a page. Where the two overlap, the import is a second opinion, which is worth having and is not a promotion.

A section that does promote is tagged and audited before the command returns, so a promotion that breaks a rule fails there rather than in CI later.

## What is here

| Book | Section | Answers | Source |
| --- | --- | --- | --- |
| Theory of Sets | Introduction | 7 | [share](https://chatgpt.com/share/6a7af1d4-31e0-83ec-afd1-608a29c56c91) |
| Theory of Sets | I § 1 Terms and relations | 13 | [share](https://chatgpt.com/share/6a7af1eb-3f74-83ec-9612-45e6992e80d6) |
| Theory of Sets | I § 2 Theorems | 4 | [share](https://chatgpt.com/share/6a7af1fc-8b58-83ec-a536-d08d9af4ceeb) |
| Theory of Sets | I § 3 Logical theories | 11 | [share](https://chatgpt.com/share/6a7af21b-ad94-83ec-a26f-0cee7f09077f) |

Theory of Sets is in `manifests/books.yaml` now, with a page map behind it, so all three §§ can be and have been held against the printed volume by `share audit`: 13 no., 46 labels and 21 pages accounted for, nothing missing. What none of them has is a reader, and `content/en/ens` already holds a reading of each from the pages, so `share promote` refuses all four files today and says which of the two reasons applies to each.
