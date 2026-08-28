---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 3
section_title: Applications and examples
lang: en
source: int-vii-ix
book_pages: INT VII.53-INT VII.73, INT VII.91-INT VII.94
pdf_pages: 0059-0079, 0097-0100
extraction: ocr
subsections:
    - "no": 1
      title: Compact groups of linear mappings
      page: 53
      pdf_page: 59
    - "no": 2
      title: Triviality of fibered spaces and of group extensions
      page: 55
      pdf_page: 61
    - "no": 3
      title: Examples
      page: 60
      pdf_page: 66
statements: 24
exercises: 12
content_sha256: 078f19722008dfae813e659f6b11ae7131834f184493c91a7d14517868b1259e
---

## § 3. APPLICATIONS AND EXAMPLES

### 1. Compact groups of linear mappings

Let $E$ be a finite-dimensional vector space over $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$. Then $\mathrm{End}(E)$ is a finite-dimensional algebra over $\mathbf{R}$, and the canonical topology on $\mathrm{End}(E)$ (\S 1, No. 10) is the topology of compact convergence. The group $\mathrm{Aut}(E) = \mathbf{GL}(E)$ is an open subset of $\mathrm{End}(E)$, hence is a locally compact group. Let $(e_1, e_2, \ldots, e_n)$ be a basis of $E$ and, for every endomorphism $u$ of $E$, let $M(u) = (\alpha_{ij}(u))$ be the matrix of $u$ with respect to this basis; to say that a subset $S$ of $\mathrm{End}(E)$ is relatively compact in $\mathrm{End}(E)$ is equivalent to saying that the functions $\alpha_{ij}(u)$ are bounded in $S$.

#### Proposition 1 {#int-vii-s3-prop-1 .statement}

— *Let G be a subgroup of Aut(E)*. *The following three properties are equivalent*:

(i) *G is relatively compact in End(E)*;
(ii) *G is relatively compact in Aut(E)*;
(iii) *G leaves invariant a nondegenerate$^1$ positive hermitian form on E*.

(iii) $\Rightarrow$ (i): Suppose that $G$ leaves invariant a nondegenerate positive hermitian form $\Psi$. Let $(e_1, \ldots, e_n)$ be an orthonormal basis for $\Psi$ (*Alg.*, Ch. IX, \S 6, No. 1, Cor. 1 of Th. 1). For every $u \in G$, let $(u_{ij})$ be its matrix with respect to $(e_i)$. For any $j$, we have $\sum_{i=1}^n |u_{ij}|^2 = 1$, thus $|u_{ij}| \leq 1$ for all $i$ and $j$, which proves (i).

(i) $\Rightarrow$ (ii): This follows from GT, X, \S 3, No. 5, Cor. of Th. 4, taking into account the fact that the topology of $\mathrm{End}(E)$ is that of compact convergence.

(ii) $\Rightarrow$ (iii): Suppose that the closure $\overline{G}$ of $G$ in $\mathrm{Aut}(E)$ is compact. Let $\Phi$ be a nondegenerate positive hermitian form on $E$. If the field of scalars is $\mathbf{R}$ or $\mathbf{C}$, the giving of $\Phi$ makes $E$ a finite-dimensional Hilbert space, and condition (iii) will result from the following lemma:

$^1$ Non dégénérée; in EVT, the term is replaced by séparante, subsequently translated as "separating" (TVS, V, \S 1, No. 1).

#### Lemma 1 {#int-vii-s3-lem-1 .statement}

Let F be a Hilbert space, K a compact group, and s ↦ U(s) a representation of K in the group of invertible elements of $\mathcal{L}(F; F)$, continuous for the topology of pointwise convergence. There exists a nondegenerate positive hermitian form $\varphi$ on F such that

$$
\varphi(U(s)x, U(s)y) = \varphi(x, y)
$$

for all $s \in K, x \in F, y \in F$, and such that the topological vector space structure of F defined by $\varphi$ (TVS, V, §1, No. 3) is identical to the original structure of F.

Let $\alpha$ be a Haar measure on K. For any $x, y$ in F, the mapping $s \mapsto (U(s)x|U(s)y)$ is continuous. Set

$$
\varphi(x, y) = \int (U(s)x|U(s)y)\, d\alpha(s).
$$

It is immediate that $\varphi(x, y)$ is a sesquilinear form on F. Since the set of endomorphisms $U(s)$ is compact in $\mathcal{L}_s(F; F)$, there exists a constant M such that $\|U(s)\| \leq M$ for all $s \in K$. For every $x \in F$, we therefore have

$$
M^{-1}\|x\| \leq \|U(s)x\| \leq M\|x\|,
$$

whence the inequalities

$$
M^{-2}\alpha(K)\|x\|^2 \leq \varphi(x, x) \leq M^2\alpha(K)\|x\|^2,
$$

which shows that $\varphi$ is positive and nondegenerate, and that the norm $\varphi(x, x)^{1/2}$ is equivalent to the norm $\|x\|$. Finally, for all $t \in K$,

$$
\begin{align*}
\varphi(U(t)x, U(t)y) &= \int (U(st)x|U(st)y)\, d\alpha(s) \\
&= \int (U(s)x|U(s)y)\, d\alpha(s) = \varphi(x, y).
\end{align*}
$$

When the field of scalars is $\mathbf{H}$, one argues exactly as before on replacing everywhere the function $s \mapsto (U(s)x|U(s)y)$ by the function $s \mapsto \Phi(sx, sy)$ defined on G, with values in $\mathbf{H}$. This completes the proof of the proposition.

#### Remark {#int-vii-s3-n1-rem-1 .statement}

Let $\Phi$ be a nondegenerate positive hermitian form on E. The unitary group $\mathbf{U}(\Phi)$ is closed in $\mathrm{Aut}(E)$, hence is compact (Prop. 1). Prop. 1 also shows that every compact subgroup of $\mathrm{Aut}(E)$ is contained in a subgroup of the form $\mathbf{U}(\Phi)$. If now $\mathbf{U}(\Phi)$ is contained in a compact subgroup K of $\mathrm{Aut}(E)$, one sees that there exists a nondegenerate positive hermitian form $\Phi'$ on E such that $\mathbf{U}(\Phi) \subset K \subset \mathbf{U}(\Phi')$, and it follows easily

(Exer. 1) that $\Phi$ and $\Phi'$ are proportional, whence $\mathbf{U}(\Phi) = K$. Thus the maximal compact subgroups of $\mathrm{Aut}(E)$ are the subgroups of the form $\mathbf{U}(\Phi)$.

### 2. Triviality of fibered spaces and of group extensions

#### Proposition 2 {#int-vii-s3-prop-2 .statement}

*Let X be a locally compact space in which a locally compact group H acts on the right, continuously and properly, by $(x, \xi) \mapsto x\xi$. Assume that X/H is paracompact. Let g be a continuous representation of H in $\mathbf{R}^n$. Then there exists a continuous mapping f of X into $\mathbf{R}^n$ such that $f(x\xi) = f(x) + g(\xi)$ for all $x \in X$ and $\xi \in H$.*

One reduces immediately to the case that $n = 1$. Since the additive group $\mathbf{R}$ is isomorphic to the multiplicative group $\mathbf{R}_+^*$, the proposition is then an immediate consequence of Prop. 7 of §2, No. 4.

#### Corollary {#int-vii-s3-n2-cor-1 .statement}

*Let X be a locally compact space in which a finite-dimensional real vector space V operates on the right, continuously and properly, by $(x, v) \mapsto xv$. Let $\pi$ be the canonical mapping of X onto $B = X/V$. Assume that B is paracompact.*

a) *There exists a continuous mapping f of X into V such that $f(xv) = f(x) + v$ for all $x \in X$ and $v \in V$.*

b) *If f is a mapping satisfying the conditions of a), then the mapping $x \mapsto (\pi(x), f(x))$ is a homeomorphism of X onto $B \times V$.*

