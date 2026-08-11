---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Simple Modules
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.45-A VIII.54
pdf_pages: 0062-0071
extraction: native
subsections:
    - "no": 1
      title: Simple Modules
      page: 45
      pdf_page: 62
    - "no": 2
      title: Schur’s Lemma
      page: 47
      pdf_page: 64
    - "no": 3
      title: Maximal Submodules
      page: 48
      pdf_page: 65
    - "no": 4
      title: Simple Modules over an Artinian Ring
      page: 50
      pdf_page: 67
    - "no": 5
      title: Classes of Simple Modules
      page: 51
      pdf_page: 68
statements: 21
exercises: 10
content_sha256: bff4b36855d84372e48ee844b0f9e58c694e1d3c3aefe7f5ff2288527b337fc5
---

## § 3. SIMPLE MODULES

### 1. Simple Modules

Recall the following definition (II, §1, No. 10, p. 212).

#### Definition 1 {#alg-viii-s3-def-1 .statement tag=0035}

Let A be a ring. An A-module M is called simple if it is nonzero and has no submodule distinct from 0 and M.

An A-module M is simple if and only if M is a simple module over its ring of homotheties $A_M$. Every simple module is indecomposable, of length 1, and therefore primordial (VIII, p. 31, Proposition 4, b)).

#### Example 1 {#alg-viii-s3-n1-exa-1 .statement tag=0036}

The module $A_s$ is a simple A-module if and only if A is a field (I, §9, No. 1, p. 115, Theorem 1). The simple A-modules are then the vector spaces of dimension 1 over the field A.

#### Example 2 {#alg-viii-s3-n1-exa-2 .statement tag=0037}

Let A be a principal ideal domain (VII, §1, No. 1, p. 1, Definition 1) that is not a field. For every irreducible element $\pi$ of A, the A-module $A_s/(\pi )$ is simple, and every simple A-module is isomorphic to such a module (VII, §4, No. 8, p. 25, Remark 4). For $n\geqslant 2$, the A-module $A_s/(\pi^n)$ is indecomposable (VII, §4, No. 8, p. 24, Proposition 8) but not simple.

#### Example 3 {#alg-viii-s3-n1-exa-3 .statement tag=0038}

Let K be a field, V a nonzero right vector space over the field K, and A a subring of the ring End$_K(V)$ containing the endomorphisms of V of finite rank (for example, A = End$_K(V))$. Let us prove that V is a simple A-module: let W be a nonzero A-submodule of V and $x$ a nonzero element of W; there exists a linear form $\varphi$ on V such that $\varphi (x)\not= 0$ (II, §7, No. 5, p. 300, Theorem 6). For every $y$ in V, the mapping $z\mapsto y\varphi (z)$, which is linear of rank $\leqslant 1$, belongs to A; we therefore have $Ax= V$, hence a fortiori W = V, which proves that V is a simple A-module. **Proposition 1.** — Let A be a ring.

a) Let $\mathfrak{m}$ be a left ideal of A. The A-module $A_s/\mathfrak{m}$ is simple if and only if $\mathfrak{m}$ is a maximal left ideal.

b) Let M be a simple A-module, and let $x$ be a nonzero element of M. We have the equality $M = Ax$, the annihilator $\mathfrak{m}$ of $x$ is a maximal left ideal of A, and the mapping $a\mapsto ax$ defines, by passing to the quotient, an isomorphism from $A_s/\mathfrak{m}$ to M.

c) Let M be a nonzero A-module. If we have $M = Ax$ for every nonzero element $x$ of M, then M is simple.

The submodules of $A_s/\mathfrak{m}$ are of the form $\mathfrak{n}/\mathfrak{m}$, where $\mathfrak{n}$ is a left ideal of A containing $\mathfrak{m}$ (I, §4, No. 6, p. 41, Theorem 4); consequently, the A-module $A_s/\mathfrak{m}$ is simple if and only if we have $\mathfrak{m}\not= A$ and every left ideal $\mathfrak{n}$ of A containing $\mathfrak{m}$ satisfies $\mathfrak{n}/\mathfrak{m}= 0$ or $\mathfrak{n}/\mathfrak{m}= A_s/\mathfrak{m}$, that is, $\mathfrak{n}=\mathfrak{m}$ or $\mathfrak{n}= A$. This proves a).

