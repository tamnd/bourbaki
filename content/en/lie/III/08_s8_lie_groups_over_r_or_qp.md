---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 8
section_title: Lie groups over R or Qp
lang: en
source: lie-i-iii
pdf_pages: 0355-0360, 0413-0415
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS MORPHISMS
      page: 0
      pdf_page: 355
    - "no": 2
      title: CLOSED SUBGROUPS
      page: 0
      pdf_page: 358
statements: 9
exercises: 7
content_sha256: d48cff3608394e0ece5f613b8605904b3d3dfbf75e89fa6fec2532a22ecc23fc
---

## § 8. LIE GROUPS OVER $\mathbf{R}$ AND $\mathbf{Q}_p$

### 1. CONTINUOUS MORPHISMS

#### Theorem 1 {#lie-iii-s8-thm-1 .statement}

*Let G and H be two Lie group germs over $\mathbf{R}$ or $\mathbf{Q}_p$. Let f be a continuous morphism of G into H. Then f is analytic.*

We give $L(G)$ and $L(H)$ norms which define their topologies and such that $\| [x, y] \| \leq \|x\| \|y\|$ for all $x, y$. There exist an open ball V of centre 0 in $L(G)$ and an exponential mapping $\phi$ of G defined on V such that: (1) $\phi(V)$ is an open neighbourhood of $e$ in G; (2) $\phi$ is an isomorphism of the analytic manifold V onto the analytic manifold $\phi(V)$; (3) $\phi(nx) = \phi(x)^n$ for all $x \in V$ and all $n \in \mathbf{Z}$ such that $nx \in V$. We define similarly W and $\psi$ for H. By shrinking V if necessary, it can be assumed that $f(\phi(V)) \subset \psi(W)$. Then $g = \psi^{-1} \circ f \circ \phi$ is a continuous mapping of V into W.

