---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 4
section_title: Finitely generated modules over a principal ideal domain
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.15-A VII.28, A VII.62-A VII.70
pdf_pages: 0374-0387, 0421-0429
extraction: ocr
subsections:
    - "no": 1
      title: Direct sums of cyclic modules
      page: 15
      pdf_page: 374
    - "no": 2
      title: Content of an element of a free module
      page: 16
      pdf_page: 375
    - "no": 3
      title: Invariant factors of a submodule
      page: 18
      pdf_page: 377
    - "no": 4
      title: Structure of finitely generated modules
      page: 19
      pdf_page: 378
    - "no": 5
      title: Calculation of invariant factors
      page: 20
      pdf_page: 379
    - "no": 6
      title: Linear mappings of free modules, and matrices over a principal ideal domain
      page: 21
      pdf_page: 380
    - "no": 7
      title: Finitely generated abelian groups
      page: 22
      pdf_page: 381
    - "no": 8
      title: Indecomposable modules. Elementary divisors
      page: 23
      pdf_page: 382
    - "no": 9
      title: Duality in modules of finite length over a principal ideal domain
      page: 25
      pdf_page: 384
statements: 40
exercises: 9
content_sha256: 9924d30e0670032b6d984c3497a581e35a1418ed291f12578eb182b04990f795
---

## § 4. FINITELY GENERATED MODULES OVER A PRINCIPAL IDEAL DOMAIN

### 1. Direct sums of cyclic modules

Let A be a commutative ring. Recall (II, p. 220, Prop. 22) that a cyclic A-module is isomorphic to a *quotient module* $A/a$, where a is an ideal of A. We will see later (Sect. 4) that every finitely generated module over a principal ideal domain is a direct sum of finitely many cyclic modules.

#### Proposition 1 {#alg-vii-s4-prop-1 .statement}

— *Let E be a module over a commutative ring A; suppose E is a direct sum of n cyclic modules $\Lambda/\mathfrak{a}_k$ ($1 \leq k \leq n$), where the $\mathfrak{a}_k$ are ideals of A;*

then, for each integer $p > 0$, the $A$-module $\bigwedge^p E$ is isomorphic to the direct sum of the modules $A / a_H$, where for each $p$-element subset $H = \{ k_1, \ldots, k_p \}$ of $[1, n]$, the ideal $a_H$ is $\sum_{j=1}^p a_{k_j}$.

Let $x_k$ be the canonical generator of $A / a_k$, that is the image of the unit element of $A$, so that $E$ is the direct sum of the $Ax_i$ ($1 \leq i \leq n$). Then we know (III, p. 515, Prop. 10) that the exterior algebra $\bigwedge^n E$ is isomorphic as an $A$-module to the tensor product $\bigotimes_{i=1}^n (\bigwedge (Ax_i))$. Now $\bigwedge (Ax_i)$ is just the direct sum $A \oplus Ax_i$, since the exterior product of any two elements of $Ax_i$ is zero, and so $\bigwedge^p E$ is the direct sum of the modules $M_H = (Ax_{k_1}) \otimes \ldots \otimes (Ax_{k_p})$ as $H = \{ k_1, \ldots, k_p \}$ runs over the set of $p$-element subsets of $[1, n]$ (with $k_1 < \ldots < k_p$) ; now $M_H$ is known to be isomorphic to $A / a_{11}$ (II, p. 257, Cor. 4), which completes the proof.

We now see that, in the notation of Prop. 1, if the ideals $a_k$ form an increasing sequence, they are completely determined by the module $E$. More precisely :

#### Proposition 2 {#alg-vii-s4-prop-2 .statement}

— *Let $A$ be a commutative ring, and let $E$ be a direct sum of $n$ cyclic modules $A / a_k$, where the $a_k$ satisfy $a_1 \subset a_2 \subset \ldots \subset a_n$. Then, for $1 \leq p \leq n$, the ideal $a_p$ is the annihilator of $\bigwedge^p E$; if $a_n \neq A$ then $\bigwedge^p E \neq 0$ for $1 \leq p \leq n$ and $\bigwedge^m E = 0$ for $m > n$.*

Indeed, in the notation of Prop. 1, we have $a_p = a_{s(H)}$, where $s(H)$ denotes the greatest element of the subset $H$. Since $s(H) \geq p$ for every $p$-element subset $H$, and since $s(H) = p$ for $H = \{ 1, \ldots, p \}$, it follows that $a_p$ is the intersection of $a_r$, as $H$ varies over the set of $p$-element subsets of $(1, n)$; the ideal $a_p$ is thus indeed the annihilator of $\bigwedge^p E$, by Prop. 1.

#### Corollary {#alg-vii-s4-n1-cor-1 .statement}

— *In the notation of Prop. 2, if $a_n \neq A$, and if $E$ is also isomorphic to the direct sum of $m$ cyclic modules $A / a'_j$ with $a'_1 \subset a'_2 \subset \ldots \subset a'_m \neq A$, then $m = n$ and $a_k = a'_k$ for $1 \leq k \leq n$ (*uniqueness of the $a_k *$).

### 2. Content of an element of a free module

Let $A$ be a principal ideal domain, let $L$ be a free $A$-module, and let $x$ be an element of $L$. As $f$ runs through the set $L^*$ of linear forms on $L$, the elements $f(x)$ form an ideal $c_L(x)$ of $A$, called the *content* of $x$ in $L$. An element $c$ of $A$ is called a *content* of $x$ in $L$ if it generates the ideal $c_{L}(x)$; this amounts to saying that there exists a linear form $f$ on $L$ such that $f(x) = c$ and that $c$ divides $g(x)$ for every linear form $g$ on $L$. Let $(e_i)_{i \in I}$ be a basis of $L$; put $x = \sum a_i e_i, a_i \in A$; then the ideal $c_L(x)$ consists of sums $\sum a_i b_i$, as $(b_i)$ runs through the set $A'$; it follows immediately that an element $c$ of $A$ is a content of $x$ in $L$ if and only if it is a gcd of the family $(a_i)$ of coordinates of $x$.