Under the assumptions of b), $Ax$ is a nonzero submodule of M, hence is equal to M. Consequently, the mapping $a\mapsto ax$ defines, by passing to the quotient, an isomorphism from $A_s/\mathfrak{m}$ to M; the A-module $A_s/\mathfrak{m}$ is therefore simple, and the left ideal $\mathfrak{m}$ is maximal by a). This proves b).

Under the assumptions of c), let N be a nonzero submodule of M. If $x$ is a nonzero element of N, then we have $Ax\subset N$ and $Ax= M$, and therefore M = N. Hence M is simple.

#### Corollary 1 {#alg-viii-s3-def-1-cor-1 .statement tag=0039}

If the ring A is not reduced to 0, then there exist simple A-modules.

Indeed, by Krull’s theorem (I, §8, No. 6, p. 104, Theorem 1), there exist maximal left ideals of A.

#### Corollary 2 {#alg-viii-s3-def-1-cor-2 .statement tag=003A}

Let A be a local ring (VIII, p. 26, Definition 1) and $\mathfrak{r}$ its maximal ideal. The A-module $A_s/\mathfrak{r}$ is simple, and every simple A-module is isomorphic to $A_s/\mathfrak{r}$.

#### Remark 1 {#alg-viii-s3-n1-rem-1 .statement tag=003B}

Let A be a commutative ring and $\mathfrak{m}$ an ideal of A. Then $\mathfrak{m}$ is the annihilator (II, §1, No. 12, p. 219, Definition 11) of the A-module $A_s/\mathfrak{m}$. Hence, if $\mathfrak{m}$ and $\mathfrak{m}'$ are distinct ideals of A, then the A-modules $A_s/\mathfrak{m}$ and $A_s/\mathfrak{m}'$ are not isomorphic. There exists a faithful simple A-module (II, §1, No. 12, p. 219) if and only if (0) is a maximal ideal of A, that is, A is a field.

#### Remark 2 {#alg-viii-s3-n1-rem-2 .statement tag=003C}

We can give an example of a noncommutative ring A and two distinct maximal left ideals $\mathfrak{m}$ and $\mathfrak{m}'$ of A such that the A-modules $A_s/\mathfrak{m}$ and $A_s/\mathfrak{m}'$ are isomorphic (VIII, p. 52, Exercise 3).

### 2. Schur’s Lemma

#### Proposition 2 {#alg-viii-s3-prop-2 .statement tag=003D}

Let A be a ring, M and N two A-modules, and $f$ a nonzero homomorphism from M to N.

a) If M is simple, then $f$ is injective.

b) If N is simple, then $f$ is surjective.

c) If M and N are simple,then $f$ is an isomorphism.

The kernel of $f$ is a proper submodule of M, and the image of $f$ is a nonzero submodule of N.

a) If M is simple, then we have Ker($f) = 0$, so $f$ is injective.

b) If N is simple, then we have Im($f) = N$, so $f$ is surjective.

c) If M and N are simple, then $f$ is both injective and surjective.

Corollary (Schur’s lemma). — The endomorphism ring of a simple module is a field.

If M is a simple A-module, then every nonzero element of the nonzero ring End$_A(M)$ is invertible (Proposition 2, c)), so End$_A(M)$ is a field.

#### Theorem 1 {#alg-viii-s3-thm-1 .statement tag=003E}

Let K be an algebraically closed commutative field, A a K-algebra, and M a simple A-module. Suppose that the dimension of M as a vector space over K is finite or, more generally, strictly less than the cardinal of K. Then the endomorphism ring of the A-module M consists of the homotheties $\alpha_M$ with $\alpha \in K$.

Let E be the endomorphism ring of the A-module M; it is a field by the corollary of Proposition 2 and an algebra over the field K. If we view M as a left vector space over the field E, then we have dim$_KM =$ (dim$_EM)[E : K]$ by Proposition 25 of II, §1, No. 13, p. 222, hence dim$_KM\geqslant [E : K]$. Since dim$_KM<$ Card(K) by assumption, the equality $E = K\cdot 1_M$ is then a consequence of the following lemma.