The assertion a) results from Prop. 2 in which g is taken to be the identity mapping of V. Let f be a mapping satisfying the conditions of a). The mapping $x \mapsto x \cdot (-f(x))$ of X into X is continuous, and is constant on each orbit, hence is of the form $\varphi \circ \pi$, where $\varphi$ is a continuous mapping of B into X; for every $b \in B$, $\pi(\varphi(b)) = b$. The mappings $x \mapsto (\pi(x), f(x))$ of X into $B \times V$ and $(b, v) \mapsto \varphi(b) \cdot v$ of $B \times V$ into X are inverse to each other, because $\varphi(\pi(x)) \cdot f(x) = x \cdot (-f(x)) \cdot (f(x)) = x$, $\pi(\varphi(b) \cdot v) = \pi(\varphi(b)) = b$, and, if $b = \pi(y)$, then

$$
f(\varphi(\pi(y)) \cdot v) = f(y \cdot (-f(y)) \cdot v) = f(y) - f(y) + v = v .
$$

Since these mappings are continuous, they are homeomorphisms.

#### Remark {#int-vii-s3-n2-rem-1 .statement}

— Let E be a finite-dimensional real affine space, T a compact space, $\mu$ a measure on T of *total mass* 1, and f a continuous mapping of T into E. If an origin a in E is chosen, E becomes equipped with a vector space structure, and the integral $\int_T f(t) d\mu(t)$ therefore has meaning; it represents the point x of E such that

$$
x - a = \int_T (f(t) - a) d\mu(t) .
$$

This point is independent of the choice of $a$. For, let $a' \in \mathbf{E}$ and $x' \in \mathbf{E}$ be such that $x' - a' = \int_{\mathbf{T}} (f(t) - a') d\mu(t)$. Then

$$
x' - a = (x' - a') + (a' - a) = \int_{\mathbf{T}} (f(t) - a') d\mu(t) + \int_{\mathbf{T}} (a' - a) d\mu(t)
$$
$$
= \int_{\mathbf{T}} (f(t) - a) d\mu(t) = x - a,
$$

whence $x' = x$. We may therefore employ the symbol $\int_{\mathbf{T}} f(t) d\mu(t)$ without specifying the choice of origin in $\mathbf{E}$. If $u$ is an affine mapping of $\mathbf{E}$ into another finite-dimensional affine space $\mathbf{E}'$, then

$$
u \left( \int_{\mathbf{T}} f(t) d\mu(t) \right) = \int_{\mathbf{T}} u(f(t)) d\mu(t).
$$

For, $\mathbf{E}$ and $\mathbf{E}'$ may be identified with vector spaces in such a way that $u$ becomes a linear mapping, in which case the formula is known (Ch. III, §3, No. 2, Prop. 2 and No. 3, Prop. 7).

#### Lemma 2 {#int-vii-s3-lem-2 .statement}

*Let $G$ be a compact group, $\mu$ the normalized Haar measure of $G$, $\mathbf{E}$ a finite-dimensional real affine space, $A$ the affine group of $\mathbf{E}$, and $\rho$ a homomorphism of $G$ into $A$. Assume that, for every $x \in \mathbf{E}$, the mapping $s \mapsto \rho(s)x$ of $G$ into $\mathbf{E}$ is continuous. Then, for every $x \in \mathbf{E}$, the point*

$$
x_0 = \int_G \rho(s)x\, d\mu(s) \in \mathbf{E}
$$

*is invariant under $G$.*

For, for every $t \in G$,

$$
\rho(t)x_0 = \int_G \rho(t)\rho(s)x\, d\mu(s) = \int_G \rho(ts)x\, d\mu(s) = \int_G \rho(s)x\, d\mu(s) = x_0.
$$

#### Proposition 3 {#int-vii-s3-prop-3 .statement}

*Let $G$ be a locally compact group. Let $H$ be a closed normal subgroup of $G$, isomorphic to $\mathbf{R}^n$ and such that $G/H$ is compact.*

a) *There exists a closed subgroup $L$ of $G$ such that $G$ is the topological semi-direct product of $L$ and $H$.*

b) *If $M$ is a compact subgroup of $G$, there exists an element $x \in H$ such that $x^{-1}Mx \subset L$.*

c) *Every compact subgroup of $G$ is contained in a maximal compact subgroup.*

d) *The maximal compact subgroups of $G$ are the subgroups that are the transforms of $L$ by the inner automorphisms of $G$.*

Let $\pi$ be the canonical homomorphism of $G$ onto $K = G/H$. By passage to the quotient, the mapping $(s, h) \mapsto shs^{-1}$ of $G \times H$ into $H$ defines a continuous mapping $(\sigma, h) \mapsto \sigma \cdot h$ of $K \times H$ into $H$ such that $shs^{-1} = \pi(s) \cdot h$. We shall identify $H$ with $\mathbf{R}^n$ (and will therefore employ, as the case may be, either the multiplicative or the additive notation for the group law in $H$). By the Cor. of Prop. 2, there exists a continuous mapping $f$ of $G$ into $H$ such that $f(xh) = f(x) + h$ for $x \in G, h \in H$. For every $x \in G$, let $p(x) = x \cdot (-f(x))$, which depends only on the coset of $x$ with respect to $H$. Set

$$
\begin{align*}
(1) \quad F(x, y) &= p(xy)^{-1} p(x)p(y) = f(xy)y^{-1}x^{-1}x(-f(x))y(-f(y)) \\
&= f(xy)[y^{-1}(-f(x))y](-f(y)) \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y).
\end{align*}
$$

We see that *if* $F(x, y) = 0$ *for all* $x, y$ *in* $G$, then $p(G) = L$ is a subgroup of $G$ that intersects each coset of $H$ in one and only one point. Since $p$ is continuous, $G$ is then the topological semi-direct product of $L$ and $H$ (GT, III, §2, No. 10).

Now, for any $h, h' \in H$,

$$
\begin{align*}
F'(xh, yh') &= f(xhyh') - \pi(y)^{-1}f(xh) - f(yh') \\
&= f(xhy) + h' - \pi(y)^{-1}f(x) - \pi(y)^{-1}h - f(y) - h' \\
&= f(xy(\pi(y)^{-1}h)) - \pi(y)^{-1}f(x) - f(y) - \pi(y)^{-1}h \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y) = F(x, y).
\end{align*}
$$

Therefore $F$ defines, by passage to quotients, a continuous mapping $\varphi$ of $K \times K$ into $H$.

On the other hand, for all $x, y, z$ in $G$, we have

$$
\begin{align*}
F(z, xy) + F(x, y) &= f(zxy) - \pi(xy)^{-1}f(z) - f(xy) + f(xy) \\
&\phantom{=} - \pi(y)^{-1}f(x) - f(y) \\
&= \pi(y)^{-1}f(zx) - \pi(xy)^{-1}f(z) - \pi(y)^{-1}f(x) + f(zxy) \\
&\phantom{=} - \pi(y)^{-1}f(zx) - f(y) \\
&= \pi(y)^{-1}F(z, x) + F(zx, y),
\end{align*}
$$

therefore, for all $x', y', z'$ in $K$,

