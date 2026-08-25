---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 4
section_title: Some classes of operators in hilbertian spaces
lang: en
source: evt-i-v
pdf_pages: 0295-0318
extraction: ocr
subsections:
    - "no": 1
      title: Adjoint
      page: 38
      pdf_page: 296
    - "no": 2
      title: Partially isometric linear mappings
      page: 41
      pdf_page: 299
    - "no": 3
      title: Normal endomorphisms
      page: 43
      pdf_page: 301
    - "no": 4
      title: Hermitian endomorphisms
      page: 44
      pdf_page: 302
    - "no": 5
      title: Positive endomorphisms
      page: 45
      pdf_page: 303
    - "no": 6
      title: Trace of an endomorphism
      page: 48
      pdf_page: 306
    - "no": 7
      title: Hilbert-Schmidt mappings
      page: 52
      pdf_page: 310
    - "no": 8
      title: Diagonalization of Hilbert-Schmidt mappings
      page: 55
      pdf_page: 313
    - "no": 9
      title: Trace of a quadratic form with respect to another
      page: 57
      pdf_page: 315
statements: 48
exercises: 0
content_sha256: e91bc304651ce770d0fd7f9268828dea76e99a75428b9ae2fa319330bd7c91db
---

## § 4. SOME CLASSES OF OPERATORS IN HILBERTIAN SPACES

Throughout this paragraph, $l_E$ denotes the identity mapping of a hilbertian space E. The composition $v \circ u$ of two linear mappings will usually be denoted by $vu$ or $v.u$.

### 1. Adjoint

#### Proposition 1 {#evt-v-s4-prop-1 .statement}

— Let E and F be two hilbertian spaces. For every mapping $u \in \mathcal{L}(E; F)$, there exists a unique mapping $u^* \in \mathcal{L}(F; E)$ such that

$$
\langle u(x)|y \rangle_F = \langle x|u^*(y) \rangle_E
$$

for all $x \in E$ and all $y \in F$. The mapping $u \mapsto u^*$ from $\mathcal{L}(E, F)$ into $\mathcal{L}(F; E)$ is bijective, isometric and semi-linear (with respect to the automorphism $\xi \mapsto \overline{\xi}$ of K).

Let $\mathscr{S}(E, F)$ be the space of all continuous sesquilinear forms on $E \times F$, endowed with the norm

$$
\| \Phi \| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| .
$$

We define the space $\mathscr{S}(F, E)$ similarly. We defined (V, p. 16, cor. 2) a Banach space isomorphism from $\mathcal{L}(E; F)$ onto $\mathscr{S}(F, E)$, denoted by $u \mapsto \Phi_u$ and characterized by

$$
\Phi_u(y, x) = \langle y|u(x) \rangle_F \quad (x \in E, \ y \in F) .
$$

In an analogous way we define an isomorphism from $\mathcal{L}(F, E)$ onto $\mathscr{S}(E, F)$. Finally we define a mapping $\Phi \mapsto \Phi^*$ from $\mathscr{S}(F, E)$ onto $\mathscr{S}(E, F)$ by

$$
\Phi^*(x, y) = \overline{\Phi(y, x)} \quad (x \in E, \ y \in F) .
$$

This mapping is bijective, semi-linear and isometric. But formula (1) translates as $\Phi_{u^*} = (\Phi_u)^*$, hence the proposition.

#### Definition 1 {#evt-v-s4-def-1 .statement}

— Let E and F be two hilbertian spaces. For every continuous linear mapping $u : E \to F$, the continuous linear mapping from F into E defined by formula (1) is called the adjoint of u and is denoted by $u^*$.

We have

$$
\begin{align*}
(u + v)^* &= u^* + v^* \\
(\lambda u)^* &= \overline{\lambda} u^* \\
(u^*)^* &= u \\
(1_E)^* &= 1_E \\
(wu)^* &= u^* w^* ;
\end{align*}
$$

in all these formulas, $u$ and $v$ belong to $\mathcal{L}(E; F)$, $\lambda$ is in K, and $w$ in $\mathcal{L}(F; G)$ where G is a hilbertian space. Formulas (5) and (6) mean that $u \mapsto u^*$ is semi-linear. Formula (8) is obvious. To prove (7), we take the conjugate of the two members of (1), which gives $\langle u^*(y)|x\rangle = \langle y|u(x)\rangle$, and this proves that $u$ is the adjoint of $u^*$. Finally, with the notations of (9), we have, for all $z \in G$

$$
\langle w(u(x))|z\rangle = \langle u(x)|w^*(z)\rangle = \langle x|u^*(w^*(z))\rangle ,
$$

hence $u^*w^*$ is the adjoint of $wu$.

Let $u : E \to F$ be a bijective and continuous linear mapping; then it is also bicontinuous (I, p. 19, cor. 1). From (8) and (9) we immediately deduce that $u^*$ is bijective and bicontinuous and that

(10)
$$
(u^{-1})^* = (u^*)^{-1} .
$$

#### Proposition 2 {#evt-v-s4-prop-2 .statement}

*For every $u \in \mathcal{L}(E ; F)$, we have*

(11)
$$
\|u^*u\| = \|uu^*\| = \|u\|^2 = \|u^*\|^2 .
$$

By prop. 1, $\|u^*\| = \|u\|$, hence $\|u^*u\| \leq \|u^*\|\cdot\|u\| \leq \|u\|^2$. On the other hand,

$$
\|u\|^2 = \sup_{\|x\| \leq 1} \|u(x)\|^2 = \sup_{\|x\| \leq 1} \langle u(x)|u(x)\rangle = \sup_{\|x\| \leq 1} \langle x|u^*u(x)\rangle \leq \|u^*u\| ,
$$

hence $\|u^*u\| = \|u\|^2$. Replacing $u$ by $u^*$, we get $\|uu^*\| = \|u^*\|^2$, hence (11) follows since $\|u\| = \|u^*\|$.

Let $E_1, ..., E_n$ and $F_1, ..., F_n$ be hilbertian spaces, and for every integer $i$ between 1 and $n$, let $u_i$ be a continuous linear mapping from $E_i$ into $F_i$. Then

(12)
$$
(u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n)^* = u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^* .
$$

Let $v$ be the continuous linear mapping $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ from

$$
E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n \quad \text{into} \quad F = F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n
$$

and $w$ the continuous linear mapping $u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^*$ from $F$ into $E$. It is enough to prove the equality $\langle y|v(x)\rangle = \langle w(y)|x\rangle$ for $x \in E$ and $y \in F$. By linearity and continuity, we reduce to the case when $x$ and $y$ have the following form

$$
x = x_1 \otimes ... \otimes x_n , \quad y = y_1 \otimes ... \otimes y_n
$$

with $x_i \in E_i$ and $y_i \in F_i$ for $1 \leq i \leq n$. From the definition of scalar product in a tensor product (V, p. 27, formula (6)), we then get

$$
\langle y|v(x)\rangle = \prod_{i=1}^n \langle y_i|u_i(x_i)\rangle = \prod_{i=1}^n \langle u_i^*(y_i)|x_i\rangle = \langle w(y)|x\rangle .
$$

This proves our assertion.

Let $E$ and $F$ be two hilbertian spaces, $u \in \mathcal{L}(E ; F)$ and $n$ a positive integer. If we put $u_1 = ... = u_n = u$ in formula (12) we obtain the result that the continuous linear mapping $\hat{T}^n(u^*)$ from $\hat{T}^n(F)$ into $\hat{T}^n(E)$ is the adjoint of the continuous linear mapping $\hat{T}^n(u)$ from $\hat{T}^n(E)$ into $\hat{T}^n(F)$. The formulas

$$
\hat{S}^n(u)^* = \hat{S}^n(u^*) , \quad \hat{\Lambda}^n(u)^* = \hat{\Lambda}^n(u^*)
$$

can be established in the same way as formula (12), on account of the definition of the scalar product in $\hat{S}^n(E)$ (V, p. 30, formula (15)) and in $\hat{\Lambda}^n(E)$ (V, p. 33, formula (26)).

#### Remark 1 {#evt-v-s4-n1-rem-1 .statement}

Suppose the hilbertian space E does not reduce to 0. We identify $\mathcal{L}(K;E)$ with E by the mapping $u \mapsto u(1)$; in other words, the vector x of E is identified with the mapping $\lambda \mapsto \lambda.x$ from K into E. Then the adjoint of x is the mapping $x^*:E \to K$ given by $x^*(y) = \langle x|y \rangle$. In other words, $x \mapsto x^*$ is the canonical semi-linear mapping from E onto its dual (V, p. 15).

Similarly, we identify the number $\lambda \in K$ with the endomorphism $\lambda.1_E$ of E. Then $\lambda^*$ is precisely the conjugate of $\lambda$.

With these identifications, we can define a product $t_1 ... t_n$ where each $t_i$ is, either a number in K, or a vector in E, or a linear form belonging to E', or an element of $\mathcal{L}(E)$, provided that there are never two consecutive factors $t_i$ and $t_{i+1}$ of one of the following types :
• xy where x, y are both in E, or both in E';
• xA or Ax' with $A \in \mathcal{L}(E)$, $x \in E$ and $x' \in E'$.

We have the following rules of composition :
a) associativity ;
b) every element of K commutes with all the other factors ;
c) we have $(t_1 ... t_n)^* = t_n^* ... t_1^*$; in other words, the adjoint of a product is the product of the adjoints taken in the reverse order. Also $t^{**} = t$.

For example, let x, y be in E and let A be in $\mathcal{L}(E)$. Then $x^*y$ represents the scalar product $\langle x|y \rangle$ and $x^*Ay$ represents the scalar product $\langle x|Ay \rangle$. We also have $(A^*x)^* = x^*A^{**} = x^*A$, hence $(A^*x)^*y = x^*Ay$, which can be interpreted as

$$
\langle A^*x|y \rangle = \langle x|Ay \rangle
$$

