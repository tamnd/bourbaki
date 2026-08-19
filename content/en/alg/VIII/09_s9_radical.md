---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 9
section_title: Radical
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.151-A VIII.172
pdf_pages: 0168-0189
extraction: native
subsections:
    - "no": 1
      title: The Radical of a Module
      page: 151
      pdf_page: 168
    - "no": 2
      title: The Radical of a Ring
      page: 154
      pdf_page: 171
    - "no": 3
      title: Nakayama’s Lemma
      page: 158
      pdf_page: 175
    - "no": 4
      title: Lifts of Idempotents
      page: 159
      pdf_page: 176
    - "no": 5
      title: Projective Cover of a Module
      page: 161
      pdf_page: 178
statements: 49
exercises: 31
content_sha256: 89095724e574bba079cd13ef874a02941adc59513c6a22e5a09bd9f01b4fa6cc
---

## § 9. RADICAL

### 1. The Radical of a Module

#### Definition 1 {#alg-viii-s9-def-1 .statement tag=00A1}

Let A be a ring. The radical of an A-module M is the submodule defined as the intersection of the maximal submodules of M (VIII, p. 48, Definition 2) or, equivalently, the set of elements of M annihilated by every homomorphism from M to a simple A-module.

In the remainder of this chapter, we denote the radical of an A-module M by $\mathfrak{R}_A(M)$ or simply $\mathfrak{R}(M)$.

Let A be a ring. The radical of an A-module M is reduced to 0 (in which case we say, by abuse of language, that M is without radical) if and only if there exist a family $(S_i)_{i\in I}$ of simple A-modules and a family $(f_i)_{i\in I}$ of A-linear mappings $f_i: M\rightarrow S_i$ such that we have $\cap_{i\in I}$ Ker($f_i$) $= 0$. This is equivalent to M being isomorphic to a submodule of a product of simple A-modules.

#### Example 1 {#alg-viii-s9-n1-exa-1 .statement tag=00A2}

Let $\mathfrak{a}$ be a left ideal of A. The radical of the A-module $A_s/\mathfrak{a}$ is equal to $\mathfrak{a}'/\mathfrak{a}$, where $\mathfrak{a}'$ is the intersection of the maximal left ideals of A containing $\mathfrak{a}$. In particular, the radical of the $\mathbf{Z}$-module $\mathbf{Z}$ is reduced to 0, and that of the $\mathbf{Z}$-module $\mathbf{Z}/p^n\mathbf{Z}$ is equal to $p\mathbf{Z}/p^n\mathbf{Z}$ for every prime number $p$ and every integer $n\geqslant 1$.

#### Example 2 {#alg-viii-s9-n1-exa-2 .statement tag=00A3}

Let A be a principal ideal domain that is not a field, and let K be its field of fractions. As a K-module, K is without radical. Let us prove that the radical of K, viewed as an A-module, is equal to K; equivalently, we must prove that every A-linear mapping $f$ from K to a simple A-module S is zero. By VII, §4, No. 8, p. 25, we may assume that S is equal to $A/(\pi )$, where $\pi$ is an irreducible element of A. We have $f(x) =f(\pi \frac{x}{\pi})=\pi f(\frac{x}{\pi})= 0$ for every $x\in K$ because $\pi S = 0$.

#### Proposition 1 {#alg-viii-s9-prop-1 .statement tag=00A4}

Let M and N be A-modules and $f$ a homomorphism from M to N. We have $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$, and we even have equality if $f$ is surjective and the kernel of $f$ is contained in the radical of M.

Let $g$ be a homomorphism from N to a simple A-module; then $\mathfrak{R}(M)$ is contained in the kernel of $g\circ f$, so that $f(\mathfrak{R}(M))$ is contained in the kernel of $g$. We therefore have $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$. Now suppose that $f$ is surjective and that its kernel is contained in $\mathfrak{R}(M)$. Let $y$ be an element of $\mathfrak{R}$(N), and let $x$ be an element of the inverse image of $y$. If $g$ is a homomorphism from M to a simple A-module S, then its kernel contains the radical of M, hence the kernel of $f$. Since the homomorphism $f$ is surjective, there exists a homomorphism $h$ from N to S such that $g=h\circ f$. Since $y=f(x)$ belongs to $\mathfrak{R}$(N), we have $h(f(x)) = 0$, that is, $g(x) = 0$; thus $x$ belongs to $\mathfrak{R}$(M), which proves the inclusion $\mathfrak{R}(N)\subset f(\mathfrak{R}(M))$.

#### Corollary 1 {#alg-viii-s9-prop-1-cor-1 .statement tag=00A5}

Let M be an A-module and N a submodule of M.

a) We have $\mathfrak{R}(N)\subset \mathfrak{R}(M)\cap N$.

b) We have $(\mathfrak{R}(M) + N)/N\subset \mathfrak{R}(M/N)$. If N is contained in $\mathfrak{R}(M)$, then we have the equality $\mathfrak{R}(M/N) =\mathfrak{R}(M)/N$.

c) The module $M/\mathfrak{R}(M)$ is without radical. If the module $M/N$ is without radical, then we have $\mathfrak{R}(M)\subset N$.

Assertion a) follows from Proposition 1 applied to the canonical injection from N to M, and assertion b) follows from Proposition 1 applied to the canonical mapping from M to $M/N$. From b), we deduce that $M/N$ is without radical if $N =\mathfrak{R}(M)$ and that we have $\mathfrak{R}(M)\subset N$ if $M/N$ is without radical.

It follows from Example 1 that there can exist submodules N containing $\mathfrak{R}(M)$ such that the radical of $M/N$ is not zero.

#### Corollary 2 {#alg-viii-s9-prop-1-cor-2 .statement tag=00A6}

Let $(M_i)_{i\in I}$ be a family of A-modules, P its product, and S its direct sum. We have $\mathfrak{R}(P)\subset \prod_{i\in I}\mathfrak{R}(M_i)$ and $\mathfrak{R}(S) =\bigoplus_{i\in I}\mathfrak{R}(M_i)$.