#### Lemma 1 {#alg-viii-s3-lem-1 .statement tag=003F}

Let E be a field and K a subfield of the center of E not equal to E. If the field K is algebraically closed, then we have $[E : K]\geqslant$ Card(K).

Let $x$ be an element of E K and L the (commutative) subfield of E generated by $K\cup  \{x\}$. Since K is algebraically closed, $x$ is transcendent over K. By VII, §2, No. 3, p. 10, Theorem 2 and p. 11, the elements $(x-\alpha )^{-1}$ of L, where $\alpha$ runs through K, are linearly independent over K. We therefore have $[E : K]\geqslant [L : K]\geqslant$ Card(K).

#### Example {#alg-viii-s3-n2-exa-1 .statement tag=003G}

$*$ Let A be a $\mathbf{C}$-algebra generated by a countable family of elements; it has countable dimension over $\mathbf{C}$. Let M be a simple A-module; it is monogenous, so admits a countable basis over $\mathbf{C}$. Since the field $\mathbf{C}$ is not countable (Gen. Top., IV, §4, No. 1, p. 44), we have $[M :\mathbf{C}]<$ Card($\mathbf{C})$. Therefore the endomorphisms of the A-module M are the homotheties $\alpha_M$ with $\alpha \in \mathbf{C}$. This applies, in particular, when A is the universal enveloping algebra of a finite-dimensional Lie algebra over $\mathbf{C}($Lie, I, §2, No. 7, p. 21, Corollary $3).*$

#### Corollary 1 {#alg-viii-s3-lem-1-cor-1 .statement tag=003H}

Keep the assumptions of Theorem 1, and suppose, moreover, that the algebra A is commutative. Then M has dimension 1 over K.

Since the ring A is commutative, $a_M$ is an endomorphism of the A-module M for every $a\in A$. By Theorem 1, we therefore have $A_M= K\cdot 1_M$, and M is a simple K-module, that is, a 1-dimensional vector space over the field K.

#### Corollary 2 {#alg-viii-s3-lem-1-cor-2 .statement tag=003I}

Let K be a commutative field, A a K-algebra, and M an A-module. Suppose that for every extension L of K, the $A_{(L)}$-module $M_{(L)}$ is simple. Then the endomorphism ring of M consists of the homotheties $\alpha_M$ with $\alpha \in K$.

Let I be a set of cardinal strictly greater than the dimension of M over K (for example, the set of subsets of M). Let L be an algebraic closure of the field $K((X_i)_{i\in I})$ (V, §4, No. 3, p. 23, Theorem 2). Choose a K-linear form $\varphi$ on L such that $\varphi (1) = 1$, and let $v: M_{(L)}\rightarrow M$ be the K-linear mapping characterized by $v(\alpha \otimes m) =\varphi (\alpha )m$. Let $u$ be an endomorphism of M. The dimension of $M_{(L)}$ over L is equal to that of M over K and is strictly less than the cardinal of L. By Theorem 1, the endomorphism $1_L\otimes u$ of the $A_{(L)}$-module $M_{(L)}$ is of the form $\lambda \otimes 1_M$ with $\lambda \in L$. For every $x\in M$, we have

$$
u(x) =v1\otimes u(x)=v(1_L\otimes u)(1\otimes x)
$$

$$
=v(\lambda \otimes 1_M)(1\otimes x)=v(\lambda \otimes x) =\varphi (\lambda )x
$$

so that $u$ is the homothety $\varphi (\lambda )_M$.

### 3. Maximal Submodules

#### Definition 2 {#alg-viii-s3-def-2 .statement tag=003J}

Let A be a ring and M an A-module. A maximal submodule of M is a maximal element, for the inclusion, of the set of proper submodules of M.

A maximal submodule of $A_s$ is simply a left maximal ideal of A.

Let N be a submodule of M. The submodules of $M/N$ are of the form $P/N$, where P is a submodule of M containing N (I, §4, No. 6, p. 41, Theorem 4). Consequently, N is a maximal submodule of M if and only if the module $M/N$ is simple.

