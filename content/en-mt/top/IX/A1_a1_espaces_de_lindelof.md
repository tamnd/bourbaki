---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 1
section_title: Espaces de Lindelöf
appendix: true
lang: en
source: top-v-x-fr
pdf_pages: 0195-0197
extraction: ocr
statements: 8
exercises: 0
content_sha256: 5aac80a9b98ddbb1cf5a95c04cc8ed38c807091d7166c22e6a9660e70b077fde
translated_from: content/fr/top/IX/A1_a1_espaces_de_lindelof.md
source_lang: fr
translation_method: machine
source_content_sha256: 82bfed792246d4a3deff3f24ca86e0dd2545d6e631cac69468985fcbd6107a27
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-en-mt-8d180061
glossary_version: 34
glossary_terms_sha256: 92b13f6c2b473ece78abc2ebd696ecbaaca68d12c26a8be377b05ee8117b4d0a
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## APPENDIX 1

# LINDELÖF SPACES

#### Definition 1 {#top-ix-a1-def-1 .statement}

One says that a topological space $X$ (not necessarily separated) is a Lindelöf space if, from every open covering of $X$, one can extract a countable covering of $X$.

#### Proposition 1 {#top-ix-a1-prop-1 .statement}

Let $X$ be a topological space.

(i) If the topology of $X$ admits a countable base, $X$ is a Lindelöf space.

(ii) Let $f : X \to Y$ be a continuous mapping from $X$ into a topological space $Y$ (not necessarily separated). If $X$ is a Lindelöf space, the same is true of the subspace $f(X)$ of $Y$.

(i) Let $\mathcal{R}$ be an open covering of $X$, $\mathcal{B}$ a countable base of the topology of $X$, $\mathcal{B}'$ the set of elements $A \in \mathcal{B}$ such that there exists an element of $\mathcal{R}$ containing $A$; $\mathcal{B}'$ is a countable covering of $X$, since every $x \in X$ is contained in a set $U \in \mathcal{R}$, and there exists then $A \in \mathcal{B}$ such that $x \in A \subset U$. There then exists a mapping $\Phi$ from $\mathcal{B}'$ into $\mathcal{R}$ such that one has $A \subset \Phi(A)$ for every $A \in \mathcal{B}'$; it is clear that $\Phi(\mathcal{B}')$ is a countable open covering of $X$ contained in $\mathcal{R}$.

(ii) Let $(V_\lambda)_{\lambda \in L}$ be a family of open sets in $Y$ forming a covering of $f(X)$. The sets $f^{-1}(V_\lambda)$ then form an open covering of $X$, and there exists consequently a countable subset $J$ of $L$ such that the open sets $f^{-1}(V_\lambda)$ for $\lambda \in J$ form a covering of $X$. But then the sets $V_\lambda$ for $\lambda \in J$ form a covering of $f(X)$, which proves that $f(X)$ is a Lindelöf space.

#### Corollary {#top-ix-a1-n0-cor-1 .statement}

*Every sub-Lindelöf space, and in particular every Polish or Lusin space, is a Lindelöf space.*

This follows immediately from the preceding prop. 1 and from the definition of sub-Lindelöf spaces (IX, p. 59, def. 2), since a Polish space admits a countable base.

#### Proposition 2 {#top-ix-a1-prop-2 .statement}

*Every regular Lindelöf space is paracompact.*

Soit $X$ a regular Lindelöf space, and $\mathcal{R}$ an open covering of $X$. For every $x \in X$, let $U_x \in \mathcal{R}$ containing $X$, and let $V_x$ be an open neighbourhood of $x$ such that $V_x \subset U_x$. Since $X$ is a Lindelöf space, there exists a sequence $(x_n)_{n \geq 0}$ of points of $X$ such that the $V_{x_n}$ form a covering of $X$. Put then, for every integer $n \geq 0$, $W_n = U_{x_n} \cap \complement \left( \bigcup_{k < n} V_{x_k} \right)$. The sets $W_n$ are open and form a covering of $X$ finer than $\mathcal{R}$. On the other hand, this covering is locally finite, since every $x \in X$ belongs to some $V_{x_i}$ for at least one $i$; then $V_{x_i}$ is a neighbourhood of $x$, which meets no set $W_n$ for $n > i$.

#### Corollary {#top-ix-a1-n0-cor-2 .statement}

*Every regular sublinian space is paracompact* (and in particular *normal* (IX, p. 49, prop. 4) and *a fortiori completely regular*).

#### Proposition 3 {#top-ix-a1-prop-3 .statement}

*Let $X$ be a topological space (not necessarily separated). The following properties are equivalent*:
a) *Every open subspace of $X$ is a Lindelöf space*.
b) *Every set of lower (resp. upper) semicontinuous functions in $X$ contains a countable subset which admits the same upper (resp. lower) envelope*.