We say that $x$ is *indivisible* if $c_L(x) = A$, that is if the coordinates of $x$ with respect to a basis of $L$ are setwise coprime.

#### Lemma 1 {#alg-vii-s4-lem-1 .statement}

*Let $L$ be a free module over a principal ideal domain $A$ and let $x$ be an element of $L$. Then the following conditions are equivalent*:

(i) $x$ is indivisible ;
(ii) *there exists a linear form $f$ on $L$ such that $f(x) = 1$ ;
(iii) $x$ is nonzero and the submodule $Ax$ is a direct factor of $L$ ;
(iv) $x$ is an element of some basis of $L$.

(i) $\Rightarrow$ (ii) : this follows from the definition.
(ii) $\Rightarrow$ (iii) : let $f$ be a linear form on $L$ such that $f(x) = 1$ ; then $x \neq 0$ and the map $y \mapsto f(y)x$ is a projector of $L$, with image $Ax$.
(iii) $\Rightarrow$ (iv) : let $L'$ be a complement of $Ax$ in $L$, and let $B'$ be a basis of $L'$ (*VII*, p. 15, Cor. 2) ; then $B' \cup \{x\}$ is a basis of $L$.
(iv) $\Rightarrow$ (i) : trivial.

#### Remark {#alg-vii-s4-n2-rem-1 .statement}

— 1) If $x$ is a nonzero element of $L$ and $c$ a content of $x$, then there exists a unique element $y$ of $L$ such that $x = cy$ ; denote this element $x/c$ ; then $x/c$ is an indivisible element of $L$.
2) The content $c_L(x)$ is the annihilator of the torsion module of $L/Ax$.

Let $L$ be a free module over a principal ideal domain $A$ and let $M$ be a submodule of $L$ ; by *VII*, p. 4, Lemma 1, the family $c_L(x), x \in M$, has a maximal element ; if $M \neq \{0\}$ then such a maximal element is nonzero.

#### Proposition 3 {#alg-vii-s4-prop-3 .statement}

*Let $L$ be a free module over a principal ideal domain $A$ and let $M$ be a nonzero submodule of $L$. Let $x$ be an element of $M$ such that $c_L(x)$ is maximal among the contents of elements of $M$, let $c$ be a content of $x$ in $L$, and let $f$ be a linear form on $L$ such that $f(x) = c$.

a) $L$ is the direct sum of $A(x/c)$ and the kernel $K$ of $f$.
b) $M$ is the direct sum of $Ax$ and $K \cap M$.
c) $g(M) \subset Ac$ for every linear form $g$ on $L$.

Put $y = x/c$ ; clearly $Ay \cap K = \{0\}$, since $f(y) = 1$. Furthermore, for each $u \in L$ we have
$$
u = f(u)\,y + (u - f(u)\,y),
$$
with $f(u)y \in Ay$ and $u - f(u)y \in K$ ; this proves *a)*. Now note that for $u \in M$ we have $f(u) \in Ac$ : indeed, let $u \in M$, and let $d$ be a gcd of $f(u)$ and $c$ ; then there exist $\lambda, \mu \in A$ such that $d = Xf(u) + \mu c = f(Xu + \mu x)$ ; hence the content of the element $\lambda u + \mu x$ of $M$ divides $d$ ; by the maximality of $c$, this implies that $d$ is an associate of $c$, so $f(u) \in Ac$. Hence for all $u$ in $M$, we can write
$$
u = (f(u)/c)\,x + (u - (f(u)/c)\,x) \in Ax + (K \cap M),
$$
which shows *b)*. Finally, let $g$ be a linear form on $L$ ; by *a)* there exists a scalar $\alpha \in A$ and a linear form $h$ on $K$ such that $g(u) = \alpha f(u) + h(u - f(u)\,y)$ ; thus by

b) we have $g(M) \subset Ac + h(K \cap M)$. To prove c), it is therefore sufficient to prove that $h(K \cap M) \subset Ac$ for every linear form $h$ on $K$, or equivalently for every linear form $h$ on $L$ such that $h(x) = 0$; now, if $u \in K \cap M$ and $d$ is a gcd of $h(u)$ and $c$, then there exist $A, \mu \in A$ with $d = \lambda h(u) + \mu c$; then $(f + h)(Au + \mu x) = d$, which implies as above that $h(u) \in Ac$, and c) follows.

### 3. Invariant factors of a submodule

#### Theorem 1 {#alg-vii-s4-thm-1 .statement}

— Let $L$ be a free module over a principal ideal domain $A$, and let $M$ be a submodule of $L$ of finite rank $n$. Then there exist a basis $B$ of $L$, $n$ elements $e_i$ of $B$, and $n$ nonzero elements $\alpha_i$ of $A$ ($1 \leq i \leq n$) such that:
a) the $\alpha_i e_i$ form a basis of $M$;
b) $a_i$ divides $\alpha_{i-1}$, for $1 \leq i \leq n-1$.

Moreover the module $M'$ generated by the $(e_i)$ and the principal ideals $A\alpha_i$ are uniquely determined by the above conditions; the module $M'/M$ is the torsion submodule of $L/M$, and is isomorphic to the direct sum of the $A$-modules $A/A\alpha_i$; finally $L/M$ is the direct sum of $M'/M$ and a free module isomorphic to $L/M'$.

1) Existence of the $e_i$ and the $\alpha_i$.

If $M = \{0\}$ then the theorem is trivial. If $M \neq \{0\}$ then it follows from Prop. 3 that there exist an element $e_1$ of $L$, a nonzero element $a$, of $A$, and a submodule $L_1$ of $L$, such that $L$ is the direct sum of $Ae_1$ and $L_1$, such that $M$ is the direct sum of $A\alpha_1 e_1$ and the submodule $M_1 = M \cap L_1$ of $L$, and such that $g(M) \subset A\alpha_1$ for every linear form $g$ on $L$.