For $i\in I$, let $\pi_i$ be the projection with index $i$ from P to $M_i$. By Proposition 1, we have $\pi_i(\mathfrak{R}(P))\subset \mathfrak{R}(M_i)$ for every $i\in I$; this proves the first assertion. We have $S\subset P$, hence

$$
\mathfrak{R}(S)\subset S\cap \mathfrak{R}(P)\subset S\cap \prod_{i\in I}\mathfrak{R}(M_i) =\bigoplus_{i\in I}\mathfrak{R}(M_i)
$$

Moreover, we have $M_i\subset S$ and therefore $\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$ for every $i\in I$, and consequently $\oplus_{i\in I}\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$.

There exist families of modules such that the radical of the product is not isomorphic to the product of the radicals (Exercise 3 of VIII, p. 166).

#### Proposition 2 {#alg-viii-s9-prop-2 .statement tag=00A7}

Let M be a finitely generated A-module.

a) If M is not reduced to 0, then we have $\mathfrak{R}(M)\not= M$.

b) If N is a submodule of M such that $N +\mathfrak{R}(M) = M$, then we have N = M.

Let N be a proper submodule of M. By Proposition 3 of VIII, p. 49, there exists a maximal submodule L of M containing N. We have $N +\mathfrak{R}(M)\subset L$, and a fortiori $N +\mathfrak{R}(M)\not= M$. This proves b); the specific case N = 0 gives assertion a).

#### Corollary {#alg-viii-s9-n1-cor-1 .statement tag=00A8}

Let M be an A-module, $(x_i)_{i\in I}$ a generating family of M, and $x$ an element of M. The following properties are equivalent:

(i) We have $x\in \mathfrak{R}(M)$.

(ii) Every submodule N of M such that $N + Ax= M$ is equal to M.

(iii) For every family $(a_i)_{i\in I}$ of elements of A, the family $(x_i+a_ix)_{i\in I}$ generates the A-module M.

(i) $\Rightarrow$ (ii): Suppose that $x$ belongs to $\mathfrak{R}(M)$. Let N be a submodule of M such that $N + Ax= M$. We have $N +\mathfrak{R}(M) = M$; hence the A-module $M/N$ is equal to its radical (Corollary 1, b) of Proposition 1). Since it is monogenous, it is zero (Proposition 2), and we have M = N.

(ii) $\Rightarrow$ (iii): Let $(a_i)_{i\in I}$ be a family of elements of A. Denote by N the submodule of M generated by the family $(x_i+a_ix)_{i\in I}$. We have $x_i\in N + Ax$ for every $i\in I$, hence $N + Ax= M$. If property (ii) holds, then N is equal to M.

(iii) $\Rightarrow$ (i): Suppose that $x$ does not belong to $\mathfrak{R}(M)$. Then there exists a maximal submodule N of M that does not contain $x$. Since N is maximal, we have $N + Ax= M$; each of the elements $x_i$ can therefore be written as $y_i-a_ix$ with $y_i\in N$ and $a_i\in A$. The family $(x_i+a_ix)_{i\in I}$ is contained in N, hence does not generate M.

#### Proposition 3 {#alg-viii-s9-prop-3 .statement tag=00A9}

a) A semisimple module is without radical.

b) A module is semisimple and finitely generated if and only if it is without radical and Artinian.

By definition, the radical of a simple module is reduced to 0. If the module M is semisimple, then it is the direct sum of a family $(S_i)_{i\in I}$ of simple submodules, and we have $\mathfrak{R}(M) =\bigoplus_{i\in I}\mathfrak{R}(S_i)$ by Corollary 2 of Proposition 1 above, hence $\mathfrak{R}(M) = 0$.

If, moreover, M is finitely generated, then it is Artinian by Proposition 10 of VIII, p. 71.

Conversely, suppose that M is Artinian and without radical. By VIII, p. 2 applied to the set of maximal submodules of M, there exists a finite family $(N_i)_{i\in I}$ of maximal submodules of M whose intersection is reduced to 0. Then M is isomorphic to a submodule of $\bigoplus_{i\in I}(M/N_i)$. Therefore, it is semisimple and has finite length, and is a fortiori finitely generated.

### 2. The Radical of a Ring

#### Definition 2 {#alg-viii-s9-def-2 .statement tag=00AA}

The Jacobson radical (or simply radical) of a ring A, denoted by $\mathfrak{R}(A)$, is the radical of the A-module $A_s$, that is, the intersection of the maximal left ideals of A.

By abuse of language, we say that the ring A is without radical if we have $\mathfrak{R}(A) = 0$.

#### Proposition 4 {#alg-viii-s9-prop-4 .statement tag=00AB}

A ring A is semisimple if and only if it is left Artinian and without radical.

This follows from Proposition 3, b) applied to the A-module $A_s$.

#### Example 1 {#alg-viii-s9-n2-exa-1 .statement tag=00AC}

If A is a local ring, then it has a unique maximal left ideal $\mathfrak{r}$, consisting of the noninvertible elements of A (VIII, p. 25, Proposition 1); so $\mathfrak{r}$ is the radical of A. In particular, a field is without radical.

#### Example 2 {#alg-viii-s9-n2-exa-2 .statement tag=00AD}

Let K be a commutative field and E the algebra $K[[X_i]]_{i\in I}$ of formal power series in the variables $X_i$ with coefficients in K. By the previous example and Example 4 of VIII, p. 26, the radical of E consists of the formal power series with constant term zero. Observe that the ring E is an integral domain and that its radical is not reduced to 0, even though E is a subring of its field of fractions, which is without radical.

#### Example 3 {#alg-viii-s9-n2-exa-3 .statement tag=00AE}

Suppose that A is a principal ideal domain, and let P be a system of representatives consisting of irreducible elements (VII, §1, No. 3, p. 3). If A is a field, then it is without radical by Example 1. If the set P is infinite, then the intersection of the maximal ideals $Ap$ of A is reduced to 0, so A is without radical. But if P is finite and nonempty, and if we set $x=\prod_{p\in P}p$, then the radical of A is equal to $\cap_{p\in P}Ap= Ax$ (VII, §1, No. 2, p. 3, Proposition 4), hence is not reduced to 0.