in conformity with the definition of the adjoint. We observe that $yx^*$ is the endomorphism $z \mapsto y \langle x|z \rangle$ of E, since $yx^*z$ can be interpreted as $y(x^*z)$ by associativity, or as $y.\langle x|z \rangle$.

Following Dirac $^1$, in most works of Mathematical Physics, the elements of E are represented by the symbol $|x\rangle$, those of E' by $\langle t|$. The scalar product is written as $\langle x|y \rangle = \langle x|.|y \rangle$ and the first rule of interdiction in the products excludes the combinations of the signs $|$ and $|<$, for example $|x\rangle|y\rangle$.

#### Proposition 3 {#evt-v-s4-prop-3 .statement}

— Let E and F be two hilbertian spaces and $u \in \mathcal{L}(E;F)$. The following conditions are equivalent :

(i) $u$ is a topological vector space isomorphism, with an inverse equal to $u^*$;
(ii) $u$ is surjective and $u^*u = 1_E$;
(iii) $u$ is injective and $uu^* = 1_F$;
(iv) $u$ is an isomorphism of normed spaces;
(v) $u$ is a hilbertian space isomorphism.

Condition (1) means that we have $u^*u = 1_E$ and $uu^* = 1_F$. Hence the equivalence of (i), (ii) and (iii) follows from E, II, § 3, No. 8, prop. 8. We have already seen the equivalence of (iv) and (v) (V, p. 5). Finally, the relation $u^*u = 1_E$ is equivalent to

$^1$ See P. A. M. Dirac, Quantum Mechanics, Oxford University Press, New York, 1935.

$
\langle x|u^*u(y)\rangle = \langle x|y\rangle$, that is, to $\langle u(x)|u(y)\rangle = \langle x|y\rangle$ for all $x, y$ in $E$, and evidently implies that $u$ is injective; this proves the equivalence of (ii) and (v).

An automorphism of the hilbertian space $E$ is also called a *unitary operator*, that is, an operator $u \in \mathcal{L}(E)$ satisfying $uu^* = u^*u = 1_E$.

#### Remark 2 {#evt-v-s4-n1-rem-2 .statement}

— The relation $u^*u = 1_E$ does not characterize all the automorphisms of the hilbertian space $E$. For example, let $E = \ell^2(\mathbf{N})$ and let $u$ be defined by $u(x_n) = x_{n-1}$ for $n \geq 1$ and $u(x)_0 = 0$. We have $\|u(x)\| = \|x\|$ for all $x \in E$, that is, $u^*u = 1_E$, but $u$ is not surjective.

#### Remark 3 {#evt-v-s4-n1-rem-3 .statement}

— The definition (1) of the adjoint $u^*$ can also be written as
$$
\langle y|u(x)\rangle = \langle u^*(y)|x\rangle ,
$$
or, by V, p. 15, as
$$
\langle u(x), y^*\rangle = \langle x, (u^*(y))^*\rangle .
$$
But we also have $\langle u(x), y^*\rangle = \langle x, {}^t u(y^*)\rangle$, hence we can express the adjoint in terms of the transpose,
$$
(u^*(y))^* = {}^t u(y^*) .
$$

### 2. Partially isometric linear mappings

#### Definition 2 {#evt-v-s4-def-2 .statement}

*Let $E$ and $F$ be two hilbertian spaces and $u \in \mathcal{L}(E; F)$. The orthogonal of the kernel of $u$ in $E$ is said to be the initial subspace of $u$ and the closure of the image of $u$ in $F$ is called the final subspace of $u$. The orthoprojector from $E$ (resp. $F$) onto the initial (resp. final) subspace of $u$ is called the initial (resp. final) orthoprojector of $u$.*

Let $P$ be the initial subspace of $u$. Since $E$ is the direct sum of $P$ and of the kernel of $u$, we have $u(P) = u(E)$.

#### Proposition 4 {#evt-v-s4-prop-4 .statement}

(i) *The initial (resp. final) subspace of $u^*$ is equal to the final (resp. initial) subspace of $u$.*

(ii) *Suppose that $E = F$. Let $M$ be a closed vector subspace of $E$ and $M^\circ$ its orthogonal. The relations $u(M) \subset M$ and $u^*(M^\circ) \subset M^\circ$ are equivalent.*

Let $Q = \overline{u(E)}$ be the final subspace of $u$. The orthogonal $Q^\circ$ of $Q$ in $F$ consists of all vectors $y$ such that $\langle u(x)|y\rangle = 0$ for all $x \in E$; this is equivalent to : $\langle x|u^*(y)\rangle = 0$ for all $x \in E$, or to $u^*(y) = 0$. Hence we have $Q^\circ = \mathrm{Ker}\, u^*$, and $Q$ is the initial subspace of $u^*$. Since $u$ is the adjoint of $u^*$, the final subspace of $u^*$ is also the initial subspace of $u$. This proves (i).

The relation $u(M) \subset M$ implies that $u(M)$ is orthogonal to $M^\circ$, and the relation $u^*(M^\circ) \subset M^\circ$ implies that $u^*(M^\circ)$ is orthogonal to $M$. But we have $\langle u(x)|y\rangle = \langle u^*(y)|x\rangle$ for all $x \in M$ and $y \in M^\circ$; hence (ii) follows.

We remark that prop. 4 can be deduced from the general properties of the transpose (II, p. 51, cor. 2) in view of remark 3, V, p. 41.

#### Definition 3 {#evt-v-s4-def-3 .statement}

*Let $E$ and $F$ be two hilbertian spaces. A mapping $u \in \mathcal{L}(E; F)$ is* said to be partially isometric if $\|u(x)\| = \|x\|$ for all $x$ belonging to the initial subspace of $u$.

Let $u \in \mathcal{L}(E; F)$ and let $N$ be its kernel and $I$ its image. To say that $u$ is partially isometric is the same as saying that the linear mapping $\tilde{u}: E/N \to I$ deduced from $u$ is isometric (V, p. 13). Then the subspace $I$ of $F$ is complete, hence closed, and is the final subspace of $u$. Consequently, $u$ induces a hilbertian space isomorphism from the initial subspace of $u$ onto its final subspace.

#### Proposition 5 {#evt-v-s4-prop-5 .statement}

*Let $u \in \mathcal{L}(E; F)$, let $P$ be its initial subspace and $Q$ be the final subspace. Let $p$ (resp. $q$) denote the initial (resp. final) orthoprojector of $u$. Assume that $u$ is partially isometric.*

(i) *The mapping $u^* \in \mathcal{L}(F; E)$ is partially isometric, with initial subspace $Q$ and final subspace $P$. The isomorphism from $P$ onto $Q$ induced by $u$ is then the inverse of the isomorphism from $Q$ onto $P$ induced by $u^*$.*

(ii) *We have $u^*u = p$ and $uu^* = q$.*

On account of prop. 4 (i), assertion (i) is a consequence of (ii).

We now prove (ii). Since $P$ contains the image of $u^*$, the mapping $u^*u$ maps $E$ into $P$. Let $x \in E$ and $y \in P$, then

$$
\langle u^*u(x)|y \rangle = \langle u(x)|u(y) \rangle .
$$

If $x$ belongs to $P$, then $\langle u(x)|u(y) \rangle = \langle x|y \rangle$ by the definition of a partially isometric mapping; if $x$ belongs to the kernel $N$ of $u$, then $u(x) = 0$, hence $\langle u(x)|u(y) \rangle = 0$ and $\langle x|y \rangle = 0$ since $N$ and $P$ are orthogonal. Since $E = P \oplus N$, we have $\langle u^*u(x) - x|y \rangle = 0$ in all the cases, and so $u^*u$ is the orthoprojector $p$ from $E$ onto $P$. That $uu^* = q$ follows by interchanging $u$ and $u^*$ in the above.

#### Proposition 6 {#evt-v-s4-prop-6 .statement}

*For every $u \in \mathcal{L}(E; F)$, the following conditions are equivalent :*

(i) *$u$ is partially isometric ;*
(ii) *$u^*$ is partially isometric ;*
(iii) *$u^*u$ is an orthoprojector ;*
(iv) *$uu^*$ is an orthoprojector ;*
(v) *$uu^*u = u ;*$
(vi) *$u^*uu^* = u^* .*$

By prop. 5, (i) is equivalent to (ii).

(i) $\Rightarrow$ (v) : Suppose $u$ is partially isometric. Then $u^*u$ is the initial orthoprojector of $u$ by prop. 5. Hence for every $x \in E$, $u^*u(x) - x$ belongs to the kernel of $u$, that is, $uu^*u(x) = u(x)$.

(v) $\Rightarrow$ (iii) : Suppose that $uu^*u = u$ and let $p = u^*u$; then $p = p^*$ and $p^2 = p$. Let $M$ (resp. $N$) be the image (resp. the kernel) of $p$. For $x \in M$ and $y \in N$, we have $\langle x|y \rangle = \langle p(x)|y \rangle = \langle x|p^*(y) \rangle = \langle x|p(y) \rangle = 0$. Since $M$ and $N$ are orthogonal, $p$ is the orthoprojector from $E$ onto $M$.

(iii) $\Rightarrow$ (i) : Suppose $p = u^*u$ is an orthoprojector with image $M$ and kernel $N$.

For all $x \in E$, we have
$$
\|u(x)\|^2 = \langle u^*u(x)|x \rangle = \langle p(x)|x \rangle .
$$
Hence $u(x) = 0$ for $x \in N$ and $\|u(x)\| = \|x\|$ for $x \in M$, and so $u$ is partially isometric with kernel $N$ and initial subspace $M$.

We have proved the equivalence of (i), (iii) and (v). Replacing $u$ by $u^*$, we can deduce the equivalence of (ii), (iv) and (vi). This proves prop. 6.

### 3. Normal endomorphisms

#### Definition 4 {#evt-v-s4-def-4 .statement}

Let $E$ be a hilbertian space and $u \in \mathcal{L}(E)$. We say that $u$ is normal if it commutes with its adjoint $u^*$.

