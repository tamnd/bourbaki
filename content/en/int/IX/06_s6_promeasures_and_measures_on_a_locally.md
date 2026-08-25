---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 6
section_title: Promeasures and measures on a locally convex space
lang: en
source: int-vii-ix
book_pages: INT IX.72-INT IX.101, INT IX.117
pdf_pages: 0254-0283, 0299-0299
extraction: ocr
subsections:
    - "no": 1
      title: Promeasures on a locally convex space
      page: 72
      pdf_page: 254
    - "no": 2
      title: Image of a promeasure
      page: 74
      pdf_page: 256
    - "no": 3
      title: Fourier transform of a promeasure
      page: 75
      pdf_page: 257
    - "no": 4
      title: Calculation of Gaussian integrals
      page: 77
      pdf_page: 259
    - "no": 5
      title: Gaussian promeasures and measures
      page: 78
      pdf_page: 260
    - "no": 6
      title: Examples of Gaussian promeasures
      page: 82
      pdf_page: 264
    - "no": 7
      title: Wiener measure
      page: 85
      pdf_page: 267
    - "no": 8
      title: Continuity of the Fourier transform
      page: 92
      pdf_page: 274
    - "no": 9
      title: Minlos’s lemma
      page: 93
      pdf_page: 275
    - "no": 10
      title: Measures on the dual of a nuclear space
      page: 96
      pdf_page: 278
    - "no": 11
      title: Measures on a Hilbert space
      page: 97
      pdf_page: 279
statements: 33
exercises: 1
content_sha256: 58e45819d7a42959dc83ab3b30467ce024124a58cd273e90753ba86f78cc31a1
---

## § 6. PROMEASURES AND MEASURES ON A LOCALLY CONVEX SPACE

Throughout this section, only vector spaces over the field of real numbers are considered. By locally convex space, is meant a topological vector space over $\mathbf{R}$ that is Hausdorff and locally convex. The topological dual of a locally convex space E will be denoted $E'$; for $x \in E$ and $x' \in E'$, one writes $\langle x, x' \rangle = x'(x)$.

### 1. Promeasures on a locally convex space

Let E be a locally convex space. We denote by $\mathcal{F}(E)$ the set of closed linear subspaces of E of finite codimension, ordered by the relation $\supset$. For every $V \in \mathcal{F}(E)$, $p_V$ denotes the canonical mapping of E onto $E/V$. Let V and W be two elements of $\mathcal{F}(E)$ such that $V \supset W$; we denote by $p_{VW}$ the mapping of $E/W$ into $E/V$ deduced from the identity mapping of E by passage to the quotients. The family $\mathcal{Q}(E) = (E/V, p_{VW})$ is an inverse system of locally convex spaces, indexed by $\mathcal{F}(E)$. It is called the *inverse system of finite-dimensional quotients of E*.

It can be shown that the inverse limit of the inverse system $\mathcal{Q}(E)$ is canonically isomorphic to the algebraic dual $E'{}^*$ of $E'$, equipped with the weak topology $\sigma(E'{}^*, E')$.

#### Definition 1 {#int-ix-s6-def-1 .statement}

*Let $E$ be a locally convex space. One calls promeasure on $E$ every inverse system$^{(1)}$ of measures (\S 4, No. 2, Def. 1) on the inverse system of finite-dimensional quotients of $E$.*

In other words, a promeasure $\mu$ on $E$ is a family $(\mu_V)_{V \in \mathscr{F}(E)}$, where $\mu_V$ is a bounded (positive) measure on the finite-dimensional space $E/V$, and where $\mu_V = p_{VW}(\mu_W)$ when $V \supset W$. All of the measures $\mu_V$ have the same total mass, which is called the *total mass* of the promeasure $\mu$.

For a subspace $V$ of $E$ to belong to $\mathscr{F}(E)$, it is necessary and sufficient that there exist a finite number of elements $x'_1, \ldots, x'_n$ of $E'$ such that $V$ consists of the $x \in E$ satisfying $\langle x, x'_i \rangle = 0$ for $1 \leq i \leq n$ (TVS, II, \S 6, No. 3, Cor. 2 of Th. 1 and No. 5, Cor. 2 of Prop. 7). Moreover, on a finite-dimensional vector space there exists one and only one Hausdorff topological vector space topology (TVS, I, \S 2, No. 3, Th. 2). Consequently, the concept of promeasure on $E$ depends only on the dual $E'$ of $E$.

Let $\lambda$ be a bounded measure on $E$. For every $V \in \mathscr{F}(E)$, let us denote by $\widetilde{\lambda}_V$ the image of $\lambda$ under the canonical mapping $p_V$ of $E$ onto $E/V$. One has $p_V = p_{VW} \circ p_W$ for any two elements $V$ and $W$ of $\mathscr{F}(E)$ such that $V \supset W$; consequently, the family $\widetilde{\lambda} = (\widetilde{\lambda}_V)_{V \in \mathscr{F}(E)}$ is a promeasure on $E$. We shall say that $\widetilde{\lambda}$ is the promeasure *associated* with the measure $\lambda$. One sees immediately that $\lambda$ and $\widetilde{\lambda}$ have the same total mass.

#### Proposition 1 {#int-ix-s6-prop-1 .statement}

*Let $E$ be a locally convex space. The mapping $\lambda \mapsto \widetilde{\lambda}$ is a bijection of the set of bounded measures on $E$ onto the set of promeasures $(\mu_V)_{V \in \mathscr{F}(E)}$ on $E$ satisfying the following condition:

For every $\varepsilon > 0$, there exists a compact subset $K$ of $E$ such that $\mu_V(E/V - p_V(K)) \leq \varepsilon$ for all $V \in \mathscr{F}(E)$.*

One knows that the intersection of the kernels of the continuous linear forms on $E$ is equal to 0 (TVS, II, \S 4, No. 1, Cor. 1 of Prop. 2); consequently $\bigcap_{V \in \mathscr{F}(E)} V = \{0\}$ and the family $(p_V)_{V \in \mathscr{F}(E)}$ is coherent and separating. The proposition then follows from Th. 1 of \S 4, No. 2.

In particular, the mapping $\lambda \mapsto \widetilde{\lambda}$ is injective. If $\mu$ is a promeasure on $E$, and if there exists a bounded measure $\lambda$ on $E$ such that $\mu = \widetilde{\lambda}$, we shall say, by an abuse of language, that $\mu$ is a measure. If $E$ is finite-dimensional, every promeasure $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ is a measure: for, $\{0\} \in \mathscr{F}(E)$, $E/\{0\} = E$ and $p_{V,\{0\}} = p_V$, whence $\mu_V = p_V(\mu_{\{0\}})$ for all $V \in \mathscr{F}(E)$; in other words, $\mu = \widetilde{\lambda}$ with $\lambda = \mu_{\{0\}}$.

(1) Also called a 'projective system'.

#### Proposition 2 {#int-ix-s6-prop-2 .statement}

— Let T be a countable set, and E the vector space of real functions on T, equipped with the topology of pointwise convergence. Every promeasure on E is a measure.

For every $t \in T$, let $\varepsilon_t$ be the linear form $f \mapsto f(t)$ on E. One knows (TVS, II, §6, No. 6, Cor. 2 of Prop. 8) that the family $(\varepsilon_t)_{t \in T}$ is a basis of the vector space $E'$. Denote by $\Phi$ the set of finite subsets of 'T', and for every $J \in \Phi$ let $E_J$ be the set of functions on T that are zero at every point of J. Let $F \in \mathcal{F}(E)$; since the orthogonal $F^\circ$ of F is a finite-dimensional subspace of $E'$, there exists a $J \in \Phi$ such that $F^\circ$ is contained in the linear subspace G of $E'$ generated by the $\varepsilon_t$ for $t \in J$. Since $F^\circ \subset G$, we have $E_J = G^\circ \subset F^{\circ\circ} = F$ and the countable family $(E_J)_{J \in \Phi}$ is cofinal in $\mathcal{F}(E)$. The proposition then follows from Th. 2 of §4, No. 3.

### 2. Image of a promeasure

Let E and $E_1$ be two locally convex spaces, and $u$ a continuous linear mapping of E into $E_1$. For every $V_1 \in \mathcal{F}(E_1)$, the subspace $V = \overline{u}^{-1}(V_1)$ of E belongs to $\mathcal{F}(E)$, and $u$ defines, by passage to the quotients, a linear mapping $u_{V_1}$ of $E/V$ into $E_1/V_1$. Let $V_1$ and $W_1$ in $\mathcal{F}(E_1)$ be such that $V_1 \supset W_1$; set $V = \overline{u}^{-1}(V_1)$ and $W = \overline{u}^{-1}(W_1)$. We have $V \supset W$, and a commutative diagram

$$
\begin{array}{ccc}
E & \xrightarrow{pw} & E/W & \xrightarrow{pvw} & E/V \\
\downarrow u & & \downarrow u_{W_1} & & \downarrow u_{V_1} \\
E_1 & \xrightarrow{pw_1} & E_1/W_1 & \xrightarrow{pv_{1W_1}} & E_1/V_1
\end{array}
$$

Now let $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ be a promeasure on E. For every $V_1 \in \mathcal{F}(E_1)$, set

(1)
$$
\nu_{V_1} = u_{V_1}(\mu_{u^{-1}(V_1)}).
$$

The commutativity of the preceding diagram shows that the family $\nu = (\nu_{V_1})_{V_1 \in \mathcal{F}(E_1)}$ is a promeasure on $E_1$. We say that $\nu$ is the image of $\mu$ under $u$, and denote it by $u(\mu)$.

Let $\lambda$ be a bounded measure on E, and $u(\lambda)$ the measure on $E_1$ that is the image of $\lambda$ under $u$. If the promeasure $\mu$ is associated with $\lambda$, then the promeasure $u(\mu)$ is associated with $u(\lambda)$. This follows from the commutativity of the preceding diagram.

Let $V \in \mathcal{F}(E)$. It is immediate that the image promeasure on $E/V$ of the promeasure $\mu$ under the canonical mapping $p_V : E \to E/V$ is associated with the measure $\mu_V$.

Let $u_1$ be a continuous linear mapping of $E_1$ into a locally convex space $E_2$. One establishes without difficulty the relation

$$
(u_1 \circ u)(\mu) = u_1(u(\mu))
$$

*(transitivity of the images of promeasures)*.

