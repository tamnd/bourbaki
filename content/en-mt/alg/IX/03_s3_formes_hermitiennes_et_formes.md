---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 3
section_title: Formes hermitiennes et formes quadratiques
lang: en
source: alg-ix-fr
pdf_pages: 0047-0061
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes et $\varepsilon$-hermitiennes.
      page: 0
      pdf_page: 47
    - "no": 2
      title: '*Modules sur une extension quadratique*.'
      page: 0
      pdf_page: 49
    - "no": 3
      title: Formes bilinéaires associées à une forme hermitienne.
      page: 0
      pdf_page: 50
    - "no": 4
      title: Formes quadratiques.
      page: 0
      pdf_page: 52
statements: 7
exercises: 0
content_sha256: 278c5bc9bff3866993e4760bfeae099bc9f8ff1babdcbb3c044603d90386b02b
translated_from: content/fr/alg/IX/03_s3_formes_hermitiennes_et_formes.md
source_lang: fr
translation_method: machine
source_content_sha256: c0d7c8b724352f8b0f88aedc95fe9241b73de923d6f20ae8f8560d6971352e3d
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-en-mt-8fe7369c
glossary_version: 34
glossary_terms_sha256: e9c1b6f677042b3c6a4e827e45855745626b5de271e28f0978e9bb97ee16655f
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. Hermitian forms and quadratic forms

In all that follows in this Chapter, unless expressly stated otherwise, $A$ denotes a ring and $E$ a left $A$-module. We suppose that $A$ is endowed with an involutive antiautomorphism $J$, denoted $\alpha \to \overline{\alpha}$; we therefore have $(\alpha + \beta) = \overline{\alpha} + \overline{\beta}$, $(\alpha \beta) = \overline{\beta} \cdot \overline{\alpha}$ and $\overline{\alpha} = \alpha$ whatever $\alpha, \beta$ in A may be. Unless expressly stated otherwise, the sesquilinear forms considered are right sesquilinear (§ 1, No. 2, def. 4) for this antiautomorphism.

### 1. Hermitian and $\varepsilon$-hermitian forms.

#### Definition 1 {#alg-ix-s3-def-1 .statement}

Let $\varepsilon$ be an element of the center of A. A sesquilinear form $\Phi$ on E such that one has $\Phi(x, y) = \varepsilon \overline{\Phi(y, x)}$ whatever $x$ and $y$ in E may be is called an $\varepsilon$-hermitian form. A 1-hermitian form (resp. (−1)-hermitian) is called hermitian (resp. antihermitian).

When J is the identity (which implies that A is commutative) a hermitian form (resp. antihermitian form) (for J) is nothing other than a symmetric (resp. antisymmetric) bilinear form (Chapter III, § 5, No. 1, def. 2). Recall that an alternating bilinear form (Chapter III, § 5, No. 2, def. 4) is antisymmetric; the converse is true if, in A, the relation $2a = 0$ implies $a = 0$.

The orthogonality relation ($§ 1, n° 3$) with respect to an $\varepsilon$-hermitian form is obviously symmetric (cf. exerc. 1).

If $\alpha$ is an invertible element of A, the mapping $T : \lambda \to \alpha^{-1} \overline{\lambda} \alpha$ is an antiautomorphism of A, and one readily verifies that the form $\Phi \alpha$ is sesquilinear with respect to T. If, moreover, one has $\alpha = \overline{\alpha}$, then T is involutive, and, if $\Phi$ is $\varepsilon$-hermitian, $\Phi \alpha$ is so also; indeed one has
$$
(\lambda^T)^T = \alpha^{-1} (\overline{\alpha^{-1} \lambda \alpha}) \alpha = \alpha^{-1} \overline{\alpha} \lambda \overline{\alpha^{-1}} \alpha = \lambda
$$
$$
\Phi(y, x) \alpha = \varepsilon \overline{\Phi(x, y)} \alpha = \varepsilon (\Phi(x, y) \alpha)^T.
$$

In particular, when A is a field, the elements $\alpha$ of the center of A such that $\overline{\alpha} = \alpha$ form a subfield K of A, and the $\varepsilon$-hermitian forms on E (for J) form a vector space over K.

#### Remark 1 {#alg-ix-s3-n1-rem-1 .statement}

If $\Phi$ is an $\varepsilon$-hermitian form on E, one has $\Phi(x, y) = \varepsilon \overline{\Phi(x, y)} \overline{\varepsilon}$ whatever $x, y$ in E may be. Hence, if $\Phi$ takes invertible values, one has $\varepsilon \overline{\varepsilon} = 1$.
2) If there exists an invertible element $i$ of the center of A such that $\overline{i} = i \varepsilon$, then, for $\Phi$ to be $\varepsilon$-hermitian, it is necessary and sufficient that $i \Phi$ be hermitian.