Let us first show that b) implies a). Let $U$ be an open subspace of $X$, and let $(U_\lambda)_{\lambda \in L}$ be a family of open sets in $U$ (hence in $X$) covering $U$. The functions $\varphi_{U_\lambda}$ being lower semicontinuous in $X$, there exists a countable subset $J$ of $L$ such that the family $(\varphi_{U_\lambda})_{\lambda \in J}$ has the same upper envelope $\varphi_U$ as the family $(\varphi_{U_\lambda})_{\lambda \in L}$. Consequently, $U = \bigcup_{\lambda \in J} U_\lambda$, and $U$ is a Lindelöf space.

Let us now prove that a) implies b). Let $\mathcal{F}$ be a set of lower semicontinuous functions in $X$, and let $s$ be the upper envelope of $\mathcal{F}$. Let $D$ be a countable dense subset of $\overline{\mathbf{R}}$. For every function $f \in \mathcal{F}$ and every number $d \in D$, let $U_{f,d}$ be the open set of the $x \in X$ such that $f(x) > d$ (IV, p. 29). By assumption, there exists a countable subset $\mathcal{F}_d'$ of $\mathcal{F}$ such that

$$
\bigcup_{f \in \mathcal{F}} U_{f,d} = \bigcup_{f \in \mathcal{F}_d'} U_{f,d}.
$$

Let $\mathcal{F}' = \bigcup_{d \in D} \mathcal{F}'_d$, and denote by $s'$ the upper envelope of $\mathcal{F}'$. We obviously have $s \geqslant s'$; on the other hand, let $x$ be a point of $X$, and let $d$ be an element of $D$ such that $s(x) > d$; there exists a function $f \in \mathcal{F}$ such that $f(x) > d$; hence $x \in U_{f,d}$, and there exists a function $f' \in \mathcal{F}'_d$ such that $x \in U_{f',d}$. Consequently, we also have $s'(x) > d$, whence the inequality $s' \geqslant s$, and finally $s' = s$. Since $\mathcal{F}'$ is countable, the assertion is established for lower semi-continuous functions; the case of upper semi-continuous functions is reduced to it by changing the sign.

#### Corollary 1 {#top-ix-a1-prop-3-cor-1 .statement}

*Let $X$ be a regular souslinian space, $H$ a set of continuous numerical functions in $X$, which separates the points of $X$* (IX, p. 9, def. 5). *There then exists a countable subset $H'$ of $H$ which separates the points of $X$*.

Indeed, $X \times X$ is a souslinian space (IX, p. 60, prop. 7); the same is true of every open subspace of $X \times X$ (IX, p. 59, prop. 5), which is therefore a Lindelöf space (IX, p. 76, corollary). To every function $h \in H$, associate the closed set $F_h$ of the pairs $(x, y) \in X \times X$ such that $h(x) = h(y)$. By virtue of prop. 3, there exists a countable subset $H'$ of $H$ such that one has $\bigcap_{h \in H'} F_h = \bigcap_{h \in H} F_h$. But by assumption the second member is the diagonal of $X \times X$; the same is therefore true of the first, and consequently $H'$ separates the points of $X$.

#### Corollary 2 {#top-ix-a1-prop-3-cor-2 .statement}

*Every compact souslinian space is metrizable*.

Let $X$ be a compact souslinian space, $I$ the interval $[0, 1]$ of $\mathbf{R}$, $H$ the set of continuous mappings of $X$ into $I$. Since $X$ is completely regular, $H$ separates the points of $X$, and cor. 1 implies the existence of a sequence $(f_n)$ of elements of $H$ which separates the points of $X$. But then the mapping $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ of $X$ into $I^\mathbf{N}$, continuous and injective, is a homeomorphism of the compact space $X$ onto a subspace of $I^\mathbf{N}$; this proves that $X$ is metrizable.