For example, every automorphism $u$ of the hilbertian space $E$ is normal since we have $uu^* = u^*u = 1_E$.

#### Proposition 7 {#evt-v-s4-prop-7 .statement}

For $u \in \mathcal{L}(E)$ to be normal, it is necessary and sufficient that $\|u(x)\| = \|u^*(x)\|$ for all $x \in E$.

We define a hermitian form $\Phi$ on $E$ by
$$
\Phi(x, y) = \langle uu^*(x)|y \rangle - \langle u^*u(x)|y \rangle .
$$
For $u$ to be normal, it is necessary and sufficient that $\Phi = 0$. By the polarization formulas (V, p. 2), this is equivalent to $\Phi(x, x) = 0$ for all $x \in E$. The proposition now follows since
$$
\Phi(x, x) = \|u^*(x)\|^2 - \|u(x)\|^2 .
$$

#### Proposition 8 {#evt-v-s4-prop-8 .statement}

Suppose that $u \in \mathcal{L}(E)$ is normal. Let $N$ be the kernel of $u$ and $M$ the orthogonal of $N$ in $E$; let $m$ and $n$ be two positive integers such that $m + n \geq 1$. Then $N$ is the kernel of $u^m(u^*)^n$ and $M$ is both the initial and the final subspace of $u^m(u^*)^n$. In particular, $M$ is both the initial and the final subspace of $u$ and of $u^*$, and is stable under $u$ and $u^*$.

Prop. 7 shows that $u$ and $u^*$ have the same kernel $N$. By prop. 4, (ii) of V, p. 41, the subspace $M$ of $E$ is stable under $u$ and $u^*$ since this is so for $N = M^\circ$, since $M \cap N = \{0\}$, the endomorphisms of $M$ induced by $u$ and $u^*$ are injective. Let $v = u^m(u^*)^n$; the preceding argument shows that the restriction of $v$ to $M$ (resp. $N$) is injective (resp. null), hence $N$ is the kernel of $v$. Consequently, $M = N^\circ$ is the initial subspace of $v$. By prop. 4, (i) of V, p. 41, the final subspace of $v$ is equal to the initial subspace of $v^*$. But $v^* = u^n(u^*)^m$ and so the initial subspace of $v^*$ is equal to $M$ by the preceding.

#### Corollary {#evt-v-s4-n3-cor-1 .statement}

Let $\lambda \in K$. The following subspaces of $E$ are equal :
a) the eigen subspace of $u$ relative to $\lambda$;
b) the eigen subspace of $u^*$ relative to $\overline{\lambda}$;

c) *the primary subspace of u relative to* $\lambda$ (in other words, by LIE, VII, § 1, No. 1, the set of all vectors $x$ of E for which there exists an integer $n \geqslant 0$ such that $(u - \lambda.1_E)^n(x) = 0$);
d) *the primary subspace of* $u^*$ *relative to* $\overline{\lambda}$.

It is clear that $w = u - \lambda.1_E$ is a normal endomorphism of E, hence the endomorphisms $w, w^* = u^* - \overline{\lambda}.1_E, w^n$ and $(w^*)^n$ of E have the same kernel by prop. 8.

### 4. Hermitian endomorphisms

#### Definition 5 {#evt-v-s4-def-5 .statement}

*Let E be a hilbertian space and let* $u \in \mathcal{L}(E)$. *We say that u is hermitian if* $u^* = u$.

Let $\mathcal{H}(E)$ denote the set of all hermitian elements of $\mathcal{L}(E)$; this is a vector subspace of the vector space $\mathcal{L}(E)_{[\mathbf{R}]}$ over $\mathbf{R}$ which is deduced from $\mathcal{L}(E)$ by restricting the scalars.

To each $u \in \mathcal{L}(E)$, we associated (V, p. 16, cor. 2) a sesquilinear form $\Phi_u : (x, y) \mapsto \langle x|u(y)\rangle$ on $E \times E$. We have

$$
\Phi_{u^*}(x, y) = \overline{\Phi_u(y, x)} \quad (x, y \text{ in } E);
$$

consequently, $u$ is hermitian if and only if the form $\Phi_u$ is hermitian. When K is $\mathbf{C}$, it is enough to assume that $\Phi_u(x, x) = \langle x|u(x)\rangle$ is real for all $x \in E$ (V, p. 2, *Remark*).

Let $u \in \mathcal{L}(E)$. We have seen (V, p. 16, cor. 2) that the norm of $u$ can be calculated by the formula

$$
\|u\| = \sup_{\|x\| \leqslant 1, \|y\| \leqslant 1} |\Phi_u(x, y)|.
$$

When $u$ is hermitian, we have the following result :

#### Proposition 9 {#evt-v-s4-prop-9 .statement}

*For every hermitian endomorphism u of* E, *we have*

$$
\|u\| = \sup_{\|x\| \leqslant 1} |\langle x|u(x)\rangle|.
$$

Put $\Phi = \Phi_u$ and $c = \sup_{\|x\| \leqslant 1} |\Phi(x, x)|$, then evidently $c \leqslant \|u\|$. Let $x, y$ be in E such that $\|x\| \leqslant 1, \|y\| \leqslant 1$. Then

$$
\Phi(x + y, x + y) = \Phi(x, x) + \Phi(y, y) + 2\Re\Phi(x, y),
$$
hence
$$
4\Re\Phi(x, y) = \Phi(x + y, x + y) - \Phi(x - y, x - y);
$$
but $|\Phi(t, t)| \leqslant c\|t\|^2$ for all $t \in E$, thus
$$
4|\Re\Phi(x, y)| \leqslant c(\|x + y\|^2 + \|x - y\|^2) = 2c(\|x\|^2 + \|y\|^2) \leqslant 4c.
$$
Let $a = \Phi(x, y)$; there exists a complex number $\lambda$ with absolute value 1 such that

λa = |a|. Replacing y by λy in the preceding inequality, we get $|\Phi(x, y)| \leq c$. By (15), $\|u\| \leq c$ and the proposition follows. Q.E.D.

Evidently every hermitian endomorphism is normal. Conversely :

#### Proposition 10 {#evt-v-s4-prop-10 .statement}

— Suppose K is C. Let $u \in \mathcal{L}(E)$. Then there exists a unique pair $(h_1, h_2)$ of hermitian endomorphisms of E, such that $u = h_1 + ih_2$. In order that u is normal, it is necessary and sufficient that $h_1$ and $h_2$ commute.

For, the relation « $u = h_1 + ih_2,\ h_1^* = h_1,\ h_2^* = h_2$ » is equivalent to

$$
\text{« } h_1 = \frac{1}{2}(u + u^*) \text{ and } h_2 = \frac{i}{2}(u^* - u) \text{ »}.
$$

In addition, we have $h_1 h_2 - h_2 h_1 = \frac{i}{2}(uu^* - u^*u)$. This proves prop. 10.

#### Proposition 11 {#evt-v-s4-prop-11 .statement}

— Let $p \in \mathcal{L}(E)$. In order that p is the orthoprojector from E onto a closed vector subspace of E, it is necessary and sufficient that $p^2 = p = p^*$.

Suppose $p^2 = p$. Let M be the image of p and N its kernel. E is the topological direct sum of M and N. In order that p is an orthoprojector, it is necessary and sufficient that M is orthogonal to N, that is to say that we have $\langle p(x)|y - p(y) \rangle = 0$ for all x, y in E. This latter relation is equivalent to $p = p^*p$, and implies that $p^* = (p^*p)^* = p^*p = p$; conversely if $p^* = p$, we have $p = p^2 = p^*p$.

### 5. Positive endomorphisms

#### Definition 6 {#evt-v-s4-def-6 .statement}

— Let E be a hilbertian space and $u \in \mathcal{L}(E)$. We say that u is positive, and write $u \geq 0$, if u is hermitian and if $\langle x|u(x) \rangle \geq 0$ for all $x \in E$.

When K is equal to C, the relation

$$
\langle x|u(x) \rangle \geq 0 \quad \text{for all } x \in E
$$

implies that u is hermitian (V, p. 2, Remark), hence positive.

Let $\mathcal{L}_+(E)$ denote the set of all positive elements of $\mathcal{L}(E)$; this is a proper pointed convex cone in the real vector space $\mathcal{L}(E)_{[\mathbf{R}]}$ underlying $\mathcal{L}(E)$. In order that u is positive, it is necessary and sufficient that the sesquilinear form $\Phi_u$ on $E \times E$ associated with u is positive hermitian. Given u and v in $\mathcal{L}(E)$, the relation $u - v \geq 0$ can also be written as $u \geq v$ or $v \leq u$; this is an order relation on $\mathcal{L}(E)_{[\mathbf{R}]}$ compatible with its real vector space structure.

#### Proposition 12 {#evt-v-s4-prop-12 .statement}

— Let u be a hermitian (resp. positive) element of $\mathcal{L}(E)$ and let v be a continuous linear mapping from E into a hilbertian space F. Then $vuv^*$ is a hermitian (resp. positive) element of $\mathcal{L}(F)$.

For, we have $(vuv^*)^* = v^{**}u^*v^* = vuv^*$. On the other hand, if $u \geq 0$, we have

$$
\langle y|vuv^*(y) \rangle = \langle v^*(y)|u(v^*(y)) \rangle \geq 0
$$

for all $y \in F$, hence $vuv^* \geq 0$.

Prop. 12 shows, in particular, that $vv^*$ is positive for all $v \in \mathcal{L}(E; F)$. Since, in particular, an orthoprojector $p$ satisfies $p = p^2 = pp^*$, it is positive.

#### Remark 1 {#evt-v-s4-n5-rem-1 .statement}

