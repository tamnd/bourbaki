---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 2
section_title: Torsion modules over a principal ideal domain
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.6-A VII.14, A VII.54-A VII.59
pdf_pages: 0365-0373, 0413-0418
extraction: ocr
subsections:
    - "no": 1
      title: Modules over a product of rings
      page: 6
      pdf_page: 365
    - "no": 2
      title: Canonical decomposition of a torsion module over a principal ideal domain
      page: 7
      pdf_page: 366
    - "no": 3
      title: 'Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate'
      page: 10
      pdf_page: 369
    - "no": 4
      title: 'Applications : II. The multiplicative group of units of the integers modulo a'
      page: 12
      pdf_page: 371
statements: 16
exercises: 15
content_sha256: 97d9eb4cdec80e2771b1c17555ea38f2de9fce79c4beef410353e551f5136a5e
---

## § 2. TORSION MODULES OVER A PRINCIPAL IDEAL DOMAIN

### 1. Modules over a product of rings

Let $ A $ be a ring and $ (b_i)_{i \in I} $ a direct decomposition of $ A $, that is (I, p. 110, Def. 7) a finite family of two-sided ideals of $ A $ such that the natural homomorphism from $ A $ into the product of the $ A/b_i $ is bijective. By *loc. cit.*, Prop. 10, there exists a family $ (e_i)_{i \in I} $ of central idempotents of $ A $ such that $ b_i = A(1 - e_i) $, $ \sum_{i \in I} e_i = 1 $ and $ e_i e_j = 0 $ for $ i \neq j $.

For every left $ A $-module $ M $, let $ M_i $ denote the set of $ m \in M $ such that $ b_i m = 0 $; since $ b_i $ is a two-sided ideal, this is a submodule of $ M $; moreover, if $ a, b \in A $ and $ a - b \in b_i $, then the homotheties $ a_{M_i} $ and $ b_{M_i} $ coincide; there is thus a unique $ (A/b_i) $-module structure on $ M_i $ such that the $ A $-module structure of $ M_i $ is induced via the homomorphism $ A \to A/b_i $.

#### Proposition 1 {#alg-vii-s2-prop-1 .statement}

The $ A $-module $ M $ is the direct sum of its submodules $ M_i $.

Let $ p_i : M \to M $ denote the homothety $ m \mapsto e_i m $; the map $ p_i $ is $ A $-linear since $ e_i $ is central; since $ e_i^2 = e_i $, $ \sum_{i \in I} e_i = 1 $ and $ e_i e_j = 0 $ for $ i \neq j $, we have

$$
p_i \circ p_i = p_i , \quad \sum_{i \in I} p_i = 1_M , \quad p_i \circ p_j = 0 \quad \text{for} \quad i \neq j ,
$$

and the $ p_i $ form an orthogonal family of projectors whose sum is the identity (II, p. 209, Def. 7). By *loc. cit.*, Prop. 12, the module M is the direct sum of the submodules $ p_i(M) = e_iM $. In addition $ e_iM $ is annihilated by $ b_i = A(1 - e_i) $; if $ i \neq j $ and $ m \in M $ then $ (1 - e_i)e_jm = e_jm $, whence no nonzero element of $ e_jM $ is annihilated by $ 1 - e_i $, and so a fortiori by $ b_i $. It follows that $ e_iM = M_i $, and the proposition is proved.

#### Remark {#alg-vii-s2-n1-rem-1 .statement}

— 1) Conversely, let $ M'_i $ be an $ (A/b_i) $-module for each i, and consider the A-module M, the direct sum of the A-modules $ M'_i $; then the submodules $ M_i $ constructed above coincide with the $ M'_i $ (it is enough to note that if $ i \neq j $ then no nonzero element of $ M'_j $ is annihilated by $ b_i $ because $ b_i + b_j = A $). Thus, roughly speaking, it amounts to the same thing to consider an A-module M or a family $ (M_i) $ of modules over the rings $ A/b_i = A_i $.

2) By the above proof, the projectors of M onto the components $ M_i $ are homotheties.

