---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 1
section_title: Convolution
lang: en
source: int-vii-ix
pdf_pages: 0101-0108, 0159-0159
extraction: ocr
subsections:
    - "no": 1
      title: Definition and examples
      page: 0
      pdf_page: 101
    - "no": 2
      title: Associativity
      page: 3
      pdf_page: 103
    - "no": 3
      title: The case of bounded measures
      page: 6
      pdf_page: 106
    - "no": 4
      title: Properties concerning supports
      page: 6
      pdf_page: 106
    - "no": 5
      title: Vectorial expression of the convolution product
      page: 7
      pdf_page: 107
statements: 13
exercises: 2
content_sha256: 05a5c461e581e8c2e10046aed639d554454123e90cb161ea1a5ac41500577113
---

## § 1. CONVOLUTION

### 1. Definition and examples

Recall (Ch. V, §6, Nos. 1 and 4; Ch. VI, §2, No. 10) that, if X and Y are locally compact spaces, $\mu$ a measure on X, and $\varphi$ a mapping of X into Y, $\varphi$ is said to be $\mu$-proper if: a) $\varphi$ is $\mu$-measurable; b) for every compact subset K of Y, $\varphi^{-1}(K)$ is essentially $\mu$-integrable. Then the image measure $\nu = \varphi(\mu)$ on Y exists and has the following property: for a function f on Y, with values in a Banach space or in $\overline{\mathbf{R}}$, to be essentially integrable for $\nu$, it is necessary and sufficient that $f \circ \varphi$ be so for $\mu$, in which case,

$$
\int_Y f(y)\, d\nu(y) = \int_X f(\varphi(x)) d\mu(x).
$$

#### Definition 1 {#int-viii-s1-def-1 .statement}

*Let $X_1, \ldots, X_n$ be locally compact spaces, $\mu_i$ a measure on $X_i$ ($1 \leq i \leq n$); let X be the product of the $X_i$, $\mu$ that of the $\mu_i$. Let $\varphi$ be a mapping of X into a locally compact space Y. One says that the sequence $(\mu_i)$ is $\varphi$-convolvable, or that $\mu_1, \ldots, \mu_n$ are $\varphi$-convolvable, if $\varphi$ is $\mu$-proper; in this case, the image $\nu = \varphi(\mu)$ of $\mu$ under $\varphi$ is called the convolution product of the $\mu_i$ for $\varphi$, and is denoted $*_{\varphi}(\mu_i)_{1 \leq i \leq n}$, or $*_{i=1}^n \mu_i$, or $\mu_1 * \mu_2 * \cdots * \mu_n$.

The last two notations are of course used only when there can be no doubt as to $\varphi$.

Let f be a function on Y, with values in a Banach space or in $\overline{\mathbf{R}}$. In order that f be essentially integrable for $\mu_1 * \cdots * \mu_n$, it is necessary and sufficient that the function

$$
(x_1, \ldots, x_n) \mapsto f(\varphi(x_1, \ldots, x_n))
$$

be essentially integrable for $\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$, in which case

$$
(1) \quad \int f\ d(\mu_1 * \cdots * \mu_n) = \int f(\varphi(x_1, \ldots, x_n)) d\mu_1(x_1) \ldots d\mu_n(x_n),
$$

a formula that may be regarded as *defining* $\mu_1 * \cdots * \mu_n$ when one takes $f \in \mathcal{K}(Y)$.

The definitions imply at once that the $\mu_i$ are convolvable if and only if the $|\mu_i|$ are. When this is the case,

$$
|\varphi(\mu_1 \otimes \cdots \otimes \mu_n)| \leq \varphi(|\mu_1 \otimes \cdots \otimes \mu_n|) = \varphi(|\mu_1| \otimes \cdots \otimes |\mu_n|)
$$
(Ch. VI, §2, No. 10), that is,

$$
(2) \quad |*_i \mu_i| \leq *_i |\mu_i|.
$$

If the $\mu_i$ are convolvable and positive, and if $\nu_i$ is a measure on $X_i$ such that $0 \leq \nu_i \leq \mu_i$, then the $\nu_i$ are convolvable and