$$
-\varphi(x', y') = \varphi(z', x'y') - {y'}^{-1}\varphi(z', x') - \varphi(z'x', y').
$$

Let us integrate with respect to $z'$ by means of the normalized Haar measure $\alpha$ of $K$. Setting $\psi(x') = \int \varphi(z', x')\, d\alpha(z')$, $\psi$ is a continuous function on K, and (on observing that the operations of K in $\mathbf{R}^n$ respect the vector space structure of $\mathbf{R}^n$ by GT, VII, §2, No. 1, Prop. 1), one obtains

$$
-\varphi(x', y') = \psi(x'y') - {y'}^{-1}\psi(x') - \psi(y').
$$

In other words, setting $k - \psi \circ \pi$, which is a continuous function on G,

(2)
$$
-F(x, y) = k(xy) - \pi(y)^{-1}k(x) - k(y).
$$

Comparing (1) and (2), one sees that if $f$ is replaced by the continuous function $f + k$ (which leaves verified the property $f(xh) = f(x) + h$), F is replaced by 0 and, as we saw earlier, this completes the proof of a).

For every $g \in G$, let $l_g$ (resp. $h_g$) be the unique element of L (resp. H) such that $g = h_g l_g$. If $h_1 \in H$ and $g \in G$, then

$$
gh_1 = h_g l_g h_1 = h_g(l_g h_1 l_g^{-1})l_g,
$$

thus $h_g h_1 = h_g + l_g h_1 l_g^{-1}$. For every $g \in G$, let $\psi_g$ be the mapping of H into itself defined by

$$
\psi_g(h_1) = h_g + l_g h_1 l_g^{-1}.
$$

One sees that the mapping $(g, h_1) \mapsto \psi_g(h_1)$ of $G \times H$ into H is continuous and makes H a homogeneous space for G, in which the stabilizer of the origin is L. We observe moreover that when H is identified with $\mathbf{R}^n$, $\psi_g$ is an *affine* mapping of H into itself. This said, let M be a compact subgroup of G; by Lemma 2, there exists an $x \in H$ such that $\psi_m(x) = x$ for *all* $m \in M$. For $y \in H$, $\psi_y$ is the translation with vector $y$; it follows that for every $m \in M$, $\psi_{x^{-1}} \circ \psi_m \circ \psi_x$ transforms the origin of H into itself, therefore $x^{-1}mx \in L$. This proves that $x^{-1}Mx \subset L$, whence b).

Let $L'$ be a closed subgroup of G containing L. Then $L'$ is the topological semi-direct product of L and $L' \cap H$. If $L'$ is compact, then $L' \cap H$ is compact hence reduces to a point (GT, IV, §2, No. 2, Cor. 1 of Th. 2), therefore $L' = L$. This proves that L is a maximal compact subgroup of G; the same is therefore true of the subgroups that are the transforms of L by the inner automorphisms of G. The assertions c) and d) of Prop. 3 are then immediate consequences of b).

#### Proposition 4 {#int-vii-s3-prop-4 .statement}

*Let G be a locally compact group and H a closed normal subgroup of G such that K = G/H is compact. Then every continuous representation u of H in $\mathbf{R}$, such that $u(s\xi s^{-1}) = u(\xi)$ for all $\xi \in H$ and $s \in G$, may be extended to a continuous representation of G in $\mathbf{R}$.*

Let $L = G \times \mathbf{R}$ and let M be the set of $(\xi, -u(\xi))$, where $\xi$ runs over H. It is clear that M is a closed normal subgroup of L. Let $L' = L/M$ and let $\pi$ be the canonical mapping of L onto $L'$. The subgroup of L generated by M and R is H × R, hence is closed; therefore π(R) is a closed subgroup N of L'. The restriction ρ of π to R is a bijective continuous representation of R onto N. Lemma 2 of Appendix 1 proves that ρ is bicontinuous. Moreover, L'/N is isomorphic to L/(H × R) = G/H, hence is compact. By Prop. 3, and taking into account the fact that N is in the center of L', L' is the product of N with another subgroup. Therefore there exists a continuous representation of L' onto N that reduces on N to the identity mapping. Therefore there exists a continuous representation v of L onto R that is trivial on M and reduces on R to the identity mapping. For ξ ∈ H, one has v((ξ, 0)) = v((ξ, −u(ξ))(e, u(ξ))) = u(ξ), which completes the proof.

#### Lemma 3 {#int-vii-s3-lem-3 .statement}

Let G be a topological group generated by a compact neighborhood of e. Let H be a closed subgroup of G such that the homogeneous space G/H is compact. Then H is generated by a compact neighborhood of e in H.

Let C be a compact set such that G = CH. Enlarging C if necessary, we can suppose that C generates G and that G = ĈH. Then C^2 is compact and is covered by the Ĉs (s ∈ H), which are open. Therefore there exist s_1, ..., s_n in H such that C^2 ⊂ Ĉs_1 ∪ ... ∪ Ĉs_n. Let Γ be the subgroup of H generated by the s_i. Then C^2 ⊂ CΓ. By induction, it follows that C^n ⊂ CΓ for every n, therefore G = CΓ. Every element of H may be put in the form ab with a ∈ C, b ∈ Γ, whence a ∈ H, whence a ∈ C ∩ H. Therefore H is generated by C ∩ H and the s_i, that is, by a compact set.

#### Lemma 4 {#int-vii-s3-lem-4 .statement}

Let G be a connected topological group, D a totally disconnected normal subgroup of G. Then D is contained in the center of G.

For, let d ∈ D. The image of G under the continuous mapping x ↦ xdx^{-1} is a connected subset of D, hence reduces to {d}, which proves that xd = dx for all x ∈ G.

#### Proposition 5 {#int-vii-s3-prop-5 .statement}

Let G be a connected topological group admitting a discrete normal subgroup D such that K = G/D is compact, and such that the commutator subgroup of K is dense in K. Then D is finite and G is compact.

The group G is locally isomorphic to K (GT, III, §2, No. 6, Prop. 19), hence is locally compact; since it is connected, it is generated by a compact neighborhood of e. By Lemmas 3 and 4, D is a finitely generated abelian group, hence is isomorphic to a group $\mathbf{Z}^r \times D_1$ with D_1 finite (A, VII, §4, No. 7, Th. 3). Suppose that r > 0. Then there exists a representation f of D onto $\mathbf{Z}$. By Prop. 4, f may be extended to a continuous representation g of G in R. By passage to quotients, g defines a continuous representation $g'$ of $K$ in $\mathbf{R}/\mathbf{Z}$; since $\mathbf{R}/\mathbf{Z}$ is abelian, the kernel of $g'$ contains the commutator subgroup of $K$, therefore $g'$ is trivial; in other words, $g(G) \subset \mathbf{Z}$. Since $G$ is connected, it follows that $g(G) = \{0\}$, which is absurd since $f(D) = \mathbf{Z}$. Thus $r = 0$ and $D$ is finite. Consequently $G$ is compact (GT, III, §4, No. 1, Cor. 2 of Prop. 2).

### 3. Examples

In this subsection (with the exception of Examples 7 and 8), $K$ denotes a nondiscrete locally compact commutative field; $dx$ denotes a Haar measure on the additive group of $K$.

Recall that $\operatorname{mod} x = |x|$ when $K = \mathbf{R}$, $\operatorname{mod} x = |x|^2$ when $K = \mathbf{C}$, $\operatorname{mod} x = |x|_p$ when $K = \mathbf{Q}_p$.

#### Example 1 {#int-vii-s3-n3-exa-1 .statement}

General linear group.

Let $A$ be the algebra $M_n(K)$. The group $A^*$ of invertible elements of $A$ is none other than the general linear group $\mathbf{GL}(n, K)$. For every $X \in A$, the reduced norm $\operatorname{Nrd}_{A/K}(X)$ is $\det X$; consequently $N_{A/K}(X) = (\det X)^n$ (Alg., Ch. VIII, §12, No. 3, Prop. 8; cf. A, III, §9, No. 3, Example 3). Since $X \mapsto {}^t X$ is an isomorphism of $A$ onto the opposite algebra,

$$
N_{A^0/K}(X) = N_{A/K}({}^t X) = \det ({}^t X)^n = (\det X)^n.
$$

Then, Prop. 16 of §1, No. 11 proves that the measure

$$
\operatorname{mod}(\det X)^{-n} \cdot \bigotimes_{i,j} dx_{ij} \quad (X = (x_{ij}))
$$

is a left and right Haar measure on $\mathbf{GL}(n, K)$.

To determine the relatively invariant measures on $\mathbf{GL}(n, K)$, we shall rely on the following lemma:

#### Lemma 5 {#int-vii-s3-lem-5 .statement}

The continuous representations of $\mathbf{GL}(n, K)$ in $\mathbf{C}^*$ are the mappings of the form $X \mapsto \chi(\det X)$, where $\chi$ is a continuous representation of $K^*$ in $\mathbf{C}^*$.

