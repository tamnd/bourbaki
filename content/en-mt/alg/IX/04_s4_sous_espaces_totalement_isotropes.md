---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 4
section_title: Sous-espaces totalement isotropes. Théorème de Witt
lang: en
source: alg-ix-fr
pdf_pages: 0061-0077
extraction: ocr
subsections:
    - "no": 1
      title: Sous-espaces isotropes.
      page: 0
      pdf_page: 62
    - "no": 2
      title: Décomposition de Witt.
      page: 0
      pdf_page: 63
    - "no": 3
      title: Théorème de Witt.
      page: 0
      pdf_page: 69
statements: 17
exercises: 0
content_sha256: 65bf44b0c346820d6e7a371b59c844daffa3b62294d94711af9f34642b033939
translated_from: content/fr/alg/IX/04_s4_sous_espaces_totalement_isotropes.md
source_lang: fr
translation_method: machine
source_content_sha256: 6501e14acfaa6e7ef3faff319553f4fa16f2473df952a0c3d55ef2d0084076ae
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-en-mt-dc2ffc45
glossary_version: 34
glossary_terms_sha256: 7164fd13e2322a6d0f0ee4ee39e0c1a99ebdbb8396b67d28c78d70d7d7fa8c11
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. Totally isotropic subspaces. Witt's Theorem

In this paragraph it is assumed, unless expressly stated otherwise, that A is a field. By Φ we denote either an ε-hermitian form on E (with respect to the involutory antiautomorphism $λ \to \overline{λ}$ of A), or the symmetric bilinear form associated with a quadratic form Q on E (A being assumed commutative in the latter case).

### 1. Isotropic subspaces.

#### Definition 1 {#alg-ix-s4-def-1 .statement}

Given a module E over the ring A, an element x of E is said to be isotropic if $\Phi(x, x) = 0$. A submodule F of E is said to be
    1) isotropic if there exists an element $x \neq 0$ of F orthogonal to F;
    2) totally isotropic if the restriction of $\Phi$ to F is zero.

When the module E is endowed with a quadratic form Q, an element of E will be said to be isotropic (resp. a submodule of E to be isotropic, or totally isotropic) if this element is isotropic (resp. if this submodule is isotropic, or totally isotropic) relative to the bilinear form associated with Q.

An isotropic vector is simply a vector orthogonal to itself. To say that a submodule F is isotropic means that $F \cap F^0 \neq \{0\}$, or, equivalently, that the restriction of $\Phi$ to F is degenerate; a non-isotropic submodule G of E is therefore a submodule such that the restriction of $\Phi$ to G is non-degenerate. In order that a submodule F of E be totally isotropic, it is necessary and sufficient that $F \subset F^0$. If F is a totally isotropic submodule of E, the same is true of every submodule $F'$ contained in F. The sum of a family of pairwise orthogonal totally isotropic submodules is a totally isotropic submodule. The set of totally isotropic submodules of E, ordered by inclusion, is obviously inductive; it follows that every totally isotropic submodule is contained in a maximal totally isotropic submodule.

#### Proposition 1 {#alg-ix-s4-prop-1 .statement}

Suppose that A is a field. Let F be a non-isotropic finite-dimensional subspace of E; then E is the direct sum of F and $F^0$.

Indeed, since the restriction $\Phi'$ of $\Phi$ to F is non-degenerate by assumption, the mapping $d_{\Phi'}$ from F into its dual $F^*$ associated on the right with $\Phi'$ is injective, hence bijective since F and $F^*$ are two spaces of the same finite dimension. Consequently, for every $y \in E$, there exists one and only one element $y_0$ of F such that $\Phi(x, y) = \Phi(x, y_0)$ for every $x \in F$, that is, $y - y_0 \in F^0$; this proves that E is the direct sum of F and $F^0$.

#### Corollary {#alg-ix-s4-n1-cor-1 .statement}

If F is a finite-dimensional subspace of E, and if Φ is non-degenerate, the following conditions are equivalent:

a) F is non-isotropic.
b) F^0 is non-isotropic.
c) E is the direct sum of F and F^0.

Proposition 1 shows indeed that a) implies c), and that c) implies a) and b). Finally, if F^0 is non-isotropic, we have F ∩ F^0 ⊂ F^0 ∩ F^{00} = {0}; hence F is non-isotropic, which shows that b) implies a).

#### Definition 2 {#alg-ix-s4-def-2 .statement}

Let Q be a quadratic form on E. An element x of E is said to be singular (relative to Q) if Q(x) = 0. A submodule F of E is said to be:
1) singular if there exists an element x ≠ 0 of F which is singular and orthogonal to F;
2) totally singular if the restriction of Q to F is zero.

The kernel of the quadratic module (E, Q) (§ 3, n° 4) consists of the singular elements of E^0; in order that a submodule F be singular, it is necessary and sufficient that its kernel be ≠ {0}. Since Φ(x, y) = Q(x + y) − Q(x) − Q(y), every totally singular submodule ≠ {0} is singular. Since Φ(x, x) = 2Q(x), every singular vector is isotropic and every singular submodule (resp. totally singular submodule) is isotropic (resp. totally isotropic); the converse is true if A is a field of characteristic ≠ 2. Every submodule contained in a totally singular submodule is itself totally singular. The sum of a family of pairwise orthogonal totally singular submodules is a totally singular submodule. The set of totally singular submodules of E, ordered by inclusion, is inductive; hence every totally singular submodule of E is contained in a maximal totally singular submodule.

### 2. Witt decomposition.

To the conventions already in force since the beginning of the present paragraph, we shall add the following:

Bourbaki XXIV.

CONDITION (T). — For every $x \in E$, there exists $\alpha \in A$ such that $\Phi(x, x) = \alpha + \varepsilon \bar{\alpha}$.