$$
*_i \nu_i \leq *_i \mu_i.
$$

Suppose $\mu_1, \mu_2, \ldots, \mu_n$ are convolvable, and that $\mu'_1, \mu_2, \ldots, \mu_n$ are convolvable ($\mu'_1$ being a measure on $X_1$). By Ch. V, §6, No. 3, Cor. 1 of Prop. 6, $\mu_1 + \mu'_1, \mu_2, \ldots, \mu_n$ are convolvable and

$$
(\mu_1 + \mu'_1) * \mu_2 * \cdots * \mu_n = \mu_1 * \mu_2 * \cdots * \mu_n + \mu'_1 * \mu_2 * \cdots * \mu_n.
$$

#### Example {#int-viii-s1-n1-exa-1 .statement}

— 1) For any $\varphi$, the measures $\varepsilon_{x_i}$, where $x_i \in X_i$ for $1 \leq i \leq n$, are always convolvable and have convolution product $\varepsilon_y$, with $y = \varphi(x_1, x_2, \ldots, x_n)$. Consequently, if each of the $\mu_i$ has finite support, then the $\mu_i$ are convolvable and $\mu_1 * \cdots * \mu_n$ has finite support. In particular, let $M$ be a monoid$^1$ equipped with a locally compact topology; if one takes $\varphi$ to be the law of composition in $M$ then the measures on $M$ with finite support form, for convolution, an algebra that is none other than the *algebra of the monoid* $M$ (over $\mathbf{R}$ or over $\mathbf{C}$, according as one considers real or complex measures) (A, III, §2, No. 6).

2) Let $M$ be a monoid equipped with the discrete topology; assume that for each $m \in M$, there are only finitely many pairs $(m', m'') \in M \times M$ such that $m'm'' = m$; this amounts to saying that the law of composition in $M$ is a proper mapping of $M \times M$ into $M$; the measures on $M$ then form an algebra for convolution, an algebra that is none other than the *total*

(1) Monoïde, in the sense of Exer. 17 of Ch. VII, §1.

algebra of the monoid $M$ (A, III, §2, No. 10); we note the following two special cases:

a) $M = N$, the law of composition being addition. To every measure $\mu$ on $N$, let us associate the formal series

$$
S(\mu) = \sum_{n=0}^{\infty} \mu(\{n\}) t^n
$$

in an indeterminate $t$. Then $S(\mu * \mu') = S(\mu)S(\mu')$. An analogous remark holds for formal series in any number of indeterminates.

$*b)$ $M = N^*$, the law of composition being multiplication. To every measure $\mu$ on $N^*$, let us associate the formal Dirichlet series

$$
D(\mu) = \sum_{n=1}^{\infty} \mu(\{n\}) n^{-s}.
$$

Then $D(\mu * \mu') = D(\mu)D(\mu')$.

3) Let $X, Y, Z$ be locally compact spaces, $\varphi$ a continuous mapping of $X \times Y$ into $Z$. If $x \in X$ and $\mu$ is a measure on $Y$, to say that $\varepsilon_x$ and $\mu$ are $\varphi$-convolvable comes to saying that the mapping $\varphi(x, \cdot)$ of $Y$ into $Z$ is $\mu$-proper. One then has $\varepsilon_x * \mu = \varphi(x, \cdot)(\mu)$.

### 2. Associativity

The following lemma completes Prop. 11 of Ch. V, §8, No. 5:²

#### Lemma 1 {#int-viii-s1-lem-1 .statement}

For $1 \leq i \leq n$, let $X_i, Y_i$ be two locally compact spaces, $\mu_i$ a measure on $X_i$, and $\varphi_i$ a continuous mapping of $X_i$ into $Y_i$. Let $X = \prod_i X_i$, $Y = \prod_i Y_i$, $\mu = \bigotimes_i \mu_i$, and $\varphi$ the mapping of $X$ into $Y$ that is the product of the $\varphi_i$. If $\varphi$ is $\mu$-proper and $\mu_i \neq 0$ for each $i$, then the $\varphi_i$ are $\mu_i$-proper and $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$.