Now we can proceed by induction on the rank $n$ of $M$. Since $L_1$ is a free module (VII, p. 15, Cor. 2) and $M_1$ has rank $n-1$, there exist a basis $B_1$ of $L_1$, $(n-1)$ elements $e_2, \ldots, e_n$ of $B_1$, and nonzero elements $\alpha_2, \ldots, a$, of $A$ such that $(\alpha_2 e_2, \ldots, \alpha_n e_n)$ is a basis of $M_1$, and $\alpha_i$ divides $\alpha_{i+1}$ for $2 \leq i \leq n-1$. If $L'$ is the submodule of $L$, generated by the elements of $B_1$ distinct from $e_1, \ldots, e_n$, then $L$ is the direct sum of $L'$ and the module $M'$ generated by $e_1, \ldots, e_n$; now $(e_1, \ldots, e_n)$ is a basis for $M'$, and $(\alpha_1 e_1, \ldots, \alpha_n e_n)$ is a basis for $M$. It now remains only to show that $a_i$ divides $a_i$; but $A\alpha_2$ has the form $g(M_1)$, where $g$ is the linear form on $L$ defined by $g(e_2) = 1, g(e_i) = 0$ for $i \neq 2$, and $g(L') = (0)$; and we have seen above that $g(M_1) \subset A\alpha_1$.

2) Uniqueness properties.

Since the $a_i$ are nonzero, the module $M'$ is the set of $x \in L$ such that $\beta x \in M$ for some $\beta \neq 0$ in $A$; in other words $M'/M$ is the torsion submodule of $L/M$. This uniquely determines $M'$.

It is clear that $M'/M$ is isomorphic to the direct sum of the $n$ cyclic modules $A/A\alpha_i$ (II, p. 204, formula (26)). Let $r$ be the number of the ideals $A\alpha$, which are distinct from $A$: so that the first $n-r$ ideals $A\alpha_i$ are equal to $A$, and the last rare distinct from $A$. Then $M'/M$ is also isomorphic to the direct sum of the modules $A/A\alpha_n, \ldots, A/A\alpha_{n-r+1}$, where $A\alpha_n \subset A\alpha_{n-1} \subset \ldots \subset A\alpha_{n-r+1} \neq A$.

Thus the conditions of the Cor. to Prop. 2 (VII, p. 16) are satisfied: the ideals $Aa_i$ ($1 \leq i \leq n$) are thus uniquely determined by the module $M'/M$.