Let $y$ be a nonzero element of A; we write it as $y=up^{i_1}_1\cdots p^{i_r}_r$, where $u$ is invertible in $A,p_1, . . . , p_r$ are pairwise distinct elements of P, and $i_1, . . . , i_r$ are strictly positive integers. The maximal ideals of the ring $A/Ay$ are the ideals $Ap_1/Ay, . . . ,Ap_r/Ay$; the radical of the ring $A/Ay$ is therefore the ideal $Ap_1\cdots p_r/Ay$. In particular, the ring $A/Ay$ is without radical if and only if we have $i_1=\cdots =i_r= 1$; in this case, we say that $y$ is without multiple factors.

#### Proposition 5 {#alg-viii-s9-prop-5 .statement tag=00AF}

a) The radical of a ring A is the intersection of the annihilators of simple A-modules; it is also the smallest annihilator of a semisimple A-module. It is, in particular, a two-sided ideal of A. If A is not reduced to 0, then the radical of A is distinct from A.

b) Let $\mathfrak{a}$ be a two-sided ideal of A. We have $(\mathfrak{R}(A) +\mathfrak{a})/\mathfrak{a}\subset \mathfrak{R}(A/\mathfrak{a})$. If $\mathfrak{a}$ is contained in $\mathfrak{R}(A)$, then we have $\mathfrak{R}(A/\mathfrak{a}) =\mathfrak{R}(A)/\mathfrak{a}$.

c) The ring $A/\mathfrak{R}(A)$ is without radical; conversely, every two-sided ideal $\mathfrak{a}$ of A such that $A/\mathfrak{a}$ is without radical contains $\mathfrak{R}(A)$.

d) The radical of A is contained in the intersection of the maximal two-sided ideals of A.

Let $x\in A$. Saying that $x$ belongs to the annihilator of every simple A-module is equivalent to saying that $x$ belongs to the annihilator of every element of every simple A-module, in other words (VIII, p. 46, Proposition 1), to every maximal left ideal of A.

Let M be a semisimple A-module. Its annihilator is the intersection of the annihilators of the simple submodules of M, so it contains $\mathfrak{R}(A)$. Furthermore, if $\mathscr{S}$ is the set of classes of simple A-modules (VIII, p. 51), then the direct sum $\oplus_{\lambda\in\mathscr{S}}\lambda$ is a semisimple A-module whose annihilator is $\mathfrak{R}(A)$. Suppose that A is not reduced to 0; the relation $\mathfrak{R}(A)\not= A$ follows from Proposition 2, a) of VIII, p. 153 applied to the A-module $A_s$. We have proved a).

Let $\mathfrak{a}$ be a two-sided ideal of A. The maximal left ideals of $A/\mathfrak{a}$ are the ideals of the form $\mathfrak{m}/\mathfrak{a}$, where $\mathfrak{m}$ is a maximal left ideal of A containing $\mathfrak{a}$. Consequently, the radical of the ring $A/\mathfrak{a}$ is equal to the radical of the A-module $A_s/\mathfrak{a}$. Assertions b) and c) therefore follow from Corollary 1 of VIII, p. 152.

Let $\mathfrak{a}$ be a maximal two-sided ideal of A. In the ring $A/\mathfrak{a}$, the only two-sided ideals are 0 and $A/\mathfrak{a}$. Since the ring $A/\mathfrak{a}$ is not reduced to 0, its radical is not equal to $A/\mathfrak{a}$. The ring $A/\mathfrak{a}$ is therefore without radical, and we have $\mathfrak{R}(A)\subset \mathfrak{a}$ by c). This proves d).

We say that a left (or right) ideal of A is a nil ideal if it consists of nilpotent elements. We say that a two-sided ideal $\mathfrak{a}$ of A is nilpotent if there exists an integer $n\geqslant 1$ such that $\mathfrak{a}^n= 0$, that is (I, §8, No. 9, p. 107), such that we have $x_1\cdots x_n= 0$ for every sequence $(x_1, . . . , x_n)$ of elements of $\mathfrak{a}$. Every nilpotent two-sided ideal is a nil ideal, but there can exist nil ideals that are not contained in a nilpotent two-sided ideal (VIII, p. 167, Exercise 9).

#### Theorem 1 (Jacobson) {#alg-viii-s9-thm-1 .statement tag=00S5}

The radical of a ring A consists of the elements $x\in A$ such that $1 +ax$ is left invertible (I, §2, No. 3, p. 15) for every $a\in A$. It is also the largest two-sided ideal $\mathfrak{a}$ such that $1 +x$ is invertible for every $x\in \mathfrak{a}$. The radical of A contains every left nil ideal of A.

The element 1 generates the A-module $A_s$, and $1 +ax$ is left invertible if and only if it generates the A-module $A_s$. The first assertion of Theorem 1 is therefore a specific case of the corollary of Proposition 2 (VIII, p. 153).

Let $x\in \mathfrak{R}(A)$. By the above, $1 +x$ is left invertible; let $y$ be an element of A such that $y(1 +x) = 1$. We then have $1-y=yx$, so $1-y$ belongs to $\mathfrak{R}(A)$; consequently, $y$ is left invertible. Since $y$ is also right invertible, it is invertible (I, §2, No. 3, p. 16, Proposition 3), and so is its right inverse $1 +x$.

Let $\mathfrak{a}$ be a left ideal of A such that $1 +x$ is invertible for every $x\in \mathfrak{a}$. This holds, for example, when $\mathfrak{a}$ is a nil ideal because the relation $x^n= 0$ implies that $1-x+\cdots + (-x)^{n-1}$ is the inverse of $1 +x$. Let $x\in \mathfrak{a}$. For every $a\in A$, we have $ax\in \mathfrak{a}$, so $1 +ax$ is invertible; hence, we have $x\in \mathfrak{R}(A)$. It follows that $\mathfrak{a}$ is contained in $\mathfrak{R}(A)$.