This condition is always satisfied when $\Phi$ is alternating, or when $\varepsilon = 1$ and $A$ is a field of characteristic $\neq 2$, by taking $\alpha = \frac{1}{2} \Phi(x, x)$ (cf. exerc. 1 and 14).

#### Lemma 1 {#alg-ix-s4-lem-1 .statement}

Let $\Phi$ be an $\varepsilon$-hermitian form satisfying (T) (resp. the bilinear form associated with a quadratic form Q) on $E$, and let F be a totally isotropic (resp. totally singular) subspace of $E$, not reduced to 0. For every $x \in E$ not orthogonal to F and every $\alpha \in A$, there exists $y \in F$ such that

$$
\Phi(x + y, x + y) = \alpha + \varepsilon \bar{\alpha} \quad (\text{resp. } Q(x + y) = \alpha).
$$

Put $\Phi(x, x) = \beta + \varepsilon \bar{\beta}$ (resp. $Q(x) = \beta$). For $y \in F$ we then have $\Phi(x + y, x + y) = (\beta + \Phi(x, y)) + \varepsilon (\beta + \Phi(x, y))$ since $\Phi(y, y) = 0$ (resp. $Q(x + y) = \beta + \Phi(x, y)$ since $Q(y) = 0$). Since $x$ is not orthogonal to F, the affine linear function $y \to \Phi(x, y) + \beta$ on F is not constant; it therefore takes the value $\alpha$ for some element $y$ of F, which thus answers the question.

On appelle décomposition de Witt de E toute décomposition de E en somme directe de trois sous-espaces F, F', G tels que F et F' soient totalement isotropes (resp. totalement singuliers) et que G soit non isotrope et soit orthogonal à $F + F'$; si E est de dimension finie, la matrice de $\Phi$ par rapport à une base de E adaptée à une décomposition de Witt de E se met sous la forme

$$
\begin{pmatrix}
0 & U & 0 \\
\varepsilon \overline{U} & 0 & 0 \\
0 & 0 & V
\end{pmatrix}
$$

(1)

On dit que $\Phi$ est une forme neutre si elle est non dégénérée et si E est de dimension finie et est somme directe de deux sous-espaces totalement isotropes (resp. totalement singuliers). La somme directe de deux formes neutres est une forme neutre.

#### Proposition 2 {#alg-ix-s4-prop-2 .statement}

Soit $\Phi$ une forme $\varepsilon$-hermitienne non dégénérée vérifiant (T) (resp. la forme bilinéaire associée à une forme quadratique non dégénérée Q), et soit F un sous-espace totalement isotrope (resp. totalement singulier) de dimension finie r.

a) Si $F'$ est un sous-espace totalement isotrope de dimension r tel que $F' \cap F^0 = \{0\}$, alors $F + F'$ est non isotrope et, pour toute base $(f_i)$ de F, il existe une base $(f'_i)$ de $F'$ telle que $\Phi(f_i, f'_j) = \delta_{ij}$ (indice de Kronecker) pour $i, j = 1, \ldots, r$.

b) Si G est un sous-espace totalement isotrope (resp. totalement singulier) de dimension $\leq r$ tel que $G \cap F^0 = \{0\}$, il existe un sous-espace totalement isotrope (resp. totalement singulier) $F' \supset G$ de dimension r tel que $F' \cap F^0 = \{0\}$.

Soit $\Psi$ la restriction de $\Phi$ à $F \times F'$; pour $x' \in F'$, la relation «$\Phi(x, x') = 0$ pour tout $x \in F$ » entraîne $x = 0$ puisque $F' \cap F^0 = \{0\}$. L’assertion a) résulte alors du cor. de la prop. 6 du § 1, No. 6, à l’exception du fait que $F + F'$ est non isotrope. Or le sous-espace $H = (F + F') \cap (F + F')^0$ est égal à $(F + F') \cap F^0 \cap F'^0$. Comme $F \subset F^0$, on a $(F + F') \cap F^0 = F + (F' \cap F^0) = F$, d’où $H = F \cap F'^0$; donc $H = \{0\}$ puisqu’on a vu que $\Psi$ est non dégénérée. Ceci prouve bien que $F + F'$ est non isotrope.

Pour démontrer b), nous procéderons par récurrence descendante sur $s = \dim G$. Il nous suffit ainsi de prouver que, si $s < r$, il existe un sous-espace totalement isotrope (resp. totalement singulier) $G'$ contenant G, de dimension $s + 1$, et tel que $G' \cap F^0 = \{0\}$. Comme $\dim G < \dim F$, la restriction de $\Phi$ à $F \times G$ est dégénérée, et comme $G \cap F^0$ est nul, $F \cap G^0$ est non nul. Si l’on avait alors $G + F^0 \supset G^0$, on en déduirait, en prenant les sous-espaces orthogonaux et en remarquant que $F = F^{00}$ et que $G = G^{00}$ ($\S 1$, No. 6, cor. 1 de la prop. 4), que $G^0 \cap F \subset G$, d’où

$$
G^0 \cap F \subset G \cap F \subset G \cap F^0 = \{0\},
$$

ce qui est impossible. Il existe alors un élément $x$ de $G^0$ tel que $x \notin G + F^0$; comme $F \subset F^0$, on peut ajouter à $x$ un vecteur de $G^0 \cap F$ sans modifier ces propriétés; comme $G^0 \cap F$ est totalement isotrope (resp. totalement singulier) et $\neq \{0\}$, le lemme 1 montre qu’on peut choisir $x$ isotrope (resp. singulier).

Then the subspace $G' = G + Ax$ is of dimension $s + 1$, and is totally isotropic (resp. totally singular); moreover we have $G' \cap F^0 = \{0\}$ since, if $y = z + ax$ ($z \in G,\ a \in A$) is in $F^0$, we have $a = 0$, for otherwise $x \in F^0 + G$, contrary to the choice of $x$, whence $y = z \in G \cap F^0 = \{0\}$ and $y = 0$. Consequently the subspace $G'$ answers the question.

