---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Compact Lie algebras
lang: en
source: lie-vii-ix
book_pages: A IX.281-A IX.287, A IX.389-A IX.391
pdf_pages: 0288-0294, 0396-0398
extraction: native
subsections:
    - "no": 1
      title: INVARIANT HERMITIAN FORMS
      page: 281
      pdf_page: 288
    - "no": 2
      title: CONNECTED COMMUTATIVE REAL LIE GROUPS
      page: 282
      pdf_page: 289
    - "no": 3
      title: COMPACT LIE ALGEBRAS
      page: 283
      pdf_page: 290
    - "no": 4
      title: GROUPS WHOSE LIE ALGEBRA IS COMPACT
      page: 284
      pdf_page: 291
statements: 13
exercises: 9
content_sha256: a0ea6ff66efb6fd732a160af583d309a29e61483daaa1bf8d67281c2bb6279df
---

## § 1. COMPACT LIE ALGEBRAS

### 1. INVARIANT HERMITIAN FORMS

In this number, the letter $k$ denotes the field $\mathbf{R}$ or $\mathbf{C}$. Let V be a finite dimensional $k$-vector space, $\Phi$ a separating$^2$ positive hermitian form on V, G a group, $\mathfrak{g}$ an $\mathbf{R}$-Lie algebra, $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ a group homomorphism, $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ a homomorphism of $\mathbf{R}$-Lie algebras.

$a)$ The form $\Phi$ is invariant under G (resp. $\mathfrak{g})$ if and only if $\rho (g)$ is unitary with respect to $\Phi$ for all $g\in G$ (resp. $\varphi (x)$ is anti-hermitian$^3$ with respect to $\Phi$ for all $x\in \mathfrak{g})$. Indeed, denote by $a^*$ the adjoint of an endomorphism $a$ of V with respect to $\Phi$; for $g$ in $G,x$ in $\mathfrak{g},u$ and $v$ in V, we have

$$
\Phi (\rho (g)u, \rho (g)v) =\Phi (\rho (g)^*\rho (g)u, v)
$$

$$
\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) =\Phi ((\varphi (x) +\varphi (x)^*).u, v)
$$

$^1$ Throughout this chapter, references to Algebra, Chap. VIII, are to the new edition

(in preparation)

$^2$ Recall (Algebra, Chap. IX, in preparation) that a hermitian form H on V is said

to be separating (or non-degenerate) if, for every non-zero element $u$ of V, there

exists $v\in V$ such that $H(u, v)\not= 0$.

$^3$ An element $a\in$ End(V) is said to be anti-hermitian with respect to $\Phi$ if the

adjoint $a^*$ of $a$ with respect to $\Phi$ is equal to $-a$. When $k=\mathbf{C}$ (resp. $k=\mathbf{R})$ this

also means that the endomorphism $ia$ of V (resp. of $\mathbf{C}\otimes_{\mathbf{R}}V)$ is hermitian. thus, $\Phi (\rho (g)u, \rho (g)v) =\Phi (u, v)$ for all $u, v$ in V if and only if $\rho (g)^*\rho (g) =$ Id$_V$; similarly, $\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) = 0$ for all $u, v$ in V if and only if $\varphi (x) +\varphi (x)^*= 0$, hence the stated assertion.

$b)$ If the form $\Phi$ is invariant under G (resp. $\mathfrak{g})$, the orthogonal complement of a stable subspace of V is stable; in particular, the representation $\rho$ (resp. $\varphi )$ is then semi-simple (cf. Algebra, Chap. IX); moreover, for all $g\in G$ (resp. $x\in \mathfrak{g})$, the endomorphism $\rho (g)$ (resp. $\varphi (x))$ of V is then semi-simple, with eigenvalues of absolute value 1 (resp. with purely imaginary eigenvalues); indeed $\rho (g)$ is unitary (resp. $i\varphi (x)$ is hermitian, cf. Algebra, Chap. IX).

$c)$ Assume that $k=\mathbf{R}$. If G is a connected Lie group, $\rho$ a morphism of Lie groups, $\mathfrak{g}$ the Lie algebra of G and $\varphi$ the homomorphism induced by $\rho$, then $\Phi$ is invariant under G if and only if it is invariant under $\mathfrak{g}$ (Chap. III, §6, no. 5, Cor. 3).

