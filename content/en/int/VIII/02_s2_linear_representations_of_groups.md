---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 2
section_title: Linear representations of groups
lang: en
source: int-vii-ix
book_pages: INT VIII.8-INT VIII.17
pdf_pages: 0108-0117, 0159-0161
extraction: ocr
subsections:
    - "no": 1
      title: Continuous linear representations
      page: 8
      pdf_page: 108
    - "no": 2
      title: Contragredient representation
      page: 10
      pdf_page: 110
    - "no": 3
      title: 'Example: linear representations in spaces of continuous functions'
      page: 11
      pdf_page: 111
    - "no": 4
      title: 'Example: linear representations in spaces of measures'
      page: 12
      pdf_page: 112
    - "no": 5
      title: 'Example: linear representations in the spaces $L^p$'
      page: 13
      pdf_page: 113
    - "no": 6
      title: Extension of a linear representation of $G$ to the measures on $G$
      page: 15
      pdf_page: 115
    - "no": 7
      title: Relations between the endomorphisms $U(\mu)$ and the endomorphisms $U(s)$
      page: 16
      pdf_page: 116
statements: 22
exercises: 10
content_sha256: dcacb32e43faf87afa9b413eaa1d8bbbe9c968d661d131b722608dd9e997415d
---

## § 2. LINEAR REPRESENTATIONS OF GROUPS

### 1. Continuous linear representations

Let G be a topological group, E a locally convex space, U a linear representation of G in E.

#### Definition 1 {#int-viii-s2-def-1 .statement}

— (i) $U$ is said to be separately continuous if, for every $s \in G$, $U(s)$ is a continuous endomorphism of $E$, and if, for every $x \in E$, the mapping $s \mapsto U(s)x$ of $G$ into $E$ is continuous.

(ii) $U$ is said to be continuous if $(s, x) \mapsto U(s)x$ is a continuous mapping of $G \times E$ into $E$.

(iii) $U$ is said to be equicontinuous if it is continuous and if the set of endomorphisms $U(s)$, where $s$ runs over $G$, is equicontinuous.

#### Remark 1 {#int-viii-s2-n1-rem-1 .statement}

To say that $U$ is separately continuous means that $s \mapsto U(s)$ is a continuous mapping of $G$ into the space $\mathcal{L}(E; E)$ of continuous endomorphisms of $E$, equipped with the topology of pointwise convergence.

#### Remark 2 {#int-viii-s2-n1-rem-2 .statement}

To say that $U$ is continuous is equivalent to the following set of three conditions:

a) for every $s \in G$, $U(s)$ is continuous; b) there exists a neighborhood $V$ of $e$ such that $U(V)$ is equicontinuous; c) there exists a total set $D$ in $E$ such that, for every $x \in D$, the mapping $s \mapsto U(s)x$ is continuous.

These conditions are obviously necessary. Conversely, suppose that the conditions $a)$, $b)$, $c)$ are satisfied. On $U(V)$, the topology of pointwise convergence is identical to the topology of pointwise convergence in $D$ (TVS, III, §3, No. 4, Prop. 5). Therefore the mapping $(s, x) \mapsto U(s)x$ of $V \times E$ into $E$ is continuous (GT, X, §2, No. 1, Cor. 3 of Prop. 1). Since $U(s_0s)x = U(s_0)(U(s)x)$ for all $s_0 \in G$, $s \in G$, $x \in E$, one sees that $U$ is continuous.

When $G$ is locally compact, the conditions $a)$ and $b)$ are equivalent to the condition:
$a')$ for every compact subset $K$ of $G$, $U(K)$ is equicontinuous.

#### Remark 3 {#int-viii-s2-n1-rem-3 .statement}

