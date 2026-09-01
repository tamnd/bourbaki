---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 2
section_title: Produits infinis dans les algèbres normées
appendix: true
lang: en
source: top-v-x-fr
book_pages: TG IX.125-TG IX.126
pdf_pages: 0198-0204, 0245-0246
extraction: ocr
subsections:
    - "no": 1
      title: Suites multipliables dans une algèbre normée
      page: 0
      pdf_page: 198
    - "no": 2
      title: Critères de multipliabilité
      page: 79
      pdf_page: 199
    - "no": 3
      title: Produits infinis
      page: 82
      pdf_page: 202
statements: 16
exercises: 8
content_sha256: 15e574616b9216e369d5739775c51f5a56269afe461ad7819939a1d7fc3a9931
translated_from: content/fr/top/IX/A2_a2_produits_infinis_dans_les_algebres.md
source_lang: fr
translation_method: machine
source_content_sha256: 08e13ee94a1406e81b201e3c665c3629632ff1cabff45c15f5a1c0046f18485c
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-7b2672d1
glossary_version: 34
glossary_terms_sha256: f670a01ad9d838e9ba662cb92d2b4183eb2fc88c010d6047f21c97292758cb5d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## APPENDIX 2

# INFINITE PRODUCTS IN NORMED ALGEBRAS

### 1. Multipliable sequences in a normed algebra

Let $A$ be a normed algebra over a commutative non-discrete valued field (IX, p. 37, def. 9); we shall denote by $\|x\|$ the norm of an element $x \in A$, and we shall suppose moreover that $A$ admits a unit element $e$.

Let $(x_n)_{n \geq N}$ be an infinite sequence of points of $A$; every finite subset $J$ of $\mathbf{N}$, totally ordered by the order of $\mathbf{N}$, defines a sequence (A, I, p. 3) $(x_n)_{n \in J}$ of points of $A$; in Algebra (A, I, p. 3) the product $p_J = \prod_{n \in J} x_n$ of this sequence has been defined, which we shall call the finite partial product of the sequence $(x_n)_{n \in \mathbf{N}}$, corresponding to the finite subset $J$ of $\mathbf{N}$ (recall that, for $J = \varnothing$, one puts $\prod_{n \in \varnothing} x_n = e$).

#### Definition 1 {#top-ix-a2-def-1 .statement}

One says that the sequence $(x_n)_{n \geq N}$ is multipliable in the normed algebra $A$ if the mapping $J \mapsto p_J$ has a limit following the filter of sections of the set $\mathcal{F}(\mathbf{N})$ of finite subsets of $\mathbf{N}$, ordered by the relation $\subset$; this limit is called the product of the sequence $(x_n)_{n \in \mathbf{N}}$, and is denoted $\prod_{n \in \mathbf{N}} x_n$ (or simply $\prod_n x_n$); the $x_n$ are called the factors of this product.

Def. 1 is equivalent to the following one: the sequence $(x_n)$ is multipliable and has product $p$ if, for every $\varepsilon > 0$, there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for every finite subset $J \supset J_0$ of $\mathbf{N}$, one has $\|p_J - p\| \leq \varepsilon$.

#### Remark 1 {#top-ix-a2-n1-rem-1 .statement}

When $A$ is a commutative algebra, def. 1 is identical with that which was given in III, p. 37 (Remark 3); but when $A$ is not commutative, the order structure of the set of indices $\mathbf{N}$ intervenes in an essential way in def. 1; if $\sigma$ is any permutation of $\mathbf{N}$, nothing permits one to assert in general that the sequence $(\mathbf{x}_{\sigma(n)})$ is multipliable when the sequence $(\mathbf{x}_n)$ is; moreover, when these two sequences are multipliable, their products are in general different.

#### Remark 2 {#top-ix-a2-n1-rem-2 .statement}

