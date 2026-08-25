---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 4
section_title: Normal spaces
lang: en
source: top-v-x
pdf_pages: 0185-0196, 0245-0255
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NORMAL SPACES
      page: 0
      pdf_page: 185
    - "no": 2
      title: EXTENSION OF A CONTINUOUS REAL-VALUED FUNCTION
      page: 0
      pdf_page: 188
    - "no": 3
      title: LOCALLY FINITE OPEN COVERINGS OF A CLOSED SET IN A NORMAL SPACE
      page: 0
      pdf_page: 191
    - "no": 4
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 193
    - "no": 5
      title: PARACOMPACTNESS OF METRIZABLE SPACES
      page: 0
      pdf_page: 194
statements: 24
exercises: 7
content_sha256: 5a6d198ba815a6b655dfe1a7d2ffc8cb1105b770a7bb04499c7a43e1d1d1167e
---

## 4. NORMAL SPACES

### 1. DEFINITION OF NORMAL SPACES

Axiom ($O_{IV}$) for uniformizable spaces ($\S 1$, no. 5) can be stated in the following form: *given any closed set* $A$ *and any point* $x \in \mathbf{C}A$, *there is a continuous mapping of* $X$ *into* $[0, 1]$ *which is equal to* 0 *at* $x$ *and is equal to* 1 *at* every point of $A$; this property can again be expressed by saying that in a uniformizable space we can separate a point and a closed set (not containing the point) by a continuous real-valued function.

We shall now study spaces in which it is possible in the same way to separate two disjoint closed sets by a continuous real-valued function:

#### Definition 1 {#top-ix-s4-def-1 .statement}

*A topological space $X$ is said to be normal if it is Hausdorff and satisfies the following axiom:*

$(O_v)$ *If $A$ and $B$ are any two disjoint closed subsets of $X$, there exists a continuous mapping of $X$ into $[0, 1]$ which is equal to $0$ at every point of $A$ and to $1$ at every point of $B$.*

Clearly every normal space is completely regular; but there are completely regular spaces which are not normal (see Exercises 9, 10, 13, 26 and § 5, Exercises 15 and 16).

The statement of Axiom $(O_v)$, like that of $(O_{IV})$, involves the real line $\mathbf{R}$ as an auxiliary set. But there is a condition equivalent to $(O_v)$ which involves no auxiliary set:

#### Theorem 1 (Urysohn) {#top-ix-s4-thm-1 .statement}

*Axiom $(O_v)$ is equivalent to the following:*

