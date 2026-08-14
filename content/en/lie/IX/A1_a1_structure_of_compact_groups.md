---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Structure of compact groups
appendix: true
lang: en
source: lie-vii-ix
book_pages: A IX.381-A IX.385, A IX.424-A IX.425
pdf_pages: 0388-0392, 0431-0432
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING A COMPACT GROUP IN A PRODUCT OF LIE GROUPS
      page: 381
      pdf_page: 388
    - "no": 2
      title: PROJECTIVE LIMITS OF LIE GROUPS
      page: 382
      pdf_page: 389
    - "no": 3
      title: STRUCTURE OF CONNECTED COMPACT GROUPS
      page: 384
      pdf_page: 391
statements: 9
exercises: 1
content_sha256: 41872eb014d688a41d6d3ba05be1302df46947f174e42f3298da768560d2a8da
---

## APPENDIX I

# STRUCTURE OF COMPACT GROUPS

### 1. EMBEDDING A COMPACT GROUP IN A PRODUCT OF LIE GROUPS

#### Proposition 1 {#lie-ix-a1-prop-1 .statement tag=01II}

Every compact topological group G is isomorphic to a closed subgroup of a product of compact Lie groups.

Denote by $\widehat{G}$ the set of classes of irreducible continuous unitary representations of G on finite dimensional complex Hilbert spaces (Spectral Theory, in preparation). For all $u\in \widehat{G}$, let $Hu$ be the space of $u$ and $\rho_u: G\rightarrow \mathbf{U}(H_u)$ the homomorphism associated to $u$. By the Peter-Weyl theorem (Spectral Theory, in preparation), the continuous homomorphism $\rho = (\rho_u)_{u\in\widehat{G}}$ from G to $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$ is injective; since G is compact, $\rho$ induces an isomorphism

from G onto a closed subgroup of the group $\prod_{u\in\widehat{G}}\mathbf{U}(H_u)$.

#### Corollary 1 {#lie-ix-a1-prop-1-cor-1 .statement tag=01IJ}

Let V be a neighbourhood of the identity element of G. Then V contains a closed normal subgroup H of G such that the quotient $G/H$ is a Lie group.

Let $(K_{\lambda})_{\lambda\in L}$ be a family of compact Lie groups such that G can be identified with a closed subgroup of $\prod_{\lambda\in L}K_{\lambda}$; for $\lambda \in L$, demote by $p_{\lambda}: G\rightarrow K_{\lambda}$ the restriction to G of the canonical projection. There exists a finite subset $J\subset L$, and for each $\lambda \in J$ a neighbourhood $V_{\lambda}$ of the origin in $K_{\lambda}$, such that V contains $\bigcap_{\lambda\in J}p^{-1}_{\lambda}(V_{\lambda})$. It now suffices to put $H =\bigcap_{\lambda\in J}$ Ker($p_{\lambda}$).

Denote by $(H_{\alpha})_{\alpha\in I}$ the decreasing filtered family of closed normal subgroups of G, such that the quotient $G/H_{\alpha}$ is a Lie group. Consider the projective system of compact Lie groups $G/H_{\alpha}$ (cf. General Topology, Chap. III, §7, no. 2, Prop. 2).

#### Corollary 2 {#lie-ix-a1-prop-1-cor-2 .statement tag=01IK}

The canonical map $G\rightarrow$ lim$_{_{\leftarrow -}}G/H_{\alpha}$ is an isomorphism of topological groups. $\alpha$

Indeed, Cor. 1 implies that condition (PA) of General Topology, Chap. III, §7, no. 2, is satisfied; the assertion now follows from Prop. 2 of loc. cit.

#### Corollary 3 {#lie-ix-a1-prop-1-cor-3 .statement tag=01IL}

G is a Lie group if and only if there exists a neighbourhood of the identity element $e$ of G that contains no normal subgroup distinct from $\{e\}$.

The necessity of this condition has already been proved (Chap. III, §4, no. 2, Cor. 1 of Th. 2), and the sufficiency is an immediate consequence of Cor. 1.

### 2. PROJECTIVE LIMITS OF LIE GROUPS

