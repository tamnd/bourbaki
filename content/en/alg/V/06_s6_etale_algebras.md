---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 6
section_title: Etale algebras
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.26-A V.36, A V.151
pdf_pages: 0140-0150, 0265-0265
extraction: ocr
subsections:
    - "no": 1
      title: Linear independence of homomorphisms
      page: 26
      pdf_page: 140
    - "no": 2
      title: Algebraic independence of homomorphisms
      page: 28
      pdf_page: 142
    - "no": 3
      title: Diagonalizable algebras and etale algebras
      page: 28
      pdf_page: 142
    - "no": 4
      title: Subalgebras of an etale algebra
      page: 30
      pdf_page: 144
    - "no": 5
      title: Separable degree of a commutative algebra
      page: 31
      pdf_page: 145
    - "no": 6
      title: Differential characterization of etale algebras
      page: 33
      pdf_page: 147
    - "no": 7
      title: Reduced algebras and etale algebras
      page: 34
      pdf_page: 148
statements: 22
exercises: 2
content_sha256: 1e1d8007a12d561b9aab4fe1f0fdc218310c13da2cf43b259e24998de8869633
---

## § 6. ETALE ALGEBRAS

Throughout this paragraph K denotes a field.

### 1. Linear independence of homomorphisms

Let L be an extension of K and V a vector space over K. In this paragraph we shall denote by $ \operatorname{Hom}_K(V, L) $ the set of all K-linear mappings of V into L, equipped with the vector space structure on L such that:

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

for $x \in V,\ a \in L$ and $f,\ g$ in $\mathrm{Hom}_K(V, L)$. Let $V_{(L)} = L \otimes_K V$ be the vector space on L derived from V by extension of scalars, and $(V_{(L)})^*$ its dual. By II, p. 277 we have a canonical isomorphism $u \mapsto 3$ of vector L-spaces from $(V_{(L)})^*$ onto $\mathrm{Hom}_K(V, L)$ such that $\tilde{u}(x) = u(1 \otimes x)$ for $x \in V$ and $u$ in $(V_{(L)})^*$. If V is of *finite* dimension $n$ over $K$, the vector space $(V_{(L)})$ over $L$ is of dimension $n$, as well as its dual $(V_{(L)})^* = V_{(\bar{L})}^*$, whence the formula

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### Theorem 1 {#alg-v-s6-thm-1 .statement}

— *Let L be an extension of a field K and A an algebra over K; let $\mathcal{H}$ be the set of all K-algebra homomorphisms of A into L. Then $\mathcal{H}$ is a free subset of the vector space $\mathrm{Hom}_K(A, L)$ over L.*

Let us show by induction on the integer $n \geq 0$ that every sequence $(u_1, \ldots, u_n)$ of distinct elements of $\mathcal{H}$ is free. The case $n = 0$ being trivial, we may henceforth suppose that $n \geq 1$; let $a_1, \ldots, a_n$ be elements of L such that $$\sum_{i=1}^n \alpha_i u_i = 0.$$ For $x,\ y$ in A we have
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
whence $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ By the induction hypothesis, the elements $u_1, \ldots, u_{n-1}$ of $\mathcal{H}$ are linearly independent, whence $\alpha_i [u_i(x) - u_n(x)] = 0$ for $1 \leq i \leq n-1$ and for all $x$ in A. Since the $u_i$ are distinct, this implies that $\alpha_i = 0$ for $i \neq n$, hence $\alpha_n u_n = 0$ and so $\alpha_n = \alpha_n u_n(1) = 0$ (on denoting by 1 the unit element of A). We have thus shown that $a_1, \ldots, a_{n-1}, \alpha_n$ are zero, and this proves the theorem.

#### Corollary 1 {#alg-v-s6-thm-1-cor-1 .statement}

— *Let $\Gamma$ be a monoid, L a field and X a set of homomorphisms of $\Gamma$ into the multiplicative monoid of L. Then X is a free subset of the vector L-space $L^\Gamma$ of mappings of $\Gamma$ into L.*

Let A be the algebra of the monoid $\Gamma$ with coefficients in L and $(e,)_{\gamma}$, the canonical basis of A over L (III, p. 446). For every L-linear mapping $u$ of A into L let us write $\tilde{u}(\gamma) = u(e,\gamma)$ (for $\gamma \in \Gamma$); then the mapping $u \mapsto 3$ is an isomorphism of vector L-spaces of $\mathrm{Hom}_L(A, L)$ onto $L^\Gamma$ which maps onto X the set of L-algebra homomorphisms of A into L. Now it suffices to apply Th. 1 with $K = L$.