3) The A-module M is cyclic if and only if each $ M_i $ is cyclic: if $ M = Am $, then $ M_i = A_i e_i m $; conversely if $ M_i = A_i m_i $ and $ m = \sum_{i \in I} m_i $, then $ M = Am $; indeed, if $ n \in M $ projects onto $ a_i m_i $ for each i, and if $ a \in A $ is congruent to $ a_i $ mod $ b_i $ for each i, then am and n have the same image in each $ M_i $, so coincide.

4) Let M and N be two A-modules, with components $ (M_i) $ and $ (N_i) $. Let $ u \in \mathrm{Hom}_A(M, N) $ be an A-linear map from M to N; then for all i and for all $ m \in M_i $ we have $ u(m) \in N_i $, so u induces an $ A_i $-linear map $ u_i \in \mathrm{Hom}_{A_i}(M_i, N_i) $. It is easy to check that the map $ u \mapsto (u_i) $ is an isomorphism of Z-modules (resp. of A-modules when A is commutative)

$$
\mathrm{Hom}_A(M, N) \to \prod_{i \in I} \mathrm{Hom}_{A_i}(M_i, N_i).
$$

### 2. Canonical decomposition of a torsion module over a principal ideal domain

Let M be a module over a commutative ring A. For each $ a \in A $ let $ M(\alpha) $ denote the kernel of the endomorphism $ x \mapsto \alpha x $ of M. If $ a $ and $ \beta $ are two elements of A such that $ \alpha $ divides $ \beta $, then clearly $ M(a) \subset M(\beta) $. In particular, as n runs through the set of rational integers $ \geq 1 $, the submodules $ M(\alpha^n) $ form an increasing sequence; the union $ M $, of the $ M(\alpha^n) $ is thus a submodule of M, consisting of those elements of M which are annihilated by some power of a. For each submodule N of M, it is clear that $ N_1 = N \cap M_a $.

#### Definition 1 {#alg-vii-s2-def-1 .statement}

Let $ \pi $ be an irreducible element of a principal ideal domain A; an A-module M is called rr-primary *if*, for all $ x \in M $, there exists an integer $ n \geq 1 $ such that $ \pi^n x = 0 $ (in other words, if M is equal to the submodule $ M_\pi $).

Clearly every cyclic module of the form $ A/(\pi^s) $ is rr-primary. For an arbitrary A-module M, the submodule $ M_\pi $ is rr-primary.

#### Lemma 1 {#alg-vii-s2-lem-1 .statement}

— Let M be a module over a principal ideal domain A; for all $ a \in A $ such that $ a \neq 0 $, let $ \alpha = \varepsilon \sum_{i=1}^r \pi_i^{n(i)} $ be a decomposition of $ \alpha $ into irreducible factors (VII, p. 4). The submodule $ N = M(a) $ of elements of M annihilated by a is the direct sum of the submodules $ M(\pi_i^{n(i)}) $, and the map which sends each $ x \in M(\alpha) $ to its component in $ M(\pi_i^{n(i)}) $ has the form $ x \mapsto \gamma_i x \ (\gamma_i \in A) $. Moreover
$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}
$$
Note first that N is annihilated by a, so has a natural $ A/(\alpha) $-module structure. By Prop. 4 of VII, p. 3, the canonical homomorphism from $ A/(\alpha) $ into the product of the rings $ A/(\pi_i^{n(i)}) $ is a ring isomorphism; now applying Prop. 1 of VII, p. 6, we deduce that N is the direct sum of the $ M(\pi_i^{n(i)}) $; the projectors of this decomposition are homotheties, by VII, p. 7, Remark 2. The inclusion $ M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i} $ is obvious; conversely, let $ x \in M(\alpha) \cap M_{\pi_i} $. Then there exists a power $ \pi_i^s $ of $ \pi_i $ which annihilates x; we may assume $ s \geq n(i) $; by Bezout's identity, there exist $ \lambda, \mu \in A $ such that $ \pi_i^{n(i)} = \lambda \pi_i^s + pa $, so $ \pi_i^{n(i)} x = 0 $ and so finally $ x \in M(\pi_i^{n(i)}) $.

#### Lemma 2 {#alg-vii-s2-lem-2 .statement}