$d)$ There exists a separating positive hermitian form on V invariant under G if and only if the subgroup $\rho (G)$ of $\mathbf{G}\mathbf{L}(V)$ is relatively compact (Integration, Chap. VII, §3, no. 1, Prop. 1).

### 2. CONNECTED COMMUTATIVE REAL LIE GROUPS

Let G be a connected commutative (real) Lie group. The exponential map

exp$_G: L(G)\rightarrow G$

is a morphism of Lie groups, surjective with discrete kernel (Chap. III, §6, no. 4, Prop. 11), hence the fact that L(G) is a connected covering of G.

$a)$ The following conditions are equivalent: G is simply-connected, exp$_G$ is an isomorphism, G is isomorphic to $\mathbf{R}^n(n=$ dim G). In this case, transporting the vector space structure of L(G) to G by the isomorphism exp$_G$ gives a vector space structure on G, which is the only one compatible with the topological group structure of G. Simply-connected commutative Lie groups are called vector (Lie) groups; unless stated otherwise, they are always given the $\mathbf{R}$-vector space structure defined above.

$b)$ Denote by $\Gamma (G)$ the kernel of exp$_G$. By General Topology, Chap. VII, §1, no. 1, Th. 1, the group G is compact if and only if $\Gamma (G)$ is a lattice in L(G), in other words (loc. cit.) if the rank of the free $\mathbf{Z}$-module $\Gamma (G)$ is equal to the dimension of G. Conversely, if L is a finite dimensional $\mathbf{R}$-vector space and $\Gamma$ a lattice in L, the quotient topological group $L/\Gamma$ is a compact connected commutative Lie group.

The compact connected commutative Lie groups are called real tori, or (in this chapter) tori.

$c)$ In the general case, let E be the vector subspace of L(G) generated by $\Gamma$ (G), and let V be a complementary subspace. Then G is the direct product of its Lie subgroups exp(E) and exp(V); the first is a torus, the second is vector. Finally, every compact subgroup of G is contained in exp(E) (since its projection onto exp(V) is necessarily reduced to the identity element); thus, the subgroup exp(E) is the unique maximal compact subgroup of G.

For example, take $G = C^*$; identify L(G) with $\mathbf{C}$ so that the exponential map of G is $x \rightarrow e^x$. Then $\Gamma (G) = 2\pi i\mathbf{Z},E =i\mathbf{R}$, and so exp(E) $=\mathbf{U}$; if we take $V =\mathbf{R}$, then exp(V) $=\mathbf{R}^*_+$ and we recover the isomorphism $\mathbf{C}^*\rightarrow \mathbf{U}\times \mathbf{R}^*_+$ constructed in General Topology, Chap. VIII, §1, no. 3, Prop. 1.

$d)$ Note finally that exp$_G: L(G)\rightarrow G$ is a universal covering of G, hence $\Gamma (G)$ can be identified naturally with the fundamental group of G.

### 3. COMPACT LIE ALGEBRAS

#### Proposition 1 {#lie-ix-s1-prop-1 .statement tag=019D}

Let $\mathfrak{g}$ be a (real) Lie algebra. The following conditions are equivalent:

(i) $\mathfrak{g}$ is isomorphic to the Lie algebra of a compact Lie group.

(ii) The group Int($\mathfrak{g}$) (Chap. III, §6, no. 2, Def. 2) is compact.

(iii) $\mathfrak{g}$ has an invariant bilinear form (Chap. I, §3, no. 6) that is symmetric, positive and separating.

(iv) $\mathfrak{g}$ is reductive (Chap. I, §6, no. 4, Def. 4); for all $x\in \mathfrak{g}$, the endomorphism ad $x$ is semi-simple, with purely imaginary eigenvalues.

(v) $\mathfrak{g}$ is reductive and its Killing form B is negative.

(i) $=\Rightarrow$ (ii): if $\mathfrak{g}$ is the Lie algebra of a compact Lie group G, the group Int($\mathfrak{g}$) is separating and isomorphic to a quotient of the compact group $G_0$ (Chap. III, §6, no. 4, Cor. 4), hence is compact.

(ii) $=\Rightarrow$ (iii): if the group Int($\mathfrak{g}$) is compact, there exists a symmetric bilinear form on $\mathfrak{g}$ that is positive, separating and invariant under Int($\mathfrak{g}$) (no. 1), hence also invariant under the adjoint representation of $\mathfrak{g}$.