**COROLLARY 2** (Dedekind's theorem). — *Let E and L be two extensions of K. The set of K-homomorphisms of E into L is free over L. If E is of finite degree over K, the number of K-homomorphisms of E into L is at most equal to $[E : K]$.*

The last assertion follows from the first, taking account of Formula (2).

### 2. Algebraic independence of homomorphisms

#### Theorem 2 {#alg-v-s6-thm-2 .statement}

— Let K be an infinite field, L an extension of K and A an algebra over K. Let $ u_1, \ldots, u_n $ be distinct K-algebra homomorphisms of A into L and f a polynomial in $ L[X_1, \ldots, X_j] $. If we have $ f(u_1(x), \ldots, u_n(x)) = 0 $ for all $ x \in A $, then $ f = 0 $.

Let B be the set of elements of $ L^n $ of the form $ (u_1(x), \ldots, u_n(x)) $ with $ x \in A $. By Th. 1, there is no sequence $ (a,, \ldots, a,) $ of elements not all zero in L such that $ \sum_{i=1}^n \alpha_i u_i(x) = 0 $ for all $ x \in A $; therefore (II, p. 301, Th. 7) B generates the vector space $ L^n $ over L. So there exist elements $ a,, \ldots, a, $ of $ A $ such that the matrix $ (u_i(a_j))_{1 \leq i,j \leq n} $ is invertible.

Let us define the polynomial $ g \in L[Y_1, \ldots, Y_n] $ by
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
Let $ y_1, \ldots, y, $ be in $ K $; writing $ x = \sum_{i=1}^n y_i a_i $, we have
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
whence $ g(y_1, \ldots, y_n) = 0 $
by the hypothesis on $ f $. Since the field $ K $ is infinite, we have $ g = 0 $ (IV, p. 18, Cor. 2); now the matrix $ (u_i(a_j)) $ has an inverse $ (b_{ij}) $ and we have
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
whence $ f = 0 $.

Th. 2 has no analogue for finite fields. Thus let $ K $ be a finite field with q elements, $ A = L = K $ and $ f(X) = X^q - X $. We have $ x^q = x $ for all $ x \in K $ (V, p. 93, Prop. 2); therefore if $ u $ is the identity automorphism of $ K $, we have $ f(u(x)) = 0 $ for all $ x \in K $, even though $ f $ is not zero.

### 3. Diagonalizable algebras and etale algebras

#### Definition 1 {#alg-v-s6-def-1 .statement}

— Let A be an algebra over K; then A is said to be diagonalizable if there exists an integer $ n \geq 0 $ such that A is isomorphic to the product algebra $ K^n $. We say that A is diagonalized by an extension L of K if the algebra $ A_{(L)} $ over L derived from A by extension of scalars is diagonalizable. We shall say that A is etale if there exists an extension of K which diagonalizes A.

We recall that the product algebra $ K'' $ is the vector space $ K'' $ equipped with the product defined by

$$
(x_1, \ldots, x_n) \cdot (y_1, \ldots, y_n) = (x_1 y_1, \ldots, x_n y_n)
$$

If $ \varepsilon_1, \ldots, \varepsilon_n $ is the canonical basis of $ K^n $, we have

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{if} \quad i \neq j
$$

and $ 1 = \varepsilon_1 + \ldots + \varepsilon_n $.

Every etale algebra over $ \mathbf{K} $ is *commutative* and of *finite degree* over $ K $.

#### Proposition 1 {#alg-v-s6-prop-1 .statement}

*Let A be an algebra of finite degree n over the field K ; then the following conditions are equivalent :*
  *a)* *The algebra A is diagonalizable.*
  *b)* *There is a basis $ (e_1, \ldots, e_n) $ of A such that $ e_i^2 = e_i $ and $ e_i e_j = 0 $ for $ i \neq j $.*
  *c)* *The K-algebra homomorphisms of A into $ \mathbf{K} $ generate the dual of the vector K-space A.*
  *d)* *Every A-module is a direct sum of submodules which are of dimension 1 over K.*

The equivalence of *a)* and *b)* follows from Formula (6); on the other hand the n projections $ K^n \to K $ are algebra homomorphisms, hence *a)* implies *c)*. If *c)* holds, the algebra homomorphisms of A into $ \mathbf{K} $ form a basis of the dual of A (*V*, p. 27, Th. 1), we denote them by $ u_1, \ldots, u_n $; then $ a \mapsto (u_i(a)) $ is an isomorphism of A onto the algebra $ K'' $, whence *a)*. We have thus established the equivalence of the conditions *a)*, *b)* and *c)*.

