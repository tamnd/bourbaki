---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 1
section_title: Essential upper integral
lang: en
source: int-i-vi
book_pages: INT V.2-INT V.11
pdf_pages: 0257-0266, 0349-0350
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the essential upper integral
      page: 2
      pdf_page: 257
    - "no": 2
      title: Moderated functions and measures
      page: 4
      pdf_page: 259
    - "no": 3
      title: Essentially integrable functions
      page: 7
      pdf_page: 262
    - "no": 4
      title: A property special to the essential upper integral
      page: 10
      pdf_page: 265
statements: 22
exercises: 6
content_sha256: 9adb07a62fadd6e5f8620bda6421cb8411520345e999c2b98de2982037c52e39
---

## § 1. ESSENTIAL UPPER INTEGRAL

### 1. Definition of the essential upper integral

#### Definition 1 {#int-v-s1-def-1 .statement}

For every function $f \in \mathcal{F}_+(T)$ one calls essential upper integral of $f$ with respect to $\mu$, and denotes by $\mu^\bullet(f)$, the supremum, finite or not, of the set of numbers $\mu^*(f \varphi_K)$, where $K$ runs over the set of compact subsets of $T$. For every subset $A$ of $T$, one sets $\mu^\bullet(A) = \mu^\bullet(\varphi_A)$.

The notations $\int^\bullet f d\mu$, $\int^\bullet f(t) d\mu(t)$, $\int^\bullet f \mu$ are also used.
Since $f \varphi_K \leq f$ for every compact subset $K$ of $T$, one has

$$
\int^\bullet f d\mu \leq \int^* f d\mu .
$$

It can happen that $\mu^\bullet(f) \neq \mu^*(f)$; for, the condition $\mu^*(f) = 0$ means that $f$ is negligible, whereas the condition $\mu^\bullet(f) = 0$ means that $f$ is locally negligible (Ch. IV, §5, No. 2, Prop. 5), and there may exist locally negligible sets that are not negligible (Ch. IV, §1, Exer. 5).

The mapping $\mu^\bullet$ of $\mathcal{F}_+(T)$ into $\overline{\mathbf{R}}$ coincides with $\mu$ on $\mathcal{K}_+(T)$. It follows that two measures $\mu_1$ and $\mu_2$ such that $\mu_1^\bullet = \mu_2^\bullet$ are equal.

#### Proposition 1 {#int-v-s1-prop-1 .statement}

a) If $f$ and $g$ are two numerical functions $\geq 0$ that are equal locally almost everywhere, then $\mu^\bullet(f) = \mu^\bullet(g)$.
b) If $f$ and $g$ are two numerical functions $\geq 0$ such that $f \leq g$, then $\mu^\bullet(f) \leq \mu^\bullet(g)$.
c) If $f$ is a numerical function $\geq 0$, and $\alpha$ is a number $\geq 0$, then $\mu^\bullet(\alpha f) = \alpha \mu^\bullet(f)$.
d) If $f$ and $g$ are two numerical functions $\geq 0$, then $\mu^\bullet(f + g) \leq \mu^\bullet(f) + \mu^\bullet(g)$.
e) If $(f_n)_{n \in \mathbf{N}}$ is an increasing sequence of numerical functions $\geq 0$, and if $f = \lim_{n \to \infty} f_n$, then $\mu^\bullet(f) = \lim_{n \to \infty} \mu^\bullet(f_n)$.

The properties a), b), c), d) may be deduced immediately from the corresponding properties of the upper integral: a) from Proposition 6 of Ch. IV, §2, No. 3 and Proposition 5 of Ch. IV, §5, No. 2; b), c), d) from Propositions 10, 11, 12 of Ch. IV, §1, No. 3. To establish e), denote by $\mathfrak{K}$ the set of compact subsets of $T$; by Theorem 3 of Ch. IV, §1, No. 3, we have

$$
\lim_{n \to \infty} \mu^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{K \in \mathfrak{K}} \mu^*(f_n \varphi_K) = \sup_{K \in \mathfrak{K}} \sup_{n \in \mathbf{N}} \mu^*(f_n \varphi_K)
= \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K) = \mu^\bullet(f) .
$$

Equality holds in the relation d) if $f$ and $g$ are measurable, by Cor. 4 of Th. 5, Ch. IV, §5, No. 6. More generally, we have the following result:

#### Proposition 2 {#int-v-s1-prop-2 .statement}

*Let $f, g, h$ be three elements of $\mathcal{F}_+$; if $g$ and $h$ are measurable, then*

$$
\int^\bullet f(g + h)\, d\mu = \int^\bullet fg\, d\mu + \int^\bullet fh\, d\mu.
$$

One is immediately reduced to the proof of the analogous formula for the upper integral. Since $f(g + h) = fg + fh$ (with the convention that $0 \cdot (+\infty) = 0$), we have

$$
\int^* f(g + h)\, d\mu \leq \int^* fg\, d\mu + \int^* fh\, d\mu;
$$

it remains to establish the reverse inequality. Let $u$ be a lower semi-continuous function such that $u \geq f(g + h)$. Set $v = \frac{u}{g + h}$ on the set where $g + h > 0$, and $v = +\infty$ on the set where $g + h = 0$; then $v \geq f$ and $u \geq v(g + h)$, whence

$$
\int^* v(g + h)\, d\mu \leq \int^* u\, d\mu
$$

and consequently, $v$ being measurable (Ch. IV, §5, No. 6, Cor. 4 of Th. 5),

$$
\int^* fg\, d\mu + \int^* fh\, d\mu \leq \int^* vg\, d\mu + \int^* vh\, d\mu \\
= \int^* v(g + h)\, d\mu \leq \int^* u\, d\mu,
$$

which implies the desired inequality since $u$ is arbitrary.

#### Corollary {#int-v-s1-n1-cor-1 .statement}

*Let $f$ be a function $\geq 0$, $(g_n)$ a sequence of measurable functions $\geq 0$; then $\int^\bullet f \left( \sum_n g_n \right) d\mu = \sum_n \left( \int^\bullet f g_n\, d\mu \right)$.

For the case of a finite sequence, this is an immediate consequence of Prop. 2. The case of an infinite sequence may be deduced from this by means of Prop. 1, e).

#### Proposition 3 {#int-v-s1-prop-3 .statement}

*For every finite number $\alpha \geq 0$ and every pair of measures $\mu, \nu$ on $\mathbf{T}$,

$$
(\alpha \mu)^\bullet = \alpha \mu^\bullet \\
(\mu + \nu)^\bullet = \mu^\bullet + \nu^\bullet.
$$

Moreover, the relation $\mu \leq \nu$ implies $\mu^\bullet \leq \nu^\bullet$.*

The proof is immediate from the analogous statement in Ch. IV (§1, No. 3, Prop. 15).

#### Proposition 4 {#int-v-s1-prop-4 .statement}

— *For every numerical function* $f \geqslant 0$ *that is lower semi-continuous on* $T$, $\mu^\bullet(f) = \mu^*(f)$.

For, let $g$ be a function in $\mathcal{K}_+(T)$ such that $g \leqslant f$. If $K$ is the (compact) support of $g$, then $\mu(g) \leqslant \mu^*(f \varphi_K) \leqslant \mu^\bullet(f)$. It follows, by the definition of upper integral, that $\mu^*(f) \leqslant \mu^\bullet(f)$, therefore $\mu^*(f) = \mu^\bullet(f)$ (formula (1)).

### 2. Moderated functions and measures

#### Proposition 5 {#int-v-s1-prop-5 .statement}

— *Let* $A$ *be a subset of* $T$; *the following properties are equivalent*:
a) *The set* $A$ *is contained in the union of a sequence of* $\mu$*-integrable open sets*.
b) *The set* $A$ *is contained in the union of a sequence of* $\mu$*-integrable sets*.
c) *The set* $A$ *is contained in the union of a sequence of compact sets and a* $\mu$*-negligible set*.

It is clear that each of the properties a) and c) implies b). Conversely, b) implies a) because every set of finite outer measure is contained in an integrable open set (Ch. IV, §1, No. 4, Prop. 19), and b) implies c) because every integrable set is the union of a sequence of compact sets and a negligible set (Ch. IV, §4, No. 6, Cor. 2 of Th. 4).

#### Definition 2 {#int-v-s1-def-2 .statement}

— *A subset of* $T$ *is said to be* $\mu$*-moderated if it satisfies the equivalent conditions of Proposition 5*. *A function defined on* $T$, *with values in a vector space or in* $\overline{\mathbf{R}}$, *is said to be* $\mu$*-moderated if it is zero on the complement of a* $\mu$*-moderated subset of* $T$. *The measure* $\mu$ *is said to be moderated if* $T$ *is a* $\mu$*-moderated set*.