(iii) $=\Rightarrow$ (iv): if (iii) is satisfied, the adjoint representation of $\mathfrak{g}$ is semi-simple (no. 1), hence $\mathfrak{g}$ is reductive; moreover, the endomorphisms ad $x$, for $x\in \mathfrak{g}$, have the indicated properties (no. 1).

(iv) $=\Rightarrow$ (v): for all $x\in \mathfrak{g}, B(x, x) =$ Tr((ad $x)^2)$; consequently, $B(x, x)$ is the sum of the squares of the eigenvalues of ad $x$, and hence is negative if these are purely imaginary.

(v) $=\Rightarrow$ (i): assume that $\mathfrak{g}$ is reductive, hence the product of a commutative subalgebra $\mathfrak{c}$ and a semi-simple subalgebra $\mathfrak{s}$ (Chap. I, §6, no. 4, Prop. 5). The Killing form of $\mathfrak{s}$ is the restriction of the form B to $\mathfrak{s}$, hence is negative and separating if B is negative. The subgroup Int($\mathfrak{s}$) of $\mathbf{G}\mathbf{L}(\mathfrak{s})$ is closed (it is the identity component of Aut($\mathfrak{s}$), Chap. III, §10, no. 2, Cor. 2) and leaves the separating positive form $-B$ invariant; thus, it is compact, and $\mathfrak{s}$ is isomorphic to the Lie algebra of the compact Lie group Int($\mathfrak{s}$). Further, since $\mathfrak{c}$ is commutative, it is isomorphic to the Lie algebra of a torus T. Thus $\mathfrak{g}$ is isomorphic to the Lie algebra of the compact Lie group Int($\mathfrak{s}$)$\times T$.

#### Definition 1 {#lie-ix-s1-def-1 .statement tag=019E}

A compact Lie algebra$^4$ is a Lie algebra that has properties (i) to (v) of Proposition 1.

Thus, the compact Lie algebras are the products of a commutative algebra with a compact semi-simple algebra. In other words, a Lie algebra is compact if and only if it is reductive and its derived Lie algebra is compact.

The Lie algebra of a compact Lie group is compact.

#### Proposition 2 {#lie-ix-s1-prop-2 .statement tag=019F}

a) The product of a finite number of Lie algebras is a compact Lie algebra if and only if each factor is compact.

b) A subalgebra of a compact Lie algebra is compact.

c) Let $\mathfrak{h}$ be an ideal of a compact Lie algebra $\mathfrak{g}$. Then the algebra $\mathfrak{g}/\mathfrak{h}$ is compact and the extension $\mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{h}$ is trivial.

Assertions $a)$ and $b)$ follow from the characterization (iii) of Prop. 1. Part $c)$ follows from $a)$ and the fact that, in a reductive Lie algebra, every ideal is a direct factor (Chap. I, §6, no. 4, Cor. of Prop. 5).

#### Proposition 3 {#lie-ix-s1-prop-3 .statement tag=019G}

Let G be a Lie group of which the group of connected components is finite. The following conditions are equivalent:

(i) The Lie algebra L(G) is compact.

(ii) The group Ad(G) is compact.

(iii) There exists a separating positive symmetric bilinear form on L(G) invariant under the adjoint representation of G.

$^*$(iv) G has a riemannian metric invariant under left and right translations.$_*$

(i) $=\Rightarrow$ (ii): if L(G) is compact, the group Ad(G$_0) =$ Int(L(G)) is compact; since it has finite index in Ad(G), this latter group is also compact.

(ii) $=\Rightarrow$ (iii): this follows from no. 1.

(iii) $=\Rightarrow$ (i): since Int(L(G)) $\subset$ Ad(G), this follows from the characterization (iii) of Prop. 1.

$^*$(iii) $\Leftarrow \Rightarrow$ (iv): this follows from Chap. III, §3, no. $13._*$

### 4. GROUPS WHOSE LIE ALGEBRA IS COMPACT

#### Theorem 1 {#lie-ix-s1-thm-1 .statement tag=019H}

(H. Weyl) Let G be a connected Lie group whose Lie algebra is compact semi-simple. Then G is compact and its centre is finite.