Def. 1 generalizes immediately to the case of a family $(\mathbf{x}_n)_{n \in I}$ whose set of indices $I$ is a subset of $\mathbf{Z}$ (totally ordered by the order induced by that of $\mathbf{Z}$); we leave to the reader the task of extending to this case the following properties (cf. IX, p. 125, exerc. 1 and 2).

### 2. Criteria of multipliability

We shall henceforth restrict ourselves to the case where the normed algebra $A$ is complete.

#### Theorem 1 {#top-ix-a2-thm-1 .statement}

Let $(\mathbf{x}_n)_{n \in \mathbf{N}}$ be a sequence of points of a complete normed algebra $A$.

a) If $(\mathbf{x}_n)$ is multipliable and has for product an invertible element of $A$, for every $\varepsilon > 0$, there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for every finite subset $L$ of $\mathbf{N}$ not meeting $J_0$, one has $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$.

b) Conversely, if the sequence $(\mathbf{x}_n)$ satisfies this condition, it is multipliable. Moreover, if each of the $\mathbf{x}_n$ is invertible, $\prod_{n \in \mathbf{N}} \mathbf{x}_n$ is invertible.

a) Let $\mathbf{p}$ be the product of the multipliable sequence $(\mathbf{x}_n)$, and suppose that $\mathbf{p}$ is invertible in $A$; then (IX, p. 40, prop. 14), there exist $\alpha > 0$ and $a > 0$ such that, for every $y \in A$ such that $\| y - \mathbf{p} \| \leq \alpha$, $y$ is invertible, and $\| y^{-1} \| \leq a$. By assumption, for every $\varepsilon$ such that $0 < \varepsilon < \alpha$, there exists a finite subset $H_0$ of $\mathbf{N}$ such that, for every finite subset $H$ of $\mathbf{N}$ containing $H_0$, one has $\| \mathbf{p}_H - \mathbf{p} \| \leq \varepsilon$. Let $J_0 = \{0, m\}$ be an interval of $\mathbf{N}$ containing $H_0$; for every finite subset $L$ of $\mathbf{N}$ not meeting $J_0$ the integers belonging to $L$ are all greater than those belonging to $H_0$; therefore, if one sets $H = H_0 \cup L$, one has $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$. Now, since $\| \mathbf{p}_{H_0} - \mathbf{p} \| \leq \varepsilon \leq \alpha$, $\mathbf{p}_{H_0}$ is invertible, and one has $\| \mathbf{e} - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$; from the relation $\| \mathbf{p}_{H_0} \mathbf{p}_L - \mathbf{p} \| \leq \varepsilon$, one deduces $\| \mathbf{p}_L - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$ and finally $\| \mathbf{e} - \mathbf{p}_L \| \leq 2a \varepsilon$.

b) Suppose that, for every $\varepsilon > 0$, there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for every finite subset $L$ of $\mathbf{N}$ not meeting $J_0$, one has $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$. Let $H_0 = \{0, p\}$ be an interval of $\mathbf{N}$ containing $J_0$; every finite subset $H$ of $\mathbf{N}$ containing $H_0$ can be written $H_0 \cup L$, where the integers belonging to $L$ are greater than those belonging to $H_0$; we therefore have $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$, and since $L$ does not meet $J_0$, $\| \mathbf{p}_H - \mathbf{p}_{H_0} \| \leq \varepsilon \| \mathbf{p}_{H_0} \|$, and consequently $\| \mathbf{p}_H \| \leq (1 + \varepsilon) \| \mathbf{p}_{H_0} \|$. If $\mathbf{p}_{H_0} = 0$, the sequence $(\mathbf{x}_n)$ is obviously multipliable and has product 0; excluding this trivial case, there exists an interval $H_1 = \{0, q\}$, containing $H_0$ and such that, for every finite subset $L$ of $\mathbf{N}$ not meeting $H_1$, one has $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon (\| \mathbf{p}_{H_0} \|)^{-1}$. We deduce as above that, for every finite subset $H \supset H_1$

