---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 18
section_title: Simple Algebras over a Finite Field
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.355-A VIII.360
pdf_pages: 0372-0377
extraction: native
subsections:
    - "no": 1
      title: Polynomials over a Finite Field
      page: 355
      pdf_page: 372
    - "no": 2
      title: Simple Algebras over Finite Fields
      page: 357
      pdf_page: 374
statements: 8
exercises: 7
content_sha256: b06076ea74d4968c307b10c1909cd737ab1b315f796eba98fe11c59e5e46b063
---

## § 18. SIMPLE ALGEBRAS OVER A FINITE FIELD

### 1. Polynomials over a Finite Field

Theorem 1 (Chevalley–Warning). — Let K be a finite commutative field of characteristic $p$. Let $n$ be an integer $\geqslant 1$ and $(f_i)_{i\in I}$ a finite family of nonzero elements of $K[X_1, . . . ,X_n]$. Denote by Z the set of elements $\mathbf{x}$ of $K^n$ such that we have $f_i(\mathbf{x}) = 0$ for $i\in I$. If we have $n >\sum_{i\in I}$ deg($f_i)$, then the cardinal of Z is divisible by $p$.

#### Lemma 1 {#alg-viii-s18-lem-1 .statement}

Let L be a field, G a finite group, and $\chi$ a nontrivial homomorphism from G to the multiplicative group $L^*$. We have $\sum_{x\in G}\chi (x) = 0$.

By assumption, there exists an element $a$ of G such that $\chi (a)\not= 1$; since multiplication by $a$ is a permutation of G, we have

$$
_x\sum_{\in G}\chi (x) =_x\sum_{\in G}\chi (ax) =\chi (a)_x\sum_{\in G}\chi (x)
$$

this gives Lemma 1.

#### Lemma 2 {#alg-viii-s18-lem-2 .statement}

Let $q$ be the cardinal of K. For any integer $m\geqslant 0$, set $S_m=$ $\sum_{x\in K}x^m$. We have $S_m=-1$ if $m$ is a nonzero multiple of $q-1$ and $S_m= 0$ in all other cases.

Recall that $0^0= 1$ (I, §2, No. 1, p. 14). Suppose that $m$ is a multiple of $q-1$. Since the abelian group $K^*$ has order $q-1$, we have $x^m= 1$ for every $x\in K^*$ and $S_m= 0^m+ (q-1)\cdot 1$, which gives the assertion in this case.

Suppose that $m$ is not a multiple of $q-1$. Set $\chi (x) =x^m$ for $x\in K^*$. Since the multiplicative group $K^*$ is cyclic of order $q-1$ (V, §12, No. 1, p. 93, Proposition 1), there exists an element $a$ of $K^*$ such that $\chi (a)\not= 1$. By Lemma 1 applied to $G = K^*$, we have

$$
S_m= 0^m+_x\sum_{\in K^*}\chi (x) = 0
$$

this gives Lemma 2.

Let us now prove Theorem 1. Let $\mathbf{x}= (x_1, . . . , x_n)$ be an element of $K^n$. We have $1-f_i(\mathbf{x})^{q-1}= 0$ if $f_i(\mathbf{x})\not= 0$ and $1-f_i(\mathbf{x})^{q-1}= 1$ if $f_i(\mathbf{x}) = 0$. Set $P =\prod^r_{i=1}(1-f_i^{q-1})$. We have

1 if $\mathbf{x}\in Z$, (1) $P(\mathbf{x}) =$

0 if $\mathbf{x}\notin Z$.

Let us expand the polynomial P as $\sum_{\alpha\in\mathbf{N}^n}c_{\alpha}X^{\alpha}$; by assumption, it has degree $<(q-1)n$. Let $\alpha$ be an element of $\mathbf{N}^n$ such that $c_{\alpha}$ is nonzero. Since we have $\alpha_1+\cdots +\alpha_n<(q-1)n$, there exists an integer $`$ such that $1\leqslant `\leqslant n$ and $0\leqslant \alpha_`< q-1$. By Lemma 2, we then have $\sum_{x\in K}x^{\alpha_`}= 0$, and therefore

