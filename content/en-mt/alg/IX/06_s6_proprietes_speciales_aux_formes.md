---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 6
section_title: Propriétés spéciales aux formes hermitiennes
lang: en
source: alg-ix-fr
pdf_pages: 0088-0112
extraction: ocr
subsections:
    - "no": 1
      title: Bases orthogonales.
      page: 0
      pdf_page: 88
    - "no": 2
      title: Groupe unitaire et groupe orthogonal.
      page: 0
      pdf_page: 91
    - "no": 3
      title: Projecteurs orthogonaux et involutions.
      page: 0
      pdf_page: 93
    - "no": 4
      title: Symétries dans le groupe orthogonal.
      page: 0
      pdf_page: 95
    - "no": 5
      title: Groupe des similitudes.
      page: 0
      pdf_page: 96
    - "no": 6
      title: Géométrie hermitienne.
      page: 0
      pdf_page: 98
statements: 17
exercises: 0
content_sha256: 0a78bb4f9097987044d8c3ed41f08dfb8b84d8c4686fda2d034f7fc2795186ac
translated_from: content/fr/alg/IX/06_s6_proprietes_speciales_aux_formes.md
source_lang: fr
translation_method: machine
source_content_sha256: 47f1f659ab524c37f71e815f6a42017440fa35076b74ec187bcb8b0be0c99277
translation_model: gpt-5-6-mini
translation_run: translate-en-mt-bddeeb87
glossary_version: 34
glossary_terms_sha256: cbd95fa60b6c2f0c6e25b1cf552a6b660a4f403d230e153aeb482a1cd65421d6
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. Special Properties of Hermitian Forms

### 1. Orthogonal Bases.

#### Definition 1 {#alg-ix-s6-def-1 .statement}

Let $\Phi$ be a Hermitian form on $E$. A basis $(e_i)$ of $E$ is said to be orthogonal for $\Phi$ if any two elements of this basis are orthogonal for $\Phi$.

If in addition $\Phi(e_i, e_i) = 1$ for every $i$, the basis $(e_i)$ is said to be orthonormal.

Let $(e_i)$ be an orthogonal basis; if we put $\Phi(e_i, e_i) = \alpha_i$, we have
$$
\Phi(\sum_i \xi_i e_i, \sum_i \eta_i e_i) = \sum_i \xi_i \alpha_i \overline{\eta_i}.
$$

#### Lemma 1 {#alg-ix-s6-lem-1 .statement}

Suppose that $A$ is a field and $\Phi$ a Hermitian form $\neq 0$ on $E$. If all the vectors of $E$ are isotropic, $A$ is a commutative field of characteristic 2, the antiautomorphism $J$ is the identity and $\Phi$ is alternating.

Indeed, on expanding $\Phi(x + y, x + y) = 0$, taking into account the hypotheses $\Phi(x, x) = \Phi(y, y) = 0$, we obtain the relation $\Phi(x, y) = -\overline{\Phi(x, y)}$ for arbitrary $x, y$ in $E$. Since $\Phi$ is $\neq 0$, there exist $x, y$ in $E$ such that $\Phi(x, y) = 1$. Writing that $\Phi(\lambda x, y) = -\Phi(\lambda x, y)$, we obtain $\overline{\lambda} = -\lambda$ for every $\lambda \in A$. Taking first $\lambda = 1$, we see that $A$ is of characteristic 2; the relation $\overline{\lambda} = -\lambda$ then shows that $J$ is the identity, hence $A$ is commutative and $\Phi$ is alternating.

#### Theorem 1 {#alg-ix-s6-thm-1 .statement}

Suppose that $A$ is a field and $E$ a finite-dimensional vector space of dimension $n$ over $A$. Then, for every Hermitian form $\Phi$ on $E$, $E$ admits an orthogonal basis, unless the following conditions are simultaneously satisfied:

(C) $A$ is commutative of characteristic 2, the antiautomorphism $J$ is the identity, $\Phi$ is alternating and nonzero.

Let us reason by induction on $n$, the result being obvious for $n = 0$. We may suppose $\Phi \neq 0$. If (C) is not satisfied, lemma 1 shows that there exists an element $x \in E$ such that $\Phi(x, x) \neq 0$. Let $H$ be the subspace of $E$ orthogonal to $x$; it is of dimension $\geq n - 1$, and, since $x \in \mathbf{H}$, $\mathbf{H}$ is exactly of dimension $n - 1$. If the restriction $\Psi$ of $\Phi$ to $\mathbf{H}$ does not satisfy (C), there exists, by the induction hypothesis, a basis $(e_2, \ldots, e_n)$ of $\mathbf{H}$ which is orthogonal for $\Psi$; putting $e_1 = x$, we obtain an orthogonal basis $(e_1, e_2, \ldots, e_n)$ of $\mathbf{E}$. It remains to examine the case where $\mathbf{A}$ is a commutative field of characteristic 2, where $\mathbf{J}$ is the identity, and where $\Psi$ is alternating and $\neq 0$. There then exist $y, z$ in $\mathbf{H}$ such that $\Psi(y, z) \neq 0$; put $e_1 = x + y$; in order that $x + \lambda z (\lambda \in \mathbf{A})$ be orthogonal to $e_1$, it is necessary and sufficient that $0 = \Phi(x + y, x + \lambda z) = \Phi(x, x) + \lambda \Psi(y, z)$, a condition which determines $\lambda$ uniquely; the scalar $\lambda$ being thus chosen, we have $\Phi(x + \lambda z, x + \lambda z) = \Phi(x, x) \neq 0$, hence the restriction $\Psi'$ of $\Phi$ to the subspace $\mathbf{H}'$ of $\mathbf{E}$ orthogonal to $e_1$ is not alternating; we may consequently apply the induction hypothesis to $\mathbf{H}'$, which proves the theorem.

When (C) is satisfied, there is obviously no orthogonal basis for $\Phi$.

#### Corollary 1 {#alg-ix-s6-thm-1-cor-1 .statement}

*The notations being those of th. 1, suppose in addition that (C) is not satisfied, that $\Phi$ is non-degenerate and that, for every $x \in \mathbf{E}$, there exists $\rho \in \mathbf{A}$ such that $\Phi(x, x) = \rho \bar{\rho}$. Then $\mathbf{E}$ admits an orthonormal basis for $\Phi$*.

So indeed let $(e_i)$ ($i = 1, \ldots, n$) be an orthogonal basis of $\mathbf{E}$. Put $\Phi(e_i, e_i) = \alpha_i$. We have $\alpha_i \neq 0$ for $i = 1, \ldots, n$ since $\Phi$ is non-degenerate. By assumption, there exist elements $\beta_i$ of $\mathbf{A}$ such that $\alpha_i = \beta_i \overline{\beta_i}$ for $i = 1, \ldots, n$; we have $\beta_i \neq 0$. On putting $f_i = \beta_i^{-1} e_i$, we have $\Phi(f_i, f_i) = \beta_i^{-1} \alpha_i \overline{\beta_i^{-1}} = 1$ for all $i$, and $\Phi(f_i, f_j) = 0$ for $i \neq j$. Thus $(f_i)$ is an orthonormal basis.

#### Remark {#alg-ix-s6-n1-rem-1 .statement}

The last assumption of the corollary is satisfied when $\mathbf{J}$ is the identity, and every element of $\mathbf{A}$ is the square of an element of $\mathbf{A}$ (for example when $\mathbf{A}$ is algebraically closed).

#### Corollary 2 {#alg-ix-s6-thm-1-cor-2 .statement}

*Let $\mathbf{A}$ be a field and $R$ a hermitian matrix of order $n$ and of rank $r$ over $\mathbf{A}$. Then, unless the following condition is satisfied:

(C') $\mathbf{A}$ is commutative of characteristic 2, $\mathbf{J}$ is the identity, $R$ is alternating and non-zero,* there exists an invertible matrix $P$ of order $n$ over $A$ such that

$$
tP . R . \overline{P} = \begin{pmatrix}
\alpha_1 & 0 \ldots 0 \ldots 0 \\
0 & \alpha_2 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots \alpha_r \ldots 0 \\
0 & 0 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots 0 \ldots 0
\end{pmatrix}
$$

where $\overline{\alpha}_i = \alpha_i \neq 0$ for $i = 1, \ldots, r$.

#### Proposition 1 {#alg-ix-s6-prop-1 .statement}

*Suppose that $A$ is a commutative field. Let $\Phi$ be a hermitian form on $E$, and let $(x_n)$ ($n = 1, 2, \ldots$) be a sequence (finite or infinite) of linearly independent vectors of $E$ such that, for every $n$, the subspace $E_n = Ax_1 + \cdots + Ax_n$ is non-isotropic. Let $D_{jn}$ ($j \leq n$) be the cofactor of $\Phi(x_j, x_n)$ in the matrix $(\Phi(x_s, x_t))_{(s,t=1,\ldots,n)}$. Then $D_{nn} \neq 0$ for every $n$. Put*

$$
e_n = \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j.
$$

Then, for every $n$, $(e_1, \ldots, e_n)$ is an orthogonal basis of $E_n$ and we have

$$
\Phi(e_n, e_n) = D_{nn}^{-1} D_{n+1, n+1}.
$$

Indeed, since the restriction of $\Phi$ to $E_{n-1}$ is non-degenerate, one has $D_{nn} \neq 0$ (§ 2, prop. 3); note that $D_{11} = 1$ since the determinant of the empty matrix is equal to 1. Formulas (2) imply first that one has $e_n \equiv x_n$ (mod. $E_{n-1}$) for every $n$, and hence that the $e_n$ are linearly independent, and that $(e_1, \ldots, e_n)$ is a basis of $E_n$. For every $j < n$, one has

$$
\Phi(e_n, x_j) = D_{nn}^{-1} \sum_{k=1}^n D_{kn} \Phi(x_k, x_j) = 0
$$

(chap. III, § 6, no. 1, formula (12)); hence $e_n$ is orthogonal to $E_{n-1}$, and in particular to $e_j$ for $j < n$. On the other hand, one has

$$
\Phi(e_n, e_n) = \Phi(e_n, \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j) = \Phi(e_n, x_n) = \Phi(\sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j, x_n)
$$
$$
= D_{nn}^{-1} \sum_{j=1}^n D_{jn} \Phi(x_j, x_n) = D_{nn}^{-1} D_{n+1, n+1}
$$

(chap. III, § 6, no. 1, formula (10)). This proves our assertions.

With the notation of prop. 1, we say that the sequence $(e_n)$ is obtained from the sequence $(x_n)$ by the Gram-Schmidt orthogonalization process.

#### Proposition 2 {#alg-ix-s6-prop-2 .statement}

Let $\Phi$ be a hermitian form on $E$, and let $(e_i)$ $(i = 1, \ldots, n)$ be an orthogonal (resp. orthonormal) basis of $E$ for $\Phi$. Then, for every $p \geqslant 0$, the basis of $\bigotimes^p E$ formed by the $e_{i_1} \otimes \cdots \otimes e_{i_p}$ and the basis $(e_H)$ of $\wedge^p E$ (where $H$ runs through the set of parts with $p$ elements of $\{1, n\}$; cf. chap. III, § 5, no. 6) are orthogonal (resp. orthonormal) for the extensions of $\Phi$ to $\bigotimes^p E$ and $\wedge^p E$ respectively ($§ 1$, no. 9). If, moreover, the mappings associated with $\Phi$ are bijective, the basis $(e'_i)$ of $E^*$ dual to $(e_i)$ is orthogonal (resp. orthonormal) for the inverse form $\widehat{\Phi}$ of $\Phi$ ($§ 1$, no. 7).

The assertions concerning $\bigotimes^p E$ and $\wedge^p E$ follow at once from formulas (35) and (37) of the $§ 1$, no. 9. The assertion concerning the inverse form follows from the fact that the matrix of $\widehat{\Phi}$ with respect to $(e'_i)$ is the inverse of the matrix of $\Phi$ with respect to $(e_i)$ ($§ 1$, no. 10).

### 2. Unitary group and orthogonal group.

Let $\Phi$ be a hermitian form on $E$; the automorphisms of the A-module $E$ which leave $\Phi$ invariant are called unitary automorphisms (or unitary transforms) relative to $\Phi$, and their group is called the unitary group associated with $\Phi$; it is denoted by $\mathbf{U}(\Phi)$. Given a quadratic form $Q \neq 0$ on $E$, the automorphisms of the A-module $E$ which leave $Q$ invariant are called orthogonal automorphisms (or orthogonal transforms) relative to $Q$; their group is called the orthogonal group associated with $Q$; it is denoted by $\mathbf{O}(Q)$.

Every orthogonal transform for a quadratic form $Q$ is unitary for the bilinear form associated with $Q$. The converse is true when the scalar 2 is not equal to 0 or a divisor of zero in $A$ ($§ 3$, n° 4, (13)), for example if $A$ is a field of characteristic $\neq 2$.

Consider, in particular, on the module $E = A^n$, the hermitian form $\Phi_0$ whose matrix with respect to the canonical basis (e_i) of E is the unity matrix $I_n$. The unitary automorphisms associated with $\Phi_0$ are simply called *automorphisms* (or *transforms*) *unitary in n variables*; their group is called the *unitary group in n variables* and is sometimes denoted by $\mathbf{U}(n, A)$ or $\mathbf{U}_n(A)$. The matrix $U$ of a unitary automorphism with respect to $(e_i)$ is called a *unitary matrix*. Such a matrix is invertible, and satisfies, according to formula (48) of § 1, n° 10, the relation

$$(4)$$
$$
{}^t U \cdot \overline{U} = I_n;
$$

conversely, if A is a commutative ring or is a field, a matrix $U$ which satisfies (4) is invertible, and is then unitary.

When J is the identity and 2 is neither equal to 0 nor a divisor of 0 in A, the terms *orthogonal group in n variables*, *orthogonal automorphism* (or *orthogonal transform*) *in n variables* and *orthogonal matrix* are used instead of the preceding terms, and one writes $\mathbf{O}(n, A)$ (resp. $\mathbf{O}_n(A)$) instead of $\mathbf{U}(n, A)$ (resp. $\mathbf{U}_n(A)$). Relation (4) then reads

$$(5)$$
$$
{}^t U \cdot U = I_n
$$

and, since A is commutative, it is a necessary and sufficient condition for $U$ to be an orthogonal matrix.

#### Proposition 3 {#alg-ix-s6-prop-3 .statement}

*Suppose that A is a commutative field and that E is of finite dimension $> 0$. Let $\Phi$ be a non-degenerate hermitian form on E. The mapping $u \to \det u$ is a homomorphism of the unitary group $\mathbf{U}(\Phi)$ associated with $\Phi$ onto the multiplicative subgroup H of A formed by the elements $\rho$ such that $\rho \overline{\rho} = 1$ (subgroup reduced to $\{1, -1\}$ when J is the identity).*

So let $u$ be an element of $\mathbf{U}(\Phi)$, $U$ its matrix with respect to a basis of E, and $R$ the matrix of $\Phi$ with respect to this basis. The relation $R = {}^t U \cdot R \cdot \overline{U}$ ($§ 1$, n° 10, formula (48)) shows that $(\det U)(\det \overline{U}) = 1$ since $R$ is invertible; whence $(\det u)(\det u) = 1$. The homomorphism $u \to \det u$ maps $\mathbf{U}(\Phi)$ onto H. Indeed, when A has characteristic 2 and J is the identity, H is reduced to the element 1. Otherwise there exists an orthogonal basis $(e_i)$ ($i = 1, \ldots, n$) of E (th. 1); for every $\rho \in A$ such that $\rho \overline{\rho} = 1$, let $u$ be the automorphism of E defined by $u(e_1) = \rho e_1$ and $u(e_i) = e_i$ for $i = 2, \ldots, n$; then $u$ is unitary and $\det u = \rho$, whence the proposition.

Under the conditions of prop. 3, the kernel of the homomorphism $u \to \det u$ is a normal subgroup of $\mathbf{U}(\Phi)$, called the special unitary group associated with $\Phi$; it is sometimes denoted by $\mathbf{SU}(\Phi)$.

When $J$ is the identity and $A$ is not of characteristic 2, this group is also called the special orthogonal group associated with $\Phi$ (or with the quadratic form $Q(x) = \Phi(x, x)$) and is sometimes denoted by $\mathbf{SO}(Q)$.

If $E = A^n$ and $\Phi$ is the form whose matrix with respect to the canonical basis of $E$ is the unit matrix, the notations $\mathbf{SU}(n, A)$ or $\mathbf{SU}_n(A)$ and $\mathbf{SO}(n, A)$ or $\mathbf{SO}_n(A)$ are used.

### 3. Orthogonal projectors and involutions.

Throughout this No., we suppose that the scalar 2 is invertible in $A$ (for example, that $A$ is a field of characteristic $\neq 2$), and that $\Phi$ is a non-degenerate hermitian form on $E$. We denote by $\frac{1}{2}$ the inverse of 2.

#### Lemma 2 {#alg-ix-s6-lem-2 .statement}

For an endomorphism $u$ of $E$ to be such that $u^2 = 1$, it is necessary and sufficient that $\frac{1}{2}(1 - u)$ be a projector in $E$; then $u$ is the difference of the two projectors $\frac{1}{2}(1 + u)$ and $\frac{1}{2}(1 - u)$.

Indeed, in the ring $\mathcal{L}(E)$, the relation $\left( \frac{1}{2}(1 - u) \right)^2 = \frac{1}{2}(1 - u)$ is equivalent to $u^2 = 1$. The rest is trivial.

An endomorphism $u$ of $E$ such that $u^2 = 1$ (which is then necessarily an automorphism of $E$ equal to its inverse) is called an involution. Put $\varphi = \frac{1}{2}(1 - u)$, $U^- = \varphi(E)$, $U^+ = \varphi^{-1}(0)$ ($= \omega(E)$ on putting $\omega = \frac{1}{2}(1 + u)$); it is known that $E$ is the direct sum of $U^+$ and $U^-$ (Chap. VIII, § 1, No. 1), and we have $u(x) = x$ in $U^+$, $u(x) = -x$ in $U^-$. When $A$ is a field and $E$ is finite-dimensional, it follows, since $A$ is of characteristic $\neq 2$, that the only eigenvectors $\neq 0$ of $u$ are the elements ≠ 0 in U^+ or in U^-; they correspond respectively to the eigenvalues + 1 and -1.

#### Proposition 4 {#alg-ix-s6-prop-4 .statement}

Let u ∈ GL(E) be an involution. The following properties are equivalent:
a) u belongs to the unitary group associated with Φ ;
b) the submodules U^+ = $\frac{1}{2}(1 + u)(E)$ and U^- = $\frac{1}{2}(1 - u)(E)$
are orthogonal (and consequently non-isotropic).
Moreover, if A is a field and E is finite-dimensional, properties a) and b) are equivalent to:
c) u = u*.
Indeed, for x ∈ U^+ and y ∈ U^-, the relation $\Phi(u(x), u(y)) = \Phi(x, y)$
gives $2\Phi(x, y) = 0$, hence a) implies b). Conversely, we obviously have $\Phi(u(x), u(y)) = \Phi(x, y)$ when x and y both belong to U^+ or both belong to U^-, and, in view of b), this relation is still true when one of them belongs to U^+ and the other to U^-; since E is the direct sum of U^+ and U^-, we see that b) implies a). Finally, when E is a finite-dimensional vector space, the adjoint u* is defined since Φ is non-degenerate; relation a) is equivalent to $uu^* = 1$ (§ 1, No. 8, cor. of prop. 8); since $u^2 = 1$ by assumption, a) and c) are equivalent.