If $\mu$ is a moderated measure, then every function on $T$ is $\mu$-moderated and every subset of $T$ is $\mu$-moderated.

#### Remark {#int-v-s1-n2-rem-1 .statement}

— 1) If $\theta$ is a complex measure on $T$, one says that a function $f$ is $\theta$-moderated (resp. that $\theta$ is moderated) if $f$ is $|\theta|$-moderated (resp. if $|\theta|$ is moderated).
2) Every bounded measure is moderated; if $T$ is a countable union of compact sets, then every measure on $T$ is moderated.
3) Let $(f_n)$ be a sequence of $\mu$-moderated functions with values in $\overline{\mathbf{R}}$. For each $n$, let $U_n$ be an open set that is a countable union of open sets of finite outer measure, such that $f_n$ is zero outside $U_n$. The function $s = \sum_{n \in \mathbf{N}} |f_n|$ is then zero outside $\bigcup_{n \in \mathbf{N}} U_n$; it is therefore $\mu$-moderated, and the same is true of all functions $f$ such that $|f| \leq s$. This applies in particular to the functions $\liminf_{n \to \infty} f_n$, $\limsup_{n \to \infty} f_n$ and $\sum_{n \in \mathbf{N}} f_n$ (if the sum is defined).

4) A function equal almost everywhere to a moderated function is moderated.

#### Proposition 6 {#int-v-s1-prop-6 .statement}

— *Let $f$ be a positive numerical function defined on $T$ that is $\mu$-measurable and $\mu$-moderated. Then there exists a sequence $(h_n)_{n \in \mathbf{N}}$ of elements of $\mathcal{F}_+(T)$, with sum equal to $f$, having the following properties:*

1) *The function $h_0$ is $\mu$-negligible.*
2) *For every $n \geq 1$, there exists a compact set $K_n$ such that $h_n$ is zero outside $K_n$, and such that the restriction of $h_n$ to $K_n$ is finite and continuous.*

Suppose that $f$ is the sum of a sequence $(f_n)$ of positive measurable functions, each of which has the property in the statement; it is clear that $f$ also has it. Set
$$
f_n = \inf(f, n+1) - \inf(f, n)
$$
for every $n \in \mathbf{N}$; since $f$ is equal to the sum of the sequence $(f_n)$, it will thus suffice to establish the proposition assuming $f$ to be moderated and *bounded*. Denote then by $A$ the set of $t \in T$ such that $f(t) > 0$; $A$ is measurable and moderated, therefore there exists a sequence $(A_n)$ of pairwise disjoint integrable sets such that $A = \bigcup_n A_n$. We are reduced to proving the statement for the functions $f \varphi_{A_n}$; in other words, we may suppose $f$ to be bounded and to be zero outside an integrable set $I$. But $I$ is the union of a negligible set $N$ and a sequence $(L_n)$ of pairwise disjoint compact sets (Ch. IV, §4, No. 6, Cor. 2 of Th. 4). We are thus reduced to treating the case that $f$ is bounded and is zero outside a compact set $L$.

Let $\mathcal{K}$ be the set of compact subsets $K$ of $T$ such that $f|K$ is continuous; since $\mathcal{K}$ is $\mu$-dense (Ch. IV, §5, No. 10, Prop. 15), $L$ is the union of a negligible set $N$ and a sequence $(K_n)_{n \geq 1}$ of pairwise disjoint elements of $\mathcal{K}$ (Ch. IV, §5, No. 8, Def. 6). The functions $h_0 = f \varphi_N$, $h_n = f \varphi_{K_n}$ for $n \geq 1$ then satisfy the conditions of the statement.

The following proposition makes it possible to reduce the study of the upper integral to that of the essential upper integral.

#### Proposition 7 {#int-v-s1-prop-7 .statement}

— *Let $f$ be an element of $\mathcal{F}_+(T)$.*
1) *If the function $f$ is not $\mu$-moderated, then $\mu^*(f) = +\infty$.*
2) *If the function $f$ is $\mu$-moderated, then $\mu^*(f) = \mu^*(f)$.*
3) *If $\mu^*(f) < +\infty$ then there exists a $\mu$-moderated subset $A$, the union of a sequence of compact subsets of $T$, such that $f = f \varphi_A$ locally almost everywhere.*