For every hermitian $u$ in $\mathcal{L}(E)$, put $m(u) = \inf_{\|x\|=1} \langle x|u(x)\rangle$, $M(u) = \sup_{\|x\|=1} \langle x|u(x)\rangle$. If $E$ is not just 0, $m(u)$ and $M(u)$ are finite; moreover, $M(u)$ is the smallest real number $\lambda$ such that $u \leq \lambda \cdot 1_E$ and $m(u)$ the largest real number $\mu$ such that $u \geq \mu \cdot 1_E$. Clearly we have $m(-u) = -M(u)$ and $M(-u) = -m(u)$. It is clear that
$$
\sup(|m(u)|, |M(u)|) = \sup_{\|x\|=1} |\langle x|u(x)\rangle|
$$
and prop. 9 (V, p. 44) implies (for $E \neq \{0\}$) that
$$
\|u\| = \sup(|m(u)|, |M(u)|).
$$
\* For another proof of this formula when $K$ is $\mathbf{C}$, see prop. 14 of TS, I, § 6, No. 8. \*
2) Let $M$ and $N$ be two closed vector subspaces of $E$, and $p_M$ (resp. $p_N$) the orthoprojector from $E$ onto $M$ (resp. $N$). Then $M \subset N$ if and only if $p_M \leq p_N$. For, we have $p_M^* p_M = p_M$, hence
$$
\|p_M(x)\|^2 = \langle p_M(x)|p_M(x)\rangle = \langle x|p_M^* p_M(x)\rangle = \langle x|p_M(x)\rangle
$$
for all $x \in E$. The relation $p_M \leq p_N$ is therefore equivalent to « $\|p_M(x)\| \leq \|p_N(x)\|$ for all $x \in E$ ». If $M \subset N$, we have $p_M = p_M p_N$, hence $\|p_M(x)\| \leq \|p_N(x)\|$ since $\|p_M\| \leq 1$. Conversely, if $\|p_M(x)\| \leq \|p_N(x)\|$ for all $x \in E$, the kernel of $p_M$ contains the kernel of $p_N$, that is, that $M^\circ \supset N^\circ$, which implies that $M \subset N$.

#### Proposition 13 {#evt-v-s4-prop-13 .statement}

— *Let $\mathcal{H}(E)$ be the set of all continuous hermitian endomorphisms of the hilbertian space $E$. Let $\mathcal{F}$ be a non-empty, directed increasing and bounded subset of $\mathcal{H}(E)$.*

(i) *The set $\mathcal{F}$ has an upper bound $u_0$ in $\mathcal{H}(E)$; we have*
$$
\langle x|u_0(x)\rangle = \sup_{u \in \mathcal{F}} \langle x|u(x)\rangle \quad \text{for all} \quad x \in E .
$$

(ii) *The filter of sections of $\mathcal{F}$ converges to $u_0$ in the space $\mathcal{L}(E)$ endowed with the topology of simple convergence.*

Let $\Sigma$ be the filter of sections of $\mathcal{F}$; for every $u \in \mathcal{H}(E)$, let $\Phi_u$ be the continuous hermitian form on $E$ defined by
$$
\Phi_u(x, y) = \langle x|u(y)\rangle .
$$
Let
$$
\Psi_u(x) = \Phi_u(x, x)
$$
for $u \in \mathcal{H}(E)$ and $x \in E$. By the polarization formulas (V, p. 2), we have
$$
\begin{align*}
(19) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) & \text{if } K = \mathbf{R} \\
(20) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) - i\Psi_u(x+iy) + i\Psi_u(x-iy) & \text{if } K = \mathbf{C} .
\end{align*}
$$

For every $x \in E$, the mapping $u \mapsto \Psi_u(x)$ from into $\mathbf{R}$ is increasing and bounded, hence has a limit with respect to $\Sigma$. By the preceding formulas, the limit
$$
\lim_{u,\Sigma} \Phi_u(x, y) = \Phi(x, y)
$$
exists for every pair $(x, y)$ of elements of $E$. It is clear that $\Phi$ is a hermitian form on $E$. If $v_1 \in \mathcal{F}$ and $v_2$ is a bound of $\mathcal{F}$, the hermitian forms $f_1 = \Phi - \Phi_{v_1}$ and $f_2 = \Phi_{v_2} - \Phi$ are positive; there exists a real number $M \geq 0$ such that
$$
f_1(x, x) + f_2(x, x) = \Phi_{v_2 - v_1}(x, x) \leq M \|x\|^2,
$$
hence
$$
f_1(x, x) \leq M \|x\|^2, \quad f_2(x, x) \leq M \|x\|^2 \quad (x \in E);
$$
consequently the semi-norms $x \mapsto f_i(x, x)^{1/2}$ are continuous on $E$. Since
$$
f_2 - f_1 = \Phi_{v_2} + \Phi_{v_1} - 2\Phi,
$$
we conclude that $x \mapsto \Phi(x, x)$ is a continuous function on $E$, and by formulas (19) and (20), that $\Phi$ is continuous on $E \times E$. Therefore there exists (V, p. 16, cor. 2) an element $u_0$ of $\mathcal{H}(E)$ such that $\Phi = \Phi_{u_0}$. Formula (18) is evidently satisfied, hence $u_0$ is the upper bound of $\mathcal{F}$ in $\mathcal{H}(E)$. This proves (i).

We have, by construction
$$
\lim_{u,\Sigma} \langle x|(u_0 - u)(x)\rangle = 0 \quad \text{for all } x \in E.
$$
Let $v_1 \in \mathcal{F}$; given a $u \in \mathcal{F}$ such that $u \geq v_1$, let $v = u_0 - u$. If we apply the Cauchy-Schwarz inequality to the positive hermitian form $\Phi_v$ on $E$, we get
$$
\begin{align*}
\|v(x)\|^4 &= |\Phi_v(v(x), x)|^2 \leq \Phi_v(v(x), v(x)) \cdot \Phi_v(x, x) \\
&= \langle v(x)|v^2(x)\rangle \langle x|v(x)\rangle \leq \|v\|^3 \|x\|^2 \langle x|v(x)\rangle \\
&\leq \|u_0 - v_1\|^3 \|x\|^2 \langle x|v(x)\rangle,
\end{align*}
$$
since $\|v\| \leq \|u_0 - v_1\|$ by V, p. 44, prop. 9. Then by (21) we get $\lim_{u,\Sigma} \|(u_0 - u)(x)\| = 0$ for all $x \in E$; which proves assertion (ii).

In particular, prop. 13 can be applied to the case of an increasing and bounded sequence $(u_n)_{n \in \mathbf{N}}$ of elements of $\mathcal{H}(E)$. Then there exists an element $v$ of $\mathcal{H}(E)$ characterized by
$$
\langle x|v(x)\rangle = \lim_{n \to \infty} \langle x|u_n(x)\rangle = \sup_{n \in \mathbf{N}} \langle x|u_n(x)\rangle \quad (x \in E),
$$
and we have $v(x) = \lim_{n \to \infty} u_n(x)$ for all $x \in E$. Moreover, $v$ is the upper bound of the set of the $u_n$ in $\mathcal{H}(E)$.

### 6. Trace of an endomorphism

Let E and F be two hilbertian spaces. Conforming to the conventions of V, p. 40, we let $ba^*$, for $a$ in E and $b$ in F, denote the continuous linear mapping $x \mapsto b \langle a|x \rangle$ from E into F.

#### Lemma 1 {#evt-v-s4-lem-1 .statement}

*There exists an isomorphism $\theta$ from the vector space $F \otimes E'$ onto the space $\mathcal{L}_f(E; F)$ of all finite rank continuous linear mappings from E into F, characterized by $\theta(b \otimes a^*) = ba^*$ for $a \in E, b \in F$.

By A, II, § 4, No. 2, there exists an injective linear mapping $\theta$ from $F \otimes E'$ into $\mathcal{L}(E; F)$ and only one such, which transforms $b \otimes a'$ into the linear mapping $x \mapsto ba'(x)$ for $a' \in E', b \in F$. Evidently $\theta(b \otimes a^*) = ba^*$, and the image of $\theta$ is contained in $\mathcal{L}_f(E; F)$. However, let $u \in \mathcal{L}_f(E; F)$ and let $(e_1, ..., e_n)$ be an orthonormal basis of the image of $u$ in F. Let $f_i = u^*(e_i)$ for $1 \leq i \leq n$. For every $x \in E$, we have

$$
u(x) = \sum_{i=1}^n \langle e_i|u(x) \rangle \cdot e_i = \sum_{i=1}^n \langle f_i|x \rangle \cdot e_i,
$$

hence $u = \sum_{i=1}^n e_i f_i^* = \theta(\sum_{i=1}^n e_i \otimes f_i^*)$. Therefore the image of $\theta$ is equal to $\mathcal{L}_f(E; F)$.