#### Corollary 1 {#alg-viii-s9-thm-1-cor-1 .statement tag=00AG}

The radical of A is equal to the radical of the opposite ring $A^o$, that is, to the intersection of the maximal right ideals of A.

For every $x\in \mathfrak{R}$(A), $1 +x$ is invertible in the ring A, hence in the ring $A^o$. Since $\mathfrak{R}(A)$ is a two-sided ideal of $A^o$, we have $\mathfrak{R}(A)\subset \mathfrak{R}(A^o)$. The equality follows by interchanging the roles of A and $A^o$.

#### Corollary 2 {#alg-viii-s9-thm-1-cor-2 .statement tag=00AH}

An element of A is invertible if and only if its canonical image in the ring $A/\mathfrak{R}(A)$ is invertible.

The condition is obviously necessary. Let us prove that it is sufficient. Let $x$ be an element of A whose canonical image in the ring $A/\mathfrak{R}(A)$ is invertible. There then exists an element $y$ of A such that $xy$ belongs to $1 +\mathfrak{R}(A)$. By Theorem 1$,xy$ is invertible; hence $x$ is right invertible. The proof that $x$ is left invertible is analogous.

#### Corollary 3 {#alg-viii-s9-thm-1-cor-3 .statement tag=00AI}

The radical of the product of a family $(A_i)_{i\in I}$ of rings is the product of the $\mathfrak{R}(A_i)$.

Let $x= (x_i)_{i\in I}$ be an element of $\prod_{i\in I}A_i$. For every element $a= (a_i)_{i\in I}$ of $\prod_{i\in I}A_i$, the element $1 +ax$ is left invertible if and only if $1 +a_ix_i$ is left invertible in $A_i$ for every $i\in I$. Corollary 3 follows.

#### Corollary 4 {#alg-viii-s9-thm-1-cor-4 .statement tag=00AJ}

The ring A is local if and only if the ring $A/\mathfrak{R}(A)$ is a field. If this is the case, then $\mathfrak{R}(A)$ is the set of noninvertible elements of A.

Denote the set of noninvertible elements of A by $\mathfrak{r}$. If the ring A is local, then its radical is equal to $\mathfrak{r}$ (VIII, p. 154, Example 1) and the ring $A/\mathfrak{r}$ is a field (VIII, p. 26). Conversely, suppose that the ring $A/\mathfrak{R}(A)$ is a field. By Corollary 2, we have $\mathfrak{r}=\mathfrak{R}$(A), so $\mathfrak{r}$ is a two-sided ideal of A. It follows that the ring A is local (VIII, p. 26, Definition 1).

#### Example 4 {#alg-viii-s9-n2-exa-4 .statement tag=00AK}

Let K be an integral domain, I a nonempty set, and A the polynomial ring $K[X_i]_{i\in I}$. Let us prove that the ring A is without radical. The only invertible elements of A are the invertible elements of K (IV, §1, No. 5, p. 9, Corollary 2). Let $f\in \mathfrak{R}(A)$. Choose an element $i\in I$. Then $1 +fX_i$ is invertible (Theorem 1), which implies $f= 0$.

Note that when K is a commutative field, the ring $A = K[X_i]_{i\in I}$ is a subring of $B = K[[X_i]]_{i\in I}$ and we have $\mathfrak{R}(A) = 0$ and $A\cap \mathfrak{R}(B)\not= 0$ (cf. VIII, p. 154, Example 2).

#### Example 5 {#alg-viii-s9-n2-exa-5 .statement tag=00AL}

Let $\mathfrak{a}$ be a two-sided ideal of A. The $\mathfrak{a}$-adic topology on A is the topology, compatible with the ring structure of A, for which the ideals $\mathfrak{a}^n$ (for $n\geqslant 1$) form a fundamental system of neighborhoods of 0 (Gen. Top., III, §6, No. 3, p. 275, Example 3). Suppose that the ring A is Hausdorff and complete (Gen. Top., III, §6, No. 5, p. 276) for this topology; this is, for example, the case when the ideal $\mathfrak{a}$ is nilpotent. For every $x\in \mathfrak{a}$, the series $\sum^{\infty}_{n=0}(-x)^n$ is then convergent. Let $y$ be its sum. We have $y-1 =\sum^{\infty}_{n=1}(-x)^n=-xy$, hence $(1 +x)y= 1$. Likewise, we have $y(1 +x) = 1$, so $1 +x$ is invertible. By Theorem 1, it follows that the ideal $\mathfrak{a}$ is contained in the radical of A.

#### Remark 1 {#alg-viii-s9-n2-rem-1 .statement tag=00AM}

By Theorem 1, every left nil ideal of a ring A is contained in

its radical. Let $x$ be a nilpotent and central element of A; then $Ax$ is a nil ideal of A, so $x$ belongs to the radical of A. It is, however, possible that there exist nonzero nilpotent elements of A but that A is without radical. For example, for every integer $n\geqslant 2$, the matrix ring $\mathbf{M}_n(K)$ over a field K is simple, hence without radical (VIII, p. 154, Proposition 4), and it contains nilpotent elements, for example the matrix units $E_{ij}$ with $i\not=j$.

#### Remark 2 {#alg-viii-s9-n2-rem-2 .statement tag=00AN}

Let A be a commutative ring. The set of nilpotent elements $a$ of A is an ideal $\mathfrak{N}(A)$ of A, called the nilradical of A; it is the intersection of the prime ideals of A (V, §15, No. 1, p. 118, Proposition 2). We have $\mathfrak{N}(A)\subset \mathfrak{R}(A)$; $*$we have equality if A is an Artinian ring (VIII, p. 173, Corollary 2) or a finitely generated commutative algebra over a commutative field (Comm. Alg., V, § 3, n$^{\circ}4$, Theorem $3$)$*$. We can certainly have $\mathfrak{N}(A)\not=\mathfrak{R}(A)$. This is the case when A is the ring K[[X]], where K is a commutative field: we then have $\mathfrak{N}(A) = 0$ and $\mathfrak{R}(A) =$ AX (VIII, p. 154, Example 2).