The mapping $(y, x) \to \overline{\Phi(x, y)}$ being sesquilinear for J, in order that $\Phi$ be $\varepsilon$-hermitian, it is necessary and sufficient that one have $\Phi(y, x) = \varepsilon \overline{\Phi(x, y)}$ when $x$ and $y$ run through a system of generators of E. In particular, if E admits a finite basis $(e_i)_{1 \leq i \leq n}$, in order that a sesquilinear form $\Phi$ on E be $\varepsilon$-hermitian, it is necessary and sufficient that its matrix $R = (\rho_{ij}) = (\Phi(e_i, e_j))$ satisfy the relations $\rho_{ji} = \varepsilon \overline{\rho_{ij}}$ whatever $i, j$ may be, that is to say $'R = \varepsilon \overline{R}$ ; a matrix $R$ possessing this property is said to be $\varepsilon$-hermitian. When $\varepsilon = 1$ (resp. $-1$) one says that $R$ is hermitian (resp. antihermitian) relative to the antiautomorphism J. When J is the identity (hence A commutative), a hermitian (resp. antihermitian) matrix $R$ is such that $'R = R$ (resp. $'R = -R$) ; it is then said that $R$ is a symmetric (resp. antisymmetric) matrix. In order that $\Phi$ be an alternating form, it is necessary and sufficient that its matrix be antisymmetric and, in addition, that the diagonal terms of $R$ all be zero; a matrix possessing these properties is said to be alternating.

Let $\Phi$ be a sesquilinear form on $E$, and let $s_\Phi$ and $d_\Phi$ be the mappings of $E$ into $E^*$ associated with $\Phi$ on the left and on the right ($\S 1$, n° 6). In order that $\Phi$ be $\varepsilon$-hermitian, it is necessary and sufficient that $\langle x, s_\Phi(y) \rangle = \bar{\varepsilon} \langle x, d_\Phi(y) \rangle$ for all elements $x, y$ of $E$, hence that $s_\Phi = \bar{\varepsilon} d_\Phi$, or again that $\langle x, d_\Phi(y) \rangle = \varepsilon \langle x, s_\Phi(y) \rangle$, hence that $d_\Phi = \varepsilon s_\Phi$.

Let $\Phi$ be an $\varepsilon$-hermitian form such that the mapping $d_\Phi$ of $E$ into $E^*$ associated on the right with $\Phi$ is bijective. For every endomorphism $u$ of $E$ one then has
$$
u^{**} = \varepsilon \bar{\varepsilon} u.
$$
Indeed, for all elements $x$ and $y$ of $E$, one has
$$
\begin{align*}
\Phi(x, u^{**(y)}) &= \Phi(u^*(x), y) = \varepsilon \overline{\Phi(y, u^*(x))} = \varepsilon \overline{\Phi(u(y), x)} \\
&= \varepsilon \Phi(x, u(y)) \bar{\varepsilon} = \Phi(x, \varepsilon \bar{\varepsilon} u(y))
\end{align*}
$$
hence $u^{**(x)} = \varepsilon \bar{\varepsilon} u(x)$ since $\Phi$ is non-degenerate.

Si $\Phi$ est une forme $\varepsilon$-hermitienne telle que les applications $s_\Phi$ et $d_\Phi$ soient bijectives, alors la *forme inverse* $\widehat{\Phi}$ de $\Phi$ ($\S 1$, No. 7) *est une forme* $\bar{\varepsilon}$-hermitienne. En effet, en posant $s = s_\Phi$, $d = d_\Phi$ pour abréger, on déduit de $d = \varepsilon s$ que $s^{-1} = \bar{\varepsilon} d^{-1}$, $s$ étant semilinear. Par suite, quels que soient $u, v$ dans $E$, on a
$$
\widehat{\Phi}(u, v) = \Phi(s^{-1}(u), d^{-1}(v)) = \bar{\varepsilon} \Phi(d^{-1}(u), d^{-1}(v)),
$$
d’où
$$
\widehat{\Phi}(v, u) = \bar{\varepsilon} \varepsilon \overline{\Phi(d^{-1}(u), d^{-1}(v))} = \bar{\varepsilon} \overline{\widehat{\Phi}(u, v)},
$$
puisque, $\varepsilon$ est dans le center de $A$.

Enfin, lorsque le ring $A$ est commutative, les prolongements canoniques d’une forme $\varepsilon$-hermitienne $\Phi$ aux puissances tensorielle et extérieure $\bigotimes^p E$ et $\wedge^p E$ de $E$ sont des formes $\varepsilon^p$-hermitiennes, comme il résulte aussitôt des formules (35) et (37) du $\S 1$, No. 9.

### 2. *Modules over a quadratic extension*.

Soit $K$ un commutative ring. On prend pour $A$ l’extension quadratique $A = K(i)$ avec $i^2 = -1$, et pour $J$ l’automorphisme λ + iμ → λ − iμ ($\lambda \in K, \mu \in K$) (chap. II, § 7, No. 7). Si E est un A-module, nous noterons $E_0$ le K-module déduit de E par restriction de l’anneau des scalaires, et par j l’automorphisme $x \to ix$ de $E_0$; on a évidemment $j^2 = -I$, où I est le mapping identique de $E_0$. Inversement soit $E_0$ un K-module et soit j un automorphism de $E_0$ tel que $j^2 = -I$; l’application $\lambda + i\mu \to \lambda I + \mu j$ est évidemment un homomorphism de A dans le ring $\mathcal{L}(E_0)$ des endomorphisms de $E_0$; on a donc défini sur $E_0$ une structure de A-module, pour laquelle on a

(2) $$(\lambda + i\mu)x = \lambda x + \mu j(x)$$ $(x \in E_0, \lambda \in K, \mu \in K).$

If $E'$ is another A-module, $E'_0$ the K-module underlying $E'$, $j'$ the automorphism $x' \to ix'$ of $E'_0$, then the A-linear mappings f of E into $E'$ are none other than the K-linear mappings of $E_0$ into $E'_0$ such that $f \circ j = j' \circ f$. In particular, if we denote by $E^*$ and $(E_0)^*$ the respective duals of E and $E_0$, and if $f_1$ and $f_2$ are two mappings of E into K, for the mapping $x \to f_1(x) + if_2(x)$ of E into A to be A-linear, it is necessary and sufficient that $f_1$ and $f_2$ belong to $(E_0)^*$ and that one has $f_1 \circ j + i(f_2 \circ j) = if_1 - f_2$, that is to say $f_1 = f_2 \circ j$ and $f_1 \circ j = -f_2$. Since j is an automorphism of $E_0$ and since $j^2 = -I$, these two conditions are equivalent. Eliminating $f_1$ or $f_2$, one sees that the formulas

(3) $$f(x) = f_1(x) - if_1(j(x))$$
(4) $$f(x) = f_2(j(x)) + if_2(x)$$

$(x \in E,\ f \in E^*,\ f_1 \in (E_0)^*,\ f_2 \in (E_0)^*)$ establish two one-to-one correspondences between $E^*$ and $(E_0)^*$.

### 3. Bilinear forms associated with a Hermitian form.

We suppose here again that the ring A is the quadratic extension $A = K(i)$ (where $i^2 = -1$) of a commutative ring K, and that J is the automorphism $\lambda + i\mu \to \lambda - i\mu$ of A ($\lambda \in K, \mu \in K$). Let E and $E'$ be two A-modules, $E_0$ and $E'_0$ the K-modules underlying E and $E'$, j and $j'$ the automorphisms $x \to ix$ and $x' \to ix'$ of E and $E'$ (cf. n° 2). A K-bilinear form $f$ on $E_0 \times E'_0$ will be said to be *invariant under j and $j'$* if one has

(5) $$f(j(x), j'(x')) = f(x, x')$$

for $x \in E_0$ and $x' \in E'_0$. Replacing $x$ by $j(x)$, one sees that this condition is equivalent to

$$
f(x, j'(x')) = - f(j(x), x')
$$

whatever $x \in E_0$ and $x' \in E'_0$ may be.

#### Proposition 1 {#alg-ix-s3-prop-1 .statement}

Let $\Phi_1$ (resp. $\Phi_2$) be a K-bilinear form on $E_0 \times E'_0$, invariant under $j$ and $j'$. The mapping which to $\Phi_1$ (resp. $\Phi_2$) associates the mapping $\Phi$ of $E \times E'$ into $A$ defined by

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$)