Since G is semi-simple, its centre D is discrete. Moreover, the quotient group $G/D$ is isomorphic to Ad(G) (Chap. III, §6, no. 4, Cor. 4), hence compact (Prop. 3). Finally, the group $G/D$ is equal to its derived group (Chap. III, §9, no. 2, Cor. of Prop. 4). The theorem now follows from Integration, Chap. VII, §3, no. 2, Prop. 5.

#### Proposition 4 {#lie-ix-s1-prop-4 .statement tag=019I}

Let G be a connected Lie group whose Lie algebra is compact. There exist a torus T, a simply-connected compact semi-simple Lie

$^4$ Note that a real topological vector space cannot be a compact topological space

unless it is reduced to 0. group S, a vector group V and a surjective morphism $f: V\times T\times S\rightarrow G$ with finite kernel. If G is compact, the group V is reduced to the identity element.

Let C (resp. S) be a simply-connected Lie group whose Lie algebra is isomorphic to the centre (resp. the derived algebra) of L(G). Then C is a vector group, S is a compact group with finite centre (Th. 1) and G can be identified with the quotient of $C\times S$ by a discrete subgroup D, which is central (Integration, Chap. VII, §3, no. 2, Lemma 4). Since the image of the projection of D onto S is central, hence finite, $D\cap C$ is of finite index in D. Let $C'$ be the vector subspace of C generated by $D\cap C$, and V a complementary subspace. Then the group $T = C'/(D\cap C)$ is a torus, and G is isomorphic to the quotient of the product group $V\times T\times S$ by a finite group.

If G is compact, so is $V\times T\times S ($General Topology, Chap. III, §4, no. 1, Cor. 2 of Prop. 2), hence so is V, which implies that $V =\{e\}$.

#### Corollary 1 {#lie-ix-s1-prop-4-cor-1 .statement tag=019J}

Let G be a connected compact Lie group. Then $C(G)_0$ is a torus, D(G) is a connected compact semi-simple Lie group and the morphism $(x, y) \rightarrow xy$ from $C(G)_0\times D(G)$ to G is a finite covering.

With the notation in Prop. 4, we have $V =\{e\}$ and the subgroups $f(T)$ and $f(S)$ of G are compact, hence closed. Thus it suffices to show that $f(T) =$ $C(G)_0,f(S) = D(G)$. Now, $L(G) = L(f(T))\times L(f(S))$; since S is semi-simple and T is commutative, this implies that $L(f(T)) =\mathscr{C}(L(G)) = L(C(G)_0)$ (Chap. III, §9, no. 3, Prop. 8) and $L(f(S)) =\mathscr{D}L(G) = L(D(G))$ (Chap. III, §9, no. 2, Cor. of Prop. 4), hence the stated assertion.

#### Corollary 2 {#lie-ix-s1-prop-4-cor-2 .statement tag=019K}

The centre and the fundamental group of a connected compact semi-simple Lie group are finite. Its universal covering is compact.

With the notation in Prop. 4, the groups V and T are reduced to the identity element; thus S is a universal covering of G, and the fundamental group of G is isomorphic to Ker $f$, hence finite. The centre D of G is discrete since G is semi-simple, so D is finite.

#### Corollary 3 {#lie-ix-s1-prop-4-cor-3 .statement tag=019L}

The fundamental group of a connected compact Lie group G is a $\mathbf{Z}$-module of finite type, of rank equal to the dimension of C(G).

Indeed, with the notations in Cor. 1, the fundamental group of $C(G)_0$ is isomorphic to $\mathbf{Z}^n$, with $n=$ dim $C(G)_0$, and the fundamental group of D(G) is finite (Cor. 2).

#### Corollary 4 {#lie-ix-s1-prop-4-cor-4 .statement tag=019M}

Let G be a connected compact Lie group. The following conditions are equivalent:

(i) G is semi-simple;

(ii) C(G) is finite;

(i) $\pi_1(G)$ is finite.

If G is simply-connected, it is semi-simple.

This follows from Cor. 1 to 3.

#### Corollary 5 {#lie-ix-s1-prop-4-cor-5 .statement tag=019N}

Let G be a connected compact Lie group. Then Int(G) is the identity component of the Lie group Aut(G) (Chap. III, §10, no. 2).