The first assertion follows immediately from Lemma 1 of Ch. IV, §5, No. 6. To establish the second, denote by $A$ a moderated subset such that f is zero outside A; A is the union of a negligible set $A_0$ and a sequence $(A_n)_{n \geq 1}$ of compact sets, which we may suppose to be increasing. The function $f$ is then almost everywhere equal to the upper envelope of the functions $f \varphi_{A_n}$ ($n \geq 1$), therefore (Ch. IV, §1, No. 3, Th. 3 and §2, No. 3, Prop. 6)

$$
\mu^*(f) = \lim_{n \to \infty} \mu^*(f \varphi_{A_n}) \leq \mu^\bullet(f),
$$

whence the equality $\mu^*(f) = \mu^\bullet(f)$ by virtue of the formula (1). Finally, suppose that $\mu^\bullet(f) < +\infty$; there exists an increasing sequence $(A_n)$ of compact sets such that

$$
\mu^\bullet(f) = \sup_n \mu^*(f \varphi_{A_n}).
$$

Set $A = \bigcup_n A_n$; the second member is equal to $\mu^*(f \varphi_A)$ (Ch. IV, §1, No. 3, Th. 3), that is, to $\mu^\bullet(f \varphi_A)$ (by Prop. 1, or by 2) above). Since $\mu^\bullet(f) = \mu^\bullet(f \varphi_A) + \mu^\bullet(f \varphi_{\mathbf{C}_A})$ (Prop. 2), we have $\mu^\bullet(f \varphi_{\mathbf{C}_A}) = 0$, from which 3) follows.

#### Corollary 1 {#int-v-s1-prop-7-cor-1 .statement}

*For f to be negligible, it is necessary and sufficient that it be locally negligible and moderated.*

#### Corollary 2 {#int-v-s1-prop-7-cor-2 .statement}

*If $\mu$ is a moderated measure (in particular if $\mu$ is bounded, or if T is countable at infinity), then $\mu^* = \mu^\bullet$.*

#### Proposition 8 {#int-v-s1-prop-8 .statement}

a) *Let H be a set of functions $\geq 0$, lower semi-continuous, directed for the relation $\leq$; then*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

b) *Let H be a set of functions $\geq 0$, upper semi-continuous, directed for the relation $\geq$; if there exists in H a function $h_0$ such that $\mu^\bullet(h_0) < +\infty$, then*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

The assertion a) is, in view of Prop. 4, a repetition of Theorem 1 of Ch. IV, §1, No. 1. To establish b), set $\eta = \inf_{h \in H} h$, and let $a$ be a number $> 0$. There exists a compact set K such that (Ch. IV, §4, No. 4, Cor. 1 of Prop. 5):

$$
\mu^\bullet(h_0) - a \leq \mu^*(h_0 \varphi_K) = \mu(h_0 \varphi_K) \leq \mu^\bullet(h_0).
$$

The functions $h\varphi_K$, where $h$ runs over $H$, form a set of upper semi-continuous functions, directed for the relation $\geqslant$, which contains an integrable function. Therefore (Ch. IV, §4, No. 4, Cor. 2 of Prop. 5):

$$
\mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K).
$$

But (Ch. IV, §4, No. 4, Cor. 1 of Prop. 5) $\mu^\bullet(h_0\varphi_{C_K}) \leqslant a$, whence $\mu^\bullet(h\varphi_{C_K}) \leqslant a$ for every function $h \in H$ such that $h \leqslant h_0$. Therefore, finally:

$$
\mu^\bullet(\eta) \geqslant \mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K) \geqslant \inf_{h \in H} \mu^\bullet(h) - a.
$$

The inequality $\mu^\bullet(\eta) \leqslant \inf_{h \in H} \mu^\bullet(h)$ being obvious, and $a$ being arbitrary, the proposition is established.

### 3. Essentially integrable functions

Let $F$ be a real Banach space; recall that the elements of the spaces $\mathcal{F}_F^p$ (Ch. IV, §3, No. 3) and $\mathcal{L}_F^p$ (Ch. IV, §3, No. 4, Def. 2) are $\mu$-moderated functions (Ch. IV, §5, No. 6, Lemma 1); with $\mathcal{N}_F$ still denoting the space of negligible mappings of $T$ into $F$, we shall introduce the space $\mathcal{N}_F^\infty$ of locally negligible mappings of $T$ into $F$.

