---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 19
section_title: Quaternion Algebras
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.361-A VIII.371
pdf_pages: 0378-0388
extraction: native
subsections:
    - "no": 1
      title: General Properties of Quaternion Algebras
      page: 361
      pdf_page: 378
    - "no": 2
      title: The Center of a Quaternion Algebra
      page: 363
      pdf_page: 380
    - "no": 3
      title: Simplicity of Quaternion Algebras
      page: 363
      pdf_page: 380
    - "no": 4
      title: Criteria for a Quaternion Algebra to Be a Field
      page: 366
      pdf_page: 383
    - "no": 5
      title: Algebras over Maximal Ordered Fields
      page: 367
      pdf_page: 384
statements: 15
exercises: 8
content_sha256: d95e3efb2419800092f75323d4131d2a82c14d1a1f6ca91acbfc26abb30857fc
---

## § 19. QUATERNION ALGEBRAS

In this section, K is a commutative field.

### 1. General Properties of Quaternion Algebras

Let $\alpha , \beta , \gamma$ be elements of K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$. Recall (III, §2, No. 5, p. 445)[^1] that F is an associative unital K-algebra that has a basis $(1, i, j, k)$ over K satisfying the relations (1) $i^2=\alpha +\beta i ,j^2=\gamma  ,ij=k ,ji=\beta j-k$.

It is a Cayley algebra (III, §2, No. 4, p. 441, Definition 1) whose conjugation satisfies (2) $i=\beta -i ,j=-j ,k=-k$.

Recall that the Cayley trace and norm of F are the mappings $T_F$ and $N_F$ from F to K defined by $T_F(q) =q+q$ and $N_F(q) =qq$.

The linear subspace E of F with basis $(1, i)$ is a commutative Cayley subalgebra of F; it is a quadratic algebra of type $(\alpha , \beta )$, and F can be identified with the Cayley extension of E defined by $\gamma$ (III, §2, No. 5, p. 444). For every $z\in E$, we have $zj=jz$. Every element $q$ of F can be written uniquely as $x+jy$ with $x, y\in E$, and we have

$$
q=x-jy ,T_F(q) =x+x ,N_F(q) =xx-\gamma yy \tag{3}
$$

#### Proposition 1 {#alg-viii-s19-prop-1 .statement}

The characteristic polynomial of an element $q$ of F is equal to $X^2-T_F(q)X + N_F(q)^2$.

By the above, the algebra F is a free right E-module with basis $(1, j)$. Consequently, F[X] is a free right E[X]-module with basis $(1, j)$. We denote by $u$ the endomorphism of the right E[X]-module F[X] defined by $u(P) =$ $(X-q)P$ for $P\in F[X]$. The characteristic polynomial of $q$ is the determinant of $u$ viewed as an endomorphism of the K[X]-module F[X]. By Proposition 6 of III, §9, No. 4, p. 546, it is equal to N(det $u)$, where N denotes the norm from E[X] to K[X]. Let us write $q$ as $x+jy$ with $x, y\in E$. The matrix of $u$ with respect to the basis $(1, j)$ is $^X_-^-_y^x_X^-_-^{\gamma y}_x$ ; its determinant is equal to $D = (X-x)(X-x)-\gamma yy= X^2-T_F(q)X + N_F(q)$ (cf. formula (3)). Since D belongs to K[X], we have $N(D) = D^2$; Proposition 1 follows.

#### Remark 1 {#alg-viii-s19-n1-rem-1 .statement}

Suppose that the characteristic of K is different from 2, and set $i'= 2i-\beta$. Then $(1, i')$ is a basis of E over K, and we have $i'^2= 4\alpha +\beta^2$. It follows that E is isomorphic to the quadratic algebra of type $(4\alpha +\beta^2,0)$ and F to the quaternion algebra of type $(4\alpha +\beta^2,0, \gamma )$.

#### Remark 2 {#alg-viii-s19-n1-rem-2 .statement}

