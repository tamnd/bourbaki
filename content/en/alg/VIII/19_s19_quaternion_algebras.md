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
statements: 16
exercises: 8
content_sha256: b5996028b55144473fe8f797e1f0ef1f96e74a63697ee6e4b018df44f20f01cd
---

## § 19. QUATERNION ALGEBRAS

In this section, K is a commutative field.

### 1. General Properties of Quaternion Algebras

Let $\alpha , \beta , \gamma$ be elements of K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$. Recall (III, §2, No. 5, p. 445)[^1] that F is an associative unital K-algebra that has a basis $(1, i, j, k)$ over K satisfying the relations

$$
i^2=\alpha +\beta i ,j^2=\gamma  ,ij=k ,ji=\beta j-k \tag{1}
$$

It is a Cayley algebra (III, §2, No. 4, p. 441, Definition 1) whose conjugation satisfies

$$
\overline{i}=\beta -i ,\overline{j}=-j ,\overline{k}=-k \tag{2}
$$

Recall that the Cayley trace and norm of F are the mappings $T_F$ and $N_F$ from F to K defined by $T_F(q) =q+\overline{q}$ and $N_F(q) =qq$.

The linear subspace E of F with basis $(1, i)$ is a commutative Cayley subalgebra of F; it is a quadratic algebra of type $(\alpha , \beta )$, and F can be identified with the Cayley extension of E defined by $\gamma$ (III, §2, No. 5, p. 444). For every $z\in E$, we have $zj=jz$. Every element $q$ of F can be written uniquely as $x+jy$ with $x, y\in E$, and we have

$$
\overline{q}=\overline{x}-jy ,T_F(q) =x+x ,N_F(q) =xx-\gamma yy \tag{3}
$$

#### Proposition 1 {#alg-viii-s19-prop-1 .statement tag=00LQ}

The characteristic polynomial of an element $q$ of F is equal to $X^2-T_F(q)X + N_F(q)^2$.

By the above, the algebra F is a free right E-module with basis $(1, j)$. Consequently, F[X] is a free right E[X]-module with basis $(1, j)$. We denote by $u$ the endomorphism of the right E[X]-module F[X] defined by $u(P) =$ $(X-q)P$ for $P\in F[X]$. The characteristic polynomial of $q$ is the determinant of $u$ viewed as an endomorphism of the K[X]-module F[X]. By Proposition 6 of III, §9, No. 4, p. 546, it is equal to N(det $u)$, where N denotes the norm from E[X] to K[X]. Let us write $q$ as $x+jy$ with $x, y\in E$. The matrix of $u$ with respect to the basis $(1, j)$ is $^X_-^-_y^x_X^-_-^{\gamma y}_{\overline{\overline{x}}}$ ; its determinant is equal to $D = (X-x)(X-\overline{x})-\gamma yy= X^2-T_F(q)X + N_F(q)$ (cf. formula (3)). Since D belongs to K[X], we have $N(D) = D^2$; Proposition 1 follows.

#### Remark 1 {#alg-viii-s19-n1-rem-1 .statement tag=00LR}