Such a mapping is obviously a continuous representation of $\mathbf{GL}(n, K)$ in $\mathbf{C}^*$. Conversely, suppose that $\psi$ is a continuous representation of $\mathbf{GL}(n, K)$ in $\mathbf{C}^*$. For $x \in K^*$, set

$$
\tilde{x} = \begin{pmatrix}
x & & \\
& 1 & 0 \\
& & 1 \\
0 & \cdots & 1
\end{pmatrix}
$$

and $\chi(x) = \psi(\widetilde{x})$. Then, for every matrix $X \in \mathbf{GL}(n, K)$, we have $(\det X^{-1}) \sim \cdot X \in \mathbf{SL}(n, K)$. Since $\mathbf{SL}(n, K)$ is the commutator subgroup of $\mathbf{GL}(n, K)$ (A, III, §8, No. 9, Cor. of Prop. 17), $\psi((\det X^{-1}) \sim \cdot X) = 1$, whence
$$
\psi(X) = \psi((\det X) \sim) = \chi(\det X).
$$
This established, Cor. 1 of Prop. 10 of §1, No. 8 proves that the relatively invariant measures on $\mathbf{GL}(n, K)$ are, up to a constant factor, the measures of the form
$$
(4) \quad \chi(\det X) \cdot \bigotimes_{ij} dx_{ij} \qquad (X = (x_{ij})),
$$
where $\chi$ is a continuous representation of $K^*$ in $\mathbf{C}^*$.

**Example 2. — Affine group.**
For every $X \in \mathbf{GL}(n, K)$ and every $x \in K^n$, let $(X, x)$ be the affine linear mapping $\xi \mapsto X\xi + x$ in $K^n$. The set of $(X, x)$ is the affine group $G$ of $K^n$ (A, II, §9, No. 4). The set $T$ of translations is a closed normal subgroup of $G$, canonically isomorphic to $K^n$; on the other hand, $\mathbf{GL}(n, K)$ is a closed subgroup of $G$, and $G$ is the semi-direct product of $\mathbf{GL}(n, K)$ and $T = K^n$. One equips $G$ with the (locally compact) topology for which $G$ is the topological semi-direct product of $\mathbf{GL}(n, K)$ and $T$ (GT, III, §2, No. 10). One has
$$
(X, x) = (1, x) \cdot (X, 0).
$$
On the other hand, if $X \in \mathbf{GL}(n, K)$ and $x \in T$ then, for every $\xi \in K^n$,
$$
(X, 0)(1, x)(X, 0)^{-1}\xi = X(X^{-1}\xi + x) = \xi + Xx = (1, Xx)\xi,
$$
therefore the automorphism $(1, x) \mapsto (X, 0)(1, x)(X, 0)^{-1}$ of $T$ has modulus $\mod(\det X)$ (§1, No. 10, Prop. 15). In view of Example 1 and §2, No. 9, *Remark*, the measure
$$
(5) \quad \mod(\det X)^{-n-1} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right) \qquad (X = (x_{ij}), \ x = (x_i))
$$
is a left Haar measure on $G$. On the other hand, by Prop. 14 of §2, No. 9,
$$
\Delta_G((X, x)) = \Delta_{\mathbf{GL}(n, K)}(X) \Delta_{K^n}(x) (\mod \det X)^{-1},
$$
or
$$
(6) \quad \Delta_G((X, x)) = \mod(\det X^{-1}).
$$

Thus, a right Haar measure on $G$ is given by

$$
(\mod \det X)^{-n} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right).
$$

**Example 3. — Strict triangular group.**

Let $[1, n]$ be the set of integers $m$ such that $1 \leq m \leq n$. Let $J$ be a subset of $[1, n] \times [1, n]$ satisfying the following conditions:
1) if $(i, j) \in J$ then $i < j$;
2) if $(i, j) \notin J$ then, for every integer $k$ such that $i < k < j$, at least one of the two pairs $(i, k)$ and $(k, j)$ does not belong to $J$.

Let $T_J$ be the set of matrices $Z = (z_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ with elements in $K$, such that $z_{ii} = 1$, and $z_{ij} = 0$ if $i \neq j$ and $(i, j) \notin J$. This is a closed subset of $\mathbf{GL}(n, K)$. The mapping $Z \mapsto (z_{ij})_{(i, j) \in J}$ is a homeomorphism of $T_J$ onto $K^s$ (where $s$ denotes the number of elements of $J$). If $Z' = (z'_{ij}) \in T_J$, then $Z'Z = (z''_{ij})$ with

$$
z''_{ij} = z_{ij} + z'_{ij} + \sum_{i < h < j} z'_{ih} z_{hj} \quad \text{for } i < j,
$$
$$
z''_{ij} = 0 \text{ for } i > j, \quad z''_{ii} = 1,
$$

whence $Z'Z \in T_J$. If $T_J$ is identified with $K^s$, then the mapping $Z \mapsto Z'Z$ (for fixed $Z'$) is identified with an affine mapping, and its determinant is 1, as one sees by ordering the pairs $(i, j) \in J$ lexicographically and applying the following lemma:

**Lemma 6. — Let $L$ be a totally ordered finite set. For every $\lambda \in L$, let $V_\lambda$ be a free module of finite dimension over a commutative ring $k$; for $\lambda, \mu$ in $L$ such that $\lambda \leq \mu$, let $f_{\lambda \mu} \in \mathrm{Hom}_k(V_\mu, V_\lambda)$. Then the linear mapping
$$
(v_\lambda)_{\lambda \in L} \mapsto \left( \sum_{\mu \geq \lambda} f_{\lambda \mu}(v_\mu) \right)_{\lambda \in L},
$$
from $\prod_{\lambda \in L} V_\lambda$ into $\prod_{\lambda \in L} V_\lambda$, has determinant $\prod_{\lambda \in L} \det f_{\lambda \lambda}$.

One reduces immediately to the case that $L$ is an interval of integers, and the lemma then follows from A, III, §8, No. 6, formula (31).

If $Z \in T_J$, one then sees that there exists $Z' \in T_J$ such that $Z'Z = I_n$, whence $Z' = Z^{-1}$. Thus, $T_J$ is a closed subgroup of $\mathbf{GL}(n, K)$. On the other hand, Prop. 15 of §1, No. 10 shows that the measure

$$
\bigotimes_{(i, j) \in J} dz_{ij}
$$

is a left Haar measure on $T_J$. By calculating $ZZ'$ one sees in the same way that this measure is a right Haar measure on $T_J$.

There is an analogous result if, in the definition of $T_J$, the roles of rows and columns are interchanged.

When $J$ is the set of pairs $(i, j)$ such that $i < j$, the group $T_J$ is called the *upper strict triangular group* of order $n$ over $K$, and is denoted $T_1(n, K)$. Its transpose is called the *lower strict triangular group*.

#### Example 4 {#int-vii-s3-n3-exa-4 .statement}

— *Large triangular group.*

Let $n_1, \ldots, n_r$ be integers $\geqslant 1$. Set $p_k = n_1 + \ldots + n_{k-1}$ and $n = p_{r+1} = n_1 + \cdots + n_r$. Let $I_k$ be the set of integers $j$ such that $p_k < j \leqslant p_{k+1}$, and $J$ the union of the $I_k \times I_l$ for $k < l$. Let $G$ be the closed subgroup of $\mathbf{GL}(n, K)$ whose elements are the matrices $(Z_{kl})_{1 \leqslant k \leqslant r, 1 \leqslant l \leqslant r}$ such that:
1) each $Z_{kl}$ is a matrix $(z_{ij})_{i \in I_k, j \in I_l}$ of elements of $K$, with $n_k$ rows and $n_l$ columns;
2) $Z_{kl} = 0$ for $k > l$;
3) $Z_{kk} \in \mathbf{GL}(n_k, K)$ for $1 \leqslant k \leqslant r$.

