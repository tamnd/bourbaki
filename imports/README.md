# imports

Sections read off public ChatGPT share links, before anything has checked them.

This is not corpus. It is raw material, and it is kept in a tree of its own so that it cannot be mistaken for corpus by a person or by a program. Every audit rule the project has runs over `content/`, so a file dropped in there passes 46 rules by default. Nothing in here has passed anything.

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

## What is here

| Book | Section | Answers | Source |
| --- | --- | --- | --- |
| Theory of Sets | Introduction | 7 | [share](https://chatgpt.com/share/6a7af1d4-31e0-83ec-afd1-608a29c56c91) |
| Theory of Sets | I § 1 Terms and relations | 13 | [share](https://chatgpt.com/share/6a7af1eb-3f74-83ec-9612-45e6992e80d6) |
| Theory of Sets | I § 2 Theorems | 4 | [share](https://chatgpt.com/share/6a7af1fc-8b58-83ec-a536-d08d9af4ceeb) |
| Theory of Sets | I § 3 Logical theories | 11 | [share](https://chatgpt.com/share/6a7af21b-ad94-83ec-a26f-0cee7f09077f) |

Theory of Sets is not in `manifests/books.yaml` and has no PDF here, which is the other reason these sit apart: there is nothing to check them against yet.