Since $L$ is the direct sum of $M'$ and $L'$, it follows that $L/M$ is the sum of $M'/M$ and $(L' + M)/M$, and this sum is direct since $(L' + M) \cap M' = M$; on the other hand $(L' + M)/M$ is isomorphic to $L'/(M \cap L')$ (I, p. 41, Th. 4, c)), that is to $L'$, which shows that $(L' + M)/M$ is a free module isomorphic to $L/M'$.

#### Corollary {#alg-vii-s4-n3-cor-1 .statement}

— A submodule $M$ of finite rank in a free module $L$ over a principal ideal domain $A$ has a complement in $L$ if and only if $L/M$ is torsion free.

In the notation of Th. 1, if $L/M$ is torsion free, then $M = M'$, and $M'$ has a complement $L'$ in $L$. Conversely if $M$ has a complement $L'$ in $L$, then $L/M$ is isomorphic to $L'$, which is free (VII, p. 15, Cor. 2), and a fortiori torsion free.

#### Remark {#alg-vii-s4-n3-rem-1 .statement}

It can happen that a submodule $M$ of infinite rank in a free module $L$ can be such that $L/M$ is torsion free, but $M$ has no complement in $L$ (VII, p. 60, Ex. 6, b)).

#### Definition 1 {#alg-vii-s4-def-1 .statement}

— In the notation and hypotheses of Th. 1, the ideals $A\alpha_i$ of $A$ are called the invariant factors of the submodule $M$ with respect to the module $L$.

In the case where $A$ is either the ring $\mathbf{Z}$ of rational integers or the polynomial ring $K[X]$ in one indeterminate over a field $K$, there is a canonical way of choosing a generator for each ideal of $A$: a positive integer in the case of $\mathbf{Z}$, or a monic polynomial in the case of $K[X]$ (VII, p. 5). In each of these cases, the canonical generator of the invariant factor $Aa_i$ is also called an invariant factor of $M$ with respect to $L$, by abuse of language.

### 4. Structure of finitely generated modules

#### Theorem 2 {#alg-vii-s4-thm-2 .statement}

— Every finitely generated module $E$ over a principal ideal domain $A$ is isomorphic to a direct sum of a finite number $m$ of cyclic modules $A/a_k$, where the $a_k$ are ideals of $A$ (some of which may be zero) such that $a_1 \subset a_2 \subset \ldots \subset a_m \neq A$, and which are uniquely determined by these conditions.

If $E$ can be generated by $q$ elements then it is isomorphic to a quotient module $L/M$, where $L = A^q$ (II. p. 218). Since $M$ has finite rank $n \leq q$ (VII, p. 15, Prop. 1), the conditions of Th. 1 (VII, p. 18) are satisfied. Then in the notation of Th. 1 $L/M$ is isomorphic to a direct sum of a complement $L'$ of $M'$ in $L$ and the torsion module $M'/M$. The module $L'$ is free of finite rank $p = q - n$, so isomorphic to $A^p$. If $r$ is the smallest index such that $A\alpha_r \neq A$, then $M'/M$ is isomorphic to the direct sum of modules $A/A\alpha_i$ for $r \leq i \leq n$. The stated conditions will then be satisfied if we take $m = p + (n - r + 1)$, $a_k = (0)$ for $1 \leq k \leq p$, and $a_j = A\alpha_n , - ,$ for $1 \leq j \leq n - r + 1$. Uniqueness follows from the Cor. of VII, p. 16.

#### Corollary 1 {#alg-vii-s4-thm-2-cor-1 .statement}

— *Every finitely generated module E over a principal ideal domain is the direct sum of the torsion submodule of E and a free module.*

The torsion submodule of E has in general several distinct complements. For example, if $E = \mathbf{Z} \times (\mathbf{Z}/(2))$ then the torsion submodule of E is $\{0\} \times (\mathbf{Z}/(2))$; it has as a complement the submodule $\mathbf{Z} \times (0)$, and also the submodule consisting of all elements $(n, \overline{n})$, where $n$ runs through $\mathbf{Z}$ and $\overline{n}$ is the residue class of $n$ mod 2.

#### Corollary 2 {#alg-vii-s4-thm-2-cor-2 .statement}

— *Every torsion free finitely generated module over a principal ideal domain is free of finite rank.*
This follows immediately from Cor. 1.

The condition that the module be finitely generated is essential. For example the additive group of the field of fractions K of A is torsion free as an A-module; however it is not a free module if $A \neq K$, for on the one hand any two elements of K have a common divisor, and on the other hand K is not a cyclic A-module, for otherwise $K = ab^{-1}A$ ($a, b \in A$), whence $b^{-2} = acb^{-1}$ ($c \in A$), so $b^{-1} = ac \in A$, and $K = A$.

#### Definition 2 {#alg-vii-s4-def-2 .statement}

— *In the notation and hypotheses of Th. 2, the ideals $a_k$ are called the invariant factors of the module E.*
As in Def. 1 (VII, p. 19), when $A = \mathbf{Z}$ or $A = K[X]$, the canonical generator of the ideal $a_k$ (a positive integer or a monic polynomial) is also called, by abuse of language, an *invariant factor* of the finitely generated module E.

We must be careful not to confuse the invariant factors of a module E with those of a submodule M of a free module L *with respect to the* module L (Def. I).

### 5. Calculation of invariant factors

#### Proposition 4 {#alg-vii-s4-prop-4 .statement}

— *Let A be a principal ideal domain, let L be a free A-module with finite basis $(u_j)$ ($1 \leq j \leq k$), let M be a submodule of L, let $(x_i)$ be a system of generators of M and let $A \alpha_i$ ($1 \leq i \leq n$) be the invariant factors of M with respect to L. Then for $1 \leq m \leq n$ the product $\delta_m = \alpha_1 \ldots \alpha_m$ is a gcd of the m-th order minors of the matrix whose columns are the coordinate vectors of the $x_i$ with respect to the basis $(u_j)$.

By Th. 1 it is clear that $M \subset \alpha_1 L$; hence the coordinates of any element of M are multiples of $a_1$. On the other hand, there exists an element $x$ of M for which $a_1$ is a content in L. Expressing $x$ as a linear combination of the $x_i$, it follows that $a_1$ is an element of the ideal generated by the coordinates of the $x_i$. As these are all multiples of $a_1$, it follows that $a_1$ is indeed their gcd, and our assertion is proved in the case $m = 1$.

For general $m$, consider the m-th *exterior power* $\bigwedge^m M$ of M (III, p. 507). In the notation of Th. 1 there exists a basis $(a_i)$ for M where $a_i = \alpha_i e_i$ ($1 \leq i \leq n$); thus $\bigwedge^m M$ has a basis consisting of the elements $a_{i_1} \wedge \ldots \wedge a_{i_m}$, as $(i_1, \ldots, i_m)$ runs through the set of strictly increasing sequences of $m$ elements of $(1, n)$. Now the elements $e_{i_1} \wedge \ldots \wedge e_{i_m}$ belong to a basis $B_m$ of $\bigwedge^m L$. Hence the canonical map from $\bigwedge^m M$ into $\bigwedge^m L$ is an isomorphism from $\bigwedge^m M$ onto the submodule of $\bigwedge^m L$ having as a basis the elements $(\alpha_{i_1} \ldots \alpha_{i_m})\, e_{i_1} \wedge \ldots \wedge e_{i_m}$, and we identify this submodule with $\bigwedge^m M$. Since $\alpha_j$ is a multiple of $\alpha_k$ for $j \geq k$, the elements $\alpha_{i_1} \ldots \alpha_{i_m}$ are all multiples of $\delta_m = \alpha_1 \ldots \alpha_m$, and one of them is equal to $\delta_m$; thus $\delta_m$ is a gcd of the coordinates with respect to $B_m$ of the elements of a system of generators of $\bigwedge^m M$. The first part of the argument shows that then $\delta_m$ is a gcd of the set of coordinates of any system of generators of $\bigwedge^m M$, with respect to any basis of $\bigwedge^m L$. Taking the basis for $\bigwedge^m L$ induced from the basis $(u_j)$ of $L$, and the system of generators for $\bigwedge^m M$ consisting of exterior products of the $(x_i)$, the expression for the coordinates of these products in terms of determinants (III, p. 528, Prop. 9) gives the stated result.

### 6. Linear mappings of free modules, and matrices over a principal ideal domain

Let $A$ be a principal ideal domain. Consider a linear mapping $f$ from a free $A$-module $L$ of rank $m$ into a free $A$-module $L'$ of rank $n$. The preceding results allow us, by choosing suitable bases for $L$ and $L'$, to put the matrix for $f$ in a particularly simple form, called the *canonical form* of the matrix.

#### Proposition 5 {#alg-vii-s4-prop-5 .statement}

*Let $A$ be a principal ideal domain, and $f$ a linear map of rank $r$ from a free $A$-module $L$ of rank $m$ into a free $A$-module $L'$ of rank $n$. Then there exist bases $(e_i)$ ($1 \leq i \leq m$) of $L$ and $(e'_j)$ ($1 \leq j \leq n$) of $L'$ such that $f(e_i) = \alpha_i e'_i$ for $1 \leq i \leq r$ and $f(e_i) = 0$ for $i > r$, where the $\alpha_i$ are nonzero elements of $A$, each of which divides the next; the ideals $A \alpha_i$ are the invariant factors of $f(L)$ in $L'$, and are thus uniquely determined.*

Let $L_0 = f^{-1}(0)$ be the kernel of $f$; the quotient $L/L_0$ is isomorphic to the module $f(L)$, which is a submodule of $L'$ and so free (*VII*, p. 15, Cor. 2); thus $L_0$ has a complement $L_1$ in $L$ (*II*, p. 218, Prop. 21), and the restriction of $f$ to $L_1$ is an isomorphism from $L_1$ onto $f(L) = M'$. If the ideals $A \alpha_i$ ($1 \leq i \leq r$) are the invariant factors of $M'$ in $L'$, then Th. 1 of *VII*, p. 18 shows that there exists a basis $(e'_j)$ ($1 \leq j \leq n$) of $L'$ such that $(\alpha_i e'_i)$ ($1 \leq i \leq r$) is a basis of $M'$. Since the restriction of $f$ to $L_1$ is an isomorphism from $L_1$ onto $M'$, there exists a basis $(e_i)$ ($1 \leq i \leq r$) of $L_1$ such that $f(e_i) = \alpha_i e'_i$. This basis extends to a basis $(e_s)$ ($1 \leq k \leq m$) of $L$ by taking $(e_s)$ ($r+1 \leq s \leq m$) to be a basis of the kernel $L_0$.

#### Corollary 1 {#alg-vii-s4-prop-5-cor-1 .statement}

— Let X be a matrix of rank r, with n rows and m columns, over a principal ideal domain A; then there exists a matrix $X_0$ equivalent to X (II, p. 354) of the form

$$
\begin{pmatrix}
\alpha_1 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & \alpha_2 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & \alpha_r & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0
\end{pmatrix}
$$

where the $\alpha_i$ are nonzero elements of A, each of which divides the next. Under these conditions the $\alpha_i$ are uniquely determined up to multiplication by invertible elements.

Given that two matrices X and $X'$ are equivalent if there exist invertible square matrices P and Q, of orders n and m, over A, such that $X' = PXQ$, Cor. 1 is just Prop. 5 expressed in terms of matrices.

In the notation of Prop. 5 and Cor. 1, the (nonzero) ideals $Au$, are called the invariant factors of the linear map f, or of the matrix X. It then follows immediately from Cor. I that:

#### Corollary 2 {#alg-vii-s4-prop-5-cor-2 .statement}

— Two matrices X and $X'$ with n rows and m columns over a principal ideal domain A are equivalent if and only if they have the same invariant factors.

Note that when A is a field we can take the $\alpha_i$ to be equal to 1, and then we recover Prop. 13 of II, p. 360.

If X is the matrix of the linear mapping f with respect to an arbitrary basis of L and an arbitrary basis of L', then the columns of X are the coordinate vectors, with respect to the basis of L', of elements of L' which form a system of generators for $f(L)$. The following result is thus an immediate consequence of Prop. 4.

#### Proposition 6 {#alg-vii-s4-prop-6 .statement}

— Let X be a matrix of rank r over a principal ideal domain A, and let $A \alpha_i$ ($1 \leq i \leq r$) be its sequence of invariant factors. Then $\alpha_1$ is a gcd of the elements of X; and the product $\alpha_1 \ldots \alpha_q$ is a gcd of the q-th order minors of X for $q \leq r$.

### 7. Finitely generated abelian groups

In the case $A = \mathbf{Z}$, the results of section 4 can be expressed

#### Theorem 3 {#alg-vii-s4-thm-3 .statement}

— Every finitely generated abelian group G is a direct sum of its torsion subgroup F (subgroup of elements of finite order in G) und a free abelian group of finite rank p (isomorphic to $\mathbf{Z}^p$). The group F is a direct sum of a finite number of cyclic groups of orders $n_1, n_2, \ldots, n_q$, where the $n_i$ are integers $> 1$, each of which divides the previous one; moreover, the integers $p, q$ and $n_i$ ($1 \leq i \leq q$) are uniquely determined by $G$.

#### Remark {#alg-vii-s4-n7-rem-1 .statement}

While the orders $n_1, \ldots, n_q$ of the cyclic groups of which F is the direct sum are well defined by the divisibility condition of Th. 3, it is *not* the same for the groups themselves: for example, in the product G of $\mathbf{Z}/(p)$ with itself (for p prime), the subgroups are precisely the $\mathbf{F}_p$-vector subspaces, and G is the direct sum of two 1-dimensional subspaces in $p(p+1)$ different ways.

#### Corollary 1 {#alg-vii-s4-thm-3-cor-1 .statement}

— *In a finite abelian group G, there exists an element whose order is the lcm of all the orders of elements of G; this order n is the first invariant factor of G.*

#### Corollary 2 {#alg-vii-s4-thm-3-cor-2 .statement}

— *Any finite abelian group G whose order is not divisible by the square of any integer $> 1$ is cyclic.*
Let us keep to the notation of Th. 3. Then $p = 0$ since G is finite, and $q \leq 1$, for otherwise the order of G would be divisible by $n_q^2$. Hence G is cyclic.

#### Corollary 3 {#alg-vii-s4-thm-3-cor-3 .statement}

— *Let L and M be two free $\mathbf{Z}$-modules of rank n, let $(e_i)$ be a basis for L and $(f_i)$ a basis for M ($1 \leq i \leq n$), let u be a homomorphism from L into M, and let U be its matrix with respect to the bases $(e_i)$ and $(f_i)$. Then $\mathrm{Coker}\,u = M/u(L)$ is finite if and only if $\det(U) \neq 0$, and then $\mathrm{Card}(\mathrm{Coker}(u)) = |\det(U)|$.
By changing bases in L and M if necessary, we may assume that U has the form described in VII, p. 22, Cor. 1 to Prop. 5 (where the $a_i$ are in this case integers); the corollary then becomes obvious, since the order of a direct sum of $\mathbf{Z}$-modules $\mathbf{Z}/\alpha_i \mathbf{Z}$ ($1 \leq i \leq n$) is infinite if one of the $a_i$ is zero, and is equal to $|\alpha_1 \alpha_2 \ldots a_n|$ otherwise.

### 8. Indecomposable modules. Elementary divisors

#### Definition 3 {#alg-vii-s4-def-3 .statement}

— *A left module M over a ring A is said to be decomposable if it is the direct sum of a family of proper nonzero submodules. Otherwise it is said to be indecomposable.*
The zero module is thus *decomposable*, being the direct sum of the empty family of submodules.
Let $\mathfrak{a}$ be a left ideal of the ring A; the submodules of $A/\mathfrak{a}$ are just the quotients $b/\mathfrak{a}$, where $b$ is an ideal of A containing $\mathfrak{a}$ (I, p. 41, Th. 4); if $b$ and $c$ are two ideals of A containing $\mathfrak{a}$, then the module $A/\mathfrak{a}$ is the direct sum of the submodules $b/\mathfrak{a}$ and $c/\mathfrak{a}$ if and only if $A = b + c$ and $b \cap c = \mathfrak{a}$. As a result:

#### Lemma 2 {#alg-vii-s4-lem-2 .statement}

— *The module $A/\mathfrak{a}$ is indecomposable if and only if $\mathfrak{a} \neq A$ and there is no pair $(b, c)$ of ideals of A, distinct from A and $\mathfrak{a}$, such that $A = b + c$ and $b \cap c = \mathfrak{a}$.*

#### Proposition 7 {#alg-vii-s4-prop-7 .statement}

— Let $A$ be a commutative ring, let $\mathfrak{p}$ be a prime ideal of $A$ (I, p. 117, Def. 3), and let $q$ be an ideal of $A$ contained in $\mathfrak{p}$. Suppose that for every $x \in \mathfrak{p}$ there exists an integer $n > 0$ such that $x^n \in q$. Then the $A$-module $A/q$ is indecomposable.

Let $b$ and $c$ be two ideals of $A$, such that $A = b + c$ and $b \cap c = q$. Then $bc \subset b \cap c = q \subset \mathfrak{p}$; if $x \notin \mathfrak{p}$ and $x \in c$, then $xb \subset p$, so $b \subset \mathfrak{p}$ (I, p. 316, Prop. 4); hence either $b \subset \mathfrak{p}$ or $c \subset p$. Suppose for example that $c \subset \mathfrak{p}$, so $b + p = A$; then there exist $x \in b$ and $y \in \mathfrak{p}$ such that $1 = x + y$; let $n \in \mathbf{N}$ be such that $y^n \in q$; then $1 = (x + y)^n$. so $1 \in xA + y^nA \subset b + q \subset b$, so $b = A$. Lemma 2 now shows that $A/q$ is indecomposable.

Now suppose that $A$ is a principal ideal domain; by VII, p. 2, Prop. 2, the prime ideals of $A$ are the ideals $(p)$, where $p$ is an irreducible element of $A$, and the ideal $0$; by the previous proposition, the modules $A$ and $A/(p^n)$, for $p$ irreducible and $n > 0$, are indecomposable. Since every cyclic module is a direct sum of modules of this type (VII, p. 3, Prop. 4) and since every finitely generated $A$-module is a direct sum of cyclic modules (VII, p. 19, Th. 2), we deduce:

#### Proposition 8 {#alg-vii-s4-prop-8 .statement}

— Let $A$ be a principal ideal domain and let $M$ be a finitely generated $A$-module.

a) $M$ is indecomposable if and only if it is isomorphic to $A$ or to a module of the form $A/(p^n)$, where $p$ is an irreducible element of $A$ and $n > 0$ is an integer.

b) $M$ is a direct sum of a finite family of indecomposable submodules.

Part b) of the above proposition can be made more precise as follows:

#### Proposition 9 {#alg-vii-s4-prop-9 .statement}

— Let $A$ be a principal ideal domain, let $P$ be a system of representatives of irreducible elements of $A$ and let $M$ be a finitely generated $A$-module. Then there exist positive integers $m(0)$ and $m(p^n)$ ($p \in P, n > 0$), uniquely determined by $M$ and zero except for finitely many of them, such that $M$ is isomorphic to the direct sum of $A^{m(0)}$ and the $(A/(p^n))^{m(p^n)}$ ($p \in P, n > 0$).

The existence of the integers $m(0)$ and $m(p^n)$ ($p \in P, n > 0$) follows from Prop. 8. The integer $m(0)$ is uniquely determined: it is the rank of the free module which is the quotient of $M$ by its torsion submodule. Finally, the $p$-primary component of $M$ is isomorphic to the direct sum of the $(A/(p^n))^{m(p^n)}$; since the family of ideals $(p^n)$ ($n \geq 1$) is totally ordered by inclusion, the uniqueness of the $m(p^n)$ follows from the Cor. to Prop. 2 of VII, p. 16.

#### Definition 4 {#alg-vii-s4-def-4 .statement}

— In the notation of Prop. 9, those ideals $(p^n)$ ($p \in P, n \geq 1$ an integer) such that $m(p^n) > 0$ are called the elementary divisors of the module $M$, and the integers $m(p^n)$ are called their multiplicities; if the integer $m(0)$ is $> 0$, it is called the multiplicity of the elementary divisor 0.

As for the invariant factors (VII, p. 19, Def. 1), when $A = \mathbf{Z}$ or $A = K[X]$ (K a commutative field), then the canonical generator of the ideal $(p^n)$ (a positive integer or a monic polynomial) is also called, by abuse of language, an elementary divisor of the finitely generated module $M$.

#### Remark 1 {#alg-vii-s4-n8-rem-1 .statement}

If $M$ is a finite abelian group, then its structure can be described by writing down its elementary divisors, each repeated as often as its multiplicity. We will say, for example, that $M$ is « of type $(2, 2, 4, 27, 27, 25)$ » (or that it is « a group $(2, 2, 4, 27, 27, 25)$ ») if it is isomorphic to the product of two groups $\mathbf{Z}/(2)$, one group $\mathbf{Z}/(2^2)$, two groups $\mathbf{Z}/(3^3)$ and one group $\mathbf{Z}/(5^2)$.

#### Remark 2 {#alg-vii-s4-n8-rem-2 .statement}

If a finitely generated torsion module $M$ over a principal ideal domain $A$ is given as a direct sum of cyclic modules isomorphic to $A/(a_i)$ (in particular if the invariant factors of $M$ are known), then the elementary divisors of $M$, and their multiplicities, can be determined by noticing that $A/(a)$ is isomorphic to the product of the $A/(p^{n(p)})$, where $a = e \prod_{p \in P} p^{n(p)}$ is the decomposition of $a$ into irreducible factors ($VII$, p. 3). Let us study for example the multiplicative group $G(464\ 600)$, where $G(n)$ denotes the multiplicative group $(\mathbf{Z}/n\mathbf{Z})^*$ ($VII$, p. 12). Since $464\ 600 = 2^3 \cdot 5 \cdot 23 \cdot 101$, this group is isomorphic to the product of the groups $G(2^3)$, $G(5^2)$, $G(23)$ and $G(101)$ ($VII$, p. 13, Th. 3); now the last three groups are cyclic of orders 20, 22 and 100, and $G(2^3)$ is the product of two cyclic groups of order 2 (\emph{loc. cit.}); since $20 = 2^2 \cdot 5$, $22 = 2 \cdot 11$ and $100 = 2' \cdot 5^2$, the group $G(464\ 600)$ is of type $(2, 2, 2, 2^2, 2^2, 2^2, 5, 5^2, 11)$.

#### Remark 3 {#alg-vii-s4-n8-rem-3 .statement}

To calculate the invariant factors of a torsion module whose elementary divisors are known, we again lean on the fact that, if the $a_i$ are pairwise coprime elements of $A$, then the product $\prod A/(a_i)$ is a cyclic module isomorphic to $A/(a_1 a_2 ... a_n)$ ($VII$, p. 3, Prop. 4). Let us illustrate the method by looking at the example of the group $G(464\ 600) = M$: write the elementary divisors $p^n$ of $M$ which are powers of the same irreducible $p$ on the same line, beginning with those of greatest exponent; extend these lines to lines of equal length by putting in 1's where necessary:

$$
\begin{array}{cccccc}
2^2 & 2^2 & 2 & 2 & 2 \\
5^2 & 5 & 1 & 1 & 1 \\
11 & 1 & 1 & 1 & 1 .
\end{array}
$$

Then the invariant factors are the products of elements in the same column: $1100, 20, 2, 2, 2$. Indeed $M$ is isomorphic to a product of cyclic groups of orders 1100, 20, 2, 2, 2 by Prop. 4 of $VII$, p. 3; since each of these orders is a multiple of the next, these are the invariant factors of $M$ ($VII$, p. 22, Th. 3).

#### Remark 4 {#alg-vii-s4-n8-rem-4 .statement}

An $A$-module is called simple ($I$, p. 37) if it is nonzero and has no submodules other than itself and $0$; it is then necessarily cyclic, so finitely generated, and indecomposable; since the modules $A/(p^n)$ are not simple for $n \neq 1$, while the modules $A/(p)$ are, and since $A$ is simple only if the ring $A$ is a field, we deduce that the simple $A$-modules are:
$a)$ free modules of rank 1, when $A$ is a field;
$b)$ modules isomorphic to quotients $A/(p)$, where $p$ is an irreducible element of $A$, when $A$ is not a field.