$(x \in E, x' \in E)$, is an isomorphism of the K-vector space of K-bilinear forms on $E_0 \times E'_0$ invariant under $j$ and $j'$ onto the K-vector space of sesquilinear forms on $E \times E'$. Suppose moreover that $E = E'$; for $\Phi$ to be hermitian, it is necessary and sufficient that $\Phi_1$ be symmetric (resp. that $\Phi_2$ be antisymmetric) (cf. Exercise 4).

Indeed every mapping $\Phi$ of $E \times E'$ into $A$ can be written, in one and only one way, in the form $\Phi = \Phi_1 + i \Phi_2$, where $\Phi_1$ and $\Phi_2$ are mappings of $E \times E'$ into $K$. For the partial mapping $x \to \Phi(x, x')$ to be A-linear, it is necessary and sufficient, by the formula (3) (resp. (4)) of No. 2, that $\Phi_1$ (resp. $\Phi_2$) be K-linear in $x$ and that one have

$$
\Phi(x, x') = \Phi_1(x, x') - i \Phi_1(j(x), x')
$$
(resp. $\Phi(x, x') = \Phi_2(j(x), x') + i \Phi_2(x, x')$).

Analogously, for $\overline{\Phi}(x, x')$ to be A-linear in $x'$, it is necessary and sufficient that $\Phi_1$ (resp. $\Phi_2$) be K-linear in $x'$ and that one have

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$).

It follows immediately that, for $\Phi$ to be sesquilinear, it is necessary and sufficient that it be written in one or the other of the forms (9) and (11) (resp. (10) and (12)) with $\Phi_1$ (resp. $\Phi_2$) a K-bilinear form invariant under $j$ and $j'$.

It follows from this that, for a sesquilinear form $\Phi = \Phi_1 + i \Phi_2$ to be zero, it is necessary and sufficient that $\Phi_1$ (resp. $\Phi_2$) be zero. Now, if $E = E'$, one has $\Phi(y, x) = \Phi_1(y, x) + i \Phi_2(y, x)$ and $\overline{\Phi(x, y)} = \Phi_1(x, y) - i \Phi_2(x, y)$; for these two expressions to be equal, in other words for $\Phi$ to be hermitian, it is necessary and sufficient therefore that $\Phi_1$ be symmetric (resp. that $\Phi_2$ be antisymmetric).

#### Remark 1 {#alg-ix-s3-n3-rem-1 .statement}

The formulas (7) and (8) show that, if $x \in E$, in order that $\Phi(x, x') = 0$ for all $x' \in E'$, it is necessary and sufficient that $\Phi_1(x, x') = 0$ (resp. $\Phi_2(x, x') = 0$) for all $x' \in E'$.
2) The adjoint of an endomorphism $u$ of $E$ with respect to $\Phi$ ($\S 1$, n° 8) is the same as the adjoint of $u$ (considered as an endomorphism of $E_0$) with respect to $\Phi_1$ (resp. $\Phi_2$).

### 4. Quadratic forms.

#### Definition 2 {#alg-ix-s3-def-2 .statement}

We suppose that the ring $A$ is commutative. We say that a mapping $Q$ of $E$ into $A$ is a quadratic form on $E$ if
1) $Q(\alpha x) = \alpha^2 Q(x)$ for $\alpha \in A$ and $x \in E$;
2) the mapping $\Phi : (x, y) \to Q(x + y) - Q(x) - Q(y)$ of $E \times E$ into $A$ is a bilinear form.
The bilinear form $\Phi$ (which is necessarily symmetric) is called the bilinear form associated with $Q$. If $\Phi$ is non-degenerate, we say that $Q$ is non-degenerate.

Since $Q(2x) = 4Q(x)$, it follows at once from 2) that
$$
\Phi(x, x) = 2Q(x).
$$
In particular, if $A$ is a ring of characteristic 2, the form $\Phi$ is alternating.

We shall say that two elements (resp. two subsets) of $E$ are orthogonal relative to $Q$ if they are orthogonal relative to the bilinear form associated with $\Phi$.

Let $(x_i)_{i \in I}$ be a family of elements of $E$ and $(a_i)_{i \in I}$ a family of elements of $A$ all but a finite number of which are zero. By induction on the number of indices $i$ for which $a_i \neq 0$, one easily shows that
$$
Q(\sum_i a_i x_i) = \sum_i a_i^2 Q(x_i) + \sum_{\{i, j\}} a_i a_j \Phi(x_i, x_j),
$$

the last summation being extended over the two-element subsets of I.

For every bilinear form $f$ on $E \times E$, we define a quadratic form $Q$ by putting $Q(x) = f(x, x)$; the bilinear form $\Phi$ associated with $Q$ is then defined by $\Phi(x, y) = f(x, y) + f(y, x)$ for $x, y$ in $E$. Moreover, if one supposes that the scalar 2 has an inverse $\frac{1}{2}$ in $A$, there exists one and only one symmetric bilinear form $f$ such that $Q(x) = f(x, x)$, namely $f = \frac{1}{2} \Phi$; the discriminant of $f$ with respect to a system $S = (x_1, \ldots, x_n)$ is also called the discriminant of $Q$ with respect to $S$. There is therefore in this case a one-to-one correspondence between the quadratic forms and the symmetric bilinear forms on $E$ (cf. exerc. 6).

In the case of a free module, we have in addition the following result:

#### Proposition 2 {#alg-ix-s3-prop-2 .statement}

Suppose that $A$ is commutative and that $E$ admits a basis $(e_i)_{i \in I}$. Then, for every quadratic form $Q$ on $E$, there exists a bilinear form $f$ on $E \times E$ such that $Q(x) = f(x, x)$ for every $x \in E$. For every family $(b_{ij})_{(i,j) \in I \times I}$ of scalars such that $b_{ij} = b_{ji}$ for $(i, j) \in I \times I$, there exists one and only one quadratic form $Q$ such that

$$
Q(e_i) = b_{ii}, \quad \Phi(e_i, e_j) = b_{ij} \text{ pour } i \neq j,
$$

where $\Phi$ denotes the bilinear form associated with $Q$; then $Q$ is given by the formula

$$
Q(\sum_i a_i e_i) = \sum_{\{i,j\}} b_{ij} a_i a_j,
$$

the last summation extending over the subsets $\{i, j\}$ of $I$ having one or two elements.

En effet, comme the formula (16) is only a transcription of formula (14), the uniqueness of a quadratic form $Q$ satisfying (15) is proved. To prove its existence, let us first remark that there exists a family $(b'_{ij})$ of elements of $A$ such that $b'_{ii} = b_{ii}$ and that $b'_{ij} + b'_{ji} = b_{ij}$ for $i \neq j$; one obtains, for example, such a family by endowing $I$ with an ordered set structure (*Theory of Sets*, Chapter III, § 2, No. 3, Theorem 1) and by setting $b'_{ij} = b_{ij}$ for $i < j$ and $b'_{ij} = 0$ for $i > j$. Since the $e_i$ form a basis of $E$, there exists a bilinear form $f$ on $E \times E$ such that $f(e_i, e_j) = b'_{ij}$; by setting $Q'(x) = f(x, x)$ and denoting by $\Phi'$ the bilinear form associated with the quadratic form $Q'$, one obtains $Q'(e_i) = b_{ii}$ and $\Phi'(e_i, e_j) = f(e_i, e_j) + f(e_j, e_i) = b_{ij}$. This proves our second assertion. As for the first, it follows immediately, since, by virtue of the uniqueness, if a quadratic form $Q$ satisfies (15), one has $Q(x) = Q'(x) = f(x, x)$.

The module $E$ endowed with the structure defined by a quadratic form $Q$ is called a *quadratic module*. A homomorphism of the quadratic module $(E, Q)$ into a quadratic module $(E', Q')$ is a linear mapping $u$ of $E$ into $E'$ such that $Q = Q' \circ u$; if $\Phi$ and $\Phi'$ are the bilinear forms associated with $Q$ and $Q'$, one then has $\Phi(x, y) = \Phi'(u(x), u(y))$ for $x \in E,\ y \in E$; in other words $\Phi'$ is the inverse image of $\Phi$ by $u$ (§ 1, No. 1). One says that two quadratic forms $Q$ and $Q'$ on two $A$-modules $E$ and $E'$ are *equivalent* if the corresponding quadratic modules are isomorphic.

Let $(E_i, Q_i)_{i \in I}$ be a family of quadratic modules, and let $E$ be the direct sum of the modules $E_i$. The *external direct sum* of the quadratic modules $(E_i, Q_i)$ is the quadratic module obtained by endowing $E$ with the quadratic form $Q$ defined by $Q(\sum_i x_i) = \sum_i Q_i(x_i)$ for $x_i \in E_i$. One also says that the quadratic form $Q$ is the *external direct sum* of the quadratic forms $Q_i$.

If the forms $Q_i$ are non-degenerate, the same is true of $Q$.

Let $Q$ be a quadratic form on the $A$-module $E$; if $F$ is a submodule of $E$ and if $Q$ is constant on each class modulo $F$, the mapping $\overline{Q}$ of $E/F$ into $A$ deduced from $Q$ by passing to the quotient is obviously a quadratic form, and the canonical mapping of $E$ onto $E/F$ is a homomorphism for the structures of quadratic modules. For $Q$ to be constant on each class modulo $F$, it is necessary and sufficient that we have $Q(x + y) = Q(x)$ for $x \in E$ and $y \in F$, that is, denoting by $\Phi$ the bilinear form associated with $Q$, that we have $Q(y) + \Phi(x, y) = 0$ for $y \in F$ and $x \in E$. Taking $x = 0$, we see that we have $Q(y) = 0$ for $y \in F$, and therefore

$\Phi(x, y) = 0$ for $x \in E$ and $y \in F$. In other words, if we call the kernel of the quadratic module $(E, Q)$ the set $N$ of elements $x$ of $E$ such that $Q(x) = 0$ and $\Phi(x, z) = 0$ for all $z \in E$, for $Q$ to be constant on each class modulo $F$, it is necessary and sufficient that $F$ be contained in the kernel $N$ of $(E, Q)$. It is readily verified that $N$ is a submodule of $E$. For $Q$ to be constant on each class modulo $F$, it is therefore necessary and sufficient that $F$ be generated by elements of $N$.

It is immediately seen that the kernel of the quadratic module $|E/N$ is $\{0\}$.

#### Proposition 3 {#alg-ix-s3-prop-3 .statement}

*Let $h$ be a homomorphism of $A$ into a commutative ring $A'$. For every quadratic form $Q$ on the $A$-module $E$, there exists one and only one quadratic form $Q'$ on the $A'$-module $A' \otimes_A E$ (chap. III, 2nd ed., App. II, No. 10) such that one has*
$$
Q'(1 \otimes x) = h(Q(x))
$$
for every $x \in E$. *Moreover the bilinear form $\Phi'$ associated with $Q'$ is obtained by extension of the ring of scalars from the bilinear form $\Phi$ associated with $Q$.*

We first prove that, if there exists a quadratic form $Q'$ satisfying (17), it is unique and the bilinear form $\Phi'$ associated with $Q'$ is obtained by extension of the ring of scalars from the form $\Phi$ associated with $Q$. Indeed this last assertion follows from the fact that one has
$$
\Phi'(1 \otimes x, 1 \otimes y) = Q'(1 \otimes x + 1 \otimes y) - Q'(1 \otimes x) - Q'(1 \otimes y)
= h(\Phi(x, y))
$$
for $x \in E, y \in E$. The formula (14) then shows that one has
$$
Q'(\sum_i a'_i \otimes x_i) = \sum_i a'_i{}^2 h(Q(x_i)) + \sum_{\{i, j\}} a'_i a'_j h(\Phi(x_i, x_j))
$$
for $a'_i \in A'$ and $x_i \in E$, which proves the uniqueness of $Q'$.

To prove the existence of $Q'$, we shall first suppose that the module $E$ admits a basis $(e_i)_{i \in I}$. There then exist elements $b_{ij}$ of $A$ such that $b_{ij} = b_{ji}$ and that $Q(\sum_i a_i e_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$ for $a_i \in A$ (prop. 2). Since the elements $1 \otimes_A e_i$ form a basis of the

A'-module $A' \otimes_A E$, we define a quadratic form $Q'$ on this latter module by putting
$$
Q'(\sum_i a'_i \otimes e_i) = \sum_{\{i,j\}} a'_i a'_j h(b_{ij})
$$
for $a'_i \in A'$; whence, for $x = \sum_i a_i e_i \in E$
$$
Q'(1 \otimes x) = Q'(\sum_i h(a_i) \otimes e_i) = \sum_{\{i,j\}} h(a_i) h(a_j) h(b_{ij}) = h(Q(x)),
$$
which proves the existence of $Q'$ in this case.

Let us now pass to the general case. Let $(x_i)_{i \in I}$ be a system of generators of $E$, $A^{(t)}$ the module of formal linear combinations of elements of $I$ (Chap. II, § 1, No. 8), and $(e_i)_{i \in I}$ the canonical basis of $A^{(t)}$. The linear mapping $u$ of $A^{(t)}$ into $E$ defined by $u(e_i) = x_i$ is surjective since the elements $x_i$ generate $E$. It follows (Chap. III, 2nd ed., App. II, No. 5, Prop. 4) that the mapping $1 \otimes u$ of $A' \otimes A^{(t)}$ into $A' \otimes E$ is surjective, and that its kernel $P'$ is generated by the elements of the form $1 \otimes p$ with $u(p) = 0$. Let then $Q'_1$ be the extension to $A' \otimes_A A^{(t)}$ of the quadratic form $Q_1 = Q \circ u$ on $A^{(t)}$. If $p$ is an element of $A^{(t)}$ such that $u(p) = 0$, we have $Q'_1(1 \otimes p) = h(Q_1(p)) = 0$ and (denoting by $\Phi'_1$ the bilinear form associated with $Q'_1$) $\Phi'_1(1 \otimes p, 1 \otimes x) = h(\Phi(u(p), u(x))) = 0$ for all $x \in A^{(t)}$. Thus, if $u(p) = 0$ ($p \in A^{(t)}$), then $1 \otimes p$ belongs to the kernel of the quadratic module $A' \otimes_A A^{(t)}$, and there exists consequently, as we have seen above, a quadratic form $Q'$ on $A' \otimes_A E$ such that $Q'_1 = Q' \circ (1 \otimes u)$. Since $u$ is surjective, we see that $Q'$ satisfies condition (17). Q.E.D.

The quadratic form $Q'$, whose existence and uniqueness are assured by Prop. 3, is called the extension of $Q$ to $A' \otimes_A E$ (with respect to $h$). One also says that $Q'$ is obtained from $Q$ by extension of the ring of scalars.

Exercises. — 1) Let $A$ be a field, $E$ a left vector space over $A$, $\Phi$ a sesquilinear form on $E$ (for an antiautomorphism $J$ of $A$). Assume that the rank (finite or infinite) of $\Phi$ is $\geqslant 2$, and that the relations $\Phi(x, y) = 0$ and $\Phi(y, x) = 0$ are equivalent.
a) Now prove that there exists $\lambda \neq 0$ in $A$ such that one has $\Phi(y, x) = \lambda (\Phi(x, y))^J$. (Use exerc. 8 of § 1).
b) Now prove that there exists $\alpha \in A$ such that the sesquilinear form $\Phi \alpha$ (for the antiautomorphism $\xi \to \alpha^{-1} \xi^J \alpha$) is hermitian or alternating.