#### Corollary 1 {#alg-ix-s6-prop-4-cor-1 .statement}

Suppose that A is a field and that E is finite-dimensional. The mapping $u \to \frac{1}{2}(1 + u)(E)$ is a bijection from the set of involutions u belonging to the unitary group associated with Φ onto the set of non-isotropic subspaces of E; the subspace U^+ corresponding to u is the set of elements of E invariant under u.

By prop. 4, it suffices to show that every non-isotropic subspace M of E is the set of vectors invariant under an involution $u \in \mathbf{U}(\Phi)$, and that the latter is unique. Now E is the direct sum of M and M^0 (§ 4, No. 1, cor. of prop. 1), and necessarily $u(x) = x$ for $x \in M$ and $u(x) = -x$ for $x \in M^0$ by virtue of prop. 4; these relations determine u uniquely, and the endomorphism u thus determined obviously answers the question (prop. 4).

We say that the involution $u$ thus determined is the symmetry with respect to the non-isotropic subspace M.

#### Corollary 2 {#alg-ix-s6-prop-4-cor-2 .statement}

Suppose that $\mathbf{A}$ is a field and that $\mathbf{E}$ is finite-dimensional. In order that a projector $\nu$ in $\mathbf{E}$ be such that $\nu(\mathbf{E})$ and $\nu(0)$ are orthogonal (and consequently non-isotropic), it is necessary and sufficient that $\nu = \nu^*$.

It suffices to apply prop. 4 to the involution $u = 1 - 2\nu$.

A projector satisfying the condition of Corollary 2 is called an orthogonal projector for $\Phi$.

### 4. Symmetries in the orthogonal group.

Unless expressly stated otherwise, we suppose, in this No., that $\mathbf{A}$ is a commutative field of characteristic $\neq 2$, and that $\Phi$ is the symmetric bilinear form associated with a non-degenerate quadratic form Q on $\mathbf{E}$. Recall that we have $\Phi(x, x) = 2Q(x)$ for $x \in \mathbf{E}$ (§ 3, No. 4).

Let $H$ be a non-isotropic hyperplane in $\mathbf{E}$, and let $u$ be the symmetry with respect to $H$ (No. 3). Let $a \neq 0$ be a vector orthogonal to $H$; by hypothesis, $u(a) = -a$. Every vector $x \in \mathbf{E}$ can be written in one and only one way in the form $x = \lambda a + y$ with $\lambda \in \mathbf{A}$ and $y \in \mathbf{H}$; since $a$ and $y$ are orthogonal, we have $\Phi(x, a) = \lambda \Phi(a, a)$, whence, since $a$ is non-isotropic (§ 4, No. 1, cor. of Prop. 1), $\lambda = \Phi(x, a)\Phi(a, a)^{-1}$. Consequently, we have

$$
u(x) = \lambda u(a) + u(y) = -\lambda a + y = x - 2\lambda a,
$$

whence

$$
u(x) = x - 2\Phi(x, a)\Phi(a, a)^{-1}.a = x - \Phi(x, a)Q(a)^{-1}.a.
$$

It should be noted that the last member of (6) still has a meaning when $\mathbf{A}$ is a field of characteristic 2, and $a$ a non-singular vector of $\mathbf{E}$; it is immediately verified that one still has then $Q(u(x)) = Q(x)$ for all $x \in \mathbf{E}$, in other words $u \in \mathbf{O}(Q)$. The involution $u$ thus defined is again called the symmetry with respect to the hyperplane orthogonal to $a$ (cf. exerc. 28).

#### Proposition 5 {#alg-ix-s6-prop-5 .statement}

Suppose the vector space $\mathbf{E}$ to be of finite dimension n. The orthogonal group $\mathbf{O}(Q)$ associated with $Q$ is then generated by the symmetries with respect to the non-isotropic hyperplanes of $\mathbf{E}$.

The proposition being obvious for $n = 0$, we reason by induction on $n$. Let $u$ be an orthogonal transformation of $E$, and let $x$ be a non-isotropic vector of $E$ (Lemma 1); distinguish three cases:

a) First suppose that $u(x) = x$. Then the hyperplane $H$ orthogonal to $x$ is non-isotropic, and we have $u(H) = H$. The restriction $u'$ of $u$ to $H$ therefore belongs to the orthogonal group $O(Q')$ associated with the restriction $Q'$ of $Q$ to $H$. The induction hypothesis entails, since $Q'$ is non-degenerate, that we have $u' = v_1' \ldots v_m'$, where $v_i'$ is a symmetry with respect to a hyperplane $L_i$ of $H$. The endomorphism $v_i$ of $E$ which extends $v_i'$ and is such that $v_i(x) = x$ is then the symmetry with respect to the hyperplane $Ax + L_i$ of $E$. Obviously $u = v_1 v_2 \ldots v_m$.

b) In the second place, suppose that $u(x) = -x$. If $s$ denotes the symmetry with respect to the hyperplane $H$ orthogonal to $x$, and if we put $v = su$, we have $v(x) = x$, and we are reduced to case a).

c) Finally, let us pass to the general case, and put $y = u(x)$, so that $Q(y) = Q(x)$. Under these conditions, the vectors $x - y$ and $x + y$ cannot both be isotropic, for, from the relations $Q(x - y) = 0$ and $Q(x + y) = 0$, we would deduce, on adding member to member, $2(Q(x) + Q(y)) = 0$ ($§ 3$, no 4, déf. 2), whence $4Q(x) = 0$, contrary to the assumption. Suppose, for example, that $a = x - y$ is not isotropic; we then have

$$
\Phi(y, a) = Q(y + a) - Q(y) - Q(a) = Q(x) - Q(y) - Q(a) = -Q(a);
$$

consequently, if $s$ denotes the symmetry with respect to the hyperplane orthogonal to $a$, formula (6) proves that $s(y) = y + a = x$; on putting $v = su$, we have $v(x) = x$, and we are reduced to case a). If $a = x - y$ is isotropic and $b = x + y$ is not isotropic, we see analogously that we are reduced to case b).

### 5. Group of similitudes.

Let $\Phi$ be a hermitian form on $E$. An automorphism $u$ of the $A$-module $E$ is called a similitude (relative to $\Phi$) if there exists an invertible element $\alpha$ of $A$ such that

$$
\Phi(u(x), u(y)) = \alpha \Phi(x, y)
$$

for all $x, y$ in $E$. The similitudes form a group $\Gamma$.

When $\Phi$ takes values which are regular elements of $A$ (for example when $A$ is a field and $\Phi \neq 0$), the element $\alpha$ of $A$ satisfying (7) is uniquely determined by $u$; it is called the *multiplier* of the similitude $u$. Replacing $x$ by $\lambda x$ in (7), one sees then that $\alpha$ belongs to the *center* of $A$; exchanging $x$ and $y$ in (7), one sees in addition that $\overline{\alpha} = \alpha$. If, for $u \in \Gamma$, one denotes by $\alpha(u)$ the multiplier of $u$, the mapping $u \to \alpha(u)$ is a homomorphism of $\Gamma$ into the multiplicative group of the invertible elements of the center of $A$. The kernel of this homomorphism is the unitary group associated with $\Phi$, which is therefore a normal subgroup of $\Gamma$. Let $\beta$ be an invertible element of the center of $A$, $\nu$ the homothety of ratio $\beta$, and $\omega$ a unitary automorphism of $E$; then $\nu \omega = \omega \nu$ is a similitude of $E$, and its multiplier is $\beta \overline{\beta}$. Conversely, let $u$ be a similitude whose multiplier is of the form $\beta \overline{\beta}$ ($\beta$ denoting an invertible element of the center of $A$); then $u \nu^{-1}$ is a unitary automorphism $\omega$, and hence $u$ is of the form $\nu \omega$.

Suppose now that $A$ is a field, $E$ a finite-dimensional vector space, and that $\Phi$ is non-degenerate. For every similitude $u$ of multiplier $\alpha$ one has
$$
\Phi(x, \alpha y) = \alpha \Phi(x, y) = \Phi(u(x), u(y)) = \Phi(x, u^*(u(y))),
$$
hence $u^* u$ is the homothety of ratio $\alpha$. If $A$ is commutative, and if $n$ denotes the dimension of $E$, one deduces from this and from formula (50) of § 1, No. 10 that one has
$$
(\det u)(\overline{\det u}) = \alpha^n.
$$

Distinguish then two cases:
1°) The integer $n$ is *odd*, that is, $n = 2q + 1$. Then, putting $\rho = \alpha^{-q} (\det u)$, we have $\alpha = (\det u) (\det u)^{-2q} = \rho \overline{\rho}$. Hence $u$ is the product of the homothety of ratio $\rho$ and a unitary automorphism.
2°) The integer $n$ is *even*, that is, $n = 2q$. Then, putting $\rho = \alpha^{-q} (\det u)$, we have $\rho \overline{\rho} = 1$. In particular, when $J$ is the identity, we have $(\det u)^2 = \alpha(u)^{2q}$; the similitudes $u$ such that $\det u = \alpha(u)^q$ (resp. $\det u = -\alpha(u)^q$) are called *direct* (resp. *inverse*); the direct similitudes form a normal subgroup of index 2 of $\Gamma$;

the homotheties of ratio $\neq 0$ are direct similitudes; the same is true of the orthogonal transformations of determinant 1 (No. 2); the orthogonal transformations of determinant -1 are inverse similitudes.

The preceding definitions and results are still valid for $\varepsilon$-hermitian forms ($§ 3$, No. 1), and in particular for alternating forms.

Let A be a commutative field and Q a quadratic form $\neq 0$ on E. A similitude (relative to Q) is any automorphism $u$ of E such that there exists a nonzero element $\alpha$ of A (called the multiplier of $u$) for which $Q(u(x)) = \alpha Q(x)$ for every $x \in E$. It is clear that $u$ is then a similitude with multiplier $\alpha$ relative to the bilinear form associated with Q; the converse is true when the characteristic of A is $\neq 2$.