— Let M be a torsion module (II, p. 313) over an integral domain A. For every finite family $ (x_i)_{1 \leq i \leq n} $ of elements of M, there exists an element $ \gamma \neq 0 $ in A such that the $ x_i $ all belong to $ M(\gamma) $.
Indeed, for each index i there exists an element $ \alpha_i \neq 0 $ in A which annihilates $ x_i $, and the element $ \gamma = \prod_{i=1}^n \alpha_i $ will fit the bill.

Theorem 1. — Let M be a torsion module over a principal ideal domain A; for each irreducible element $ \pi $ of A, let $ M_\pi $ be the submodule of M consisting of elements annihilated by some power of $ \pi $. If P is a system of representatives of irreducible elements of A, then M is the direct sum of its submodules $ M_\pi $ for $ \pi \in P $.
Every element $ x \in M $ belongs to the submodule $ M(\alpha) $ for some $ a \neq 0 $, so by Lemma 1 is a sum of a finite number of elements, each of which belongs to some submodule $ M_\pi $. On the other hand, if $ \sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi $, where $ x_\pi, y_\pi \in M_\pi $ for all $ \pi \in P $, and where all but finitely many of the $ x_\pi $ and $ y_\pi $ are zero, then Lemma 2 shows that there exists $ \gamma \neq 0 $ in A such that all the $ x_\pi $ and $ y_\pi $ belong to the same submodule $ M(\gamma) $; applying Lemma 1 to $ M(\gamma) $ shows that $ x_\pi = y_\pi $ for all $ \pi \in P $, which completes the proof.

Clearly, if $ \pi $ and $ \pi' $ are two associate irreducible elements, then $ M_\pi = M_{\pi'} $; thus, for a given module M, the submodule $ M_\pi $ depends only on the ideal $ (\pi) $ of A; it is called the rr-primary component of the module M, and the decomposition of M as a direct sum of the $ M_\pi $ is called the canonical decomposition of M as a direct sum of its rr-primary components.

#### Corollary 1 {#alg-vii-s2-lem-2-cor-1 .statement}

— *Every submodule N of a torsion module M is the direct sum of its submodules N ∩ M*.

This follows from the fact that N ∩ M, is the π-primary component N, of N.

#### Corollary 2 {#alg-vii-s2-lem-2-cor-2 .statement}

— *The submodule N of the torsion A-module M is a direct factor if and only if N, is a direct factor of M, for every irreducible element π of A*.

Indeed, if N and N' are two submodules of M, then M = N ⊕ N' if and only if M, − N, ⊕ N'_π for every irreducible element π of $ \mathcal{A} $ (Cor. 1).

#### Corollary 3 {#alg-vii-s2-lem-2-cor-3 .statement}

— *Let N be a submodule of the torsion A-module M. If, for every irreducible element π of A, either N, = 0 or $ (M/N)_\pi = 0 $, then N is a direct factor of M*.

Indeed, the condition $ (M/N)_\pi = 0 $ implies N, = M,, and Cor. 2 applies.

An A-module M is called *semi-simple* if every submodule of M is a direct factor (cf. A, VIII, § 3).

#### Corollary 4 {#alg-vii-s2-lem-2-cor-4 .statement}

— *Let A be a principal ideal domain which is not a field, and let M be an A-module. Then M is semi-simple if and only if M is a torsion module and M, = M(π) for every irreducible element π of A*.

First suppose that M is semi-simple; let x ∈ M and let π be an irreducible element of $ \mathcal{A} $. If N is a complement of $ Annx $ in M, then we can write $ x = \alpha \pi x + y $, with $ \alpha \in \mathcal{A} $ and $ y \in N $; but that implies $ y = (1 - \alpha n)x $, so
$$
\pi(1 - \alpha \pi)x \in A\pi x \cap N = 0 .
$$
It follows first of all that M is a torsion module; if moreover $ x \in M_π $, then $ \pi(1 - \alpha \pi)x = 0 $, thus $ \pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x $ is zero and $ M_π = M(\pi) $.

Conversely, by Cor. 2 it is enough to prove that an A-module M annihilated by an irreducible element π is semi-simple; but that is clear, since M then has a natural structure of a vector space over the field $ \mathcal{A}/(\pi) $, and the submodules of M are precisely the vector subspaces under this structure.

#### Remark 1 {#alg-vii-s2-n2-rem-1 .statement}