(First note that one has $\xi^{J^2} = \lambda^{-1} \xi \lambda^{-J}$ and $\lambda \lambda^J = \lambda^J \lambda = 1$. Then distinguish two cases according as $\xi + \xi^J \lambda^{-1} = 0$ for every $\xi \in A$ or not; in the second case, prove that every element $\neq 0$ of the form $\alpha = \xi + \xi^J \lambda^{-1}$ answers the question).

2) Let $\Phi$ be an $\varepsilon$-hermitian sesquilinear form on a finite-dimensional vector space $E$ over a field $A$.

a) Now prove that for every vector subspace $M$ of $E$, one has $(M^0)^0 = M + E^0$ and $\dim M^0 + \dim M = \dim E + \dim (M \cap E^0)$.

b) If $M_1, M_2$ are two vector subspaces of $E$, now prove that one has $\dim (M_1 \cap M_2^0) + \dim (M_2 + M_1^0) = \dim E + \dim (M_1 \cap E^0)$ (consider the canonical mapping of $E$ onto $E/E^0$).

3) Let $K$ be a commutative ring, $f$ a monic polynomial of $K[X]$, of degree $n \geqslant 1$; let $A$ be the quotient algebra $K[X]/(f)$ admitting as basis over $K$ the elements $1, \xi, \xi^2, \ldots, \xi^{n-1}$ (chap. IV, § 1, no 5, prop. 4). Now prove that the datum of an $A$-module $E$ is equivalent to the datum of a $K$-module $E_0$ and of a $K$-endomorphism $j$ of $E_0$ such that $f(j) = 0$. For every $u \in E^*$, one sets $u(x) = \sum_{k=0}^{n-1} u_k(x) \xi^k$; prove that if $\alpha_0 = f(0)$ is invertible in $K$, the mapping $u \to u_0$ is a $K$-isomorphism of $E^*$ onto $(E_0)^*$, whose inverse isomorphism is to be made explicit.