### 3. Nakayama’s Lemma

#### Proposition 6 {#alg-viii-s9-prop-6 .statement tag=00AO}

For every A-module M, we have $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$. We have equality if the A-module M is projective.

Let P be a maximal submodule of M; the A-module $M/P$ is simple, hence annihilated by $\mathfrak{R}(A)$ by Proposition 5 of VIII, p. 155. We therefore have $\mathfrak{R}(A)M\subset P$ for every maximal submodule P of M, hence $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$.

We clearly have $\mathfrak{R}(A_s) =\mathfrak{R}(A)A_s$. If the A-module M is projective, then there exists an A-module N such that $M\oplus N$ is free, that is, the direct sum of a family $(L_i)_{i\in I}$ of modules isomorphic to $A_s$. By Corollary 2 of VIII, p. 152, we have $\mathfrak{R}(M\oplus N) =\mathfrak{R}(M)\oplus \mathfrak{R}(N)$ and $\mathfrak{R}(\bigoplus_{i\in I}L_i)=\bigoplus_{i\in I}\mathfrak{R}(L_i)$. We then deduce $\mathfrak{R}(M) =\mathfrak{R}(A)M$ from the equality $\mathfrak{R}(L_i) =\mathfrak{R}(A)L_i$.

#### Theorem 2 (“Nakayama’s lemma”) {#alg-viii-s9-thm-2 .statement tag=00S6}

Let M be an A-module and $\mathfrak{a}$ a two-sided ideal of A. Suppose that one of the following conditions is satisfied:

(i) The A-module M is finitely generated, and $\mathfrak{a}$ is contained in the radical of A.

(ii) The ideal $\mathfrak{a}$ is nilpotent.

If N is a submodule of M such that $M = N +\mathfrak{a}M$, then we have N = M. In particular, if the module M is nonzero, then we have $M\not=\mathfrak{a}M$.

Suppose that M is finitely generated and that we have $\mathfrak{a}\subset \mathfrak{R}(A)$. Let N be a submodule of M such that $M = N +\mathfrak{a}M$. By Proposition 6, we have $M = N +\mathfrak{R}$(M), hence M = N by Proposition 2, b) of VIII, p. 153.

Now suppose that $\mathfrak{a}$ is nilpotent, and let N be a submodule of M such that $M = N +\mathfrak{a}M$. By induction on the integer $n\geqslant 0$, we establish the relation $M = N +\mathfrak{a}^nM$. By assumption, there exists an integer $n\geqslant 0$ such that $\mathfrak{a}^n= 0$; hence M = N.

The last assertion of the theorem follows from the above by taking N to be 0.

#### Corollary 1 {#alg-viii-s9-thm-2-cor-1 .statement tag=00R9}

We keep the assumptions of Theorem 2. Let $(x_i)_{i\in I}$ be a family of elements of M, and let $\overline{x}_i$ be the canonical image of $x_i$ in $M/\mathfrak{a}M$. If the family $(\overline{x}_i)_{i\in I}$ generates the $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$, then the family $(x_i)_{i\in I}$ generates the A-module M.

This follows from Theorem 2 applied to the submodule N of M generated by the family $(x_i)_{i\in I}$.

#### Corollary 2 {#alg-viii-s9-thm-2-cor-2 .statement tag=00AP}

We keep the assumptions of Theorem 2. Furthermore, let $M'$ be an A-module and $u: M'\rightarrow M$ be a homomorphism. If the homomorphism $\overline{u}$ from $M'/\mathfrak{a}M'$ to $M/\mathfrak{a}M$ deduced from $u$ by passing to the quotients is surjective, then $u$ is surjective.

It suffices to apply Theorem 2 to the image N of $u:$ indeed, the image of $\overline{u}$ is $(N +\mathfrak{a}M)/\mathfrak{a}M$, so $\overline{u}$ is surjective if and only if we have $N +\mathfrak{a}M = M$.

### 4. Lifts of Idempotents

#### Lemma 1 {#alg-viii-s9-lem-1 .statement tag=00AQ}

Let $a$ be an element of a ring A such that $a-a^2$ is nilpotent. There exists a polynomial P in $X + (X-X^2)\mathbf{Z}[X]$ such that $P(a)$ is idempotent in A.

Let $n$ be a strictly positive integer such that $(a-a^2)^n= 0$. Set P(X) = $1-(1-X^n)^n$. The polynomial P(X) is a multiple of $X^n$, and the polynomial $1-P(X)$ is a multiple of $(1-X)^n$, so $P(X)-P(X)^2$ is a multiple of $(X-X^2)^n$, and we have $P(a) = P(a)^2$. Moreover, $X-P(X)$ is a multiple of X and $1-X$, hence a multiple of $X-X^2$.

#### Proposition 7 {#alg-viii-s9-prop-7 .statement tag=00AR}

Let $\mathfrak{a}$ be a two-sided nil ideal of A, and let $\overline{e}$ be an idempotent in the ring $A/\mathfrak{a}$. There exists an idempotent $e$ in A whose canonical image in $A/\mathfrak{a}$ is equal to $\overline{e}$.

Let $a$ be an arbitrary representative of $\overline{e}$ in A. The element $a-a^2$ of A is nilpotent because it belongs to $\mathfrak{a}$. Choose a polynomial $P\in \mathbf{Z}[X]$ satisfying the conditions of Lemma 1. We have $a-P(a)\in A(a-a^2)$, so the element $e= P(a)$ of A has the desired property.

Suppose that $\overline{e}$ belongs to the center of the ring $A/\mathfrak{a}$. There does not necessarily exist an idempotent $e$ in the center Z of A lifting $\overline{e}$ (VIII, p. 172, Exercise 31). However, if $\overline{e}$ belongs to the image of Z in $A/\mathfrak{a}$, then it lifts to an idempotent in Z because $Z\cap \mathfrak{a}$ is a nil ideal of Z.