### 3. Fourier transform of a promeasure

Let $E$ be a locally convex space and $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ a promeasure on $E$. For every continuous linear form $x'$ on $E$, we denote by $\mu_{x'}$ the measure on $\mathbf{R}$ that is the image under $x'$ of the promeasure $\mu$ on $E$. The Fourier transform of $\mu$ is the function $\mathcal{F}\mu$ on $E'$ defined by

$$
(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it} d\mu_{x'}(t).
$$

Let $\lambda$ be a bounded measure on $E$. The Fourier transform of $\lambda$ is the function on $E'$ defined by

$$
(\mathcal{F}\lambda)(x') = \int_E e^{i\langle x, x' \rangle} d\lambda(x).
$$

Let $\mu$ be the promeasure associated with $\lambda$. For every $x' \in E'$, the measure $\mu_{x'}$ on $\mathbf{R}$ is the image under $x' : E \to \mathbf{R}$ of the measure $\lambda$ on $E$; from the formulas (2) and (3), one immediately deduces $\mathcal{F}\mu = \mathcal{F}\lambda$.

Let $\mu$ be any promeasure on $E$, and $u$ a continuous linear mapping of $E$ into a locally convex space $E_1$. Denote by $^t u$ the linear mapping of $E'_1$ into $E'$ that is the transpose of $u$, and by $\nu$ the promeasure $u(\mu)$ on $E_1$. For every $x'_1 \in E'_1$, we have $^t u(x'_1) = x'_1 \circ u$, whence

$$
\nu_{x'_1} = x'_1(\nu) = x'_1(u(\mu)) = (x'_1 \circ u)(\mu) = \mu_{^t u(x'_1)}.
$$

Consequently,

$$
\mathcal{F}(u(\mu)) = (\mathcal{F}\mu) \circ {}^t u.
$$

In particular, let us take for $u$ the canonical mapping $p_V$ of $E$ onto $E/V$ (for $V \in \mathcal{F}(E)$). The promeasure $p_V(\mu)$ on $E/V$ is associated with the measure $\mu_V$, and $^t p_V$ is an isomorphism of the dual of $E/V$ onto the subspace $V^\circ$ of $E'$ orthogonal to $V$. If $(E/V)'$ is identified with $V^\circ$ by means of $^t p_V$, then

$$
(\mathcal{F}\mu)(x') = \int_{E'/V} e^{i\langle x, x' \rangle} d\mu_V(x)
$$

for all $x' \in V^\circ$. One has $E' = \bigcup_{V \in \mathscr{F}(E)} V^\circ$, so that the preceding formula characterizes the function $\mathcal{F}\mu$ on $E'$. Finally, if one sets $x' = 0$ in (5), one sees that the total mass of $\mu$ is equal to $(\mathcal{F}\mu)(0)$.

#### Proposition 3 {#int-ix-s6-prop-3 .statement}

*Let $E$ be a locally convex space. The mapping $\mu \mapsto \mathcal{F}\mu$ of the set of promeasures on $E$ into the set of functions on $E'$ is injective.*

The formula (5) permits reducing to the case that $E$ is finite-dimensional; since every finite-dimensional space is isomorphic to a space $\mathbf{R}^n$, we can even suppose that there exists an integer $n \geqslant 0$ such that $E = \mathbf{R}^n$. We therefore have to prove that if $\mu$ is a bounded measure (not necessarily positive) on $\mathbf{R}^n$ and if

$$
\int_{\mathbf{R}^n} e^{i\langle x, y \rangle} d\mu(x) = 0
$$

for every linear form $y$ on $\mathbf{R}^n$, then $\mu = 0$.

For every integer $m \geqslant 0$, let $G_m$ be the subgroup $m \cdot \mathbf{Z}^n$ of $\mathbf{R}^n$. Denote by $\mathscr{C}_m$ the vector space of continuous functions $f$ on $\mathbf{R}^n$ such that $f(x + a) = f(x)$ for $x \in \mathbf{R}^n$ and $a \in G_m$. By Prop. 8 of GT, X, §4, No. 4, every function in $\mathscr{C}_m$ is the uniform limit of finite linear combinations of functions of the type $x \mapsto e^{2\pi i \langle x, q \rangle}$ with $q \in m^{-1} \cdot \mathbf{Z}^n$. Therefore $\mu(f) = 0$ for every function $f \in \mathscr{C}_m$.

Let $f$ be a continuous function on $\mathbf{R}^n$ with compact support. For every integer $m \geqslant 0$, set $f_m(x) = \sum_{q \in G_m} f(x + q)$. It is immediate that for every $x \in \mathbf{R}^n$, the preceding series has only finitely many terms, and that $f_m$ belongs to $\mathscr{C}_m$. Moreover, it is easy to see that the sequence $(f_m)$ tends to $f$ uniformly on every compact set, and that there exists a constant $C \geqslant 0$ such that $|f_m| \leqslant C$ for all $m$. Consequently, $\mu(f) = \lim_{m \to \infty} \mu(f_m)$ by Prop. 12 of §5, No. 6. Since $f_m \in \mathscr{C}_m$, we have $\mu(f_m) = 0$, whence finally $\mu(f) = 0$. Thus $\mu = 0$.

#### Remark {#int-ix-s6-n3-rem-1 .statement}

— When $E$ is finite-dimensional, every character of $E$ is of the form $x \mapsto e^{i\langle x, x' \rangle}$ with $x' \in E'$ (*Théor. spect.*, Ch. II, §1, No. 9, Cor. 3 of Prop. 12). In this case, Prop. 3 follows from the uniqueness theorem for the Fourier transformation (*loc. cit.*, §1, No. 6, Cor. of Prop. 6).*

### 4. Calculation of Gaussian integrals

#### Lemma 1 {#int-ix-s6-lem-1 .statement}

For every integer $n \geqslant 0$,

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2^{n+1 \over 2} \Gamma \left( {n+1 \over 2} \right)
$$
(6)

$$
\int_{\mathbf{R}} x^{2n} e^{-x^2/2} dx = (2\pi)^{1/2} \frac{(2n)!}{2^n n!}
$$
(7)

$$
\int_{\mathbf{R}} x^{2n+1} e^{-x^2/2} dx = 0.
$$
(8)

Recall the formula

$$
\Gamma(s) = \int_0^\infty u^{s-1} e^{-u} du
$$
(9)

valid for every real number $s > 0$ (FRV, VII, §1, No. 3, Prop. 3). On making the change of variable $x = (2u)^{1/2}$, it follows from (9) that

$$
\int_0^\infty x^n e^{-x^2/2} dx = \int_0^\infty (2u)^{n/2} e^{-u} {1 \over 2} 2^{1/2} u^{-1/2} du = 2^{n-1 \over 2} \Gamma \left( {n+1 \over 2} \right),
$$

whence the formula (6) since

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2 \int_0^\infty x^n e^{-x^2/2} dx.
$$

The formula (7) follows from (6) and the relation

$$
\Gamma \left( n + \frac{1}{2} \right) = \pi^{1/2} \frac{(2n)!}{2^{2n} n!}.
$$
(10)

For $n = 0$, this relation reduces to $\Gamma(\frac{1}{2}) = \pi^{1/2}$, that is, to the formula (21) of FRV, VII, §1, No. 3. The general case then follows by induction on $n$, on taking into account the relation $\Gamma(x+1) = x \cdot \Gamma(x)$ (loc. cit., §1, No. 1).

Finally, the formula (8) follows from the fact that the function $x \mapsto x^{2n+1} e^{-x^2/2}$ is odd.

#### Lemma 2 {#int-ix-s6-lem-2 .statement}

For every complex number $y$,

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = e^{-y^2/2}.
$$
(11)

In particular,

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} dx = 1.
$$

The change of variable $x \mapsto -x$ yields

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{-ixy} dx;
$$

since $\cos u = \frac{e^{iu} + e^{-iu}}{2}$ for every complex number $u$, it follows that

$$
(12) \quad (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx .
$$

For every integer $n \geqslant 0$, set

$$
g_n(x) = (-1)^n (2\pi)^{-1/2} \frac{(xy)^{2n}}{(2n)!} e^{-x^2/2}.
$$

By (7),

$$
(13) \quad \int_{\mathbf{R}} |g_n(x)| \, dx = \frac{1}{n!} \left( \frac{|y|^2}{2} \right)^n
$$
$$
(14) \quad \int_{\mathbf{R}} g_n(x) \, dx = \frac{1}{n!} \left( -\frac{y^2}{2} \right)^n,
$$

whence

$$
\sum_{n=0}^{\infty} \int_{\mathbf{R}} |g_n(x)| \, dx = e^{|y|^2/2} < +\infty.
$$

Since, moreover,

$$
(2\pi)^{-1/2} e^{-x^2/2} \cos xy = \sum_{n=0}^{\infty} g_n(x),
$$

this equality can be integrated term by term, whence

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx = \sum_{n=0}^{\infty} \int_{\mathbf{R}} g_n(x) \, dx = e^{-y^2/2}
$$

by (14). The formula (11) then follows from (12).

### 5. Gaussian promeasures and measures

#### Proposition 4 {#int-ix-s6-prop-4 .statement}

*Let E be a locally convex space. For every positive quadratic form Q on E', there exists one and only one promeasure $\Gamma_Q$ on E such that $\mathcal{F} \Gamma_Q = e^{-Q/2}$. The total mass of $\Gamma_Q$ is equal to 1.*

The uniqueness of $\Gamma_Q$ follows from Prop. 3 of No. 3. The total mass of $\Gamma_Q$ is equal to $(\mathcal{F}\Gamma_Q)(0) = e^{-Q(0)/2} = 1$. We will prove existence in stages.

A) E of finite dimension n, and Q nondegenerate.

By Lemma 2 of No. 4, the measure $\gamma_1$ on $\mathbf{R}$ having density $t \mapsto (2\pi)^{-1/2}e^{-t^2/2}$ is bounded, of total mass 1. Set $\gamma = \gamma_1 \otimes \cdots \otimes \gamma_1$ (n factors). From Lemma 2 of No. 4, one deduces

$$
\int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n) = \prod_{j=1}^n \int_{\mathbf{R}} e^{ia_j t} d\gamma_1(t)
$$
$$
= \prod_{j=1}^n (2\pi)^{-1/2} \int_{\mathbf{R}} e^{ia_j t} e^{-t^2/2} dt
$$
$$
= \prod_{j=1}^n e^{-a_j^2/2}
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right).
$$

Since Q is positive and nondegenerate, there exists a basis $(e'_1, \ldots, e'_n)$ of E' orthonormal for Q (Alg., Ch. IX, §7, No. 1). Let us denote by f the isomorphism $x \mapsto (e'_1(x), \ldots, e'_n(x))$ of E onto $\mathbf{R}^n$, and by $\Gamma_Q$ the measure $f^{-1}(\gamma)$ on E. Let $x' = a_1 e'_1 + \cdots + a_n e'_n$ be in E'; then $x'(f^{-1}(t_1, \ldots, t_n)) = \sum_{j=1}^n t_j a_j$ for $t_1, \ldots, t_n$ real, whence

$$
\int_E e^{i\langle x, x' \rangle} d\Gamma_Q(x) = \int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n)
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right) = \exp \left( -\frac{1}{2}Q(x') \right).
$$

Consequently, $\mathcal{F}\Gamma_Q = e^{-Q/2}$.

B) E finite-dimensional.

Let N be the linear subspace of E' formed by the $x'$ such that $Q(x') = 0$. Denote by M the orthogonal of N in E, and by j the canonical injection of M into E. The linear mapping ${}^t j : E' \to M'$ is surjective, with kernel N, therefore there exists on $M'$ a nondegenerate positive quadratic form q such that $Q = q \circ {}^t j$. By the foregoing, there exists a bounded measure $\Gamma$ on M such that $\mathcal{F}\Gamma = e^{-q/2}$. Setting $\Gamma_Q = j(\Gamma)$, we have

$$
\mathcal{F}\Gamma_Q = (\mathcal{F}\Gamma) \circ {}^t j = \exp(-q \circ {}^t j/2) = e^{-Q/2}
$$

by formula (4) of No. 3.

C) *The general case.*
Let $V \in \mathcal{F}(E)$. Denote by $p_V$ the canonical mapping of $E$ onto $E/V$, and by $Q_V$ the positive quadratic form $Q \circ {}^t p_V$ on $(E/V)'$; finally, let $\mu_V$ be the measure on $E/V$ with Fourier transform $e^{-Q_V/2}$ (cf. B)). If $W \in \mathcal{F}(E)$ is contained in $V$, then $p_V = p_{VW} \circ p_W$, whence $Q_V = Q_W \circ {}^t p_{VW}$; by formula (4) of No. 3, the measure $p_{VW}(\mu_W)$ has as Fourier transform the function $(e^{-Q_W/2}) \circ {}^t p_{VW} = e^{-Q_V/2}$, hence is equal to $\mu_V$. The family $(\mu_V)_{V \in \mathcal{F}(E)}$ is therefore a promeasure $\mu$ on $E$. Formula (5) of No. 3 shows that $\mathcal{F}\mu$ is equal to $e^{-Q/2}$.

#### Definition 2 {#int-ix-s6-def-2 .statement}

*Let $E$ be a locally convex space. For every positive quadratic form $Q$ on $E'$, the promeasure on $E$ whose Fourier transform is equal to $e^{-Q/2}$ is called the Gaussian promeasure on $E$ with variance $Q$, and is denoted $\Gamma_Q$. A promeasure $\mu$ on $E$ is said to be Gaussian if there exists a positive quadratic form $Q$ on $E'$ such that $\mu = \Gamma_Q$.*

By an abuse of language, a bounded measure $\mu$ on $E$ will be said to be Gaussian with variance $Q$ if the associated promeasure $\widetilde{\mu}$ is equal to $\Gamma_Q$.

#### Remark {#int-ix-s6-n5-rem-1 .statement}

— 1) Let $E$ be a finite-dimensional vector space, and let $\mu$ be a positive measure on $E$ of mass 1, such that every linear form on $E$ belongs to $\mathcal{L}^2(E, \mu)$. One defines an element $m$ of $E$ and a positive quadratic form $V$ on $E'$ by the formulas
$$
\langle m, x' \rangle = \int_E \langle x, x' \rangle d\mu(x), \quad V(x') = \int_E \langle x - m, x' \rangle^2 d\mu(x).
$$
In the traditional terminology of Probability Theory, $m$ is called the *mean* and $V$ the *variance* of $\mu$; $\mu$ is said to be *centered* if $m = 0$.

Now let $a$ be an element of $E$ and $Q$ a positive quadratic form on $E'$. Let us denote by $\Gamma_{a,Q}$ the image of the measure $\Gamma_Q$ under the translation $x \mapsto x + a$. It is easily seen that $\Gamma_{a,Q}$ is a positive measure on $E$ of mass 1, with Fourier transform $x' \mapsto e^{i\langle a, x' \rangle - \frac{1}{2} Q(x')}$ and mean $a$. Moreover, Prop. 6 below implies that $Q$ is the variance of $\Gamma_{a,Q}$. One traditionally says that $\Gamma_{a,Q}$ is the Gaussian measure with mean $a$ and variance $Q$, and that $\Gamma_Q = \Gamma_{0,Q}$ is the *centered* Gaussian measure with variance $Q$. Since we shall only be considering *centered* Gaussian measures, we shall omit this qualifier.

2) Let $Q$ be a quadratic form on the dual $E'$ of a locally convex space $E$. If there exists a promeasure on $E$ with Fourier transform $e^{-Q/2}$, the quadratic form $Q$ is necessarily positive: for, the function $e^{-Q/2}$ is bounded on $E'$; therefore, for every $x' \in E'$, the function $t \mapsto e^{-t^2 Q(x')/2} = e^{-Q(tx')/2}$ on $\mathbf{R}$ is bounded, whence $Q(x') \geq 0$.

3) The dual of $\mathbf{R}$ is canonically isomorphic to $\mathbf{R}$ and the positive quadratic forms on $\mathbf{R}$ are the functions of the form $t \mapsto at^2$ with $a \geq 0$. Therefore, there exists for every $a \geq 0$ one and only bounded measure $\gamma_a$ on $\mathbf{R}$ whose Fourier transform is equal to the function $t \mapsto e^{-at^2/2}$; by an abuse of language, $\gamma_a$ is said to be *the Gaussian measure on $\mathbf{R}$ with variance $a$*.

The Fourier transform of $\gamma_0$ is the constant 1, whence $\gamma_0 = \varepsilon_0$ (unit mass at the origin of $\mathbf{R}$). Suppose $a > 0$ and denote by $u_a$ the linear mapping $x \mapsto a^{1/2} x$; then $\mathcal{F}\gamma_a = \mathcal{F}\gamma_1 \circ {}^t u_a$, whence $\gamma_a = u_a(\gamma_1)$. Lemma 2 shows that $\gamma_1$ is the measure with density $x \mapsto (2\pi)^{-1/2} e^{-x^2/2}$ with respect to Lebesgue measure; from this, one easily deduces

$$
(15) \quad d\gamma_a(x) = (2\pi a)^{-1/2} e^{-x^2/2a} dx .
$$

The image of a Gaussian promeasure under a continuous linear mapping is a Gaussian promeasure. More precisely, we have the following result:

#### Proposition 5 {#int-ix-s6-prop-5 .statement}

*Let E and E₁ be two locally convex spaces, and u a continuous linear mapping of E into E₁. Let Q be a positive quadratic form on E', and Q₁ the positive quadratic form Q $\circ {}^t u$ on E'₁. Then $u(\Gamma_Q) = \Gamma_{Q_1}$.*

Set $\mu = u(\Gamma_Q)$. By formula (4) of No. 3,

$$
\mathcal{F}\mu = (\mathcal{F}\Gamma_Q) \circ {}^t u = e^{-Q/2} \circ {}^t u = e^{-Q_1/2} = \mathcal{F}\Gamma_{Q_1} ,
$$

whence $\mu = \Gamma_{Q_1}$ by Prop. 3 of No. 3.

#### Corollary {#int-ix-s6-n5-cor-1 .statement}

*Let E be a locally convex space and Q a positive quadratic form on E'. For every $x' \in E'$, the image of $\Gamma_Q$ under $x'$ is the Gaussian measure on $\mathbf{R}$ with variance $Q(x')$.*

#### Proposition 6 {#int-ix-s6-prop-6 .statement}

*Let E be a locally convex space, and $\mu$ a Gaussian measure on E, with variance Q. For every integer $n \geq 0$ and every $x' \in E'$, one has the relations*

$$
\begin{align*}
(16) & \quad \int_E |\langle x, x' \rangle|^n d\mu(x) = \pi^{-1/2} 2^{n/2} \Gamma\left( \frac{n+1}{2} \right) Q(x')^{n/2} \\
(17) & \quad \int_E \langle x, x' \rangle^{2n} d\mu(x) = \frac{(2n)!}{2^n n!} Q(x')^n \\
(18) & \quad \int_E \langle x, x' \rangle^{2n+1} d\mu(x) = 0 .
\end{align*}
$$

*In particular,*

$$
(19) \quad \int_E \langle x, x' \rangle^2 d\mu(x) = Q(x') \qquad (x' \in E') .
$$

If these formulas are true for an element $x'$ of $E'$, then they are true for all of its multiples $t \cdot x'$ (with $t$ real). We may therefore content ourselves with establishing them when $Q(x')$ is equal to 0 or 1.