¶ 4) a) Let $A$ be a ring (commutative or not), $\sigma$ an automorphism of $A$ such that there exists an invertible element $\gamma \in A$ satisfying $\gamma^\sigma = \gamma$, and such that $\xi^{\sigma^2} = \gamma \xi \gamma^{-1}$ for all $\xi \in A$. Let $B$ be a left $A$-module having a basis of two elements $(e_1, e_2)$; now prove that a ring structure is defined on $B$ by taking as multiplication in $B$ the law of composition

$$
(\xi e_1 + \eta e_2)(\xi' e_1 + \eta' e_2) = (\xi \xi' + \eta \eta' \gamma) e_1 + (\eta \xi'^\sigma + \xi \eta') e_2.
$$

For this ring structure, $e_1$ is the unit element (which we identify with the unit element 1 of $A$); if we put $e_2 = \rho$, we have $\rho^2 = \gamma$ and $\rho \xi = \xi^\sigma \rho$ for all $\xi \in A$; moreover, $B$ is a right $A$-module, of which 1 and $\rho$ form a basis. If $A$ is a field, a necessary and sufficient condition for $B$ to be a field is that $\gamma$ not be of the form $\lambda^\sigma \lambda$ (where $\lambda \in A$). (Cf. Chapter VIII, § 12, exerc. 8).

