---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 15
section_title: Brauer Groups
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.277-A VIII.284
pdf_pages: 0294-0301
extraction: native
subsections:
    - "no": 1
      title: Classes of Algebras
      page: 277
      pdf_page: 294
    - "no": 2
      title: Definition of the Brauer Group
      page: 278
      pdf_page: 295
    - "no": 3
      title: Change of Base Field
      page: 281
      pdf_page: 298
    - "no": 4
      title: Examples of Brauer Groups
      page: 283
      pdf_page: 300
statements: 12
exercises: 2
content_sha256: de0ee49b9fce0132064e5387825b803ddb4c6aeb3c6c606b44846dc5403449fc
---

## § 15. BRAUER GROUPS

In this section, K is a commutative field.

### 1. Classes of Algebras

We denote by Iso$_K(A,B)$ the relation

“A and B are isomorphic K-algebras of finite degree.”

This is an equivalence relation with respect to A and B. Let A be a K-algebra of finite degree; the class of A, denoted by cl(A) (or sometimes cl$_K$(A)), is the class of objects equivalent to A for the relation Iso$_K($Set Theory, II, §6, No. 9, p. 122). By definition, cl(A) is a K-algebra isomorphic to A; two K-algebras of finite degree are in the same class if and only if they are isomorphic.

We denote by $\mathscr{A}$ the set of pairs $(W, \mu)$, where W is a linear subspace of $K^{(\mathbf{N})}$ that is finite-dimensional over K and $\mu$ is a K-bilinear mapping from $W\times W$ to W that makes W into an (associative and unital) K-algebra. Every K-algebra of finite degree is isomorphic to such an algebra. By loc. cit., the relation

“$\alpha$ is a class of K-algebras of finite degree”

is therefore collectivizing in $\alpha ($Set Theory, II, §1, No. 4, p. 68). We denote the set of classes of K-algebras of finite degree by $\mathscr{C}_K$.

#### Proposition 1 {#alg-viii-s15-prop-1 .statement tag=00HV}

The set $\mathscr{C}_K$, endowed with the law of composition given by $(\alpha , \beta )\mapsto$ cl($\alpha \otimes_K\beta$ ), is a commutative monoid. The identity element of $\mathscr{C}_K$ is the class $\varepsilon$ of the K-algebra K. Moreover, if A and B are K-algebras of finite degree, then we have the relation

(1) cl(A $\otimes_KB$) $=$ cl(A) cl(B).

Let A, B, and C be K-algebras of finite degree, with respective classes $\alpha$, $\beta$, and $\gamma$. The K-algebras A and $\alpha$ are isomorphic, as are B and $\beta$. Therefore, the K-algebras $A\otimes_KB$ and $\alpha \otimes_K\beta$ are isomorphic, and we have cl(A$\otimes_KB$) $=$ cl($\alpha \otimes_K\beta$ ), which gives formula (1). It follows that $(\alpha \beta )\gamma$ is the class of the K-algebra $(A\otimes_KB)\otimes_KC$ and $\alpha (\beta \gamma )$ that of the K-algebra $A\otimes_K(B\otimes_KC)$. Now, these K-algebras are isomorphic (III, §4, No. 1, p. 461), so we have the equality $(\alpha \beta )\gamma =\alpha (\beta \gamma )$. Analogously, the relation $\alpha \varepsilon =\varepsilon \alpha =\alpha$ follows from the fact that the K-algebras $A\otimes_KK, K\otimes_KA$, and A are isomorphic, and the relation $\alpha \beta =\beta \alpha$ follows from the fact that the algebras $A\otimes_KB$ and $B\otimes_KA$ are isomorphic.

In the set $\mathscr{C}_K$, the relation “$\alpha$ and $\beta$ are Morita equivalent algebras” is an equivalence relation (VIII, p. 100). It is compatible with the law of composition on $\mathscr{C}_K$ by Proposition 13, d) of VIII, p. 111. We denote by $\mathscr{M}_K$ the quotient monoid of $\mathscr{C}_K$ by this equivalence relation and by $\varphi$ the canonical homomorphism from $\mathscr{C}_K$ to $\mathscr{M}_K$. For every K-algebra A of finite degree, we denote by [A] the image of cl(A) by $\varphi$. If A and B are K-algebras of finite degree, then we have [A] = [B] if and only if the K-algebras A and B are Morita equivalent; moreover, we have the relation