#### Corollary 1 {#alg-ix-s4-prop-2-cor-1 .statement}

*If F is a totally isotropic (resp. totally singular) subspace of dimension r, there exists a totally isotropic (resp. totally singular) subspace F' of dimension r such that $F \cap F' = \{0\}$ and $F + F'$ is non-isotropic.*

It suffices to take $G = \{0\}$ in prop. 2, b).

#### Corollary 2 {#alg-ix-s4-prop-2-cor-2 .statement}

*Two neutral $\varepsilon$-hermitian forms on spaces of the same dimension over A are equivalent.*

#### Remark {#alg-ix-s4-n2-rem-1 .statement}

Under the conditions of Corollary 1, E is the direct sum of $F + F'$ and the orthogonal of $F + F'$. We therefore have a Witt decomposition of E. By prop. 2, a), there exist bases of F and F’ such that, in matrix (1) of $\Phi$, the block $U$ is the unit matrix $1_r$.

#### Proposition 3 {#alg-ix-s4-prop-3 .statement}

*Let $\Phi$ be a non-degenerate $\varepsilon$-hermitian form satisfying (T) (resp. the bilinear form associated with a non-degenerate quadratic form Q). Let $F_1$ and $F_2$ be two maximal totally isotropic (resp. totally singular) subspaces of E, one of them being finite-dimensional. Put $F = F_1 \cap F_2$. Let $S_i \ (i = 1, 2)$ be a supplementary subspace to $F$ in $F_i$; put $S = S_1 + S_2$. Then there exist two subspaces G and H of E such that
a) The subspaces $G + F, S$ and H are non-isotropic and pairwise orthogonal;
b) E is the direct sum of F, S, G and H;
c) There is no nonzero isotropic (resp. singular) vector in H;
d) G is totally isotropic (resp. totally singular).
Moreover $F_1$ and $F_2$ are both finite-dimensional and we have dim $F_1 = \dim F_2, \dim G = \dim F, \dim S_1 = \dim S_2, \operatorname{codim} H = 2 \dim F_1$.

First observe that, if $N$ is a maximal totally isotropic (resp. totally singular) subspace, then every isotropic (resp. singular) vector $x$ orthogonal to $N$ is an element of $N$, since otherwise $N + Ax$ would contradict the maximal character of $N$. Hence if, for $i = 1,\ 2,\ x_i$ is an isotropic (resp. singular) vector of $F_i^0$, we have $x_i \in F_i$. On the other hand, if $y$ is an element of $S_1$ orthogonal to $S_2$, it is orthogonal to $F_1$ since $F_1$ is totally isotropic, hence to $F$, and consequently to $F_2 = S_2 + F$. Since $y$ is isotropic (resp. singular) and is orthogonal to $F_2$, we have

$$
y \in S_1 \cap F_2 = S_1 \cap F_1 \cap F_2 = S_1 \cap F = \{0\}.
$$

One therefore has $S_1 \cap S_2^0 = \{0\}$, and analogously $S_2 \cap S_1^0 = \{0\}$. Since one of the two subspaces $F_1, F_2$, for example $F_1$, is finite-dimensional, $S_1$ is finite-dimensional, and hence $S_1^0$ is of finite codimension ($\S 1, \mathrm{n}^\circ 6, \mathrm{cor.\ 1\ de\ la\ prop.\ 4}$), and consequently $S_2$ is finite-dimensional since $S_2 \cap S_1^0 = \{0\}$; moreover this shows that $\dim S_2 \leqslant \operatorname{codim} S_1^0 = \dim S_1$; analogously $\dim S_1 \leqslant \dim S_2$, whence $\dim S_1 = \dim S_2$. Prop. 2 a) then shows that $S = S_1 + S_2$ is non-isotropic.

Now the orthogonal $N$ of $S$ is non-isotropic ($\mathrm{n}^\circ 1, \mathrm{cor.\ de\ la\ prop.\ 1}$) and contains $F$; Cor. 1 of Prop. 2 therefore shows that there exists a subspace $G$ totally isotropic (resp. totally singular) of $N$ such that $\dim G = \dim F$, that $G \cap F = \{0\}$ and that $G + F$ is non-isotropic. Thus d) is satisfied by $G$. We shall then satisfy a) and b) by taking for $H$ the orthogonal of $G + F$ in $N$. As for c), we note that, since $H$ is orthogonal to $F_1 = S_1 + F$, there is no nonzero isotropic (resp. singular) vector in $H$ by virtue of what was noted at the beginning of the proof and of the fact that $H \cap F_1 = \{0\}$. Finally some of the assertions concerning dimensions have been proved along the way; the others follow from them trivially.

#### Corollary 1 {#alg-ix-s4-prop-3-cor-1 .statement}

Under the hypotheses of Prop. 3, two maximal totally isotropic (resp. totally singular) subspaces of finite dimension have the same dimension. For every maximal totally isotropic (resp. totally singular) subspace F of finite dimension, there exists another F' such that F ∩ F' = {0}, and under these conditions F + F' is non-isotropic.

If F ∩ F' = {0}, we shall have G = {0} with the notation of Prop. 3, and F + F' will be non-isotropic. The other assertions follow trivially from Prop. 3 and Cor. 1 of Prop. 2.

#### Corollary 2 {#alg-ix-s4-prop-3-cor-2 .statement}

Let Q be a non-degenerate quadratic form on a vector space E of finite dimension n over an algebraically closed field A; there then exists a basis (e_i)_{1 \leq i \leq n} of E such that

(2)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} \qquad si\ n = 2\nu,
$$

(3)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} + x_{2\nu+1}^2 \qquad si\ n = 2\nu + 1.
$$