#### Lemma 1 {#lie-ix-a1-lem-1 .statement tag=01IM}

Let $(G_{\alpha}, f_{\alpha \beta})$ be a projective system of topological groups relative to a filtered index set I, and G its limit. Assume that the canonical maps $f_{\alpha}: G\rightarrow G_{\alpha}$ are surjective.

a) The subgroups $D(G_{\alpha})$ (resp. $C(G_{\alpha})$, resp. $C(G_{\alpha})_0)$ form a projective system of subsets of $G_{\alpha}$.

b) We have D(G) = lim$_{_{\leftarrow -}}\overline{D(G_{\alpha})}$ and C(G) = lim$_{_{\leftarrow -}}C(G_{\alpha})$.

$\alpha \alpha$

c) If $G_{\alpha}$ is compact for all $\alpha \in I$, then $C(G)_0=$ lim$_{_{\leftarrow -}}C(G_{\alpha})_0$.

$\alpha$

Let $\alpha , \beta$ be two elements of I, with $\alpha \leq \beta$. Then $f_{\alpha \beta}(D(G_{\beta}))\subset D(G_{\alpha})$, and $f_{\alpha \beta}(C(G_{\beta}))\subset C(G_{\alpha})$ since $f_{\alpha \beta}$ is surjective; since $f_{\alpha \beta}$ is continuous, it follows that $f_{\alpha \beta}(D(G_{\beta}))\subset D(G_{\alpha})$ and $f_{\alpha \beta}(C(G_{\beta})_0)\subset C(G_{\alpha})_0$, hence $a)$. Since $f_{\alpha}$ is surjective, $f_{\alpha}(D(G)) = D(G_{\alpha}) ($Algebra, Chap. I, §6, no. 2, Prop. 6), so D(G) = lim$_{\leftarrow -}D(G_{\alpha}) ($General Topology, Chap. I, §4, no. 4, Cor. of Prop. 9). The surjectivity of $f_{\alpha}$ also implies the inclusion $f_{\alpha}(C(G))\subset$ $C(G_{\alpha})$ and hence $C(G)\subset$ lim$_{\leftarrow -}C(G_{\alpha})$; the opposite inclusion is immediate. Finally, assertion $c)$ follows from $b)$ and General Topology, Chap. III, §7, no. 2, Prop. 4).

#### Lemma 2 {#lie-ix-a1-lem-2 .statement tag=01IN}

Let $(S_a)_{a\in A},(T_b)_{b\in B}$ be two finite families of almost simple, simply-connected Lie groups (Chap. III, § 9, no. 8, Def. 3)$,u:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ a surjective morphism. Then there exist an injective map $l: B\rightarrow A$ and isomorphisms $u_b: S_{l(b)}\rightarrow T_b(b\in B)$ such that $u((s_a)_{a\in A}) = (u_b(s_{l(b)}))_{b\in B}$ for every element $(s_a)_{a\in A}$ of $\prod_{a\in A}S_a$.

Denote by $\mathfrak{s}_a$ (resp. $\mathfrak{t}_b)$ the Lie algebra of $S_a$ (resp. $T_b)$ for $a\in A$ (resp. $b\in B)$, and consider the homomorphism $L(u) :\prod_{a\in A}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$. Its kernel

is an ideal of the semi-simple Lie algebra $\prod_{a\in A}\mathfrak{s}_a$, and hence is of the form $\prod_{a\in A''}\mathfrak{s}_a$, with $A''\subset A$ (Chap. I, §6, no. 2, Cor. 1). Put $A'= A$**--** $A''$. By