We show that
$$
(x \in V, \lambda \in \mathbf{Q} \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
It can be assumed that $\lambda \neq 0$. Let $\lambda = \frac{r}{q}$ with $r, q$ in $\mathbf{Z} - \{0\}$. Let $y = \frac{r}{q} x$.

If $K = \mathbf{R}$, we write $z = \frac{x}{q} = \frac{y}{r} \in V$. Then $x = qz, y = rz$, whence
$$
g(x) = \psi^{-1}(f(\phi(qz))) = \psi^{-1}(f(\phi(z)^q)) = \psi^{-1}(f(\phi(z))^q).
$$
We show that $\psi^{-1}(f(\phi(z))^q) = q \psi^{-1}(f(\phi(z))) = qg(z)$. It suffices to verify that, if $u \in \psi(W)$ is such that $u^q \in \psi(W)$, then $\psi^{-1}(u^q) = q \psi^{-1}(u)$; but if $u = \psi(v)$, $u^q = \psi(v^q)$, then $v^1/q \in W$ and $(\psi(v^1/q))^q = u^q$, hence $\psi(v^1/q) = u = \psi(v)$ and therefore $v^1 = qv$.

Similarly, $g(y) = rg(z)$, whence (1).

If $K = \mathbf{Q}_p$, we write $z = rx = qy \in V$, whence $g(z) = rg(x) = qg(y)$, whence again (1).

As $\mathbf{Q}$ is dense in $K$, (1) implies that
$$
(x \in V, \lambda \in K \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
Let $x \in L(G)$ and $\lambda, \lambda'$ be elements of $K^*$ such that $\lambda x \in V, \lambda' x \in V$. Then
$$
g(\lambda' x) = g\left( \frac{\lambda'}{\lambda} \lambda x \right) = \frac{\lambda'}{\lambda} g(\lambda x)
$$
by (2) and hence $\frac{1}{\lambda} g(\lambda x) = \frac{1}{\lambda'} g(\lambda' x)$. Thus an extension $h$ of $g$ to $L(G)$ is defined by writing $h(x) = \frac{1}{\lambda} g(\lambda x)$ for all $\lambda$ such that $\lambda x \in V$. Clearly $h$ is continuous. We show that
$$
(x \in L(G) \text{ and } \lambda \in K) \Rightarrow h(\lambda x) = \lambda h(x).
$$
Let $\lambda' \in K^*$ be such that $\lambda' x \in V$ and $\lambda' \lambda x \in V$. Then
$$
h(\lambda x) = \frac{1}{\lambda'} g(\lambda' \lambda x) = \frac{1}{\lambda'} \lambda g(\lambda' x) = \lambda \frac{1}{\lambda'} g(\lambda' x) = \lambda h(x).
$$
Let $x, y$ be in $L(G)$. Then, by Proposition 4 of § 4, no. 3,
$$
\begin{align*}
h(x) + h(y) &= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(\lambda h(x)) \psi(\lambda h(y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(h(\lambda x)) \psi(h(\lambda y))).
\end{align*}
$$
For $|\lambda|$ sufficiently small, $\lambda x \in V$ and $\lambda y \in V$ and hence the above expression is equal to
$$
\begin{align*}
&\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(f(\phi(\lambda x)) f(\phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} (\psi^{-1} \circ f)(\phi(\lambda x) \phi(\lambda y)) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} g(\phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} h(\lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(x + y).
\end{align*}
$$
Thus $h$ is continuous and linear, hence $g = h|V$ is analytic, hence $f$ is analytic on $\phi(V)$ and hence $f$ is analytic (\S 1, no. 10).

#### Corollary 1 {#lie-iii-s8-thm-1-cor-1 .statement}

Let $G$ be a topological group. There exists on $G$ at most one analytic manifold structure over $\mathbf{R}$ (resp. $\mathbf{Q}_p$) compatible with the topological group structure on $G$.

This follows immediately from Theorem 1.

#### Definition 1 {#lie-iii-s8-def-1 .statement}

*A topological group G is called a real (resp. p-adic) Lie group if there exists on G a real (resp. p-adic) Lie group structure compatible with its topology.*

That structure is then unique and we can speak of the *dimension* of such a group. If G and H are two such groups, every continuous morphism of G into H is analytic.

#### Corollary 2 {#lie-iii-s8-def-1-cor-2 .statement}

*Let G be a topological group and V an open neighbourhood of e. Suppose that V has an analytic manifold structure which makes it into a real (resp. p-adic) Lie group germ. Then G is a real (resp. p-adic) Lie group.*

Let $g \in G$. There exists an open neighbourhood $V'$ of $e$ in G such that $V' \cup gV'g^{-1} \subset V$. The mapping $v \mapsto gv g^{-1}$ of $V'$ into $V$ is a continuous and hence analytic morphism of the Lie group germ $V'$ into the Lie group germ $V$. It then suffices to apply Proposition 18 of § 1, no. 9.

#### Remark {#lie-iii-s8-n1-rem-1 .statement}

(1) Theorem 1 and its corollaries are no longer true if $\mathbf{R}$ (resp. $\mathbf{Q}_p$) is replaced by $\mathbf{C}$ (Exercise 1).

(2) Let G be a topological group. It can be shown† that the following conditions are equivalent: (a) G is a finite-dimensional real Lie group; (b) G is locally compact and there exists a neighbourhood of $e$ containing no subgroup distinct from $\{e\}$; (c) there exists an open neighbourhood of $e$ homeomorphic to an open ball of a space $\mathbf{R}^n$. (For a much less difficult result, cf. Exercise 6.)

#### Proposition 1 {#lie-iii-s8-prop-1 .statement}

*Let G, G' be topological groups and f a continuous morphism of G into G'. Suppose that one of the following three cases holds:
(a) G is a real Lie group and G' is a p-adic Lie group;
(b) G is a p-adic Lie group and G' is a real Lie group;
(c) G is a p-adic Lie group and G' is a $p'$-adic Lie group with $p \neq p'$.
Then f is locally constant.*

Case (a). Let $G_0$ be the identity component of G. Then $f(G_0)$ is a connected subgroup of $G'$ and hence $f(G_0) = \{e\}$ and $G_0$ is open in G.

Case (b). Let $V'$ be a neighbourhood of $e$ in $G'$ such that every subgroup of $G'$ contained in $V'$ reduces to $\{e\}$ (\S 4, no. 2, Corollary 1 to Theorem 2). There exists a neighbourhood V of $e$ in G such that $f(V) \subset V'$. Then there exists an open subgroup $G_1$ of G such that $G_1 \subset V$ (\S 7, no. 1, Proposition 1). Then $f(G_1) = \{e\}$.

Case (c). By \S 7, Theorem 4 and the Corollary to Proposition 8, there exists a neighbourhood $V'$ of $e$ in $G'$ such that, for all $x' \in V' - \{e\}$, ${x'}^{p^n}$ does not tend

† See for example D. Montgomery and L. Zippin, *Topological transformation groups*, Interscience tracts in pure and applied mathematics, no. 1, Interscience publishers, New York 1955 (in particular pp. 169 and 184).

to $e$ as $n$ tends to $+\infty$. There exists a neighbourhood $V$ of $e$ in $G$ such that $f(V) \subset V'$. By § 7, Theorem 4 and Proposition 9, there exists an open subgroup $G_1$ of $G$ such that $G_1 \subset V$ and such that, for all $x \in G_1$, $x^{p^n}$ tends to $e$ as $n$ tends to $+\infty$. Then $f(G_1) = \{e\}$.

### 2. CLOSED SUBGROUPS

#### Theorem 2 {#lie-iii-s8-thm-2 .statement}

*Let $G$ be a finite-dimensional Lie group over $\mathbf{R}$ or $\mathbf{Q}_p$. Every closed subgroup of $G$ is a Lie subgroup of $G$. More generally, let $U$ be a symmetric open neighbourhood of $e$ in $G$ and $H$ a non-empty closed subspace of $U$ such that the conditions $x \in H$, $y \in H$ and $xy^{-1} \in U$ imply $xy^{-1} \in H$. Then $H$ is a Lie subgroup germ of $G$.*

Let $\mathfrak{h}$ be the Lie subalgebra tangent to $H$ at $e$ (\S 4, no. 5, Definition 2). There exists a Lie subgroup germ $H_0$ of $G$ with Lie algebra $\mathfrak{h}$ and contained in $H$. We prove that $H_0$ is open in $H$ with the topology induced by that on $G$. This will prove that $H$ is an analytic submanifold of $G$ and will establish the theorem.

There exist a vector subspace $\mathfrak{k}$ supplementary to $\mathfrak{h}$ in $L(G)$, symmetric open neighbourhoods $V_1, V_2$ of zero in $\mathfrak{h}$ and $\mathfrak{k}$ respectively and an exponential mapping $\phi$ of $G$ defined on $V_1 + V_2$ and possessing the following properties:

(a) the mapping $(a_1, a_2) \mapsto \phi(a_1)\phi(a_2)$ is an analytic isomorphism of $V_1 \times V_2$ onto an open subset $V$ of $G$;
(b) $\phi(V_1) \subset H_0$;
(c) $V^2 \subset U$.

We shall prove (and this will achieve the proof) that there exists an open neighbourhood $V'_2$ of 0 in $V_2$ such that $H \cap (\phi(V_1)\phi(V'_2)) = \phi(V_1)$.

Suppose that the assertion is false. Then we can find a sequence $(x_n)$ in $V_1$ and a sequence $(y_n)$ in $V_2 - \{0\}$ tending to 0, such that $\phi(x_n)\phi(y_n) \in H$ for all $n$. Then $\phi(y_n) \in H$ by (c).

If $K = \mathbf{Q}_p$, it can be assumed that $V_2$ is an additive subgroup of $\mathfrak{k}$ and that $\phi(pa) = \phi(a)^p$ for all $a \in V_2$ and all $p \in \mathbf{Z}$. Then $\phi(\lambda y_1) \in H$ for all $\lambda \in \mathbf{Z}$ and hence by continuity for all $\lambda \in \mathbf{Z}_p$. The mapping $f : \lambda \mapsto \phi(\lambda y_1)$ of $\mathbf{Z}_p$ into $G$ is analytic and takes its values in $H$ and $(T_0f)(1) = y_1$. Hence $y_1 \in \mathfrak{h}$, which is absurd. The theorem is therefore established in the case of $\mathbf{Q}_p$.

If $K = \mathbf{R}$, it can be assumed that $V_2$ is connected and that $y_n$ belongs to $\frac{1}{2}V_2 - \{0\}$. By taking a subsequence of $(y_n)$ if necessary, we can find a sequence $(\lambda_n)$ of non-zero scalars such that $\lambda_n^{-1}y_n$ tends to an element $y$ of $V_2 - \{0\}$. The sequence $(\lambda_n)$ tends to 0. Let $\lambda \in \mathbf{R}$ be such that $\lambda y \in \frac{1}{2}V_2$; we prove that $\exp(\lambda y) \in H$. It can be assumed that $\lambda \lambda_n^{-1}y_n \in \frac{1}{2}V_2$ for all $n$. Let $k_n \in \mathbf{Z}$ be such that $|\lambda - k_n \lambda_n|$ tends to 0. For $n$ sufficiently large, $(\lambda - k_n \lambda_n)\lambda_n^{-1}y_n \in \frac{1}{2}V_2$ and hence $k_n y_n \in \frac{1}{2}V_2$. Hence $\exp(h y_n) \in H$ for $h$ an integer and $0 \leq |h| \leq |k_n|$ (as is seen by induction on $|h|$). Then
$$
\exp(\lambda y) = \lim_{n \to \infty} \exp(\lambda \lambda_n^{-1}y_n) = \lim_{n \to \infty} (\exp((\lambda - k_n \lambda_n)\lambda_n^{-1}y_n) \exp(k_n y_n))
= \lim_{n \to \infty} \exp k_n y_n \in H.
$$

Hence the mapping $f : \lambda \mapsto \exp \lambda y$, where $\lambda y \in \frac{1}{4}V_2$, takes its values in $H$ and $(T_0f)(1) = y$. Hence $y \in \mathfrak{h}$, which is absurd. The theorem is thus established in the case of $\mathbf{R}$.

Theorem 2 is no longer true if $G$ is not assumed to be finite-dimensional (Exercise 12).

#### Corollary 1 {#lie-iii-s8-thm-2-cor-1 .statement}

*Let $G'$ be a locally compact group, $G$ a finite-dimensional Lie group over $\mathbf{R}$ (resp. $\mathbf{Q}_p$) and $f$ a continuous morphism of $G'$ into $G$. If the kernel of $f$ is discrete, $G'$ is a finite-dimensional real (resp. $p$-adic) Lie group.*

There exists a compact neighbourhood $V$ of $e$ in $G'$ such that $f|V$ is a homeomorphism of $V$ onto a compact subspace of $G$. If $U$ is a sufficiently small open neighbourhood of $e$ in $G$, the hypotheses of Theorem 2 are satisfied with $H = f(V) \cap U$. Hence $H$ is a Lie subgroup germ of $G$. Let $W$ be the inverse image of $H$ under $f|V$. Then $W$ is a neighbourhood of $e$ in $G'$. Let $W$ be given the analytic manifold structure transported from that on $H$ by $(f|W)^{-1}$. For all $z \in G'$, the mapping $x \mapsto f(z)x f(z)^{-1}$ of $G$ into $G$ is analytic; hence there exists an open neighbourhood $W'$ of $e$ in $W$ such that the mapping $x' \mapsto zx'z^{-1}$ of $W'$ into $W$ is analytic. By Proposition 18 of § 1, no. 9, there exists on $G'$ a Lie group structure which induces on a sufficiently small open neighbourhood of $e$ the same analytic structure as $W$ and hence the same topology as the initial topology on $G'$.

#### Corollary 2 {#lie-iii-s8-thm-2-cor-2 .statement}

*Let $G$ be a finite-dimensional Lie group over $K$, $H$ a subgroup of $G$, $V$ an open neighbourhood of $e$ in $G$ and $(M_i)_{i \in I}$ a family of analytic manifolds over $K$; for all $i \in I$, let $f_i$ be a $K$-analytic mapping of $V$ into $M_i$ such that*

$$
H \cap V = \{ x \in V \mid f_i(x) = f_i(e) \text{ for all } i \in I \}.
$$

(i) *If $K = \mathbf{C}$, $H$ is a Lie subgroup of $G$.*
(ii) *If $K$ is a finite extension of $\mathbf{Q}_p$ and $I$ is finite, $H$ is a Lie subgroup of $G$.*

(i) Suppose that $K = \mathbf{C}$. We consider $G$ as a real Lie group. Then $H$ is a real Lie subgroup of $G$ (Theorem 2). Let $a \in L(H)$. There exists a connected open neighbourhood $W$ of $0$ in $\mathbf{C}$ such that $\exp \lambda a \in V$ for all $\lambda \in W$. Let $i \in I$. Then $f_i(\exp \lambda a) = f_i(e)$ if $\lambda \in \mathbf{R} \cap W$. Hence $f_i(\exp \lambda a) = f_i(e)$ if $\lambda \in W$ by analytic continuation. Thus, $\exp \lambda a \in H$ for $\lambda \in W$ and therefore $\mu a \in L(H)$ for all $\mu \in \mathbf{C}$. Therefore $H$ is a Lie subgroup of the complex Lie group $G$ (\S 4, no. 2, Proposition 2).

(ii) Suppose that $K$ is a finite extension of $\mathbf{Q}_p$. We consider $G$ as a Lie group over $\mathbf{Q}_p$. It is finite-dimensional and Theorem 2 implies that $H$ is a $p$-adic Lie subgroup of $G$. Since $I$ is finite, $\prod_{i \in I} M_i$ is a manifold and it can be assumed that the family $(f_i)$ reduces to a single mapping $f$. Let $a \in L(G)$. Let $\phi$ be an exponential mapping of $G$. Then $f(\phi(\lambda a)) = f(e)$ for $\lambda \in \mathbf{Q}_p$ and $|\lambda|$ sufficiently small. Since $f$ is K-analytic, it follows that $f(\phi(\lambda a)) = f(e)$ for $\lambda \in K$ and $|\lambda|$ sufficiently small. Hence $\phi(\lambda a) \in H$ for $\lambda \in K$ and $|\lambda|$ sufficiently small and therefore $\mu a \in L(H)$ for all $\mu \in K$. The proof is completed as in (i).

Corollary 2 (ii) is no longer true if we omit the hypothesis that I is finite.

### Exercises {#lie-iii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