b) Let $J$ be an involutory antiautomorphism of $A$. Suppose that there exists an invertible element $\delta \in A$ satisfying the following conditions:

(1) $\delta^J = \delta, \quad \delta^\sigma \delta = \gamma \gamma^J, \quad (\xi^J)^\sigma = \delta (\xi^\sigma)^J \delta^{-1}$ for all $\xi \in A$.

Now prove that $J$ can be extended to an involutory antiautomorphism of $B$ (again denoted by $J$) by putting

(2) $$ (\xi + \eta \rho)^J = \xi^J + \gamma^{-1} \delta^\sigma (\eta^J)^\sigma \rho. $$

If, moreover, $A$ and $B$ are fields and if $\sigma$ is not an inner automorphism, now prove that the conditions (1) are necessary for the existence of an extension of $J$ to an involutory antiautomorphism of $B$ (putting $\rho^J = \alpha + \beta \rho$, with $\alpha, \beta$ in $A$, now prove that necessarily $\alpha = 0$, by writing the condition $(\rho \xi)^J = \xi^J \rho^J$ for all $\xi \in A$).

c) Suppose the conditions (1) are satisfied and the involutive antiautomorphism J extended to B by (2). Let F be a unitary B-module, E the unitary A-module deduced from F by restriction to A of the ring of scalars; the mapping $j : x \to \rho x$ is then a bijective semilinear mapping of E onto itself, relative to the automorphism $\sigma$ of A and such that $j^2(x) = \gamma x$. Let $\Phi$ be a hermitian form on F (for J); for $x \in E$, $y \in E$, put $\Phi(x, y) = \Phi_1(x, y) + \Phi_2(x, y)\rho$, where $\Phi_1(x, y) \in A$, $\Phi_2(x, y) \in A$. Now prove that $\Phi_1$ is a hermitian form on E (for J), such that
$$
\Phi_1(j(x), j(y)) = (\Phi_1(x, y))^{\sigma \delta};
$$
we have $\Phi_2(x, y) = \Phi_1(x, j(y))\delta^{-1}$, $\Phi_2$ is a sesquilinear form on E for the antiautomorphism (in general non-involutive) $\xi \to (\xi^J)^{\sigma}$, such that
$$
\Phi_2(j(x), j(y)) = (\Phi_2(x, y))^{\sigma \delta^{\sigma}}
$$
and
$$
\Phi_2(y, x) = \gamma^J \delta^{-1}((\Phi_2(x, y))^J)^{\sigma}.
$$

Conversely. In order that $\Phi$ be non-degenerate, it is necessary and sufficient that $\Phi_1$ or $\Phi_2$ be non-degenerate. Special case where B is a quaternion algebra over a commutative ring K, corresponding to a pair $(\alpha, \beta)$ of elements of K, $\beta$ being invertible, A the subalgebra $K + Ku$ of B, and J and $\sigma$ the mapping $\xi \to \bar{\xi}$ (chap. II, § 7, no 8).

d) Let $u$ be an automorphism of the A-module E. In order that $u$ be an automorphism of the B-module F, leaving the form $\Phi$ invariant, it is necessary and sufficient that $u$ satisfy any two of the following three conditions:
1° $u$ leaves $\Phi_1$ invariant;
2° $u$ leaves $\Phi_2$ invariant;
3° $u$ commutes with $j$.