$a)$ Suppose $Q(x') = 0$. The measure $x'(\mu)$ is equal to $\gamma_0 = \varepsilon_0$, therefore $x'$ is zero $\mu$-almost everywhere; the formulas (16) to (19) are then obvious.

b) Suppose $Q(x') = 1$, whence $x'(\mu) = \gamma_1$. Then
$$
\int_E |\langle x, x' \rangle|^n d\mu(x) = \int_{\mathbf{R}} |t|^n d\gamma_1(t) = (2\pi)^{-1/2} \int_{\mathbf{R}} |t|^n e^{-t^2/2} dt
$$
and (16) follows immediately from (6) (No 4, Lemma 1). Similarly, formulas (17) and (18) follow from (7) and (8). Finally, (19) is obtained by setting $n = 1$ in (17).

We can now prove a converse of the Cor. of Prop. 5.

#### Proposition 7 {#int-ix-s6-prop-7 .statement}

*Let E be a locally convex space and $\mu$ a promeasure on E. Suppose that $x'(\mu)$ is a Gaussian measure on $\mathbf{R}$ for every $x' \in E'$. Then $\mu$ is a Gaussian promeasure on E.*

For every $x' \in E'$, let $Q(x')$ be the variance of the Gaussian measure $x'(\mu)$ on $\mathbf{R}$. One has $x'(\mu) = \gamma_{Q(x')}$, whence
$$
(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it \cdot 1} d\gamma_{Q(x')}(t) = e^{-Q(x') \cdot 1^2 / 2}
$$
by the definition of $\mathcal{F}\mu$ (No. 3, formula (2)). In other words, $\mathcal{F}\mu = e^{-Q/2}$, and it remains to prove that $Q$ is a positive quadratic form on $E'$.