The formula for block multiplication

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$

$$
= \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

shows that $G$ is the topological semi-direct product of the subgroup $D$ of elements $(Z_{kl}) \in G$ such that $Z_{kl} = 0$ for $k \neq l$ and the subgroup $T_J$ of Example 3. Moreover, $D$ is isomorphic to the direct product of the groups $\mathbf{GL}(n_k, K)$ for $1 \leqslant k \leqslant r$.

Let $J'$ be the set of pairs $(j, i)$ for $(i, j) \in J$ and let $H$ be the set of pairs $(i, j) \in [1, n] \times [1, n]$ not belonging to $J'$. Let $Z' = (z_{ij})_{1 \leqslant i \leqslant n, 1 \leqslant j \leqslant n}$ be an element of $G$. By Prop. 14 of §2, No. 9 and the above Examples 1 and 3, one obtains a left Haar measure on $G$ by taking the image of the measure

$$
\bigotimes_{k=1}^r ((\mathrm{mod}\ \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes \left( \bigotimes_{(i,j) \in J} dz_{ij} \right)
$$

under the mapping

$$
((Z_{kk}), (Z_{kl})) \mapsto \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}.
$$

Now, consider, for $k < l$, the vector space of matrices $Z_{kl} = (z_{ij})_{i \in I_k, j \in I_l}$. It is the direct sum of the $n_l$ subspaces $M_j$ ($j \in I_l$) formed by the matrices such that $z_{ih} = 0$ for $h \neq j$. Each of these subspaces $M_j$ is stable under the mapping $Z_{kl} \mapsto Z_{kk}Z_{kl}$, and the restriction of this mapping to $M_j$ has matrix $Z_{kk}$. Consequently (\S 1, No. 10, Prop. 15) the image of the measure $\bigotimes_{i \in I_k, j \in I_l} dz_{ij}$ under the mapping $Z_{kl} \mapsto Z_{kk}Z_{kl}$ is

$$
(\operatorname{mod} \det Z_{kk})^{-n_l} \cdot \bigotimes_{i \in I_k, j \in I_l} dz_{ij}.
$$

A left Haar measure on $G$ is therefore given by

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-q_k} \cdot \bigotimes_{(i,j) \in H} dz_{ij}
$$

with $q_k = \sum_{k \leq l \leq r} n_l = n - p_k$.

Let us calculate the *modulus* of $G$, again using Prop. 14 of \S 2. The groups $D$ and $T_J$ are unimodular; on the other hand:

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}^{-1}
$$
$$
= \begin{pmatrix}
1 & Z'_{12} & \ldots & Z'_{1r} \\
0 & 1 & \ldots & Z'_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix},
$$

where $Z'_{kl} = Z_{kk}Z_{kl}Z_{ll}^{-1}$. Taking into account Example 3, and Prop. 15 of \S 1, No. 10, and arguing as above, one sees that if $X = \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \in D$ then the modulus of the automorphism $Z \mapsto X^{-1}ZX$ of $T_J$ is

$$
\prod_{k < l} (\operatorname{mod} \det Z_{kk})^{-n_l} (\operatorname{mod} \det Z_{ll})^{n_k},
$$

therefore

$$
\Delta_G(Z) = \prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2q_k}.
$$

The transposed group $G'$ of $G$ is studied in the same manner. For $G'$, one finds as left Haar measure

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-p_{k+1}} \cdot \bigotimes_{(j,i) \in \mathbb{H}} dz_{ij},
$$

and as modulus

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2p_{k+1}}.
$$

If in particular one takes $n_1 = \ldots = n_r = 1$, one finds as group $G$ the group $T(n, K)^*$ of invertible elements of the subalgebra of $M_n(K)$ formed by the matrices $X = (x_{ij})$ such that $x_{ij} = 0$ for $i > j$. This algebra, which we shall denote $T(n, K)$, is called the *upper triangular algebra*, and the group $T(n, K)^*$ is called the *upper large triangular group* of order $n$ over $K$. The preceding formulas then take the following form: a left Haar measure on $T(n, K)^*$ is

$$(9\ bis)$$
$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{i-n-1} \cdot \bigotimes_{i \leq j} dz_{ij} \quad (Z = (z_{ij}))
$$

and the modulus of $T(n, K)^*$ is

$$(10\ bis)$$
$$
\Delta_{T(n,K)^*}(Z) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1} \quad (Z = (z_{ij})).
$$

For the transpose of $T(n, K)^*$, or *lower large triangular group*, one finds as left Haar measure

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{-i} \cdot \bigotimes_{i \geq j} dz_{ij},
$$

and as modulus

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{n+1-2i}.
$$

#### Remark {#int-vii-s3-n3-rem-1 .statement}

The group $T(n, K)^*$ is a closed subgroup of $\mathbf{GL}(n, K)$, and $\Delta_{T(n, K)^*}((z_{ij})) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1}$. We saw in Example 1 that $\Delta_{\mathbf{GL}(n, K)} = 1$. If $n > 1$, the function
$$
\Delta_{T(n, K)^*}/\Delta_{\mathbf{GL}(n, K)}
$$
on $T(n, K)^*$ cannot be extended to a continuous representation of $\mathbf{GL}(n, K)$ in $\mathbf{C}^*$ (because such a representation would be equal to 1 on $\mathbf{SL}(n, K)$ by Lemma 5, whereas $\operatorname{mod}(z_{11})^{1-n} \neq 1$ for $z_{11}$ suitably chosen). It follows that the homogeneous space $\mathbf{GL}(n, K)/T(n, K)^*$ *admits no relatively invariant measure* if $n > 1$ (\S 2, No. 6, Cor. 1 of Th. 3).

This homogeneous space may be identified, for $n = 2$, with the *projective line* over $K$. For, let $(e_1, e_2)$ be the canonical basis of $K^2$. The group $\mathbf{GL}(2, K)$ operates transitively on the set of lines of $K^2$ with 0 omitted, and the stabilizer of $Ke_1 - \{0\}$ is $T(2, K)^*$.

#### Example 5 {#int-vii-s3-n3-exa-5 .statement}

— *Special triangular group.*
Let us take up again the notations at the beginning of Example 4, and consider the subgroup $G_1 = G \cap \mathbf{SL}(n, K)$. This subgroup is the topological semi-direct product of the group $D_1 = D \cap \mathbf{SL}(n, K)$ with $T_J$. The group $D_1$ has a normal subgroup $A$ isomorphic to $\mathbf{SL}(n_r, K)$, namely the subgroup consisting of the elements $\operatorname{diag}(Z_{kk})$ with $Z_{kk} = 1$ for $k < r$. The homomorphism
$$
\varphi : \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \mapsto (Z_{11}, \ldots, Z_{r-1, r-1})
$$
of $D_1$ into $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$ is surjective and has kernel $A$. On the other hand, $\varphi$ is continuous. Taking into account Lemma 2 of Appendix I, $D_1/A$ may be identified with $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$. We shall denote by $\mu$ the Haar measure of $A$ (cf. Example 6) and by
$$
\alpha = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes' d\mu(Z_{rr})
$$
the Haar measure on $D_1$ such that
$$
\alpha/\mu = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right)
$$
(\S 2, No. 7, Prop. 10). One then shows as in Example 4 that a left Haar measure on $G_1$ is given by
$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{n_k-q_k} \right)
$$
$$
\cdot \left[ \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes' d\mu(Z_{rr}) \right] \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

Since $G_1$ is normal in $G$, the *modulus* of $G_1$ is the restriction of that of $G$ (\S 2, No. 7, Prop. 10 b)).

If $n_r = 1$, the subgroup $A$ reduces to the neutral element, and a left Haar measure on $G$ is