#### Lemma {#int-v-s1-n3-lem-1 .statement}

*Let $g$ and $g'$ be two $\mu$-moderated mappings with values in $F$; if $g$ and $g'$ are equal locally almost everywhere to a same function $f$, then $g = g'$ almost everywhere.*

For, let $D$ be the set of $t \in T$ such that $g(t) \neq g'(t)$; $D$ is locally negligible and moderated, therefore negligible (Cor. 1 of Prop. 7).

We shall denote by $\overline{\mathcal{F}}_F^p(T, \mu)$ (or simply $\overline{\mathcal{F}}_F^p(\mu)$, $\overline{\mathcal{F}}_F^p$, if no confusion can result) the set of mappings $f$ of $T$ into $F$, such that there exists a function $g \in \mathcal{F}_F^p$ equal to $f$ locally almost everywhere. Since the number $N_p(g)$ depends only on $f$ by the Lemma, we will write $\overline{N}_p(f) = N_p(g)$. The function $\overline{N}_p$ is obviously a semi-norm on $\overline{\mathcal{F}}_F^p$, and we shall always assume that $\overline{\mathcal{F}}_F^p$ is equipped with the topology defined by $\overline{N}_p$. The closure of 0 for this topology is the space $\mathcal{N}_F^\infty$; the relations $\overline{\mathcal{F}}_F^p = \mathcal{F}_F^p + \mathcal{N}_F^\infty$, $\mathcal{N}_F^\infty \cap \mathcal{F}_F^p = \mathcal{N}_F$ (Lemma) show that the normed space $\overline{\mathcal{F}}_F^p / \mathcal{N}_F^\infty$ may be canonically identified with $\mathcal{F}_F^p / \mathcal{N}_F$, which is complete (Ch. IV, §3, No. 3, Prop. 5); therefore $\overline{\mathcal{F}}_F^p$ is itself complete.

We shall similarly denote by $\overline{\mathcal{L}}_F^p(T, \mu)$ (or $\overline{\mathcal{L}}_F^p(\mu)$, or $\overline{\mathcal{L}}_F^p$) the subspace $\mathcal{L}_F^p + \mathcal{N}_F^\infty$ of $\overline{\mathcal{F}}_F^p$; one can also characterize $\overline{\mathcal{L}}_F^p$ as the subspace of $\overline{\mathcal{F}}_F^p$ constituted by the *measurable* mappings (Ch. IV, §5, No. 6, Th. 5).

The normed space $\overline{\mathcal{L}}_F^p / \mathcal{N}_F^\infty$ may be canonically identified with $L_F^p$; $\overline{\mathcal{L}}_F^p$ is therefore complete. Its elements are called the *p-th power essentially integrable functions*, this terminology being justified by the following proposition:

#### Proposition 9 {#int-v-s1-prop-9 .statement}

*For a mapping f of T into F to belong to $\overline{\mathcal{F}}_F^p$ (resp. to $\overline{\mathcal{L}}_F^p$), if is necessary and sufficient that* (resp. *that f be measurable and that*)

$$
\mu^\bullet(|f|^p) < +\infty .
$$

*One then has* $\overline{N}_p(f) = (\mu^\bullet(|f|^p))^{1/p}$.

We may clearly limit ourselves to the assertion concerning $\overline{\mathcal{F}}_F^p$. If f belongs to $\overline{\mathcal{F}}_F^p$, let g be a function belonging to $\mathcal{F}_F^p$ that is equal to f locally almost everywhere; then $|f|^p = |g|^p$ locally almost everywhere, therefore

$$
\mu^\bullet(|f|^p) = \mu^\bullet(|g|^p) = \mu^*(|g|^p) < +\infty
$$

(Prop. 1, a) and Prop. 7), and, on the other hand, by the definition of $\overline{N}_p$,

$$
\overline{N}_p(f) = N_p(g) = (\mu^*(|g|^p))^{1/p} .
$$

Conversely, suppose that $\mu^\bullet(|f|^p) < +\infty$; then there exists a moderated set A such that f is zero locally almost everywhere in T − A (Prop. 7). The function $f \varphi_A$, equal locally almost everywhere to f, is such that $N_p(f \varphi_A) = \overline{N}_p(f) < +\infty$, therefore it belongs to $\mathcal{F}_F^p$, and $f \in \overline{\mathcal{F}}_F^p$.