Let $f\in$ Aut(G)$_0$. Then $f$ induces an automorphism $f_1$ of $C(G)_0$ and an automorphism $f_2$ of D(G), and we have $f_1\in$ Aut(C(G)$_0)_0, f_2\in$ Aut(D(G))$_0$. Since Aut(C(G)$_0)$ is discrete (General Topology, Chap. VII, §2, no. 4, Prop. 5), we have $f_1=$ Id; since D(G) is semi-simple, by Chap. III, §10, no. 2, Cor. 2 of Th. 1 there exists an element $g$ of D(G) such that $f_2(x) =gxg^{-1}$ for all $x\in$ D(G). For all $x\in C(G)_0$, we have $gxg^{-1}=x$ = $f_1(x)$; since $G = C(G)_0.D(G)$, it follows that $gxg^{-1}=f(x)$ for all $x\in G$, so $f=$ Int $g$.

#### Proposition 5 {#lie-ix-s1-prop-5 .statement tag=019O}

Let G be a Lie group whose Lie algebra is compact.

a) Assume that G is connected. Then G has a largest compact subgroup K; it is connected. There exists a closed central vector subgroup (no. 2) N of G such that G is the direct product $N\times K$.

b) Assume that the group of connected components of G is finite. Then:

(i) Every compact subgroup of G is contained in a maximal compact subgroup.

(ii) If $K_1$ and $K_2$ are two maximal compact subgroups of G, there exists $g\in G$ such that $K_2=gK_1g^{-1}$.

(iii) Let K be a maximal compact subgroup of G. Then $K\cap G_0$ is equal to $K_0$; it is the largest compact subgroup of $G_0$.

(iv) There exists a closed central vector subgroup N of $G_0$, normal in G, such that, for any maximal compact subgroup K of G, $G_0$ is the direct product of $K_0$ by N, and G is the semi-direct product of K by N.

$a)$ We retain the notations of Prop. 4. The projection of Ker $f$ onto V is a finite subgroup of the vector group V, hence is reduced to the identity element. It follows that Ker $f$ is contained in $T\times S$, hence that G is the direct product of the vector group $N =f(V)$ and the compact group $K =f(T\times S)$. Every compact subgroup of G has a projection onto N that is reduced to the identity element, hence is contained in K. This proves $a)$.

$b)$ Assume now that $G/G_0$ is finite. By $a), G_0$ is the direct product of its largest compact subgroup M and a vector subgroup P; the subgroup M of G is clearly normal. Let $\mathfrak{n}$ be a vector subspace complement of L(M) in L(G), stable under the adjoint representation of G (no. 1 and no. 3, Prop. 3); this is an ideal of L(G) and we have $L(G) = L(M)\times \mathfrak{n}$. Let N be the integral subgroup of G with Lie algebra $\mathfrak{n}$; by Chap. III, §6, no. 6, Prop. 14, it is normal in G. The projection of L(G) onto L(P) with kernel L(M) induces an isomorphism from $\mathfrak{n}$ to L(P); it follows that the projection of $G_0$ onto P induces an étale morphism from N to P; since P is simply-connected, this is an isomorphism, and N is a vector group. The morphism $(x, y) \rightarrow xy$ from $M\times N$ to $G_0$ is an injective étale morphism (since $M\cap N$ is reduced to the identity element), hence an isomorphism. It follows that N is a closed subgroup of G and that the quotient $G/N$ is compact, since $G_0/N$ is compact and $G/G_0$ is finite (General Topology, Chap. III, §4, no. 1, Cor. 2 of Prop. 2).

By Integration, Chap. VII, §3, no. 2, Prop. 3, every compact subgroup of G is contained in a maximal compact subgroup, these are conjugate, and for any maximal compact subgroup K of G, G is the semi-direct product of K by N. Since $G_0$ contains N, it is the semi-direct product of N by $G_0\cap K$; it follows that $G_0\cap K$ is connected, hence equal to $K_0$, since $K/(G_0\cap K)$ is isomorphic to $G/G_0$, hence finite; finally, $K_0$ is clearly the largest compact subgroup of $G_0$ by $a)$.

#### Corollary {#lie-ix-s1-n4-cor-1 .statement tag=019P}

If N satisfies the conditions of b) (iv), and if $K_1$ and $K_2$ are two maximal compact subgroups of G, there exists $n\in$ N such that $nK_1n^{-1}= K_2$.

Indeed, by (ii) there exists an element $g\in G$ such that $gK_1g^{-1}= K_2$; by (iv), there exists $n\in N$ and $k\in K_1$ such that $g=nk$. The element $n$ then has the required properties.

### Exercises {#lie-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