We can suppose that the $\mu_i$ are positive and $n = 2$. Let $f_1 \in \mathcal{K}_+(Y_1)$. Since $\mu_2 \neq 0$, there exists an $f_2 \in \mathcal{K}_+(Y_2)$ such that $f_2 \circ \varphi_2$ is not $\mu_2$-negligible. The function $(x_1, x_2) \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$ is essentially $\mu$-integrable and continuous, hence $\mu$-integrable. Therefore there exists an $x_2 \in X_2$ such that $f_2(\varphi_2(x_2)) \neq 0$ and such that the function $x_1 \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$ is $\mu_1$-integrable. Therefore $f_1 \circ \varphi_1$ is $\mu_1$-integrable,

²The lemma follows by induction on part b) of the cited Prop. 11, which is the case $n = 2$; the corresponding result in the first edition of Ch. V (§8, No. 3, Prop. 7) did not include the result of part b).

which proves that $\varphi_1$ is $\mu_1$-proper. One argues similarly for $\varphi_2$. Then $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$ by Prop. 11 of Ch. V, §8, No. 5.

The following lemma completes Prop. 4 of Ch. V, §6, No. 3.\footnote{The assertion of this lemma is in fact part *b*) of the cited Prop. 4, a part that was not included in the first edition of Ch. V.}

#### Lemma 2 {#int-viii-s1-lem-2 .statement}

*Let T, T', T'' be three locally compact spaces, $\mu$ a measure on T, $\pi$ a $\mu$-measurable mapping of T into T', $\pi'$ a continuous mapping of T' into T'', and $\pi'' = \pi' \circ \pi$. If $\pi''$ is $\mu$-proper, then $\pi$ is $\mu$-proper, $\pi'$ is $\pi(\mu)$-proper, and $\pi''(\mu) = \pi'(\pi(\mu))$.

Let K' be a compact subset of T'. Then $K'' = \pi'(K')$ is compact, therefore $\pi''(K'')$ is essentially $\mu$-integrable, therefore $\pi^{-1}(K') \subset \pi''(K'')$ is essentially $\mu$-integrable, thus $\pi$ is $\mu$-proper. Then $\pi'$ is $\pi(\mu)$-proper and $\pi''(\mu) = \pi'(\pi(\mu))$ by Ch. V, §6, No. 3, Prop. 4.

#### Proposition 1 {#int-viii-s1-prop-1 .statement}

*Let $X_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq n_i$), $Y_i$ ($1 \leq i \leq m$), and Z be locally compact spaces; for each i, let $\varphi_i$ be a mapping of $X_i = \prod_j X_{ij}$ into $Y_i$; let $\varphi$ be the product of the $\varphi_i$, mapping $X = \prod_i X_i$ into $Y = \prod_i Y_i$; let $\psi$ be a mapping of Y into Z.

(i) *Let $\mu_{ij}$ be measures given, respectively, on the $X_{ij}$, such that, for each i, the $\mu_{ij}$ ($1 \leq j \leq n_i$) are $\varphi_i$-convolvable, and such that the measures $*| \mu_{ij} |$ are $\psi$-convolvable; then the $\mu_{ij}$, for $1 \leq i \leq m, 1 \leq j \leq n_i$, are $(\psi \circ \varphi)$-convolvable and*

$$
*_{i,j} \mu_{ij} = *_i \left( *_j \mu_{ij} \right).
$$

(ii) *Assume $\psi$ and the $\varphi_i$ continuous, and let $\mu_{ij}$ be measures $\neq 0$ given, respectively, on the $X_{ij}$ and $(\psi \circ \varphi)$-convolvable; then, for each i, the $\mu_{ij}$ ($1 \leq j \leq n_i$) are $\varphi_i$-convolvable, the measures $*_j |\mu_{ij}|$ are $\psi$-convolvable, and the formula (3) holds.*

It suffices to consider the case that all of the measures in question are $\geq 0$.

Let us place ourselves under the hypotheses of (i). The mapping $\varphi$ is proper for $\bigotimes_{i,j} \mu_{ij}$, and