Suppose that *b)* holds and let M be an A-module; then the homotheties $ (e_i)_M $ of ratio $ e_i $ are projectors of $ M $, and $ M $ is a direct sum of the $ e_i M $, which are sub-A-modules. We may thus suppose that there exists an index $ i $ such that $ (e_j)_M = 0 $ for $ j \neq i $. Hence every vector subspace of $ M $ is a sub-A-module, whence *d)*.

Conversely suppose that *d)* holds and consider the A-module A,. There exists then a basis $ (f_i) $ of the vector K-space A such that $ Af_i = Kf_i $ for $ i = 1, \ldots, n $. After replacing each $ f_i $ by a suitable scalar multiple, if necessary, we may suppose that $ 1 = f_i + \ldots + f_n $. If $ i \neq j $, then $ f_i f_j $ belongs to $ Af_i \cap Af_j = Kf_i \cap Kf_j $ hence it is zero. Now $ f_i = f_i f_1 + \ldots + f_i f_n = f_i^2 $, whence *b)*.

#### Corollary {#alg-v-s6-n3-cor-1 .statement}

*Let L be an extension of K and $ \mathcal{H} $ the set of algebra homomorphisms of A into L. We have Card $ \mathcal{H} \leq [A : K] $, with equality if and only if A is diagonalized by L. If A is diagonalized by L, then $ \mathcal{H} $ is a basis of the vector L-space $ \mathrm{Hom}_K(A, L) $.*

The vector space $ \mathrm{Hom}_K(A, L) $ over L has dimension $ [A : K] $, by Formula (2), and $ \mathcal{H} $ is a free subset of $ \mathrm{Hom}_K(A, L) $ by Th. 1 (*V*, p. 27). We thus have Card $ \mathcal{H} \leq [A : K] $ with equality if and only if $ \mathcal{H} $ is a basis of $ \mathrm{Hom}_K(A, L) $. There exists an isomorphism of vector L-spaces, say $ \pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^* $, characterized by $ u(x) = (\pi u)(1 \otimes x) $ for $ x \in A $, and $ \pi $ maps $ \mathcal{H} $ onto the set $ \mathcal{H}_L $ of L-algebra homomorphisms of $ A(\cdot) $ into L. Finally the equivalence of $ a) $ and $ c) $ in Prop. 1 shows that the algebra $ A_{(L)} $ over L is diagonalizable if and only if $ \mathcal{H}_L $ generates the vector space $ A_{(L)}^* $ over L. This completes the proof of the Corollary.

#### Proposition 2 {#alg-v-s6-prop-2 .statement}

— *Let A be an algebra over K and $ \Omega $ an algebraically closed extension of K. The following assertions are equivalent*:

$ a) $ *The algebra A is etale*.
$ b) $ *There exists an extension of finite degree which diagonalizes A*.
$ c) $ *The extension $ \Omega $ of K diagonalizes A*.

Suppose that A is etale. Let $ n $ be the degree of A over K, let L be an extension of K which diagonalizes A and let $ \mathcal{H} $ be the set of algebra homomorphisms of A into L. By the Cor. to Prop. 1 we have Card $ \mathcal{H} = n $. On the other hand, for each $ u \in \mathcal{H} $, we have $[u(A):K] \leq n$. By V, p. 18, Th. 2, the subextension L' of L generated by the images of elements of $ \mathcal{H} $ is of finite degree over K. Since there exist $ n $ distinct homomorphisms of A into L', the extension L' diagonalizes A, by the Cor. 1 of Prop. 1. This shows that a) implies b).

Since every extension of finite degree of K is isomorphic to a subextension of $ \Omega $ (V, p. 20, Th. 1), b) implies c). Finally c) clearly implies a).

### 4. Subalgebras of an etale algebra

#### Proposition 3 {#alg-v-s6-prop-3 .statement}

— *Let A be an etale algebra over K. There exist only a finite number of subalgebras and ideals of A. Moreover, every extension of K which diagonalizes A also diagonalizes every subalgebra and every quotient algebra of A; in particular these algebras are etale*.

It suffices to show that an algebra $ K^n $ has only a finite number of subalgebras and ideals, and that the subalgebras and quotient algebras of $ K^n $ are diagonalizable. We denote by $ (\varepsilon_1, \ldots, \varepsilon_n) $ the canonical basis of $ K^n $.