For every closed linear subspace V of E with finite codimension, denote by $p_V$ the canonical mapping of E onto $E/V$, by $\mu_V$ the measure $p_V(\mu)$ on $E/V$, and set $Q_V = Q \circ {}^t p_V$. Since $E' = \bigcup_{V \in \mathcal{F}(E)} \operatorname{Im}({}^t p_V)$ and ${}^t p_V$ is injective, it suffices to prove that $Q_V$ is a positive quadratic form on $(E/V)'$. Let $u \in (E/V)'$ and $x' = {}^t p_V(u)$. We have
$$
u(\mu_V) = u(p_V(\mu)) = x'(\mu) = \gamma_{Q(x')} ;
$$
Prop. 6 then implies
$$
Q_V(u) = Q(x') = \int_{\mathbf{R}} t^2 d\gamma_{Q(x')}(t) = \int_{E/V} u(x)^2 d\mu_V(x),
$$
thus $Q_V$ is a positive quadratic form on $(E/V)'$.

### 6. Examples of Gaussian promeasures

1) Let E be a real Hilbert space. The mapping $x' \mapsto \|x'\|^2$ is a positive quadratic form on $E'$. The corresponding Gaussian promeasure is called the *canonical Gaussian promeasure* on E. It can be shown that this promeasure is not a measure if E is infinite-dimensional.

Let $A$ be a continuous linear operator on $E$. The mapping $x' \mapsto \|{}^tA \cdot x'\|^2$ is a positive quadratic form on $E'$. The corresponding promeasure $\mu_A$ on $E$ is a measure if and only if $A$ is a Hilbert–Schmidt operator (cf. No. 11, Cor. 2 of Th. 3).

2) *Kernels of positive type.* Let $T$ be a set and $E = \mathbf{R}^T$ the vector space of real functions on $T$, equipped with the topology of pointwise convergence. For every $t \in T$, one denotes by $\varepsilon_t$ the linear form $f \mapsto f(t)$ on $E$. The family $(\varepsilon_t)_{t \in T}$ is a basis of $E'$ (TVS, II, §6, No. 6, Cor. 2 of Prop. 8).

One calls (real) kernel of positive type on $T$ every real-valued function $K$ on $T \times T$ satisfying the relations

$$
\text{(20)} \qquad K(t, t') = K(t', t) \quad \text{for } t, t' \text{ in } T,
$$
$$
\text{(21)} \qquad \sum_{i,j=1}^p c_i c_j K(t_i, t_j) \geqslant 0
$$

for any positive integer $p$, elements $t_1, \ldots, t_p$ of $T$, and real numbers $c_1, \ldots, c_p$. If this is so, the formula

$$
\text{(22)} \qquad q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t,t' \in T} c_t c_{t'} K(t, t')
$$

defines a positive quadratic form on $E'$. Conversely, if $q$ is a positive quadratic form on $E'$, then the formula

$$
\text{(23)} \qquad K(t, t') = \frac{1}{2} [q(\varepsilon_t + \varepsilon_{t'}) - q(\varepsilon_t) - q(\varepsilon_{t'})]
$$

defines a kernel $K$ of positive type on $T$. One thus obtains two mutually inverse bijections between the set of kernels of positive type on $T$, and that of the positive quadratic forms on $E'$.

Let $K$ be a kernel of positive type on $T$, and $q$ the associated quadratic form on $E'$. The Gaussian promeasure on $E$ with variance $q$ is also called the *Gaussian promeasure on $E$ with covariance* $K$. If $T$ is countable, Prop. 2 of No. 1 implies that this promeasure is a measure.

3) Let $T$ be a countable set. A kernel $\delta$ on $T$ of positive type is defined by setting

$$
\text{(24)} \qquad \delta(t, t') = \begin{cases}
1 & \text{if } t = t' \\
0 & \text{if } t \neq t'.
\end{cases}
$$

The corresponding quadratic form is given by $q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t \in T} c_t^2$. For every $t \in T$, let us denote by $\mu_t$ the Gaussian measure on $\mathbf{R}$ with variance 1;

one shows easily that the Gaussian measure on $\mathbf{R}^T$ with covariance $\delta$ is equal to $\bigotimes_{t \in T} \mu_t$.

4) Let $n \geq 1$ be an integer. A square matrix $C = (c_{ij})$ of order $n$ is said to be *positive symmetric* if it is symmetric and $\sum_{i,j=1}^n c_{ij} x_i x_j \geq 0$ for any real $x_1, \ldots, x_n$; it comes to the same to say that the mapping $(i, j) \mapsto c_{ij}$ is a kernel of positive type on the set $\{1, 2, \ldots, n\}$. We may therefore speak of the Gaussian measure $\gamma_C$ on $\mathbf{R}^n$, with covariance $C$; it is characterized by the formula

$$
(25) \quad \int_{\mathbf{R}^n} e^{i(x_1 t_1 + \cdots + x_n t_n)} d\gamma_C(t_1, \ldots, t_n) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_{jk} x_j x_k \right),
$$

for $x_1, \ldots, x_n$ real. From Prop. 6 of No. 5 (formula (19)), one deduces

$$
(26) \quad \int_{\mathbf{R}^n} t_j t_k d\gamma_C(t_1, \ldots, t_n) = c_{jk} \quad (1 \leq j, k \leq n).
$$

From Prop. 5 of No. 5, one deduces the formula

$$
(27) \quad u(\gamma_C) = \gamma_{UC^t U},
$$

where $u$ is a linear mapping of $\mathbf{R}^n$ into $\mathbf{R}^m$ with matrix $U$. Moreover, one sees easily (cf. the first part of the proof of Prop. 4 of No. 5) that if $I_n$ is the identity matrix of order $n$, then the measure $\gamma_{I_n}$ admits the density

$$
(2\pi)^{-n/2} \exp \left( - \frac{1}{2}(t_1^2 + \cdots + t_n^2) \right)
$$

with respect to the Lebesgue measure $\lambda_n$ on $\mathbf{R}^n$.

We are going to show that if the matrix $C$ is invertible, with inverse $D = (d_{jk})$, then

$$
(28) \quad d\gamma_C(t_1, \ldots, t_n) =
(2\pi)^{-n/2} (\det D)^{1/2} \left( \exp \left( - \frac{1}{2} \sum_{j,k=1}^n d_{jk} t_j t_k \right) \right) dt_1 \cdots dt_n.
$$

For, if $C$ is invertible, the quadratic form $q$ on $\mathbf{R}^n$ defined by

$$
q(x_1, \ldots, x_n) = \sum_{j,k=1}^n c_{jk} x_j x_k
$$

is nondegenerate. Using the existence of a basis of $\mathbf{R}^n$ orthonormal for $q$, one proves the existence of a square matrix $U$ of order $n$ such that $C = U \cdot {}^tU$, whence $\gamma_C = u(\gamma_{I_n})$ by (27) (where $u$ denotes the automorphism of $\mathbf{R}^n$ with matrix $U$). Let $Q$ be the quadratic form on $\mathbf{R}^n$ defined by
$$
Q(t_1, \ldots, t_n) = t_1^2 + \cdots + t_n^2;
$$
then
$$
\gamma_{I_n} = (2\pi)^{-n/2} e^{-Q/2} \cdot \lambda_n,
$$
whence
$$
u(\gamma_{I_n}) = (2\pi)^{-n/2} e^{-(Qou^{-1})/2} \cdot u(\lambda_n).
$$
It is immediate that the quadratic form $Q \circ u^{-1}$ on $\mathbf{R}^n$ takes the value $\sum_{j,k=1}^n d_{jk} t_j t_k$ at the point $(t_1, \ldots, t_n)$, and Prop. 15 of Ch. VII, §1, No. 10 shows that
$$
u(\lambda_n) = (\det U)^{-1} \cdot \lambda_n = (\det D)^{1/2} \cdot \lambda_n.
$$
Formula (28) then follows from this.

### 7. Wiener measure

In this No., we denote by $T$ the interval $]0, 1]$ of $\mathbf{R}$ and by $\mathcal{H}$ the Hilbert space of real functions on $T$ square-integrable with respect to Lebesgue measure, where the scalar product is denoted $(f|g)$. We also denote by $\mathcal{C}$ the space of continuous real functions on $T$ tending to 0 at the point 0; we equip $\mathcal{C}$ with the norm $\|f\| = \sup_{t \in T} |f(t)|$. The compact interval $[0, 1] = T \cup \{0\}$ is the Alexandroff compactification of the locally compact but noncompact interval $T$; consequently, the set of continuous functions on $T$ with compact support is dense in $\mathcal{C}$, and the dual of $\mathcal{C}$ may be identified with the space $\mathcal{M}^1$ of bounded measures (not necessarily positive) on $T$ (Ch. III, §1, No. 8, Def. 3).