Suppose that the characteristic of K is different from 2, and set $i'= 2i-\beta$. Then $(1, i')$ is a basis of E over K, and we have ${i'}^2= 4\alpha +\beta^2$. It follows that E is isomorphic to the quadratic algebra of type $(4\alpha +\beta^2,0)$ and F to the quaternion algebra of type $(4\alpha +\beta^2,0, \gamma )$.

#### Remark 2 {#alg-viii-s19-n1-rem-2 .statement tag=00LS}

The quaternion algebra of type $(\alpha ,0, \gamma )$ is isomorphic to the quaternion algebra of type $(\gamma ,0, \alpha )$ (III, §2, No. 5, p. 445). It is also isomorphic to the quaternion algebra of type $(\alpha a^2,0, \gamma c^2)$ for every pair $(a, c)$ of nonzero elements of K.

#### Remark 3 {#alg-viii-s19-n1-rem-3 .statement tag=00LT}

Let $q$ be an element of F. Then $q$ is nilpotent if and only if its characteristic polynomial is equal to $X^4$, that is, $T_F(q) = N_F(q) = 0$; we then have $q^2= 0$.

#### Example {#alg-viii-s19-n1-exa-1 .statement tag=00LU}

The matrix algebra $\mathbf{M}_2(K)$ is isomorphic to the quaternion algebra of type $(0,1,1)$. Indeed, consider the quadratic algebra $E = K\times K$ (of type $(0,1))$ and the quaternion algebra $F = E + Ej$, which is the Cayley extension of E defined by the element $\gamma = 1$. The mapping $(a, b)\mapsto (^a_0^0_b)$ is an algebra homomorphism from E to $\mathbf{M}_2(K)$. Since for $a, b$ in K, we have

$$
(01)((01)(10)(01)((a0)(b0)((01)
$$

=, =,

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0

this homomorphism extends to an algebra homomorphism $\theta : F\longrightarrow \mathbf{M}_2(K)$ defined by

$$
(ac)
$$

$\theta (a, b) + (c, d)j$ =.

$$
db
$$

This homomorphism is bijective. When the characteristic of K is different from 2, the algebra $\mathbf{M}_2(K)$ is also isomorphic to the quaternion algebra of type $(1,0,1)$ (Remark 1).

### 2. The Center of a Quaternion Algebra

Let $\alpha ,\beta ,\gamma$ be elements of K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$.

#### Proposition 2 {#alg-viii-s19-prop-2 .statement tag=00LV}

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

#### Proposition 3 {#alg-viii-s19-prop-3 .statement tag=00LW}

Let $\alpha ,\beta ,\gamma$ be elements of K, and let $f$ be a quaternion algebra of type $(\alpha , \beta , \gamma )$. Denote its Cayley trace and norm by $T_F$ and $N_F$. The following properties are equivalent:

(i) The algebra F is central simple.

(ii) For every nonzero element $x$ of F, there exists an element $y$ in F such that $T_F(xy)\not= 0$.

(iii) We have $(4\alpha +\beta^2)\gamma \not= 0$.

Suppose that these properties hold. Then for every $x$ in F, the reduced characteristic polynomial of $x$ is $X^2-T_F(x)X + N_F(x)$. In particular, $T_F(x)$ is the reduced trace of $x$, and $N_F(x)$ is its reduced norm.

(i)$\Rightarrow$(ii): If the algebra F is central simple, then it follows from Proposition 1 of VIII, p. 361 and the definition of the reduced trace (VIII, p. 340, Definition 2) that $T_F$ is its reduced trace; assertion (ii) follows (VIII, p. 343, Proposition 5).

(ii)$\Leftrightarrow$(iii): Let $(e_i)_{1\leqslant i\leqslant 4}$ be a basis of F of type $(\alpha , \beta , \gamma )$ (III, §2, No. 5, p. 445). The matrix $(T_F(e_ie_j))$ is equal to

2 $\beta$ 0 0

$\beta 2\alpha +\beta^2$ 0 0

.

0 0 $2\gamma \beta \gamma$

0 0 $\beta \gamma -2\alpha \gamma$

Its determinant is $-\gamma^2(4\alpha +\beta^2)^2$. The equivalence of properties (ii) and (iii) follows from V, §8, No. 2, p. 49, Lemma 1.

(iii)$\Rightarrow$(i): Suppose $(4\alpha +\beta^2)\gamma \not= 0$. We then have $\gamma \not= 0$, and we have $\beta \not= 0$ if K has characteristic 2. By Proposition 2, the algebra F is central. Let $x$ be an element of the Jacobson radical of F. For every $y\in F,xy$ is nilpotent, so $T_F(xy) = 0$ (Remark 3 of VIII, p. 362). Since (ii) is equivalent to (iii), we have $x= 0$. This proves that F is a semisimple K-algebra. Since its center is K, it is simple.

The last assertion follows from Proposition 1 of VIII, p. 361 and the definition of the reduced characteristic polynomial (VIII, p. 340, Definition 1).

Denote the characteristic of K by $p$. By Proposition 3, if $p\not= 2$, then every quaternion algebra over K of type $(\alpha ,0, \gamma )$ with $\alpha$ and $\gamma$ in $K^*$ is central simple. If $p= 2$, then every quaternion algebra of type $(\alpha ,1, \gamma )$ with $\alpha \in K$ and $\gamma \in K^*$ is central simple. Conversely, we have the following.

#### Proposition 4 {#alg-viii-s19-prop-4 .statement tag=00LX}

Let A be a central simple algebra of degree 4 over K. Denote the characteristic of K by $p$.

a) If $p\not= 2$, then there exist nonzero elements $\alpha$ and $\gamma$ of K such that the algebra A is isomorphic to the quaternion algebra of type $(\alpha ,0, \gamma )$.

b) If $p= 2$, then there exist an element $\alpha$ of K and an element $\gamma$ of $K^*$ such that the algebra A is isomorphic to the quaternion algebra of type $(\alpha ,1, \gamma )$.

By Wedderburn’s theorem (VIII, p. 120, Theorem 1), there exist an integer $r\geqslant 1$ and a field D with center K such that A is isomorphic to $\mathbf{M}_r(D)$. We then have $r^2[D : K] = [A : K] = 4$. If $r= 2$, then A is isomorphic to $\mathbf{M}_2$(K), and Proposition 4 follows from the example of VIII, p. 362. Otherwise, we have $r= 1$, and A is a field with center K. It then has a maximal commutative subfield E that is a separable extension of K; since A has degree 4 over K, the extension E has degree 2 over K (VIII, p. 265, Corollary 2). It is therefore quadratic (III, §2, No. 3, p. 439). Let $s$ be the conjugation of E (III, §2, No. 3, p. 440). By the Skolem–Noether theorem (VIII, p. 256, Corollary 1), there exists an invertible element $j$ of A such that we have $s(x) =jxj^{-1}$ for every $x$ in E. The field E is separable over K, so we have $s\not=$ Id$_E$, so that $j /\in E$. Since A is a vector space of dimension 4 over K, it is a left vector space of dimension 2 over E, so we have $A = E\oplus Ej$. We have $s^2=$ Id$_E$, so the element $j^2$ of A belongs to the center of A; hence there exists an element $\gamma$ of $K^*$ such that $j^2=\gamma$.

When $p\not= 2$, there exist an element $i$ of E and an element $\alpha \in K^*$ such that $E = K(i)$ and $i^2=\alpha$ (V, §11, No. 9, p. 93, Example 3); in this case, A is isomorphic to the quaternion algebra of type $(\alpha ,0, \gamma )$. When $p= 2$, there exist an element $i$ of E and an element $\alpha$ of K such that $E = K(i)$ and $i^2=i+\alpha$ (V, §11, No. 9, p. 93, Example 2), so that A is isomorphic to the quaternion algebra of type $(\alpha ,1, \gamma )$.

#### Corollary 1 {#alg-viii-s19-prop-4-cor-1 .statement tag=00LY}

Let A be a central simple K-algebra of finite degree $>1$ whose elements are all algebraic of degree $\leqslant 2$ over K. Then A is isomorphic to a quaternion algebra over K.

If K is finite, then the algebra A is isomorphic to a matrix algebra $\mathbf{M}_n(K)$ (VIII, p. 357, Corollary 2) and therefore contains elements of degree $n$ over K; the assumption implies $n= 2$ and therefore the result in this case (VIII, p. 362, Example). Suppose that the field K is infinite. Let L be a maximal étale subalgebra of A. By V, §7, No. 4, p. 41, Proposition 7, there exists an element $x$ of A such that the K-algebra L is equal to $K[x]$, hence by assumption has degree $\leqslant 2$. Since we have $[A : K] = [L : K]^2$ (VIII, p. 264, Proposition 4 and p. 262, Proposition 3), we conclude that [A : K] = 4. Corollary 1 then follows from Proposition 4.

#### Corollary 2 {#alg-viii-s19-prop-4-cor-2 .statement tag=00LZ}

Let $(E, s)$ be a Cayley algebra over K such that the K-algebra E is central simple of finite degree $>1$ over K. Then E is isomorphic to a quaternion algebra over K.

Every element $u$ of E satisfies $u^2-T_E(u)u+ N_E(u) = 0$, so the K-algebra E is isomorphic to a quaternion algebra (Corollary 1).

### 4. Criteria for a Quaternion Algebra to Be a Field

Let $\alpha , \beta , \gamma$ be elements of the field K, and let F be the quaternion algebra of type $(\alpha , \beta , \gamma )$. As in No.1, we denote the canonical basis of F by $(1, i, j, k)$ and the subalgebra $K + Ki$ of F by E.

#### Proposition 5 {#alg-viii-s19-prop-5 .statement tag=00M0}

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

Finally, suppose that property (vi) holds. Let $q$ be a nonzero element of F; we write it as $u+vj$ with $u$ and $v$ in E. If $v$ is zero, then $q$ is invertible. If $v$ is not zero, then we have $N_F(q) = N_F(v)N_F(v^{-1}u+j) =$ $N_{E/K}(v) N_{E/K}(v^{-1}u)-\gamma$ by III, §2, No. 5, p. 443, formula (24). Since $\gamma$ is not a norm, $N_F(q)$ is not zero, and $q$ is invertible.

#### Remark {#alg-viii-s19-n4-rem-1 .statement tag=00RQ}

Suppose that the quaternion algebra F is a field. It follows from the equality $j^2=\gamma$ that we have $\gamma \not= 0$. By Proposition 2 of VIII, p. 363, the center of F is equal to K unless K has characteristic 2 and $\beta$ is zero, in which case the algebra F is commutative.

### 5. Algebras over Maximal Ordered Fields

Let R be a maximal ordered field (VI, §2, No. 5, p. 25). Let C be the quadratic R-algebra of type $(-1,0)$; if $(1, i)$ is its canonical basis, then we have $i^2=-1$. Moreover, C is an algebraic closure of R (VI, §2, No. 6, p. 26, Theorem 3). Let H be the quaternion R-algebra of type $(-1,0,-1)$. The multiplication table of H in its canonical basis $(1, i, j, k)$ is given by

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j ,jk=-kj=i
$$

We identify C with the subalgebra $R + Ri$ of H. The conjugate of an element $q=x+yi+zj+tk$ of H is $\overline{q}=x-yi-zj-tk$. The Cayley trace and norm of $q$ are given by

$$
T(q) =q+\overline{q}= 2x ,N(q) =qq=x^2+y^2+z^2+t^2
$$

Since R is an ordered field, we have $N(q)>0$ if $q\not= 0$, so H is a field, with center R (VIII, p. 363, Proposition 2). The reduced trace and norm of an element $q$ of H are $T(q)$ and $N(q)$, respectively.

#### Theorem 1 {#alg-viii-s19-thm-1 .statement tag=00M1}

Let D be an R-algebra of finite degree that is a field. Then D is isomorphic to R, C, or H.

Denote the center of D by Z, and let L be a maximal commutative subfield of D. We have $[D : Z] = [L : Z]^2$ by VIII, p. 265, Corollary 2; we also have $[L : R]\leqslant 2$ because C is an algebraic closure of R. There are consequently three possible cases:

a) We have R = Z = L, so [D : Z] = 1 and D = R.

b) We have $R\not= Z$ and Z = L, so [D : Z] = 1 and D = L. In this case, D is isomorphic to C.