Let A be a subalgebra of $ K^n $ and let $ v_1, \ldots, v_n $ be the restrictions to A of the n projections $ K^n \to K $. Since the intersection of the kernels of the $ v_i $ is clearly 0, the $ v_i $ generate the vector K-space dual to A (II, p. 302, Cor. 1); hence the K-algebra A is diagonalizable (V, p. 29, Prop. 1).

For every subset I of $ \{1, 2, \ldots, n\} $ put $ \varepsilon_I = \sum_{i \in I} \varepsilon_i $. It is clear that the elements $ \varepsilon_I $ are idempotents of $ K^n $; we have $ \varepsilon_I = 0 $ if and only if I is empty, and $ \varepsilon_I \varepsilon_J = \varepsilon_{I \cap J} $. By what has been said, every subalgebra A of $ K^n $ is diagonalizable; by condition $ b) $ of Prop. 1 every subalgebra A of $ K^n $ therefore admits a basis $ (\varepsilon_{I_1}, \ldots, \varepsilon_{I_p}) $, where $ (I_1, \ldots, I_p) $ is a partition of $ \{1, 2, \ldots, n\} $, and there are only a finite number of such subalgebras.

For every subset I of $ (1, 2, \ldots, n) $ let $ a_i $ be the vector subspace of $ K^n $ having as basis the idempotents $ \varepsilon_i $ for $ i \in I $; then it is clear that $ a_i $ is an ideal of $ K^n $; moreover if $ J = (1, 2, \ldots, n) - I $, then the residue classes $ \overline{\varepsilon}_j $ of $ \varepsilon_j $ mod $ a_i $, for $ j \in J $ form a basis of $ K^n / a_i $. We have $ \overline{\varepsilon}_j^2 = \overline{\varepsilon}_j $ and $ \overline{\varepsilon}_j \overline{\varepsilon}_k = 0 $ if $ j \neq k $, hence the algebra $ K^n / a_I $ is diagonalizable, by Prop. 1 of V, p. 29.

It remains to show that every ideal of $ K^n $ is of the form $ a_I $. Let I be the set of integers $ i $ such that $ 1 \leq i \leq n $ and $ \varepsilon_i \in a $, then $ a_i \subset a $. Let $ x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n $ be an element of $ a $ (with $ x_1, \ldots, x_n $ in $ K $) and let $ i $ be in $ (1, 2, \ldots, n) - I $. We have $ x_i \varepsilon_i = x \varepsilon_i \in a_i $, and $ \varepsilon_i \notin a $, whence $ x_i = 0 $. Thus $ x = \sum_{i \in I} x_i \varepsilon_i $ and this shows that $ x \in a_i $. We have now shown $ a \subset a_I $, whence finally $ a = a_i $.

#### Corollary {#alg-v-s6-n4-cor-1 .statement}

— *Let $ A_1, \ldots, A_r $ be algebras over $ K $ and $ A = A_1 \times \cdots \times A_r $. For $ A $ to be etale it is necessary and sufficient that $ A_1, \ldots, A_r $ are etale.*

Suppose that $ A $ is etale; each of the algebras $ A_1, \ldots, A_r $ is isomorphic to a quotient of $ A $, and hence is etale by Prop. 3. Conversely, every extension of $ K $ which diagonalizes $ A_1, \ldots, A_r $ clearly diagonalizes $ A $.

### 5. Separable degree of a commutative algebra

Let $ A $ be a commutative algebra of finite degree $ n $ over $ K $. For any extension $ L $ of $ K $, the number $ h(L) $ of algebra homomorphisms of $ A $ into $ L $ is finite and is bounded above by $ n $ (V, p. 29, Cor.).

#### Lemma 1 {#alg-v-s6-lem-1 .statement}

— *Let $ \Omega $ be an algebraic closure of $ K $; then we have $ h(L) \leq h(\Omega) $ for every extension $ L $ of $ K $, with equality when $ L $ is algebraically closed.*