### 9. Duality in modules of finite length over a principal ideal domain

In this section $A$ denotes a principal ideal domain which is not a field (and hence has at least one irreducible element), and $K$ the field of fractions of $A$. For every $A$-module $M$, put

$$
D(M) = \operatorname{Hom}_A(M, K/A);
$$

we know that $D(M)$ is equipped with the structure of an A-module in a natural way, namely for every homomorphism $u : M \to K/A$ and every $\alpha \in A$, the homomorphism $\alpha u$ maps $x$ to $\alpha u(x) = u(\alpha x)$. To every homomorphism $f : M \to N$ of A-modules is associated the homomorphism $D(f) : D(N) \to D(M)$, where $D(f)(v) = v \circ f$ (II, p. 196). For $x \in M$ and $x' \in D(M)$, we put $\langle x, x' \rangle = x'(x) \in K/A$ ; then $(x, x') \mapsto \langle x, x' \rangle$ is an *A-bilinear* map from $M \times D(M)$ into $K/A$, called *canonical*.

If M and $N$ are two A-modules, then to every A-bilinear map $\varphi : M \times N \to K/A$ are associated the A-linear maps $d_\varphi : N \to D(M)$ and $s_\varphi : M \to D(N)$, where $d_\varphi(y)(x) = \varphi(x, y) = s_\varphi(x)(y)$ (II, p. 268, Cor. to Prop. *1*). In particular the canonical A-bilinear map $M \times D(M) \to K/A$ defines an A-linear map (also called *canonical*)