5) Let $A$ be a commutative ring, $E$ an $A$-module, $(x_i)_{i \in I}$ a system of generators of $E$; let $R$ be the submodule of the module $A^{(1)}$ formed by the elements $(y_i)_{i \in I}$ such that $\sum_i y_i x_i = 0$, and let $(a_{\lambda})_{\lambda \in L}$ be a system of generators of $R$ (with $a_{\lambda} = (a_{\lambda i})_{i \in I}$). Let $(b_{ij})$ be a family of elements of $A$ $(i \in I, j \in I)$. In order that there exist a quadratic form $Q$ such that $Q(x_i) = b_{ii}$ and $\Phi(x_i, x_j) = b_{ij}$ for $i \neq j$ ($\Phi$ denoting the bilinear form associated with $Q$), it is necessary and sufficient that $b_{ij} = b_{ji}$ whatever $i, j$ in $I$, and that, whatever $\lambda \in L$ and $i \in I$, one has
$$
\sum_{\{i, j\}} b_{ij} a_{\lambda i} a_{\lambda j} = \sum_{j \neq i} b_{ij} a_{\lambda j} + 2b_{ii} a_{\lambda i} = 0;
$$
one then has $Q(\sum a_i x_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$. Deduce a new proof of Proposition 3 of No. 4. (Notice that the $x'_i = 1 \otimes x_i$ form a system of generators of $A' \otimes_A E$, and that the a-module $A' \otimes_A E$ is isomorphic to $A'^{(1)}/R'$, where $A'^{(1)}$ is identified with $A' \otimes_A A^{(1)}$ and $R'$ is generated by the image of R by the canonical mapping of $A^{(1)}$ into $A'^{(1)}$.

6) Let $A$ be a commutative ring of characteristic 2, $E$ a free $A$-module, $\mathcal{A}$ (resp. $\mathcal{S}$, $\mathcal{Q}$) the $A$-module of alternating bilinear forms (resp. symmetric bilinear forms, quadratic forms) on $E$. One has $\mathcal{A} \subset \mathcal{S}$; one defines in addition a linear mapping $\omega$ of $\mathcal{S}$ into $\mathcal{Q}$, and a linear mapping $\theta$ of $\mathcal{Q}$ into $\mathcal{A}$ as follows: for every bilinear form $\Phi \in \mathcal{S}$, $\omega(\Phi)$ is the quadratic form $x \to \Phi(x, x)$, and for every quadratic form $Q \in \mathcal{Q}$, $\theta(Q)$ is the bilinear form associated with $Q$, which is alternating. Show that $\omega(0) = \mathcal{A}$, $\theta(\mathcal{Q}) = \mathcal{A}$ and $\theta(0) = \omega(\mathcal{S})$.

¶ 7) Let $A$ be a commutative ring, $E, F$ two $A$-modules. A mapping $Q$ of $E$ into $F$ is said to be *quadratic* if it satisfies the following conditions: $1^\circ$ $Q(\alpha x) = \alpha^2 Q(x)$ for $\alpha \in A, x \in E$; $2^\circ$ the mapping $(x, y) \to Q(x + y) - Q(x) - Q(y)$ of $E \times E$ into $F$ is bilinear. If $f$ is a linear mapping of an $A$-module $E_1$ into $E$, $Q \circ f$ is a quadratic mapping of $E_1$ into $F$.

$a)$ Let $E$ be an $A$-module, $A^{(E)}$ the module of formal linear combinations of the elements of $E$ with coefficients in $A$ (chap. II, § 1, no 8), and for every $x \in E$, let $\varepsilon_x$ be the corresponding element of the canonical basis of $A^{(E)}$. Let $\Gamma^2(E)$ be the quotient of $A^{(E)} \times (E \otimes_A E)$ by the submodule $R$ generated by the elements $(\varepsilon_{x+y} - \varepsilon_x - \varepsilon_y, -x \otimes y)$ and $(\varepsilon_{\lambda x} - \lambda^2 \varepsilon_x, 0)$, for $x \in E, y \in E, \lambda \in A$. For every $x \in E$, put $\gamma(x) = \varphi(\varepsilon_x, 0)$, denoting by $\varphi$ the canonical mapping of $A^{(E)} \times (E \otimes E)$ onto $\Gamma^2(E)$; $\gamma$ is called the *canonical mapping* of $E$ into $\Gamma^2(E)$. Prove that $\gamma$ is a quadratic mapping of $E$ into $\Gamma^2(E)$ and that, for every quadratic mapping $Q$ of $E$ into an $A$-module $F$, there exists one and only one *linear mapping* $q$ of $\Gamma^2(E)$ into $F$ such that $Q = q \circ \gamma$ (in other words, $(\Gamma^2(E), \gamma)$ is a solution of a universal mapping problem; cf. *Ens.*, chap. IV, § 3).

Pour every couple of $A$-modules $E, E'$ and every linear mapping $f$ of $E$ into $E'$, now prove that, if $\gamma'$ denotes the canonical mapping of $E'$ into $\Gamma^2(E')$, there exists one and only one linear mapping $\bar{f}$ of $\Gamma^2(E)$ into $\Gamma^2(E')$ such that $\gamma' \circ f = \bar{f} \circ \gamma$.

$b)$ Suppose that $E$ is direct sum of two submodules $M, N$. Define a canonical isomorphism of $\Gamma^2(E)$ onto the direct sum of the modules $\Gamma^2(M), \Gamma^2(N)$ and $M \otimes N$ (show that this direct sum is solution of the same universal mapping problem as $\Gamma^2(E)$).

$c)$ Let $F$ be a submodule of $E$, $j$ the canonical injection of $F$ into $E$. Define a canonical isomorphism of $\Gamma^2(E/F)$ onto

$$
\Gamma^2(E)/(\bar{j}(\Gamma^2(F)) + \psi(E \times F)),
$$

where $\psi(x, y) = \varphi(0, x \otimes j(y))$ for $x \in E, y \in F$. (Same method).