Let $ L' $ be the algebraic closure of $ K $ in $ L $. For every homomorphism $ u $ of $ A $ into $ L $ we have $ [u(A) : K] \leq n $, hence $ u(A) \subset L' $ by V, p. 18, Prop. 2; we thus have $ h(L') = h(L) $. Since the extension $ L' $ of $ K $ is isomorphic to a subextension of $ \Omega $ (V, p. 20, Th. 1), we have $ h(L') \leq h(\Omega) $. If $ L $ is algebraically closed, then $ L' $ is an algebraic closure of $ K $; the extensions $ L' $ and $ \Omega $ of $ K $ are then isomorphic (V, p. 23, Th. 2) and so $ h(L') = h(\Omega) $; the Lemma follows directly from this.

By Lemma 1, the number $ h(L) $ has the same value for all algebraically closed extensions $ L $ of $ K $; this number will be denoted by $ [A : K] $, and called the *separable degree* of $ A $.

Let $ A $ and $ B $ be two commutative algebras of finite degree over $ K $. We shall establish the formula

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

Let $ L $ be an algebraically closed extension of $ K $ and denote by $ \mathcal{H}(A) $ the set of algebra homomorphisms of $ A $ into $ L $, and similarly define $ \mathcal{H}(B) $ and $ \mathcal{H}(A \otimes_K B) $. By definition we have Card $ \mathcal{H}(A) = [A : K] $, and corresponding formulae for [B : K], and [A \otimes_K B : K]. Moreover (III, p. 465, Formula (6)), the formula $(u * v)(a \otimes b) = u(a)v(b)$ defines a bijection $(u, v) \mapsto u * v$ of $\mathcal{H}(A) \times \mathcal{H}(B)$ onto $\mathcal{H}(A \otimes_K B)$, whence Formula (7) follows.

Let $K'$ be an extension of $K$; we shall prove the formula
$$
[A_{(K')}: K'], = [A: K], .
$$
For take $L$ to be an algebraic closure of $K'$. The formula $\tilde{u}(x) = u(1 \otimes x)$ (for $x \in A$) defines a bijection $u \mapsto \tilde{u}$ between the set of $K'$-homomorphisms of $A_{(K')}$ into $L$ and the set of $K$-homomorphisms of $A$ into $L$, whence (8).

Finally, suppose that $K'$ is an extension of finite degree of $K$; if $A'$ is a commutative $K'$-algebra of finite degree, then it is also a commutative $K$-algebra of finite degree and we have $[A': K] = [A': K'] \cdot [K': K]$ (V. p. 10, Th. 1). We shall prove the formula
$$
[A': K], = [A': K']_s \cdot [K': K], .
$$
For let $S$ (resp. $T$) be the set of $K$-homomorphisms of $K'$ (resp. $A'$) into an algebraic closure $L$ of $K$; for every $\sigma \in S$ we denote by $T_\sigma$ the set of elements $f$ of $T$ such that $f(a \cdot 1) = \sigma(a)$ for all $a \in K'$. Then the family $(T_\sigma)_\sigma$ is a partition of $T$ and we have Card $S = [K': K]$; now for each $\sigma \in S$ the set $T_\sigma$ consists of $K'$-homomorphisms of $A'$ into the algebraically closed extension $(L, \sigma)$ of $K'$, hence Card $T_\sigma = [A': K']_s$, and so we have proved (9).

#### Proposition 4 {#alg-v-s6-prop-4 .statement}

— Let $A$ be a commutative algebra of finite degree over $K$; then $[A: K], \leq [A: K]$ with equality if and only if $A$ is etale.

Let $\Omega$ be an algebraic closure of $K$ and $A?$ the set of algebra homomorphisms of $A$ into $\mathbf{R}$. We have Card $A? = [A: K]$, and $A$ is etale if and only if $A$ is diagonalized by the extension $\Omega$ of $K$ (V, p. 30, Prop. 2). Thus Prop. 4 follows from the Cor. of V, p. 29.

#### Corollary 1 {#alg-v-s6-prop-4-cor-1 .statement}

— Let $A, B$ be two commutative algebras over $K$, of finite non-zero degrees. Then for the algebra $C = A \otimes_K B$ to be etale it is necessary and sufficient for $A$ and $B$ to be etale.

We have $[C: K] = [A: K] \cdot [B: K]$ and the corresponding Formula (7) for the separable degrees. Further we have $[A: K], \leq [A: K]$ and corresponding formulae for $B$ and $C$. It follows that $[C: K] = [C: K]$, if and only if we have both $[A: K] = [A: K]$, and $[B: K] = [B: K]$; now it is enough to apply Prop. 4.

#### Corollary 2 {#alg-v-s6-prop-4-cor-2 .statement}

— Let $K'$ be an extension of $K$.

a) For a $K$-algebra $A$ to be etale, it is necessary and sufficient that the $K'$-algebra $A_{(K')}$ should be etale.