$n$

$$
_{\mathbf{x}}\sum_{\in K^n}\mathbf{x}^{\alpha}=_j\prod_{=1}(\sum_{x\in K}x^{\alpha_j}= 0
$$

We consequently have

$$
_{\mathbf{x}}\sum_{\in K^n}P(\mathbf{x}) =_{\alpha}\sum_{\in\mathbf{N}^n}c_{\alpha}(\sum_{\mathbf{x}\in K^n}\mathbf{x}^{\alpha}= 0
$$

Now, by formula (1), we have $\sum_{\mathbf{x}\in K^n}P(\mathbf{x}) =$ Card(Z) $\cdot 1$, and therefore Card(Z) $\cdot 1 = 0$, which means that Card(Z) is divisible by $p$.

#### Corollary {#alg-viii-s18-n1-cor-1 .statement}

Let V be a vector space of finite dimension $n$ over K and I a finite set, and for each $i\in I$, let $F_i: V\rightarrow K$ be a homogeneous polynomial mapping of degree $d_i>0$. If we have $\sum_{i\in I}d_i< n$, then there exists a nonzero element $x$ of V such that $F_i(x) = 0$ for every $i\in I$.

Let $(e_1, . . . , e_n)$ be a basis of V over K. By the definition of homogeneous polynomial mappings (IV, §5, No. 9, p. 55, Definition 3), for every $i\in I$, there exists a homogeneous polynomial $f_i$ in $K[X_1, . . . ,X_n]$ of degree $d_i$ such that we have $F_i(\xi_1e_1, . . . , \xi_ne_n) =f_i(\xi_1, . . . , \xi_n)$. Let Z be the set of elements $x$ of V such that $F_i(x) = 0$ for every $i\in I$. By Theorem 1, the cardinal of Z is divisible by $p$, and since 0 belongs to S, we have Card(Z) $\geqslant p >1$.

### 2. Simple Algebras over Finite Fields

Theorem 2 (Wedderburn). — Every finite field is commutative.

Let D be a finite field, and let K be its center. The K-algebra D is central simple of degree $m^2$, where $m$ is a strictly positive integer. The reduced norm is a homogeneous polynomial mapping Nrd$: D\rightarrow K$ of degree $m$ (VIII, p. 345, Proposition 6), and we have Nrd($a)\not= 0$ for every $a\not= 0$ in D (VIII, p. 340, Proposition 3). The corollary above implies that $m\geqslant m^2$, and therefore $m= 1$. So we have D = K.

#### Corollary 1 {#alg-viii-s18-lem-2-cor-1 .statement}

Every finite simple ring is isomorphic to a matrix ring $\mathbf{M}_n(L)$, where $n$ is a strictly positive integer and L is a finite commutative field.

This follows from Theorem 2 and the structure theorem for simple rings (VIII, p. 120, Theorem 1).

#### Corollary 2 {#alg-viii-s18-lem-2-cor-2 .statement}

Let K be a finite commutative field. Every central simple algebra over K is isomorphic to a matrix algebra $\mathbf{M}_n(K)$, where $n$ is a strictly positive integer.

This follows from Theorem 2 and the structure theorem for central simple algebras (VIII, p. 252, Theorem 1).

#### Remark 1 {#alg-viii-s18-n2-rem-1 .statement}

Here is another proof of Theorem 2. Let D be a finite field, let K be its center, and let L be a maximal commutative subfield of D. Let $x$ be an element of $D^*$. It belongs to a maximal commutative subfield $L_1$ of D. We have the equality

$$
[D : K] = [L : K]^2= [L_1: K]^2
$$

by Corollary 2 of VIII, p. 265, and therefore $[L : K] = [L_1: K]$. By Proposition 3 of V, §12, No. 2, p. 94, the extensions L and $L_1$ of K are isomorphic. By VIII, p. 263, Corollary, there exists an element $a$ of $D^*$ such that $aLa^{-1}= L_1$, so $a^{-1}xa$ belongs to L. We then have $(ay)^{-1}x(ay) =a^{-1}xa$ for every $y\in L^*$. Consequently, if S is a set of representatives of the left cosets of $D^*$ modulo $L^*$, then every element of $D^*\{1\}$ can be written as $sxs^{-1}$ with $s\in S$ and $x\in L^*\{1\}$. We denote the order of $D^*$ by $d$ and that of $L^*$ by $`$. Since the cardinal of S is equal to $d/`$, we have $d-1\leqslant (d/`)(`-1) =d-d/`$. It follows that $`=d$, and therefore L = D, which proves that the field D is commutative.

#### Remark 2 {#alg-viii-s18-n2-rem-2 .statement}

Let L be a commutative field with the following property: $(C_1)$ Let V be a vector space of finite dimension $n$ over the field L, and let $d$ be such that $0< d < n$. For every homogeneous polynomial mapping $F : V\rightarrow L$ of degree $d$, there exists a nonzero element $x$ of V such that $F(x) = 0$.

The proof of Theorem 2 shows that every field of finite degree over L with center L is equal to L.

By the corollary of VIII, p. 356, every finite field has property $(C_1)$. We can prove (VIII, p. 360, Exercise 7) that the following fields have property $(C_1):$ – every algebraic extension of a finite field – every field of rational fractions in one variable with coefficients in an algebraically closed field (Tsen’s theorem). – $*$every field endowed with a discrete valuation for which it is complete and

whose residue field is algebraically closed (VIII, p. 332, Exercise 17$).*$

#### Remark 3 {#alg-viii-s18-n2-rem-3 .statement}

Suppose that the field K satisfies the following condition: – If L is an extension of K of finite degree, then it is cyclic and the norm mapping $N : L^*\rightarrow K^*$ is surjective. This condition is satisfied, in particular, when the field K is finite (V, §12, No. 2, p. 95, Proposition 4). We can then prove that every field of finite degree over K with center K is equal to K (Exercise 10 of VIII, p. 329).

### Exercises {#alg-viii-s18-exercises}

1) Let D be a field. a) Let E be a proper subfield of D whose multiplicative group $E^*$ has finite index in $D^*$. Prove that D is finite (for a sequence $(a_n)$ of distinct elements of E and an element $x$ of D E, consider the classes mod $E^*$ of the elements $x+a_n)$. b) Prove that an element of D that has only finitely many conjugates belongs to the center Z of D (apply a) to the commutant of this element in D, which is a field). c) Deduce that a polynomial in Z[X] that has a root in D Z has infinitely many roots in D Z.