$$
\operatorname{mod}\left( \prod_{k=1}^{r-1} (\det Z_{kk})^{-q_k} \right) \cdot \bigotimes_{k=1}^{r-1} \left( \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

If one takes $n_1 = n_2 = \ldots = n_r = 1$, the group $G_1$ obtained is called the *upper special triangular group* and its transpose $G'_1$ is called the *lower special triangular group*. A left Haar measure on $G_1$ is

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{i-n-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq i < j \leq n} dz_{ij} \right)
$$
and the modulus of $G_1$ is
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2i-2n} \right).
$$
For $G'_1$ one finds similarly the left Haar measure
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{n-i-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq j < i \leq n} dz_{ij} \right)
$$
and modulus
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2n-2i} \right).
$$

#### Example 6 {#int-vii-s3-n3-exa-6 .statement}

— *Special linear group.*
The closed subgroups $T_1(n, K)$ and ${}^t(T(n, K)^*)$ of $\mathbf{GL}(n, K)$ have intersection $\{e\}$. Thus the mapping $(M, N) \mapsto M \cdot N$ is a continuous bijection $\varphi$ of $T_1(n, K) \times {}^t(T(n, K)^*)$ onto a subset $\Omega$ of $\mathbf{GL}(n, K)$.

#### Lemma 7 {#int-vii-s3-lem-7 .statement}

— a) *Let $U = (u_{ij}) \in \mathbf{GL}(n, K)$. In order that $U \in \Omega$, it is necessary and sufficient that $\det(u_{ij})_{k \leq i, j \leq n} \neq 0$ for $k = 2, 3, \ldots, n$.*
b) $\Omega$ *is an open subset of $\mathbf{GL}(n, K)$*.
c) *The mapping $\varphi$ is a homeomorphism of $T_1(n, K) \times {}^t(T(n, K)^*)$ onto $\Omega$*.

In order that $U \in \Omega$, it is necessary and sufficient that there exist a $Z = (z_{ij}) \in T_1(n, K)$ such that $ZU \in {}^t(T(n, K))$ (then necessarily

$ZU \in {}^t(T(n, K)^*)$ since $U$ and $Z$ are invertible). By what we saw earlier, if $Z$ exists then it is unique. Thus, in order that $U \in \Omega$, it is necessary and sufficient that the linear system

$$
\sum_{k=1}^n z_{ik} u_{kj} = 0 \qquad (1 \leq i < j \leq n)
$$

(where $(z_{ij}) \in T_1(n, K)$) admit a unique solution. Now, this system may be written

$$
(13) \qquad \sum_{k=i+1}^n z_{ik} u_{kj} = -u_{ij} \qquad (1 \leq i < j \leq n).
$$

For fixed $i$, one has a system of $n-i$ equations in the unknowns $z_{i,i+1}, z_{i,i+2}, \ldots, z_{i,n}$; for these systems to admit unique solutions, it is necessary and sufficient that

$$
\det(u_{kj})_{i+1 \leq k \leq n,\ i+1 \leq j \leq n} \neq 0
$$

for $i = 1, 2, \ldots, n-1$. This proves a). From this it follows that $\Omega$ is open in $\mathbf{GL}(n, K)$. On the other hand, on solving the system (13) by means of Cramer’s formulas, the $z_{ij}$ are obtained as rational functions of the $u_{ij}$ with nonzero denominators in $\Omega$, therefore $Z$ depends continuously on $U$ in $\Omega$, which proves c).

Now let $G'_1 \subset {}^t(T(n, K)^*)$ be the lower special triangular group. The mapping $(M, N) \mapsto M \cdot N$ is a continuous bijection $\psi$ of $T_1(n, K) \times G'_1$ onto a subset $\Omega'$ of $\mathbf{SL}(n, K)$.

**Lemma 8. — a)** *Let $U = (u_{ij}) \in \mathbf{SL}(n, K)$. In order that $U \in \Omega'$, it is necessary and sufficient that $\det(u_{ij})_{k \leq i, j \leq n} \neq 0$ for $k = 2, 3, \ldots, n$.*

b) $\Omega'$ *is an open subset of $\mathbf{SL}(n, K)$*.

c) *The mapping $\psi$ is a homeomorphism of $T_1(n, K) \times G'_1$ onto $\Omega'$*.

For, let $M \in T_1(n, K)$ and $N \in {}^t(T(n, K)^*)$. In order that $M \cdot N \in \mathbf{SL}(n, K)$, it is necessary and sufficient that $N \in G'_1$. Therefore $\Omega' = \mathbf{SL}(n, K) \cap \Omega$ and Lemma 8 follows at once from Lemma 7.

**Proposition 6. — a)** *The group $\mathbf{SL}(n, K)$ is unimodular.*

b) *Let $\mu_1$ and $\mu_2$ be left Haar measures on the upper strict triangular group $T_1(n, K)$ and the lower special triangular group $G'_1$, respectively. The image of $\mu_1 \otimes \mu_2$ under the homeomorphism $(M, N) \mapsto M \cdot N^{-1}$ of $T_1(n, K) \times G'_1$ onto $\Omega'$ is the restriction to $\Omega'$ of a Haar measure on $\mathbf{SL}(n, K)$*.

c) *The complement of $\Omega'$ in $\mathbf{SL}(n, K)$ is negligible for the Haar measure of $\mathbf{SL}(n, K)$*.

The group $\mathbf{GL}(n, K)$ is unimodular (Example 1), and $\mathbf{SL}(n, K)$ is a normal subgroup of $\mathbf{GL}(n, K)$, hence is unimodular (\S 2, No. 7, Prop. 10 b)). The assertion b) follows from a), Lemma 8, and Prop. 13 of \S 2, No. 9. Let us prove c). By Lemma 8 a), it suffices to prove the following: if $p((u_{ij})_{1 \leq i,j \leq n})$ is a polynomial, not identically zero on $\mathbf{SL}(n, K)$, then the set E of $U \in \mathbf{SL}(n, K)$ such that $p(U) = 0$ is negligible for the Haar measure. Taking into account \S 1, No. 10, Cor. of Prop. 13, the topology of $\mathbf{SL}(n, K)$ has a countable base. It therefore suffices to prove that for every $U_0 \in E$, there exists a neighborhood of $U_0$ in $\mathbf{SL}(n, K)$ whose intersection with E is negligible; or again that there exists a neighborhood W of I in $\mathbf{SL}(n, K)$ such that $U_0^{-1}E \cap W$ is negligible. Let us take $W = \Omega'$. In view of b), it all comes down to showing that the set of pairs $(M, N) \in T_1(n, K) \times G'_1$ such that $p(U_0 MN) = 0$ is negligible for $\mu_1 \otimes \mu_2$. By the expressions for $\mu_1$ and $\mu_2$ (calculated in Examples 3 and 5), this will result from the following lemma:

#### Lemma 9 {#int-vii-s3-lem-9 .statement}

*Let $\psi$ be a polynomial $\neq 0$ of $K[X_1, \ldots, X_r]$. In the space $K^r$, the set N defined by $\psi(x_1, \ldots, x_r) = 0$ is negligible for the Haar measure.*

Let us argue by induction on $r$. The lemma is evident for $r = 1$, since N is then a finite set. Changing if necessary the numbering of the variables, we can suppose that $\psi \notin K[X_1, \ldots, X_{r-1}]$; write

$$
\psi(X_1, \ldots, X_r) = X_r^m \psi_0(X_1, \ldots, X_{r-1}) + \cdots + \psi_m(X_1, \ldots, X_{r-1})
$$

with $m > 0$ and $\psi_0 \neq 0$. In the space $K^{r-1}$, let $N_0$ be the set defined by $\psi_0(x_1, \ldots, x_{r-1}) = 0$, which is negligible by the induction hypothesis. For every $(x_1, \ldots, x_{r-1}) \notin N_0$, the set of $x_r \in K$ such that $(x_1, \ldots, x_{r-1}, x_r) \in N$ is finite, therefore negligible. Since $K^r$ is countable at infinity (\S 1, No. 10, Cor. of Prop. 13), $N \cap [(K^{r-1} - N_0) \times K]$ is negligible in $K^r$ (Ch. V, \S 8, No. 2, Prop. 4). Therefore N is negligible.