For every function $f \in \mathcal{H}$, one defines a function $Pf$ on $T$ by
$$
(Pf)(t) = \int_0^t f(x) \, dx = (f|I_t),
$$
where $I_t$ is the characteristic function of the interval $]0, t]$. The Cauchy–Schwarz inequality implies the inequalities
$$
|(Pf)(t)| \leq \|f\|_2 \cdot t^{1/2}
$$
$$
|(Pf)(t) - (Pf)(t')| \leq \|f\|_2 \cdot |t - t'|^{1/2};
$$

consequently, $Pf$ belongs to $\mathcal{C}$, and the linear mapping $P$ of $\mathcal{H}$ into $\mathcal{C}$ is continuous with norm $\leqslant 1$.

Let us identify the Hilbert space $\mathcal{H}$ with its dual (TVS, V, §1, No. 7, Th. 3), and denote by $\Pi : \mathcal{M}^1 \to \mathcal{H}$ the transpose of $P : \mathcal{H} \to \mathcal{C}$. For every measure $\mu \in \mathcal{M}^1$ and every function $f \in \mathcal{H}$, we have

$$
(\Pi \mu | f) = \mu(Pf) = \int_{\mathbf{T}} d\mu(t) \int_{\mathbf{T}} I_t(x) f(x) \, dx
$$
$$
= \int_{\mathbf{T}} f(x) \, dx \int_{\mathbf{T}} I_t(x) \, d\mu(t)
$$

by the Lebesgue–Fubini theorem. Now,

$$
I_t(x) = \begin{cases}
1 & \text{if } 0 < x \leq t \leq 1 \\
0 & \text{otherwise},
\end{cases}
$$

whence finally

(34) $$ (\Pi \mu)(x) = \mu([x, 1]) \quad \text{for } x \in \mathbf{T}. $$

Let $\mu, \nu$ be in $\mathcal{M}^1$. Then

$$
(\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \Pi \mu(x) \Pi \nu(x) \, dx = \int_{\mathbf{T}} dx \int_{\mathbf{T}} I_t(x) \, d\mu(t) \int_{\mathbf{T}} I_{t'}(x) \, d\nu(t')
$$
$$
= \int_{\mathbf{T}} \int_{\mathbf{T}} d\mu(t) \, d\nu(t') \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx.
$$

Now, $I_t \cdot I_{t'}$ is the characteristic function of the interval $]0, t] \cap ]0, t']$, whence immediately

(35) $$ \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx = \inf(t, t'). $$

It follows that

(36) $$ (\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\nu(t'). $$

By the preceding result, one defines a positive quadratic form $W$ on $\mathcal{M}^1$ by the formula

(37) $$ W(\mu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\mu(t') = \| \Pi \mu \|_2^2. $$

In particular, if $t_1, \ldots, t_n$ are elements of T, and $c_1, \ldots, c_n$ are real numbers, then
$$
W \left( \sum_{j=1}^n c_j \varepsilon_{t_j} \right) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k)
$$
and since W is positive, the function $(t, t') \mapsto \inf(t, t')$ is a kernel of positive type on T.

**THEOREM 1 (Wiener).** — *Let w be the image under $P : \mathcal{H} \to \mathcal{C}$ of the canonical Gaussian promeasure on the Hilbert space $\mathcal{H}$. Then w is a Gaussian measure on $\mathcal{C}$ with variance W.*

By construction, $W(\mu) = \|^tP(\mu)\|_2^2$; Prop. 5 of No. 5 shows that w is a Gaussian promeasure with variance W. It remains to prove that w is a measure on $\mathcal{C}$.

A) *Construction of an auxiliary measured space*^{(2)} $(\Omega, m)$:
For every integer $n \geqslant 0$, denote by $D_n$ the set of numbers of the form $k/2^n$ with $k = 1, 2, 3, \ldots, 2^n$. Set $D = \bigcup_{n \geqslant 0} D_n$ (the set of dyadic numbers contained in T) and $\Omega = \mathbf{R}^D$. For every $t \in D$, denote by $X(t)$ the linear form $f \mapsto f(t)$ on $\Omega$.

For $t, t'$ in D, set $M(t, t') = \inf(t, t')$; we have seen that M is a kernel of positive type on D. Since the set D is countable, one can define the Gaussian *measure* m on $\Omega$ with covariance M (No. 6, *Example 2*).

#### Lemma 3 {#int-ix-s6-lem-3 .statement}

*For any $t, t'$ in D,
$$
\int_\Omega \left| X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2} \right|^3 dm = \frac{1}{(8\pi)^{1/2}} |t - t'|^{3/2}.
$$
Note that $\frac{t + t'}{2}$ belongs to D. One knows (No. 6, *Example 2*) that the family $(X(t))_{t \in D}$ is a basis of the topological dual $\Omega'$ of $\Omega$; therefore there exists a symmetric bilinear form $\widehat{M}$ on $\Omega' \times \Omega'$ characterized by $\widehat{M}(X(t), X(t')) = \inf(t, t')$. By construction, the variance of the Gaussian measure m on $\Omega$ is the quadratic form $\xi \mapsto \widehat{M}(\xi, \xi)$ on $\Omega'$. Set, in particular,
$$
\xi = X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2};
$$
an easy calculation yields
$$
\widehat{M}(\xi, \xi) = \frac{|t - t'|}{4}.
$$

(2) *Espace mesuré*: a locally compact space equipped with a measure (Ch. III, 1st edn., §2, No. 2, p. 52).

By Prop. 6 of No. 5 (formula (16)),

$$
\int_{\Omega} |\xi|^3 \, dm = \pi^{-1/2} 2^{3/2} \Gamma(2) \widehat{M}(\xi, \xi)^{3/2};
$$

the lemma follows immediately from formulas (40) and (41).

B) *Construction of a mapping u of $\Omega$ into $\mathcal{C}$:*
For every integer $n \geqslant 0$, denote by $E_n$ the subspace of $\mathcal{C}$ formed by the functions that are affine on each of the intervals $\left[ \frac{k-1}{2^n}, \frac{k}{2^n} \right]$ for $1 \leqslant k \leqslant 2^n$. An affine function on a compact interval I of $\mathbf{R}$ attains its bounds at the endpoints of I; consequently,

$$
\|f\| = \sup_{1 \leqslant k \leqslant 2^n} \left| f\left( \frac{k}{2^n} \right) \right|
$$

for $f \in E_n$.

For every function $g \in \Omega$ and every integer $n \geqslant 0$, there exists one and only one function $u_n(g)$ that belongs to $E_n$ and coincides with $g$ at every point of $D_n$; we shall write $T_n g = u_{n+1}(g) - u_n(g)$. Since $D_n$ is finite, the mapping $T_n$ of $\Omega$ into $\mathcal{C}$ is continuous, hence $m$-measurable.

#### Lemma 4 {#int-ix-s6-lem-4 .statement}

— *For every integer $n \geqslant 0$,*

$$
\int_{\Omega} \|T_n g\|^3 \, dm(g) \leqslant \frac{1}{(8\pi)^{1/2}} 2^{-n/2}.
$$

Let $g \in \Omega$ and $n \in \mathbf{N}$. One has $E_n \subset E_{n+1}$; consequently, the function $T_n g$ belongs to $E_{n+1}$ and is zero at every point of $D_n$; therefore, by (42),

$$
\|T_n g\|^3 = \sup_{1 \leqslant k \leqslant 2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \leqslant \sum_{k=1}^{2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3.
$$

Let us make the convention $g(0) = 0$. The construction of $u_n(g)$ by linear interpolation of $g$ implies the relations

$$
T_n g\left( \frac{2k-1}{2^{n+1}} \right) = g\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( g\left( \frac{k-1}{2^n} \right) + g\left( \frac{k}{2^n} \right) \right)
$$

for $1 \leqslant k \leqslant 2^n$. From this, one deduces, by integration,

$$
\int_{\Omega} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \, dm(g) = \int_{\Omega} \left| X\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( X\left( \frac{k-1}{2^n} \right) + X\left( \frac{k}{2^n} \right) \right) \right|^3 \, dm;
$$

![Figure 1](../images/figure_1.png)

FIGURE 1

one can then apply Lemma 3 with $t = \frac{k-1}{2^n}$, $t' = \frac{k}{2^n}$, whence

$$
\int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^{-\frac{3n}{2}} .
$$

By (44), we then have

$$
\int_{\Omega} \| T_n g \|^3 dm(g) \leq \sum_{k=1}^{2^n} \int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^n \cdot 2^{-\frac{3n}{2}} ,
$$

whence the lemma.

By Lemma 4, the mapping $T_n$ of $\Omega$ into the Banach space $\mathcal{C}$ belongs to $L^3_{\mathcal{C}}(\Omega, m)$ and $N_3(T_n) \leq \frac{1}{(8\pi)^{1/6}} (2^{-1/6})^n$, whence $\sum_{n=0}^{\infty} N_3(T_n) < +\infty$. By Prop. 6 of Ch. IV, §3, No. 3, there exists a set $\Omega_0 \subset \Omega$ such that $\Omega - \Omega_0$ is $m$-negligible and such that the series $\sum_{n=0}^{\infty} T_n(g)$ converges absolutely in $\mathcal{C}$ for every $g \in \Omega_0$. One then defines an $m$-measurable mapping $u$ of $\Omega$ into $\mathcal{C}$ by

$$
u(g) = \begin{cases}
\sum_{n=0}^{\infty} T_n g = \lim_{n \to \infty} u_n(g) & \text{for } g \in \Omega_0 \\
0 & \text{for } g \in \Omega - \Omega_0 .
\end{cases}
$$

Since $u_n(g)$ and $g$ coincide on $D_m \subset D_n$ for $0 \leq m \leq n$, it is immediate that the restriction of $u(g)$ to $D$ is equal to $g$ for every $g \in \Omega_0$.

C) Construction of a Gaussian measure on $\mathcal{C}$:
Let $w'$ be the bounded measure on $\mathcal{C}$ that is the image of $m$ under the $m$-measurable mapping $u : \Omega \to \mathcal{C}$. We are going to show that $w'$ is a Gaussian measure on $\mathcal{C}$, with variance $W$, whence $w = w'$. Denote by $\mathcal{D}$ the linear subspace of $\mathcal{M}^1$ generated by the measures $\varepsilon_t$ for $t$ running over $D$.

#### Lemma 5 {#int-ix-s6-lem-5 .statement}

For every measure $\mu \in \mathcal{D}$,

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = e^{-W(\mu)/2}.
$$

Set $\mu = c_1 \varepsilon_{t_1} + c_2 \varepsilon_{t_2} + \cdots + c_n \varepsilon_{t_n}$ with $t_1, \ldots, t_n$ in $D$ and $c_1, \ldots, c_n$ in $\mathbf{R}$. For every $g \in \Omega_0$, the function $u(g)$ coincides with $g$ on $D$; therefore

$$
\langle u(g), \mu \rangle = \sum_{j=1}^n c_j g(t_j) \qquad (g \in \Omega_0).
$$

Also,

$$
W(\mu) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k),
$$

and, since $m$ is the Gaussian measure on $\Omega$ with covariance $M$, and $\Omega - \Omega_0$ is $m$-negligible, we have

$$
\int_{\Omega_0} e^{i \sum_{j=1}^n c_j g(t_j)} \, dm(g) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k) \right).
$$

Now, $\Omega - \Omega_0$ is $m$-negligible and $w' = u(m)$; it follows that

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = \int_{\Omega_0} e^{i \langle u(g), \mu \rangle} \, dm(g).
$$

The formula (48) follows immediately from the formulas (49) to (52).

#### Lemma 6 {#int-ix-s6-lem-6 .statement}

Let $\mu \in \mathcal{M}^1$. There exists a sequence of measures $\mu_n \in \mathcal{D}$ such that $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ for all $f \in \mathcal{C}$ and $W(\mu) = \lim_{n \to \infty} W(\mu_n)$.

Let $I = [0, 1]$. The space $\mathcal{M}^1$ of bounded measures on $T = ]0, 1[$ will be identified with the subspace of $\mathcal{M}(I)$ formed by the measures that place no weight at $0$. (3) We equip $\mathcal{M}(I)$ with the vague topology. The mapping

(3) That is, the measures on $I$ that are concentrated on $T = I - \{0\}$.

$t \mapsto \varepsilon_t$ of $I$ into $\mathcal{M}(I)$ is continuous (Ch. III, §1, No. 9, Prop. 13); since D is dense in I, the closure $\overline{\mathcal{D}}$ of $\mathcal{D}$ contains all of the point measures. Let A be the set of measures $\nu \in \mathcal{D}$ such that $\| \nu \| \leq \| \mu \|$; the measure $\mu$ is in the closure of A (Ch. III, §2, No. 4, Cor. 1 of Th. 1). The set A is relatively compact in $\mathcal{M}(I)$ (Ch. III, §1, No. 9, Prop. 15) and the compact subsets of $\mathcal{M}(I)$ are metrizable (TVS, III, §3, No. 4, Cor. 2 of Prop. 6,(4) and GT, X, §3, No. 3, Th. 1). Therefore there exists a sequence of measures $\mu_n \in A$ converging to $\mu$ in $\mathcal{M}(I)$. Since $\mathcal{C}$ is identified with the subspace of continuous functions on I zero at the origin, we have $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ for all $f \in \mathcal{C}$. Moreover, since $\mathcal{C}(I) \otimes \mathcal{C}(I)$ is dense in the normed space $\mathcal{C}(I \times I)$ (Ch. III, §4, No. 1, Lemma 1), the relations $\lim_{n \to \infty} \mu_n = \mu$ and $\| \mu_n \| \leq \| \mu \|$ imply that $\lim_{n \to \infty} (\mu_n \otimes \mu_n) = \mu \otimes \mu$ (Ch. III, §1, No. 10, Prop. 17); since the measures $\mu_n$ and $\mu$ place no weight at 0, we have

$$
W(\mu_n) = \int_I \int_I \inf(t, t') d\mu_n(t) d\mu_n(t'),
$$
$$
W(\mu) = \int_I \int_I \inf(t, t') d\mu(t) d\mu(t'),
$$

whence $\lim_{n \to \infty} W(\mu_n) = W(\mu)$.

It remains to prove that the Fourier transform of $w'$ is equal to $e^{-W/2}$. Let $\mu \in \mathcal{M}^1$; choose measures $\mu_n \in \mathcal{D}$ as in Lemma 6. The measure $w'$ is bounded, and $|e^{i \langle f, \mu_n \rangle}| = 1$ for all $n$; Lemma 5 and Lebesgue's convergence theorem (Ch. IV, §4, No. 3, Th. 2) then imply

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} dw'(f) = \lim_{n \to \infty} \int_{\mathcal{C}} e^{i \langle f, \mu_n \rangle} dw'(f)
= \lim_{n \to \infty} e^{-W(\mu_n)/2} = e^{-W(\mu)/2}.
$$

Q.E.D.

The measure $w$ on $\mathcal{C}$ whose Fourier transform is equal to $e^{-W/2}$ is called the *Wiener measure on $\mathcal{C}$*.

#### Remark {#int-ix-s6-n7-rem-1 .statement}

— For every semi-open interval $J = ]a, b]$ contained in T, let us set $l(J) = b - a$ (the length of J) and denote by $A_J$ the linear form $f \mapsto f(b) - f(a)$ on $\mathcal{C}$. It can be shown that the Wiener measure is characterized by the following property:

*Let $J_1, \ldots, J_n$ be semi-open intervals contained in T and pairwise disjoint. The image of the measure w under the linear mapping $f \mapsto (A_{J_1}(f), \ldots, A_{J_n}(f))$ of $\mathcal{C}$ into $\mathbf{R}^n$ is equal to $\gamma_{a_1} \otimes \cdots \otimes \gamma_{a_n}$ with $a_i = l(J_i)^{1/2}$ for $1 \leq i \leq n$.*

### 8. Continuity of the Fourier transform

#### Proposition 8 {#int-ix-s6-prop-8 .statement}

— Let E be a locally convex space, $\mu$ a promeasure on E, and $\Phi$ the Fourier transform of $\mu$. One has the inequalities

$$
|\Phi(x')| \leq \Phi(0)
$$
$$
|\Phi(x') - \Phi(y')|^2 \leq 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right)
$$

for $x', y'$ in $E'$.

Formula (5) of No. 3 permits reducing to the case that E is finite-dimensional and $\mu$ is a measure. Then

$$
|\Phi(x')| = \left| \int_E e^{i\langle x, x' \rangle} d\mu(x) \right| \leq \int_E |e^{i\langle x, x' \rangle}| d\mu(x) = \int_E d\mu(x) = \Phi(0),
$$

whence (53). Moreover, if $a$ and $b$ are real numbers, then

$$
|e^{ia} - e^{ib}|^2 = |e^{ib}|^2|e^{i(a-b)} - 1|^2 = (e^{i(a-b)} - 1)(e^{-i(a-b)} - 1) = 2 - 2\cos(a - b);
$$

by the Cauchy–Schwarz inequality, we then have

$$
|\Phi(x') - \Phi(y')|^2 = \left| \int_E (e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}) d\mu(x) \right|^2
$$
$$
\leq \int_E |e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}|^2 d\mu(x) \int_E 1^2 d\mu(x)
$$
$$
= \int_E (2 - 2\cos\langle x, x' - y' \rangle)) d\mu(x) \cdot \Phi(0)
$$
$$
= 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right),
$$