The quaternion algebra of type $(\alpha ,0, \gamma )$ is isomorphic to the quaternion algebra of type $(\gamma ,0, \alpha )$ (III, §2, No. 5, p. 445). It is also isomorphic to the quaternion algebra of type $(\alpha a^2,0, \gamma c^2)$ for every pair $(a, c)$ of nonzero elements of K.

#### Remark 3 {#alg-viii-s19-n1-rem-3 .statement}

Let $q$ be an element of F. Then $q$ is nilpotent if and only if its characteristic polynomial is equal to $X^4$, that is, $T_F(q) = N_F(q) = 0$; we then have $q^2= 0$.

#### Example {#alg-viii-s19-n1-exa-1 .statement}

The matrix algebra $\mathbf{M}_2(K)$ is isomorphic to the quaternion algebra of type $(0,1,1)$. Indeed, consider the quadratic algebra $E = K\times K$ (of type $(0,1))$ and the quaternion algebra $F = E + Ej$, which is the Cayley extension of E defined by the element $\gamma = 1$. The mapping $(a, b)\mapsto (^a_0^0_b)$ is an algebra homomorphism from E to $\mathbf{M}_2(K)$. Since for $a, b$ in K, we have

$$
(01)((01)(10)(01)((a0)(b0)((01)
$$

= $$, = $$,

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0 this homomorphism extends to an algebra homomorphism $\theta : F\longrightarrow \mathbf{M}_2(K)$ defined by

$$
(ac)
$$

$\theta (a, b) + (c, d)j$ = $db$.

This homomorphism is bijective. When the characteristic of K is different from 2, the algebra $\mathbf{M}_2(K)$ is also isomorphic to the quaternion algebra of type $(1,0,1)$ (Remark 1).

### 2. The Center of a Quaternion Algebra

Let $\alpha ,\beta ,\gamma$ be elements of K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$.

#### Proposition 2 {#alg-viii-s19-prop-2 .statement}

a) Suppose that the field K has characteristic different from 2. If $\gamma$ or $4\alpha +\beta^2$ is nonzero, then the center of F is equal to K; otherwise, it has dimension 2 and is generated by 1 and $ij-ji$.

b) Suppose that the field K has characteristic 2. If $\beta \not= 0$, then the center of F is equal to K; if $\beta = 0$, then the algebra F is commutative.

By formula (30) of III, §2, No. 5, p. 444, we have

$$
ij-ji=-\beta j+ 2k ,jk-kj=\beta \gamma -2\gamma i ,ki-ik=-2\alpha j-\beta k \tag{4}
$$

An element $q=x+yi+zj+tk$ of F is central if and only if it commutes with $i$ and $j$, that is, we have

(5) $2z+\beta t=-\beta z+ 2\alpha t= 0$ and $2\gamma t=\beta \gamma t= 2y=\beta y= 0$.

First suppose that the characteristic of K is different from 2. If $\gamma$ is nonzero, then the equalities in (5) imply $y=t= 0$ and then $z= 0$; consequently, we have $q\in K$. If $\gamma = 0$ and $4\alpha +\beta^2\not= 0$, then they imply $y=z=t= 0$, so we have $q\in K$. If $\gamma = 4\alpha +\beta^2= 0$, then the system (5) reduces to $y= 2z+\beta t= 0$, so we have $q=x+t/2(ij-ji)$, which completes the proof of a).

Now suppose that the field K has characteristic 2. The system (5) can then be written as $\beta t=\beta z=\beta y= 0$; assertion b) follows.

### 3. Simplicity of Quaternion Algebras

#### Proposition 3 {#alg-viii-s19-prop-3 .statement}

Let $\alpha ,\beta ,\gamma$ be elements of K, and let $f$ be a quaternion algebra of type $(\alpha , \beta , \gamma )$. Denote its Cayley trace and norm by $T_F$ and $N_F$. The following properties are equivalent:

(i) The algebra F is central simple.