$$
\varphi \left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i \varphi_i \left( \bigotimes_j \mu_{ij} \right) = \bigotimes_i \left( *_j \mu_{ij} \right)
$$

(Ch. V, §8, No. 5, Prop. 11). The mapping $\psi \circ \varphi$ is proper for $\bigotimes_{i,j} \mu_{ij}$, and
$$
(\psi \circ \varphi)\left( \bigotimes_{i,j} \mu_{ij} \right) = \psi\left( \bigotimes_i (*_j \mu_{ij}) \right) = *_i (*_j \mu_{ij})
$$
(Ch. V, §6, Prop. 4). Therefore the $\mu_{ij}$ ($1 \leq i \leq m,\ 1 \leq j \leq n_i$) are $(\psi \circ \varphi)$-convolvable and formula (3) holds.

Let us place ourselves under the hypotheses of (ii). First of all, Lemma 2 proves that $\varphi$ is proper for $\bigotimes_{i,j} \mu_{ij}$. Lemma 1 then proves that for every $i$, $\varphi_i$ is proper for $\bigotimes_j \mu_{ij}$, and that
$$
\varphi\left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i (*_j \mu_{ij}).
$$
By Lemma 2, $\psi$ is proper for $\bigotimes_i (*_j \mu_{ij})$. Whence the proposition.

#### Corollary {#int-viii-s1-n2-cor-1 .statement}

— Let $X_i, X'_i$ ($1 \leq i \leq n$), $Y, Y'$ be locally compact spaces; let $\varphi, \varphi'$ be continuous mappings of $X = \prod_i X_i$ into $Y$ and of $X' = \prod_i X'_i$ into $Y'$, respectively; let $f_i$ be continuous mappings of $X_i$ into $X'_i$ ($1 \leq i \leq n$) and $g$ a continuous mapping of $Y$ into $Y'$, such that $\varphi' \circ f = g \circ \varphi$, $f$ being the mapping of $X$ into $X'$ that is the product of the $f_i$. Let $\mu_i$ be measures given respectively on the $X_i$, all $\neq 0$. Then the following two assertions are equivalent:
(i) $f_i$ is $\mu_i$-proper for all $i$, and the measures $f_i(|\mu_i|)$ are $\varphi'$-convolvable;
(ii) the $\mu_i$ are $\varphi$-convolvable, and $g$ is proper for $*_{\varphi}(|\mu_i|)$.