#### Corollary 1 {#alg-viii-s9-prop-7-cor-1 .statement tag=00AS}

Let M and P be A-modules and $u$ a surjective A-linear mapping from P to M. Suppose that P is projective and that there exists a nilpotent two-sided ideal $\mathfrak{a}$ of A such that the kernel N of $u$ is contained in $\mathfrak{a}P$. Let $M'$ and $M''$ be submodules of M whose direct sum is M. Then P is the direct sum of submodules $P'$ and $P''$ such that $u(P') = M'$ and $u(P'') = M''$.

Denote by B the subring of End$_A(P)$ consisting of the endomorphisms $f$ of P such that $f(N)\subset N$. Let $\overline{B}$ be the endomorphism ring of M. For $f\in B$, let $\overline{f}$ be the unique endomorphism of M such that $\overline{f}\circ u=u\circ f$. The mapping $f\mapsto \overline{f}$ is a ring homomorphism from B to B. Since the module P is projective, this homomorphism is surjective; its kernel $\mathfrak{b}$ consists of the endomorphisms $f\in B$ such that $f(P)\subset N$. Let $n$ be a natural number such that $\mathfrak{a}^n= 0$. We have

$$
P =\mathfrak{a}^0P\supset \mathfrak{a}^1P\supset  \cdots  \supset \mathfrak{a}^{n-1}P\supset \mathfrak{a}^nP = 0
$$

and, for every $f\in \mathfrak{b}$ and every integer $j\geqslant 0$,

$$
f(\mathfrak{a}^jP) =\mathfrak{a}^jf(P)\subset \mathfrak{a}^jN\subset \mathfrak{a}^{j+1}P
$$

because $N\subset \mathfrak{a}P$ by assumption. We therefore have $f(P)\subset \mathfrak{a}^jP$ for every natural number $j$ and every $f\in \mathfrak{b}^j$. In particular, we have $\mathfrak{b}^n= 0$.

Let $\varepsilon '$ be the projector of M with image $M'$ and kernel $M''$. By Proposition 7 applied to the ring B and the nilpotent two-sided ideal $\mathfrak{b}$, there exists an idempotent $e'$ in B such that $\overline{e'}=\varepsilon '$, that is, $\varepsilon '\circ u=u\circ e'$. Set $e''= 1-e'$, $\varepsilon ''=\overline{e''}, P'=e'$(P), and $P''=e''(P)$. Then P is the direct sum of the submodules $P'$ and $P''$, and we have

$$
u(P') =u(e'(P)) =\varepsilon '(u(P)) =\varepsilon '(M) = M'
$$

the equality $u(P'') = M''$ is proved analogously.

#### Corollary 2 {#alg-viii-s9-prop-7-cor-2 .statement tag=00AT}

Let A be a ring, and let $\mathfrak{a}$ be a nilpotent two-sided ideal of A. If P is a projective A-module, then $P/\mathfrak{a}P$ is a projective module over $A/\mathfrak{a}$, and the A-module P is indecomposable if and only if the $A/\mathfrak{a}$-module $P/\mathfrak{a}P$ is indecomposable.

Let P be a projective A-module, and let $\overline{P}$ be the $A/\mathfrak{a}$-module $P/\mathfrak{a}P$. The A-module P is zero if and only if $\overline{P}$ is zero (Theorem 2 of VIII, p. 158). Now suppose $P\not= 0$. Since the $A/\mathfrak{a}$-module P is isomorphic to $\overline{A}\otimes_AP$, it is projective (II, §5, No. 1, p. 279, Corollary of Proposition 4). If P is indecomposable, then so is $\overline{P}$ by Corollary 1. Conversely, suppose that P is decomposable and nonzero, and let $P'$ and $P''$ be two nonzero submodules of P such that $P = P'\oplus P''$. By Nakayama’s lemma (VIII, p. 158, Theorem 2), we have $P'+\mathfrak{a}P\not= P$ and $P''+\mathfrak{a}P\not= P$; if $\overline{P}'$ and $\overline{P}''$ are the canonical images of $P'$ and $P''$ in P, then we have $\overline{P}'\not= P,\overline{P}''\not= P$, and $\overline{P}=\overline{P}'\oplus \overline{P}''$. This proves that $\overline{P}$ is decomposable.

### 5. Projective Cover of a Module

#### Definition 3 {#alg-viii-s9-def-3 .statement tag=00AU}

Let A be a ring, and let M be an A-module. A projective cover of M is a pair $(P, u)$, where P is a projective A-module and $u$ a surjective homomorphism from P to M such that we have $u(P')\not= M$ for every proper A-submodule $P'$ of P.

#### Remark 1 {#alg-viii-s9-n5-rem-1 .statement tag=00AV}

For every projective A-module M, the pair $(M,1_M)$ is a projective cover of M.

#### Remark 2 {#alg-viii-s9-n5-rem-2 .statement tag=00AW}

Suppose that $(P, u)$ is a projective cover of the A-module M. Let $(x_i)_{i\in I}$ be a family of elements of P, and let $P'$ be the submodule of P that it generates; then $u(P')$ is generated by the family $(u(x_i))_{i\in I}$. Consequently, the family $(x_i)_{i\in I}$ generates the A-module P if and only if the family $(u(x_i))_{i\in I}$ generates the A-module M. In particular, P is finitely generated if and only if M is finitely generated.

#### Proposition 8 {#alg-viii-s9-prop-8 .statement tag=00AX}

Let M and $M'$ be A-modules, $(P, u)$ and $(P', u')$ projective covers of M and $M'$, respectively, and $g: M\rightarrow M'$ an A-linear mapping.

a) There exists an A-linear mapping $f: P\rightarrow P'$ such that $u'\circ f=g\circ u$.

b) Let $f$ be such a mapping. If $g$ is surjective (resp. bijective), then $f$ is surjective (resp. bijective). If $g$ is injective and its image is a direct factor of $M'$, then $f$ is injective and its image is a direct factor of $P'$.