$d)$ Let $A'$ be a commutative ring, $h$ a homomorphism of $A$ into $A'$. Define a canonical isomorphism of $\Gamma^2(A' \otimes_A E)$ onto $A' \otimes_A \Gamma^2(E)$ (same method).

$e)$ There exists one and only one linear mapping $s$ of $\Gamma^2(E)$ into $E \otimes E$ such that $s(\gamma(x)) = x \otimes x$ for all $x \in E$; show that if $E$ is a free module, s is an isomorphism onto the submodule of symmetric tensors of order 2 on E.

f) Suppose that $A = \mathbf{Z}$ and that E is a finite cyclic group of order n. Show that $\Gamma^2(E)$ is a cyclic group of order n if n is odd, of order $2n$ if n is even. (First remark that if a is a generator of E, $\gamma(a)$ is a generator of $\Gamma^2(E)$, and that $\gamma(-ha) = \gamma(ha)$ for every integer h; deduce from this that if n is odd, $n\gamma(a) = 0$ by taking $h = (n-1)/2$; show in the same way that $2n\gamma(a) = 0$ if n is even. Finally prove that if n is odd (resp. even), there exists a quadratic mapping Q of E into a cyclic group of order n (resp. $2n$) applying a to a generator of this group).

8) Let A be a commutative field, E, F two vector spaces over A. Let g be a mapping of E into F, such that there exist three mappings $a, b, c$ of $E \times E$ into F, satisfying the identity

$$
g(\lambda x + \mu y) = \lambda^2 a(x, y) + \lambda \mu b(x, y) + \mu^2 c(x, y)
$$

whatever $x, y$ in E, $\lambda, \mu$ in A.

a) Show that one has $a(x, y) = g(x), c(x, y) = g(y), b(y, x) = b(x, y)$ and $b(\lambda x, y) = \lambda b(x, y)$; moreover, if one sets

$$
d(x, y, z) = b(x + y, z) - b(x, z) - b(y, z)
$$

show that one has $d(x, y, z) = d(y, z, x) = d(z, x, y)$ and conclude that $d(\lambda x, \mu y, v z) = \lambda \mu v d(x, y, z)$.

b) Deduce from a) that if $A \neq \mathbf{F}_2$, one necessarily has $d(x, y, z) = 0$ and consequently that g is a quadratic mapping (Exercise 7). On the contrary, if $A = \mathbf{F}_2$ and if dim E $\geqslant 3$, show that there exist mappings g of E into A, satisfying (4) and for which $d(x, y, z)$ is not identically zero.

9) Let A be a commutative ring, E an A-module having a basis of n elements, $\Phi$ a symmetric bilinear form on E. Let e be an element of $\bigwedge^n E$ forming a basis of this module, $\Delta$ the discriminant of $\Phi$ with respect to e, $\varphi_p$ the canonical isomorphism of $\bigwedge^p E$ onto $\bigwedge^{n-p} E^*$ relative to e (Chapter III, § 8, No. 5). For $x \in \bigwedge^p E$, let $d_{(p)}(x) = \varphi_{n-p}^{-1}(d_{\Phi_{(p)}}(x))$; show that the mapping $d_{(p)}$ of $\bigwedge^p E$ into $\bigwedge^{n-p} E$ has the following properties:

a) For every $x \in \bigwedge^p E$, $d_{(n-p)}(d_{(p)}(x)) = (-1)^{p(n-p)} \Delta x$.

b) For every pair of elements $x, y$ of $\bigwedge^p E$, one has

$$
x \wedge d_{(p)}(y) = \Phi_{(p)}(x, y)e \quad \text{and} \quad \Phi_{(n-p)}(d_{(p)}(x), d_{(p)}(y)) = \Delta \Phi_{(p)}(x, y).
$$

c) Suppose in addition that A is a field and that $\Phi$ is non-degenerate. Then, if x is a decomposable p-vector $\neq 0$ corresponding to a subspace F of E (Chapter III, § 7, No. 3), $d_{(p)}(x)$ is a decomposable $(n-p)$-vector $\neq 0$ corresponding to the subspace $F^0$ orthogonal to F.

d) Extend the preceding results to the case where (A being a commutative ring), Φ is an ε-hermitian sesquilinear form for an involutive automorphism J ≠ 1 of A.

10) a) Let A be a commutative ring, E an A-module having a basis of 3 elements, Φ a symmetric bilinear form on E. With the notation of Exercise 9, for two arbitrary elements x, y of E, put $x \overline{\wedge} y = d_{(2)}(x \wedge y)$, and say that this element is the vector product of x and y (relative to $\Phi$ and to the basis e of $\bigwedge^3 E$). Show that $(x, y) \to x \overline{\wedge} y$ is an alternating bilinear mapping of $E \times E$ into E, and that $x \overline{\wedge} y$ is orthogonal to x and to y.

b) Let α, β be two invertible elements of A, B the quaternion algebra over A corresponding to the pair ($α, β$) (Chapter II, § 7, No. 8), 1, u, v, ω the canonical basis of B over A; let E be the submodule of B having u, v, ω as basis. Show that if x, y are two quaternions belonging to E, one has
$$
xy = \Phi(x, y) + x \overline{\wedge} y
$$
where Φ is a symmetric bilinear form on E, such that the linear mappings associated with Φ are bijective, and $x \overline{\wedge} y$ is the vector product of x and y relative to the form Φ and to the basis $α^{-1}β^{-1}u \wedge v \wedge \omega$ of $\bigwedge^3 E$.

11) Let Φ be a non-degenerate ε-hermitian sesquilinear form on a finite-dimensional vector space E. A vector subspace M of E is said to be weakly orthogonal to a vector subspace N (relative to Φ) if one of the two subspaces M, N° contains the other.

a) Show that the relation "M is weakly orthogonal to N" is symmetric.

b) If M and N are weakly orthogonal, M° and N° are weakly orthogonal.

c) If M and N are weakly orthogonal and if $M \cap N = \{0\}$, M and N are orthogonal.