### 6. Hermitian Geometry.

#### Definition 2 {#alg-ix-s6-def-2 .statement}

Let A be a field, L an affine space over A and T the space of translations of L (Chapter II, 2nd ed., App. II). If T is endowed with a non-degenerate hermitian form $\Phi$, L is said to be a hermitian space over A, and $\Phi$ the metric form of L.

If J is the identity (which implies that A is commutative), L is rather called a Euclidean space.

If $a$ and $b$ are two points of L, put $e(a, b) = \Phi(b - a, b - a)$. Let c be a third point of L. For $b - a$ and $c - a$ to be orthogonal, it is necessary, by formula (17) of $§ 1$, No. 5, that we have $e(b, c) = e(a, b) + e(a, c)$, and this condition is sufficient when $J = 1$ and A is not of characteristic 2 (“Pythagorean theorem”).

Two linear varieties of L are said to be orthogonal if their directions (Chapter II, 2nd ed., App. II, No. 3) are orthogonal. A linear variety of L is said to be isotropic (resp. totally isotropic) if its direction is isotropic (resp. totally isotropic). A vector of T is said to be orthogonal to a linear variety of L if it is orthogonal to the direction of that variety.

Let V be a linear variety in L, and $x$ a point of L. The set of points $y$ of L such that $y - x$ is orthogonal to V is a linear variety W passing through $x$; W is said to be the totally orthogonal variety (or, more simply, the orthogonal variety) to V passing through x. If L is of finite dimension, the dimension of W is equal to the codimension of V. Moreover, if V is nonisotropic, the directions of V and W are supplementary (§ 4, No. 1, cor. of prop. 1); then W meets V in a single point $x_1$; taking an origin in V, one sees at once that, for fixed V, the mapping $x \to x_1$ is an affine idempotent linear mapping; it is called the orthogonal projection of L onto V; the linear mapping associated with it (Chapter II, 2nd ed., App. II, No. 4) is the orthogonal projector of T onto the direction of V (No. 3).

#### Definition 3 {#alg-ix-s6-def-3 .statement}

Let L be a hermitian space over a field A, T the space of translations of L. A displacement (resp. similitude) of L is any affine bijection u of L onto L such that the linear mapping $\varphi$ associated with u in T (Chapter II, 2nd ed., App. II, No. 4) is unitary (resp. is a similitude).

The group of translations is a normal subgroup of the affine group; it is therefore a normal subgroup of the group of similitudes and of the group of displacements. For every $a \in L$, let $G_a$ be the group of similitudes (resp. displacements) leaving a fixed; if L is identified with T by taking a as origin, $G_a$ is the group of similitudes (resp. the unitary group) of T. Every similitude (resp. displacement) u can be written, in one and only one way, in the form $u = u_1 t_1$ where $u_1 \in G_a$ and $t_1 \in T$, and also in the form $u = t_2 u_2$ where $u_2 \in G_a$ and $t_2 \in T$; moreover $u_2 = u_1$ and $t_2 = u_1 t_1 u_1^{-1}$ (Chapter II, 2nd ed., App. II, No. 4).

Let $u$ be a similitude in L, $\varphi$ the associated similitude in T. The multiplier of $\varphi$ is also called the multiplier of $u$ (No. 5). If this multiplier is denoted by $\alpha(u)$, the mapping $u \to \alpha(u)$ is a homomorphism of the group of similitudes of L into the multiplicative group of the invertible elements of the center of A; its kernel is the group of displacements, which is therefore a normal subgroup of the group of similitudes. When A is commutative and L is of finite dimension, there are, between the determinant det $u$ (equal by definition to det $\varphi$) and $\alpha(u)$, the same relations as in No. 5. The displacements $u$ such that det $u = 1$ form a normal subgroup of the group of displacements; this subgroup is of index 2 if A is a commutative field of characteristic $\neq 2$ and J is the identity.

#### Proposition 6 {#alg-ix-s6-prop-6 .statement}

*Let L be a finite-dimensional hermitian space over A, whose metric form has index 0. Any similitude u of L, with multiplier $\mu \neq 1$, then admits one and only one fixed point.*

Indeed, let $a$ be a point of L. There exists a similitude $\varphi$ of L leaving $a$ fixed and a translation $t$ of L such that $u = t \varphi$. Saying that $b$ is a fixed point of $u$ amounts to saying that $\varphi(b) - b = t$. To show that this equation admits one and only one solution $b$, identify L with its space of translations T by taking $a$ as origin. It is then enough to prove that the endomorphism $\varphi - 1$ of T is invertible, in other words that the relation $\varphi(x) - x = 0$ ($x \in T$) implies $x = 0$. Now, if $\varphi(x) - x = 0$, we have $\Phi(x, x) = \Phi(\varphi(x), \varphi(x)) = \mu \Phi(x, x)$, hence $\Phi(x, x) = 0$ since $\mu \neq 1$; this implies $x = 0$ since $\Phi$ has index 0. QED.

Suppose that A is a field of characteristic $\neq 2$. Every displacement $u$ of L such that $u^2 = 1$ admits at least one fixed point, for example the midpoint $\frac{1}{2}(x + u(x))$ of two homologous points; by taking this point as origin, one sees that the unitary automorphism of T associated with $u$ is a symmetry (No. 3). Let V be a non-isotropic linear variety in L; a displacement $u$ is said to be the *symmetry with respect to V* if, by taking an origin in V, $u$ is identified with the symmetry with respect to V of T. This amounts to saying that $u(x)$ is obtained in the following way: denoting by $x_1$ the orthogonal projection of $x$ on V, one has $u(x) - x = 2(x_1 - x)$.

*Exercises.* — 1) Suppose that A is a commutative field. Given a hermitian matrix $R$ of order $n$ over A, the *principal minors* of order $r$ of $R$ are called the minors obtained by deleting in $R$ $n - r$ rows and the $n - r$ columns of *the same indices*.

a) If a principal minor of order $r$ of $R$ is not zero, but if all the principal minors of orders $r + 1$ and $r + 2$ which contain this minor of order $r$ are zero, now prove that $R$ is of rank $r$ (cf. Chapter III, § 7, Exercise 1 and § 8, Exercise 11 and Chapter IV, § 2, Exercise 10). Deduce that, in order that $R$ be of rank $r$, it is necessary and sufficient that there exist a principal minor of order $r$ which is $\neq 0$, and that all the principal minors of orders $r + 1$ and $r + 2$ be zero.

b) Deduce from a) that if $R$ is of rank $r$, there exists a permutation $\sigma \in \mathfrak{S}_n$ such that, if the same permutation $\sigma$ is performed on the rows and columns of $R$, and if $S$ denotes the matrix obtained, and $\Delta_k$ the principal minor of order $k$ of $S$ obtained by suppressing in $S$ the rows and columns of index $> k$, the following two properties hold: $1^\circ \Delta_r \neq 0$; $2^\circ$ there is no index $k < r$ such that $\Delta_k = \Delta_{k+1} = 0$.

2) Suppose that $A$ is a commutative field, and that $E$ is of finite dimension $n$. Let $\Phi$ be a hermitian sesquilinear form on $E$, satisfying condition (T) of § 4, No. 2, $R = (\alpha_{ij})$ the matrix of $\Phi$ with respect to a basis $(e_i)$ of $E$.

a) If $\Phi$ is of rank $r$, and if the principal minor (Exercise 1) obtained by suppressing in $R$ the rows and columns of indices $> r$ is not zero, show that there exists a new basis $(f_i)$ of $E$ such that $e_i = f_i$ for $1 \leq i \leq r$ and that the matrix of $\Phi$ with respect to $(f_i)$ is obtained by replacing by 0 in $R$ all the $\alpha_{ij}$ such that $i > r$ or $j > r$ (consider the subspace $E^0$ orthogonal to $E$).

b) Deduce from a) that if $\Phi$ is of rank $n$, and if the cofactor $\Delta_{n-1}$ of $\alpha_{nn}$ in the determinant $\Delta = \det R$ is not zero, there exists a new basis $(f_i)$ of $E$ such that $f_i = e_i$ for $1 \leq i \leq n-1$, and such that

$$
\Phi(x, y) = \Phi\left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-1} \sum_{j=1}^{n-1} \alpha_{ij} \xi_i \overline{\eta_j} + \frac{\Delta}{\Delta_{n-1}} \xi_n \overline{\eta_n}
$$

(consider the hermitian form whose matrix with respect to $(e_i)$ is obtained by replacing $\alpha_{nn}$ by $\alpha_{nn} - \frac{\Delta}{\Delta_{n-1}}$ in $R$).

c) Suppose that $\Phi$ is of rank $n$, that $\Delta_{n-1} = 0$, but that the principal minor $\Delta_{n-2}$ of $R$ obtained by deleting the rows and columns with indices $n-1$ and $n$ in $R$ is not zero. Now prove that there exists a new basis $(f_i)$ of $E$ such that $f_i = e_i$ for $1 \leq i \leq n-2$, and such that

$$
\Phi(x, y) = \left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-2} \sum_{j=1}^{n-2} \alpha_{ij} \xi_i \overline{\eta_j} + \xi_{n-1} \overline{\eta_n} + \xi_n \overline{\eta_{n-1}}.
$$

(If $H$ is the hyperplane generated by $e_1, \ldots, e_{n-1}$, which is isotropic, observe that the right orthogonal to $H$ is not in the subspace generated by $e_1, \ldots, e_{n-2}$, and use Prop. 2 of § 4, No. 2).

3) Let $A$ be a finite field, $E$ a finite-dimensional vector space over $A$, $\Phi$ a non-degenerate hermitian sesquilinear form on $E$, relative to an automorphism $J \neq 1$ of $A$. Now prove that $E$ admits an orthonormal basis for $\Phi$ (cf. Chap. V, § 11, No. 5, Cor. of Th. 3).