Indeed, let F_1 and F_2 be two maximal totally singular subspaces such that F_1 ∩ F_2 = {0} (Cor. 1) and let q be their dimension. We then have G = {0} with the notation of Prop. 3. Taking a basis (e_i)_{1 \leq i \leq q} of F_1 and a basis (e_i)_{q+1 \leq i \leq 2q} of F_2 such that Φ(e_i, e_{j+q}) = δ_{ij} for i, j = 1, ..., q (Prop. 2 a)), we see that it suffices to show that dim H ≤ 1. Now, if x ∈ H, y ∈ H and if x ≠ 0, the equation Q(y - ax) = Q(y) - aΦ(x, y) + a^2 Q(x) = 0 has at least one solution a_0 since Q(x) ≠ 0, and we have y = a_0 x since every singular vector of H is zero.

#### Definition 3 {#alg-ix-s4-def-3 .statement}

Suppose that E is of finite dimension and that Φ is a non-degenerate ε-hermitian form satisfying (T) (resp. the bilinear form associated with a non-degenerate quadratic form Q). We call the index of Φ (resp. Q) the common dimension of the maximal totally isotropic (resp. totally singular) subspaces of E.

If n is the dimension of E and ν the index of Φ (resp. Q), Prop. 3 shows that

(4)
$$
n \geq 2\nu.
$$

Moreover, since every totally isotropic (resp. totally singular) subspace is contained in a maximal totally isotropic (resp. totally singular) subspace, the totally isotropic (resp. totally singular) subspaces which are maximal are those which are of dimension $v$. The assertion that $\Phi$ (resp. Q) is of index 0 means that every isotropic (resp. singular) vector of E is zero. In a space of even dimension $n$, the neutral forms are those of index $\frac{1}{2}n$; there is no neutral form in a space of odd dimension. Prop. 3 shows that every form is a direct sum of a neutral form and a form of index 0.

#### Proposition 4 {#alg-ix-s4-prop-4 .statement}

*A non-degenerate quadratic form Q on E such that there exists a vector $x \neq 0$ of E such that $Q(x) = 0$ being given, for every element a of A, there then exists $y \in E$ such that $Q(y) = a$.*

Indeed, according to Cor. 1 of Prop. 2, there exists a subspace $G = F + F'$ ($F, F'$: totally singular subspaces of dimension 1) of E, of dimension 2, such that the restriction of Q to G is neutral. If $\{ e, e' \}$ ($e \in F, e' \in F'$) is a basis of G, we have
$$
Q(xe + x'e') = bxx' \quad (x \in A, x' \in A, b \in A, b \neq 0).
$$
It suffices therefore to take for $y$ the vector $ae + b^{-1}e'$.

### 3. Witt's Theorem.

Given two vector spaces E, $E'$ over A provided respectively with two sesquilinear forms $\Phi, \Phi'$ (resp. with two quadratic forms Q, $Q'$), a *metric homomorphism* from E into $E'$ is any linear mapping $u$ from E into $E'$ such that $\Phi'(u(x), u(y)) = \Phi(x, y)$ (resp. $Q'(u(x)) = Q(x)$) for $x \in E, y \in E$. If E and $E'$ have the same finite dimension and if $\Phi$ (resp. Q) is non-degenerate, every metric homomorphism $u$ from E into $E'$ is an isomorphism, since $u(x) = 0$ implies $\Phi(x, y) = 0$ for every $y \in E$, hence $x = 0$; thus $u$ is injective, hence bijective since E and $E'$ have the same finite dimension.

**Theorem 1** (Witt). — *Let E and $E'$ be two vector spaces of finite dimensions, provided respectively with two non-degenerate $\varepsilon$-hermitian forms $\Phi$ and $\Phi'$ satisfying condition (T) of No. 2* (resp. with two non-degenerate quadratic forms Q and Q'), and isomorphic for these structures. Given an arbitrary subspace F of E, every injective metric homomorphism from F into E' extends to a metric isomorphism from E onto E'.

Using the given isomorphism from E onto E', one sees that it suffices to show that every injective metric homomorphism u from F into E extends to a metric automorphism of E. Let us remark that if, for i = 1, 2, F_i is a subspace of E and u_i a metric homomorphism from F_i into E, such that F_1 ∩ F_2 = {0} and that Φ(u_1(x_1), u_2(x_2)) = Φ(x_1, x_2) for x_i ∈ F_i (i = 1, 2), then the homomorphism ψ : x_1 + x_2 → u_1(x_1) + u_2(x_2) from F_1 + F_2 into E which extends u_1 and u_2 is metric: indeed, whatever x_i, y_i in F_i (i = 1, 2), the expansion of each of the expressions Φ(x_1 + x_2, y_1 + y_2) and Φ(u_1(x_1) + u_2(x_2), u_1(y_1) + u_2(y_2)) (resp. Q(x_1 + x_2) and Q(u_1(x_1) + u_2(x_2))) contains four (resp. three) terms equal each to each according to the assumptions made. Moreover, if u_1 and u_2 are injective and if u_1(F_1) ∩ u_2(F_2) = {0}, then ψ is injective.

1) We first prove the Witt theorem in the case where the set of elements invariant by u is a hyperplane U of F. The set of vectors of the form u(x) − x with x ∈ F is then a right D. If F' is a subspace orthogonal to D such that F' ∩ F = F' ∩ u(F) = {0}, we shall have Φ(u(x), y) = Φ(x, y) for x ∈ F and y ∈ F' ; our initial remark therefore applies to u and to the identical mapping of F' into E, showing that u extends to F + F' by leaving the points of F' fixed; the set of vectors of the form u(x) − x (x ∈ F + F') is still the right D. Now we have, for x ∈ F, y ∈ F

(5) $\Phi(u(x), u(y) - y) = \Phi(u(x), u(y)) - \Phi(u(x), y) = \Phi(x - u(x), y)$,

which, when x ∈ U (that is to say when u(x) = x), shows that x ∈ D^0; in other words we have U ⊂ D^0. We shall distinguish two cases:

a) $F \not\subset D^0$. Formula (5) shows that $u(F)$ is not contained in $D^0$, hence $F \cap D^0 = u(F) \cap D^0 = U$. One may then take for F' a supplementary subspace of U in D^0; since F + F' contains the hyperplane D^0 and is distinct from it, we have F + F' = E, and in this case we have found the required extension of u to E.