$$
c_M : M \to D(D(M))
$$

such that $\langle x', c_M(x) \rangle = \langle x, x' \rangle$ for $x \in M$ and $x' \in D(M)$.

#### Proposition 10 {#alg-vii-s4-prop-10 .statement}

— If *M is an A-module of finite length, then $D(M)$ is* (in general non-naturally) *isomorphic to M, and the canonical map $c_M : M \to D(D(M))$ is an isomorphism.*
Using VII, p. *19*, Th. 2 and **II**, p. 203, Cor. 1, we reduce to the case where $M$ is cyclic. Thus we may suppose that $M = A/tA$ with $t \neq 0$. Note that any homomorphism $u : A/tA \to K/A$ is completely determined by the image $\xi \in K/A$ under $u$ of the class $\varepsilon$ of *1* mod $tA$, and this element must satisfy the relation $t\xi = 0$ ; conversely, for any $\xi \in K/A$ such that $t\xi = 0$, there exists a homomorphism $u : A/tA \to K/A$ such that $u(\varepsilon) = \xi$. It follows that $D(M)$ is isomorphic to $t^{-1}A/A$, and since the homothety by $t$ is a bijection on K, we also have $D(M)$ isomorphic to $A/tA$, which proves the first assertion. This proves that $M$ and $D(D(M))$ are isomorphic, so have the same length ; on the other hand $c_M$ is injective, for if $y \in A$ is such that the relation $tz \in A$ (for $z \in K$) implies $yz \in A$, then taking $z = t^{-1}$ we have $y \in tA$. It follows that the image $c_M(M)$ is necessarily equal to $D(D(M))$.