4) Let $A$ be a finite field of characteristic $\neq 2$, $E$ a finite-dimensional vector space of dimension $n$ over $A$.

a) Prove that for every non-degenerate symmetric bilinear form $\Phi$ on $E$, there exists an orthogonal basis $(e_i)$ of $E$ such that $\Phi(e_i, e_i) = 1$ for $1 \leq i \leq n-1$, $\Phi(e_n, e_n) = \Delta$ (discriminant of $\Phi$ with respect to $(e_i)$). (Remark that if $\alpha \beta \neq 0$, the equation $\alpha \xi^2 + \beta \eta^2 = \gamma$ always admits solutions $(\xi, \eta)$ in $A$ if $\gamma \neq 0$ (chap. V, § 11, exerc. 4)).

b) In order that two non-degenerate symmetric bilinear forms on E be equivalent, it is necessary and sufficient that the quotient of their discriminants (with respect to the same basis of E) be a square in A. Deduce that, if n is odd, for every non-degenerate symmetric bilinear form $\Phi$ on E, there exists an orthogonal basis with respect to which the matrix of $\Phi$ is of the form $\lambda I_n \ (\lambda \in A)$; the index of $\Phi$ is then $(n-1)/2$.

c) If $n = 2m$ is even, prove that the index of a non-degenerate symmetric bilinear form $\Phi$ on E is m if $(-1)^m \Delta$ is a square in A, $m-1$ otherwise.

5) Let A be a commutative field of characteristic $\neq 2$. Let I be a polynomial with coefficients in A, with respect to $n(n+1)/2$ indeterminates $X_{ij} \ (1 \leq i \leq j \leq n)$; for every symmetric matrix $R = (\alpha_{ij})$ over a commutative overfield $A'$ of A, denote by $I(R)$ the element of $A'$ obtained by substituting $\alpha_{ij}$ for the indeterminate $X_{ij} \ (i \leq j)$ in I.

Suppose that I is such that, for the matrix $U = (u_{ij})$ with $u_{ij} = X_{ij}$ for $i \leq j$, $u_{ij} = X_{ji}$ for $i > j$ and the square matrix $P = (Y_{ij})$ of order n (where the $Y_{ij}$ are $n^2$ other indeterminates), one has

$$
I(PUP) = (\det P)^h I(U)
$$

where h is an integer $> 0$. Prove that h is even and that $I(U) = \gamma (\det U)^k$, where $h = 2k$ and $\gamma \in A$. (Using th. 1, prove that for every symmetric matrix $R$ over the algebraic closure $\Omega$ of A, one has $(I(R))^2 = \lambda (\det R)^h$, where $\lambda \in \Omega$, and use the fact that the polynomial $\det U$ with respect to the $X_{ij}$ is not a square, by considering the terms of this polynomial containing an $X_{ii}$.

Soient A un corps valué complet non discret, commutatif et de caractéristique $\neq 2$ (Top. gén., chap. IX, § 3, no 2), $\Phi$ une forme hermitienne non dégénérée sur un espace vectoriel E de dimension finie n sur A, $R = (\alpha_{ij})$ la matrice de $\Phi$ par rapport à une base $(e_i)$ de E. Show that there exists $\varepsilon > 0$ such that, for every hermitian matrix $R' = (\chi'_{ij})$ satisfying the conditions $|\alpha'_{ij} - \alpha_{ij}| \leq \varepsilon$ for every pair $(i, j)$, the form $\Phi'$ having $R'$ as matrix with respect to the basis $(e_i)$ is equivalent to $\Phi$. (Reduce to the case where $R$ is diagonal; use exerc. 2 b) by relying on the following lemma: there exists a number $a > 0$ such that for $|\eta| \leq a$, there exists in A an element $\xi$ such that $\xi^2 = 1 - \eta$. To prove this lemma, the binomial series for $(1-x)^{1/2}$ will be used.)

Soient A un corps commutatif non ordonnable (chap. VI, § 2, exerc. 8) de caractéristique $\neq 2$, E un espace vectoriel de dimension finie $n > 0$ sur A, Q une forme quadratique non dégénérée sur E, $(e_i)$ une base orthogonale pour Q, de sorte que $Q \left( \sum_{i=1}^n \xi_i e_i \right) = \sum_{i=1}^n \alpha_i \xi_i^2$. Pour $1 \leq r \leq n$, on pose $Q_r(\xi_1, \ldots, \xi_r) = \sum_{i=1}^r \alpha_i \xi_i^2$, et on désigne par $M_r$ l’ensemble des valeurs de Q_r lorsque les $\xi_i \ (1 \leq i \leq r)$ parcourent A.

(a) Show that if, for an index r, one has $M_r = M_{r+1}$, it follows that $M_r = A$ (observe that every element of A is a sum of squares (chap. VI, § 2, exerc. 7)).

(b) Suppose that the subgroup S of the multiplicative group $A^*$, formed by the squares of elements of A, is of finite index s in $A^*$. Deduce from (a) that if $n > s$, every non-degenerate quadratic form on E has index $> 0$ (observe that every set $M_r$ is the union of 0 and of classes mod. S). *Application to the case where A is a $p$-adic field $\mathbf{Q}_p$ (Top. gén., chap. III, § 5, exerc. 35).*

Soient A un corps commutatif de caractéristique $\neq 2$, E un espace vectoriel de dimension finie n sur A, Q une forme quadratique non dégénérée d’indice 0 sur E. Soient $A'$ une extension algébrique de A, de degré fini et impair, $E'$ l’espace vectoriel sur $A'$ obtenu par extension à $A'$ du corps des scalaires de E. Show that the extension $Q'$ of Q to $E'$ ($§ 3$, no 4, prop. 3) is still of index 0. (Reduce to the case where $A' = A[X]/(f)$, f being an irreducible polynomial of odd degree m over A. Let $(e_i)$ be an orthogonal basis of E for Q, and let $\rho_i = Q(e_i)$; show that, in $A[X]$, a relation of the form $\sum_i \rho_i(g_i(X))^2 = f(X)h(X)$, where the $g_i$ are non-zero polynomials not all zero, of degree $\leq m - 1$, is impossible; observe for this that h would necessarily be of odd degree, and consider an irreducible factor of h, of odd degree).

Soient A un corps, E un espace vectoriel sur A admettant une base dénombrable $(e_n)_{n \geq 1}$, $\Phi$ une forme sesquilinéaire hermitienne non dégénérée sur E, satisfaisant à la condition (T) ($§ 4$, no 2).

(a) Show that if the conditions (C) of th. 1 are not simultaneously verified, there exists in E an orthogonal basis for $\Phi$ (reason as in exerc. 4 of the $§ 5$).

b) Suppose in addition that A is commutative, and that there exists an integer s such that on every finite-dimensional vector space of dimension $> s$ over A, every non-degenerate Hermitian sesquilinear form has index $> 0$ (cf. exerc. 7). Now prove that there then exists in E an orthonormal basis for $\Phi$. (Reason as in a), observing that for every element of A of the form $\alpha = \lambda + \overline{\lambda}$, and every non-degenerate Hermitian form $\Psi$ on a space F of dimension $> s$, there exists $z \in F$ such that $\Psi(z, z) = \alpha$ (cf. $§ 4$, no 2, prop. 4).)

¶ 10) a) Let A be a principal ideal domain in which there is only one maximal ideal $A\pi$, such that 2 is not divisible by $\pi$ (chap. VII, § 1, exerc. 4). Let E be a free module over A, of dimension n. Now prove that every symmetric bilinear form $\Phi$ on E admits an orthogonal basis. (Let r be the greatest exponent such that $\pi^r$ divides all the elements $\Phi(x, y)$; show that there exists $a \in E$ such that $\Phi(a, a) = \alpha \pi^r$, where $\alpha$ is invertible in A; deduce that E is the direct sum of $F = Aa$ and the submodule $F^0$ orthogonal to F.)

b) Give an example (for $n = 2$) in which $\Phi$ is non-degenerate and in which there exists a non-isotropic submodule F of E, of rank 1, admitting a complement in E but such that $F^0$ is not a complement of F.

c) Let $(e_i)$ be an orthogonal basis for $\Phi$, and $\alpha_i = \Phi(e_i, e_i)$. Now prove that the ideals $A\alpha_i$ are, up to order, independent of the orthogonal basis considered (cf. $§ 5$, th. 1).

These ideals are called the invariant factors of the form $\Phi$. Give an example of two forms having the same invariant factors and not equivalent (take two forms for which the quotient of the discriminants is not a square).

d) Soient $F$ un sous-module de $E$, $\Phi_F$ la restriction de $\Phi$ à $F \times F$, $A\alpha_i$ ($1 \leq i \leq r$) les facteurs invariants non nuls de $\Phi$, rangés de sorte que $\alpha_i$ divise $\alpha_{i+1}$, $A\beta_i$ ($1 \leq i \leq s$) les facteurs invariants non nuls de $\Phi_F$, rangés de sorte que $\beta_i$ divise $\beta_{i+1}$. Montrer que l’on a $s \leq r$ et que $\beta_i$ est multiple de $\alpha_i$ pour $1 \leq i \leq s$ (même méthode que dans l’exerc. 1 a) du § 5).

e) Suppose $\Phi$ is non-degenerate; let $F$, $G$ be two non-isotropic submodules of $E$ such that $F^0$ (resp. $G^0$) is supplementary to $F$ (resp. $G$). Suppose that the restrictions of $\Phi$ to $F$ and to $G$ are equivalent; now prove that there exists an automorphism $u$ of $E$, leaving $\Phi$ invariant, and such that $u(F) = G$. (Using $a$), reduce to the case where $F = Aa, G = Ab, \Phi(a, a) = \Phi(b, b)$. Let $(c_j)$ be a base of $G^0$, and let $b', c'_j$ ($1 \leq j \leq n-1$) be the components of $b$ and $c_j$ respectively in $F^0$; now prove that there exist scalars $\mu_j$ ($1 \leq j \leq n-1$) such that the elements $d_j = c'_j + \mu_j b'$ satisfy the relations $\Phi(d_j, d_k) = \Phi(c_j, c_k)$ for every pair of indices; one will note for this that for every $\lambda \in A$, one of the elements $1 \pm \lambda$ is invertible in $A$.