(ii) For every nonzero element $x$ of F, there exists an element $y$ in F such that $T_F(xy)\not= 0$.

(iii) We have $(4\alpha +\beta^2)\gamma \not= 0$. Suppose that these properties hold. Then for every $x$ in F, the reduced characteristic polynomial of $x$ is $X^2-T_F(x)X + N_F(x)$. In particular, $T_F(x)$ is the reduced trace of $x$, and $N_F(x)$ is its reduced norm.

(i)$\Rightarrow$(ii): If the algebra F is central simple, then it follows from Proposition 1 of VIII, p. 361 and the definition of the reduced trace (VIII, p. 340, Definition 2) that $T_F$ is its reduced trace; assertion (ii) follows (VIII, p. 343, Proposition 5).

(ii)$\Leftrightarrow$(iii): Let $(e_i)_{1\leqslant i\leqslant 4}$ be a basis of F of type $(\alpha , \beta , \gamma )$ (III, §2, No. 5, p. 445). The matrix $(T_F(e_ie_j))$ is equal to

2 $\beta$ 0 0

$\beta 2\alpha +\beta^2$ 0 0

$$.

0 0 $2\gamma \beta \gamma$

0 0 $\beta \gamma -2\alpha \gamma$

Its determinant is $-\gamma^2(4\alpha +\beta^2)^2$. The equivalence of properties (ii) and (iii) follows from V, §8, No. 2, p. 49, Lemma 1.

(iii)$\Rightarrow$(i): Suppose $(4\alpha +\beta^2)\gamma \not= 0$. We then have $\gamma \not= 0$, and we have $\beta \not= 0$ if K has characteristic 2. By Proposition 2, the algebra F is central. Let $x$ be an element of the Jacobson radical of F. For every $y\in F,xy$ is nilpotent, so $T_F(xy) = 0$ (Remark 3 of VIII, p. 362). Since (ii) is equivalent to (iii), we have $x= 0$. This proves that F is a semisimple K-algebra. Since its center is K, it is simple.

The last assertion follows from Proposition 1 of VIII, p. 361 and the definition of the reduced characteristic polynomial (VIII, p. 340, Definition 1).

Denote the characteristic of K by $p$. By Proposition 3, if $p\not= 2$, then every quaternion algebra over K of type $(\alpha ,0, \gamma )$ with $\alpha$ and $\gamma$ in $K^*$ is central simple. If $p= 2$, then every quaternion algebra of type $(\alpha ,1, \gamma )$ with $\alpha \in K$ and $\gamma \in K^*$ is central simple. Conversely, we have the following.

#### Proposition 4 {#alg-viii-s19-prop-4 .statement}

Let A be a central simple algebra of degree 4 over K. Denote the characteristic of K by $p$.

a) If $p\not= 2$, then there exist nonzero elements $\alpha$ and $\gamma$ of K such that the algebra A is isomorphic to the quaternion algebra of type $(\alpha ,0, \gamma )$.

b) If $p= 2$, then there exist an element $\alpha$ of K and an element $\gamma$ of $K^*$ such that the algebra A is isomorphic to the quaternion algebra of type $(\alpha ,1, \gamma )$.

By Wedderburn’s theorem (VIII, p. 120, Theorem 1), there exist an integer $r\geqslant 1$ and a field D with center K such that A is isomorphic to $\mathbf{M}_r(D)$. We then have $r^2[D : K] = [A : K] = 4$. If $r= 2$, then A is isomorphic to $\mathbf{M}_2$(K), and Proposition 4 follows from the example of VIII, p. 362. Otherwise, we have $r= 1$, and A is a field with center K. It then has a maximal commutative subfield E that is a separable extension of K; since A has degree 4 over K, the extension E has degree 2 over K (VIII, p. 265, Corollary 2). It is therefore quadratic (III, §2, No. 3, p. 439). Let $s$ be the conjugation of E (III, §2, No. 3, p. 440). By the Skolem–Noether theorem (VIII, p. 256, Corollary 1), there exists an invertible element $j$ of A such that we have $s(x) =jxj^{-1}$ for every $x$ in E. The field E is separable over K, so we have $s\not=$ Id$_E$, so that $j /\in E$. Since A is a vector space of dimension 4 over K, it is a left vector space of dimension 2 over E, so we have $A = E\oplus Ej$. We have $s^2=$ Id$_E$, so the element $j^2$ of A belongs to the center of A; hence there exists an element $\gamma$ of $K^*$ such that $j^2=\gamma$.