b) F ⊂ D^0. Formula (5) shows that u(F) ⊂ D^0, and therefore that

D ⊂ D^0 ; the right D is therefore isotropic (resp. singular, since we have Q(u(x) − x) = Q(u(x)) − Φ(x, u(x)) + Q(x) = 2Q(x) − Φ(x, x) = 0 for x ∈ F). We shall show that, under these conditions, there exists a subspace F' of D^0 which is supplementary to F and u(F) in D^0. This is immediate if F = u(F). Otherwise, let x and y be vectors such that x ∈ F, x ∉ U, y ∈ u(F), y ∉ U; we then have F = U + Ax, u(F) = U + Ay, and F does not contain x + y otherwise y = (x + y) − x would belong to F ∩ u(F) = U; one sees analogously that x + y does not belong to u(F); thus the right A(x + y) is supplementary to F and u(F) in the subspace F + u(F); it suffices then to put F' = A(x + y) + G where G is supplementary to F + u(F) in D^0. This being so, we have F + F' = u(F) + F' = D^0, and, in this case, what was said at the beginning of 1) shows that there exists an extension of u to the hyperplane D^0 of E, and that D^0 is stable for this extension.

We are therefore reduced to the case where F is the hyperplane D^0 and where u is an automorphism of F. We prove that, for every z ∈ E, there exists z' ∈ E such that

(6)
$$
\Phi(u(x), z') = \Phi(x, z)
$$
for every x ∈ F; indeed the linear form x → Φ(u^{-1}(x), z) on F is the restriction of a linear form on E, a form which is of the type x → Φ(x, z') since Φ is non-degenerate; hence (6) holds. Moreover, if z ∉ F, there exists a vector z' ∈ E satisfying (6) and such that Φ(z', z') = Φ(z, z) (resp. Q(z') = Q(z)): indeed formula (6) remains valid if one adds to z' an element u(y) − y (y ∈ F) of D since F = D^0, and Lemma 1 of No. 2 allows one to conclude since z is not orthogonal to D. Our initial remark then shows that there exists a metric homomorphism ϕ from F + Az = E into E which extends u and which transforms z into z'. Since Φ is non-degenerate, ϕ is the required metric automorphism of E.

2) In the general case, we reason by induction on r = dim F. The case r = 0 is trivial. Let then r > 0, that is to say F ≠ {0}, and let U be a hyperplane of F. The restriction u_0 of u to U extends, by the induction hypothesis, to a metric automorphism ϕ_0 of E. If ϕ_0 extends u, the theorem is proved. Otherwise U is the set of elements invariant by v_0^{-1}u, and there exists, according to 1), a metric automorphism v_1 of E extending v_0^{-1}u. The automorphism v_0v_1 is then the required extension of u. QED.

#### Corollary 1 {#alg-ix-s4-prop-4-cor-1 .statement}

Let, for i = 1, 2, E_i be a finite-dimensional vector space, Φ_i a non-degenerate ε-hermitian form on E_i satisfying (T) (resp. Q_i a non-degenerate quadratic form on E_i), E'_i and E''_i two orthogonal subspaces of E_i whose direct sum is E_i. If the forms Φ_1 and Φ_2 (resp. Q_1 and Q_2) are equivalent, and if their restrictions to E'_1 and E'_2 are equivalent, the same is true of their restrictions to E''_1 and E''_2.

Indeed, let u be a metric isomorphism of E'_1 onto E'_2. By Theorem 1, u extends to a metric isomorphism ϕ of E_1 onto E_2. Since Φ_i is non-degenerate, E''_i is the orthogonal of E'_i in E_i, hence ϕ maps E''_1 onto E''_2. QED.

#### Corollary 2 {#alg-ix-s4-prop-4-cor-2 .statement}

The hypotheses being those of Theorem 1, the group of metric automorphisms of E permutes transitively the totally isotropic (resp. totally singular) subspaces of given dimension of E. Moreover, if F is a totally isotropic (resp. totally singular) subspace of E, every bijective linear mapping of F onto F is induced by a metric automorphism of E.

#### Corollary 3 {#alg-ix-s4-prop-4-cor-3 .statement}

Let Q be a non-degenerate quadratic form on a finite-dimensional vector space E over an algebraically closed field A. The group of metric automorphisms of E permutes transitively the non-isotropic subspaces of given dimension of E.

This follows immediately from Theorem 1 and Corollary 2 of Proposition 3.

Exercises. — 1) a) Let K be a field of characteristic 2, J : ξ → ¯ξ an involutory antiautomorphism of K, Z the center of K. Show that if the restriction of J to Z is not the identity, every element μ of K such that ¯μ = μ is of the form λ + ¯λ (observe that there is an element ρ ≠ 0 in Z which can be written in the form ζ + ¯ζ, with ζ ∈ Z); every hermitian form on a vector space over K then satisfies condition (T).

b) Give examples of fields of characteristic 2, admitting an involutory antiautomorphism ξ → ¯ξ distinct from the identity map, and for which there are elements $\mu = \bar{\mu}$ which are not of the form $\lambda + \bar{\lambda}$ (cf. Chapter VIII, § 11, Exercise 4).

2) Let A be a field, E a vector space over A, $\Phi$ (resp. Q) a non-degenerate $\varepsilon$-hermitian form on E, satisfying condition (T) (resp. a non-degenerate quadratic form on E, Φ then denoting the symmetric bilinear form associated with Q).