b) Let $A'$ be an algebra over $K'$, not reduced to 0. For $A'$ to be etale over $K$ it is necessary and sufficient that $A'$ should be etale over $K'$ and $K'$ etale over $K$.

We argue as for Cor. 1, applying this time (8) for $a)$ and (9) for $b)$.

### 6. Differential characterization of etale algebras

#### Theorem 3 {#alg-v-s6-thm-3 .statement}

— Let $ A $ be a commutative algebra of finite degree over $ K $. For $ A $ to be etale it is necessary and sufficient that the module $ \Omega_K(A) $ of $ K $-differentials of $ A $ should be reduced to $ 0 $.

$ A) $ Let $ L $ be an algebraic closure of $ K $ ($ V $, p. 23, Th. 2). For $ A $ to be etale it is necessary and sufficient that the algebra $ A_{(L)} $ over $ L $ should be diagonalizable ($ V $, p. 30, Prop. 2). Further, the $ A $-module $ \Omega_L(A_{(L)}) $ is isomorphic to $ \Omega_K(A) \otimes_A A_{(L)} $ (III, p. 572, Prop. 20), hence to $ \Omega_K(A) \otimes_K L $, by the associativity of the tensor product; therefore $ \Omega_K(A) = 0 $ is equivalent to $ \Omega_L(A_{(L)}) = 0 $. To prove Th. 3 it is therefore enough to consider the case where $ K $ is algebraically closed and to show that the algebra $ A $ is diagonalizable if and only if $ \Omega_K(A) = 0 $.

$ B) $ Suppose that $ A $ is diagonalizable; then ($ V $, p. 29, Prop. 1), the vector space $ A $ is generated by the idempotents of $ A $. The assertion $ \Omega_K(A) = 0 $ is thus a consequence of the following lemma:

#### Lemma 2 {#alg-v-s6-lem-2 .statement}

— Let $ A $ be a commutative algebra over $ K $ and $ e $ an idempotent of $ A $; then we have $ de = 0 $ in $ \Omega_K(A) $.

From the relation $ e = e^2 $ we deduce $ de = 2e \cdot de $; on multiplying by $ e $ we obtain $ e \cdot de = 2e \cdot de $, hence $ e \cdot de = 0 $, and so finally, $ de = 2e \cdot de = 0 $.

$ C) $ We first prove two lemmas:

#### Lemma 3 {#alg-v-s6-lem-3 .statement}

— Let $ A $ be a commutative algebra of finite degree over the algebraically closed field $ K $, such that $ \Omega_K(A) = 0 $. Then we have $ m = m^2 $ for every maximal ideal $ m $ of $ A $.

The algebra $ A/m $ is an extension of finite degree of the algebraically closed field $ K $, whence $[A/m : K] = 1$. Hence for each $ a \in A $ there exists a unique scalar $ \lambda $ such that $ a - \lambda \cdot 1 \in m $; write $ D(a) $ for the residue class of $ a - \lambda \cdot 1 $ mod $ m^2 $. It is clear that $ D $ is a $ K $-derivation of $ A $ into the $ A $-module $ m/m^2 $. The universal property of $ \Omega_K(A) $ (III, p. 569) and the hypothesis $ \Omega_K(A) = 0 $ now imply that $ D = 0 $, whence $ m/m^2 = 0 $ and so $ m = m^2 $.

#### Lemma 4 {#alg-v-s6-lem-4 .statement}

— Let $ A $ be a commutative ring and let $ a $ be a finitely generated ideal of $ A $ such that $ a = a^2 $. Then there exists an idempotent $ e $ in $ A $ such that $ a = Ae $.

Let $ (a,, ..., a,) $ be a generating system of the ideal $ a $; since $ a = a^2 $, there exist elements $ x_{ij} $ in $ a $ such that $ a_i = \sum_{j=1}^r x_{ij} a_j $ for $ 1 \leq i \leq r $. Write $ M $ for the square matrix of order $ r $ whose elements are $ \delta_{ij} - x_{ij} $ and let $ D $ be its determinant. There exists (III, p. 532, Formula (26)) a square matrix $ N $ of order $ r $ with elements in $ A $ such that $ N \cdot M = D \cdot I $, whence immediately $ Da_j = 0 $ for $ 1 \leq j \leq r $ and so finally $ Da = 0 $. Now the matrix $ M $ is congruent to $ I $, mod $ a $, hence $ D \equiv I $ mod $ a $. Put $ e = 1 - D $; then $ e \in a $ and $ ex = x $ for all $ x \in a $. It follows that $ e $ is an idempotent and $ a $ is equal to $ Ae $.