When $p\not= 2$, there exist an element $i$ of E and an element $\alpha \in K^*$ such that $E = K(i)$ and $i^2=\alpha$ (V, §11, No. 9, p. 93, Example 3); in this case, A is isomorphic to the quaternion algebra of type $(\alpha ,0, \gamma )$. When $p= 2$, there exist an element $i$ of E and an element $\alpha$ of K such that $E = K(i)$ and $i^2=i+\alpha$ (V, §11, No. 9, p. 93, Example 2), so that A is isomorphic to the quaternion algebra of type $(\alpha ,1, \gamma )$.

#### Corollary 1 {#alg-viii-s19-prop-4-cor-1 .statement}

Let A be a central simple K-algebra of finite degree $>1$ whose elements are all algebraic of degree $\leqslant 2$ over K. Then A is isomorphic to a quaternion algebra over K.

If K is finite, then the algebra A is isomorphic to a matrix algebra $\mathbf{M}_n(K)$ (VIII, p. 357, Corollary 2) and therefore contains elements of degree $n$ over K; the assumption implies $n= 2$ and therefore the result in this case (VIII, p. 362, Example). Suppose that the field K is infinite. Let L be a maximal étale subalgebra of A. By V, §7, No. 4, p. 41, Proposition 7, there exists an element $x$ of A such that the K-algebra L is equal to $K[x]$, hence by assumption has degree $\leqslant 2$. Since we have $[A : K] = [L : K]^2$ (VIII, p. 264, Proposition 4 and p. 262, Proposition 3), we conclude that [A : K] = 4. Corollary 1 then follows from Proposition 4.

#### Corollary 2 {#alg-viii-s19-prop-4-cor-2 .statement}

Let $(E, s)$ be a Cayley algebra over K such that the K-algebra E is central simple of finite degree $>1$ over K. Then E is isomorphic to a quaternion algebra over K.

Every element $u$ of E satisfies $u^2-T_E(u)u+ N_E(u) = 0$, so the K-algebra E is isomorphic to a quaternion algebra (Corollary 1).

### 4. Criteria for a Quaternion Algebra to Be a Field

Let $\alpha , \beta , \gamma$ be elements of the field K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$. As in No.1, we denote the canonical basis of F by $(1, i, j, k)$ and the subalgebra $K + Ki$ of F by E.

#### Proposition 5 {#alg-viii-s19-prop-5 .statement}

The following properties are equivalent:

(i) The quaternion algebra F is a field.

(ii) There is no nonzero element $q\in F$ such that $T_F(q) = N_F(q) = 0$.

(iii) Every element of F of square zero is zero.

(iv) There does not exist any nonzero vector $(x, y, z, t)$ in $K^4$ such that

$$
x^2+\beta xy-\alpha y^2-\gamma (z^2+\beta zt-\alpha t^2) = 0
$$

(v) There does not exist any nonzero vector $(x, y, z)$ in $K^3$ such that

$$
x^2+\beta xy-\alpha y^2-\gamma z^2= 0
$$

(vi) The quadratic algebra E is a field, and $\gamma$ is not the norm of an element of E.

An element $q$ of F is invertible if and only if $N_F(q)$ is not 0. The equivalence of (i) and (iv) therefore follows from formula (31) of III, §2, No. 5, p. 445; it is clear that (i) implies (iii) and that (iv) implies (v).

The equivalence of (ii) and (iii) follows from Remark 3 of VIII, p. 362.