restriction, $L(u)$ induces an isomorphism $f:\prod_{a\in A'}\mathfrak{s}_a\rightarrow \prod_{b\in B}\mathfrak{t}_b$. By loc. cit., for all $a\in A'$ the ideal $f(\mathfrak{s}_a)$ is equal to one of the $\mathfrak{t}_b$; hence, there exists a bijection $l: B\rightarrow A'$ such that $f(\mathfrak{s}_{l(b)}) =\mathfrak{t}_b$ for $b\in B$, and $f$ induces an isomorphism $f_b:\mathfrak{s}_{l(b)}\rightarrow \mathfrak{t}_b$. Since the groups $S_a$ and $T_b$ are simply-connected, there exist isomorphisms $u_b: S_{l(b)}\rightarrow T_b$ such that $L(u_b) =f_b$ for $b\in B$ (Chap. III, §6, no. 3, Th. 3).

Denote by $\widetilde{u}:\prod_{a\in A}S_a\rightarrow \prod_{b\in B}T_b$ the morphism defined by $\widetilde{u}((s_a)_{a\in A}) =$

$(u_b(s_{l(b)}))_{b\in B}$. By construction, $L(\widetilde{u}) =f= L(u)$, so $\widetilde{u}=u$, which proves the lemma.

#### Lemma 3 {#lie-ix-a1-lem-3 .statement tag=01IO}

Under the hypotheses of Lemma 1, assume that the $G_{\alpha}$ are simply-connected compact Lie groups. Then, the topological group G is isomorphic to the product of a family of almost simple, simply-connected compact Lie groups.

For all $\alpha \in I$, the group $G_{\alpha}$ is the direct product of a finite family of almost simple, simply-connected subgroups $(S^{\lambda}_{\alpha})_{\lambda\in L_{\alpha}}$ (Chap. III, §9, no. 8, Prop. 28). Let $\beta \in I,\beta \geq \alpha$. By Lemma 2, there exists a map $l_{\beta \alpha}: L_{\alpha}\rightarrow L_{\beta}$ such that $f_{\alpha \beta}(S^l_{\beta^{\beta \alpha}}^{(\lambda)}) = S^{\lambda}_{\alpha}$ for $\lambda \in L_{\alpha}$. We have $l_{\gamma \beta}\circ l_{\beta \alpha}=l_{\gamma \alpha}$ for $\alpha \leq \beta \leq \gamma$, so $(L_{\alpha}, l_{\beta \alpha})$ is an inductive system of sets relative to I. Let L be its limit; the maps $l_{\beta \alpha}$ being injective, $L_{\alpha}$ can be identified with a subset of L, so that $L =\bigcup_{\alpha\in I}L_{\alpha}$.

Let $\lambda \in L$. Put $S^{\lambda}_{\alpha}=\{1\}$ when $\lambda  /\in L_{\alpha}$, and denote by $\varphi^{\lambda}_{\alpha \beta}: S^{\lambda}_{\beta}\rightarrow S^{\lambda}_{\alpha}$ the morphism induced by $f_{\alpha \beta}$; this gives a projective system of topological groups $(S^{\lambda}_{\alpha}, \varphi^{\lambda}_{\alpha \beta})$, whose limit is isomorphic to $S_{\lambda}$. The canonical homomorphism of topological groups

lim$_{_{\leftarrow -\alpha\in I}}((\prod_{\lambda\in L}S^{\lambda}_{\alpha})\rightarrow \prod_{\lambda\in L}($lim$_{_{\alpha\leftarrow -\in I}}S^{\lambda}_{\alpha})$

is bijective (Theory of Sets, Chap. III, §7, no. 3, Cor. 2); it is thus an isomorphism since the groups in question are compact. But the first of these groups can be identified with G and the second with the product of the $S_{\lambda}$, hence the lemma.

### 3. STRUCTURE OF CONNECTED COMPACT GROUPS

Let G be a commutative compact group. Recall (Spectral Theory, Chap. II, §1, no. 9, Prop. 11) that G is then isomorphic to the dual topological group of a discrete commutative group $\widehat{G}$. The group G is connected if and only if $\widehat{G}$ is torsion-free (Spectral Theory, Chap. II, §2, no. 2, Cor. 1 of Prop. 4).

The following properties are equivalent (Spectral Theory, Chap. II, §2, no. 2, Cor. 2 of Prop. 4 and §1, no. 9, Cor. 2 of Prop. 11):

(i) G is totally discontinuous;

(ii) $\widehat{G}$ is a torsion group;

(iii) the topological group G is isomorphic to the limit of a projective system of finite (commutative) groups, each having the discrete topology.

The proposition below generalizes Cor. 1 of Prop. 4 of §1, no. 4.

#### Proposition 2 {#lie-ix-a1-prop-2 .statement tag=01IP}

Let G be a connected compact group.

a$) C(G)_0$ is a commutative connected compact group; D(G) is a connected compact group, equal to its derived group.

b) The continuous homomorphism $(x, y) \rightarrow xy$ from $C(G)_0\times D(G)$ to G is surjective and its kernel is a central subgroup of $C(G)_0\times D(G)$ that is compact and totally discontinuous.