Moreover, when these assertions are verified,
$$
*_{\varphi'}(f_i(\mu_i)) = g(*_{\varphi}(\mu_i)) = *_{g \circ \varphi}(\mu_i).
$$

For, let $h = \varphi' \circ f = g \circ \varphi$. By Prop. 1, the conditions (i) and (ii) are each equivalent to the following condition:
(iii) the $\mu_i$ are $h$-convolvable.
When this is so,
$$
*_{\varphi'}(f_i(\mu_i)) = *_h(\mu_i) = g(*_{\varphi}(\mu_i)).
$$

### 3. The case of bounded measures

#### Proposition 2 {#int-viii-s1-prop-2 .statement}

— Let $X_1, \ldots, X_n, Y$ be locally compact spaces, $\mu_i$ a bounded measure on $X_i$ ($1 \leq i \leq n$), $\mu$ the product of the $\mu_i$, $\varphi$ a $\mu$-measurable mapping of $\prod_{i=1}^n X_i$ into $Y$. Then the $\mu_i$ are $\varphi$-convolvable and
$$
\left\| *_{i=1}^n \mu_i \right\| \leq \prod_{i=1}^n \| \mu_i \|.
$$
If the $\mu_i$ are moreover positive, then
$$
\left\| *_{i=1}^n \mu_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$
For, $\mu'_i = |\mu_i|$ is bounded and $\| \mu'_i \| = \| \mu_i \|$ (Ch. III, §1, No. 8, Cor. 1 of Prop. 10). One has $|\mu_1 \otimes \cdots \otimes \mu_n| = \mu'_1 \otimes \cdots \otimes \mu'_n$ (Ch. III, §4, Nos. 2, 4), therefore $\mu_1 \otimes \cdots \otimes \mu_n$ is bounded and
$$
\| \mu_1 \otimes \cdots \otimes \mu_n \| = \| \mu_1 \| \cdots \| \mu_n \|
$$
(ibid., Prop. 4). Therefore $\varphi$ is $\mu$-proper (Ch. V, §6, No. 1, Remark 1), that is, the $\mu_i$ are $\varphi$-convolvable. One has $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \otimes \cdots \otimes \mu'_n \|$ (Ch. V, §6, No. 2, Th. 1), consequently $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \| \cdots \| \mu'_n \|$. Finally, $| *_{i} \mu_i | \leq *_{i} \mu'_i$ (No. 1, formula (2)), therefore
$$
\left\| *_{i} \mu_i \right\| \leq \left\| *_{i} \mu'_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$

#### Proposition 3 {#int-viii-s1-prop-3 .statement}

— Let $X_1, \ldots, X_n, Y$ be locally compact spaces, $\varphi$ a continuous mapping of $\prod_{i=1}^n X_i$ into $Y$. Then the mapping
$$
(\mu, \ldots, \mu_n) \mapsto *_{\varphi} (\mu_i)
$$
of $\prod_{i=1}^n \mathcal{M}^1(X_i)$ into $\mathcal{M}^1(Y)$ is a continuous multilinear mapping.
This follows from Prop. 2 and what has been said in No. 1.

### 4. Properties concerning supports

#### Proposition 4 {#int-viii-s1-prop-4 .statement}

— Let $X_1, \ldots, X_n, Y$ be locally compact spaces, $\mu_i$ a measure on $X_i$ ($1 \leq i \leq n$), $S_i$ its support, and $\varphi$ a continuous mapping of $\prod_i X_i$ into $Y$ such that the restriction of $\varphi$ to $\prod_i S_i$ is proper. Then the $\mu_i$ are $\varphi$-convolvable.

For, let $K$ be a compact subset of $Y$. The support of $\mu = \mu_1 \otimes \cdots \otimes \mu_n$ is $S = \prod_i S_i$ (Ch. III, §4, No. 2, Prop. 2). Therefore $\overline{\varphi}(K) \cap \left( \prod_i X_i - S \right)$ is $\mu$-negligible. On the other hand, $\overline{\varphi}(K) \cap S$ is compact. Therefore $\overline{\varphi}(K)$ is $\mu$-integrable.

#### Proposition 5 {#int-viii-s1-prop-5 .statement}

*Let $X_1, \ldots, X_n, Y$ be locally compact spaces, $\mu_i$ a measure on $X_i$ ($1 \leq i \leq n$), $\mu$ the product of the $\mu_i$, $\varphi$ a $\mu$-proper mapping of $\prod_i X_i$ into $Y$, and $S_i$ the support of $\mu_i$.

a) *The support of $*_{i} \mu_i$ is contained in the closure of $\varphi \left( \prod_i S_i \right)$.*

b) *If $\varphi$ is continuous and the $\mu_i$ are positive, then the support of $*_{i} \mu_i$ is the closure of $\varphi \left( \prod_i S_i \right)$.*

Let $S = \prod_i S_i$ be the support of $\mu$. The support of $*_{i} \mu_i$ is contained in $\overline{\varphi(S)}$ by Ch. V, §6, No. 2, Cor. 3 of Prop. 2. *If $\varphi$ is continuous and the $\mu_i$ are positive, then the support of $*_{i} \mu_i$ is $\overline{\varphi(S)}$* (*loc. cit.*, Cor. 4 of Prop. 2).

#### Corollary {#int-viii-s1-n4-cor-1 .statement}

*If $\varphi$ is continuous and the $\mu_i$ have compact support, then the $\mu_i$ are convolvable and $*_{i} \mu_i$ has compact support.*

### 5. Vectorial expression of the convolution product

#### Proposition 6 {#int-viii-s1-prop-6 .statement}

