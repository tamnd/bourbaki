---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 0
section_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
kind: front
lang: en
source: ts-iii-v-fr
book_pages: TS III.1-TS III.2
pdf_pages: 0015-0016
extraction: native
statements: 0
exercises: 0
content_sha256: cf641e4cbb31fe3db85b127e2ad05f309c8c542af9c2da074b4581d2bd1d69cb
translated_from: content/fr/ts/III/00_frontmatter.md
source_lang: fr
translation_method: machine
source_content_sha256: 9c67ed516de2b1d0b8a9b5cd130ad06d36e82e59f0d089c902435a9e6cd50783
translation_model: gpt-5-6-mini
translation_run: translate-en-mt-ce3df524
glossary_version: 34
glossary_terms_sha256: d96a120c424c90a7234ac4be214f6beeeec2756c8be736530f9f174a57fe5b06
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## CHAPTER III

# Compact linear mappings and perturbations

In this chapter, all the vector spaces considered are vector spaces over a field K equal to $\mathbf{R}$ or $\mathbf{C}$. The references to EVT, II made in this book concern in general the case where $K =\mathbf{R}$; for the case where $K =\mathbf{C}$, cf. EVT, II, p. 64 to 68.

A semi-normed space is called a vector space E endowed with a semi-norm $p$ and the topology defined by $p($cf. EVT, II, p. 2). The unit ball of E, or of $p$, is called the set of elements $x$ of E such that $p(x)\leqslant 1$.

For every vector space E, $1_E$ denotes the identity mapping of E. If E, F and G are vector spaces and $u: E\rightarrow F,v: F\rightarrow G$ are linear mappings, one sometimes denotes by $vu$ the linear mapping $v\circ u$ from E into G.

Let E and F be topological vector spaces. A continuous linear mapping from E into F will also be called a morphism and an endomorphism when F = E. A bijective linear mapping from E into F which is continuous as well as its inverse will be called an isomorphism and, when F = E, an automorphism. When E and F are semi-normed spaces, the notions of endomorphism, isomorphism and automorphism refer to the underlying topological vector space structure.

Given topological vector spaces E and F, $\mathscr{L}^f(E; F)$ denotes the vector space of continuous linear mappings of finite rank from E into F. One also denotes by $\mathscr{L}^f(E)$ the vector space $\mathscr{L}^f(E; E)$.

Recall that a continuous linear mapping $u$ from E into F is strict if it induces by passing to the quotient an isomorphism of $E/$ Ker($u$) into $u(E)$ (TG, III, p. 16, déf. 1); it is equivalent to saying that the image of every neighbourhood of 0 in E is a neighbourhood of 0 in $u(E)$ (TG, III, p. 16, prop. 24).