$\P 2)$ Let A be a K-algebra and $m$ an integer. Suppose that every element of A is algebraic of degree $\leqslant m$ over K. a) Prove that if A is a primitive ring, then there exist an integer $r\leqslant m$ and a field D whose elements all have degree $\leqslant m$ over K such that A is isomorphic to the matrix algebra $\mathbf{M}_r(D)$. (If A is not simple, then deduce from the density theorem that for every integer $n$, there exist a subalgebra $A_n$ of A and a surjective homomorphism $A_n\rightarrow \mathbf{M}_n(D)$. Observe that the algebra $\mathbf{M}_n(D)$ contains elements X such that $X^{n-1}\not= 0$ and $X^n= 0.)$ b) Suppose that the field K is infinite. Prove that the algebra $A/\mathfrak{R}(A)$ is semisimple and admits at most $m$ simple components (observe that the algebra $K^n$ contains elements of degree $n$ over K; deduce that A admits at most $m$ maximal two-sided ideals, and conclude using a)). Prove that if K is, moreover, perfect, then $A/\mathfrak{R}(A)$ has finite rank over K.

$\P 3)$ Let K be a commutative field. We say that a K-algebra A is algebraic if all its elements are algebraic over K. Every algebra of finite rank is algebraic; every subalgebra and quotient algebra of an algebraic algebra is algebraic. The radical of an algebraic K-algebra is a nil ideal (VIII, p. 166, Exercise 5). a) Prove that an algebraic algebra is a pseudoregular ring (VIII, p. 178, Exercise 4; observe that for every $x\in A$, there exist an element $y\in K[x]$ and an integer $k$ such that $x^k=x^{k+1}y)$. b) Let A be an algebraic K-algebra without any nilpotent elements other than 0. Prove that A is isomorphic to a subalgebra of a product of fields. (Observe that every quotient algebra of A has the same properties. Prove that if A is primitive, then it is a field, by reasoning as in Exercise 2, a). In the general case, use Exercise 12 of VIII, p. 168.)