Suppose that F is not a field. If $\gamma (4\alpha +\beta^2)\not= 0$, then the algebra F is central simple of degree 4 over K; it is isomorphic to the algebra $\mathbf{M}_2(K)$ (VIII, p. 120, Theorem 1) and therefore contains a nonzero element of square zero. If $\gamma = 0$, then we have $j^2= 0$. If $4\alpha +\beta^2= 0$, then we have $(2i-\beta )^2= 0$ and $2i-\beta \not= 0$ if K has characteristic different from 2. Finally, if K has characteristic 2 and $\beta$ is zero, then we have $T_F(q) = 0$ for every $q\in F$ (III, §2, No. 5, p. 445, formula (31)). Since F is not a field, there exists a nonzero element $q$ of F such that $N_F(q) = 0$; we have $q^2= 0$. This proves the implication (iii)$\Rightarrow$(i).

Let $q=x+yi$ be an element of E. We have $N_{E/K}(q) =x^2+\beta xy-\alpha y^2$. Suppose that property (v) holds. We have $N_{E/K}(q)-\gamma \not= 0$ and $N_{E/K}(q)\not= 0$ if $q\not= 0$, and therefore (vi).

Finally, suppose that property (vi) holds. Let $q$ be a nonzero element of F; we write it as $u+vj$ with $u$ and $v$ in E. If $v$ is zero, then $q$ is invertible. If $v$ is not zero, then we have $N_F(q) = N_F(v)N_F(v^{-1}u+j) =$ $N_{E/K}(v) N_{E/K}(v^{-1}u)-\gamma$ by III, §2, No. 5, p. 443, formula (24). Since $\gamma$ is not a norm, $N_F(q)$ is not zero, and $q$ is invertible. **Remark.** — Suppose that the quaternion algebra F is a field. It follows from the equality $j^2=\gamma$ that we have $\gamma \not= 0$. By Proposition 2 of VIII, p. 363, the center of F is equal to K unless K has characteristic 2 and $\beta$ is zero, in which case the algebra F is commutative.

### 5. Algebras over Maximal Ordered Fields

Let R be a maximal ordered field (VI, §2, No. 5, p. 25). Let C be the quadratic R-algebra of type $(-1,0)$; if $(1, i)$ is its canonical basis, then we have $i^2=-1$. Moreover, C is an algebraic closure of R (VI, §2, No. 6, p. 26, Theorem 3). Let H be the quaternion R-algebra of type $(-1,0,-1)$. The multiplication table of H in its canonical basis $(1, i, j, k)$ is given by

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j ,jk=-kj=i
$$

We identify C with the subalgebra $R + Ri$ of H. The conjugate of an element $q=x+yi+zj+tk$ of H is $q=x-yi-zj-tk$. The Cayley trace and norm of $q$ are given by

$$
T(q) =q+q= 2x ,N(q) =qq=x^2+y^2+z^2+t^2
$$

Since R is an ordered field, we have $N(q)>0$ if $q\not= 0$, so H is a field, with center R (VIII, p. 363, Proposition 2). The reduced trace and norm of an element $q$ of H are $T(q)$ and $N(q)$, respectively.

#### Theorem 1 {#alg-viii-s19-thm-1 .statement}

Let D be an R-algebra of finite degree that is a field. Then D is isomorphic to R, C, or H.

Denote the center of D by Z, and let L be a maximal commutative subfield of D. We have $[D : Z] = [L : Z]^2$ by VIII, p. 265, Corollary 2; we also have $[L : R]\leqslant 2$ because C is an algebraic closure of R. There are consequently three possible cases:

a) We have R = Z = L, so [D : Z] = 1 and D = R.

b) We have $R\not= Z$ and Z = L, so [D : Z] = 1 and D = L. In this case, D is isomorphic to C.