Suppose that $U$ is a continuous linear representation of $G$ in $E$. For every $s \in G$, let $\widehat{U}(s)$ be the continuous extension of $U(s)$ to the completion $\widehat{E}$ of $E$. Then $\widehat{U}$ is a linear representation of $G$ in $\widehat{E}$, satisfying conditions $a)$ and $c)$ of Remark 2, and also condition $b)$ by GT, X, §2, No. 2, Prop. 4. Therefore $\widehat{U}$ is a continuous linear representation of $G$ in $\widehat{E}$.

#### Remark 4 {#int-viii-s2-n1-rem-4 .statement}

When $E$ is a normed space, $U$ is said to be isometric if $\|U(s)\| = 1$ for every $s \in G$. For this, it suffices that $\|U(s)\| \leq 1$ for all $s \in G$, because one then has
$$
1 = \|1\| \leq \|U(s)\| \cdot \|U(s^{-1})\|,
$$
whence $\|U(s)\| = \|U(s^{-1})\| = 1$ for all $s \in G$.

#### Proposition 1 {#int-viii-s2-prop-1 .statement}

— If $G$ is a locally compact group and $E$ is barreled, then every separately continuous linear representation $U$ of $G$ in $E$ is continuous.

For every compact subset $K$ of $G$, $U(K)$ is compact for the topology of pointwise convergence (Remark 1), therefore is equicontinuous (TVS, III, §4, No. 2, Th. 1); one then applies Remark 2.

#### Lemma 1 {#int-viii-s2-lem-1 .statement}

Let G be a locally compact group, $\rho$ a lower semi-continuous finite numerical function $\geqslant 0$ on G such that $\rho(st) \leqslant \rho(s)\rho(t)$ for all $s,t \in G$. Then $\rho$ is bounded above on every compact subset of G.

There exists a nonempty open subset U of G such that $\rho$ is bounded above on U (GT, IX, §5, No. 4, Th. 2). Let K be a compact subset of G. Then K is covered by a finite number of sets $s_1U, \ldots, s_nU$. For every $x \in U$, one has $\rho(s_ix) \leqslant \rho(s_i)\rho(x)$, therefore $\rho$ is bounded above on the $s_iU$, hence on K.

#### Lemma 2 {#int-viii-s2-lem-2 .statement}

Let G be a topological group, U a linear representation of G in a normed space E, and A a dense subset of E. Assume that for every $s \in G$, $U(s)$ is continuous, and that, for every $x \in A$, $s \mapsto U(s)x$ is a continuous mapping of G into E. Then the function $s \mapsto g(s) = \|U(s)\|$ on G is lower semi-continuous and satisfies $g(st) \leqslant g(s)g(t)$.

Let B be the unit ball of E. Then $g(s) = \sup_{x \in B \cap A} \|U(s)x\|$, and each function $s \mapsto \|U(s)x\|$ is continuous on G, therefore $g$ is lower semi-continuous. On the other hand,

$$
g(st) = \|U(s)U(t)\| \leqslant \|U(s)\| \cdot \|U(t)\| = g(s)g(t).
$$

#### Proposition 2 {#int-viii-s2-prop-2 .statement}

Let G be a locally compact group, U a linear representation of G in a normed space E. Let A be a dense subset of E. Assume that for every $s \in G$, $U(s)$ is continuous and that, for every $x \in A$, $s \mapsto U(s)x$ is a continuous mapping of G into E. Then U is continuous.

For, $\|U(s)\|$ is bounded on every compact subset of G by Lemmas 1 and 2, and one then applies Remark 2.

### 2. Contragredient representation

Let U be a separately continuous linear representation of G in E. Let E' be the dual of E. The mapping $s \mapsto {}^tU(s)$ is a linear representation in E' of the group $G^0$ opposite G; we shall say that this representation is the transpose of U. The mapping $s \mapsto {}^tU(s^{-1}) = {}^tU(s)^{-1}$ is a linear representation of G in E', called the contragredient of U.

#### Lemma 3 {#int-viii-s2-lem-3 .statement}