11) Let $A$ be a principal ideal domain of characteristic 0, in which there is only one principal ideal $\pi$, such that 2 is divisible by $\pi$. If $(e_1, e_2)$ is the canonical basis of $E = A^2$, $\Phi$ the symmetric bilinear form on $E$ defined by $\Phi(\xi_1 e_1 + \xi_2 e_2, \eta_1 e_1 + \eta_2 e_2) = \xi_1 \eta_2 + \xi_2 \eta_1$, now prove that there is no orthogonal base of $E$ for $\Phi$.

12) Let $A$ be the finite field $\mathbf{F}_{q^2}$, $J$ the involutive automorphism $\xi \to \xi^q$ of $A$, whose field of invariants is $\mathbf{F}_q$. If $E$ is a vector space of dimension $n$ over $A$, $\Phi$ a non-degenerate hermitian sesquilinear form (for $J$) on $E$, now prove that the order of the unitary group $\mathbf{U}(\Phi)$ is equal to
$$
(q^n - (-1)^n) q^{n-1}(q^{n-1} - (-1)^{n-1}) q^{n-2} \ldots (q^2 - 1) q(q + 1)
$$
(method analogous to that of Exercise 10 of § 5, using Exercise 3).

13) Let $A$ be the finite field $\mathbf{F}_q$ ($q$ not a multiple of 2), $E$ a vector space of dimension $n$ over $A$, $Q$ a non-degenerate quadratic form on $E$. Now prove that:
a) If $n$ is odd, the order of the group $\mathbf{SO}(Q)$ is
$$
(q^{n-1} - 1) q^{n-2}(q^{n-3} - 1) q^{n-4} \ldots (q^2 - 1) q.
$$
b) If $n = 2m$ is even, the order of the group $\mathbf{SO}(Q)$ is equal to
$$
(q^{2m-1} - \varepsilon q^{m-1}) (q^{2m-2} - 1) q^{2m-3} \ldots (q^2 - 1) q
$$
where $\varepsilon = 1$ if $(-1)^m \Delta$ is a square in $A$, $\varepsilon = -1$ otherwise, $\Delta$ denoting the discriminant of $Q$ with respect to any basis of $E$. (Method analogous to that of Exerc. 12, using Exerc. 3 of $§ 6$ and Exerc. 5 of Chap. V, § 11.)

14) Suppose that $A$ is a commutative field, $E$ a vector space of finite dimension $n \geqslant 2$ over $A$, $\Phi$ a non-degenerate hermitian sesquilinear form on $E$, satisfying condition (T) ($§ 4$, No. 2). Now prove that the only endomorphisms $\omega$ of $E$ commuting with all the automorphisms $u$ belonging to the special unitary group $\mathbf{SU}(\Phi)$ are the homotheties, except when one has simultaneously $n = 2$, $J = 1$, $A$ being of characteristic $\neq 2$. (If $n \geqslant 3$, write that $\omega$ commutes with the involutions $u \in \mathbf{SU}(\Phi)$, and use Exerc. 3 of the $§ 4$; if $n = 2$ and $J \neq 1$, write that $\omega$ commutes with the elements of $\mathbf{SU}(\Phi)$ whose matrix is of the form $\begin{pmatrix} \lambda & 0 \\ 0 & \lambda^{-1} \end{pmatrix}$ with respect to an orthogonal basis of $E$.)

$§ 15$) Let $A$ be a commutative field of characteristic $\neq 2$, $E$ a vector space of dimension $n \geqslant 1$ over $A$, $Q$ a non-degenerate quadratic form on $E$. For every automorphism $u \in \mathbf{O}(Q)$, let $\omega = u - 1$, and let $r$ be the rank of $\omega$, and $W = \overline{\omega}(0)$.

a) Show that $\omega(E)$ is the subspace $W^0$ orthogonal to $W$.

b) Show that if $n = 2, r = 2$, $u$ is product of two symmetries with respect to lines of $E$. (Establish that if $\omega(x)$ is isotropic for every non-isotropic vector $x \in E$, $\omega(x)$ is isotropic for every $x \in E$; one will consider separately the case where $A$ has at least 5 elements and the case $A = \mathbf{F}_3$.)

c) Suppose that $n$ and $r$ are arbitrary. Show that if $\omega(E)$ is not totally isotropic, $u$ is product of $r$ symmetries with respect to hyperplanes of $E$, and cannot be product of a smaller number of symmetries. (Reduce to the case where $W$ is totally isotropic, and proceed by induction on $n$ and $r$. If $W \neq \{0\}$, show that there exists a vector $a \in W^0$ such that $\omega(a)$ is not isotropic, by reasoning by contradiction and using the fact that a plane of which all the lines except at most one are isotropic is necessarily totally isotropic; take then the symmetry $s$ with respect to the hyperplane orthogonal to $\omega(a)$, and consider the automorphism $su$. If $W = \{0\}$, take $a \in E$ such that $\omega(a)$ is not isotropic, and, with the same meaning for $s$, consider again the automorphism $su$, and use b).)

d) Suppose that $\omega(E)$ is totally isotropic. If $s$ is a symmetry with respect to a non-isotropic hyperplane $H$, show that the subspace of vectors invariant under $su$ is $H \cap W$, hence is of dimension $n - r - 1$, and deduce that $su$ cannot be product of fewer than $r + 1$ symmetries with respect to hyperplanes. Deduce then from c) that $u$ is product of $r + 2$ symmetries with respect to hyperplanes, but cannot be product of a smaller number of symmetries.

e) Deduce from c) and d) that every orthogonal automorphism is product of at most $n$ symmetries with respect to hyperplanes.

f) Show that if $n$ is odd (resp. even), for every automorphism $u \in \mathbf{O}(Q)$ of determinant 1 (resp. – 1), there exists a vector $x \neq 0$ invariant under $u$ (use e)).

16) The hypotheses being the same as in Exerc. 15, show that, if $n \geqslant 3$, the group $\mathbf{SO}(Q)$ is generated by the symmetries with respect to the non-isotropic subspaces of $E$ of dimension $n - 2$ (reason as in Prop. 5 of No. 4).

**¶ 17) The hypotheses are the same as in Exerc. 15.**

a) Show that, for $n \geqslant 2$, the commutator group $\Omega(Q)$ of the orthogonal group $O(Q)$ is generated by the elements $(st)^2$, where $s$ and $t$ range over the set of symmetries with respect to hyperplanes (use Prop. 5 of No. 4, and observe that for every group $\Gamma$, the subgroup generated by the squares of the elements of $\Gamma$ contains the commutator group of $\Gamma$).

b) Show that if $n \geqslant 3$, the commutator group of $SO(Q)$ is generated by the squares of the elements of $SO(Q)$ (use Exerc. 16); deduce that this group is identical with $\Omega(Q)$, and that the quotient group $SO(Q)/\Omega(Q)$ is a commutative group all of whose elements are of order 2.

c) A plane $P \subset E$ is said to be *hyperbolic* if it is non-isotropic and if it contains isotropic lines (necessarily 2 in number). An automorphism $u \in O(Q)$ is said to be *hyperbolic* if there exists a hyperbolic plane $P$ such that $u(x) = x$ for all $x \in P^0$; $u$ is then said to be a hyperbolic transform associated with $P$. Show that if $Q$ is of index $\geqslant 1$, every $u \in O(Q)$ is a product of hyperbolic transforms (use Prop. 5 of No. 4 and Exerc. 4 a) of § 4). Deduce that if $P$ is a hyperbolic plane, every $u \in O(Q)$ can be written $u = t \varphi$, where $t$ is a hyperbolic transform associated with $P$ and $\varphi \in \Omega(Q)$.

**¶ 18) Let A be a commutative field, E a vector space of dimension $n$ over A, $\Phi$ a non-degenerate hermitian sesquilinear form on E, satisfying condition (T) ($§ 4$, No. 2). Let V be a vector subspace of E, $H_v$ the subgroup of the unitary group $U(\Phi)$ formed by the unitary automorphisms $u$ such that $u(V) = V$.

a) Show that, when V is not a totally isotropic subspace of dimension $n/2$, the image of $H_v$ by the mapping $u \to \det u$ is the subgroup of $A^*$ formed by the $\rho \in A$ such that $\rho \overline{\rho} = 1$.

b) If $n$ is even and if V is a totally isotropic subspace of dimension $n/2$, show that the image of $H_v$ by the mapping $u \to \det u$ is the subgroup of $A^*$ formed by the elements of the form $\bar{\lambda}/\lambda$ (use Prop. 2 of the $§ 4$, No. 2).

c) Let V, W be two vector subspaces of E such that the restrictions of $\Phi$ to V and W are equivalent. Show that there exists $u \in SU(\Phi)$ such that $u(V) = W$ in the following cases:
  1° J is distinct from the identity (use Th. 3 of Chap. V, § 11, No. 5).
  2° $J = 1$, A is of characteristic $\neq 2$, V and W are not totally isotropic subspaces of dimension $n/2$.