a) Show that in order that a plane P \subset E be isotropic (resp. singular) and not totally isotropic (resp. not totally singular), it is necessary and sufficient that it contain only one isotropic (resp. singular) right (cf. Exercise 14 e)).

b) Suppose that dim $E \geqslant 3$, and that there exist in E isotropic vectors $\neq 0$. Show that if P is a non-totally isotropic plane in E, there exists a non-isotropic vector subspace V \subset E, of dimension 3, containing isotropic vectors $\neq 0$, and such that $P \subset V$.

3) The hypotheses being the same as in Exercise 2, show that if dim $E \geqslant 3$, every isotropic right in E is the intersection of two non-isotropic planes.

4) The hypotheses are those of Exercise 2, and suppose in addition that E is finite-dimensional.

a) If the index $\nu$ of $\Phi$ (resp. Q) is $\geqslant 1$, show that for every isotropic (resp. singular) vector $a \neq 0$ in E, there exists a basis $(e_i)$ of E consisting of isotropic (resp. singular) vectors, such that $e_1 = a$ (cf. Exercise 14 e)).

b) Let V, W be two totally isotropic (resp. totally singular) subspaces of the same dimension $r \leqslant \nu$; show that there exist two maximal totally isotropic (resp. totally singular) subspaces V_1, W_1, such that V \subset V_1, W \subset W_1, and $V_1 \cap W_1 = V \cap W$. (If $U = V \cap W$, reason in $U^0/U$).

c) Let V, W, $V_1, W_1$ be four totally isotropic (resp. totally singular) subspaces of the same dimension, such that $V + W$ and $V_1 + W_1$ are non-isotropic. Show that there exists a metric automorphism $u$ of E such that $u(V) = V_1$ and $u(W) = W_1$.

d) Let $f$ be a linear form on E, $\alpha$ an element of A of the form $\lambda + \varepsilon \bar{\lambda}$ (resp. an element of $\Lambda$). Consider the sesquilinear form on E

$$
(x, y) \to \Phi_1(x, y) = \Phi(x, y) + f(x)\overline{\alpha f(y)}
$$

(resp. the quadratic form

$$
x \to Q_1(x) = Q(x) + \alpha(f(x))^2).
$$

Show that if $\Phi_1$ (resp. $Q_1$) is non-degenerate and if $\nu_1$ denotes its index, one has $|\nu_1 - \nu| \leqslant 1$.

5) a) Let B be a ring, $\xi \to \bar{\xi}$ an involutory antiautomorphism of B, $\varepsilon$ an element of the center of B such that $\varepsilon \bar{\varepsilon} = 1$. Show that if $\beta$ is an invertible element of B such that $\beta + \varepsilon \bar{\beta} \neq 0$, there exists an invertible element $\mu \neq 1$ in B, such that $\mu(\beta + \varepsilon \bar{\beta})\mu = \beta + \varepsilon \bar{\beta}$. (Show that one can take $\mu$ such that $\mu \beta \bar{\mu} = \beta$).

b) Let A be a field, E a vector space over A, $\Phi$ a non-degenerate $\varepsilon$-hermitian sesquilinear form on E, satisfying (T). Show that if $\Phi$ is not alternating, for every non-isotropic hyperplane $H$ of E, there exists a metric automorphism of E, distinct from the identity, leaving every element of $H$ invariant (use a).

6) The hypotheses being those of Exercise 2, let $a$ be an isotropic vector $\neq 0$ in $E$ (resp. a nonsingular isotropic vector (note that such vectors exist only if $A$ is of characteristic 2)). Let $\lambda \in A$ such that $\lambda + \varepsilon \bar{\lambda} = 0$ (resp. $\lambda = (Q(a))^{-1}$); show that the transvection $x \to x + \Phi(x, a)\lambda a$ (Chapter II, § 6, Exercise 7) is a metric automorphism of $E$; converse.

7) The hypotheses being those of Exercise 2, let $G$ be the group of metric automorphisms of $E$. Show that the only semilinear bijections of $E$ onto itself which commute with all the elements of $G$ are the homotheties of $E$, except in the following three cases: dim $E = 2$, $G$ is the group of metric automorphisms corresponding to a quadratic form of index 1 on $E$, and $A$ is one of the three fields $\mathbf{F}_2, \mathbf{F}_3$ or $\mathbf{F}_4$. (Use Exercises 5, 6 and 3; examine separately the case of a quadratic form on a vector space of dimension 2).

*8) Let $A$ be a field, $E$ a finite-dimensional vector space $> 0$ over $A$, $\Phi$ a non-degenerate $\varepsilon$-hermitian sesquilinear form on $E$, satisfying (T). Let $M(\Phi)$ be the group of multipliers of the similarities of $E$ for $\Phi$ ($\S 6, \mathrm{n}^o\ 5$).

a) Let $V_1, V_2$ be two vector subspaces of $E$, of the same dimension, and let $\Phi_1, \Phi_2$ be the restrictions of $\Phi$ to $V_1, V_2$ respectively. For there to exist a similarity $u$ such that $u(V_1) = V_2$, it is necessary and sufficient that there exist $\alpha \in M(\Phi)$ such that $\Phi_2$ is equivalent to $\alpha \Phi_1$ (use Witt's theorem).

b) Let $(F, F', G)$ be a Witt decomposition of $E$ ($\mathrm{n}^o\ 2$), and let $\Phi_0$ be the restriction of $\Phi$ to the non-isotropic subspace $G$. Show that $M(\Phi) = M(\Phi_0)$ if $G \neq \{0\}$. (Use Witt's theorem and Proposition 2 of $\mathrm{n}^o\ 2$).