$$
\| \mathbf{p}_H - \mathbf{p}_{H_1} \| \leq (\| \mathbf{p}_{H_0} \|)^{-1} \| \mathbf{p}_{H_1} \| \varepsilon \leq \varepsilon (1 + \varepsilon).
$$

The Cauchy criterion therefore shows that $J \mapsto \mathbf{p}_J$ has a limit in $A$ following the filtered set $\mathcal{F}(\mathbf{N})$.

If all the $x_n$ are invertible, the same is true of all the finite partial products $p_J$; for every finite subset $H$ containing $H_0$, one can therefore write

$$
\| e - p_{H_0}^{-1} p_H \| \leq \varepsilon;
$$

this shows that, in the multiplicative group $G$ of the invertible elements of $A$, the image by the mapping $J \mapsto p_J$ of the filter of sections of $\mathfrak{F}(N)$ is a Cauchy filter basis for the left uniform structure of the group $G$; but since $G$ is complete ($IX$, p. 40, prop. 14), the limit of the mapping $J \mapsto p_J$ belongs to $G$.

#### Remark {#top-ix-a2-n2-rem-1 .statement}

When $(x_n)$ is multipliable and has a noninvertible product, the condition of th. 1 is no longer necessarily verified; for example, if all the $x_n$ are equal to the same element $x$ such that $\| x \| < 1$, the sequence $(x_n)$ is multipliable and has product 0, and for every nonempty finite subset $H$ of $N$, one has $\| p_H \| \leq \| x \| < 1 \leq \| e \|$.

#### Corollary 1 {#top-ix-a2-thm-1-cor-1 .statement}

*If* $(x_n)$ *is a multipliable sequence whose product is invertible in* $A$, $\lim_{n \to \infty} x_n = e$.

#### Corollary 2 {#top-ix-a2-thm-1-cor-2 .statement}

*If* $(x_n)$ *is a multipliable sequence whose product is invertible in* $A$, *any sequence* $(x_{n_k})_{k \in \mathbf{N}}$ *extracted from* $(x_n)$ *(($n_k$) being a strictly increasing sequence of integers) is multipliable*.

This is what the criterion of th. 1 ($IX$, p. 79) immediately shows.

#### Theorem 2 {#top-ix-a2-thm-2 .statement}

*Let* $A$ *be a complete normed algebra; if* $(u_n)$ *is an absolutely convergent series of points of* $A$, *the sequence* $(e + u_n)$ *is multipliable in* $A$; *moreover, if all the elements* $e + u_n$ *are invertible in* $A$, *the same is true of* $\prod_{n \in \mathbf{N}} (e + u_n)$.

Apply the criterion of $IX$, p. 79, th. 1; for every finite subset $L$ of $N$, we have $p_L = e - \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$, $M$ ranging over the set of the non-empty subsets of $L$ (totally ordered by the induced order). Since $\left| \prod_{n \in M} u_n \right| \leq \prod_{n \in M} \| u_n \|$, one can write

$$
\| p_L - e \| \leq \sum_M \left( \prod_{n \in M} \| u_n \| \right) = \prod_{n \in L} (1 + \| u_n \|) - 1.
$$

Now, since the series of general term $\| u_n \|$ is convergent by assumption, the sequence $(1 + \| u_n \|)$ is multipliable in $\mathbf{R}_+^*$ ($IV$, p. 35, th. 4); for every $\varepsilon > 0$, there therefore exists a finite subset $J_0$ of $N$ such that, for every finite subset $L$ of $N$ not meeting $J_0$, we have $\left| \prod_{n \in L} (1 + \| u_n \|) - 1 \right| \leq \varepsilon$; whence the theorem.

#### Corollary {#top-ix-a2-n2-cor-1 .statement}

*If the series of general term* $u_n$ *is absolutely convergent, and if none of the elements* $e + u_n$ *is a divisor of 0 in* $A$, *the product* $\prod_{n \in \mathbf{N}} (e + u_n)$ *is not a divisor of 0 in* $A$.