We shall henceforth assume that $E = F$, and we set $\mathcal{L}_f(E) = \mathcal{L}_f(E; E)$. By lemma 1, there exists a unique linear form $\tau$ on $\mathcal{L}_f(E)$, such that $\tau(\theta(a \otimes a')) = a'(a)$ for $a \in E, a' \in E'$; in other words, we have

(22)
$$
\tau(ba^*) = \langle a|b \rangle \quad \text{for } a, b \text{ in } E.
$$

When E is finite dimensional, we have $\mathcal{L}_f(E) = \mathcal{L}(E)$ and $\tau(u)$ is the *trace* of the endomorphism $u$ of E (A, II, § 4, No. 3).

#### Lemma 2 {#evt-v-s4-lem-2 .statement}

*Let $(e_i)_{i \in I}$ be an orthonormal basis of E. Then*

$$
\tau(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

*for all* $u \in \mathcal{L}_f(E)$.

It is enough to consider the case when $u = ba^*$ with $a, b$ in E. Then

$$
\langle e_i|u(e_i) \rangle = e_i^* b \cdot a^* e_i = \overline{\langle e_i|a \rangle} \langle e_i|b \rangle
$$

and lemma 2 follows from formula (22) and formula (3) of V, p. 22.

#### Lemma 3 {#evt-v-s4-lem-3 .statement}

*Let u be a continuous and positive endomorphism of E, and $\mathcal{F}$ the set of all finite rank orthoprojectors on E. Then for every orthonormal basis $(e_i)_{i \in I}$ of E, we have (in $\mathbf{R}_+$) the equality*

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_{p \in \mathcal{F}} \tau(pup).
$$

For every finite subset J of I, put $p_J = \sum_{i \in J} e_i e_i^*$; this is the orthoprojector from E onto the vector subspace generated by the vectors $e_i$, where i ranges over J. We have
$$
p_J u p_J = \sum_{i \in J, j \in J} \langle e_i | u(e_j) \rangle e_i e_j^* ,
$$
hence $\tau(p_J u p_J) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$. Since $p_J \in \mathcal{F}$,
$$
\sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(p u p) ;
$$
and so we conclude that
$$
\sum_{i \in I} \langle e_i | u(e_i) \rangle = \sup_J \sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(p u p) .
$$

Let $v$ be a finite rank continuous and positive endomorphism of E and let $p \in \mathcal{F}$. By th. 2 of V, p. 23 there exists an orthonormal basis $(f_\alpha)_{\alpha \in A}$ of E and a finite subset B of A such that $(f_\alpha)_{\alpha \in B}$ is an orthonormal basis of the image of p. Then we have $p = \sum_{\alpha \in B} f_\alpha f_\alpha^*$, and so, as above, the relation $\tau(p v p) = \sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle$. By lemma 2 (V, p. 48) we have $\tau(v) = \sum_{\alpha \in A} \langle f_\alpha | v(f_\alpha) \rangle$, which gives the formula
$$
\sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle \leq \tau(v) .
$$
Applying this inequality to the case where $v = p_J . u p_J$ and where J is a finite subset of I, we get
$$
\sum_{\alpha \in B} \langle p_J(f_\alpha) | u p_J(f_\alpha) \rangle \leq \sum_{i \in J} \langle e_i | u(e_i) \rangle .
$$
For every $x \in E$, we have $p_J(x) = \sum_{i \in J} \langle e_i | x \rangle e_i$, and so $x = \lim_J p_J(x)$ with respect to the ordered directed set of finite subsets J of I. Passing to the limit over J in (23), we get
$$
\tau(p u p) = \sum_{\alpha \in B} \langle f_\alpha | u(f_\alpha) \rangle \leq \sum_{i \in I} \langle e_i | u(e_i) \rangle ,
$$
and this completes the proof of lemma 3.

#### Definition 7 {#evt-v-s4-def-7 .statement}

*Let u be a continuous and positive endomorphism of the hilbertian space E. Let*
$$
\operatorname{Tr}(u) = \sup_{p \in \mathcal{F}} \tau(p u p)
$$
*(upper bound in $\overline{\mathbf{R}}_+$), where $\mathcal{F}$ is the set of all finite rank orthoprojectors on E. We say that $\operatorname{Tr}(u)$ is the trace of u.*

Let $p$ be the orthoprojector from $E$ onto a finite dimensional vector subspace of $E$, and let $(x_1, ..., x_m)$ be an orthonormal basis of $F$. We have established the relation
$$
\tau(pup) = \sum_{i=1}^m \langle x_i | u(x_i) \rangle.
$$
Consequently, we can define the trace by the formula
$$
\text{Tr}(u) = \sup_{x_1, ..., x_m} \sum_{i=1}^m \langle x_i | u(x_i) \rangle,
$$
where $(x_1, ..., x_m)$ ranges over the set of all finite orthonormal sequences of vectors of $E$.

By lemma 3 (V, p. 48), we have
$$
\text{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle
$$
for every orthonormal basis $(e_i)_{i \in I}$ of $E$. From this, we deduce
$$
\text{Tr}(u + v) = \text{Tr}(u) + \text{Tr}(v)
$$
$$
\text{Tr}(\lambda u) = \lambda \cdot \text{Tr}(u)
$$
for all continuous and positive endomorphisms $u$ and $v$ of $E$ and for every real number $\lambda \geq 0$ (we make the convention $0.(+\infty) = 0$ in (27)). Let $\phi$ be an isomorphism from $E$ onto a hilbertian space $F$; since $\phi$ transforms every orthonormal basis of $E$ into an orthonormal basis of $F$, we get from (25) that
$$
\text{Tr}(\phi u \phi^{-1}) = \text{Tr}(u).
$$

Let $(u_\alpha)_{\alpha \in A}$ be a non-empty directed increasing and bounded family of continuous and positive endomorphisms of $E$; let $u = \sup_\alpha u_\alpha$, then $\langle x | u(x) \rangle = \sup_\alpha \langle x | u_\alpha(x) \rangle$ for all $x \in E$ (V, p. 46, prop. 13). We have $\text{Tr}(u) = \sup_{J \subset I} \sum_{i \in J} \langle e_i | u(e_i) \rangle$, where $J$ ranges over all finite subsets of $I$, hence
$$
\text{Tr}(u) = \sup_\alpha \text{Tr}(u_\alpha) \quad \text{for} \quad u = \sup_\alpha u_\alpha.
$$

Let $p_F$ be the orthoprojector from $E$ onto the hilbertian subspace $F$; there exists an orthonormal basis $(e_i)_{i \in I}$ of $E$ and a subset $J$ of $I$, such that $(e_i)_{i \in J}$ is an orthonormal basis of $F$. We have $\text{Tr}(p_F up_F) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$. This formula has two consequences : firstly, we have $\text{Tr}(p_F up_F) \leq \text{Tr}(u)$; secondly, taking $u = 1_E$, we get
$$
\text{Tr}(p_F) = \begin{cases}
\dim F & \text{if } F \text{ is finite dimensional} \\
+ \infty & \text{if not}.
\end{cases}
$$

#### Definition 8 {#evt-v-s4-def-8 .statement}

— Let E be a complex hilbertian space. We write $\mathcal{L}^1(E)$ for the vector subspace of $\mathcal{L}(E)$ generated by all continuous, positive endomorphisms of E with finite trace.

By formula (25) of V, p. 50, the trace extends to a linear form on $\mathcal{L}^1(E)$, again denoted by Tr, and satisfying the relation $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$ for all $u$ in $\mathcal{L}^1(E)$ and for every orthonormal basis $(e_i)_{i \in I}$ of E. For every $u \in \mathcal{L}^1(E)$, we have $u^* \in \mathcal{L}^1(E)$ and $\operatorname{Tr}(u^*) = \overline{\operatorname{Tr}(u)}$. Formula (28) of V, p. 50 extends to the case where $u$ belongs to $\mathcal{L}^1(E)$. Let F be a hilbertian subspace of E; by formula (30), the orthoprojector $p_F$ belongs to $\mathcal{L}^1(E)$ if and only if F is finite dimensional. For every $a$ and $b$ in E, we have $4ab^* = \sum_{\varepsilon^4 = 1} \varepsilon(a + \varepsilon b)(a + \varepsilon b)^*$ and $cc^*$ is a positive operator with finite trace for all $c \in E$; consequently, if $u$ is a finite rank, continuous endomorphism of E, then $u \in \mathcal{L}^1(E)$ and $\operatorname{Tr}(u) = \tau(u)$.

Let E be a real hilbertian space, and let $E_{(c)}$ be its complexification (V, p. 5). We identify E with a subset of $E_{(c)}$. Then $\mathcal{L}(E)$ can be identified with a real vector subspace of $\mathcal{L}(E_{(c)})$ consisting of all continuous linear mappings $u$ from $E_{(c)}$ into $E_{(c)}$ such that $u(E) \subset E$. In this case we write $\mathcal{L}^1(E) = \mathcal{L}(E) \cap \mathcal{L}^1(E_{(c)})$. For every $u \in \mathcal{L}^1(E)$, the trace $\operatorname{Tr}(u)$ is real and is equal to $\operatorname{Tr}(u^*)$. Formulas (25) and (28) are again valid, $\mathcal{L}_f(E) \subset \mathcal{L}^1(E)$ and $\operatorname{Tr}(u) = \tau(u)$ for all $u \in \mathcal{L}_f(E)$. Finally, a closed vector subspace F of E is finite dimensional if and only if $p_F$ belongs to $\mathcal{L}^1(E)$.

\* Remark 1. — We shall later define the notion of a nuclear mapping from a Banach space E into a Banach space F. We shall show that when $\mathcal{L}^1(E)$ consists of all nuclear mappings from E into E, then E is a real or complex hilbertian space. \*

#### Proposition 14 {#evt-v-s4-prop-14 .statement}

— Let $E_1, ..., E_n$ be hilbertian spaces, $E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$, and $u_i$ a continuous endomorphism of $E_i$ for $1 \leq i \leq n$. If $u_1, ..., u_n$ are positive, then so is $u = u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$, and

$$
\operatorname{Tr}(u) = \prod_{i=1}^n \operatorname{Tr}(u_i).
$$

If $u_i \in \mathcal{L}^1(E_i)$ for all $1 \leq i \leq n$, then $u \in \mathcal{L}^1(E)$ and formula (31) is again valid in this case.

Proceeding by induction on $n$, we immediately reduce to the case $n = 2$.

For $i = 1, 2$, we define a sesquilinear form $\Phi_i$ on $E_i$ by the formula $\Phi_i(x, y) = \langle x | u_i(y) \rangle$ for $x, y$ in $E_i$. If $u_1$ and $u_2$ are positive, the forms $\Phi_1$ and $\Phi_2$ are hermitian and positive. By prop. 1 of V, p. 25 there exists a positive hermitian form $\Phi$ on the vector space $E_1 \otimes E_2$ such that

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \Phi_1(x_1, y_1) \cdot \Phi_2(x_2, y_2)
$$

for $x_1, y_1$ in $E_1$ and $x_2, y_2$ in $E_2$. We verify immediately the relation $\Phi(z, t) = \langle z | u(t) \rangle$ for $z$ and $t$ in $E_1 \otimes E_2$. Since $\Phi$ is positive, we have $\langle z | u(z) \rangle \geq 0$ for all $z$ in $E_1 \otimes E_2$. Since $u$ is continuous and $E_1 \otimes E_2$ is dense in the hilbertian space $E = E_1 \hat{\otimes}_2 E_2$, we conclude that $u$ is a continuous and positive endomorphism of E.

Let $(e_i)_{i \in I}$ be an orthonormal basis of $E_1$ and $(f_j)_{j \in J}$ an orthonormal basis of $E_2$; then the family $(e_i \otimes f_j)_{i \in I, j \in J}$ is an orthonormal basis of $E$ and we have

$$
\operatorname{Tr}(u) = \sum_{i \in I} \sum_{j \in J} \langle e_i \otimes f_j | u(e_i \otimes f_j) \rangle \\
= \sum_{i \in I} \sum_{j \in J} \langle e_i | u_1(e_i) \rangle \cdot \langle f_j | u_2(f_j) \rangle \\
= \operatorname{Tr}(u_1) \cdot \operatorname{Tr}(u_2) .
$$

In particular, if $u_1$ and $u_2$ are positive endomorphisms with finite trace, then so is $u$. By linearity, we deduce that $u$ belongs to $\mathcal{L}^1(E)$ when $K = \mathbf{C}$ and that the $u_i$ belong to $\mathcal{L}^1(E_i)$ for $i = 1, 2$; formula (31) extends to this case by linearity. Finally, the case when $K = \mathbf{R}$ and the $u_i \in \mathcal{L}^1(E_i)$ reduces to the complex case by extension of the scalars.

#### Remark 2 {#evt-v-s4-n6-rem-2 .statement}

— Let $E$ be a hilbertian space, which is the hilbertian sum of a family $(E_i)_{i \in I}$ of hilbertian subspaces. Let $u$ be an element of $\mathcal{L}(E)$ such that $u(E_i) \subset E_i$ for all $i \in I$; let $u_i$ be the element of $\mathcal{L}(E_i)$ which coincides with $u$ on $E_i$. Then $\operatorname{Tr}(u) = \sum_{i \in I} \operatorname{Tr}(u_i)$ when $u$ is positive, or belongs to $\mathcal{L}^1(E)$; this relation follows from formula (25) of V, p. 50 applied to an orthonormal basis of $E$ which is the union of orthonormal bases of each of the $E_i$.

### 7. Hilbert-Schmidt mappings

#### Definition 9 {#evt-v-s4-def-9 .statement}

*Let $E$ and $F$ be two hilbertian spaces. A continuous linear mapping $u$ from $E$ into $F$ is called a Hilbert-Schmidt mapping if the trace of the positive endomorphism $u^*u$ of $E$ is finite. The set of all Hilbert-Schmidt mappings from $E$ into $F$ is denoted by $\mathcal{L}^2(E, F)$.*

When $E = F$, we write $\mathcal{L}^2(E)$ for $\mathcal{L}^2(E; E)$.

For every $u \in \mathcal{L}(E, F)$, let $\|u\|_2 = \operatorname{Tr}(u^*u)^{1/2}$, so that $u$ belongs to $\mathcal{L}^2(E; F)$ if and only if $\|u\|_2$ is finite. By the definition of the trace, we get

$$
\|u\|_2^2 = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \|u(x_i)\|^2
$$

where $(x_1, \ldots, x_m)$ range over the set of finite orthonormal sequences in $E$. In particular, taking $m = 1$ in formula (32), we have

$$
\|u\| \leq \|u\|_2 \quad (u \in \mathcal{L}(E; F)) .
$$

Let $(e_i)_{i \in I}$ be an orthonormal basis of $E$ and $(f_j)_{j \in J}$ an orthonormal basis of $F$. By formula (25) of V, p. 50 and the Parseval’s relation (V, p. 22), we have

$$
\|u\|_2^2 = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{i,j} |\langle f_j | u(e_i) \rangle|^2 .
$$

Since $|\langle f_j|u(e_i)\rangle| = |\langle e_i|u^*(f_j)\rangle|$, formula (34) implies that
$$
\|u^*\|_2 = \|u\| ;
$$
hence, the adjoint of a Hilbert-Schmidt mapping is a Hilbert-Schmidt mapping. Let $E_1, F_1$ be hilbertian spaces and $v : E_1 \to E, w : F \to F_1$ continuous linear mappings. From (32), we deduce immediately that
$$
\|wu\|_2 \leq \|w\|.\|u\|_2 .
$$
By (35), (36) and the relation $uv = (v^*u^*)^*$, we get
$$
\|uv\|_2 \leq \|u\|_2\,\|v\| .
$$
In particular, if $u$ belongs to $\mathcal{L}^2(E, F)$ then $wuv$ belongs to $\mathcal{L}^2(E_1, F_1)$.

#### Theorem 1 {#evt-v-s4-thm-1 .statement}

*Let E and F be two hilbertian spaces.*
(i) *The set $\mathcal{L}^2(E, F)$ is a vector subspace of $\mathcal{L}(E; F)$ and $u \mapsto \|u\|_2$ is a hilbertian norm* (V, p. 6) *on $\mathcal{L}^2(E; F)$.*
(ii) *The isomorphism $\theta$ from $F \otimes E'$ onto $\mathcal{L}_f(E; F)$ characterized by $\theta(y \otimes x^*) = yx^*$ extends to an isomorphism $\hat{\theta}$ from $F \otimes_2 E'$ onto $\mathcal{L}^2(E; F)$. In particular, $\mathcal{L}_f(E; F)$ is dense in $\mathcal{L}^2(E; F)$.*

Let $(e_i)_{i \in I}$ (resp. $(f_j)_{j \in J}$) be an orthonormal basis of $E$ (resp. $F$). For every $u \in \mathcal{L}(E; F)$, let $\Lambda(u)$ be the matrix of $u$ with respect to chosen orthonormal bases for $E$ and $F$ (V, p. 22). Let $\|a\|_2$ denote the norm of an element $a$ of the hilbertian space $\ell^2(J \times I)$. By formula (34), $\Lambda$ is a mapping from $\mathcal{L}^2(E; F)$ into $\ell^2(J \times I)$ such that $\|\Lambda(u)\|_2 = \|u\|$; it is clear that $\Lambda$ is *injective*. To prove (i), it is enough to prove that $\Lambda$ is *surjective*. Let $a = (a_{ji})$ be an element of $\ell^2(J \times I)$; by Cauchy-Schwarz inequality, we have
$$
|\sum_{j,i} \overline{\eta}_j a_{ji} \xi_i|^2 \leq \sum_{j,i} |a_{ji}|^2 \sum_{j,i} |\overline{\eta}_j \xi_i|^2 = \|a\|_2^2\,\|\xi\|^2\,\|\eta\|^2
$$
for every $\xi = (\xi_i)$ in $\ell^2(I)$ and $\eta = (\eta_j)$ in $\ell^2(J)$. Then there exists a continuous sesquilinear form $\Phi$ on $F \times E$ such that $\Phi(y, x) = \sum_{j,i} \overline{\eta}_j a_{ji} \xi_i$ for $x = \sum_i \xi_i e_i$ in $E$ and $y = \sum_j \eta_j f_j$ in $F$. Let $u \in \mathcal{L}(E; F)$ be such that $\Phi(y, x) = \langle y|u(x)\rangle$ (V, p. 16, cor. 2). We get
$$
a_{ji} = \Phi(f_j, e_i) = \langle f_j|u(e_i)\rangle \quad \text{for} \quad i \in I, j \in J ,
$$
hence $a = \Lambda(u)$.

Since $\Lambda$ is a hilbertian space isomorphism from $\mathcal{L}^2(E; F)$ onto $\ell^2(J \times I)$ and since $(f_j \otimes e_i^*)$ is an orthonormal basis of $F \otimes_2 E'$, there exists an isomorphism $\hat{\theta}$ from $F \otimes_2 E'$ onto $\mathcal{L}^2(E; F)$ such that
$$
\langle f_j|\hat{\theta}(t)\,e_i\rangle = \langle f_j \otimes e_i^*|t\rangle
$$

for every $i \in I,\ j \in I$ and $t \in F \otimes_2 E'$. In particular, for $t = y \otimes x^*$, we find
$$
\langle f_j | \hat{\theta}(y \otimes x^*) e_i \rangle = \langle f_j \otimes e_i^* | y \otimes x^* \rangle = \langle f_j | y \rangle \langle x | e_i \rangle = \langle f_j | y x^* e_i \rangle
$$
hence $\hat{\theta}(y \otimes x^*) = y x^*$. This proves (ii). Q.E.D.

#### Example 1 {#evt-v-s4-n7-exa-1 .statement}

Let I and J be two sets. By the proof given above, in order that a mapping $u$ from $\ell^2(I)$ into $\ell^2(J)$ be a Hilbert-Schmidt mapping, it is necessary and sufficient that there exists a matrix $(a_{ji})$ in $\ell^2(J \times I)$ such that $u(\xi)_j = \sum_{i \in I} a_{ji} \xi_i$ for all $\xi = (\xi_i)$ in $\ell^2(I)$.

#### Example 2 {#evt-v-s4-n7-exa-2 .statement}

Let X and Y be two Hausdorff topological spaces, endowed respectively with positive measures $\mu$ and $\nu$. We can show that the Hilbert-Schmidt mappings from $\mathcal{L}^2(X)$ into $\mathcal{L}^2(Y)$ correspond bijectively to classes of square integrable functions on $Y \times X$; to the class of a function $N \in \mathcal{L}^2(Y \times X, \nu \otimes \mu)$ corresponds the mapping $u_N$ given by
$$
(u_N f)(y) = \int_X N(y, x) f(x) \, d\mu(x)
$$
for $\nu$-almost all $y \in Y$ and $f \in \mathcal{L}^2(X, \mu)$. We have
$$
\| u_N \|_2^2 = \int_X \int_Y |N(y, x)|^2 \, d\mu(x) \, d\nu(y) .
$$

#### Remark 1 {#evt-v-s4-n7-rem-1 .statement}

Suppose $K = \mathbf{C}$. Let $u$ and $v$ be in $\mathcal{L}^2(E; F)$. We have the relation
$$
4\, u^* v = \sum_{\varepsilon^4 = 1} \overline{\varepsilon}(u + \varepsilon v)^* (u + \varepsilon v),
$$
hence $u^* v$ belongs to $\mathcal{L}^1(E)$. The scalar product in the hilbertian space $\mathcal{L}^2(E; F)$ is given by
$$
\langle u | v \rangle = \operatorname{Tr}(u^* v)
$$
since this formula defines a hermitian form on $\mathcal{L}^2(E; F)$ and we get $\langle u | u \rangle = \| u \|_2^2$.

If $u \in \mathcal{L}^2(E; F)$ and $v \in \mathcal{L}^2(F; E)$, then $vu$ belongs to $\mathcal{L}^1(E)$ and $uv$ to $\mathcal{L}^1(F)$ by the preceding; moreover, we have
$$
\operatorname{Tr}(uv) = \operatorname{Tr}(vu) .
$$
By linearity and continuity, it is enough to verify this formula when $u = y_1 x_1^*$ and $v = x_2 y_2^*$ (with $x_1, x_2$ in E, $y_1, y_2$ in F); but then $uv$ is the mapping $y \mapsto y_1 \langle x_1 | x_2 \rangle \langle y_2 | y \rangle$ and $vu$ the mapping $x \mapsto x_2 \langle y_2 | y_1 \rangle \langle x_1 | x \rangle$, and (41) follows from formula (22) of V, p. 48.

Consequently, if $u_1, u_2$ are two elements of $\mathcal{L}^2(E; F)$, we have, in the hilbertian space $\mathcal{L}^2(F; E)$,
$$
\langle u_1^* | u_2^* \rangle = \operatorname{Tr}(u_1 u_2^*) = \operatorname{Tr}(u_2^* u_1) = \langle u_2 | u_1 \rangle = \overline{\langle u_1 | u_2 \rangle} ;
$$
in other words, $u \mapsto u^*$ is an isomorphism from the hilbertian space $\mathcal{L}^2(E; F)$ onto the conjugate (V, p. 6) of the hilbertian space $\mathcal{L}^2(F; E)$. If we identify this conjugate with the dual of $\mathcal{L}^2(F; E)$ (V, p. 15), we see that $\mathcal{L}^2(E; F)$ can be identified with the dual of $\mathcal{L}^2(F; E)$, the canonical bilinear form $(v, u) \mapsto \langle v, u \rangle$ being identified with $(v, u) \mapsto \operatorname{Tr}(vu)$.

#### Remark 2 {#evt-v-s4-n7-rem-2 .statement}

Suppose $K = \mathbf{R}$. We leave it to the reader to verify that formulas (40) and (41) are again valid, and to show that $\mathcal{L}^2(E; F)$ can be identified with the dual of $\mathcal{L}^2(F; E)$ by means of the bilinear form $(u, v) \mapsto \operatorname{Tr}(uv)$.

### 8. Diagonalization of Hilbert-Schmidt mappings

#### Theorem 2 {#evt-v-s4-thm-2 .statement}

*Let E and F be two hilbertian spaces and u a Hilbert-Schmidt mapping from E into F. There exists an orthonormal basis $(e_i)_{i \in I}$ of E which is transformed by u into an orthogonal family in F.*

Let B denote the (closed) unit ball of E, with the weakened topology assigned to it; this is a compact space (V, p. 17). We put $Q(x) = \|u(x)\|^2$ for all $x \in B$. Finally let P denote the set of all vectors x in E satisfying the following property ;

(H) *For every $y \in E$ orthogonal to x, the element $u(y)$ of E is orthogonal to $u(x)$.*

#### Lemma 4 {#evt-v-s4-lem-4 .statement}

*The function $Q : B \to \mathbf{R}$ is continuous.*

Let $(f_j)_{j \in J}$ be an orthonormal basis of F. Put $\lambda_j = \|u^*(f_j)\|^2$ for all $j \in J$. Since $u$ belongs to $\mathcal{L}^2(E; F)$ we have $u^* \in \mathcal{L}^2(F; E)$, hence $\sum_j \lambda_j < +\infty$. Further, we have
$$
Q(x) = \|u(x)\|^2 = \sum_j |\langle u^*(f_j)|x \rangle|^2
$$
by Parseval’s formula (V, p. 22) and the definition of the adjoint (V, p. 38). For every $x \in B$, $|\langle u^*(f_j)|x \rangle|^2 \leq \lambda_j$ by Cauchy-Schwarz inequality; consequently, the convergence of the sum in formula (43) is uniform on B, hence lemma 4 (GT, X, § 1, No. 6).

#### Lemma 5 {#evt-v-s4-lem-5 .statement}

*Let $E_1$ be a closed vector subspace of E, stable under $u^*u$. If $E_1 \neq \{0\}$, then there exists a vector of norm 1 in $E_1 \cap P$.*

Since B is weakly compact, so is the weakly closed subspace $B \cap E_1$ of B. Hence there exists (GT, IV, § 6, No. 1, th. 1) a point $x_0$ in $B \cap E_1$ such that $Q(x_0) \geq Q(x)$ for all $x \in B \cap E_1$. If $Q(x_0) = 0$, we have $Q(x) = 0$ and so $u(x) = 0$ for all $x \in B \cap E_1$. Thus $E_1 \subset P$ and lemma 5 follows in this case.

Suppose now that $Q(x_0) > 0$, then $x_0 \neq 0$. Since the vector $\|x_0\|^{-1} \cdot x_0$ belongs to $B \cap E_1$, we have
$$
Q(x_0) \geq Q(\|x_0\|^{-1} \cdot x_0) = Q(x_0)/\|x_0\|^2
$$
*i.e.* $\|x_0\| = 1$. We shall prove that $x_0$ belongs to P; let $y \in E$ be orthogonal to $x_0$. It is enough to prove that $u(y)$ is orthogonal to $u(x_0)$. But since $y$ is the sum of a vector of $E_1$ and a vector orthogonal to $E_1$, and both orthogonal to $x_0$ (since $x_0 \in E_1$), it is enough to consider the following two cases :

a) $y$ is orthogonal to $E_1$: since $E_1$ is stable under $u^*u$, $u^*u(x_0) \in E_1$, hence $0 = \langle y|u^*u(x_0)\rangle = \langle u(y)|u(x_0)\rangle$.

b) $y$ belongs to $E_1$: for all $t \in \mathbf{R}$, the vector $x(t) = (x_0 + ty)/\|x_0 + ty\|$ belongs to $B \cap E_1$. We have $Q(xt) = f(t)/g(t)$ with
$$
f(t) = \|u(x_0)\|^2 + 2t \Re \langle u(x_0)|u(y)\rangle + t^2 \|u(y)\|^2 \\
g(t) = 1 + t^2 \|y\|^2 .
$$
In view of the definition of $x_0$, we have $Q(x(0)) \geq Q(x(t))$ for all real $t$, hence $\frac{d}{dt} Q(x(t))$ is zero for $t = 0$. But $f(0) = \|u(x_0)\|^2$, $g(0) = 1$, $f'(0) = 2 \Re \langle u(x_0)|u(y)\rangle$, $g'(0) = 0$. Since
$$
\frac{d}{dt} Q(x(t)) = \frac{f'(t)\,g(t) - f(t)\,g'(t)}{g(t)^2},
$$
we conclude that $f'(0) = 0$, that is, $\Re \langle u(x_0)|u(y)\rangle = 0$. When $K = \mathbf{R}$, $u(x_0)$ is orthogonal to $u(y)$, when $K = \mathbf{C}$, the vector $iy$ belongs to $E_1$ and is orthogonal to $x_0$, hence $\mathcal{I} \langle u(x_0)|u(y)\rangle = -\Re \langle u(x_0)|u(iy)\rangle = 0$, and finally $u(x_0)$ is orthogonal to $u(y)$. This proves lemma 5.

Now we prove th. 2. Applying th. 1 of S, III, § 4, No. 5 we see, as in V, p. 23, that there exists a set $S$ which is maximal among the orthonormal subsets of $E$ contained in $P$. Let $E_1$ be the set of all vectors orthogonal to $S$. Let $y \in E_1$; if $x \in S$, the vectors $x$ and $y$ are orthogonal, and since $S \subset P$, we conclude that $u(x)$ and $u(y)$ are orthogonal; then
$$
\langle x|u^*u(y)\rangle = \langle u(x)|u(y)\rangle = 0
$$
and $u^*u(y)$ is orthogonal to $S$. Hence $E_1$ is stable under $u^*u$. If we had $E_1 \neq \{0\}$, there would exist a vector $x$ of norm 1 in $E_1 \cap P$ (lemma 5) and $S \cup \{x\}$ would be an orthonormal subset of $E$ contained in $P$. This would contradict the maximal character of $S$. Hence $E_1 = \{0\}$ and $S$ is an orthonormal basis of $E$. Q.E.D.

#### Corollary 1 {#evt-v-s4-lem-5-cor-1 .statement}

— *Let $v$ be a continuous, positive endomorphism with finite trace of the hilbertian space $E$. There exists an orthonormal basis $(e_i)_{i \in I}$ of $E$ and a summable family of positive real numbers $(\lambda_i)_{i \in I}$ such that $v(e_i) = \lambda_i e_i$ for all $i \in I$.*

Let $\Phi(x, y) = \langle x|v(y)\rangle$ for $x, y$ in $E$. Then $\Phi$ is a positive hermitian form on $E$. There exists (V, p. 8, corollary) a hilbertian space $F$ and a continuous linear mapping $u$ from $E$ into $F$ such that $\Phi(x, y) = \langle u(x)|u(y)\rangle$ for $x, y$ in $E$. In other words, we have $v = u^*u$. By virtue of def. 9 (V, p. 52), $u$ is a Hilbert-Schmidt mapping from $E$ into $F$. By th. 2, there exists an orthonormal basis $(e_i)_{i \in I}$ of $E$ such that the vectors $u(e_i)$ are two by two orthogonal. Let $i \in I$; for every $j \neq i$ in $I$, we have
$$
\langle e_j|v(e_i)\rangle = \langle u(e_j)|u(e_i)\rangle = 0
$$

hence $v(e_i)$ is proportional to $e_i$ and is of the form $\lambda_i e_i$, where $\lambda_i = \langle e_i | v(e_i) \rangle$; then

$$
\lambda_i \geqslant 0 \quad \text{and} \quad \sum_{i \in I} \lambda_i = \operatorname{Tr}(v) < + \infty .
$$

#### Corollary 2 {#evt-v-s4-lem-5-cor-2 .statement}

*Let E be a hilbertian space. Then $\mathcal{L}^1(E) \subset \mathcal{L}^2(E)$.*

The real case reduces to the complex case by the extension of scalars; we can therefore assume that $K = \mathbf{C}$.

Since $\mathcal{L}^2(E)$ is a vector subspace of $\mathcal{L}(E)$, it is enough to prove that every continuous and positive endomorphism $v$ of E with finite trace belongs to $\mathcal{L}^2(E)$. With the notations of cor. 1, we have

$$
\sum_{i \in I} \| v(e_i) \|^2 = \sum_{i \in I} \lambda_i^2 \leq (\sum_i \lambda_i)^2 < + \infty .
$$

#### Corollary 3 {#evt-v-s4-lem-5-cor-3 .statement}

*Let v be a continuous positive endomorphism of the hilbertian space E with a finite trace. There exists a positive Hilbert-Schmidt endomorphism w of E such that $v = w^2$ and such that v commutes with w.*

With the notations of cor. 1, it is enough to consider the endomorphism w which transforms the vector $\sum_{i \in I} \xi_i e_i$ into the vector $\sum_i \lambda_i^{1/2} \xi_i e_i$.

#### Remark {#evt-v-s4-n8-rem-1 .statement}

— With the notations of th. 2, let J be the set of all $i \in I$ such that $u(e_i) \neq 0$. For all $i \in J$, let $\lambda_i = \| u(e_i) \|$ and $f_i = \lambda_i^{-1} u(e_i)$. Then $(e_i)_{i \in J}$ (resp. $(f_i)_{i \in J}$) is an orthonormal basis of the initial (resp. final) subspace of u, we have $u(e_i) = \lambda_i f_i$ for all $i \in J$ and $\sum_{i \in J} \lambda_i^2 = \| u \|_2^2$ is finite.

### 9. Trace of a quadratic form with respect to another

In this section, E will denote a real vector space and Q, H two *positive quadratic forms* on E. There exist two symmetric bilinear forms $(x, y) \mapsto \langle x | y \rangle_Q$ and $(x, y) \mapsto \langle x | y \rangle_H$ on $E \times E$, characterized by

$$
Q(x) = \langle x | x \rangle_Q , \quad H(x) = \langle x | x \rangle_H
$$

for all $x \in E$.

We call *the trace of Q with respect to H*, and write $\operatorname{Tr}(Q/H)$, a real positive number, finite or not, defined as follows :

*a)* If there exists $x \in E$ with $H(x) = 0$ and $Q(x) \neq 0$, we put $\operatorname{Tr}(Q/H) = + \infty$.

*b)* Otherwise, $\operatorname{Tr}(Q/H)$ is the upper bound of the set of all numbers of the form $\sum_{i=1}^m Q(x_i)$ where $(x_1, ..., x_m)$ range over the set of finite sequences of elements of E such that $\langle x_i | x_j \rangle_H = \delta_{ij}$ (Kronecker’s symbol).