d) Suppose that $J = 1$, that A is of characteristic $\neq 2$, that $n = 2m$ is even, and that $\Phi$ is a nondegenerate symmetric bilinear form of index $m$. Let V, W be two totally isotropic subspaces of dimension $m$ in E; prove that if $\dim(V \cap W) = q$, then, for every orthogonal automorphism $u$ such that $u(V) = W$, one has $\det u = (-1)^{m-q}$ (use b) and prop. 2 of the $§ 4$, no 2). Deduce that the set of totally isotropic subspaces of dimension $m$ is the union of two classes of intransitivity $N_1, N_2$ for the group $SU(\Phi)$; if V and W belong to the same class (resp. to different classes), the dimension of V ∩ W has the same parity as m (resp. does not have the same parity as m). For a similitude u (for Φ) to be direct, it is necessary and sufficient that $u(N₁) = N₁$ (use exerc. 4 c) of § 4.

19) Let A be a field, E a finite-dimensional vector space and > 0 over A, Φ an ε-hermitian sesquilinear form on E, nondegenerate and nonalternating. Let u be an automorphism of E such that one has

$$
\Phi(u(x), u(x)) = \alpha \Phi(x, x)
$$

for all $x \in E$, with $\alpha \in A$. Prove that u is a similitude of multiplier $\alpha$ except when the following conditions are simultaneously satisfied: A is commutative and of characteristic 2, J is the identity (use exerc. 8 of § 1).

20) Let A be a field, L a finite-dimensional hermitian space over A; suppose that the metric form Φ of L satisfies condition (T) (§ 4, no 2). Prove that if the index of Φ is > 0, there may be similitudes of L, of multiplier $\neq 1$, and which admit no fixed point (use the reasoning of prop. 6 of no 6, and prop. 2 of § 4, no 2).

21) Let A be a commutative field of characteristic $\neq 2$, L a finite-dimensional euclidean space over A, Φ the metric form of L.

a) Prove that every bijection u of L onto itself, such that

$$
\Phi(u(x) - u(y), u(x) - u(y)) = \Phi(x - y, x - y)
$$

whatever x, y in L may be, is a displacement (use exerc. 7 of § 1).

b) Prove that the group of displacements is generated by the symmetries with respect to the nonisotropic hyperplanes of the affine space L (using prop. 5 of no 4, reduce oneself to proving that every nonisotropic translation is the product of two such symmetries).

22) In a hermitian space L, two linear varieties are said to be perpendicular if their directions are weakly orthogonal subspaces (§ 3, exerc. 11). Suppose L finite-dimensional; let V₁, V₂ be two linear varieties, W₁, W₂ their respective directions. Suppose that $p = \dim(W₁ + W₂) < n$; prove that if $W₁ + W₂$ is not isotropic, there exists at least one linear variety U of dimension $n - p$, perpendicular to V₁ and to V₂, and meeting each of the linear varieties V₁, V₂ in a single point; moreover, if $q = \dim(W₁ \cap W₂)$, the union of all the linear varieties U having the preceding properties is a linear variety of dimension $n - p + q$.

23) Let A be a commutative field of characteristic $\neq 2$, E a finite-dimensional vector space of dimension $n + 1 \geq 2$ over A, Q a quadratic form on E, Φ the symmetric bilinear form associated with Q. The set C of the $x \in E$ such that $Q(x) = 0$ is called the isotropic cone with vertex 0 and equation $Q(x) = 0$. If it is not reduced to 0, the image S of C – {0} in the projective space $\mathbf{P}(E)$, by the canonical mapping $\pi$ of $E - \{0\}$ onto $\mathbf{P}(E)$ (chap. II, 2e éd., App. III), is called *projective quadric* (resp. *projective conic* if $n = 2$) of homogeneous equation $Q(x) = 0$. One says that S is *degenerate* if Q is degenerate. One says that two projective linear varieties $V_1, V_2$ of $\mathbf{P}(E)$ are *conjugate* with respect to S if $\overline{\pi}(V_1)$ and $\overline{\pi}(V_2)$ are orthogonal (for $\Phi$). The *polar* $V^0$ of a projective linear variety $V \subset \mathbf{P}(E)$ with respect to S is the variety such that $\overline{\pi}(V^0) \cup \{0\}$ is the totally orthogonal subspace (for $\Phi$) to $\overline{\pi}(V) \cup \{0\}$; if V is a hyperplane and if S is nondegenerate, $V^0$ is reduced to a point, called the *pole* of V. A projective linear variety V is said to be *tangent* to S if $\overline{\pi}(V) \cup \{0\}$ is an isotropic subspace (for $\Phi$).

Suppose in what follows that S is nonempty and nondegenerate.

a) Prove that the intersection of S and a projective linear variety V is empty or is a quadric *in* V; for this quadric to be degenerate, it is necessary and sufficient that V be tangent to S.

b) Prove that the tangent hyperplane to S at a point $z \in S$ is the union of the lines passing through z and tangent to S.

c) Suppose $z \notin S$. For every line D passing through z and meeting S at two points $a, b$ (distinct or not), let $z'$ be the *harmonic conjugate* of z with respect to $a$ and $b$, that is to say, the point of D such that $\begin{bmatrix} a & b \\ z' & z \end{bmatrix} = -1$ (chap. II, 2e éd., App. III, exerc. 4); prove that $z'$ belongs to the polar hyperplane of z with respect to S, and that there exist n of these points forming a projectively free family in $\mathbf{P}(E)$ and belonging to S (cf. § 4, exerc. 4 a)).

d) Suppose that $n = 3$ and that $\Phi$ is of maximum index $v = 2$. The set of lines contained in S is then the union of two sets $N_1, N_2$ such that every line of $N_1$ meets every line of $N_2$, but two distinct lines of $N_1$ (resp. $N_2$) do not meet (exerc. 18 d)). Let D, D’ be two distinct lines belonging to $N_1$; for every $z \in D$ there exists one and only one line $\Delta \in N_2$ passing through z; if $u(z)$ is the point where $\Delta$ meets D’, now prove that $u$ is a projective linear mapping of D onto D’.

e) Supposing still $n = 3$, let D, D’, D’’ be three lines of $\mathbf{P}(E)$ of which any two do not meet. Now prove that the union of the lines meeting D, D’ and D’’ is a nondegenerate quadric.

24) The hypotheses and notations are those of exerc. 23, the quadric S being supposed nonempty and nondegenerate.

a) Now prove that the subgroup $\Gamma$ of the projective group $\mathbf{PGL}(E)$ formed by the projective linear bijections transforming S into itself, is the canonical image of the group of similitudes relative to Q. (Use exerc. 23 c) above, exerc. 2 a) of § 4 and exerc. 8 of § 1.)

b) Let $a$ be a point of $\mathbf{P}(E)$ not belonging to S, and let $\Phi_1$ be the restriction of $\Phi$ to the orthogonal hyperplane to $\overline{\pi}(a)$ in E. Now prove that the subgroup of $\Gamma$ leaving $a$ invariant is isomorphic to the quotient of the orthogonal group $\mathbf{U}(\Phi_1)$ by its center.

c) Let $b$ be a point of $S$, $F$ the (isotropic) hyperplane orthogonal to $\overline{\pi}(b)$ in $E$, $M$ a nonisotropic supplementary space of $\overline{\pi}(b)$ with respect to $F$, and $\Phi_2$ the restriction of $\Phi$ to $M$. Now prove that the subgroup of $\Gamma$ leaving $b$ invariant is isomorphic to the group of similitudes of a Euclidean space $L$ of dimension $n - 1$, having as metric form the inverse form ($§ 1$, no 7) of $\Phi_2$. (Observe that if a similitude for $\Phi$ transforms the line $\overline{\pi}(b)$ into itself, it transforms $F$ into itself, and is entirely determined by its restriction to $F$).

25) Let $A$ be a commutative field of characteristic $\neq 2$, $L$ a finite-dimensional affine space of dimension $n \geqslant 2$ over $A$. We identify $L$ with the complement of a projective hyperplane $H_0$ (“hyperplane at infinity”) of a projective space $\mathbf{P}(E)$ of dimension $n$ (chap. II, 2nd ed., App. III, No. 4). We say that a nonempty set $S \subset L$ is an affine quadric (resp. affine conic if $n = 2$) if $S$ is the intersection of $L$ and a projective quadric (resp. conic) in $\mathbf{P}(E)$ (exerc. 23).

(a) Show that if there exists a non-degenerate projective quadric $\overline{S} \subset \mathbf{P}(E)$ such that $S = L \cap \overline{S}$, this quadric is the only one having these properties, unless $n = 2$, $A = \mathbf{F}_3$ and $S$ is reduced to 2 elements (observe that outside this exceptional case, for every point $z \in H_0$ not belonging to $\overline{S}$, there exists a right passing through $z$ and meeting $S$ in two distinct points). We then say that $S$ is a non-degenerate affine quadric. We say that two affine linear varieties $V_1, V_2$ contained in $L$ are conjugate with respect to $S$ if the projective linear varieties $\overline{V}_1, \overline{V}_2$ such that $V_i = L \cap \overline{V}_i \ (i = 1, 2)$ are conjugate with respect to $\overline{S}$; we define analogously the polar (when it is not contained in $H_0$) or the pole of an affine linear variety with respect to $S$, and the affine linear varieties tangent to $S$.

(b) We suppose that $S$ is non-degenerate; show that one can take an origin $a$ in $L$ such that, by identifying $L$ in this way with a vector space, there is a basis $(e_i)$ of $L$ such that $S$ is the set of the $x = \sum_{i=1}^n \xi_i e_i$ satisfying one of the two equations of the forms

$$
\alpha_1 \xi_1^2 + \cdots + \alpha_n \xi_n^2 = 1 \\
\alpha_1 \xi_1^2 + \cdots + \alpha_{n-1} \xi_{n-1}^2 + \xi_n = 0.
$$

In the first case, the point $a$ is well determined and is the pole with respect to $\overline{S}$ of the hyperplane at infinity $H_0$ (called the center of $S$). (Distinguish two cases according as $H_0$ is or is not tangent to $\overline{S}$; use Theorem 1 of § 6, No. 1 and Proposition 2 of § 4, No. 2.)