c) Now prove that if the index $v$ of $\Phi$ is such that dim $E = 2v$, $M(\Phi)$ is the group of elements $\zeta \neq 0$ of the center of $A$ such that $\bar{\zeta} = \zeta$. If dim $E = 2v + 1$, $M(\Phi)$ is the group of elements of the form $\rho \bar{\rho}$, where $\rho$ runs through the multiplicative group of the elements $\neq 0$ of the center of $A$ (use Witt's theorem). (Cf. § 10, exerc. 18).*

*9) Let $A$ be a commutative field, $E$ a vector space over $A$, $Q$ a non-degenerate quadratic form on $E$. A similarity for $Q$ is any automorphism $u$ of $E$ such that there exists an element $\alpha \neq 0$ of $A$ for which $Q(u(x)) = \alpha Q(x)$ for all $x \in E$; $u$ is then also a similarity for the bilinear form associated with $Q$. Assuming the dimension of $E$ to be finite and $> 0$, state and exercise prove, for the similarities relative to $Q$, the analogues of the results of exerc. 8.*

*10) Let $A$ be a field, $E$ a vector space over $A$ of dimension $> 2$, $\Phi_1$ (resp. $\Phi_2$) a non-degenerate sesquilinear form $\varepsilon_1$-hermitian (resp. $\varepsilon_2$-hermitian) on $E$ for an involutory antiautomorphism $J_1$ (resp. $J_2$) of $A$, satisfying condition (T). Now prove that if the group of metric automorphisms of $E$ for $\Phi_1$ is a subgroup of the group of similarities for $\Phi_2$, there exists $\alpha \in A$ such that $\Phi_2 = \Phi_1 \alpha$ (use exerc. 5 b) and 6).

Exercise prove the analogous property when A is assumed commutative, and when $\Phi_1$ and $\Phi_2$ are replaced in the statement by two non-degenerate quadratic forms $Q_1, Q_2$ on E.*

11) Let A be a ring, J an involutory antiautomorphism of A, E an A-module admitting a finite basis $(e_i)$, $\Phi$ a non-degenerate $\varepsilon$-hermitian form on E, R the matrix of $\Phi$ with respect to $(e_i)$; the group of metric automorphisms of $\Phi$ is identified with the group G of invertible matrices U such that $^tU . R . U^j = R$.

a) Suppose that there exists a matrix P such that $R = ^tP + \varepsilon P^j$. Now prove that for every matrix S such that $^tS + \varepsilon S^j = 0$, and such that $P + S$ is invertible, $U = (^tP^j - \varepsilon^j S)^{-1}(P + S)$ belongs to G, and $\varepsilon I + U$ is invertible. Conversely (show that for every matrix $U \in G$ such that $\varepsilon I + U$ is invertible, we have

$$
\varepsilon(\varepsilon I + ^tU)^{-1}R + \varepsilon^j R (\varepsilon^j I + U^j)^{-1} = R.
$$

b) Show that the condition in a) is satisfied when $\Phi$ satisfies condition (T). Case where in A the equation $2\xi = \alpha$ has one and only one solution for every $\alpha \in A$.

¶ 12) Let A be a commutative field, E a finite-dimensional vector space of dimension n over A, $\Phi$ a nondegenerate $\varepsilon$-Hermitian sesquilinear form on E.

a) Let u be an endomorphism of E; show that if the $r_i (1 \leq i \leq m)$ are the similarity invariants of u (Chapter VII, § 5, No. 1, Def. 1), the similarity invariants of the adjoint $u^*$ of u with respect to $\Phi$ are the polynomials $\bar{r}_i (1 \leq i \leq m)$, where $\bar{r}_i$ is obtained from $r_i$ by applying the automorphism J to each coefficient (cf. Chapter VII, § 5, exerc. 2). For every monic irreducible polynomial $p \in A[X]$ dividing the minimal polynomial of u, let $F_k(u, p)$ be the kernel of $(p(u))^k$ in E, and let $F(u, p)$ be the union of the $F_k(u, p)$ for all integers $k > 0$. Show that if p and q are distinct monic irreducible polynomials dividing the minimal polynomial of u, the subspaces $F(u, p)$ and $F(u^*, \bar{q})$ are orthogonal (use Bezout's identity). Finally, if G is a vector subspace of E such that $u(G) \subset G$, we have $u^*(G^0) \subset G^0$.

b) Suppose that $uu^* = u^*u$ (the case where u is said to be a normal endomorphism for $\Phi$; cf. § 7, No. 3); show that we then have $u^*(F_k(u, p)) \subset F_k(u, p)$ for every k, and consequently $u^*(F(u, p)) \subset F(u, p)$. If we put $G(p, \bar{q}) = F(u, p) \cap F(u^*, \bar{q})$, show that E is the direct sum of the subspaces $G(p, \bar{q})$, and that $G(p, \bar{q})$ and $G(p_1, \bar{q}_1)$ are orthogonal if $p \neq q_1$ or if $p_1 \neq q$; in particular $G(p, \bar{q})$ is totally isotropic if $p \neq q$. Show that $G(p, \bar{p})$ is reduced to 0 or is nonisotropic, and that if $p \neq q$, no nonzero vector of $G(p, \bar{q})$ is orthogonal to $G(q, \bar{p})$ (use the fact that $\Phi$ is nondegenerate); deduce that if $p \neq q$, $G(p, \bar{q})$ and $G(q, \bar{p})$ are totally isotropic subspaces of the same dimension, and that $G(p, \bar{q}) + G(q, \bar{p})$ is nonisotropic.