c) We have R = Z and [L : R] = 2, so [D : R] = 4. By Proposition 4 of VIII, p. 364, the R-algebra D is isomorphic to a quaternion algebra of type $(\alpha ,0, \gamma )$, where $\alpha$ and $\gamma$ are nonzero elements of R. Let $i\in D$ Z be such that $i^2=\alpha$. We have $\alpha \not= 0$. If $\alpha  >0$, then there exists an $a\in R$ such that $a^2=\alpha$ (VI, §2, No. 6, p. 26, Theorem 3); we then have $(a-i)(a+i) = 0$, which is absurd because D is a field. So we have $\alpha  <0$. The inequality $\gamma  <0$ is shown analogously. There then exist elements $a$ and $c$ of $R^*$ such that $\alpha =-a^2$ and $\gamma =-c^2$ (loc. cit.). The algebra D is therefore isomorphic to the quaternion algebra of type $(-1,0,-1)$ (VIII, p. 362, Remark 2), that is, to H.

#### Remark 1 {#alg-viii-s19-n5-rem-1 .statement}

Let O be the octonion algebra of type $(-1,0,-1,-1)$ over R (III, Appendix, No. 3, p. 615). Let D be an alternative Cayley algebra over R such that every nonzero element of D has an inverse. We can prove (VIII, p. 370, Exercise 5) that D is isomorphic to R, C, H, or O.

#### Remark 2 {#alg-viii-s19-n5-rem-2 .statement}

The above applies to the field $\mathbf{R}$ of real numbers. Every $\mathbf{R}$-algebra of finite degree that is a field is isomorphic to $\mathbf{R},\mathbf{C}$, or $\mathbf{H}$.

#### Remark 3 {#alg-viii-s19-n5-rem-3 .statement}

Let A be a normed algebra over the field $\mathbf{R}$. Suppose that A is a field. Then A is isomorphic to $\mathbf{R},\mathbf{C}$, or $\mathbf{H}$ (“Gelfand–Mazur theorem”) (cf. Comm. Alg., VI, §6, No. 4, p. 407, Theorem 1 and TS, I, §2, n$^o5$, p. 26, corollaire $2).*$

### Exercises {#alg-viii-s19-exercises}

1) a) Let D be a noncommutative field with center K whose elements all have degree $\leqslant 2$ over K. Prove that D is a quaternion algebra over K (Exercise 6, b) of VIII, p. 270). b) Prove that a Cayley K-algebra that is a noncommutative field with center K is a quaternion algebra over K.

$\P 2)$ a) Let A be a simple ring of finite rank over its center K, and let $s$ be an involutive antiautomorphism of A. Let $s'$ be an involutive antiautomorphism of A that coincides with $s$ on K. Prove that there exists an element $a$ of A such that we have $s'(x) =as(x)a^{-1}$ for every $x\in A$ and $s(a) =a$ or $s(a) =-a$ (apply the Skolem–Noether theorem and Theorem 3 of V, §11, No. 6, p. 85). Also prove the converse. b) Suppose that the restriction of $s$ to K is not the identity; let $K_0$ be the subfield of K consisting of the elements fixed by $s$. Prove that the set $A_0$ (resp. $A_1)$ of elements $a$ of A such that $s(a) =a$ (resp. $s(a) =-a)$ is a $K_0$-linear subspace of A of dimension [A : K] and that $A_0$ is a $K_0$-structure on A (use V, §10, No. 4, p. 63, Proposition 7). c) Suppose that the restriction of $s$ to K is the identity; set $[A : K] =m^2$. Prove that $A_0$ is a $K_0$-linear subspace of A of dimension $m(m+ 1)/2$ or $m(m-1)/2$ (reduce to the case when A is a matrix algebra over K and use a)).

$\P 3)$ Let $(F, s)$ be a semisimple (associative) Cayley K-algebra. a) Prove that the K-algebra F is simple or isomorphic to the product of a simple algebra and its opposite algebra (consider the action of conjugation on the set of central idempotents). b) Prove that if F is not commutative, then it is isomorphic to a quaternion algebra over K (use Exercise 1). c) Prove that if F is commutative, then we are in one of the following cases:

$\alpha ) F = K$, and $s$ is the identity.

$\beta ) F = K\times K$, and $s(\lambda , µ) = (µ, \lambda )$.

$\gamma ) F$ is a separable quadratic extension of K, and $s$ is the nontrivial automorphism of F.

$\delta ) K$ has characteristic 2, F is an 2-radical extension of K of height 1, and $s$ is the identity.

$\P 4)$ Let $(F, s)$ be an Artinian (associative) Cayley K-algebra, and let $\mathfrak{r}$ be its radical. a) Prove that we have $x^2= 0$ and $s(x) =-x$ for every $x\in \mathfrak{r}$; the algebra $F = F/\mathfrak{r}$ is Cayley and isomorphic to one of the algebras described in Exercise 3. b) Prove that if F is a quaternion algebra over K, then $\mathfrak{r}$ is reduced to 0 (observe that we have $(ab-ba)x= 0$ for $a, b\in F,x\in \mathfrak{r})$. c) Suppose that F is commutative. Prove that $\mathfrak{r}^3$ is reduced to 0 but that $\mathfrak{r}^2$ may not be. d) Suppose that F is commutative and $\mathfrak{r}^2$ is reduced to 0. Prove that there exists an F-module V such that F is isomorphic to $F\oplus V$ endowed with the structure of a K-algebra for which we have $(\lambda , v)(µ, w) = (\lambda µ, \lambda w+s(µ)v)$. (In cases $\alpha )$ through $\gamma )$ of Exercise 3, c), use Corollary 1 of VIII, p. 245. In case $\delta )$, choose a $p$-basis $(e_i)_{i\in I}$ of F over K and for each $i\in I$, an element $f_i$ of F that lifts $e_i$, and prove that the subalgebra of F generated by the $(f_i)$ is isomorphic to F.)

$\P 5)$ Suppose that the characteristic of K is $\not= 2$. Let F be a not necessarily associative alternative Cayley K-algebra (III, Appendix, No. 2); we denote its conjugation by $s:x\mapsto x$ and its Cayley trace and norm by T and N, respectively. We say that a subalgebra E of F is nondegenerate if for every nonzero element $x$ of E, there exists an $x'\in E$ such that $T(xx')\not= 0$. a) Prove the equality $x(zy) +z(xy) = T(xz)y= (yx)z+ (yz)x$ for $x, y, z$ in F (reduce to the case $z=x)$. b) Let E be a subalgebra of F containing 1, distinct from F, stable under $s$, and finite-dimensional over K; suppose that E and F are nondegenerate. Prove that there exists a nonzero element $j$ of F such that $T(xj) = 0$ for every $x\in E$ and $N(j)\not= 0$. We have $j=-j,xj=-jx$ for every $x\in E$, and $j^2=\gamma 1_F$ with $\gamma =-N(j)$. c) Let $x$ and $y$ be elements of E. Prove the formulas $x(yj) = (yx)j= (yj)x$ and $(xj)(yj) =\gamma yx$ (use a) and Exercise 2 of III, Appendix, p. 654). d) Prove that $E + Ej$ is a nondegenerate subalgebra of F, stable under $s$, and of dimension 2 dim(E) that can be identified with the Cayley extension of $(E, s)$ defined by $\gamma$. Deduce from Proposition 3 of III, Appendix, No. 2, p. 614 that E is associative. e) Deduce from the above that the nondegenerate alternative Cayley K-algebras are the following:

(i) the K-algebra K endowed with the identity involution

(ii) the quadratic algebras over K of type $(\alpha ,0)$ with $\alpha \not= 0$

(iii) the quaternion algebras over K of type $(\alpha ,0, \gamma )$ with $\alpha \gamma \not= 0$