#### Proposition 3 {#alg-viii-s3-prop-3 .statement tag=003K}

Let M be a finitely generated A-module. Every proper submodule of M is contained in a maximal submodule.

Let N be a proper submodule of M. Denote by $\mathscr{S}$ the set of proper submodules of M containing N, ordered by inclusion; let us prove that $\mathscr{S}$ is inductive. Let $\mathscr{F}$ be a totally ordered subset of $\mathscr{S}$. If $\mathscr{F}$ is empty, then N is an upper bound for $\mathscr{F}$ in $\mathscr{S}$. In the opposite case, denote by Q the union of the elements of $\mathscr{F}$. Then Q is a submodule of M. Let F be a finite generating subset of M. If Q were equal to M, then F would be contained in a submodule $P\in \mathscr{F}$, which would imply P = M, contrary to the definition of $\mathscr{F}$. We therefore have $Q\in \mathscr{S}$, which proves that $\mathscr{S}$ is inductive. Proposition 3 then follows from Corollary 1 of Set Theory, III, §2, No. 4, p. 155.

#### Corollary 1 {#alg-viii-s3-prop-3-cor-1 .statement tag=003L}

Let M be a nonzero finitely generated A-module. There exists a two-sided ideal $\mathfrak{a}$ of A, annihilator of a simple A-module, such that $\mathfrak{a}M$ is not equal to M.

Let N be a maximal submodule of M (Proposition 3), and let $\mathfrak{a}$ be the annihilator of the simple A-module $M/N$; it is a two-sided ideal of A, and we have $\mathfrak{a}(M/N) = 0$, whence $\mathfrak{a}M\subset N$ and consequently $\mathfrak{a}M\not= M$.

#### Corollary 2 {#alg-viii-s3-prop-3-cor-2 .statement tag=003M}

Let A be a commutative ring and B an A-algebra. Let M be a simple B-module that is a finitely generated A-module, and let $\mathfrak{m}$ be the annihilator of the A-module M. Then $\mathfrak{m}$ is a maximal ideal of A, and M is a finite-dimensional vector space over the field $A/\mathfrak{m}$.

Since the ring A is commutative, the annihilator of a simple A-module is a maximal ideal of A (VIII, p. 46, Proposition 1). By Corollary 1 applied to the A-module M, there exists a maximal ideal $\mathfrak{a}$ of A such that $\mathfrak{a}M\not= M$. But $\mathfrak{a}M$ is a submodule of the simple B-module M; we therefore have $\mathfrak{a}M = 0$ and consequently $\mathfrak{a}\subset \mathfrak{m}$. Since the ideal $\mathfrak{m}$ is distinct from A, it is equal to $\mathfrak{a}$, so that $\mathfrak{m}$ is maximal. The module M is a finitely generated module over the field $A/\mathfrak{m}$; the last assertion follows.

### 4. Simple Modules over an Artinian Ring

Let A be a ring. By abuse of language, we say that a left ideal $\mathfrak{a}$ is a minimal left ideal of A if it is a minimal element of the set of nonzero left ideals of A, ordered by inclusion. We define right minimal ideals and two-sided minimal ideals analogously.

Let $\mathfrak{a}$ be a left ideal of A. Then $\mathfrak{a}$ is a simple A-module if and only if it is a minimal left ideal of A.

Every nonzero left ideal of a left Artinian (VIII, p. 1, Definition 1) ring contains a minimal left ideal.

#### Proposition 4 {#alg-viii-s3-prop-4 .statement tag=003N}

Let A be a ring that has a minimal left ideal $\mathfrak{a}$. Every faithful simple A-module is isomorphic to the A-module $\mathfrak{a}$.

Let M be a faithful simple A-module. Let $\alpha$ be a nonzero element of $\mathfrak{a}$. Since the A-module M is faithful, there exists an element $x$ of M such that $\alpha x\not= 0$. The homomorphism $a\mapsto ax$ from $\mathfrak{a}$ to M is then nonzero; it is therefore an isomorphism by Proposition 2 of VIII, p. 47.