c) Suppose that $J$ is not the identity or that $A$ is not of characteristic 2, and that $u^* = u$. Let $\mathcal{M}$ be the set of non-isotropic subspaces $M \subset G(p, \bar{p})$, stable under $u$ (hence submodules of the $A[X]$-module $E_u$ (Chapter VII, § 5, No. 1)). Now prove that if $M$ is a minimal element of $\mathfrak{M}$, $M$ is an *indecomposable* submodule of $E_u$ (Chapter VII, § 4, No. 7). (Suppose that $M$ is the direct sum of an indecomposable submodule $M_1$ and a submodule $M_2 \neq \{0\}$, the minimal polynomials $p^h$ and $p^k$ of the restrictions of $u$ to $M_1$ and $M_2$ respectively being such that $h \geq k$. Observe then that $M_1$ is necessarily isotropic and that every $z \neq 0$ in $M_1$ such that $p(u).z = 0$ is orthogonal to $M_1$ (use the fact that every submodule of $M_1$ is monogenic); write $z = (p(u))^{h-1}.x$ and that $z$ is not orthogonal to $M_2$, and deduce that necessarily $k = h$. Now prove that there exists an indecomposable submodule $N_2$ of $M_2$ such that $p^h$ is the minimal polynomial of the restriction of $u$ to $N_2$, and that $M_1 + N_2$ is non-isotropic; conclude that $M_2 = N_2$. Finally, if $y \in M_2$ is not orthogonal to $z$, consider the submodule $P$ of $M$ generated by $w = x + \lambda y$, where $\lambda \in \mathbf{A}$, and prove that $\lambda$ can be chosen so that $P$ is non-isotropic, by proving that $\Phi((p(u))^{h-1}.w, w) \neq 0$; which leads to a contradiction).

d) Deduce from c) that $G(p, \overline{p})$ is the direct sum of pairwise orthogonal indecomposable submodules $H_i$. If $p^h$ is the minimal polynomial of the restriction of $u$ to $H_i$, and if $d$ is the degree of $p$, prove that there exists in $H_i$ a totally isotropic subspace of dimension $d.[h/2]$. Case where $E$ contains no isotropic vector $\neq 0$ (cf. § 7, No. 3).

e) State and prove the analogous properties to those of c) and d) when $u^* = -u$ or $u^*u = 1$.

f) Give an example where $n = 4$, $\Phi$ is symmetric and of index 2, $p = \overline{p} = X - 1$, $u$ is normal, $E = G(p, \overline{p})$, but $E$ is not the direct sum of minimal submodules of $\mathfrak{M}$, and where there exists an eigenvector of $u$ which is not an eigenvector of $u^*$ (cf. § 7, No. 3).

13) The hypotheses are those of Exercise 2, and suppose in addition that $E$ admits a countable basis $(e_n)$. Let $F$ be a totally isotropic (resp. totally singular) subspace of $E$ such that $F^{00} = F$; now prove that there exists a totally isotropic (resp. totally singular) subspace $F'$ such that: $1^\circ \ F \cap F' = \{0\}$; $2^\circ$ there exists a basis $(a_m)_{m \in I}$ of $F$ and a basis $(a'_m)_{m \in I}$ of $F'$ (the interval of $\mathbf{N}$ with origin 0) such that $\Phi(a_i, a'_j) = \delta_{ij}$ for every pair of indices; $3^\circ$ $(F + F')^{00} = F + F'$ and $E$ is the direct sum of $F + F'$ and $G = (F + F')^0$. (Form by induction an increasing sequence $(L_n)$ of non-isotropic subspaces, whose union is $E$, such that $\dim L_{n+1} - \dim L_n = 2$, and apply Proposition 2 of No. 2 to each of the $L_n$; to form this sequence, consider, for each $n$, the smallest integer $k$ such that $e_k \notin L_n$, and use Exercise 9 b) of § 1).

14) Let $A$ be a field of characteristic 2, $E$ a finite-dimensional vector space of dimension $n$ over $A$, $\Phi$ a non-degenerate hermitian form on $E$, not necessarily satisfying condition (T).

a) Show that the set $V$ of the $x \in E$ such that $\Phi(x, x)$ is of the form $\alpha + \overline{\alpha}$ is a vector subspace of $E$.

b) Let $V_1 = V \cap V^0$, $q = \dim V_1$, $V_2$ a supplementary space to $V_1$ with respect to $V$, $V_3$ a supplementary space to $V_1$ with respect to $V^0$. Now prove that there exists a base $(e_i)_{1 \leq i \leq 2q}$ of $(V_2 + V_3)^0 = V_2^0 \cap V_3^0$ such that the vectors $e_1, \ldots, e_q$ form a base of $V_1$ and that $\Phi(e_i, e_{q+j}) = \delta_{ij}$ for $1 \leq i \leq q, 1 \leq j \leq q$.

c) Let $G(\Phi)$ be the group of metric automorphisms of $E$ (for $\Phi$). Now prove that for every $u \in G(\Phi)$, we have $u(x) = x$ for every $x \in V^0$.

d) For every $u \in G(\Phi)$, we have $u(V) = V$; let $u_v$ be the restriction of $u$ to $V$, and let $G_v$ be the group formed by the $u_v$. Now prove that: $1^o$ the kernel of the homomorphism $u \to u_v$ from $G(\Phi)$ onto $G_v$ is commutative; $2^o$ if $\Phi_2$ is the restriction of $\Phi$ to $V_2$ and $G(\Phi_2)$ the group of metric automorphisms of $V_2$ for $\Phi_2$, there exists a homomorphism from $G_v$ onto $G(\Phi_2)$ whose kernel is commutative (use $b$ and $c$).

e) Suppose that $A$ is commutative and $J$ is the identity; let $E$ be a vector space of dimension 3 over $A$, $(e_i)_{1 \leq i \leq 3}$ a base of $E$, $\Phi$ the non-degenerate symmetric form on $E$ whose matrix with respect to $(e_i)$ is

$$
\begin{pmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0
\end{pmatrix}.
$$

Show that all isotropic vectors in $E$ are contained in the hyperplane generated by $e_2$ and $e_3$ (cf. exerc. 4 a)). Give an example of a non-isotropic plane containing only one isotropic right (cf. exerc. 2 a)). Show that there is no automorphism $u \in G(\Phi)$ such that $u(e_1) = e_1 + e_2$, though we have $\Phi(e_1, e_1) = \Phi(e_1 + e_2, e_1 + e_2)$.