By assumption, the A-module P is projective and the mapping $u'$ is surjective. Consequently, there exists an A-linear mapping $f: P\rightarrow P'$ such that $g\circ u=u'\circ f$ (II, §2, No. 2, p. 231, Proposition 4). Assertion a) follows.

Let $f$ be a mapping as in a). Suppose that $g$ is surjective. Since $u$ is surjective, we have $M'=g(u(P)) =u'(f(P))$. Since $(P', u')$ is a projective cover of M’, we have $f(P) = P'$, so $f$ is surjective. By loc. cit., the kernel of $f$ admits a supplementary submodule $P_1$, so $f(P_1) = P'$. Now suppose that $g$ is bijective. We have $g(u(P_1)) =u'(f(P_1)) =u'(P') = M'$, hence $u(P_1) = M$. Since $(P, u)$ is a projective cover of M, we have $P_1= P$, hence Ker($f$) $= 0$. So $f$ is injective; since we already know that $f$ is surjective, $f$ is bijective.

To conclude, suppose that $g$ is injective and that its image is a direct factor of $M'$. Then there exists an A-linear mapping $g': M'\rightarrow M$ such that $g'\circ g= 1_M$. By a), there exists an A-linear mapping $f': P'\rightarrow P$ such that $u\circ f'=g'\circ u'$. We have $u\circ (f'\circ f) =g'\circ u'\circ f= (g'\circ g)\circ u$; by the previous paragraph, the mapping $f'\circ f$ is bijective. Denote the converse bijection by $h$; we have $(h\circ f')\circ f= 1_P$, so $f$ is injective, and its image is a direct factor of $P'$ (II, §1, No. 9, p. 212, Corollary 2).

#### Corollary 1 {#alg-viii-s9-prop-8-cor-1 .statement tag=00AY}

Let M be an A-module. Let $(P, u)$ and $(P', u')$ be projective covers of M. There exists an isomorphism $f$ from P to $P'$ such that $u=u'\circ f$.

Note that $f$ is not necessarily uniquely determined by the relation $u=u'\circ f$ (VIII, p. 170, Exercise 21).

#### Corollary 2 {#alg-viii-s9-prop-8-cor-2 .statement tag=00AZ}

Let $(P, u)$ be a projective cover of the A-module M. If Q is a projective A-module and $g: Q\rightarrow M$ a surjective linear mapping, then there exists a surjective linear mapping $f: Q\rightarrow P$ such that $g=u\circ f$.

#### Proposition 9 {#alg-viii-s9-prop-9 .statement tag=00B0}

Let M be an A-module and $(P, u)$ a projective cover of M. Denote the radical of the ring A by $\mathfrak{r}$. The homomorphism $\overline{u}: P/\mathfrak{r}P\rightarrow M/\mathfrak{r}M$ deduced from $u$ by passing to the quotients is an isomorphism.

The homomorphism $u$ is surjective by definition, so $\overline{u}$ is surjective. Denote the kernel of $u$ by N. We have $u^{-1}(\mathfrak{r}M) = N +\mathfrak{r}P$. Let us prove that we have $N\subset \mathfrak{r}P$, which implies the injectivity of $\overline{u}$. For every maximal submodule $P'$ of P, we have $u(P')\not= M$, hence $P'+ N\not= P$; since $P'$ is maximal, we have $N\subset P'$. The submodule N of P is therefore contained in the radical of P. Now, the latter is equal to $\mathfrak{r}P$ by Proposition 6 of VIII, p. 158.

#### Corollary {#alg-viii-s9-n5-cor-1 .statement tag=00B1}

If an A-module M has a projective cover, then the $A/\mathfrak{r}$-module $M/\mathfrak{r}M$ is projective.

Indeed, if $(P, u)$ is a projective cover of M, then the $(A/\mathfrak{r}$)-module $M/\mathfrak{r}M$ is isomorphic to $P/\mathfrak{r}P$ (Proposition 9). Since the A-module P is projective, the $(A/\mathfrak{r}$)-module $P/\mathfrak{r}P$ is also projective.

#### Remark 3 {#alg-viii-s9-n5-rem-3 .statement tag=00B2}

Suppose that the ring A is without radical. By Proposition 9, $(P, u)$ is a projective cover of an A-module M if and only if $u$ is an isomorphism. Hence, projective covers can only exist for projective A-modules.

The ring $\mathbf{Z}$ is without radical (VIII, p. 154, Example 3). Let $n\geqslant 2$ be an integer. The $\mathbf{Z}$-module $\mathbf{Z}/n\mathbf{Z}$ is not projective and therefore does not admit a projective cover.

#### Remark 4 {#alg-viii-s9-n5-rem-4 .statement tag=00B3}

Suppose that every finitely generated A-module has a projective cover; then the quotient $A'$ of A by its radical is semisimple. Indeed, every finitely generated module over the ring $A'$ is projective by the corollary. In particular, for every left ideal $\mathfrak{a}$ of $A'$, the $A'$-module $A'_s/\mathfrak{a}$ is projective. Our assertion then follows from Proposition 4 of VIII, p. 138.

We can give examples of a commutative ring A for which $A/\mathfrak{r}$ is semisimple and of a finitely generated A-module M that does not admit a projective cover (VIII, p. 170, Exercise 22).

#### Proposition 10 {#alg-viii-s9-prop-10 .statement tag=00B4}

Let M be an A-module, P a projective A-module, and $u: P\rightarrow M$ a linear mapping. Let $\mathfrak{a}$ be a two-sided ideal of A. Suppose that the linear mapping $\overline{u}: P/\mathfrak{a}P\rightarrow M/\mathfrak{a}M$ deduced from $u$ by passing to the quotients is bijective and that one of the following conditions are satisfied:

(i) The A-modules M and P are finitely generated, and $\mathfrak{a}$ is contained in the radical of A.

(ii) The ideal $\mathfrak{a}$ is nilpotent.

Then $(P, u)$ is a projective cover of M.

Under the assumptions, the homomorphism $u$ is surjective (VIII, p. 159, Corollary 2) and its kernel N is contained in $\mathfrak{a}P$. Let $P'$ be a proper submodule of P. By Nakayama’s lemma (VIII, p. 158, Theorem 2), we have $P'+\mathfrak{a}P\not= P$ and therefore $u(P')\not= M$. So $(P, u)$ is a projective cover of M.

#### Corollary 1 {#alg-viii-s9-prop-10-cor-1 .statement tag=00B5}

Let P be a projective A-module. Suppose that P is finitely generated or that the radical $\mathfrak{r}$ of A is a nilpotent two-sided ideal. Denote the canonical mapping from P to $P/\mathfrak{r}P$ by $u$. Then $(P, u)$ is a projective cover of $P/\mathfrak{r}P$.

#### Corollary 2 {#alg-viii-s9-prop-10-cor-2 .statement tag=00B6}

Let $\mathfrak{a}$ be a two-sided ideal of A and M an A-module such that the $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$ is free. Suppose that one of the following conditions is satisfied:

(i) The module M is finitely generated, and $\mathfrak{a}$ is contained in the radical of A.

(ii) The ideal $\mathfrak{a}$ is nilpotent.

Then M has a projective cover.

More precisely, let P be a free A-module, $(e_i)_{i\in I}$ a basis of P, and let $u: P\rightarrow M$ be a homomorphism such that the canonical images of the elements $u(e_i)$ of $M/\mathfrak{a}M$ form a basis of the $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$. Then $(P, u)$ is a projective cover of M.

The $(A/\mathfrak{a}$)-module $P/\mathfrak{a}P$ is free, and the homomorphism $\overline{u}$ from $P/\mathfrak{a}P$ to $M/\mathfrak{a}M$ deduced from $u$ by passing to the quotients transforms a basis of $P/\mathfrak{a}P$ into a basis of $M/\mathfrak{a}M$, hence is bijective.

If $\mathfrak{a}$ is nilpotent, then it suffices to apply Proposition 10. Now suppose that the ring A is nonzero and that the module M is finitely generated; then so is the $(A/\mathfrak{a}$)-module $M/\mathfrak{a}M$, and consequently also the $(A/\mathfrak{a}$)-module $P/\mathfrak{a}P$. Every basis of $P/\mathfrak{a}P$ is then finite. It follows that the set I is finite and that the A-module P is finitely generated. We then apply Proposition 10 again.

#### Corollary 3 {#alg-viii-s9-prop-10-cor-3 .statement tag=00B7}

Every finitely generated module over a local ring has a projective cover.

Let A be a local ring and $\mathfrak{r}$ its radical. It is a two-sided ideal of A (VIII, p. 155, Proposition 5, a)), and the ring $A/\mathfrak{r}$ is a field (VIII, p. 157, Corollary 4). If M is an A-module, then $M/\mathfrak{r}M$ is a vector space over the field $A/\mathfrak{r}$, hence is a free $(A/\mathfrak{r}$)-module. It then suffices to apply Corollary 2.

#### Remark 5 {#alg-viii-s9-n5-rem-5 .statement tag=00B8}

Let A be a local ring and $\mathfrak{r}$ its radical. Let M be a finitely generated A-module, P a finitely generated projective A-module, and $u: P\rightarrow$ M a homomorphism. By Corollary 6 of VIII, p. 36, the A-module P is free. Choose a basis $(e_i)_{i\in I}$ of P. Set $x_i=u(e_i)$, and denote the canonical image of $x_i$ in $M/\mathfrak{r}M$ by $\overline{x}_i$. The following properties are equivalent:

(i) The pair $(P, u)$ is a projective cover of M.

(ii) The family $(x_i)_{i\in I}$ is a minimal generating family of the A-module M.

(iii) The family $(\overline{x}_i)_{i\in I}$ is a basis of the vector space $M/\mathfrak{r}M$ over the field $A/\mathfrak{r}$.

We have (i) $\Rightarrow$ (ii) by Remark 2 of VIII, p. 161 and (iii) $\Rightarrow$ (i) by Corollary 2. Furthermore, if the family $(x_i)$ is a minimal generating family of the A-module M, then the family $(\overline{x}_i)$ is a minimal generating family, that is, a basis, of the vector space $M/\mathfrak{r}M$ over $A/\mathfrak{r}$ (VIII, p. 158, Corollary 1).

#### Proposition 11 {#alg-viii-s9-prop-11 .statement tag=00B9}

Let A be a ring and $\mathfrak{a}$ a nilpotent two-sided ideal of A. Let M be a projective $A/\mathfrak{a}$-module. There exist a projective A-module P and a surjective A-linear mapping $u: P\rightarrow M$ with kernel $\mathfrak{a}P$.

Such a pair $(P, u)$ is a projective cover of M viewed as an A-module.

There exists an $A/\mathfrak{a}$-module $M'$ such that $M\oplus M'$ is a free $A/\mathfrak{a}$-module. Choose a free A-module L and a surjective A-linear mapping $v: L\rightarrow M\oplus M'$ with kernel $\mathfrak{a}L$. By Corollary 1 of Proposition 7 (VIII, p. 159), there exists a direct sum decomposition $L = P\oplus P'$ such that $v(P) = M$ and $v(P') = M'$. The A-module P is projective, and the A-linear mapping $u$ from P to M that coincides with $v$ on P is surjective, with kernel $\mathfrak{a}P$. The first assertion follows.

Let P be a projective A-module and $u$ a homomorphism from P to M with kernel $\mathfrak{a}P$. By Proposition 10, the pair $(P, u)$ is a projective cover of M.

#### Corollary {#alg-viii-s9-n5-cor-2 .statement tag=00RA}

Let P and $P'$ be projective A-modules. If the modules $P/\mathfrak{a}P$ and $P'/\mathfrak{a}P'$ are isomorphic, then P and $P'$ are isomorphic.

Since $P/\mathfrak{a}P$ and $P'/\mathfrak{a}P'$ are projective, the corollary follows from Proposition 11 and the uniqueness of the projective cover (VIII, p. 162, Corollary 1).

### Exercises {#alg-viii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