— Clearly the annihilator of every element ≠ 0 of a τ-primary module has the form $ A\pi^k $ (k > 0 an integer), since it is a principal ideal containing a power of τ. Let x be an element of M; for each $ \pi \in P $, let $ x_\pi $ be the component of x in $ M_π $; the annihilator of x is the lcm of the annihilators of the nonzero $ x_\pi $, but by the above it is equal in this case to the *product* of the annihilators of the nonzero $ x_\pi $ (VI, p. 16, Prop. 12 (DIV)).

#### Proposition 2 {#alg-vii-s2-prop-2 .statement}

— *If M is a finitely generated torsion module over a principal ideal domain A, then the n-primary components of M are zero except for a finite number of them, and the projectors of M onto these components $ M_\pi $ are homotheties*.

This follows immediately from Lemma 1, for by Lemma 2 there exists $ \alpha \neq 0 $ in $ \mathcal{A} $ such that $ M = M(\alpha) $.

#### Remark 2 {#alg-vii-s2-n2-rem-2 .statement}

— By VII, p. 7, Remark 3, a finitely generated torsion A-module is cyclic if and only if each of its π-primary components is cyclic.

An important special case where Th. 1 and Prop. 2 apply is when $ A = \mathbf{Z} $; a $ \mathbf{Z} $-module is just an *abelian group*. An abelian group is called a *torsion group* if it is a torsion $ \mathbf{Z} $-module, that is if all its elements have *finite order*. Then $ P $ is taken to be the set of prime numbers $ > 0 $; for each prime number $ p > 0 $, an (abelian) group is said to be $ p $-torsion if all its elements have orders which are powers of $ p $. In this terminology, Th. 1 shows that *every torsion abelian group is a direct sum of p-torsion groups*. In the case of finite groups, this also follows from I, p. 80, Th. 4.

### 3. Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate

#### Theorem 2 {#alg-vii-s2-thm-2 .statement}

*Let $ A $ be a principal ideal domain, let $ K $ be its field offructions and let $ P $ be a system of representatives of irreducible elements of $ A $. Given an element $ x \in K $, there exist a finite subset $ H $ of $ P $, elements $ a_0 \in A $ and $ a, \in A $ not divisible by $ p $ in $ A $ ($ p \in H $), and integers $ s(p) > 0 $ ($ p \in H $) such that*

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

*where $ H $ and the $ s(p) $ are uniquely determined by these conditions.*

*Moreover, if $ R_p $ denotes a subset of $ A $ containing precisely one element of each residue class mod $ p $ in $ A (p \in P) $, then each $ x \in K $ can be uniquely expressed in the form*

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

*where $ a \in A $ and $ r_{ph} \in R_p $ for all $ h $ and $ p $, and all but finitely many of the $ r_{ph} $ are zero.*

Consider $ K $ as an $ A $-module; then $ A $ is the submodule generated by 1. The quotient module $ K/A $ is the quotient of $ K $ by the equivalence relation $ x' - x \in A $, which is also written, in the notation of VI, p. 6, as $ x \equiv x' $ (mod 1); let $ f $ denote the natural homomorphism from $ K $ onto $ M = K/A $.

The quotient module $ M $ is a *torsion module*, for every element of $ M $ has the form $ f(a/b) $ ($ a \in A, b \in A, b \neq 0 $), whence $ b f(a/b) = f(a) = 0 $. Hence Th. 1 of VII, p. 8 applies. Let $ M_p $ ($ p \in P $) be the submodule of elements of $ M $ annihilated by powers of $ p $; then $ f^{-1}(M_p) $ is the subring $ A_p $ of elements of $ K $ of the form $ a p^{-n} $ where $ a \in A $ and $ n \geq 0 $ is an integer. The module $ M $ is the direct sum of the $ M_p $, so every $ x \in K $ is congruent mod 1 to an element in the sum of the $ A_p $; in other words, formula (1) holds, with the $ s(p) $ integers $ > 0 $, and the $ a $, finitely many elements of $ A $ such that $ a $, is not a multiple of $ p $.