#### Remark {#evt-v-s4-n9-rem-1 .statement}

— 1) For every subspace F of E, let $Q_F$ denote the restriction of Q to F and $H_F$ that of H. We have $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ and $\operatorname{Tr}(Q/H)$ is the upper bound of the set of all numbers $\operatorname{Tr}(Q_F/H_F)$ where $F$ ranges over the family of all finite dimensional vector subspaces of $E$.

2) Let $E_1$ be a real vector space, $Q_1$ and $H_1$ two positive quadratic forms on $E_1$ and $\pi : E \to E_1$ a surjective linear mapping. If $Q = Q_1 \circ \pi$ and $H = H_1 \circ \pi$, then $\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$.

#### Proposition 15 {#evt-v-s4-prop-15 .statement}

*Suppose that there exists a real hilbertian space structure on $E$ such that $H(x) = \|x\|^2$ for all $x \in E$. For $\operatorname{Tr}(Q/H)$ to be finite, it is necessary and sufficient that there exists a continuous and positive endomorphism $u$ of $E$ with finite trace, such that $Q(x) = \langle x|u(x)\rangle$ for all $x \in E$; this endomorphism $u$ is unique, and we have*

$$
\operatorname{Tr}(u) = \operatorname{Tr}(Q/H) = \sum_{i \in I} Q(e_i)
$$