Indeed, there are only a finite number of integers $n$ such that $\|u_n\| > 1$. Let $J = \{0, m\}$ be an interval of $\mathbf{N}$ containing all these integers. The product of the sequence $(\mathbf{e} + u_n)$ is the product of $p_J$ and of the element $\prod_{n > m} (\mathbf{e} + u_n)$, all of whose factors are invertible (IX, p. 39, corollary), and which is consequently itself invertible; since $p_J$ is the product of a finite number of elements which are not divisors of 0, it is not a divisor of 0, and the same is true of $\prod_{n \in \mathbf{N}} (\mathbf{e} + u_n)$.

The *sufficient* condition for multipliability given in th. 2 is not necessary in general (cf. IX, p. 126, exerc. 6). It is, however, necessary in the important case where $A$ is an algebra of *finite* rank over the field $\mathbf{R}$ (in particular when $A$ is the field of quaternions $\mathbf{K}$, or a matrix algebra $\mathbf{M}_n(\mathbf{R})$):

#### Proposition 1 {#top-ix-a2-prop-1 .statement}

*Let $A$ be a normed algebra of finite rank over $\mathbf{R}$. If $(\mathbf{e} + u_n)$ is a multipliable sequence in $A$, whose product is invertible, the series of general term $u_n$ is absolutely convergent.*

It is known (VII, p. 16, prop. 2) that there exists a number $c > 0$ such that, for every finite family $(\mathbf{x}_i)_{i \in I}$ of points of $A$, one has

(1)
$$
\sum_{i \in I} \|\mathbf{x}_i\| \leq c \cdot \sup_{J \subset I} \left\| \sum_{i \in J} \mathbf{x}_i \right\|.
$$

Let $(a_n)_{n \in \mathbf{N}}$ be any sequence of elements of $A$. For every finite subset $I$ of $\mathbf{N}$, put
$$
p_I = \prod_{i \in I} (\mathbf{e} + a_i) \qquad s_I = \sum_{i \in I} a_i, \qquad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### Lemma 1 {#top-ix-a2-lem-1 .statement}

*For every finite subset $I$ of $\mathbf{N}$, let $\varphi(I) = \sup_{J \subset I} \|p_J - \mathbf{e}\|.$ For every subset $J$ of $I$, one has*
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_J.
$$
The lemma is evident if $J$ is empty; let us prove it by induction on the number of elements of $J$. Let $J = K \cup \{j\}$, where $j$ is strictly upper to all the elements of $K$; then $p_J = p_K(\mathbf{e} + a_j)$ and $s_J = s_K + a_j$, whence
$$
p_J - \mathbf{e} - s_J = (p_K - \mathbf{e} - s_K) + (p_K - \mathbf{e}) a_j
$$
and, by virtue of the induction hypothesis and the definition of $\varphi(I)$
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_K + \varphi(I) \|a_j\| = \varphi(I) \sigma_J
$$
which proves the lemma.

#### Lemma 2 {#top-ix-a2-lem-2 .statement}

*If $I$ is a finite subset of $\mathbf{N}$ such that $\varphi(I) < 1/c$, one has $\sigma_I \leq \frac{c \varphi(I)}{1 - c \varphi(I)}$*.

Indeed, since $\sigma_J \leq \sigma_I$ for every subset $J$ of $I$, one has, after (2),
$$
\|s_J\| \leq \varphi(I) \sigma_I + \|p_J - \mathbf{e}\| \leq (1 + \sigma_I) \varphi(I);
$$

since, by virtue of (1), one has $\sigma_I \leq c \cdot \sup_{J \subset I} \| s_J \|$, it follows that $\sigma_I \leq c \varphi(I)(1 + \sigma_I)$, whence the lemma.