c) There exists a family $(S_{\lambda})_{\lambda\in L}$ of almost simple compact Lie groups and a surjective continuous homomorphism $\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$, whose kernel is a

totally discontinuous, compact, central subgroup.

Let $(G_{\alpha}, f_{\alpha \beta})$ be a projective system of compact Lie groups, relative to a filtered set I, such that G is isomorphic to lim $G_{\alpha}$ and such that the canonical maps $f_{\alpha}: G\rightarrow G_{\alpha}$ are surjective (Cor. 2 of Prop. 1). For$^{\leftarrow -}\alpha \in I$, let $\pi_{\alpha}: \widetilde{D}(G_{\alpha})\rightarrow D(G_{\alpha})$ be a universal covering of the group $D(G_{\alpha})$. The $f_{\alpha \beta}$ induce morphisms $\widetilde{f}_{\alpha \beta}: \widetilde{D}(G_{\beta})\rightarrow \widetilde{D}(G_{\alpha})$, and $( \widetilde{D}(G_{\alpha}),\widetilde{f}_{\alpha \beta})$ is a projective system of topological groups satisfying the hypotheses of Lemma 3.

It follows from this lemma that the topological group lim $\widetilde{D}(G$ ) is iso-

$\leftarrow -\alpha$

morphic to the product of a family $(S_{\lambda})_{\lambda\in L}$ of almost simple compact Lie groups. By Lemma 1, the limit of the projective system of homomorphisms $(\pi_{\alpha})$ can be identified with a continuous homomorphism $\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$, which is surjective (General Topology, Chap. I, §9, no. 6, Cor. 2 of Prop. 8).

Now observe that the group $\prod_{\lambda\in L}S_{\lambda}$ is equal to its derived group: this follows from §4, no. 5, Cor. of Prop. 10. The same is true for D(G), since $\pi$ is surjective. Consequently, $D(G)\supset D(D(G)) = D(G)$. Thus, the group D(G) is compact and equal to its derived group; this proves $a)$, since the assertions concerning $C(G)_0$ are trivial.

On the other hand, the kernel of $\pi :\prod_{\lambda\in L}S_{\lambda}\rightarrow D(G)$ can be identified with lim$_{\leftarrow -}$ Ker($\pi_{\alpha}$) $($Algebra, Chap. II, §6, no. 1, Remark 1), and thus with a compact, totally discontinuous, central subgroup, hence $c)$.

We prove $b)$. For all $\alpha$ in I, the morphism $s_{\alpha}: C(G_{\alpha})_0\times D(G_{\alpha})\rightarrow G_{\alpha}$ such that $s_{\alpha}(x, y) =xy$ for $x\in C(G_{\alpha})_0, y\in D(G_{\alpha})$, is surjective and its kernel is a finite central subgroup (§1, no. 4, Cor. 1 of Prop. 4). The $s_{\alpha}$ form a projective system of maps, whose limit can, by the preceding, be identified with the homomorphism $(x, y) \rightarrow xy$ from $C(G)_0\times D(G)$ to G. We now see as before that this map is surjective and that its kernel is central and totally discontinuous, hence $b)$.

#### Corollary {#lie-ix-a1-n3-cor-1 .statement tag=01IQ}

Every solvable connected compact group is commutative.

Indeed, the derived group is then solvable and equal to its derived group (Prop. $2a))$, hence reduced to the identity element.

### Exercises {#lie-ix-a1-exercises}

See the [exercises for Appendix 1](exercises/a1/).