Let X be a locally compact space, Y and Z topological spaces, $\varphi$ a continuous mapping of $X \times Y$ into Z, and $\varphi_x$ the mapping $y \mapsto \varphi(x,y)$ of Y into Z. The spaces $\mathcal{C}(Y), \mathcal{C}(Z)$ being equipped with the topology of compact convergence, the mapping $(x,f) \mapsto f \circ \varphi_x$ of $X \times \mathcal{C}(Z)$ into $\mathcal{C}(Y)$ is continuous.

It clearly suffices to consider the case that X is compact. Let $(x_0, f_0) \in X \times \mathcal{C}(Z)$, K a compact subset of Y, and $\varepsilon > 0$. Let $K' = \varphi(X \times K)$. Since f_0 \circ \varphi \text{ is uniformly continuous in } X \times K, \text{ there exists a neighborhood W of } x_0 \text{ such that } |f_0(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq \varepsilon \text{ for } x \in W \text{ and } y \in K. \text{ On the other hand, if one takes } f \in \mathcal{C}(Z) \text{ to be such that } |f(z) - f_0(z)| \leq \varepsilon \text{ for all } z \in K', \text{ one will have } |f(\varphi(x,y)) - f_0(\varphi(x,y))| \leq \varepsilon \text{ for } x \in X, y \in K, \text{ and therefore } |f(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq 2\varepsilon \text{ for } x \in W, y \in K. \text{ Whence the lemma.}

Let us now return to the earlier notations.

#### Proposition 3 {#int-viii-s2-prop-3 .statement}

(i) *If U is separately continuous, then $^tU$ is separately continuous when E' is equipped with the weak topology $\sigma(E', E)$.*
(ii) *If G is locally compact and U is continuous, then $^tU$ is continuous when E' is equipped with the topology of compact convergence.*

The assertion (i) is immediate. The assertion (ii) follows from Lemma 3 where one has taken $X = G, Y = Z = E, \varphi(s, x) = U(s)x$.

### 3. Example: linear representations in spaces of continuous functions

Let G be a discrete group operating on the left on a set X. A complex function $\chi$ on $G \times X$ is called a *multiplier* if

(1) $\chi(e, x) = 1$ for all $x \in X;$
(2) $\chi(st, x) = \chi(s, tx)\chi(t, x)$ for all $s, t$ in G, $x \in X$.

It follows that

(3) $\chi(t^{-1}, tx)\chi(t, x) = 1$ for all $t \in G, x \in X,$

and in particular $\chi(t, x) \neq 0$ for all $t \in G, x \in X$.

For every complex function $f$ defined on X and every $s \in G$, let $\gamma_\chi(s)f$ be the complex function on X defined by

(4) $(\gamma_\chi(s)f)(x) = \chi(s^{-1}, x)f(s^{-1}x)$.

Then $\gamma_\chi(e)f = f$ and