We now show that these conditions on the $ s(p) $ and the $ a $, completely determine $ H $ and the $ s(p) $. Indeed $ H $ is then the set of $ p \in P $ such that the component of $ f(x) $ in $ M_p $ is $ \neq 0 $. On the other hand if $ s $ and $ s' $ are two integers $ > 0 $ such that s \geq s' and if $ a $ and $ a' $ are elements of $ A $ not divisible by $ p $ such that $ ap^{-s} \equiv a'p^{-s'} \pmod{1} $, then we deduce that $ a \equiv a'p^{s-s'} \pmod{p^s} $; if $ s > s' $ then $ a \equiv 0 \pmod{p} $, contradicting the hypotheses. This argument also shows that each $ a_i $ is well defined mod $ p^{s(p)} $.

To complete the proof, we note first of all that in each residue class mod $ p^i $ in $ A $ there exists a unique element of the form $ \sum_{h=0}^{s-1} r_h p^h $ with $ r_h \in R_p $ for $ 0 \leq h \leq s-1 $. In fact, we proceed by induction on $ s $ (the property follows from the definition of $ R_p $ for $ s = 1 $) : let $ x \in A $; by hypothesis there is a unique element of the form $ \sum_{h=0}^{s-2} r_h p^h $ ($ r_h \in R_p $) in the residue class of $ x $ mod $ p^{s-1} $; then $ x - \sum_{h=0}^{s-2} r_h p^h $ is a multiple $ ap^{s-1} $ of $ p^{s-1} $; now there exists a unique element $ r_s $, of $ R_p $ such that $ a \equiv r_s \pmod{p} $; whence $ x \equiv \sum_{h=0}^{s-1} r_h p^h \pmod{p^s} $. To obtain formula (2) it is now enough to apply this fact to each $ a_p $ in formula (1). The uniqueness is clear in view of the above.

The following are the most important applications of Th. 2 :

I. *The ring A is the ring Z of rational integers, and K = Q*. Let P be the set of prime numbers > 0, and for each $ p \in P $ let $ R_p $ be the interval $ (0, p-1) $ in $ \mathbf{Z} $. Thus we have the canonical decomposition

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

with $ a \in \mathbf{Z} $, $ e_{ph} \in \mathbf{Z} $ and $ 0 \leq e_{ph} \leq p-1 $.

II. *The ring A is the ring E[X] of polynomials in one indeterminate over a commutative field E, and K = E(X)*. Let P be the set of monic irreducible polynomials in $ E[X] $ (VII, p. 5). For $ p \in P $ we can, by virtue of euclidean division of polynomials (IV, p. 10), take $ R_p $ to be the set of polynomials of degree strictly less than that of $ p $. Thus we have the decomposition (called canonical) of a rational function $ r(X) \in E(X) $:

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

where $ a(X) $ is a polynomial and $ v_{ph}(X) $ is a polynomial of degree strictly less than that of $ p(X) $, for all $ p $ and $ h $. In particular, if the field E is *algebraically closed*, then the $ p(X) $ have the form $ X - a $ with $ a \in E $, and the $ v_{ph}(X) $ are thus constants.

Hence we can say that the vector space $ E(X) $ over the field E has a basis consisting of the monomials $ X^n $ ($ n \geq 0 $ an integer) and the rational functions of the form $ X^m / (p(X))^h $, where $ p \in P $ and $ h $ and $ m $ are integers with $ h \geq 1 $ and $ 0 \leq rn < \deg(p) $.

### 4. Applications : II. The multiplicative group of units of the integers modulo a

Let a be a rational integer > 1, and let $(\mathbf{Z}/a\mathbf{Z})^*$ be the multiplicative group of invertible elements of the ring $\mathbf{Z}/a\mathbf{Z}$. If $a = \prod p_i^{n(i)}$ is the decomposition of a into prime factors, then the ring $\mathbf{Z}/a\mathbf{Z}$ is isomorphic to the product of the rings $\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$ (VII, p. 3, Prop. 4) and the group $(\mathbf{Z}/a\mathbf{Z})^*$ is isomorphic to the product of the groups $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. We are thus reduced to the study of the groups $(\mathbf{Z}/p^n\mathbf{Z})^*$, where p is a prime number; recall (V, p. 80) that the order $\varphi(p^n)$ of $(\mathbf{Z}/p^n\mathbf{Z})^*$ is $p^n - p^{n-1} = p^{n-1}(p-1)$.

Suppose first of all that $p > 2$; the natural homomorphism $\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$ restricts to a homomorphism of groups from $(\mathbf{Z}/p^n\mathbf{Z})^*$ onto $(\mathbf{Z}/p\mathbf{Z})^*$, whose kernel we denote U$(p^n)$; by VII, p. 3, Prop. 3 the residue class mod $p^n$ of an integer m is invertible if and only if m is coprime to p, that is if and only if the residue class of $m$ mod $p$ is invertible. It follows that U$(p^n)$ consists of all the residue classes mod $p^n$ of integers congruent to 1 mod p, so has $p^{n-1}$ elements, and that there is an exact sequence

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

Similarly, for $n \geq 2$ let U$(2^n)$ denote the kernel of the natural homomorphism from $(\mathbf{Z}/2^n\mathbf{Z})^*$ to $(\mathbf{Z}/4\mathbf{Z})^*$; this is a group of order $2^{n-2}$, consisting of all the residue classes mod $2^n$ of integers congruent to 1 mod 4, and there is an exact sequence

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### Lemma 3 {#alg-vii-s2-lem-3 .statement}

— Let x, y, k be integers with $k \geq 0$, and let $p > 2$ be a prime number. If $x \equiv 1 + py \mod p^2$ then $x^{p^k} \equiv 1 + p^{k+1}y \mod p^{k+2}$. *If* $x \equiv 1 + 4y \mod 8$ then $x^{2^k} \equiv 1 + 2^{k+2}y \mod 2^{k+3}$.

To prove the first assertion, it is enough to show that, if $k \geq 1$ and $x \equiv 1 + p^ky \mod p^{k+1}$, then $x^p \equiv 1 + p^{k+1}y \mod p^{k+2}$, and then to argue by induction on the integer k. For all $a \in \mathbf{Z}$ and $k \geq 1$, it is immediate that
$$
(1 + p^ka)^p \equiv 1 + p^{k+1}a \mod p^{k+2},
$$
hence
$$
(1 + p^ky + p^{k+1}z)^p = (1 + p^k(y + pz))^p \equiv \\
= 1 + p^{k+1}(y + pz) \equiv 1 + p^{k+1}y \mod p^{k+2}.
$$
Similarly, for $k \geq 1$ we have
$$
(1 + 2^{k+1}a)^2 \equiv 1 + 2^{k+2}a \mod 2^{k+3},
$$
so
$$
(1 + 2^{k+1}y + 2^{k+2}z)^2 \equiv 1 + 2^{k+2}y \mod 2^{k+3},
$$
whence the second assertion by induction on k.

Proposition 3. — Let $ p > 2 $ be a prime number and let $ n > 0 $ be an integer; then the group $ U(p^n) $ is cyclic of order $ p^{n-1} $; if $ n \geq 2 $ then the residue class mod $ p^n $ of an integer $ x $ congruent to 1 mod $ p $ is a generator of $ U(p^n) $ if and only if $ x $ is not congruent to 1 mod $ p^2 $. Let $ m > 1 $ be an integer; then the group $ U(2^m) $ is cyclic of order $ 2^{m-2} $; if $ m \geq 3 $ then the residue class mod $ 2^m $ of an integer $ x $ congruent to 1 mod 4 is a generator of $ U(2^m) $ if and only if $ x $ is not congruent to 1 mod 8.

Since $ U(p^n) $ has order $ p^{n-1} $, the order of every element $ u $ of $ U(p^n) $ is a power of $ p $, and $ u $ is a generator of $ U(p^n) $ if and only if $ u^{p^{n-2}} \neq 1 $. Now if $ u $ is the class of $ x = 1 + py $, then $ u^{p^{n-2}} $ is the class of $ 1 + p^{n-1}y $, by Lemma 3, whence $ u $ generates $ U(p^n) $ if and only if $ y \not\equiv 0 \mod p $, in other words $ x \not\equiv 1 \mod p^2 $. For example, the class $ 1 + p $ generates $ U(p^n) $. Similarly, the class $ u $ of $ x $ mod $ 2^n $ generates $ U(2^n) $ if and only if $ u^{2^{n-3}} \neq 1 $, which means that $ x $ is not congruent to 1 mod 8, by Lemma 3; this is satisfied by $ x = 5 $.

#### Lemma 4 {#alg-vii-s2-lem-4 .statement}

— Let $ A $ be a principal ideal domain and let $ 0 \to N \to M \to P \to 0 $ be an exact sequence of $ A $-modules. Suppose that there exist coprime elements $ a, b \in A $ such that $ aN = 0 $ and $ bP = 0 $. Then the exact sequence splits. If in addition $ N $ and $ P $ are both cyclic, then $ M $ is cyclic.

The module $ M $ is torsion, since $ abM = 0 $. The first assertion follows from Cor. 3 of VII, p. 9. If $ N $ and $ P $ are cyclic, then they are finitely generated, and hence so is $ M $ (II, p. 17, Cor. 5); since each $ p $-primary component of $ M $ is isomorphic to a $ p $-primary component either of $ N $ or of $ P $, it follows from Remark 2 of VII, p. 10, that $ M $ is cyclic.

Theorem 3. — If $ a = \prod p_i^{n(i)} $ is the prime decomposition of the integer $ a > 1 $, then the group $ (\mathbf{Z}/a\mathbf{Z})^* $ of invertible elements of the ring $ \mathbf{Z}/a\mathbf{Z} $ is isomorphic to the product of the groups $ (\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^* $. If $ p > 2 $ is a prime number and $ n \geq 1 $ an integer, then the group $ (\mathbf{Z}/p^n\mathbf{Z})^* $ is cyclic of order $ p^n \ ^1(p - 1) $. The group $ (\mathbf{Z}/2\mathbf{Z})^* $ is trivial; for $ n \geq 2 $ the group $ (\mathbf{Z}/2^n\mathbf{Z})^* $ is the direct product of the cyclic group of order $ 2^n \ ^2 $ generated by the residue class of 5 mod $ 2^n $ and the cyclic group of order 2 consisting of the residue classes of 1 and $ -1 $ mod $ 2^n $.

The orders $ p^n \ ^1 $ of $ U(p^n) $ and $ p - 1 $ of $ (\mathbf{Z}/p\mathbf{Z})^* $ are coprime; since $ U(p^n) $ and $ (\mathbf{Z}/p\mathbf{Z})^* $ are cyclic (Prop. 3 and V, p. 78, Lemma 1), the group $ (\mathbf{Z}/p^n\mathbf{Z})^* $ is cyclic (apply Lemma 4 to the exact sequence (3)). If $ n \geq 2 $ then the restriction of the homomorphism $ v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* $ to the subgroup $ (1, -1) $ is bijective; the group $ (\mathbf{Z}/2^n\mathbf{Z})^* $ is thus the direct product of this subgroup and the kernel $ U(2^n) $ of $ v $; the result follows from Prop. 3.

#### Remark {#alg-vii-s2-n4-rem-1 .statement}

— Let $ p > 2 $ be a prime number and let $ x $ be an integer congruent to 1 mod $ p $ and not congruent to 1 mod $ p^2 $; there is an exact sequence

$$
\{0\} \to \mathbf{Z}/p^n \ ^1\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{\nu} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

of groups, where $ v $ is the natural projection and where $ u $ is induced on the quotients by the map $ r \mapsto x^r $. Let $ \mathbf{Z}_p $ be the ring of $ p $-adic integers ($ V $, p. 96), and let $ x $ be an element of $ \mathbf{Z}_p $ such that $ x - 1 \in p\mathbf{Z}_p $ and $ x - 1 \notin p^2\mathbf{Z}_p $; on passing to inverse limits, the exact sequences (5) induce an exact sequence

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

where $ v $ is the natural map, and the continuous map $ u $ extends the map $ n \mapsto x^n $ ($ n \in \mathbf{Z} $). We often put $ x^n = u(x) $ for $ n \in \mathbf{Z}_p $.

Similarly, if $ x \in \mathbf{Z}_2 $ with $ x - 1 \in 4\mathbf{Z} $, and $ x - 1 \notin 8\mathbf{Z}_2 $, then there is a split exact sequence

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

where $ u $ is a continuous extension of the map $ n \mapsto x^n $

### Exercises {#alg-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