#### Example 7 {#int-vii-s3-n3-exa-7 .statement}

*Iwasawa decomposition of $\mathbf{GL}(n, K)$.*

In this example, K denotes one of the fields $\mathbf{R}, \mathbf{C}, \mathbf{H}$. If $\lambda \in K$, $\overline{\lambda}$ is defined to be equal to $\lambda$ if $K = \mathbf{R}$, and to the conjugate of $\lambda$ if $K = \mathbf{C}$ or $\mathbf{H}$. Let E be a right vector space over K of dimension $n$, and let $\Phi$ be a nondegenerate positive hermitian form on E.

#### Lemma 10 {#int-vii-s3-lem-10 .statement}

*Let $(f_1, f_2, \ldots, f_n)$ be a basis of E.*
a) *There exists one and only one orthonormal basis $(e_1, e_2, \ldots, e_n)$ of E such that $f_i = e_1 \alpha_{i1} + e_2 \alpha_{i2} + \cdots + e_i \alpha_{ii}$ ($i = 1, 2, \ldots, n$) with $\alpha_{ii} > 0$ for all $i$.
b) *For fixed $\Phi$, the $e_i$ and $\alpha_{ij}$ depend continuously on $(f_1, \ldots, f_n) \in E^n$.*

Let $E_i = f_1 K + f_2 K + \cdots + f_i K$, which has dimension $i$. Let $g_i$ be a nonzero element of $E_i$ orthogonal to $E_{i-1}$ and such that $\Phi(g_i, g_i) = 1$. By induction on $i$, one sees that $(g_1, \ldots, g_i)$ is an orthonormal basis of $E_i$. In particular, $(g_1, \ldots, g_n)$ is an orthonormal basis of $E$. Let $\lambda_i = \Phi(f_i, g_i)$. Since $f_i \notin E_{i-1}$, one has $\lambda_i \neq 0$. Set $e_i = g_i |\lambda_i| \lambda_i^{-1}$. Then

$$
\Phi(e_i, e_i) = |\lambda_i|^2 \overline{\lambda_i}^{-1} \Phi(g_i, g_i) \lambda_i^{-1} = 1,
$$

thus $(e_1, \ldots, e_i)$ is also an orthonormal basis of $E_i$; moreover, $\Phi(e_i, f_i) = |\lambda_i| \overline{\lambda_i}^{-1} \Phi(g_i, f_i) = |\lambda_i| > 0$, thus the $e_i$ have the properties of a). Let $(e'_1, \ldots, e'_n)$ be another orthonormal basis of $E$ with the same properties. One sees by induction on $i$ that $(e'_1, \ldots, e'_i)$ must be a basis of $E_i$, therefore $e'_i = e_i \mu_i$ for some $\mu_i \in \mathbf{K}$. Then

$$
1 = \Phi(e'_i, e'_i) = \overline{\mu_i} \Phi(e_i, e_i) \mu_i = \overline{\mu_i} \mu_i ,
$$

and $0 < \Phi(e'_i, f_i) = \overline{\mu_i} \Phi(e_i, f_i)$, therefore $\mu_i > 0$ and $\mu_i^2 = 1$, thus $\mu_i = 1$, whence a). Suppose already proven that the $e_i$ and $\alpha_{ij}$ depend continuously on $(f_1, \ldots, f_n)$ for $i < i_0$, and let us prove that $e_{i_0}$ and the $\alpha_{i_0 j}$ depend continuously on $(f_1, \ldots, f_n)$. For $j < i_0$, $\overline{\alpha}_{i_0 j} = \Phi(f_{i_0}, e_j)$ depends continuously on $(f_1, \ldots, f_n)$ by the induction hypothesis. On the other hand,

$$
\Phi(f_{i_0}, f_{i_0}) = |\alpha_{i_0 1}|^2 + |\alpha_{i_0 2}|^2 + \cdots + |\alpha_{i_0, i_0 - 1}|^2 + \alpha_{i_0 i_0}^2 ,
$$

thus $\alpha_{i_0 i_0}$ depends continuously on $(f_1, \ldots, f_n)$. Therefore

$$
e_{i_0} = (f_{i_0} - e_1 \alpha_{i_0 1} - \cdots - e_{i_0 - 1} \alpha_{i_0, i_0 - 1}) \alpha_{i_0 i_0}^{-1}
$$

depends continuously on $(f_1, \ldots, f_n)$.

Henceforth let $E = K^n$ and let us take for $\Phi$ the form

$$
\overline{x}_1 y_1 + \cdots + \overline{x}_n y_n .
$$

Recall that $\mathbf{U}(n, \mathbf{K})$ denotes the corresponding unitary group. Even when $\mathbf{K}$ is noncommutative, we shall again denote by $\mathbf{T}_1(n, \mathbf{K})$ the group of upper triangular matrices of $\mathbf{M}_n(\mathbf{K})$ whose diagonal entries are all 1.

#### Proposition 7 {#int-vii-s3-prop-7 .statement}

*Let $D_+^*$ be the group of diagonal matrices with diagonal elements $> 0$. The mapping $(U, D, T) \mapsto UDT$ is a homeomorphism of $\mathbf{U}(n, \mathbf{K}) \times D_+^* \times \mathbf{T}_1(n, \mathbf{K})$ onto $\mathbf{GL}(n, \mathbf{K})$.*

Let $(\varepsilon_1, \ldots, \varepsilon_n)$ be the canonical basis of $K^n$. Let $X \in \mathbf{GL}(n, K)$. Then the $X \cdot \varepsilon_i = f_i$ form a basis of E. To this basis $(f_i)$ one can associate a basis $(e_i)$ as in Lemma 10. Let $U$ be the matrix of the unitary automorphism of E that transforms $\varepsilon_i$ into $e_i$. Then

$$
U^{-1} \cdot f_i = \varepsilon_1 \alpha_{i1} + \varepsilon_2 \alpha_{i2} + \cdots + \varepsilon_i \alpha_{ii}
$$

with $\alpha_{ii} > 0$ for $i = 1, 2, \ldots, n$. Thus $X = UC$, where $C$ is the matrix

$$
\begin{pmatrix}
\alpha_{11} & \alpha_{21} & \cdots & \alpha_{n1} \\
0 & \alpha_{22} & \cdots & \alpha_{n2} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \alpha_{nn}
\end{pmatrix}.
$$

Moreover, $U$ and $C$ depend continuously on X by Lemma 10. On the other hand, formula (8) shows that $C$ may be put in the form $DT$ with $D \in \mathbf{D}_+^*$, $T \in \mathbf{T}_1(n, K)$, $D$ and $T$ depending continuously on $C$. The uniqueness of the decomposition $X = UDT$ follows from the uniqueness property of Lemma 10.

The homeomorphism of Prop. 7 is called the *Iwasawa decomposition* of $\mathbf{GL}(n, K)$.

The group $G = \mathbf{D}_+^* \cdot \mathbf{T}_1(n, K)$ is the set of upper triangular matrices over K whose diagonal elements are $> 0$. Let us identity the element $(z_{ij})$ of this group with the element

$$
((z_{ii})_{1 \leq i \leq n}, (z_{ij})_{1 \leq i < j \leq n}) \in (\mathbf{R}_+^*)^n \times K^{n(n-1)/2}.
$$

Arguing exactly as in Example 4, one finds as *right* Haar measure on this group the measure (when $K = \mathbf{R}$)

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < j} dz_{ij} \right).
$$

Then applying Prop. 13 of §2, No. 9, one sees that if $\mathbf{GL}(n, K)$ is identified with $\mathbf{U}(n, K) \times G$ by the mapping $(U, S) \mapsto US$, a Haar measure on $\mathbf{GL}(n, K)$ is given by (when $K = \mathbf{R}$)

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \alpha \otimes \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < n} dz_{ij} \right),
$$

where $\alpha$ denotes a Haar measure on $\mathbf{U}(n, K)$.

#### Example 8 {#int-vii-s3-n3-exa-8 .statement}