*Let $X, Y, Z$ be locally compact spaces, $\varphi$ a continuous mapping of $X \times Y$ into $Z$, and $\lambda, \mu$ measures on $X, Y$. For $\lambda$ and $\mu$ to be $\varphi$-convolvable, it is necessary and sufficient that the mapping $(x, y) \mapsto \varepsilon_{\varphi(x,y)} = \varepsilon_x * \varepsilon_y$ of $X \times Y$ into $\mathcal{M}(Z)$ be scalarly $(\lambda \otimes \mu)$-integrable for the topology $\sigma(\mathcal{M}(Z), \mathcal{H}(Z))$, in which case*

$$
\lambda * \mu = \int_{X \times Y} (\varepsilon_x * \varepsilon_y) \, d\lambda(x) \, d\mu(y).
$$

To say that $\lambda$ and $\mu$ are $\varphi$-convolvable signifies that, for every $f \in \mathcal{H}(Z)$, $f \circ \varphi$ is $(\lambda \otimes \mu)$-integrable, that is, for every $f \in \mathcal{H}(Z)$ the function $(x, y) \mapsto \langle f, \varepsilon_{\varphi(x,y)} \rangle$ is $(\lambda \otimes \mu)$-integrable, that is, again, that the mapping $(x, y) \mapsto \varepsilon_{\varphi(x,y)}$ of $X \times Y$ into $\mathcal{M}(Z)$ is scalarly $(\lambda \otimes \mu)$-integrable for $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. If this is the case, then

$$
\langle \lambda * \mu, f \rangle = \int f(\varphi(x, y)) d\lambda(x) d\mu(y) = \int_{X \times Y} \langle \varepsilon_{\varphi(x,y)}, f \rangle d\lambda(x) d\mu(y),
$$

whence $\lambda * \mu = \int_{X \times Y} \varepsilon_{\varphi(x,y)} d\lambda(x) d\mu(y)$.

#### Proposition 7 {#int-viii-s1-prop-7 .statement}

*Let X, Y, Z be locally compact spaces, $\varphi$ a continuous mapping of $X \times Y$ into Z, and $\lambda, \mu$ measures on X, Y. Assume that for every $x \in X$, $\varepsilon_x$ and $\mu$ are $\varphi$-convolvable. For $\lambda$ and $\mu$ to be $\varphi$-convolvable, it is necessary and sufficient that the mapping $x \mapsto \varepsilon_x * |\mu|$ of X into $\mathcal{M}(Z)$ be scalarly $\lambda$-integrable for the topology $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, in which case $\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$.*

Suppose that $\lambda$ and $\mu$ are $\varphi$-convolvable. For every $f \in \mathcal{K}(Z)$, $f \circ \varphi$ is $(|\lambda| \otimes |\mu|)$-integrable, therefore the function $x \mapsto \int_Y f(\varphi(x, y)) d|\mu|(y) = \langle f, \varepsilon_x * |\mu| \rangle$ (which by hypothesis is defined for all $x \in X$) is $\lambda$-integrable; thus $x \mapsto \varepsilon_x * |\mu|$ is scalarly $\lambda$-integrable for $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, and

$$
\langle f, \lambda * \mu \rangle = \int_X d\lambda(x) \int_Y f(\varphi(x, y)) d\mu(y) = \int_X \langle f, \varepsilon_x * \mu \rangle d\lambda(x),
$$

whence $\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$. Conversely, suppose that the mapping $x \mapsto \varepsilon_x * |\mu|$ of X into $\mathcal{M}(Z)$ is scalarly $\lambda$-integrable for $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. Let $f \in \mathcal{K}_+(Z)$. Then the function $(x, y) \mapsto f(\varphi(x, y))$ is continuous and (Ch. V, §8, No. 3, Prop. 5)

$$
\iint^* f(\varphi(x, y)) d|\lambda|(x) d|\mu|(y) = \int^* d|\lambda|(x) \int^* f(\varphi(x, y)) d|\mu|(y)
= \int^* \langle f, \varepsilon_x * |\mu| \rangle d|\lambda|(x) < +\infty.
$$

Therefore $f \circ \varphi$ is $(\lambda \otimes \mu)$-integrable, so that $\lambda$ and $\mu$ are $\varphi$-convolvable.

### Exercises {#int-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
