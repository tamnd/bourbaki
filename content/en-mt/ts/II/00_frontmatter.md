---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 0
section_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
kind: front
lang: en
source: ts-i-ii-fr
book_pages: TS II.199-TS II.200
pdf_pages: 0211-0212
extraction: native
statements: 0
exercises: 0
content_sha256: ac933dd2b350523831b4b93be737609a274c5a1c52ebe24ee0bd80640061df4f
translated_from: content/fr/ts/II/00_frontmatter.md
source_lang: fr
translation_method: machine
source_content_sha256: 5912ad9eba464c6032275167e5055b010b063b8c22eb36117a9aa868b2485691
translation_model: gpt-5-mini
translation_run: translate-en-mt-05cd1fae
glossary_version: 34
glossary_terms_sha256: 168c337389ee8393000bd6c4153109a500b482d478e8d3999ab1d664d71a9699
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## CHAPTER II

# Commutative locally compact groups

Throughout this chapter, the letter G denotes, unless otherwise mentioned, a commutative locally compact group endowed with a Haar measure generally denoted by $dx$; for $p\in [1,+\infty ]$, the space $L^p(G, dx)$ will simply be denoted by $L^p(G)$, and its norm will be denoted by $f\mapsto  \|f\|_p$. We identify $L^1(G)$ with a subspace of $\mathscr{M}^1(G)$ by the canonical mapping $f\mapsto f\cdot dx$. We recall that the support of the Haar measure is equal to G (INT, VII, §1, n$^o1$, remark 3); in particular (INT, III, §2, n$^o2$, proposition 9), the canonical mapping of the space $\mathscr{K}(G)$ into $L^p(G)$ is injective for $p\in [1,+\infty ]$. For $p\not= +\infty$, we shall identify $L^p(G)$ with a subspace of the space $\widetilde{\mathscr{F}}(G;\mathbf{C})$ of classes of complex-valued functions on G defined and finite almost everywhere (INT, IV, §3, n$^o5$, n$^o6$). In particular, the notation $L^1(G)\cap L^2(G)$ denotes the intersection of $L^1(G)$ and $L^2(G)$ in this space. We denote by $f\mapsto \widetilde{f}$ the involution on the involutive algebra $L^1(G)$ (example 4 of I, p. 99); we have $\widetilde{f}(x) =\overline{f(x^{-1})}$ for every $x$ in G.

We recall (INT, V, §5, n$^o3$, th. 1) that if $\mu$ is a complex measure on a locally compact topological space X and if $f$ is a locally $\mu$-integrable function on X, then the measure $\nu$ of density $f$ with respect to $\mu$ is denoted by $f\cdot \mu$ or also $f \mu$. A function $g$ of X into $\mathbf{C}$ is essentially integrable for the measure $\nu$ if, and only if, $gf$ is essentially integrable for $\mu$; one then has

$$
(f\cdot \mu)(g) =\int_Xgd(f\cdot \mu) =\int_Xgf d\mu=\mu(gf)
$$

If G is a compact topological group, the normalized Haar measure on G is called the unique Haar measure $\mu$ on G such that $\mu(G) = 1$.

If X is a discrete topological space, the counting measure on X is called the discrete measure $\mu$ on X such that $\mu(\{x\}) = 1$ for every $x\in X$. If G is a discrete topological group, the counting measure on G is a Haar measure on G.

We shall also make use of the following two lemmas.

**Lemma 1.** — Let X be a locally compact topological space and $\mu$ a positive measure on X. Let $x$ be an element of the support of $\mu$. Let U be an open neighbourhood of $x$. There exists a function $f\in \mathscr{K}_+(X)$ whose support is contained in U such that $\int f d\mu= 1$.

By definition of the support of a measure (INT, III, §2, n$^o2$, def. 1), there exists a function $g\in \mathscr{K}(X)$ with support contained in U such that $\mu(g)\not= 0$. We then have $\mu(|g|)>0$ since $\mu$ is positive, and the function $f=\mu(|g|)^{-1}|g|$ has the desired properties.

**Lemma 2.** — Let G and H be topological groups with neutral elements $e_G$ and $e_H$; suppose that the topological group G is separated. Let $f$ be a homomorphism of topological groups from G into H. Suppose that for every neighbourhood U of $e_G$ in G, there exists a neighbourhood W of $e_H$ in H such that $\overset{-1}{f}(W)\subset U$. Then, the homomorphism $f$ is injective and strict (TG, III, p. 16, def. 1).

The hypotheses imply that Ker($f$) is contained in every neighbourhood of $e_G$ in G, hence that Ker($f$) $=\{e_G\}$ since G is separated. The homomorphism from G into $f(G)$ deduced from $f$ by passing to the subspaces is then bijective; denote by $g:f(G)\rightarrow G$ the reciprocal homomorphism. The hypotheses then imply that $g$ is continuous at $e_H$, hence continuous (TG, III, p. 15, prop. 23).