#### Corollary {#int-v-s1-n3-cor-1 .statement}

*For f to belong to $\mathcal{L}_F^p$, it is necessary and sufficient that f belong to $\overline{\mathcal{L}}_F^p$ and be moderated.*

#### Definition 3 {#int-v-s1-def-3 .statement}

*The elements of $\overline{\mathcal{L}}_F^1$ are called essentially $\mu$-integrable functions with values in F. On composing the mapping $\tilde{f} \mapsto \mu(f)$ of $L_F^1$ into F with the canonical mapping of $\overline{\mathcal{L}}_F^1$ onto $L_F^1$, one obtains a continuous linear mapping of $\overline{\mathcal{L}}_F^1$ into F that extends the mapping $f \mapsto \int f d\mu$ of $\mathcal{L}_F^1$ into F. One again denotes by $\int f d\mu$ or $\mu(f)$ the value of this mapping for $f \in \overline{\mathcal{L}}_F^1$, and this element is called the integral of f with respect to $\mu$.*

Two essentially integrable functions that are equal locally almost everywhere have the same integral. For every function $f \geq 0$ that is finite and essentially integrable, $\int^\bullet f d\mu = \int f d\mu$. If A is a set whose characteristic function is essentially integrable, then A is said to be an *essentially $\mu$-integrable set*; $\int \varphi_A d\mu$ is also denoted $\mu(A)$ and is again called the *measure* of A.

If a function $f$, with values in $F$, is defined locally almost everywhere in $T$, we again say that $f$ is *essentially integrable* if it is equal, locally almost everywhere, to a function $f_1$ that is everywhere defined and integrable; we then set
$$
\int f\, d\mu = \int f_1\, d\mu,
$$
and this definition is independent of the integrable function $f_1$ everywhere defined and equal locally almost everywhere to $f$ (Lemma). One defines similarly the notion of essentially integrable function for functions with values in $\overline{\mathbf{R}}$ that are defined and finite locally almost everywhere.

The reader will have no difficulty in extending, to essentially integrable functions, the results of Ch. IV, §4 for integrable functions, on replacing 'almost everywhere' in the statements by 'locally almost everywhere.' We note for example the inequality
$$
\left| \int f\, d\mu \right| \leq \int |f|\, d\mu,
$$
valid for every essentially integrable function $f$ with values in a Banach space.

#### Proposition 10 {#int-v-s1-prop-10 .statement}

*Let $\mathfrak{K}$ be a $\mu$-dense set of compact subsets of $T$.*
a) *If $f$ is a numerical function $\geq 0$, then*
$$
\mu^\bullet(f) = \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K).
$$
b) *If $f$ is an essentially integrable function with values in a Banach space $F$, then*
$$
\int f\, d\mu = \lim_{\mathfrak{K}} \int f \varphi_K\, d\mu,
$$
*the limit being taken with respect to the directed (for $\subset$) set $\mathfrak{K}$.*

To establish a), it suffices to show that for every compact subset $L$ of $T$,
$$
\int^* f \varphi_L\, d\mu = \sup_K \int^* f \varphi_K\, d\mu,
$$
where $K$ runs over the set of subsets of $L$ belonging to $\mathfrak{K}$. Since $L$ is the union of a negligible set and an increasing sequence $(K_n)$ of elements of $\mathfrak{K}$ (Ch. IV, §5, No. 8, Prop. 12), this follows from the theorem on passage to the limit in upper integrals (Ch. IV, §1, No. 3, Th. 3).

Suppose now that $f$ belongs to $\mathcal{L}_F^1$; let $\varepsilon$ be a number $> 0$, and let $K$ be an element of $\mathfrak{K}$ such that
$$
\int |f| \varphi_K\, d\mu \geq \int |f|\, d\mu - \varepsilon
$$

(such a K exists by a)). Then, for every compact set H containing K,

$$
\left| \int f \, d\mu - \int f \varphi_H \, d\mu \right| \leq \int |f| \varphi_{\mathbf{C}_H} \, d\mu \leq \int |f| \varphi_{\mathbf{C}_K} \, d\mu \leq \varepsilon .
$$