$$
[A\otimes_KB] = [A][B] \tag{2}
$$

in the monoid $\mathscr{M}_K$.

#### Lemma 1 {#alg-viii-s15-lem-1 .statement tag=00HW}

Let A be a K-algebra of finite degree and D a field of finite degree over K. We have [A] = [D] in $\mathscr{M}_K$ if and only if there exists an integer $n\geqslant 1$ such that A is isomorphic to $\mathbf{M}_n(K)$.

By definition, we have [A] = [D] if and only if there exists an invertible $(A$, D)-bimodule, that is (VIII, p. 101, Theorem 1), a right vector space V of nonzero finite dimension over D endowed with an isomorphism of K-algebras $A\rightarrow$ End$_D(V)$. Lemma 1 follows.

### 2. Definition of the Brauer Group

We denote by Br(K) the set of elements of $\mathscr{M}_K$ of the form [A], where A is a central simple algebra of finite degree over K.

#### Proposition 2 {#alg-viii-s15-prop-2 .statement tag=00HX}

The set Br(K) is the set of invertible elements of $\mathscr{M}_K$, where the inverse of an element [A] of Br(K) is $[A^o]$. Consequently, the law of composition on the monoid $\mathscr{M}_K$ endows Br(K) with the structure of an abelian group.

Let A be a central simple algebra of finite degree over K. The algebra $A^o$ is central simple and of finite degree over K (VIII, p. 251). The algebra $A\otimes_KA^o$ is isomorphic to a matrix algebra $\mathbf{M}_n$(K), where $n^2=$ dim(A) (VIII, p. 252, Theorem 1). We therefore have $[A][A^o] = [A\otimes_KA^o] = [K]$ (Lemma 1), which proves that [A] is invertible, with inverse $[A^o]$.

Conversely, let A be a K-algebra of finite degree. If [A] is invertible in $\mathscr{M}_K$, then there exists a K-algebra B of finite degree such that [A][B] = [K]; by formula (2) and Lemma 1, this means that the K-algebra $A\otimes_KB$ is isomorphic to a matrix algebra $\mathbf{M}_n(K)$ with $n\geqslant 1$. By Remark 1 of VIII, p. 251, the algebra A is then central simple.

#### Definition 1 {#alg-viii-s15-def-1 .statement tag=00HY}

The abelian group Br(K) is called the Brauer group of the field K.

#### Lemma 2 {#alg-viii-s15-lem-2 .statement tag=00HZ}

Let I and J be finite sets, $k$ be a commutative ring, and A and B be $k$-algebras. Denote by $\mathbf{M}_I(A)$ the $k$-algebra of square matrices of type $(I,I)$ with entries in A, and define the $k$-algebras $\mathbf{M}_J(B)$ and $\mathbf{M}_{I\times J}(A\otimes_KB)$ likewise. There exists a unique $k$-algebra isomorphism

$$
\varphi :\mathbf{M}_I(A)\otimes_k\mathbf{M}_J(B)\longrightarrow \mathbf{M}_{I\times J}(A\otimes_kB)
$$

such that $\varphi ((a_{ii'})\otimes (b_{jj'}))$ is the matrix with entry of index $((i, j),(i', j'))$ equal to $a_{ii'}\otimes b_{jj'}$.

The existence of a $k$-linear bijection $\varphi$ with the property stated in the lemma follows from the compatibility of the tensor product with direct sums (II, §3, No. 7, p. 255, Proposition 7). The fact that $\varphi$ is an algebra homomorphism follows from the definition of a product matrix.

#### Proposition 3 {#alg-viii-s15-prop-3 .statement tag=00I0}

Let A and B be central simple K-algebras of finite degree. The following properties are equivalent:

(i) We have [A] = [B] in the Brauer group Br(K).

(ii) There exists an integer $t\geqslant 1$ such that the K-algebra $A\otimes_KB^o$ is isomorphic to the matrix algebra $\mathbf{M}_t(K)$.

(iii) There exist strictly positive integers $r$ and $s$ such that the K-algebras $A\otimes_K\mathbf{M}_r(K)$ and $B\otimes_K\mathbf{M}_s(K)$ are isomorphic.

(iv) There exist a field D containing K and integers $m\geqslant 1$ and $n\geqslant 1$ such that A is isomorphic to $\mathbf{M}_m(D)$ and B to $\mathbf{M}_n(D)$.

(v) The K-algebras A and B are Morita equivalent.

Suppose that we have [A] = [B]. Since $[B^o]$ is the inverse of [B] in the Brauer group, we have $[K] = [B][B^o] = [A][B^o] = [A\otimes_KB^o]$. By Lemma 1, there exists an integer $t\geqslant 1$ such that the algebras $A\otimes_KB^o$ and $\mathbf{M}_t(K)$ are isomorphic. So (i) implies (ii).

Suppose that (ii) holds. Since $B^o\otimes_KB$ is isomorphic to a matrix algebra $\mathbf{M}_s(K)$ with $s\geqslant 1$ (VIII, p. 252, Theorem 1), the algebra $A\otimes_KB^o\otimes_KB$ is isomorphic to $A\otimes_K\mathbf{M}_s$(K), on the one hand, and to $\mathbf{M}_t(K)\otimes_KB$, on the other. So property (ii) implies property (iii).

Suppose that (iii) holds. By Wedderburn’s theorem (VIII, p. 120, Theorem 1), there exist integers $m\geqslant 1$ and $n\geqslant 1$ and fields D and $D'$ of finite degree over K with center K such that A is isomorphic to $\mathbf{M}_m(D)$ and B to $\mathbf{M}_n(D')$. Then the algebra $A\otimes_K\mathbf{M}_r(K)$ is isomorphic to $\mathbf{M}_{mr}$(D), and the algebra $B\otimes_K\mathbf{M}_{r'}(K)$ is isomorphic to $\mathbf{M}_{nr'}(D')$ (Lemma 2). By Corollary 2 of VIII, p. 121, the K-algebras D and $D'$ are isomorphic. So (iii) implies (iv).

Suppose that (iv) holds. The algebras A and D are Morita equivalent, as are the algebras B and D (VIII, p. 114, Example 2). Therefore, A and B are Morita equivalent, so (iv) implies (v).

Finally, the implication (v)$\Rightarrow$(i) is the definition of the set Br(K).

When the equivalent properties of the proposition hold, we say that the algebras A and B are similar.

#### Corollary {#alg-viii-s15-n2-cor-1 .statement tag=00I1}

Let A and B be central simple algebras of finite degree over K. Then A and B are isomorphic if and only if they are similar and have the same degree.

This follows from the equivalence of properties (i) and (iv) of Proposition 3 and the fact that dim$_K(\mathbf{M}_n(D)) =$ dim$_K(D)\times n^2$.

#### Proposition 4 {#alg-viii-s15-prop-4 .statement tag=00I2}

Let $\mathscr{K}_K$ be the set of classes of central K-algebras of finite degree that are fields. The mapping $D\mapsto [D]$ from $\mathscr{K}_K$ to Br(K) is bijective.

This follows from Lemma 1 of VIII, p. 278 and Wedderburn’s theorem (VIII, p. 120, Theorem 1).

### 3. Change of Base Field

Let L be an extension of the field K. Let A and B be K-algebras of finite degree; then the L-algebras $A_{(L)}$ and $B_{(L)}$ are of finite degree. The L-algebras $A_{(L)}\otimes_LB_{(L)}$ and $(A\otimes_KB)_{(L)}$ are isomorphic (III, §4, No. 1, p. 462, Proposition 3). The L-algebra $K_{(L)}$ is isomorphic to L. Consequently, there exists a unique monoid homomorphism $\rho_{L/K}$ from $\mathscr{C}_K$ to $\mathscr{C}_L$ such that

(3) $\rho_{L/K}$(cl(A)) = cl(A$_{(L)}$)

for every K-algebra A of finite degree.

If the K-algebras A and B are Morita equivalent, then so are the L-algebras $A_{(L)}$ and $B_{(L)}$ (VIII, p. 111, Proposition 13, e)). If the K-algebra A is central simple and of finite degree, then so is the L-algebra $A_{(L)}$ (VIII, p. 251, Remark 2). So we can deduce from $\rho_{L/K}$ a group homomorphism $r_{L/K}$ from Br(K) to Br(L) such that