26) Let $A$ be a commutative algebraically closed field of characteristic $\neq 2$, $E$ a finite-dimensional vector space over $A$, $Q$ a non-degenerate quadratic form on $E$. Let $u \in \mathbf{O}(Q)$; with the notation of exerc. 12 of § 4, we have $G(p, p) = \{0\}$ unless $p(X) = X - 1$ and $p(X) = X + 1$. Let $M$ be a minimal element of the set of non-isotropic subspaces contained in $G(p, p)$ and stable under $u$, and let $p^h$ be the minimal polynomial of the restriction of $u$ to $M$. Now prove that if $h$ is odd, $M$ is an indecomposable submodule of $E_u$, and that if $h$ is even, $M$ is a direct sum of two isomorphic indecomposable submodules of $E_u$. (To see that if $h = 2k$ is even, $M$ cannot be indecomposable, show that $N = p^k(u)(M)$ would then be totally isotropic; if $(e_i)_{1 \leq i \leq 2k}$ is a basis of $M$ such that $u(e_i) = \varepsilon e_i + e_{i+1}$ for $i \leq 2k - 1$, $u(e_{2k}) = \varepsilon e_{2k}$ (with $\varepsilon = \pm 1$), show that $e_k$ cannot be orthogonal to $e_{k+1}$, and deduce that the relation $Q(u(e_k)) = Q(e_k)$ leads to a contradiction).

27) Let $A$ be a commutative field of characteristic 2, $E$ a vector space over $A$, of finite dimension $n$, $Q$ a quadratic form on $E$, $\Phi$ the associated bilinear form, which is alternating, hence of even rank $2m$ ($§ 5$, no 1, cor. 1 of th. 1).

a) Prove that if $E^0$ is the subspace of $E$ (of dimension $n - 2m$) orthogonal to $E$ for $\Phi$, one has $Q(\lambda x + \mu y) = \lambda^2 Q(x) + \mu^2 Q(y)$ for all $x, y$ in $E^0$; in other words, the restriction $Q_0$ of $Q$ to $E^0$ is a semilinear mapping from $E^0$ (considered as a vector space over $A$) into $A$ (considered as a vector space over the subfield $A^2$), relative to the isomorphism $\xi \to \xi^2$ of $A$ onto $A^2$. Let $q$ be the dimension (over $A$) of the kernel $E^0 \cap \overline{Q}(0)$ of $Q$, and let $E_1$ be a supplementary subspace of $E^0 \cap \overline{Q}(0)$ with respect to $E^0$; one has $n - 2m - q \leq [A : A^2]$.

b) Deduce from a) that there exists a base $(e_i)_{1 \leq i \leq n}$ of $E$, the first $2m$ vectors of which form a base of a supplementary subspace $E_2$ of $E^0$ in $E$, the next $n - 2m - q$ vectors a base of $E_1$, such that, for $x = \sum_{i=1}^n \xi_i e_i$

$$
Q(x) = \sum_{i=1}^m (\alpha_i \xi_i^2 + \xi_i \xi_{m+i} + \beta_i \xi_{m+i}^2) + \sum_{i=2m+1}^{n-q} \gamma_i \xi_i^2
$$

the $\gamma_i$ ($2m + 1 \leq i \leq n - q$) being elements of $A$ linearly independent with respect to $A^2$.

c) The index of $Q$ is called the maximum dimension of the totally singular subspaces $V$ of $E$ such that $V \cap E^0 = \{0\}$. Prove that if $v$ is the index of $Q$, one can take the base $(e_i)$ of $E$ having the properties stated in b) in such a way that $\alpha_i = \beta_i = 0$ for $1 \leq i \leq v$ and that the restriction of $Q$ to the subspace of $E_2$ generated by $e_{v+1}, \ldots, e_m, e_{m+v+1}, \ldots, e_{2m}$ is a quadratic form (non-degenerate) of index 0.

d) We suppose $q = 0$; let $O(Q)$ be the automorphism group of $E$ leaving $Q$ invariant. If $u \in O(Q)$, now prove that $u(x) = x$ for every $x \in E^0$. For every $x \in E_2$, let $u(x) = u_0(x) + u_2(x)$, where $u_0(x) \in E^0$ and $u_2(x) \in E_2$; show that $u_2$ belongs to the symplectic group $Sp(\Phi_2)$ (where $\Phi_2$ is the restriction of $\Phi$ to $E_2$) and that $Q(u_2(x)) + Q(x) \in Q(E^0)$. Conversely, for every automorphism $u_2 \in Sp(\Phi_2)$ such that $Q(u_2(x)) + Q(x) \in Q(E^0)$ for every $x \in E_2$, show that there exists one and only one linear mapping $u_0$ of $E_2$ into $E^0$ such that the linear mapping equal to $u_0 + u_2$ in $E_2$, to the identity in $E^0$, belongs to $\mathbf{O}(Q)$.

e) We suppose that $A$ is a *perfect* field ($A^2 = A$) and that $q = 0$. Deduce from b) that every vector subspace of $E$, of dimension $\geqslant 3$, contains at least one vector $x$ such that $Q(x) = 0$. If $n$ is *odd*, one necessarily has $m = \nu$ and $n = 2m + 1$, so that there exists a basis $(e_i)$ of $E$ with respect to which one has

$$
Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_m \xi_{2m} + \xi_{2m+1}^2,
$$

and (with the notations of $d$)) $\mathbf{O}(Q)$ is isomorphic to $\mathbf{Sp}(\Phi_2)$; all quadratic forms such that $q = 0$ are then equivalent. If $n$ is *even*, one necessarily has $n = 2m, \nu = m$ or $\nu = m - 1$, and there exists a basis $(e_i)$ of $E$ with respect to which one has

$$
(1) \quad Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_{m-1} \xi_{2m-1} + \xi_m \xi_{2m} + \lambda(\xi_m^2 + \xi_{2m}^2)
$$

where $\lambda \in A$. Let $A_1$ be the field obtained by adjoining to $A$ the roots of the polynomial $\lambda X^2 + X + \lambda$; prove that this field is independent of the basis $(e_i)$ with respect to which $Q$ can be written in the form (1), and that in order that two quadratic forms (such that $q = 0$) be equivalent, it is necessary and sufficient that the quadratic extensions of $A$ which correspond to them in this way be identical (use Witt's theorem). Case where $A$ is a finite field of characteristic 2.

**¶ 28**) Let $A$ be a commutative field of characteristic 2, distinct from $\mathbf{F}_2$, $E$ a vector space of dimension $n = 2m$ over $A$, $Q$ a non-degenerate quadratic form on $E$.

a) Prove that the orthogonal group $\mathbf{O}(Q)$ is generated by the symmetries (which here are nothing other than the transvections belonging to $\mathbf{O}(Q)$ ($§ 4$, exercise 6)) (reason as in exercise 11 of $§ 5$). Deduce that the commutator group of $\mathbf{O}(Q)$ is generated by the squares of the elements of $\mathbf{O}(Q)$ (cf. exercise 17).

b) Suppose that $Q$ is of maximum index; let $V, W$ be two totally singular subspaces of $E$ ($§ 4$, No. 1) of dimension $m$. Let $u$ be a symmetry $x \to x + \frac{\Phi(x, a)}{Q(a)} a$ ($§ 4$, exercise 6) ; let $k$ be the dimension of $V \cap W$. Prove that the dimension of $V \cap u(W)$ is $k + 1$ if $a$ is orthogonal to $V \cap W, k - 1$ otherwise (in the first case remark that $a = x + y$, or $x \in V, y \in W$, and prove that $u(y) = x$; in the second, remark that $u$ cannot leave invariant any non-orthogonal singular vector to $a$).

c) Suppose again that the index of $Q$ is arbitrary. Prove that the subgroup $\mathbf{SO}(Q)$ of $\mathbf{O}(Q)$, formed by the automorphisms of $E$ which are products of an *even* number of symmetries, is a distinguished subgroup of index 2 of $\mathbf{O}(Q)$. (Prove that the product of an odd number of symmetries cannot be the identity, by considering the extension of $Q$ to the es-

Bourbaki XXIV.

pace vectoriel E' obtained by extension of the field of scalars of E to its algebraic closure ; use then b).) (Cf. § 9, exercise 9.)

d) If V₁, V₂ are two totally singular subspaces of E, of the same dimension < m, prove that there exists an automorphism u ∈ SO(Q) such that u(V₁) = V₂. On the contrary, if V₁ and V₂ are two totally singular subspaces of dimension m, in order that there exists an automorphism u ∈ SO(Q) such that u(V₁) = V₂, it is necessary and sufficient that the dimension of V₁ ∩ V₂ have the same parity as m (reason as in exercise 18, using b)).

e) A plane P ⊂ E is said to be hyperbolic if it is non-isotropic and contains singular lines (necessarily 2 in number). A transformation u ∈ O(Q) is said to be hyperbolic if there exists a hyperbolic plane P such that u(x) = x for every x ∈ P⁰ ; one then says that u is a hyperbolic transformation associated with P. Prove that if Q is of index > 0, every u ∈ O(Q) is a product of hyperbolic transformations (use a)). Deduce that if P is a hyperbolic plane, every transformation u ∈ O(Q) can be written u = sv, where s is a hyperbolic transformation associated with P and v belongs to the commutator group of O(Q).

29) The hypotheses being those of exercise 28, suppose in addition that Q is of maximum index m; let (eᵢ) be a symplectic basis of E (for the alternating form Φ associated with Q) formed by singular vectors (§ 4, No. 2, Proposition 2), so that the matrix of Φ with respect to this basis is the matrix denoted R in exercise 14 of § 5. With the notations of this last exercise, prove that, in order that a symplectic matrix (tD + S)⁻¹(D + S) be the matrix of an automorphism u ∈ O(Q), it is necessary and sufficient that S be alternating (write that every vector u(eᵢ) is singular, remarking that one has (tD + S).u(eᵢ) = (D + S).eᵢ).