(iv) the octonion algebras over K of type $(\alpha ,0, \gamma , \delta )$ with $\alpha \gamma \delta \not= 0$. (Construct a sequence of Cayley extensions $K\subset E_1\subset E_2\subset  \cdots  \subset F$, and observe that an octonion algebra is not associative.) f ) Prove that an alternative Cayley K-algebra whose nonzero elements are all invertible is one of the aforementioned types. g) Let R a maximal ordered field. Prove that an alternative Cayley R-algebra whose nonzero elements are all invertible is isomorphic to R, C, H, or O (VIII, p. 368, Remark 1).

6) Let H be the quaternion field of type $(-1,0,-1)$ over $\mathbf{Q}$. a) An extension K of $\mathbf{Q}$ splits H if and only if $-1$ is the sum of two squares in K (apply Propositions 3 of VIII, p. 363 and 4 of VIII, p. 364). b) Let K be a cyclic extension of $\mathbf{Q}$ of degree $2^n$ that splits H. Prove that no proper subfield of K splits H (observe that the unique subfield of K of degree $2^{n-1}$ is the intersection of K and a maximal ordered field containing $\mathbf{Q})$. c) Let $k$ be an integer $\geqslant 1$ and $p$ a prime divisor of $2^{2^k}+ 1$. Prove that the greatest integer $n$ such that $2^n$ divides $p-1$ is $> k$ (observe that we have $2^{p-1}\equiv 1$ modulo $p)$. Let Ω be a primitive $p$-the root of 1 and $E =\mathbf{Q}(Ω)$. Prove that $-1$ is the sum

$$
\surd
$$

of two squares in E (let F be the extension E( $-1)$; show that $-1$ belongs to $N_{F/E}(F^*)$ by proving that this is true for $\omega$ and $1 +\omega^h$ and by using the identity $\prod^r_{j=0}^{-1}(1 + T^{2^j}) =\sum^2_{h^r=0}^{-1}T^h)$. d) Prove that a cyclic extension of $\mathbf{Q}$ of degree $2^n$ contained in E splits H (apply VIII, p. 283, Corollary 2).

$\P 7)$ Suppose that the characteristic of K is different from 2. a) Let D be a field containing K and F the quaternion algebra over K of type $(\alpha ,0, \gamma )$. Prove that $D\otimes_KF$ is not a field if and only if there exist two commuting elements $x$ and $y$ in D such that $x^2-\alpha y^2=\gamma$ (apply Exercise 4, c) of VIII, p. 351, first to $D\otimes_KK(i)$ and then to $D\otimes_KF)$. b) Let $F'$ be another quaternion algebra over K. Then $F\otimes_KF'$ is a field if and only if the only solution of $N_F(q) = N_{F'}(q')$, where $q\in F$ and $q'\in F'$ are pure quaternions (III, §2, p. 618, Exercise 3), is $q=q'= 0$. (Reduce to the case when F is a field and use the criterion of a). Note that if neither $x$ nor $y$ belongs to K, then $y$ belongs to $K(x)$, and write $x=s+q$, where $x\in K$ and $q$ is a pure quaternion.)

8) Let $K_0$ be a commutative field of characteristic different from 2, and let $(X_n)_{n\geqslant 1}$ and $(Y_n)_{n\geqslant 1}$ be two infinite sequences of variables and K be the field of rational fractions $K_0((X_n),(Y_n))$. For any $n\geqslant 1$, denote by $F_n$ the field of quaternions over K of type $(X_n,0,Y_n)$. a) Prove that the tensor product $F =\bigotimes_nF_n$ (III, §4, No. 5, p. 470) is a field with center K such that every subfield generated by a finite subset has finite rank over K (use Exercise 7, a)). b) Prove that if $u$ is an inner automorphism of F, then there exists a finite subset J of $\mathbf{N}$ such that the restriction of $u$ to $F_n$, for $n /\in J$, is the identity. Deduce that there exists an uncountable set of noninner automorphisms of F.

[^1]: In the case when $\beta = 0$, it is also said that F is a quaternion algebra of type $(\alpha , \gamma )$.