#### Corollary {#alg-vii-s4-n9-cor-1 .statement}

— *Let M, N be two A-modules of finite length, and let $\varphi$ be an A-bilinear map from $M \times N$ into $K/A$, such that : 1) the relation $\varphi(x, y) = 0$ for all $y \in N$ implies $x = 0$ ; and 2) the relation $\varphi(x, y) = 0$ for all $x \in M$ implies $y = 0$. Then the A-linear maps $s_\varphi : M \to D(N)$ and $d_\varphi : N \to D(M)$ associated to $\varphi$ are isomorphisms.*
Indeed the hypotheses on $\varphi$ mean that $s_\varphi$ and $d_\varphi$ are *injective* and since $\mathrm{long}(D(N)) = \mathrm{long}(N)$ and $\mathrm{long}(D(M)) = \mathrm{long}(M)$ by Prop. *10*, this implies that $\mathrm{long}(M) = \mathrm{long}(N)$, and consequently $s_\varphi$ and $d_\varphi$ are bijective.

#### Proposition 11 {#alg-vii-s4-prop-11 .statement}

— *If $M' \xrightarrow{u} M \xrightarrow{v} M''$ is an exact sequence of A-modules of finite length, then the sequence $D(M'') \xrightarrow{D(v)} D(M) \xrightarrow{D(u)} D(M')$ is exact* [^1].