whence (54).

#### Corollary {#int-ix-s6-n8-cor-1 .statement}

— Equip $E'$ with a topology compatible with its vector space structure. For $\Phi$ to be continuous, it is necessary and sufficient that its real part $\Re \Phi$ be continuous at the origin, in which case $\Phi$ is uniformly continuous.

This follows from the inequality (54).

Let F be a locally convex space. We equip the dual $F'$ of F with a topology compatible with the duality between F and $F'$, and we identify F with the dual of $F'$. Consequently, the Fourier transform of a bounded measure $\mu$ on $F'$ is the function $\mathcal{F}\mu$ on F defined by

$$
(\mathcal{F}\mu)(x) = \int_{F'} e^{i\langle x, x' \rangle} d\mu(x').
$$

#### Proposition 9 {#int-ix-s6-prop-9 .statement}

— *If F is barreled, then the Fourier transform of every bounded measure on F' is a uniformly continuous function on F*.

Let $\mu$ be a bounded measure on $F'$ and $\Phi$ its Fourier transform. Let $\varepsilon > 0$. There exists a compact subset K of $F'$ such that $\mu(F' - K) \leq \varepsilon$. Now, K is compact for the weak topology $\sigma(F', F)$, hence is equicontinuous because F is barreled (TVS, III, §4, No. 2, Th. 1). Therefore there exists a symmetric neighborhood U of 0 in F whose polar $U^\circ$ contains K. Let x be in $\varepsilon U$; then

$$
\Phi(0) - \Re \Phi(x) = \int_{F'} (1 - \cos \langle x, x' \rangle) d\mu(x').
$$

Now, $0 \leq 1 - \cos \langle x, x' \rangle \leq 2$ for every $x' \in F' - K$, and

$$
1 - \cos \langle x, x' \rangle \leq \frac{1}{2} \langle x, x' \rangle^2 \leq \frac{\varepsilon^2}{2}
$$

for $x' \in K \subset U^\circ$; it follows that

$$
0 \leq \Phi(0) - \Re \Phi(x) \leq 2 \mu(F' - K) + \frac{\varepsilon^2}{2} \mu(K) \leq 2\varepsilon + \frac{\varepsilon^2}{2} \mu(F').
$$

The second member of this inequality tends to 0 with $\varepsilon$; thus $\Re \Phi$ is continuous at 0 and the proposition follows from the Cor. of Prop. 8.

### 9. Minlos’s lemma

Let T be a finite-dimensional vector space and $\mu$ a bounded measure on $T'$; we shall identify T with the dual of $T'$, so that the Fourier transform $\Phi$ of $\mu$ is a function on T. We assume given two positive quadratic forms h and q on T and a number $\varepsilon > 0$. For every real number $r > 0$, we denote by $C_r$ the set of $x' \in T'$ such that $\langle x, x' \rangle^2 \leq r^2 h(x)$ for all $x \in T$.

#### Proposition 10 {#int-ix-s6-prop-10 .statement}

— *Under the hypothesis $\Phi(0) - \Re \Phi \leq \varepsilon + q$, we have*

$$
\mu(T' - C_r) \leq 3 (\varepsilon + r^{-2} \operatorname{Tr}(q/h))
$$

*for every* $r > 0$.

One writes $\operatorname{Tr}(q/h)$ for the trace of q with respect to h (cf. Annex, No. 1). The formula (55) is trivial when $\operatorname{Tr}(q/h)$ is infinite. We assume henceforth that $\operatorname{Tr}(q/h)$ is finite, hence that $h(x) = 0$ implies $q(x) = 0$ for $x \in T$.

Let $a_1, \ldots, a_n$ be elements of $T$, and $D$ the set of $x' \in T'$ such that $\sum_{j=1}^n \langle a_j, x' \rangle^2 > 1$. For every real $t \geq 0$ we have $3(1 - e^{-t/2}) \geq 0$, and we even have

$$
3(1 - e^{-t/2}) \geq 3(1 - e^{-1/2}) \geq 3\left(1 - \left(\frac{9}{4}\right)^{-1/2}\right) = 1
$$

for $t > 1$, because $e > \frac{9}{4}$. Applying these inequalities to $t = \sum_{j=1}^n \langle a_j, x' \rangle^2$, we obtain

$$
\mu(D) \leq 3 \int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x').
$$

Let $\gamma$ be the measure on $\mathbf{R}$ having density $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$ with respect to Lebesgue measure. By Lemma 2 of No. 4,

$$
\int_{\mathbf{R}} e^{iut} d\gamma(t) = e^{-u^2/2}
$$

for all real $u$. Consequently,

$$
\begin{align*}
1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right) \\
&= \int \cdots \int \left(1 - e^{i \sum_{j=1}^n \langle a_j, x' \rangle t_j}\right) d\gamma(t_1) \cdots d\gamma(t_n)
\end{align*}
$$

for all $x' \in T'$. The function of $x', t_1, \ldots, t_n$ to be integrated in the second member is continuous and is bounded above in absolute value by 2, and the measures $\mu$ and $\gamma$ are bounded; one can therefore integrate the two members of (57) with respect to $d\mu(x')$ and interchange the integrations with respect to $\mu$ and $\gamma$; one obtains

$$
\begin{align*}
\int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x') \\
&= \int \cdots \int \left(\Phi(0) - \Phi\left(\sum_{j=1}^n t_j a_j\right)\right) d\gamma(t_1) \cdots d\gamma(t_n).
\end{align*}
$$

Since $q$ is a quadratic form on $T$, there exist real numbers $q_{jk}$ such that
$$
q \left( \sum_{j=1}^n t_j a_j \right) = \sum_{j,k} q_{jk} t_j t_k
$$
for $t_1, \ldots, t_n$ real; in particular, $q_{jj} = q(a_j)$ for $1 \leq j \leq n$. Moreover, the integral $\int_{\mathbf{R}} t^n d\gamma(t)$ has the values 1, 0, 1 for $n = 0, 1, 2$, respectively (No. 4, Lemma 1). From this, one deduces immediately
$$
\int \cdots \int \left( \varepsilon + q \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n) = \varepsilon + \sum_{j=1}^n q(a_j).
$$
Now, the first member of (58) and $\Phi(0)$ are real numbers; one can therefore replace $\Phi$ by $\Re \Phi$ in the second member of (58). The inequality $\Phi(0) - \Re \Phi \leq \varepsilon + q$ and the formulas (56), (58) and (59) then imply
$$
\mu(D) \leq 3 \left( \varepsilon + \sum_{j=1}^n q(a_j) \right).
$$
Let us fix the number $r > 0$. Since the quadratic form $h$ is positive, there exist a basis $(e_1, \ldots, e_n)$ of $T$ and an integer $m$ between 0 and $n$ such that
$$
h \left( \sum_{j=1}^n t_j e_j \right) = \sum_{j=1}^m t_j^2
$$
for $t_1, \ldots, t_n$ real (Annex, No. 1, Prop. 2). It is then immediate that $C_r$ consists of the $x' \in T'$ such that
$$
\sum_{j=1}^m \langle e_j, x' \rangle^2 \leq r^2, \qquad \sum_{j=m+1}^n \langle e_j, x' \rangle^2 = 0.
$$
For every integer $l \geq 1$, let $D_l$ be the set of $x' \in T'$ satisfying the inequality
$$
\sum_{j=1}^m \langle r^{-1} e_j, x' \rangle^2 + \sum_{j=m+1}^n \langle l e_j, x' \rangle^2 > 1.
$$
One sees easily that the sequence $(D_l)_{l \geq 1}$ is increasing with union $T' - C_r$, whence
$$
\mu(T' - C_r) = \lim_{l \to \infty} \mu(D_l).
$$

But by (60),

$$
\mu(D_l) \leq 3 \left( \varepsilon + \sum_{j=1}^m r^{-2} q(e_j) + \sum_{j=m+1}^n l^2 q(e_j) \right);
$$

for $j = m+1, \ldots, n$ we have $h(e_j) = 0$, therefore $q(e_j) = 0$. Moreover, $\operatorname{Tr}(q/h) = \sum_{j=1}^m q(e_j)$ (Annex, No. 1, Prop. 2). The relation (55) then follows from (61) and (62).

Q.E.D.

### 10. Measures on the dual of a nuclear space

Let F be a locally convex space. Let $\mathcal{T}_s$ be the weak topology $\sigma(F', F)$ on $F'$, and $\mathcal{T}_c$ the topology of uniform convergence on the compact convex subsets of F. By Mackey’s theorem (TVS, IV, §1, No. 1, Th. 1) the topologies $\mathcal{T}_s$ and $\mathcal{T}_c$ on $F'$ are compatible with the duality between F and $F'$; the same is therefore true of every locally convex topology $\mathcal{T}$ on $F'$ intermediate to $\mathcal{T}_s$ and $\mathcal{T}_c$. If $\mathcal{T}$ is such a topology, and $F'_{\mathcal{T}}$ denotes the space $F'$ equipped with $\mathcal{T}$, we shall identify F with the dual of $F'_{\mathcal{T}}$. The promeasures on $F'$ are therefore the same for all topologies $\mathcal{T}$ of the preceding type, and if $\mu$ is such a promeasure then its Fourier transform is a function on F.

One calls Sazonov’s topology on F the locally convex topology $\mathcal{S}$ defined by the continuous seminorms N satisfying the following condition: $N^2$ is a positive quadratic form on F and there exists a continuous positive quadratic form H on F such that $\operatorname{Tr}(N^2/H) < +\infty$. The topology $\mathcal{S}$ is coarser than the given topology on F; if these topologies are identical, F is said to be nuclear. This class of spaces will be studied in detail later on.

#### Theorem 2 (Minlos) {#int-ix-s6-thm-2 .statement}

— *Let F be a locally convex space, $\mathcal{T}$ a locally convex topology on $F'$ intermediate to $\mathcal{T}_s$ and $\mathcal{T}_c$, and $\mu$ a promeasure on $F'_{\mathcal{T}}$. Assume that the Fourier transform $\Phi$ of $\mu$ is continuous on F for the Sazonov topology. Then $\mu$ is a measure on $F'_{\mathcal{T}}$.*

Let $\varepsilon > 0$. Since $\Phi$ is continuous for the Sazonov topology on F, there exist two continuous positive quadratic forms Q and H on F such that $\operatorname{Tr}(Q/H) < +\infty$ and

$$
\Phi(0) - \mathcal{R}\Phi(x) \leq \varepsilon/6
$$

for every $x \in F$ such that $Q(x) \leq 1$. By Prop. 8 of No. 8, $|\mathcal{R}\Phi(x)| \leq \Phi(0)$ for all $x \in F$, whence

$$
\Phi(0) - \mathcal{R}\Phi(x) \leq \varepsilon/6 + 2\Phi(0)Q(x)
$$

for all $x \in F$.

Set $r = (12\Phi(0)\operatorname{Tr}(Q/H)\varepsilon^{-1})^{1/2}$ and denote by K the set of $x' \in F'_\mathcal{T}$ such that $\langle x, x' \rangle^2 \leq r^2 H(x)$ for all $x \in F$. Since $H^{1/2}$ is a continuous seminorm on $F$, the set K is equicontinuous and closed in $F'_\mathcal{T}$; it is therefore compact in $F'_\mathcal{T}$ by Ascoli’s theorem (GT, X, §2, No. 5, Cor. 1 of Th. 2).

Let V be a closed linear subspace of $F'_\mathcal{T}$ with finite codimension; then, V is the orthogonal of a finite-dimensional linear subspace T of F. Let $\mu_V$ be the measure on $T'$ that is the image of the promeasure $\mu$ on $F'_\mathcal{T}$ under the mapping $p_V$ that is the transpose of the canonical injection of T into F; its Fourier transform is the restriction of $\Phi$ to T. Finally, by the Hahn–Banach theorem (TVS, II, §3, No. 2, Cor. 1 of Th. 1), $p_V(K)$ is equal to the set $C_r$ of $x' \in T'$ such that $\langle x, x' \rangle^2 \leq r^2 H(x)$ for all $x \in T$. By the inequality (63), one can apply Prop. 10 of No. 9 to the measure $\mu_V$ on $T'$, on taking for q the restriction of $2\Phi(0)Q$ to T and for h that of H. Then $\operatorname{Tr}(q/h) \leq 2\Phi(0)\operatorname{Tr}Q/H)$, whence

$$
\mu_V(T' - C_r) \leq 3 \left( \frac{\varepsilon}{6} + 2\Phi(0)\operatorname{Tr}(Q/H)\,r^{-2} \right) = \varepsilon.
$$

Since $p_V$ defines, by passage to the quotient, an isomorphism of $F'_\mathcal{T}/V$ onto $T'$, Prop. 1 of No. 1 then shows that $\mu$ is a measure on $F'_\mathcal{T}$.

Q.E.D.

#### Corollary {#int-ix-s6-n10-cor-1 .statement}

— *Let F be a barreled nuclear space, $\mathcal{T}$ a locally convex topology on $F'$ intermediate to $\mathcal{T}_s$ and $\mathcal{T}_c$, $\mu$ a promeasure on $F'_\mathcal{T}$, and $\Phi$ the Fourier transform of $\mu$. For $\mu$ to be a measure, it is necessary and sufficient that $\Phi$ be continuous on F.*

Necessity follows from Prop. 9 of No. 8 and sufficiency from Th. 2.

#### Remark {#int-ix-s6-n10-rem-1 .statement}

— Let F be a barreled space and $\mathcal{T}$ a locally convex topology on $F'$ intermediate to $\mathcal{T}_s$ and $\mathcal{T}_c$. Every subset of $F'$ compact for $\mathcal{T}$ is compact for the coarser topology $\mathcal{T}_s$. Conversely, let K be a subset of $F'$ compact for $\mathcal{T}_s$. Since F is barreled, K is equicontinuous (TVS, III, §4, No. 2, Th. 1); but by Ascoli’s theorem, every equicontinuous subset of $F'$ is relatively compact for $\mathcal{T}_c$ and *a fortiori* for $\mathcal{T}$, therefore K is contained in a subset of $F'$ compact for $\mathcal{T}$. It is not difficult to infer from this that the identity mapping of $F'_\mathcal{T}$ onto $F'_{\mathcal{T}_s}$ defines a bijection between the sets of measures on these two spaces.

### 11. Measures on a Hilbert space

Let E be a real Hilbert space, in which the scalar product is denoted $(x|y)$. There exists an isomorphism j of E onto its dual $E'$, characterized by the formula $\langle x, j(y) \rangle = (x|y)$ for $x, y$ in E (TVS, V, §1, No. 7, Th. 3). We will identify E and $E'$ by means of j. The Fourier transform of a promeasure $\mu$ on E is therefore a function $\mathscr{F}\mu$ on E; when $\mu$ is a measure, we have

$$(64)$$
$$(\mathcal{F}\mu)(x) = \int_{E} e^{i(x|y)} d\mu(y) \quad (x \in E).$$

**Theorem 3** (Prokhorov–Sazonov) — *Let E be a Hilbert space and Es the space E equipped with the weakened topology. Let μ be a promeasure on E, and Φ its Fourier transform. The following conditions are equivalent*:

a) *The function Φ is continuous on E for the Sazonov topology*.

b) *For every ε > 0, there exists a nuclear positive quadratic form Q on E such that Φ(0) − $\Re \Phi$ ≤ ε + Q*.

c) *The promeasure μ is a measure on Es*.

$b) \Rightarrow a)$: This follows from Prop. 8 of No. 8 (cf. the inequality (54)).

$a) \Rightarrow c)$: This follows from Theorem 2 of No. 10.