$$
r_{L/K}([A]) = [A_{(L)}] \tag{4}
$$

for every central simple K-algebra A of finite degree.

Let M be an extension of the field L. Because extension of scalars is transitive (III, §1, No. 5, p. 434), we have the relation

$$
r_{M/K}=r_{M/L}\circ r_{L/K} \tag{5}
$$

Let A be a central simple K-algebra of finite degree, and let L be an extension of K. We say that L is a splitting field for A (or splits A) if the L-algebra $A_{(L)}$ is isomorphic to a matrix algebra $\mathbf{M}_n(L)$ for an integer $n\geqslant 1$. In the aforementioned notation, this corresponds to saying that the class of A in Br(K) belongs to the kernel of the homomorphism $r_{L/K}:$ Br(K) $\rightarrow$ Br(L).

If B is similar to A, then L is a splitting field for A if and only if it is a splitting field for B.

If L is a splitting field for A, then every extension of L is a splitting field for A. By Theorem 1 of VIII, p. 252, there exists a Galois extension of K of finite degree that is a splitting field for A, and every separable closure of K is a splitting field for A.

#### Proposition 5 {#alg-viii-s15-prop-5 .statement tag=00I3}

Let A be a central simple K-algebra of finite degree, and let L be an extension of K of finite degree. The following properties are equivalent:

(i) The extension L is a splitting field for A.

(ii) There exists a central simple K-algebra of finite degree similar to A containing a maximal commutative subalgebra isomorphic to L.

Let us prove that (ii) implies (i); it suffices to consider the case when L is a maximal commutative subalgebra of A. Let $\psi : A\otimes_KA^o\rightarrow$ End$_K(A)$ be the canonical isomorphism that sends $a\otimes a'$ to the K-linear mapping $x\mapsto axa'$ (VIII, p. 252, Theorem 1). We view A as a right vector space over L; then $\psi$ sends $A\otimes_KL$ into the subspace End$_L(A)$ of End$_K(A)$ and induces, by restriction, an injective homomorphism of L-algebras $\psi ': A\otimes_KL\rightarrow$ End$_L(A)$. Set $n= [L : K]$. By VIII, p. 262, Proposition 3, we have $[A : L] =n$, and therefore $[A\otimes_KL : L] = [A : K] =n^2$ and [End$_L(A) : L] =n^2$. Consequently, $\psi '$ is an isomorphism, which proves (i).

The converse follows from Lemma 3 below.

#### Lemma 3 {#alg-viii-s15-lem-3 .statement tag=00I4}

Let A be a central simple K-algebra of finite degree, and let L be an extension of K of finite degree that is a splitting field for A. Let V be a simple $A_{(L)}$-module, so that the natural morphism $\varphi : A_{(L)}\rightarrow$ End$_L(V)$ is an isomorphism. Let C be the ring End$_A(V)$. Then C is similar to $A^o$, and the image of $L\otimes 1\subset A_{(L)}$ is a maximal commutative subalgebra of C.

We identify A with a subring of $A_{(L)}$. We view V as a K-vector space. The ring C is the commutant of $\varphi (A)$ in End$_K(V)$. It is a central simple K-algebra of finite degree, and the homomorphism $a\otimes c\mapsto ac$ from $A\otimes_KC$ to End$_K(V)$ is an isomorphism (VIII, p. 260, Theorem 6, a)). Consequently, the K-algebras A and $C^o$ are similar (VIII, p. 279, Proposition 3).