#### Proposition 5 {#alg-viii-s3-prop-5 .statement tag=003O}

Let A be a left Artinian ring and M a faithful A-module.

a) There exist a natural number $m$ and an isomorphism from $A_s$ to a submodule of $M^m$.

b) If M admits a Jordan–Hölder series $(M_i)_{0\leqslant i\leqslant n}$, then every simple A-module is isomorphic to one of the quotients $M_i/M_{i+1}$.

By VIII, p. 2 applied to the A-module $A_s$ and the annihilators of the elements of M, there exist elements $x_1, . . . , x_m$ of M such that the annihilator of M is the intersection of the annihilators of the $x_i$. Since the A-module M is faithful, the A-linear mapping $a\mapsto (ax_1, . . . , ax_m)$ from $A_s$ to $M^m$ is injective, whence a).

Under the assumption of b), every simple quotient of $A_s$ is isomorphic to a quotient of a Jordan–Hölder series of $M^m$ (I, §4, No. 7, p. 43, Corollary), hence to one of the modules $M_i/M_{i+1}$ (I, §4, No. 7, p. 43, Theorem 6). We conclude that every simple A-module is isomorphic to a quotient of $A_s$.

#### Remark {#alg-viii-s3-n4-rem-1 .statement tag=003P}

Proposition 5 applies, in particular, to the following two cases:

a) Let A be an algebra over a commutative field K, and let M be a faithful finite-dimensional module over K. Then M is an A-module of finite length, and the countermodule of M is finitely generated. The ring A is left Artinian (VIII, p. 9, Proposition 6). There exists a Jordan–Hölder series $(M_i)_{0\leqslant i\leqslant n}$ of the A-module M, and every simple A-module is isomorphic to one of the modules $M_i/M_{i+1}$ for $0\leqslant i\leqslant n-1$.

b) Let A be a left Artinian ring. The module $A_s$ has finite length (VIII, p. 6, Theorem 1). Since the A-module $A_s$ has finite length, there exists a decreasing sequence $(\mathfrak{a}_i)_{0\leqslant i\leqslant n}$ of left ideals of A such that $\mathfrak{a}_0= A$ and $\mathfrak{a}_n= 0$ and that the A-modules $S_i=\mathfrak{a}_{i-1}/\mathfrak{a}_i$ are simple for $1\leqslant i\leqslant n$. Then every simple A-module is isomorphic to one of the modules $S_1, . . . ,S_n$.

### 5. Classes of Simple Modules

Denote by Is$_A(X,Y)$ the relation

“A is a ring and $X,Y$ are isomorphic A-modules.”

This is an equivalence relation with respect to X and Y. If X is an A-module, then we denote the class of objects equivalent to X for Is$_A$ by cl(X) and call it the class of the A-module X (Set Theory, II, §6, No. 9, p. 122). By definition, cl(X) is an A-module isomorphic to X; moreover, two A-modules X and Y are isomorphic if and only if we have cl(X) = cl(Y).

Let A be a ring. The relation

“$\lambda$ is a class of finitely generated A-modules”

is collectivizing in $\lambda ($Set Theory, II, §1, No. 4, p. 68). Indeed, every finitely generated A-module is isomorphic to an A-module of the form $A^n_s/R$, where $n$ is a natural number and R a submodule of $A^n_s$, so that our assertion follows from Set Theory, II, §6, No. 9, p. 122.

We denote the set of classes of finitely generated A-modules by $\mathscr{F}(A)$. Every simple A-module is monogenous (VIII, p. 46, Proposition 1), and consequently the classes of the simple A-modules form a subset of $\mathscr{F}$ (A), which we from now on denote by $\mathscr{S}(A)$ (or simply $\mathscr{S})$. When the ring A is commutative, the mapping $\mathfrak{m}\mapsto$ cl(A$/\mathfrak{m})$ is a bijection from the set of maximal ideals of A to the set $\mathscr{S}(A)$ (loc. cit. and VIII, p. 46, Remark 1). When A is left Artinian, the set $\mathscr{S}(A)$ is finite (VIII, p. 51, Remark b)).

### Exercises {#alg-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