That being so, let $(e + u_n)$ be a multipliable sequence in $A$, whose product is invertible; according to th. 1 (IX, p. 79), there exists a finite subset $J_0$ of $\mathbf{N}$ such that, for every finite subset $H$ of $\mathbf{N}$ not meeting $J_0$, one has
$$
\left\| \prod_{i \in H} (e + u_i) - e \right\| \leq 1/2c.
$$
By Lemma 2, one deduces $\sum_{i \in H} \| u_i \| \leq 1$ for every finite subset $H$ of $\mathbf{N}$ not meeting $J_0$, which implies that the family $(\| u_n \|)$ is summable in $\mathbf{R}$ (IV, p. 32, th. 1).

### 3. Infinite products

To every sequence $(x_n)$ of points of a normed algebra $A$, let us make correspond the sequence of the *partial products* $p_n = \prod_{k=0}^n x_k$; one calls *infinite product* of general factor $x_n$, the *couple* of the sequences $(x_n)$ and $(p_n)$. The infinite product of general factor $x_n$ is said to be *convergent* if the sequence $(p_n)$ is convergent in $A$; the limit of this sequence is then called the *product* of the sequence $(x_n)$, and is denoted $\prod_{n=0}^\infty x_n$.

#### Proposition 2 {#top-ix-a2-prop-2 .statement}

*Let $(x_n)$ be a sequence of points of a complete normed algebra $A$.*

a) *If the infinite product of general factor* $x_n$ *is convergent and if* $\prod_{n=0}^\infty x_n$ *is invertible, for every* $\varepsilon > 0$, *there exists* $n_0$ *such that, for* $n_0 \leq m \leq n$, *one has* $\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon$.

b) *Conversely, if the sequence* $(x_n)$ *satisfies this condition, the infinite product of general factor* $x_n$ *is convergent; moreover, if each of the* $x_n$ *is invertible,* $\prod_{n=0}^\infty x_n$ *is invertible.*

We leave to the reader the development of the proof of this proposition, which is copied step by step from that of th. 1 of IX, p. 79 (the finite parts $L$ of $\mathbf{N}$ which occur in the latter having simply to be replaced by intervals).

#### Corollary 1 {#top-ix-a2-prop-2-cor-1 .statement}

*If the infinite product of general factor* $x_n$ *is convergent, and if* $\prod_{n=0}^\infty x_n$ *is invertible,* $\lim_{n \to \infty} x_n = e$.

#### Corollary 2 {#top-ix-a2-prop-2-cor-2 .statement}

*If the infinite product of general factor* $x_n$ *is convergent, and if* $\prod_{n=0}^\infty x_n$ *is invertible, the infinite product of general factor* $y_n = x_{n+h} (n \geq 0)$ *is convergent.*

The product of the sequence $(y_n)$ is denoted by $\prod_{n=h}^\infty x_n$, and is also called the *remainder of index h* of the infinite product of general factor $x_n$.

Assuming still that $\prod_{n=0}^{\infty} x_n$ is invertible, we deduce also from prop. 2 (IX, p. 82) that, if $(z_n)$ is a sequence such that $z_n = x_n$ except for a finite number of indices, the product of general factor $z_n$ is convergent.

#### Proposition 3 {#top-ix-a2-prop-3 .statement}

*Let* $(k_n)$ *be a strictly increasing sequence of integers* $\geqslant 0$ ($k_0 = 0$) : *if the infinite product of general factor* $x_n$ *converges, and if one sets* $u_n = \prod_{p=k_n}^{k_{n+1}-1} x_n$, *the infinite product of general factor* $u_n$ *is convergent, and one has* $\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n$.

Indeed, the sequence of partial products of the sequence $(u_n)$ is extracted from the sequence of partial products of the sequence $(x_n)$.

Finally, by the same reasoning as for commutative groups (III, p. 44), one sees that if, in a normed algebra $A$, a sequence $(x_n)$ is *multipliable*, the product of general factor $x_n$ is convergent, and one has $\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n$ (which is also written $\prod_{n=0}^{\infty} x_n$); the converse is of course false (cf. IX, p. 126, exerc. 7).

Exercises

## EXERCISES {#top-ix-a2-exercises}

See the [exercises for Appendix 2](exercises/a2/).