Spaces of hermitian forms.

In this example, K always denotes one of the fields $\mathbf{R}, \mathbf{C}, \mathbf{H}$. We write $\delta = \dim_{\mathbf{R}} K$ (thus $\delta = 1, 2$ or 4). A hermitian form $\Phi$ on the right vector space $K^n$ may be written

$$
\Phi(x, y) = \Phi(x_1, \ldots, x_n, y_1, \ldots, y_n) = \sum_{i,j=1}^n \overline{x_i} h_{ij} y_j
$$

with $h_{ij} = \overline{h_{ji}}$ for all $i$ and $j$. We denote by $\mathfrak{H}$ the vector space over $\mathbf{R}$ formed by the hermitian matrices of $M_n(K)$. The mapping $(h_{ij}) \mapsto \Phi$ is an isomorphism of $\mathfrak{H}$ onto the vector space of hermitian forms on $K^n$, by means of which we shall identify these two spaces. Let $\mathfrak{H}_+^* \subset \mathfrak{H}$ be the set of nondegenerate positive hermitian forms on $K^n$. The set $\mathfrak{H}_+^*$ is *convex* in $\mathfrak{H}$; for, if $\Phi_1, \Phi_2$ are in $\mathfrak{H}_+^*$ and if $\lambda, \mu$ are two numbers $> 0$ such that $\lambda + \mu = 1$, it is clear that $\lambda \Phi_1 + \mu \Phi_2$ is a positive hermitian form; on the other hand, if $(\lambda \Phi_1 + \mu \Phi_2)(x, x) = 0$, then $\Phi_1(x, x) = \Phi_2(x, x) = 0$, therefore $x = 0$, so that $\lambda \Phi_1 + \mu \Phi_2$ is nondegenerate. Let us now show that $\mathfrak{H}_+^*$ is an *open* subset of $\mathfrak{H}$. Let S be the set of $x = (x_1, \ldots, x_n) \in K^n$ such that $x_1 \overline{x}_1 + \cdots + x_n \overline{x}_n = 1$; this is a compact subset of $K^n$; if $\Phi \in \mathfrak{H}_+^*$, the function $x \mapsto \Phi(x, x)$ is continuous and $> 0$ on S, hence its infimum is $> 0$; if $\Phi' \in \mathfrak{H}$ is sufficiently near $\Phi$, it follows that $\Phi'(x, x) > 0$ for all $x \in S$, so that $\Phi'$ is positive and nondegenerate.

The general linear group $\mathbf{GL}(n, K)$ operates continuously on the right in $\mathfrak{H}$ by $(X, \Phi) \mapsto \Phi \circ X$, that is, by $(X, H) \mapsto t \overline{X} \cdot H \cdot X$, where $H$ denotes the hermitian matrix corresponding to $\Phi$. It is clear that $\mathfrak{H}_+^*$ is stable under $\mathbf{GL}(n, K)$. More precisely, by *Alg.*, Ch. IX, §6, No. 1, Cor. 1 of Th. 1,$^1$ $\mathfrak{H}_+^*$ is the orbit under $\mathbf{GL}(n, K)$ of the form $\sum_{i=1}^n \overline{x_i} y_i$ corresponding to the identity matrix $I_n$. The stabilizer of this form is $\mathbf{U}(n, K)$. By Lemma 2 of App. I, $\mathfrak{H}_+^*$ may be identified, as a topological homogeneous space, with $\mathbf{GL}(n, K)/\mathbf{U}(n, K)$.

For every $X \in \mathbf{GL}(n, K)$, let $\widetilde{X}$ be the automorphism $H \mapsto t \overline{X} \cdot H \cdot X$ of the *real* vector space $\mathfrak{H}$. If $\mu$ denotes the Haar measure of the additive group $\mathfrak{H}$, one has $\widetilde{X}^{-1}(\mu) = |\det \widetilde{X}| \cdot \mu$ (\S1, No. 10, Cor. 1 of Prop. 15). Let us show that

$$
| \det \widetilde{X} | = | N(X) |^\lambda ,
$$

where N denotes the norm in $M_n(K)$ *regarded as an* $\mathbf{R}\text{-algebra}$, and where $\lambda = 1 - \frac{\delta - 2}{\delta n}$. It suffices to verify (15) for $X$ running over a system of

\footnotetext{1Cf. TVS, V, §2, No. 4, Cor. 1 of Th. 2.}

generators of $\mathbf{GL}(n, K)$, hence (A, II, §10, No. 13, Cor. 2 of Prop. 14) for $X$ of the following types:

a) $X$ is the matrix of a mapping of the form
$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$
where $\sigma \in \mathfrak{S}_n$. In this case, a power of $X$ is equal to 1, therefore $|\det \widetilde{X}| = |N(X)| = 1$.

b) $X$ is the matrix of a mapping of the form
$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n).
$$
Then, if $(h_{ij}) \in \mathfrak{H}$, one has $\widetilde{X}((h_{ij})) = (h'_{ij})$ with $h'_{11} = \overline{a} h_{11} a = |a|^2 h_{11}$, $h'_{1i} = \overline{a} h_{1i}$ for $i > 1$, $h'_{ij} = h_{ij}$ for $i > 1, j > 1$; therefore
$$
|\det \widetilde{X}| = |a|^2 |a|^{\delta(n-1)} = |a|^{2+\delta(n-1)}.
$$
On the other hand, if $Y = (y_{ij}) \in M_n(K)$, then $XY = (y'_{ij})$ with $y'_{1j} = ay_{1j}$ and $y'_{ij} = y_{ij}$ for $i > 1$; therefore $|N(X)| = |a|^{\delta n}$. The formula (15) is again verified.

c) $X$ is the matrix of a mapping of the form
$$
(x_1, \ldots, x_n) \mapsto (x_1 + bx_2, x_2, \ldots, x_n).
$$
Then $\widetilde{X}((h_{ij})) = (h'_{ij})$ with $h'_{11} = h_{11}$, $h'_{12} = h_{12} + h_{11} b$, $h'_{1i} = h_{1i}$ for $i > 2$, $h'_{22} = h_{22} + \overline{b} h_{12} + \overline{h}_{12} b + \overline{b} h_{11} b$, $h'_{2i} = h_{2i} + \overline{b} h_{1i}$ for $i > 2$, $h'_{ij} = h_{ij}$ for $i > 2, j > 2$. Taking into account Lemma 6, one sees that $|\det \widetilde{X}| = 1$. One verifies similarly that $|N(X)| = 1$, which completes the proof of formula (15).

This established, the measure $|N(H)|^{-\lambda/2} d\mu(H)$ on $\mathfrak{H}$ is invariant under $\mathbf{GL}(n, K)$, since
$$
\widetilde{X}^{-1}(|N(H)|^{-\lambda/2} d\mu(H)) = |N(\widetilde{X}(H))|^{-\lambda/2} \cdot |\det \widetilde{X}| d\mu(H)
= |N(H)|^{-\lambda/2} |N(X)|^{-\lambda} |\det \widetilde{X}| d\mu(H) = |N(H)|^{-\lambda/2} d\mu(H).
$$

If $H \in \mathfrak{H}_+^*$, then $H = \widetilde{X}(I_n) = {}^t \overline{X} X$ for some $X \in \mathbf{GL}(n, K)$, therefore $N(H) = \overline{N(X)} N(X) > 0$. Consequently, on $\mathfrak{H}_+^*$, the unique (up to a constant factor) measure invariant under $\mathbf{GL}(n, K)$ (cf. §2, No. 6, Th. 3) is the measure
$$
d\gamma(H) = N(H)^{-\lambda/2} d\mu(H).
$$
In particular,
$$
d\gamma(H) = (\det H)^{-(n+1)/2} d\mu(H) \quad \text{when } K = \mathbf{R},
$$
$$
d\gamma(H) = (\det H)^{-n} d\mu(H) \quad \text{when } K = \mathbf{C}.
$$

### Exercises {#int-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