With these lemmas established, let us show by induction on the degree of $ A $ that $ A $ is diagonalizable if $ K $ is algebraically closed and $ \Omega_K(A) = 0 $. Let $ m $ be a maximal ideal of $ A $ (I, p. 104). By Lemmas 3 and 4, there exists an idempotent $ e $ such that $ m = Ae $; we have seen that $ A/m $ is of degree 1 over $ K $. Hence $ A $ is a direct sum of the ideals $ a = (1 - e)A $ and $ m $ and we have $ [a : K] = 1 $, hence $ A $ is isomorphic to $ K \times A/a $. Since $ \Omega_K(A/a) $ is isomorphic to a quotient of $ \Omega_K(A) $ (III, p. 573, Prop. 22), it is zero and the induction hypothesis shows that $ A/a $ is diagonalizable. This then shows $ A $ to be diagonalizable.

### 7. Reduced algebras and etale algebras

#### Definition 2 {#alg-v-s6-def-2 .statement}

— *Let $ A $ be a commutative ring; then $ A $ is said to be reduced if every nilpotent element (I, p. 98) of $ A $ is zero.*

If $ A $ is a field, or an integral domain, or a product of reduced rings, it is a reduced ring. For a commutative ring $ A $ to be reduced it is necessary and sufficient that $ a^2 \neq 0 $ for every $ a \neq 0 $ in $ A $: for from this we obtain by induction on $ n $, $ a^{2^n} \neq 0 $, hence $ a^n \neq 0 $ for any $ a \neq 0 $ in $ A $.

An algebra is said to be *reduced* if its underlying ring is reduced.

#### Proposition 5 {#alg-v-s6-prop-5 .statement}

— *Let $ A $ be a commutative algebra of finite degree over $ K $. For $ A $ to be reduced it is necessary and sufficient that there exist extensions $ L_1, \ldots, L_s $ of finite degree over $ K $ such that $ A $ is $ K $-isomorphic to $ L_1 \times \cdots \times L_s $.*

The stated condition is clearly sufficient.

Conversely, assume that $ A $ is reduced; arguing by induction on the degree of $ A $ we see that it suffices to prove that if $ A $ is not a field, there exist two non-zero algebras $ A_1 $ and $ A_2 $ such that $ A $ is isomorphic to $ A_1 \times A_2 $, or also that there exists in $ A $ an idempotent different from 0 and 1.

Suppose from now on that $ A $ is reduced and is not a field. Among the ideals of $ A $ different from 0 and $ A $ let $ a $ be an ideal whose dimension as vector $ K $-space is minimal. For any $ x \neq 0 $ in $ a $ we have $ x^2 \neq 0 $, because $ A $ is reduced, whence $ a' \neq \{0\} $. We have $ a^2 \subset a $ and by the minimality of $ a $ we find that $ a' = a $. By Lemma 4 there exists an idempotent $ e $ such that $ a = Ae $, and we have $ e \neq 0, e \neq 1 $ because $ a $ is distinct from 0 and $ A $.

#### Theorem 4 {#alg-v-s6-thm-4 .statement}

— *Let $ A $ be a commutative algebra of finite degree over $ K $. Then the following assertions are equivalent:
a) The algebra $ A $ is etale.
b) For every extension $ L $ of $ K $, the ring $ L \otimes_K A $ is reduced.
c) There exists a perfect extension field $ P $ of $ K $ such that the ring $ P \otimes_K A $ is reduced.
d) There exist separable algebraic extensions $ L_1, \ldots, L_s $ of $ K $ such that $ A $ is isomorphic to $ L_1 \times \cdots \times L_s $.*
In particular, every etale algebra is reduced.

A) Let us first prove the equivalence of $a$, $b$ and $c$.

Suppose that $A$ is etale and let $L$ be an extension of $K$. Let $\Omega$ be an algebraically closed extension field of $L$ (V, p. 23, Th. 2). Then $L \otimes_K A$ is isomorphic to a subring of $\Omega \otimes_K A$ and the latter is isomorphic to a ring $\Omega^n$ by Prop. 2 (V, p. 30). Therefore the ring $L \otimes_K A$ is reduced.