c) We have R = Z and [L : R] = 2, so [D : R] = 4. By Proposition 4 of VIII, p. 364, the R-algebra D is isomorphic to a quaternion algebra of type $(\alpha ,0, \gamma )$, where $\alpha$ and $\gamma$ are nonzero elements of R. Let $i\in D$- Z be such that $i^2=\alpha$. We have $\alpha \not= 0$. If $\alpha  >0$, then there exists an $a\in R$ such that $a^2=\alpha$ (VI, §2, No. 6, p. 26, Theorem 3); we then have $(a-i)(a+i) = 0$, which is absurd because D is a field. So we have $\alpha  <0$. The inequality $\gamma  <0$ is shown analogously. There then exist elements $a$ and $c$ of $R^*$ such that $\alpha =-a^2$ and $\gamma =-c^2$ (loc. cit.). The algebra D is therefore isomorphic to the quaternion algebra of type $(-1,0,-1)$ (VIII, p. 362, Remark 2), that is, to H.

#### Remark 1 {#alg-viii-s19-n5-rem-1 .statement tag=00M2}

Let O be the octonion algebra of type $(-1,0,-1,-1)$ over R (III, Appendix, No. 3, p. 615). Let D be an alternative Cayley algebra over R such that every nonzero element of D has an inverse. We can prove (VIII, p. 370, Exercise 5) that D is isomorphic to R, C, H, or O.

#### Remark 2 {#alg-viii-s19-n5-rem-2 .statement tag=00M3}

The above applies to the field $\mathbf{R}$ of real numbers. Every $\mathbf{R}$-algebra of finite degree that is a field is isomorphic to $\mathbf{R},\mathbf{C}$, or $\mathbf{H}$.

#### Remark 3 {#alg-viii-s19-n5-rem-3 .statement tag=00M4}

Let A be a normed algebra over the field $\mathbf{R}$. Suppose that A is a field. Then A is isomorphic to $\mathbf{R},\mathbf{C}$, or $\mathbf{H}$ (“Gelfand–Mazur theorem”) (cf. Comm. Alg., VI, §6, No. 4, p. 407, Theorem 1 and TS, I, §2, n$^o5$, p. 26, corollaire $2).*$

### Exercises {#alg-viii-s19-exercises}

See the [exercises for § 19](exercises/s19/).

[^1]: In the case when $\beta = 0$, it is also said that F is a quaternion algebra of type $(\alpha , \gamma )$.