Let $L_V$ be the ring of homotheties of the L-vector space V; it is the commutant of End$_L(V)$ in End$_K(V)$ (VIII, p. 82, Corollary 1). Now, the K-algebra End$_L(V)$ is generated by $\varphi (A)$ and $L_V$; therefore, in End$_K$(V), we have

$L_V=$ End$_L(V)'=\varphi (A)'\cap L'_V= C\cap L'_V$,

where for any subset B of End$_K$(V), the commutant of B in End$_K(V)$ is denoted by $B'$. So $L_V$ is a maximal commutative subalgebra of C (VIII, p. 261, Lemma 3), and therefore also of $C^o$. The mapping $\lambda \mapsto \lambda_V$ is a K-algebra isomorphism from L to $L_V$. This proves the lemma.

#### Corollary 1 {#alg-viii-s15-lem-3-cor-1 .statement tag=00I5}

Let A be a central simple K-algebra of finite degree, and let L be an extension of K of finite degree. Suppose $[A : K] = [L : K]^2$. Then L is a splitting field for A if and only if A contains a subalgebra isomorphic to L.

Suppose that there exists a morphism $\varphi$ from L to A. Let M be a maximal semisimple commutative subalgebra containing $\varphi (L)$. By Proposition 3 of VIII, p. 262, we have $[A : K] = [M : K]^2$, hence [M : K] = [L : K] and $M =\varphi (L)$. By Proposition 5, the field L splits A. Conversely, suppose that the field L splits A; then it is isomorphic to a maximal commutative subalgebra of a central simple K-algebra B similar to A (Proposition 5). We have $[B : K] = [L : K]^2$ (VIII, p. 262, Proposition 3), hence [B : K] = [A : K]. Consequently, B is isomorphic to A (VIII, p. 280, Corollary). Corollary 1 follows.

#### Corollary 2 {#alg-viii-s15-lem-3-cor-2 .statement tag=00I6}

Let D be a field of finite degree over K with center K, and let L be an extension of K of finite degree that is a splitting field for D. The reduced degree of D divides [L : K].

Denote the reduced degree of D (VIII, p. 253) by $r$; by definition, we have $[D : K] =r^2$. By Proposition 5, there exists a central simple K-algebra B similar to D of which L is a maximal commutative subalgebra. Since B is isomorphic to a matrix algebra $\mathbf{M}_n(D)$ (VIII, p. 278, Lemma 1), we have $[B : K] =n^2r^2$ and consequently $[L : K] =nr$ (VIII, p. 262, Proposition 3).

### 4. Examples of Brauer Groups

The Brauer group Br(K) is reduced to the identity element in the following three cases:

a) K is separably closed (VIII, p. 253, Corollary 1).

$*$b) K is a finite field (VIII, p. 357, Corollary 2).

c) K has property $(C_1)$ (VIII, p. 357, Remark 2).

Suppose that K is a maximal ordered field (VI, §2, No. 5, p. 25). The Brauer group of K is then cyclic of order 2; its elements are the class of K and the class of the quaternion K-algebra of type $(-1,0,-1)$ (III, §2, No. 5, p. 444 and VIII, p. 367, Theorem 1).

Suppose that K is a locally compact, nondiscrete, commutative topological field. If K is not connected, then it is a complete field for a discrete valuation, with finite residue field (Comm. Alg., VI, §9, No. 3, p. 433, Theorem 1), and there exists an isomorphism from Br(K) to $\mathbf{Q}/\mathbf{Z}$ (VIII, p. 332, Exercise 17). If K is connected, then it is isomorphic to $\mathbf{R}$ or $\mathbf{C}$. The Brauer group of the field $\mathbf{R}$ is cyclic of order 2. Its nontrivial element is the class of the algebra $\mathbf{H}$ of Hamilton quaternions (Gen. Top., VIII, §1, No. 4, p. 104); the Brauer group of $\mathbf{C}$ has order 1.

### Exercises {#alg-viii-s15-exercises}

See the [exercises for § 15](exercises/s15/).