$c) \Rightarrow b)$: Suppose that μ is a measure on Es. Let ε > 0. For every integer $n \geq 1$, the set $B_n$ of $x \in E$ with norm $\leq n$ is a closed subset of $E_s$, and $E = \bigcup_{n \geq 1} B_n$. Therefore there exists an integer $n \geq 1$ such that $\mu(E - B_n) < \frac{\varepsilon}{2}$. The formula

$$(65)$$
$$ Q(x) = \frac{1}{2} \int_{B_n} (x|y)^2 d\mu(y) $$

defines a positive quadratic form Q on E. Set $C = \frac{n^2}{2} \mu(B_n)$. If $(e_1, \ldots, e_p)$ is a finite orthonormal sequence in E, then

$$
\sum_{j=1}^p (e_j|y)^2 \leq \|y\|^2 \leq n^2
$$

for every $y \in B_n$ by Bessel’s inequality. It follows by integration that

$$
\sum_{j=1}^p Q(e_j) = \frac{1}{2} \int_{B_n} \sum_{j=1}^p (e_j|y)^2 d\mu(y) \leq \frac{n^2}{2} \mu(B_n) = C,
$$

therefore Q is nuclear.

Moreover, $1 - \cos t \leq \inf \left( 2, \frac{t^2}{2} \right)$ for every real number t, whence