$$
\begin{align*}
(\gamma_\chi(s)\gamma_\chi(s')f)(x) &= \chi(s^{-1}, x)(\gamma_\chi(s')f)(s^{-1}x) \\
&= \chi(s^{-1}, x)\chi(s'^{-1}, s^{-1}x)f(s'^{-1}s^{-1}x) \\
&= \chi((ss')^{-1}, x))f((ss')^{-1}x) = (\gamma_\chi(ss')f)(x),
\end{align*}
$$

thus $\gamma_\chi$ *is a linear representation* of G. For $\chi = 1$, one recovers the endomorphisms $\gamma(s)$ (Ch. VII, §1, No. 1, formula (3)).

Suppose now that G and X are locally compact, G operating continuously on X, and $\chi$ continuous on $G \times X$. Then $C(X)$ and $K(X)$ are stable for the $\gamma_\chi(s)$, whence linear representations of G in $C(X)$ and $K(X)$ which we shall again denote $\gamma_\chi$.

#### Proposition 4 {#int-viii-s2-prop-4 .statement}

*The linear representations $\gamma_\chi$ of G in $C(X)$ and $K(X)$ are continuous.*

The mapping $(s, f) \mapsto (s, \gamma(s)f)$ of $G \times C(X)$ into $G \times C(X)$ is continuous (No. 2, Lemma 3). On the other hand, the mapping $(s, f) \mapsto \chi(s, \cdot)f$ of $G \times C(X)$ into $C(X)$ is continuous; for, if s tends to $s_0$ in G, then $\chi(s, \cdot)$ tends to $\chi(s_0, \cdot)$ uniformly on every compact subset of X; if, moreover, $f$ tends to $f_0$ in $C(X)$, then $\chi(s, \cdot)f$ tends to $\chi(s_0, \cdot)f_0$ uniformly on every compact subset of X, whence our assertion. Thus the representation $\gamma_\chi$ of G in $C(X)$ is continuous.

Let us show that the representation $\gamma_\chi$ of G in $K(X)$ is continuous. Since $K(X)$ is the direct limit of Banach spaces, it is barreled (TVS, III, §4, No. 1, Cor. 3 of Prop. 3), thus it suffices to prove that $\gamma_\chi$ is separately continuous (No. 1, Prop. 1). Now, let H be a compact subset of X and let $s_0 \in G$. Let V be a compact neighborhood of $s_0$ in G, and let L = VH, which is compact in X. For every $f \in K(X, H)$, the support of $\gamma_\chi(s_0)f$ is contained in L, and
$$
\sup_{x \in X} |(\gamma_\chi(s_0)f)(x)| \leq \sup_{x \in L} |\chi(s_0^{-1}, x)| \cdot \sup_{x \in X} |f(x)|,
$$
therefore $f \mapsto \gamma_\chi(s_0)f$ is a continuous linear mapping of $K(X, H)$ into $K(X, L)$; it follows that $f \mapsto \gamma_\chi(s_0)f$ is a continuous linear mapping of $K(X)$ into itself (TVS, II, §4, No. 4, Prop. 5). On the other hand, the topology of $K(X, L)$ is induced by that of $C(X)$. By what has already been proved, the mapping $s \mapsto \gamma_\chi(s)f$ of V into $K(X, L)$ is continuous. This completes the proof that $\gamma_\chi$ is separately continuous.

#### Proposition 5 {#int-viii-s2-prop-5 .statement}

*Suppose that each function $\chi(s, \cdot)$ is bounded. Then $\gamma_\chi$ leaves $\overline{K(X)}$ stable, and the linear representation $\gamma_\chi$ of G in $\overline{K(X)}$ is continuous.*

It is clear that $\gamma_\chi$ leaves $\overline{K(X)}$ stable and that each of the $\gamma_\chi(s)$ is continuous in $\overline{K(X)}$. On the other hand, for every $f \in K(X)$, $s \mapsto \gamma_\chi(s)f$ is a continuous mapping of G into $K(X)$ and *a fortiori* into $\overline{K(X)}$. Therefore the representation $\gamma_\chi$ in $\overline{K(X)}$ is continuous (No. 1, Prop. 2).

### 4. Example: linear representations in spaces of measures

Again let G be a locally compact group, operating continuously on the left in a locally compact space X, and let $\chi$ be a *continuous* multiplier on $G \times X$. The linear representation $\gamma_\chi$ of $G$ in $\mathcal{K}(X)$ admits a contragredient representation in $\mathcal{M}(X)$, which we shall again denote by $\gamma_\chi$, and which is defined by the following formula (where $\mu \in \mathcal{M}(X) , f \in \mathcal{K}(X)$):

$$
\langle \gamma_\chi(s)\mu, f \rangle = \langle \mu, \gamma_\chi(s^{-1})f \rangle = \langle \chi(s, \cdot) \cdot \mu, \gamma(s^{-1})f \rangle = \langle \gamma(s)(\chi(s, \cdot) \cdot \mu), f \rangle ,
$$

whence

$$
\gamma_\chi(s)\mu = \gamma(s)(\chi(s, \cdot) \cdot \mu) = (\gamma(s)\chi(s, \cdot)) \cdot (\gamma(s)\mu) .
$$

We note that

$$
(\gamma(s)\chi(s, \cdot))(x) = \chi(s, s^{-1}x) .
$$

The linear representation $\gamma_\chi$ of $G$ in $\mathcal{C}(X)$ admits a contragredient representation in the space $\mathcal{C}'(X)$ of measures on $X$ with compact support, a representation which we again denote by $\gamma_\chi$; the endomorphisms $\gamma_\chi(s)$ of $\mathcal{C}'(X)$ are the restrictions of the endomorphisms $\gamma_\chi(s)$ of $\mathcal{M}(X)$.

#### Proposition 6 {#int-viii-s2-prop-6 .statement}

*If one equips $\mathcal{M}(X)$ (resp. $\mathcal{C}'(X)$) with the topology of uniform convergence in the compact subsets of $\mathcal{K}(X)$ (resp. $\mathcal{C}(X)$), then the linear representation $\gamma_\chi$ of $G$ in $\mathcal{M}(X)$ (resp. $\mathcal{C}'(X)$) is continuous.*

#### Proposition 7 {#int-viii-s2-prop-7 .statement}

*Suppose that each function $\chi(s, \cdot)$ is bounded. Then $\gamma_\chi$ leaves stable $\mathcal{M}^1(X)$ and, if $\mathcal{M}^1(X)$ is equipped with the topology of uniform convergence in the compact subsets of $\mathcal{K}(X)$, then the linear representation $\gamma_\chi$ of $G$ in $\mathcal{M}^1(X)$ is continuous.*
These propositions result from Props. 3, 4, 5.

### 5. Example: linear representations in the spaces $L^p$

Again let $G$ be a locally compact group, operating continuously on the left in a locally compact space $X$. Let $\beta$ be a positive measure on $X$ with support $X$. Let us assume that there exists a *continuous* function $\chi > 0$ on $G \times X$ such that, for every $s \in G$,

$$
\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta
$$

(which implies in particular that $\beta$ is quasi-invariant under $G$). *Then, $\chi$ is a multiplier.* For, given $s, t$ in $G$, one has

$$
\gamma(s)\gamma(t)\beta = \gamma(s)(\chi(t^{-1}, \cdot) \cdot \beta) = (\gamma(s)\chi(t^{-1}, \cdot)) \cdot (\gamma(s)\beta)
= (\gamma(s)\chi(t^{-1}, \cdot)) \cdot \chi(s^{-1}, \cdot) \cdot \beta ,
$$
$$
\gamma(st)\beta = \chi(t^{-1}s^{-1}, \cdot) \cdot \beta ,
$$

therefore
$$
\chi(t^{-1}, s^{-1}x)\chi(s^{-1}, x) = \chi(t^{-1}s^{-1}, x)
$$
locally $\beta$-almost everywhere, consequently everywhere, since $\chi$ is continuous and $\beta$ has support $X$.

Let $p \in [1, +\infty[$. For every $f \in \mathcal{L}_C^p(X, \beta)$ and every $s \in G$, let $\gamma_{\chi,p}(s)f$ be the function on $X$ defined by
$$
(\gamma_{\chi,p}(s)f)(x) = \chi(s^{-1}, x)^{1/p} f(s^{-1}x).
$$
One has
$$
\int^* |\chi(s^{-1}, x)^{1/p} f(s^{-1}x)|^p d\beta(x) = \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \int |f(x)|^p d\beta(x),
$$
therefore $\gamma_{\chi,p}(s)f \in \mathcal{L}_C^p(X, \beta)$. One sees that $\gamma_{\chi,p}(s)$ is an *isometric* endomorphism of $\mathcal{L}_C^p(X, \beta)$ and defines, by passage to the quotient, an isometric endomorphism of $L_C^p(X, \beta)$, also denoted $\gamma_{\chi,p}(s)$. On the other hand, $\chi^{1/p}$ is obviously a multiplier, therefore $\gamma_{\chi,p}$ is a linear representation of $G$ in $L_C^p(X, \beta)$ by what we have seen in No. 3.

#### Proposition 8 {#int-viii-s2-prop-8 .statement}

*The linear representation $\gamma_{\chi,p}$ of $G$ in $L_C^p(X, \beta)$ is continuous and isometric.*

Let $f \in \mathcal{K}(X)$. When $s$ tends to $s_0$ in $G$, $\gamma_{\chi,p}(s)f$ tends to $\gamma_{\chi,p}(s_0)f$ in $\mathcal{K}(X)$, hence in $L_C^p(X, \beta)$. Since the $\gamma_{\chi,p}(s)$ are isometric, Prop. 8 is obtained by applying *Remark 2* of No. 1.

For the case that $\chi$ is not assumed continuous, cf. §4, Exer. 13.

#### Proposition 9 {#int-viii-s2-prop-9 .statement}

*Suppose that each function $\chi(s, \cdot)$ is bounded. Then $\gamma_\chi$ leaves $L_C^p(X, \beta)$ stable, and the linear representation $\gamma_\chi$ of $G$ in $L_C^p(X, \beta)$ is continuous.*

Let $f \in \mathcal{L}_C^p(X, \beta)$. Then
$$
\int^* |\chi(s^{-1}, x)f(s^{-1}x)|^p d\beta(x)
$$
$$
\leq \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int |f(x)|^p d\beta(x),
$$
therefore $\gamma_\chi(s)f \in \mathcal{L}_C^p(X, \beta)$, and
$$
\| \gamma_\chi(s) \| \leq \sup_{x \in X} \chi(s^{-1}, x)^{1/q},
$$
(5) where $q$ denotes the exponent conjugate to $p$. If $f \in \mathcal{K}(X)$, then $\gamma_{\chi}(s)f$ tends to $\gamma_{\chi}(s_0)f$ in $\mathcal{K}(X)$, hence in $\mathcal{L}_C^p(X, \beta)$, as $s$ tends to $s_0$. Therefore the representation $\gamma_{\chi}$ of $G$ in $L_C^p(X, \beta)$ is continuous (No. 1, Prop. 2).

Properties analogous to those of Nos. 3, 4, 5 hold if $G$ operates on the right in $X$.

In particular, if one regards $G$ as operating on itself by left or right translations, and if one takes $\chi = 1$, one obtains the *left* and *right regular representations* of $G$ in $\mathcal{C}(G)$, $\mathcal{K}(G)$, $\overline{\mathcal{K}}(G)$, $\mathcal{C}'(G)$, $\mathcal{M}(G)$, $\mathcal{M}^1(G)$. If one takes $\beta$ to be a left (resp. right) Haar measure on $G$, and if one takes $\chi = 1$, one obtains the *left* (resp. *right*) *regular representation* of $G$ in $L_C^p(G, \beta)$.

### 6. Extension of a linear representation of $G$ to the measures on $G$

Let $G$ be a locally compact group, $E$ a locally convex space, $U$ a linear representation of $G$ in $E$. Assume $U$ to be continuous and $E$ quasi-complete. Then, for every measure $\mu \in \mathcal{C}'(G)$, one has

$$
\int_G U(s)\, d\mu(s) \in \mathcal{L}(E; E)
$$

(Ch. VI, §1, No. 7). We shall write $U(\mu) = \int_G U(s)\, d\mu(s)$. We equip $\mathcal{C}'(G)$ with the topology of compact convergence in $\mathcal{C}(G)$. The mapping $(\mu, x) \mapsto U(\mu)x$ of $\mathcal{C}'(G) \times E$ into $E$ is *hypocontinuous* relative to the equicontinuous subsets of $\mathcal{C}'(G)$ and the compact subsets of $E$; in particular, the mapping $\mu \mapsto U(\mu)$ of $\mathcal{C}'(G)$ into $\mathcal{L}(E; E)$ (equipped with the topology of compact convergence) is continuous (*loc. cit.*, Prop. 16).

In order to be able to apply these results later on, we note that if $X$ is a locally compact space then $\mathcal{C}(X)$, equipped with the topology of compact convergence, is complete (GT, X, §1, No. 6, Cor. 3 of Th. 2). On the other hand, $\mathcal{K}(X)$ is barreled, therefore its dual $\mathcal{M}(X)$, equipped with the topology of compact convergence in $\mathcal{K}(X)$, is quasi-complete (TVS, III, §4, No. 2, Cor. 4 of Th. 1). Of course, $\mathcal{K}(X)$ is complete for the topology deduced from its norm, therefore its *dual* $\mathcal{M}^1(X)$ is quasi-complete for the topology of compact convergence in $\mathcal{K}(X)$ (*loc. cit.*).

Let us now assume that $U$ is a continuous linear representation of the locally compact group $G$ on a *Banach space* $E$. Set $g(s) = \|U(s)\|$ for all $s \in G$. Then, if $\mu$ is a measure on $G$ such that $g$ is $\mu$-integrable, one has $\int_G U(s)\, d\mu(s) \in \mathcal{L}(E; E)$ and $\|\int_G U(s)\, d\mu(s)\| \leq \int g(s)\, d|\mu|(s)$ (Ch. VI, §1, No. 7, *Remark* 1). We again write $U(\mu) = \int_G U(s)\, d\mu(s)$.

### 7. Relations between the endomorphisms $U(\mu)$ and the endomorphisms $U(s)$

#### Lemma 4 {#int-viii-s2-lem-4 .statement}

Let $T$ be a locally compact space, $a$ a point of $T$, $M$ a subset of $\mathcal{M}(T)$, and $\mathfrak{F}$ a filter on $M$. Assume that:
(i) for every compact subset $K$ of $T$, the numbers $|\mu|(K)$, for $\mu \in M$, are bounded above;
(ii) $\lim_{\mu,\mathfrak{F}} |\mu|(K) = 0$ for every compact subset $K$ of $T - \{a\}$.
(iii) there exists a compact neighborhood $V$ of $a$ in $T$ such that $\lim_{\mu,\mathfrak{F}} \mu(V) = 1$.

Then the filter $\mathfrak{F}$ converges to $\varepsilon_a$ in $\mathcal{M}(T)$ equipped with the topology of compact convergence in $\mathcal{H}(T)$.

By the hypothesis (i), $M$ is an equicontinuous subset of $\mathcal{M}(T)$ since it is vaguely bounded and $\mathcal{H}(T)$ is barreled (TVS, III, §4, No. 2, Th. 1). It therefore suffices (GT, X, §2, No. 4, Th. 1) to prove that if $f \in \mathcal{H}(T)$, then $\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$. Let $K$ be the union of $V$ and the support of $f$; if $K'$ is the closure of $K - V$, one has

$$
|\mu(K) - \mu(V)| = |\mu(K - V)| \leq |\mu|(K');
$$

since $K'$ is compact and does not contain $a$, one concludes from this that $\lim_{\mu,\mathfrak{F}} \mu(K) = 1$. Let $\varepsilon > 0$, and let $W$ be an open neighborhood of $a$ in $K$ such that $|f(t) - f(a)| \leq \varepsilon$ for $t \in W$; one can write

$$
\mu(f) - f(a) = f(a)(\mu(K) - 1) + \int_K (f(t) - f(a)) d\mu(t);
$$

the integral over $K$ may be written as the sum of the analogous integrals over $W$ and $K - W$; if $C = \sup |f|$, one therefore has

$$
|\mu(f) - f(a)| \leq C|\mu(K) - 1| + \varepsilon \cdot |\mu|(K) + 2C \cdot |\mu|(K - W).
$$

Since the first and third terms on the right side tend to 0 with respect to $\mathfrak{F}$, one sees that indeed $\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$.

#### Corollary 1 {#int-viii-s2-lem-4-cor-1 .statement}

With hypotheses as in Lemma 4, suppose in addition that there exists a compact subset $K_0$ of $T$ containing the supports of all of the measures $\mu \in M$. Then $\mathfrak{F}$ also converges to $\varepsilon_a$ in $\mathcal{C}'(T)$ equipped with the topology of compact convergence in $\mathcal{C}(T)$.

For, the restriction mapping of $\mathcal{C}(T)$ into $\mathcal{C}(K_0)$ is continuous; therefore, if $H$ is a compact subset of $\mathcal{C}(T)$, then the restrictions to $K_0$ of the functions in $H$ form a compact subset of $\mathcal{C}(K_0)$. It then suffices to apply Lemma 4 on replacing $T$ by $K_0$.

#### Corollary 2 {#int-viii-s2-lem-4-cor-2 .statement}

*With hypotheses as in Cor. 1, let $f$ be a continuous mapping of $T$ into a quasi-complete locally convex space $E$. Then*

$$
\lim_{\mu,\mathfrak{T}} \int f(t)\, d\mu(t) = f(a).
$$

This follows from Cor. 1, and Prop. 14 of Ch. VI, §1, No. 6.

#### Corollary 3 {#int-viii-s2-lem-4-cor-3 .statement}

*Let $G$ be a locally compact group, $E$ a quasi-complete locally convex space, and $U$ a continuous linear representation of $G$ in $E$. Let $\beta$ be a positive measure on $G$, $a$ an element of $G$, and $\mathcal{B}$ a base for the filter of neighborhoods of $a$, formed of compact neighborhoods. For every $V \in \mathcal{B}$, let $f_V$ be a continuous function $\geqslant 0$ on $G$, with support contained in $V$, and such that $\int f_V\, d\beta = 1$. Then, for every $x \in E$,

$$
U(a)x = \lim_V U(f_V \cdot \beta)x,
$$

*the limit being taken with respect to the section filter of $\mathcal{B}$.*

The mapping $s \mapsto U(s)x$ of $G$ into $E$ is continuous. By Cor. 2, $U(a)x = \lim_V \int (U(s)x) \cdot f_V(s)\, d\beta(s)$ with respect to the section filter of $\mathcal{B}$, that is, $U(a)x = \lim_V U(f_V \cdot \beta)x$.

#### Proposition 10 {#int-viii-s2-prop-10 .statement}

*Let $G$ be a locally compact group, $E$ a quasi-complete locally convex space, $U$ a continuous linear representation of $G$ in $E$, and $\beta$ a positive measure on $G$ with support $G$.

(i) The vectors $U(f \cdot \beta)x$, where $f$ runs over $\mathcal{K}(G)$ and $x$ runs over $E$, are dense in $E$.

(ii) *Let $F$ be a closed linear subspace of $E$. If $F$ is stable for $U$, then $U(\mu)(F) \subset F$ for every $\mu \in \mathcal{C}'(G)$. Conversely, if $U(f \cdot \beta) \subset F$ for every $f \in \mathcal{K}(G)$, then $F$ is stable for $U$.*

The first part of (ii) is immediate, since the restrictions of the $U(s)$ to $F$ ($s \in G$) define a continuous linear representation of $G$ in the quasi-complete locally convex space $F$. The second part of (ii), and (i), follow from Cor. 3 of Lemma 4.

### Exercises {#int-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