*for every orthonormal bases $(e_i)_{i \in I}$ of $E$.*

Suppose that $\operatorname{Tr}(Q/H)$ is finite. For every $x \in E$ of norm 1, we have $H(x) = 1$, hence $Q(x) \leq \operatorname{Tr}(Q/H)$. Therefore, $Q(x) \leq \operatorname{Tr}(Q/H) \cdot \|x\|^2$ for all $x \in E$, and

$$
|\langle x|y\rangle_Q| \leq Q(x)^{1/2} Q(y)^{1/2} \leq \operatorname{Tr}(Q/H) \cdot \|x\| \cdot \|y\|
$$

by the Cauchy-Schwarz inequality. Consequently, the bilinear form $(x, y) \mapsto \langle x|y\rangle_Q$ on $E \times E$ is continuous. There exists (V, p. 16, cor. 2) a mapping $u \in \mathcal{L}(E)$ such that $\langle x|y\rangle_Q = \langle x|u(y)\rangle$. We have $\langle x|y\rangle_Q = \langle y|x\rangle_Q$ for $x, y$ in $E$, hence $u$ is hermitian; and $\langle x|u(x)\rangle = Q(x) \geq 0$, hence $u$ is positive.

Conversely, let $u$ be a continuous and positive endomorphism of $E$ such that $Q(x) = \langle x|u(x)\rangle$ for all $x \in E$. Then