$$
\Phi(0) - \Re \Phi(x) = \int_{E} (1 - \cos(x|y)) d\mu(y)
$$
$$
\leq \int_{B_n} \frac{1}{2}(x|y)^2 d\mu(y) + \int_{E - B_n} 2 \cdot d\mu(y)
$$
$$
< Q(x) + \varepsilon
$$

for all $x \in E$. Thus $b)$ is verified.

Q.E.D.

#### Corollary 1 {#int-ix-s6-thm-2-cor-1 .statement}

— *Let $E_1$ and $E_2$ be two Hilbert spaces, $u$ a Hilbert–Schmidt mapping of $E_1$ into $E_2$, and $\mu$ a promeasure on $E_1$. Assume that the Fourier transform $\Phi$ of $\mu$ is continuous on $E_1$. Then the promeasure $\nu = u(\mu)$ is a measure on $E_2$ equipped with the weak topology.*

With the identifications of $E_1$ and $E_2$ with their duals introduced in this No., the Fourier transform of $\nu$ is equal to $\Phi \circ u^*$, where $u^*$ is the adjoint of $u$. Now, $u^*$ is a Hilbert–Schmidt mapping of $E_2$ into $E_1$ (Annex, No. 2), and the quadratic form $y \mapsto \|u^*(y)\|^2$ on $E_2$ is therefore nuclear. If $(E_2)_\mathscr{S}$ denotes $E_2$ equipped with the Sazonov topology, $u^*$ is therefore a continuous linear mapping of $(E_2)_\mathscr{S}$ into $E_1$, and $\mathcal{F}_V = \Phi \circ u^*$ is continuous on $(E_2)_\mathscr{S}$; Theorem 3 then shows that $\nu$ is a measure on the space $E_2$ equipped with the weak topology.

#### Corollary 2 {#int-ix-s6-thm-2-cor-2 .statement}

— *Let $Q$ be a nuclear positive quadratic form on the Hilbert space $E$. The Gaussian promeasure $\Gamma_Q$ on $E$ with variance $Q$ is a measure on $E_s$.*

The Fourier transform $\Phi$ of $\Gamma_Q$ is equal to $e^{-Q/2}$. Now, $e^t \geq 1 + t$ for every real number $t$, whence $\Phi(0) - \Re \Phi \leq Q/2$. The condition $b)$ of Theorem 3 is therefore verified and $\Gamma_Q$ is a measure on $E_s$.

#### Remark {#int-ix-s6-n11-rem-1 .statement}

— 1) Let $E$ be a Hilbert space, $E_s$ the space $E$ equipped with the weak topology, and $j$ the identity mapping of $E$ into $E_s$. One knows that $j$ defines a bijection of the set of promeasures on $E$ onto the corresponding set for $E_s$. Moreover, if $E$ is separable, it is a Polish space and $j$ defines a bijection of the set of bounded measures on $E$ onto the set of bounded measures on $E_s$ (\S 3, No. 3, *Remark*); it can be shown (the theorem of Phillips) that this theorem still holds if $E$ is not separable. Consequently, Theorem 3 furnishes criteria for a promeasure on $E$ to be a measure.

2) One can show (Annex, Exer. 7) that the Sazonov topology on a Hilbert space $E$ is defined by the semi-norms of the type $Q^{1/2}$ where $Q$ is a *nuclear* positive quadratic form on $E$.

*12. Relations with functions of positive type*

#### Definition 3 {#int-ix-s6-def-3 .statement}

— *Let $G$ be a group. A complex-valued function $\Phi$ on $G$ is said to be of positive type if the inequality*

$$
\sum_{j,k=1}^p c_j \overline{c_k} \Phi(x_j x_k^{-1}) \geq 0
$$

*holds for any* $x_1, \ldots, x_p$ *in* $G$ *and any complex numbers* $c_1, \ldots, c_p$.

This concept will be studied in detail later on.

#### Proposition 11 {#int-ix-s6-prop-11 .statement}

— Let E be a finite-dimensional vector space, $\mu$ a bounded (positive) measure on E, and $\Phi$ the Fourier transform of $\mu$. The function $\Phi$ is continuous and of positive type on $E'$.

The continuity of $\Phi$ follows from Prop. 9 of No. 8.

Let us show that $\Phi$ is of positive type. Let $x'_1, \ldots, x'_p$ be in $E'$ and $c_1, \ldots, c_p$ complex numbers. Then

$$
\sum_{j,k} c_j \overline{c_k} \Phi(x'_j - x'_k) = \int_E \sum_{j,k} c_j \overline{c_k} e^{i \langle x, x'_j - x'_k \rangle} \, d\mu(x)
$$
$$
= \int_E \left| \sum_{j=1}^p c_j e^{i \langle x, x'_j \rangle} \right|^2 \, d\mu(x) \geq 0.
$$

Q.E.D.

One can prove a converse known as *Bochner's theorem*: every continuous function on $E'$ of positive type is the Fourier transform of a bounded (positive) measure. (*) We shall assume this result for the rest of No. 12.

#### Theorem 4 {#int-ix-s6-thm-4 .statement}

— Let E be a locally convex space. The Fourier transformation is a bijection of the set of promeasures on E onto the set of functions of positive type on $E'$ whose restriction to every finite-dimensional subspace is continuous.

We know (No. 3, Prop. 3) that the Fourier transformation is injective. Let $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ be a promeasure on E and $\Phi$ its Fourier transform. Let T be a finite-dimensional subspace of $E'$ and let V be the orthogonal of T in E. One can identify T with the dual of $E/V$; the restriction $\Phi_T$ of $\Phi$ to T is the Fourier transform of the bounded measure $\mu_V$ on $E/V$. By Prop. 11, $\Phi_T$ is continuous and of positive type on T. Since T is arbitrary, it is clear that $\Phi$ is of positive type on $E'$.

Conversely, let $\Phi$ be a function of positive type on $E'$ whose restriction to every finite-dimensional subspace of $E'$ is continuous. For every $V \in \mathcal{F}(E)$, we identify the dual of $E/V$ with the orthogonal $V^\circ$ of V in $E'$; the restriction $\Phi_V$ of $\Phi$ to $V^\circ$ is continuous and of positive type and so, by Bochner's theorem, there exists a bounded (positive) measure $\mu_V$ on $E/V$ whose Fourier transform is $\Phi_V$. Let V and W in $\mathcal{F}(E)$ be such that $W \subset V$, and let $p_{VW}$ be the canonical mapping of $E/W$ onto $E/V$; with the identifications made, ${}^t p_{VW}$ is the injection of $V^\circ$ into $W^\circ$. By formula (4) of No. 3, we then have

$$
\mathcal{F}(p_{VW}(\mu_W)) = (\mathcal{F}\mu_W) \circ {}^t p_{VW} = \Phi_W \circ {}^t p_{VW} = \Phi_V = \mathcal{F}\mu_V,
$$

(*) This question will be studied in a forthcoming chapter of the Book *Théories spectrales*. The reader may consult for this subject the book of L.H. LOOMIS, *Abstract harmonic analysis*, Van Nostrand, New York, 1953.

whence $pvw(\mu_w) = \mu_v$ by Prop. 3 of No. 3. Consequently, the family $\mu = (\mu_v)_{v \in \mathscr{F}(E)}$ is a promeasure on $E$; it is clear that $\Phi$ is the Fourier transform of $\mu$.

#### Corollary {#int-ix-s6-n11-cor-1 .statement}

— *Let F be a barreled nuclear space; equip F' with a locally convex topology $\mathcal{T}$ intermediate to the weak topology $\sigma(F', F)$ and the topology of uniform convergence on the compact convex subsets of F. The Fourier transformation is a bijection of the set of bounded (positive) measures on F' onto the set of continuous functions of positive type on F.*

This follows immediately from Theorem 4 and the Cor. of Th. 2 of No. 10.*

### Exercises {#int-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