$\P 4)$ Let K be a finite field and A an algebraic K-algebra (Exercise 3). a) Suppose that A is a field. Prove that A is commutative. (Let $x$ be a noncentral element of A. Consider the field $Z(x)$, where Z is the center of A, and prove that there exists an element $y\in A$ such that $yxy^{-1}=x^r$, with $x^r\not=x$. Deduce a contradiction by considering the subfield $K(x, y)$ of A.) b) Suppose that A does not contain any nonzero nilpotent element. Prove that the algebra A is commutative (use a) and Exercise 3).

5) Let K be a finite field, $m$ an integer, and A a K-algebra without radical whose elements all have degree $\leqslant m$. Prove that there exists a finite extension L of K such that A is isomorphic to a subalgebra of a product $(\mathbf{M}_r(L))^I$ whose projections are simple algebras (cf. Exercise 2, a)). Also prove the converse.

6) Let A be a ring such that for every $a\in A$, there exists an integer $n(a)>1$ such that $a^{n(a)}=a$. Prove that A is isomorphic to a product of finitely many reduced commutative algebraic algebras over finite fields. (Observe that A is annihilated by an integer $n$, and then that for every prime number $p$, the $p$-component $A_p$ of the additive group A is a two-sided ideal annihilated by $p$. Apply Exercise 4, b).) Also prove the converse.

7) a) Prove that if the field K has property $(C_1)$ (VIII, p. 357), then so does every algebraic extension of K. (Reduce to the case of an extension L of K of finite degree $r$. Prove that if F is a homogeneous polynomial function of degree $d$ on an L-vector space V, then the function $N_{L/K}\circ F$ is homogeneous polynomial of degree $rd$ on the K-vector space V.) $*$b) Assume from now on that K is algebraically closed. Let $F_1, . . . ,F_n$ be homogeneous polynomials of degree $>0$ in $m$ variables. Prove that if $n < m$, then there exists an $\mathbf{a}\not= 0$ in $K^n$ such that $F_1(\mathbf{a}) =\cdots = F_n(\mathbf{a}) = 0$ (use AC, VIII, §2, n$^o4$, p. 19, corollaire 1 du théorème 3 and AC, VIII, §3, n$^o1$, p. 24, proposition 2). c) Deduce from b) that the field K(X) has property $(C_1)$.

(Let $f$ be a homogeneous polynomial of degree $d$ in $n$ variables whose coefficients are polynomial in X, and let $\nu$ be the maximum of the degrees of these coefficients. Let N be an integer, and let $G_1, . . . ,G_n$ be polynomials in X of degree $\leqslant N$. Prove that the equality $F(G_1(X), . . . ,G_n(X)) = 0$ is equivalent to the annihilation of $Nd+\nu + 1$ homogeneous polynomials of degree $>0$ in the $n(N + 1)$ coefficients of the $G_i.)$ d) Deduce from a) and c) that an extension of an algebraically closed field of transcendence degree $\leqslant 1$ has property $(C_1)$ (“Tsen’s theorem”).$*$