$$
\langle x|u(y)\rangle = \frac{1}{2}(Q(x + y) - Q(x) - Q(y)) = \langle x|y\rangle_Q,
$$

which gives the uniqueness of $u$. By formula (24') (V, p. 50), we get

$$
\operatorname{Tr}(u) = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \langle x_i|u(x_i)\rangle = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m Q(x_i),
$$

where $(x_1, \ldots, x_m)$ range over the set of all finite orthonormal sequences of elements of $E$. By the definition of $\operatorname{Tr}(Q/H)$, we get $\operatorname{Tr}(u) = \operatorname{Tr}(Q/H)$. Finally, for every orthonormal basis $(e_i)_{i \in I}$ of $E$, we have $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i|u(e_i)\rangle$ by formula (25) of V, p. 50, hence $\operatorname{Tr}(u) = \sum_{i \in I} Q(e_i)$.

#### Remark 3 {#evt-v-s4-n9-rem-3 .statement}

Let $E$ and $F$ be two hilbertian spaces and $v$ a linear, not necessarily continuous mapping from $E$ into $F$. Let $H(x) = \|x\|^2$ and $Q(x) = \|v(x)\|^2$ for all $x \in E$. It follows from prop. 15 that $v$ is a Hilbert-Schmidt mapping if and only if $\operatorname{Tr}(Q/H)$ is finite, and then $\operatorname{Tr}(Q/H) = \|v\|_2^2$.

#### Remark 4 {#evt-v-s4-n9-rem-4 .statement}

Suppose $E$ is finite dimensional. When the quadratic form $H$ is invertible, prop. 15 applies. Let $(e_1, \ldots, e_n)$ be a basis of $E$. Put $q_{ij} = \langle e_i|e_j\rangle_Q$ and $h_{ij} = \langle e_i|e_j\rangle_H$ and introduce the matrices $q = (q_{ij})$ and $h = (h_{ij})$. Let $u$ be an endomorphism of $E$ such that $Q(x) = \langle x|u(x)\rangle_H$ for all $x \in E$. We have

$$
\langle x|y\rangle_Q = \langle x|u(y)\rangle_H \quad (x, y \in E),
$$

and hence the matrix of $u$ with respect to the basis $(e_1, ..., e_n)$ of E is equal to $h^{-1} q$. By prop. 15, we have

$$
\text{Tr}(Q/H) = \text{Tr}(h^{-1} q) = \text{Tr}(qh^{-1}) .
$$

If the basis $(e_1, ..., e_n)$ is orthonormal for H, then $h$ is the unit matrix of order $n$, and we get

$$
\text{Tr}(Q/H) = \text{Tr}(q) = \sum_{i=1}^n Q(e_i) ;
$$

so that we get formula (44) in this case.

Now suppose that the quadratic form H is not invertible. Let N be the kernel of H, and let $\pi$ be the canonical mapping from E onto E/N. There exists an invertible quadratic form $H_1$ on E/N such that $H = H_1 \circ \pi$. Let $(e_1, ..., e_n)$ be a sequence of elements of E such that the sequence $(\pi(e_1), ..., \pi(e_m))$ is a basis of E/N, which is orthonormal for $H_1$. Let $(e_1, ..., e_n)$ be a basis of N. Then $(e_1, ..., e_n)$ is a basis of E and we have

$$
H(\xi_1 e_1 + \cdots + \xi_n e_n) = \xi_1^2 + \cdots + \xi_m^2
$$

for all real numbers $\xi_1, ..., \xi_n$.

Suppose that for all $x \in E$, the relation $H(x) = 0$ implies $Q(x) = 0$; in other words, suppose that there exists a quadratic form $Q_1$ on E/N such that $Q = Q_1 \circ \pi$. By remark 2 and prop. 15, we have,

$$
\text{Tr}(Q/H) = Q(e_1) + \cdots + Q(e_m) .
$$

Exercises