Let us show first of all that given an exact sequence

(1)
$$
0 \to M' \to M \to M'' \to 0
$$

the corresponding sequence

$$
0 \to D(M'') \to D(M) \to D(M') \to 0
$$

is exact; indeed we know that the sequence

$$
0 \to D(M'') \to D(M) \to D(M')
$$

is exact (II, p. 227, Th. 1); on the other hand, it follows from (1) that

$$
\operatorname{long}(M) = \operatorname{long}(M') + \operatorname{long}(M'')
$$

(II, p. 212, Prop. 16); by Prop. 10 we thus have

$$
\operatorname{long}(D(M)) = \operatorname{long}(D(M')) + \operatorname{long}(D(M''))
$$

in other words $\operatorname{long}(D(M')) = \operatorname{long}(D(M)/D(M''))$. Since $D(M)/D(M'')$ is naturally identified with a submodule of $D(M')$, it must be equal to $D(M')$, which proves our assertion.

This implies immediately that if $u : M' \to M$ is injective, then $D(u) : D(M) \to D(M')$ is surjective; the conclusion then follows from II, p. 199, remark 4.

For every A-module M, let $\mathfrak{S}(M)$ denote the set of submodules of M. For every submodule N of M (resp. every submodule N' of D(M)), let $N^0$ (resp. ${N'}^0$) denote the submodule of $D(M)$ (resp. M) consisting of those $x' \in D(M)$ (resp. $x \in M$) such that $(y, x') = 0$ for all $y \in N$ (resp. $(x, y') = 0$ for all $y' \in N'$).

#### Proposition 12 {#alg-vii-s4-prop-12 .statement}

*Let M be an A-module of finite length. Then the map which sends every submodule N of M to $N^0$ is a bijection from $\mathfrak{S}(M)$ onto $\mathfrak{S}(D(M))$, and the inverse bijection sends every submodule N' of D(M) to the submodule ${N'}^0$ of M; the module $D(N)$ is naturally identified with $D(M)/N^0$ and $D(M/N)$ with $N^0$. Moreover, we have*

(2)
$$
(N_1 + N_2)^0 = N_1^0 \cap N_2^0, \quad (N_1 \cap N_2)^0 = N_1^0 + N_2^0
$$

for all submodules $N_1, N_2$ of M.

For each submodule N of M, there is an exact sequence

$$
0 \to N \to M \to M/N \to 0
$$

and hence (Prop. 11) an exact sequence

$$
0 \to D(M/N) \to D(M) \to D(N) \to 0
$$

and since the image of $D(M/N)$ in $D(M)$ is obviously $N^0$, we see (Prop. 10) that $\operatorname{long}(N^0) = \operatorname{long}(M) - \operatorname{long}(N)$; since $M$ is identified with $D(D(M))$ by Prop. 10, we have similarly

$$
\operatorname{long}(N^{00}) = \operatorname{long}(M) - \operatorname{long}(N^0) = \operatorname{long}(N);
$$

in addition it is clear that $N \subset N^{00}$, so $N^{00} = N$. Furthermore the first relation in (2) is obvious, and by applying it to the submodules $N_1^0$ and $N_2^0$ of $D(M)$, we have $(N_1^0 + N_2^0)^0 = N_1 \cap N_2$, so $N_1^0 + N_2^0 = (N_1^0 + N_2^0)^{00} = (N_1 \cap N_2)^0$. This completes the proof of the proposition.

#### Example 1 {#alg-vii-s4-n9-exa-1 .statement}

For $A = \mathbf{Z}$, the $\mathbf{Z}$-modules of finite length are precisely the finite abelian groups; then $K = \mathbf{Q}$, so $K/A = \mathbf{Q}/\mathbf{Z}$. Then to define $D(M)$, we sometimes take, instead of $\mathbf{Q}/\mathbf{Z}$, a $\mathbf{Z}$-module isomorphic to it, such as (V, p. 79, Prop. 2) the group $R$ of roots of unity (under multiplication) in an algebraically closed field of characteristic 0 ; we then put $D(M) = \operatorname{Hom}_{\mathbf{Z}}(M, R)$. We leave the reader to rewrite the preceeding results for this special case in the corresponding notation.

#### Example 2 {#alg-vii-s4-n9-exa-2 .statement}

Let $a$ be a nonzero element of $A$. The map $x \mapsto x/a$ from $A$ into $K$ induces an isomorphism on quotient modules from $A/(a)$ onto the submodule $(K/A)(a)$ of $K/A$ consisting of elements annihilated by $a$. If $M$ is an $A$-module annihilated by $a$, or equivalently an $A/(a)$-module, then the $A$-module $D(M)$ is identified with $\operatorname{Hom}_{A/(a)}(M, A/(a))$. We leave the reader to rewrite the preceding results for this special case in the corresponding notation (cf. V, p. 86).

### Exercises {#alg-vii-s4-exercises}

See the [exercises for § 4](exercises/s4/).

[^1]: We will see later (A, X, p. 18) that the A-module K/A is injective. It follows that Prop. 11 remains valid for arbitrary A-modules M, M' and M".