Extension to complex Banach spaces and measures. Let F be a complex Banach space; by an abuse of notation, the real Banach space underlying F will also be denoted by F. The Banach space $\overline{\mathcal{L}}_F^p(T, \mu)$ may then be equipped with a natural complex Banach space structure, and it is necessary to be specific as to whether one is using the real or the complex structure of this space. In this chapter, and absent express mention to the contrary, it will always be understood to be the real structure.

Let $\theta$ be a complex measure; we set $\overline{\mathcal{L}}_F^p(T, \theta) = \overline{\mathcal{L}}_F^p(T, |\theta|)$; if F is a complex Banach space, one can make the same remarks as above. In particular, a function f with values in F will be called essentially integrable for $\theta$ if it is essentially integrable for $|\theta|$. Assertion b) of Prop. 10 then extends at once to complex measures.

### 4. A property special to the essential upper integral

The following result will be used frequently in the sequel. In the statement, one cannot replace essential upper integrals by ordinary upper integrals (see Exer. 4).

#### Proposition 11 {#int-v-s1-prop-11 .statement}

— Let $(\lambda_\alpha)_{\alpha \in A}$ be a family of positive measures on T, directed for the relation $\leq$ and having a supremum $\lambda$ in $\mathcal{M}(T)$. Then, for every numerical function $f \geq 0$,

$$
\lambda^\bullet(f) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

When $f$ belongs to $\mathcal{K}(T)$, this relation reduces to the definition of the supremum of a directed set in $\mathcal{M}(T)$ (Ch. II, §2, No. 2, Lemma). Suppose next that $f \leq g$ for some function $g \in \mathcal{K}_+$ (in other words, that $f$ is bounded and is zero outside a compact set K); let $\alpha$ be an index such that $\lambda_\alpha(g) \geq \lambda(g) - \varepsilon$, where $\varepsilon$ is a number $> 0$; since the measure $\nu = \lambda - \lambda_\alpha$ is positive, we have $\nu^*(f) \leq \nu(g) \leq \varepsilon$, or $\lambda_\alpha^*(f) \geq \lambda^*(f) - \varepsilon$ (Ch. IV, §1, No. 3, Prop. 15). It follows (since $\varepsilon$ is arbitrary) that the second member of (5) is $\geq$ the first; the reverse inequality being obvious, (5) is established for the special case under consideration. Next, suppose that $f$ is zero outside K but is not necessarily bounded, and set $f_n = \inf(f, n)$ for every integer $n$. Then

$$
\lambda^\bullet(f) = \sup_{n \in \mathbf{N}} \lambda^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \sup_{n \in \mathbf{N}} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Finally, with no restriction made on $f$, denoting by $\mathcal{K}$ the set of compact subsets of $T$ we have
$$
\lambda^\bullet(f) = \sup_{K \in \mathcal{K}} \lambda^\bullet(f \varphi_K) = \sup_{K \in \mathcal{K}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f \varphi_K)
$$
$$
= \sup_{\alpha \in A} \sup_{K \in \mathcal{K}} \lambda_\alpha^\bullet(f \varphi_K) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

#### Corollary 1 {#int-v-s1-prop-11-cor-1 .statement}

*For a subset N of T to be locally $\lambda$-negligible, it is necessary and sufficient that N be locally $\lambda_\alpha$-negligible for every $\alpha \in A$.*

#### Corollary 2 {#int-v-s1-prop-11-cor-2 .statement}

*For a mapping g of T into a topological space G to be $\lambda$-measurable, it is necessary and sufficient that it be $\lambda_\alpha$-measurable for every $\alpha \in A$.*

The condition is obviously necessary, since $\lambda_\alpha \leq \lambda$ for every $\alpha$ (Ch. IV, §1, No. 3, Prop. 15). Conversely, suppose that $g$ is $\lambda_\alpha$-measurable for all $\alpha$, denote by $\mathcal{K}$ the set of compact subsets K of T such that $g|K$ is continuous, and let L be a compact set such that $L \cap K$ is $\lambda$-negligible for every $K \in \mathcal{K}$. Since the set $\mathcal{K}$ is $\lambda_\alpha$-dense, L is $\lambda_\alpha$-negligible for every $\alpha$ (Ch. IV, §5, No. 8, Prop. 12), hence is $\lambda$-negligible (Cor. 1). It follows that $\mathcal{K}$ is $\lambda$-dense and that $g$ is $\lambda$-measurable (Ch. IV, §5, No. 10, Prop. 15).

### Exercises {#int-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