$(O'_v)$ *If $A$ and $B$ are any two disjoint closed subsets of $X$, then there exist two disjoint open sets $U, V$ such that $A \subset U$ and $B \subset V$.*

It follows immediately that $(O_v)$ implies $(O'_v)$, for if $f$ is a continuous mapping of $X$ into $[0, 1]$ which is equal to $0$ on $A$ and to $1$ on $B$, then the open sets $\overline{f}^{-1}([0, 1/2[)$ and $\overline{f}^{-1}(]1/2, 1])$ contain $A$ and $B$ respectively and do not intersect.

To prove the converse, notice first that $(O'_v)$ is equivalent to the following axiom:

$(O''_v)$ *Given any closed set $A$ and any open neighbourhood $V$ of $A$, there exists an open neighbourhood $W$ of $A$ such that $\overline{W} \subset V$.*

If there is a continuous mapping $f : X \to [-1, +1]$ which is equal to $-1$ on $A$ and to $+1$ on $B$, and if we put $U(t) = \overline{f}^{-1}([-1, t[)$ for each $t \in [0, 1]$, then we have defined a family of open sets in $X$, indexed by $[0, 1]$, such that (i) $A \subset U(0)$, (ii) $B \subset \mathbf{C}U(1)$ and (iii) for each pair of real numbers $t, t'$ such that $0 \leq t < t' \leq 1$ we have

$$(1)$$
$$
\overline{U}(t) \subset U(t');
$$

for $U(t)$ is contained in the closed set $\overline{f}^{-1}([-1, t])$. Conversely, suppose that we have defined a family $(U(t))$ of open sets $(0 \leq t \leq 1)$ with these three properties (i), (ii) and (iii). For each $x \in X$, put $g(x) = 1$ if $x \in \mathbf{C}U(1)$, and if $x \in U(1)$ let $g(x)$ be the greatest lower bound of the values of $t$ such that $x \in U(t)$. Clearly $0 \leq g(x) \leq 1$ for each $x \in X$, $g(x) = 0$ on $A$, $g(x) = 1$ on $B$; also $g$ is continuous on $X$, for if we put $g(x) = a$, we have $|g(y) - g(x)| \leq \varepsilon$ for all $y \in U(a + \varepsilon) \cap \overline{\mathbf{C}U}(a - \varepsilon)$, which is a neighbourhood of $x$ by (i) [with the conventions that $U(a + \varepsilon) = X$ if $a + \varepsilon > 1$, and $U(a - \varepsilon) = \varnothing$ if $a - \varepsilon < 0$].

Hence Theorem 1 will be proved if we can define a family $(U(t))$ of open sets satisfying conditions (i), (ii) and (iii) above; to do this we use Axiom $(\mathrm{O}'_V)$. Take $U(1) = \mathbf{C}B$; since $A \subset U(1)$ there exists an open set $U(o)$ such that $A \subset U(o)$ and $U(o) \subset U(1)$ by $(\mathrm{O}'_V)$. Suppose then that for each dyadic number $k/2^n$ ($k = 0, 1, \ldots, 2^n$) we have defined an open set $U(k/2^n)$, these sets being such that $\overline{U}(k/2^n) \subset U((k+1)/2^n)$ for $0 \leq k \leq 2^n - 1$. For each dyadic number
$$
(2k + 1)/2^{n+1} \quad (0 \leq k \leq 2^n - 1)
$$
there exists by $(\mathrm{O}'_V)$ an open set $U((2k + 1)/2^{n+1})$ such that
$$
\overline{U}(k/2^n) \subset U((2k + 1)/2^{n+1})
$$
and
$$
\overline{U}((2k + 1)/2^{n+1}) \subset U((k + 1)/2^n).
$$
Hence for each dyadic number $r$ such that $0 \leq r \leq 1$ we can define an open set $U(r)$, such that $A \subset U(o)$, $B \subset \mathbf{C}U(1)$, and
$$(2)$$
$$
\overline{U}(r) \subset U(r')
$$
for each pair of dyadic numbers $r, r'$ such that $0 \leq r < r' \leq 1$.

Now define, for each real number $t \in [0, 1]$,
$$
U(t) = \bigcup_{r \leq t} U(r) \quad (r \text{ dyadic});
$$
by (2), this definition agrees with the preceding one for $t$ dyadic; also, if $0 \leq t < t' \leq 1$, then there exist two dyadic numbers $r, r'$ such that $t \leq r < r' \leq t'$; by (2) we have $U(t) \subset U(r)$, hence
$$
\overline{U}(t) \subset \overline{U}(r) \subset U(r') \subset U(t');
$$
this proves (1) and therefore completes the proof.

Theorem 1 will enable us to show that two important categories of topological spaces are normal. In the first place:

#### Proposition 1 {#top-ix-s4-prop-1 .statement}

*A compact space is normal.*

A compact space satisfies axiom $(\mathrm{O}'_V)$, by Proposition 2 of Chapter I, § 9, no. 2.

As to *locally compact* spaces, every point of such a space has a compact neighbourhood, which is a normal subspace; but there are examples of locally compact spaces which are *not normal* (cf. Exercises 9 and 26, and § 5, Exercise 15).

#### Proposition 2 {#top-ix-s4-prop-2 .statement}

*A metrizable space is normal.*

Let $X$ be a metrizable space and let $d$ be a metric compatible with the topology of $X$. Let $A, B$ be two disjoint closed subsets of $X$; since the functions $d(x, A)$ and $d(x, B)$ are continuous, the set $U$ (resp. $V$) of points $x$ such that $d(x, A) < d(x, B)$ [resp. $d(x, B) < d(x, A)$] is open; clearly $A \subset U$ and $B \subset V$ and $U \cap V = \varnothing$, hence Axiom $(O'_V)$ is satisfied.

#### Remark 1 {#top-ix-s4-n1-rem-1 .statement}

Proposition 2 gives another *necessary* condition for metrizability; but this condition, even in conjunction with all the necessary conditions given in § 2, does not give a set of sufficient conditions for metrizability (cf. Exercise 6 and § 5, Exercise 10).
2) There are examples of normal spaces which are neither metrizable nor locally compact (see § 5, Exercise 16).

By $(O'_V)$, every *closed* subset of a normal space is a *normal subspace*; but this is not always the case for an *arbitrary* subset of a normal space.

For example, a completely regular space which is not normal is homeomorphic to a subspace of a compact space (\$ 1, no. 5, Proposition 3), and the latter is normal.

Finally we record that the *product* of two normal spaces is not necessarily normal (see Exercise 9 and § 5, Exercise 16).

### 2. EXTENSION OF A CONTINUOUS REAL-VALUED FUNCTION

Let $X$ and $Y$ be two topological spaces and let $A \neq X$ be a *closed* subset of $X$. If $f$ is a continuous mapping of $A$ into $Y$, it is not always possible to *extend* $f$ to a continuous mapping of the whole of $X$ into $Y$. When $Y = \overline{\mathbf{R}}$, the possibility of such an extension is determined by the following theorem:

#### Theorem 2 (Urysohn) {#top-ix-s4-thm-2 .statement}

*Axiom* $(O_V)$ *is equivalent to the following property*: $(O''_V)$ *Given any closed subset* $A$ *of* $X$ *and any continuous real-valued function* $f$ *(finite or not)* *defined on* $A$, *there exists an extension* $g$ *of* $f$ *to the whole space* $X$, *which is a continuous mapping of* $X$ *into* $\overline{\mathbf{R}}$.

It is easy to see that $(O''_V)$ implies $(O_V)$; for if $B$ and $C$ are two disjoint closed subsets of $X$, then the function which is equal to 0 on $B$ and equal to $i$ on $C$ is defined and continuous on the closed set $B \cup C$, hence by $(O''_{V})$ has a continuous extension $f$ to $X$. If $g = \inf (f^{+}, 1)$, then $g$ is continuous on $X$, takes its values in $[0, 1]$ and is equal to $o$ on $B$ and to $i$ on $C$.

Let us show conversely that $(O_{V})$ implies $(O''_{V})$. Since $\overline{\mathbf{R}}$ and the interval $[ -i, +i ]$ are homeomorphic, we need consider only the case where the continuous mapping $f : A \to \overline{\mathbf{R}}$ takes its values in $[ -i, +i ]$. We shall construct an extension $g$ of $f$ to $X$ by forming a sequence $(g_{n})$ of continuous functions on $X$, such that the sequence $(g_{n}(x))$ converges for all $x \in X$ to a point of the interval $[ -i, +i ]$; this limit will, by definition, be the value of $g$ at $x$, and it will follow from the choice of the $g_{n}$ that the function $g$ satisfies the required conditions.

The definition of the $g_{n}$ rests on the following lemma:

#### Lemma 1 {#top-ix-s4-lem-1 .statement}

*Let $u$ be a continuous mapping of $A$ into $[ -i, +i ]$; then there is a continuous mapping $v$ of $X$ into $[ -i/3, +i/3 ]$, such that $|u(x) - v(x)| \leq 2/3$ for all $x \in A$.*

Let $H$ be the set of all $x \in A$ such that $-i \leq u(x) \leq -i/3$, and let $K$ be the set of all $x \in A$ such that $i/3 \leq u(x) \leq i$; $H$ and $K$ are closed in $A$, and therefore in $X$, and do not intersect; hence by $(O_{V})$ there is a continuous mapping $v$ of $X$ into $[ -i/3, +i/3 ]$ which is equal to $-i/3$ on $H$ and to $+i/3$ on $K$. The mapping $v$ satisfies the conditions of the lemma.

We now define the functions $g_{n}$ by induction. Applying the lemma with $u = f$, we define $g_{0}$ to be a continuous mapping of $X$ into $[ -i/3, +i/3 ]$ such that $|f(x) - g_{0}(x)| \leq 2/3$ for all $x \in A$. Suppose now that a continuous mapping $g_{n}$ of $X$ into the interval

$$
[-i + (\frac{2}{3})^{n+1}, i - (\frac{2}{3})^{n+1}]
$$

has been defined, such that $|f(x) - g_{n}(x)| \leq (\frac{2}{3})^{n+1}$ for all $x \in A$. Applying the lemma to the function $u(x) = (\frac{2}{3})^{n+1} (f(x) - g_{n}(x))$, we see that there exists a continuous mapping $h_{n+1}$ of $X$ into the interval

$$
\left[ -\frac{2^{n+1}}{3^{n+2}}, \frac{2^{n+1}}{3^{n+2}} \right]
$$

such that

$$
|f(x) - g_{n}(x) - h_{n+1}(x)| \leq (2/3)^{n+2}
$$

for all $x \in A$; the induction is completed by taking $g_{n+1} = g_{n} + h_{n+1}$, since this function satisfies the inequality $|g_{n+1}(x)| \leq 1 - (2/3)^{n+2}$ for all $x \in X$, by virtue of the definition of $h_{n+1}$.

From this definition it follows that, for $m \geq p$ and $n \geq p$, we have

$$
|g_{m}(x) - g_{n}(x)| \leq \frac{2^{p+1}}{3^{p+2}} \sum_{k=0}^{\infty} (2/3)^{k} = (2/3)^{p+1}
$$

at each point $x \in X$; hence the sequence $(g_n(x))$ is a Cauchy sequence for each $x \in X$, and therefore converges to a point $g(x)$ of the interval $[ -1, +1 ]$; and since $f(x) - g_n(x)$ tends to 0 for all $x \in A$ as $n \to \infty$, $g$ is an extension of $f$ to $X$. It remains therefore only to show that $g$ is continuous on $X$.

Now let $x$ be any point of $X$; then, given any $\varepsilon > 0$, there exists an integer $n_0$ such that $|g_m(y) - g_n(y)| \leq \varepsilon$ for all $y \in X$ and all $m \geq n_0$ and all $n \geq n_0$; hence, letting $m$ tend to $+\infty$, we have

$$
|g(y) - g_n(y)| \leq \varepsilon.
$$

Let $V$ be a neighbourhood of $x$ such that $|g_n(y) - g_n(x)| \leq \varepsilon$ for all $y \in V$; then, for each $y \in V$ we shall have

$$
|g(y) - g(x)| \leq |g(y) - g_n(y)| + |g_n(y) - g_n(x)| + |g(x) - g_n(x)| \leq 3\varepsilon,
$$

which shows that $g$ is continuous at $x$, and completes the proof of Theorem 2. (The last part of the proof uses, in a particular case, the idea of uniform convergence, which we shall study in general in Chapter X, no. 1.)

#### Corollary {#top-ix-s4-n2-cor-1 .statement}

*If $f$ is a finite continuous real-valued function defined on $A$, then there exists a finite continuous real-valued function $g$ defined on $X$, which extends $f$.*

First consider the case in which $f(x) \geq 0$ for all $x \in A$; then there is a continuous extension $g_1$ of $f$ to $X$, taking its values in $[0, +\infty]$. If we put $B = \overline{g_1}(+\infty)$, then $B$ is closed and by hypothesis does not meet $A$; the function $h$ which is equal to $f$ on $A$ and to 0 on $B$ is therefore a continuous function on the closed set $A \cup B$. Let $g_2$ be a continuous extension of $h$ to $X$, again taking its values in $[0, +\infty]$; the function $g = \inf(g_1, g_2)$ is then a continuous extension of $f$ to $X$, whose values are $\geq 0$ and *finite* at every point of $X$.

To pass to the general case, it is enough to remark that, if $f$ is finite and continuous on $A$, then so are $f^+$ and $f^-$; extending $f^+$ and $f^-$ to $X$ by finite continuous functions $g_1$ and $g_2$ respectively, we see that the function $g_1 - g_2$ is finite and continuous on $X$ and extends $f$.

#### Remark {#top-ix-s4-n2-rem-1 .statement}

If $X$ is a normal space and if $A$ is a closed subset of $X$, there exists also a continuous extension to $X$ of every continuous mapping $f$ of $A$ into a *cube* $K^1$ (\S 1, no. 5); for we have then $f = (f_i)_{i \in I}, f_i$ being a continuous mapping of $A$ into the compact interval $K$ of $\mathbf{R}$; since there exists a continuous mapping $g_i : X \to K$ which extends $f_i$, the mapping $g = (g_i)$ is a continuous extension of $f$ to $X$.

### 3. LOCALLY FINITE OPEN COVERINGS OF A CLOSED SET IN A NORMAL SPACE

#### Theorem 3 {#top-ix-s4-thm-3 .statement}

Let $(A_i)_{i \in I}$ be a locally finite open covering of a closed set $Y$ in a normal space $X$. Then there is an open covering $(B_i)_{i \in I}$ of $Y$ such that $\overline{B}_i \subset A_i$ for each $i \in I$.

Well-order the index set $I$ (Set Theory, Chapter III, § 2, no. 3, Theorem 1). We shall define a family $(B_i)_{i \in I}$ of open sets in $X$, by transfinite induction, such that (i) $\overline{B}_i \subset A_i$ for each $i \in I$; (ii) for each $i \in I$, the family formed by the $B_\lambda$ such that $\lambda \leq i$ and by the $A_\lambda$ such that $\lambda > i$ is an open covering of $Y$. Suppose that we have defined the $B_i$ for $i < \gamma$ so that (i) and (ii) are satisfied for all $i < \gamma$, and let us show that we can define $B_\gamma$ in such a way that (i) and (ii) are also satisfied for $i = \gamma$. Let us first show that the $B_i$ for which $i < \gamma$ and the $A_i$ for which $i \geq \gamma$ form a covering of $Y$. By hypothesis, for each $x \in Y$ there is only a finite number of indices $\lambda \in I$ such that $x \in A_\lambda$, say $\lambda_1 < \lambda_2 < \cdots < \lambda_n$; let $\lambda_h$ be the greatest of the $\lambda_i$ such that $\lambda_i < \gamma$; if $h < n$ we have $x \in A_{\lambda_n}$ and $\lambda_n \geq \gamma$, and if $h = n$ the inductive hypothesis shows that $x$ belongs to some $B_\lambda$ such that $\lambda \leq \lambda_n < \gamma$, and our assertion follows.

Now put $C = (\complement Y) \cup \left( \bigcup_{i < \gamma} B_i \right) \cup \left( \bigcup_{i > \gamma} A_i \right)$; $C$ is open, and from what has been said we have $\complement A_\gamma \subset C$; by virtue of Axiom $(O''_V)$ for normal spaces, there is therefore an open set $V$ such that $\complement A_\gamma \subset \overline{V} \subset V \subset C$. If we put $B_\gamma = \complement \overline{V}$, we have $\overline{B}_\gamma \subset \complement V \subset A_\gamma$ and $B_\gamma \cup C = X$, so that the $B_i$ such that $i \leq \gamma$ and the $A_i$ such that $i > \gamma$ cover $Y$.

#### Remark {#top-ix-s4-n3-rem-1 .statement}

Note that we have used only the fact that the covering $(A_i)$ is point-finite, i.e., that every point of $X$ belongs to only a finite number of sets $A_i$.

#### Definition 2 {#top-ix-s4-def-2 .statement}

Let $X$ be a topological space and let $f$ be a real-valued function defined on $X$. The support of $f$, denoted by $\operatorname{Supp}(f)$, is the smallest closed set $S$ in $X$ such that $f(x) = 0$ for all $x \notin S$.

In other words, $\operatorname{Supp}(f)$ is the closure in $X$ of the set of all $x \in X$ such that $f(x) \neq 0$; or again, it is the set of all $x \in X$ such that every neighbourhood of $x$ contains a point $y$ for which $f(y) \neq 0$.

Let $(f_i)_{i \in I}$ be a family of finite real-valued functions on $X$ whose supports form a locally finite family; then the sum $\sum_{i \in I} f_i(x)$ is defined for each $x \in X$ (since it contains only a finite number of non-zero terms). The finite real-valued function $x \to \sum_{i \in I} f_i(x)$ is called the sum of the family $(f_i)$, and is denoted by $\sum_{i \in I} f_i$. If each of the $f_i$ is continuous, then so is $f = \sum_{i \in I} f_i$; for if $x$ is any point of $X$, there is a neighbourhood $V$ of $x$ which meets only a finite number of supports of the $f_i$, and hence there is a finite subset $H$ of $I$ such that $f(y) = \sum_{i \in H} f_i(y)$ for all $y \in V$.

#### Definition 3 {#top-ix-s4-def-3 .statement}

*Given a family* $(A_i)_{i \in I}$ *of subsets of a topological space* $X$, *a family* $(f_i)_{i \in I}$ *of real-valued functions defined on* $X$ *is said to be subordinate to the family* $(A_i)_{i \in I}$ *if we have* $\operatorname{Supp}(f_i) \subset A_i$ *for each index* $i \in I$.

*A continuous partition of unity on* $X$ *is any family* $(f_i)_{i \in I}$ *of real-valued continuous functions* $\geq 0$ *on* $X$ *whose supports form a locally finite family and which are such that* $\sum_{i \in I} f_i(x) = 1$ *for all* $x \in X$.

#### Proposition 3 {#top-ix-s4-prop-3 .statement}

*Given any locally finite open covering* $(A_i)_{i \in I}$ *of a normal space* $X$, *there exists a continuous partition of unity* $(f_i)_{i \in I}$ *on* $X$, *subordinate to the covering* $(A_i)_{i \in I}$.

By Theorem 3 there exists an open covering $(B_i)_{i \in I}$ of $X$ such that $\overline{B}_i \subset A_i$ for each $i \in I$, and it is clear that the covering $(B_i)$ is locally finite. By axiom $(O''_V)$, for each $i \in I$ there exists an open set $C_i$ such that $\overline{B}_i \subset C_i \subset \overline{C}_i \subset A_i$. By axiom $(O_V)$, for each $i \in I$ there exists a continuous mapping $g_i$ of $X$ into $[0,1]$, such that $g_i(x) = 1$ on $\overline{B}_i$ and such that the support of $\overline{g}_i$ is contained in $\overline{C}_i$, and therefore contained in $A_i$. Since $(B_i)$ is a covering of $X$, we have $\sum_{i \in I} g_i(x) > 0$ for each $x \in X$; if we put
$$
f_i(x) = \frac{g_i(x)}{\sum_{i \in I} g_i(x)}
$$
for all $i \in I$ and all $x \in X$, then the $f_i$ form a continuous partition of unity subordinate to the covering $(A_i)$.

#### Corollary {#top-ix-s4-n3-cor-1 .statement}

*Given any locally finite open covering* $(A_i)$ *of a closed set* $F$ *in a normal space* $X$, *there exists a family* $(f_i)$ *of continuous real-valued functions* $\geq 0$ *on* $X$, *subordinate to the covering* $(A_i)_{i \in I}$ *and such that* $\sum_{i \in I} f_i(x) = 1$ *for all* $x \in F$ *and* $\sum_{i \in I} f_i(x) \leq 1$ *for all* $x \in X$.

The family of sets consisting of $CF$ and the $A_i$ is a locally finite open covering of $X$. There is therefore a continuous partition of unity subordinate to this covering, consisting of a family $(f_i)_{i \in I}$ such that $\operatorname{Supp}(f_i) \subset A_i$ for each $i \in I$, and a function $g$ whose support is contained in the complement of $F$. The family $(f_i)$ clearly satisfies the required conditions.

### 4. PARACOMPACT SPACES

We recall (Chapter I, § 9, no. 10) that a topological space $X$ is said to be *paracompact* if it is Hausdorff and if every open covering of $X$ has a locally finite open refinement.

#### Proposition 4 {#top-ix-s4-prop-4 .statement}

*Every paracompact space is normal.*

This is a consequence of the following lemma:

#### Lemma 2 {#top-ix-s4-lem-2 .statement}

*Let $A, B$ be two disjoint closed subsets of a paracompact space $X$. If for each $x \in A$ there is an open neighbourhood $V_x$ of $x$ and an open neighbourhood $W_x$ of $B$ which do not intersect, then there exists an open neighbourhood $T$ of $A$ and an open neighbourhood $U$ of $B$ which do not intersect.*

Assuming the truth of this lemma for the moment, we can apply it to the case where $B$ consists of a single point, because $X$ is Hausdorff, and it shows then that $X$ is *regular*. We can then apply Lemma 2 again to any two disjoint closed subsets of $X$, and this shows that Axiom $(O'_V)$ is satisfied.

To prove the lemma, consider the open covering of $X$ consisting of $CA$ and the $V_x$, where $x \in A$; let $(T_i)_{i \in I}$ be a locally finite open refinement of this covering. Then, by definition, if $A \cap T_i \neq \emptyset$ there exists $x_i \in A$ such that $T_i \subset V_{x_i}$. Let $T$ be the open set which is the union of the $T_i$ which meet $A$, and let us show that there is an open neighbourhood $U$ of $B$ which does not meet $T$. For each $y \in B$ there is an open neighbourhood $S_y$ of $y$ which meets only a finite number of sets $T_i$; let $J$ be the finite subset of $I$ consisting of those indices $i$ such that $T_i$ meets both $S_y$ and $A$; if we put $U_y = S_y \cap \bigcap_{i \in J} W_{x_i}$, then $U_y$ is an open neighbourhood of $y$ which meets none of the $T_i$ which meet $A$, and hence $U_y \cap T = \emptyset$. Let $U = \bigcup_{y \in B} U_y$; then $U'$ is an open neighbourhood of $B$ which does not meet $T$, and the lemma is proved.

There exist normal spaces which are not paracompact (Exercise 19).

#### Corollary 1 {#top-ix-s4-lem-2-cor-1 .statement}

*Given any open covering $(A_i)_{i \in I}$ of a paracompact space $X$, there exists a continuous partition of unity $(f_i)_{i \in I}$ on $x$, subordinate to the covering $(A_i)$.*

Let $(U_\lambda)_{\lambda \in L}$ be a locally finite open covering of $X$ which refines the covering $(A_i)_{i \in I}$; then there is a mapping $\varphi : L \to I$ such that $U_\lambda \subset A_{\varphi(\lambda)}$ for each $\lambda \in L$. By Propositions 3 and 4, there exists a continuous partition of unity $(g_\lambda)_{\lambda \in L}$ subordinate to $(U_\lambda)$. For each $i \in I$, put

$$
f_i = \sum_{\varphi(\lambda) = i} g_\lambda;
$$

this sum is defined and continuous since the supports of the $g_\lambda$ form a locally finite covering; moreover, the union $B_i$ of the supports of the $g_\lambda$ such that $\varphi(\lambda) = i$ is closed, by Proposition 4 of Chapter I, § 1, no. 6, and is contained in $A_i$. Since we have $f_i(x) = 0$ whenever $x \in \mathbf{C}B_i$, the support of $f_i$ is contained in $B_i$, and therefore in $A_i$. On the other hand, the family $B_i$ is locally finite, because for each $x \in X$ there is a neighbourhood $V$ of $x$ and a finite subset $H$ of $I$ such that $V \cap U_\lambda = \emptyset$ for all $\lambda \notin H$, and it follows therefore that $V \cap B_i = \emptyset$ for all $i \notin \varphi(H)$. Finally, for each $x \in X$ we have

$$
1 = \sum_{\lambda \in L} g_\lambda(x) = \sum_{i \in I} \left( \sum_{\varphi(\lambda) = i} g_\lambda(x) \right) = \sum_{i \in I} f_i(x),
$$

and the proof is complete.

#### Corollary 2 {#top-ix-s4-lem-2-cor-2 .statement}

*If F is a closed subset of a paracompact space X, then every neighbourhood of F in X contains a closed (and therefore paracompact) neighbourhood of F.*

By Proposition 16 of Chapter I, § 9, no. 10, any closed subspace of X is paracompact; the corollary therefore follows from Proposition 4 and Axiom $(O_v')$.

### 5. PARACOMPACTNESS OF METRIZABLE SPACES

The following theorem sharpens the result of Proposition 2 of no. 1:

#### Theorem 4 {#top-ix-s4-thm-4 .statement}

*Every metrizable space is paracompact.*

The theorem is a consequence of the following four lemmas.

#### Lemma 3 {#top-ix-s4-lem-3 .statement}

*Let $\mathcal{R} = (U_\alpha)_{\alpha \in A}$ be an open covering of a metrizable space X. Then there is a sequence $(\mathcal{G}_n)$ of locally finite families of open subsets of X, such that $\mathcal{S} = \bigcup_n \mathcal{S}_n$ is an open covering of X which refines $\mathcal{R}$.

Let $d$ be a metric on X compatible with its topology. For each $\alpha \in A$ and each integer $n$, let $F_{n\alpha}$ denote the set of all $x \in U_\alpha$ such that $d(x, X - U_\alpha) \geq 2^{-n}$. Since $X - U_\alpha$ is closed, we have $U_\alpha = \bigcup_n F_{n\alpha}$.

Well-order the set $A$; for each $\alpha \in A$ and each integer $n$, let $G_{n\alpha}$ be the set of all $x \in F_{n\alpha}$ such that $x \notin F_{n+1,\beta}$ for all $\beta < \alpha$, and let $V_{n\alpha}$ be the set of all $y \in X$ such that $d(y, G_{n\alpha}) > 2^{-n-3}$. $V_{n\alpha}$ is clearly an open set; on the other hand, $V_{n\alpha} \subset U_\alpha$, because for each $y \in V_{n\alpha}$ there exists $x \in G_{n\alpha}$ such that $d(x, y) \leq 2^{-n-1}$, and since $x \in F_{n\alpha}$, we have

$$
d(y, X - U_\alpha) \geq d(x, X - U_\alpha) - d(x, y) \geq 2^{-n-1},
$$

so that $y \in U_\alpha$. Furthermore, for each $x \in X$ let $\alpha$ be the smallest index in $A$ such that $x \in U_\alpha$; then there is an integer $n$ such that $x \in F_{n\alpha}$, and the definition of $\alpha$ implies that $x \in G_{n\alpha}$, so that $x \in V_{n\alpha}$. This shows that if we put $\mathfrak{S}_n = (V_{n\alpha})_{\alpha \in A}$, then $\mathfrak{S} = \bigcup_n \mathfrak{S}_n$ is an open covering of $X$ which refines $\mathcal{R}$; thus it remains to be shown that each of the families $\mathfrak{S}_n$ is *locally finite*. To this end we shall first show that $d(G_{n\alpha}, G_{n\beta}) \geq 2^{-n-1}$ if $\alpha \neq \beta$. Suppose that $\beta < \alpha$; then if $x \in G_{n\alpha}$ and $y \in F_{n\beta}$ we have $x \notin F_{n+1,\beta}$ by definition, hence $d(x, X - U_\beta) < 2^{-n-1}$ and $d(y, X - U_\beta) \geq 2^{-n}$, and therefore $d(x, y) \geq 2^{-n-1}$; since $G_{n\beta} \subset F_{n\beta}$, the assertion follows. From this it follows immediately, using the definition of $V_{n\alpha}$ and $V_{n\beta}$, that $d(V_{n\alpha}, V_{n\beta}) \geq 2^{-n-2}$. From this last inequality we deduce that, for each $z \in X$, the open ball with centre $z$ and radius $2^{-n-3}$ meets at most one set of the family $\mathfrak{S}_n$; hence $\mathfrak{S}_n$ is a locally finite family, and the proof is complete.

#### Lemma 4 {#top-ix-s4-lem-4 .statement}

*Let* $(\mathfrak{S}_n)$ *be a sequence of locally finite families of open sets in a topological space* $X$, *such that*
$$
\mathfrak{S} = \bigcup_n \mathfrak{S}_n
$$
*is a covering of* $X$. *Then there exists a locally finite (but not necessarily open) covering* $\mathcal{B}$ *of* $X$ *which refines* $\mathfrak{S}$.

Let $E_n$ be the open set in $X$ which is the union of all the sets of $\mathfrak{S}_n$; let $U_n$ denote $\bigcup_{k=1}^n E_k$ and let $A_n$ denote $U_n - U_{n-1}$ (with $U_0 = \varnothing$). Consider the set $\mathcal{B}$ of subsets $V \cap A_n$, where $V \in \mathfrak{S}_n$ and $n$ is any integer; we shall show that $\mathcal{B}$ satisfies the conditions of the lemma. For each $x \in X$ there is an integer $n$ such that $x \in A_n$, since the $A_n$ form a partition of $X$; thus $x \in E_n$ and there exists $V \in \mathfrak{S}_n$ such that $x \in V$; so $x \in V \cap A_n$, and we have proved that $\mathcal{B}$ is a covering of $X$. Clearly, this covering refines $\mathfrak{S}$. On the other hand, for each $x \in X$ there exists an integer $n$ such that $x \in U_n$; since $U_n$ is open and the $\mathfrak{S}_m$ are locally finite families, there exists a neighbourhood $W_m$ of $x$, for each $m$, contained in $U_n$, which meets only a finite number of sets of $\mathfrak{S}_m$; hence the neighbourhood $W = \bigcap_{m=1}^n W_m$ of $x$ meets only a finite number of sets of $\mathcal{B}$, because $W \cap A_p = \varnothing$ for $p > n$. Hence $\mathcal{B}$ is locally finite, and Lemma 4 is proved.

#### Lemma 5 {#top-ix-s4-lem-5 .statement}

*Let* $X$ *be a regular space such that, for each open covering* $\mathcal{R}$ *of* $X$, *there exists a (not necessarily open) locally finite covering* $\mathcal{U}$ *of* $X$ *which refines* $\mathcal{R}$. *Then for each open covering* $\mathcal{R}$ *of* $X$ *there exists a locally finite closed covering* $\mathfrak{F}$ *of* $X$ *which refines* $\mathcal{R}$.

Let $\mathcal{H}$ be any open covering of $X$. For each $x \in X$ there is an open set $U \in \mathcal{H}$ which contains $x$, and therefore (since $X$ is regular) an open neighbourhood $V_x$ of $x$ such that $\overline{V}_x \subset U$. The family $\mathcal{B}$ formed by the $V_x$ is an open covering of $X$, hence by hypothesis there is a locally finite covering $\mathcal{B}'$ which is finer than $\mathcal{B}$. Let $\mathcal{F}$ be the family of closures of the sets of $\mathcal{B}$. Since the covering $\mathcal{B}'$ formed by the $\overline{V}_x$ is finer than $\mathcal{H}$, and since $\mathcal{F}$ is finer than $\mathcal{B}'$, it follows that $\mathcal{F}$ is a closed covering of $X$ which refines $\mathcal{H}$. But also $\mathcal{F}$ is locally finite, because if an open set does not meet a set $B \in \mathcal{B}$, then it does not meet its closure $\overline{B}$ either.

#### Lemma 6 {#top-ix-s4-lem-6 .statement}

*Let $X$ be a Hausdorff space such that, given any open covering $\mathcal{H}$ of $X$, there exists a locally finite closed covering $\mathcal{F}$ of $X$ which refines $\mathcal{H}$. Then $X$ is paracompact.*

Let $\mathcal{H}$ be any open covering of $X$. We have to show that there is a locally finite open covering of $X$ which refines $\mathcal{H}$. Let $\mathcal{A}$ be a locally finite covering (closed or not) of $X$ which refines $\mathcal{H}$; for each $x \in X$, let $W_x$ be an open neighbourhood of $x$ which meets only a finite number of sets of $\mathcal{A}$. The family $\mathcal{W}$ of sets $W_x$ is an open covering of $X$. Let $\mathcal{F}$ be a locally finite *closed* covering of $X$ which refines $\mathcal{W}$. For each $A \in \mathcal{A}$, let $U_A$ be a set of $\mathcal{H}$ which contains $A$, and let $C_A$ be the union of the sets $F \in \mathcal{F}$ such that $A \cap F = \varnothing$. Since $\mathcal{F}$ is locally finite, $C_A$ is closed in $X$ (Chapter I, § 1, no. 6, Proposition 4) and therefore $A' = U_A \cap (X - C_A)$ is open. Since we have $A \cap C_A = \varnothing$ and $A \subset U_A$, it follows that $A \subset A'$, and the family $\mathcal{A}'$ of sets $A'$, as $A$ runs through $\mathcal{A}$, is an open covering of $X$; moreover, since $A' \subset U_A \in \mathcal{H}$, $\mathcal{A}'$ refines $\mathcal{H}$. It remains to show that $\mathcal{A}'$ is *locally finite*. For each $x \in X$ there is a neighbourhood $T$ of $x$ which meets only a finite number of sets of $\mathcal{F}$, say $F_1, \ldots, F_n$. Since each $F_i$ is contained in a set of the form $W_{y_i}$, by definition $F_i$ meets only a finite number of sets of $\mathcal{A}$; let $A_{ij}$ ($1 \leq j \leq s_i$) be these sets. If $A$ is a set of $\mathcal{A}$ other than one of the $A_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq s_i$), it follows from the definitions that $A'$ meets none of the $F_i$, and therefore does not meet $T \subset \bigcup_{i=1}^n F_i$. This completes the proof of Lemma 6 and of Theorem 4.

### Exercises {#top-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