We have thus shown that $a)$ implies $b)$, and $c)$ is a particular case of $b)$. Assume now that $c)$ holds. For the K-algebra $A$ to be etale it is necessary and sufficient that the P-algebra $A_{(P)}$ should be etale (V, p. 32, Cor. 2). The algebra $A$ is therefore etale by the following lemma:

#### Lemma 5 {#alg-v-s6-lem-5 .statement}

*Let B be a reduced algebra of finite degree over a perfect field P; then B is etale.*

By Prop. 5 there exist extensions $L_1, \ldots, L_n$ of $P$ such that $B$ is isomorphic to the algebra $L, x \ldots x L_n$. Since a finite product of etale algebras is etale (V, p. 31, Cor.) it is enough to examine the case where $B$ is an extension of $P$. By Th. 3 (V, p. 33) it is enough to show that $dx = 0$ in $\Omega_P(B)$ for all $x \in B$.

Let $x \in B$; since $B$ is of finite degree over $K$, $x$ is algebraic over $K$ (V, p. 18, Prop. 2). Let $f$ be the minimal polynomial of $x$ and let $f'$ be the derivative off. The polynomial $f$ is non-constant. Suppose that $f' = 0$; by V, p. 9, Cor. the field $P$ is of characteristic $p \neq 0$ and we have $f \in P[X^p]$; since $P$ is perfect, we have $P[X^p] = P[X]^p$, but the irreducible polynomial $f$ cannot lie in $P[X]^p$.

We thus have $f' \neq 0$ and since the degree of $f'$ is strictly less than that off, we have $f'(x) \neq 0$. Now from $f(x) = 0$ we deduce $f(x) \cdot dx = 0$ in $\Omega_P(B)$, whence $dx = 0$, as we had to show.

*B) Suppose that $A$ is etale; by the equivalence of $a)$ and $b)$ the algebra $A$ is reduced, so there exist extensions $L_1, \ldots, L_n$ of $K$ such that $A$ is isomorphic to $L_1 \times \cdots \times L_n$ (Prop. 5). Since $A$ is etale, each of the extensions $L_i$ is an etale algebra (V, p. 31, Cor.), and hence by definition is a separable algebraic extension of $K$.

The implication $d) \Rightarrow a)$ follows from V, p. 31, Cor. \*

#### Corollary {#alg-v-s6-n7-cor-1 .statement}

— *Suppose that $K$ has characteristic $p \neq 0$. For $A$ to be etale it is necessary and sufficient that $A = K[A^p]$. For every basis $(a_i)_i$, of $A$ over $K$, the family $(a_i^p)_i$ is then a basis of $A$ over $K$.*

Let us choose an algebraic closure $\Omega$ of $K$. Given two $K$-homomorphisms $u$ and $v$ of $A$ into $\Omega$, if $u$ and $v$ have the same restriction to $K[A^p]$, we have

$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p,
$$

whence $u(x) = v(x)$

for all $x \in A$. We thus have the inequality $[A : K], \leq [K[A^p] : K]_s$; if $A$ is etale, we thus have

$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$

whence $A = K[A^p]$

Conversely suppose that we have $ A = K[A^p] $; let $ (a_i)_{i \in I} $ be a basis of $ A $ over $ K $. By $ V $, p. 4, Prop. 2, b), the family $ (a_i^p)_{i \in I} $ generates the vector $ K $-space $ K[A^p] $ and since $ A = K[A^p] $ is of finite dimension equal to the cardinal of $ I $, the family $ (a_i^p)_{i \in I} $ is a basis of $ A $ over $ K $. Let $ u $ be an element of $ \Omega \otimes_K A $ such that $ u^2 = 0 $, whence $ u^p = 0 $; since $ (a_i)_{i \in I} $ is a basis of $ A $ over $ K $, there exists a family $ (\lambda_i)_{i \in I} $ of elements of $ \Omega $ such that $ u = \sum_{i \in I} \lambda_i \otimes a_i $, whence $ u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p $. Since $ (a_i^p)_{i \in I} $ is a basis of $ A $ over $ K $ and $ u^p = 0 $, we must have $ \lambda_i^p = 0 $, whence $ \lambda_i = 0 $ for all $ i \in I $, and so $ u = 0 $. This shows the ring $ \Omega \otimes_K A $ to be reduced; since $ \Omega $ is perfect, the algebra $ A $ over $ K $ is etale by Th. 4.

For another characterization of etale algebras see $ V $, p. 48, Prop. 1.

### Exercises {#alg-v-s6-exercises}

See the [exercises for § 6](exercises/s6/).
