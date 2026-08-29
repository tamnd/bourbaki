---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 8
section_title: Dualité des modules de longueur finie
lang: en
source: ac-x-fr
pdf_pages: 0104-0123, 0172-0174
extraction: ocr
subsections:
    - "no": 1
      title: Modules injectifs indécomposables
      page: 0
      pdf_page: 104
    - "no": 2
      title: Structure des modules injectifs indécomposables
      page: 0
      pdf_page: 105
    - "no": 3
      title: Dualité de Matlis
      page: 110
      pdf_page: 109
    - "no": 4
      title: Dualité des modules de longueur finie
      page: 114
      pdf_page: 113
    - "no": 5
      title: Foncteurs dualisants
      page: 115
      pdf_page: 114
    - "no": 6
      title: Changement d’anneaux ; dualité de Macaulay
      page: 119
      pdf_page: 118
    - "no": 7
      title: Dualité des modules d’extensions et des produits de torsion
      page: 0
      pdf_page: 119
statements: 31
exercises: 10
content_sha256: 51e31816b68f96681968fe09fb5cad0e0228d14a3641b0e6b586d1cd7ea00744
translated_from: content/fr/ac/X/08_s8_dualite_des_modules_de_longueur_finie.md
source_lang: fr
translation_method: machine
source_content_sha256: 77f9377a8e567979844890a8c62bb0a878d9c20aeb59902a661be4f0e8769c2f
translation_model: gpt-5.4
translation_run: translate-en-mt-fc5e2194
glossary_version: 34
glossary_terms_sha256: 40f631fd3b14afe7c391447c534da7eb77398df553c81d6dbdc6a551467ef181
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 8. DUALITY OF MODULES OF FINITE LENGTH

### 1. Indecomposable injective modules

Let $A$ be a ring. The relation "$I$ is a class of indecomposable injective $A$-modules" is collectivizing (A, X, p. 21, Corollary 1); we denote by $\mathscr{J}(A)$ the set of classes of indecomposable injective $A$-modules.

#### Proposition 1 {#ac-x-s8-prop-1 .statement}

Let $A$ be a noetherian ring. For every prime ideal $\mathfrak{p}$ of $A$, let $e_{\mathfrak{p}} : A/\mathfrak{p} \to I(\mathfrak{p})$ be an injective envelope of $A/\mathfrak{p}$ (A, X, § 1, No. 9).

a) The $A$-modules $I(\mathfrak{p})$ are indecomposable.

b) Let $I$ be an indecomposable injective $A$-module; the set $\mathrm{Ass}(I)$ consists of a single element.

c) The mapping $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ is a bijection of $\mathrm{Spec}(A)$ onto $\mathscr{J}(A)$. The inverse bijection associates to an element $I$ of $\mathscr{J}(A)$ the unique element of $\mathrm{Ass}(I)$.

Let $\mathfrak{p} \in \mathrm{Spec}(A)$; let us prove that the module $I(\mathfrak{p})$ is indecomposable. By A, X, p. 21, Corollary 2, it is enough to prove that if $a$ and $b$ are ideals of $A$ containing $\mathfrak{p}$ and distinct from $\mathfrak{p}$, the ideal $a \cap b$ is distinct from $\mathfrak{p}$; now if $a$ is an element of $a - \mathfrak{p}$ and $b$ an element of $b - \mathfrak{p}$, the product $ab$ belongs to $(a \cap b) - \mathfrak{p}$.

Let $I$ be an indecomposable injective $A$-module, and let $\mathfrak{p}, \mathfrak{q}$ be elements of $\mathrm{Ass}(I)$. Then $I$ contains a submodule $M$ isomorphic to $A/\mathfrak{p}$ and a submodule $N$ isomorphic to $A/\mathfrak{q}$. One has $M \cap N \neq 0$ (A, X, p. 21, Proposition 14); for every nonzero element $x$ of $M \cap N$, one has $\mathfrak{p} = \mathrm{Ann} x = \mathfrak{q}$. Since $\mathrm{Ass}(I)$ is not empty (IV, § 1, No. 1, Corollary 1 of Proposition 2), it consists of a single element $\mathfrak{p}(I)$.

We have thus defined two mappings $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ from $\mathrm{Spec}(A)$ into $\mathscr{J}(A)$ and $I \mapsto \mathfrak{p}(I)$ from $\mathscr{J}(A)$ into $\mathrm{Spec}(A)$; let us prove that these two mappings are reciprocal bijections. Let $\mathfrak{p} \in \mathrm{Spec}(A)$; then $\mathfrak{p}$ belongs to $\mathrm{Ass}(I(\mathfrak{p}))$, and is therefore the unique element of $\mathrm{Ass}(I(\mathfrak{p}))$. Let $I$ be an indecomposable injective $A$-module, and $\mathfrak{p}$ the unique element of $\mathrm{Ass}(I)$; then $I$ is an injective envelope of $A/\mathfrak{p}$ (A, X, p. 21, Prop. 14). This completes the proof of the proposition.

#### Remark 1 {#ac-x-s8-n1-rem-1 .statement}

Let $I$ be an indecomposable injective $A$-module, and let $\mathfrak{p}$ be the unique element of $\mathrm{Ass}(I)$; by Prop. 1, $I$ contains a submodule isomorphic to $A/\mathfrak{p}$ of which it is the injective envelope. In general such a submodule is not unique, as is seen by taking $A = \mathbf{Z}$, $\mathfrak{p} = 0$, $I = \mathbf{Q}$.

For each prime ideal $\mathfrak{p}$ of $A$, let us choose as above an injective envelope $(I(\mathfrak{p}), e_{\mathfrak{p}})$ of $A/\mathfrak{p}$. By A, X, p. 22, Th. 3, one has:

#### Theorem 1 {#ac-x-s8-thm-1 .statement}

Let $A$ be a noetherian ring. For every injective $A$-module $I$, there exists one and only one family of cardinals $(a_{\mathfrak{p}})_{\mathfrak{p} \in \mathrm{Spec}(A)}$ such that $I$ is isomorphic to $\bigoplus_{\mathfrak{p}} I(\mathfrak{p})^{(a_{\mathfrak{p}})}$.

#### Remark 2 {#ac-x-s8-n1-rem-2 .statement}

Let $A$ be a noetherian ring, $M$ an $A$-module, $e : M \to I$ an injective envelope of $M$. *The set Ass(M) is equal to Ass(I)*: in fact, the inclusion $Ass(M) \subset Ass(I)$ is obvious. On the other hand, if $p$ is an element of $Ass(I)$, $I$ contains a submodule $N$ isomorphic to $A/p$; since the $A$-module $e^{-1}(N)$ is nonzero, one has $Ass(e^{-1}(N)) = \{p\}$ (IV, § 1, No. 1, Prop. 1). This proves that $p$ is associated with $e^{-1}(N)$, hence with $M$, whence our assertion.

Let us retain the notation of the theorem, and suppose further that $Ass(M)$ is finite. For every $q \in Ass(M)$, let $Q_q$ denote the intersection with $M$ of $\bigoplus_{p \in Ass(M) - \{q\}} I(p)^{(a_p)}$. Then $(Q_q)_{q \in Ass(M)}$ *is a reduced primary decomposition of 0 in M* (IV, § 2, No. 3, Def. 3). For indeed $\cap Q_q = 0$; since $M/Q_q$ is identified with a nonzero a-submodule of $I(q)^{(a_q)}$, we have $Ass(M/Q_q) = \{q\}$, and it is enough to apply Prop. 4 of *loc. cit*.

#### Example {#ac-x-s8-n1-exa-1 .statement}

Let $A$ be a principal ideal domain, and let $K$ be its field of fractions. The injective $A$-modules are the divisible $A$-modules (A, X, p. 17, Cor. 2). The $A$-module $K$ is an injective envelope of $A$ (A, X, p. 20, Example 1). Let $p$ be an extremal element of $A$, and $p$ the (maximal) ideal $Ap$; let $e : A/p \longrightarrow K/A_p$ denote the homomorphism which maps the class of an element $a \in A$ to the class of $a/p$. Let us prove that $(K/A_p, e)$ *is an injective envelope of $A/p$*. The homomorphism $e$ is injective. The $A$-module $K/A_p$ is a quotient of a divisible module, hence is divisible. Let $x$ be a nonzero element of $K/A_p$; it is the class of an element $a/p^n$ of $K$, with $a \in A - \{0\}$ and $n \geqslant 1$ (A, VII, p. 10, th. 2). Then $p^{n-1}x = e(a)$, hence $e^{-1}(Ax) \neq 0$, which proves our assertion.

It then follows from th. 1 that *every divisible $A$-module is a direct sum of $A$-modules isomorphic to $K$ or to $K/A_p$ for a maximal (principal) ideal $p$ of $A$*.

### 2. Structure of indecomposable injective modules

#### Lemma 1 {#ac-x-s8-lem-1 .statement}

Let $A$ be a ring, $a$ an ideal of $A$, and $I$ an $A$-module. For every integer $n \geqslant 0$, let $I_n$ denote the a-submodule of $I$ consisting of the elements annihilated by $a^n$.

a) *Suppose that the $A$-module $I$ is injective. Then the $A/a^n$-module $I_n$ is injective for every $n \geqslant 0$*.

b) *Suppose that the ring $A$ is noetherian, and that for every $n \geqslant 0$ the $A/a^n$-module $I_n$ is injective. Then the union of the $I_n$ is an injective $A$-module*.

a) The $A/a^n$-module $I_n$ is isomorphic to $\operatorname{Hom}_A(A/a^n, I)$, which is injective (A, X, p. 18, Prop. 11).

b) Let $J$ be the union of the $I_n$, $b$ an ideal of $A$ and $f : b \to J$ an $A$-homomorphism. It is a matter (A, X, p. 16, Prop. 10) of proving that there exists an element $x$ of $J$ such that one has $f(b) = bx$ for every $b \in b$. Since $b$ is of finite type, there exists an integer $n$ such that one has $f(b) \subset I_n$, that is, $f(a^n b) = 0$. By Cor. 2 of Prop. 1 of III, § 3, No. 1, there exists an integer $m \geqslant n$ such that $a^m \cap b \subset a^n b$, hence $f(a^m \cap b) = 0$. Then $f$ induces an $A/a^m$-linear mapping of $b/(a^m \cap b)$ into $I_m$; since the $A/a^m$-module $I_m$ is injective, there exists an element $x$ of $I_m$ such that one has $f(b) = bx$ for every $b \in b$, whence b).

Let $\alpha$ be an ideal of $A$; in what follows we agree to put $\alpha^n = A$ for every integer $n \leq 0$. Let $E$ be an $A$-module. For every $n \in \mathbf{Z}$, let $E_n$ denote the submodule of $E$ consisting of the elements annihilated by $\alpha^n$; let $\mathrm{gr}^\alpha(E)$ be the graded $A$-module of type $\mathbf{Z}$ such that $\mathrm{gr}^\alpha(E)_m = E_{-m+1}/E_{-m}$ for every integer $m$. The module $\mathrm{gr}^\alpha(E)_m$ is zero for $m \geq 1$, and $\mathrm{gr}^\alpha(E)_0$ is identified with $E_1$. Let $\mathrm{gr}(A)$ denote the graded ring associated with $A$ for the $\alpha$-adic filtration: one has $\mathrm{gr}(A)_n = \alpha^n/\alpha^{n+1}$ for every $n \in \mathbf{Z}$. Let $n$ and $m$ be integers. Passing to quotients from the bilinear mapping $(a, x) \mapsto ax$ of $\alpha^n \times E_{-m+1}$ into $E_{-m-n+1}$, one deduces an $A/\alpha$-bilinear mapping

$$
\alpha_{n,m} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_m \longrightarrow \mathrm{gr}^\alpha(E)_{n+m},
$$

which defines on $\mathrm{gr}^\alpha(E)$ a structure of graded $\mathrm{gr}(A)$-module. For every $n \in \mathbf{Z}$, from the $A/\alpha$-bilinear mapping $\alpha_{n,-n} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_{-n} \longrightarrow E_1$ one deduces an $A/\alpha$-linear mapping $\beta_{E,n} : \mathrm{gr}^\alpha(E)_{-n} \longrightarrow \mathrm{Hom}_{A/\alpha}(\mathrm{gr}(A)_n, E_1)$; the mappings $\beta_{E,n}$ are the components of a homomorphism of graded $A/\alpha$-modules, called *canonical*,

$$
\beta_E : \mathrm{gr}^\alpha(E) \longrightarrow \mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1).
$$

For $a \in \mathrm{gr}(A)$, $x \in \mathrm{gr}^\alpha(E)$, $\beta_E(x)(a)$ is by definition the component in $\mathrm{gr}^\alpha(E)_0 = E_1$ of the element $ax$ of $\mathrm{gr}^\alpha(E)$. It follows that $\beta_E$ is $\mathrm{gr}(A)$-linear when one endows $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$ with the structure of $\mathrm{gr}(A)$-module defined by the formula $(bf)(a) = f(ab)$ for $a, b$ in $\mathrm{gr}(A)$ and $f$ in $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$.

#### Proposition 2 {#ac-x-s8-prop-2 .statement}

*Let $A$ be a noetherian ring, $\alpha$ an ideal of $A$, $E$ an $A$-module and $M$ a sub-$A$-module of $E$ annihilated by $\alpha$. The following conditions are equivalent:*
    (i) *$E$ is an injective envelope of $M$* ;
    (ii) *the $\Lambda/\alpha$-module $E_1$ is an injective envelope of the $A/\alpha$-module $M$, the module $E$ is the union of the $E_n$ and the canonical mapping $\beta_E$ is bijective*.

Suppose condition (i) is satisfied. The $A/\alpha$-module $E_1$ is injective (Lemma 1, a)), and contains $M$; since every sub-$\Lambda/\alpha$-module of $E_1$ is a sub-$A$-module of $E$, $E_1$ is an injective envelope of the $\Lambda/\alpha$-module $M$. By Lemma 1, the union of the $E_n$ is an injective sub-$A$-module of $E$ containing $M$, hence equal to $E$. Since $E$ is injective, for every $n \geq 0$ one has an exact sequence

$$
0 \to \mathrm{Hom}_A(A/\alpha^n, E) \longrightarrow \mathrm{Hom}_A(A/\alpha^{n+1}, E) \longrightarrow \mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E) \to 0;
$$

since $\mathrm{Hom}_A(A/\alpha^m, E)$ is identified with $E_m$ for every $m$ and the canonical injection of $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E_1)$ into $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E)$ is bijective, one deduces that the canonical homomorphism $\beta_E$ is bijective, whence (ii).

Suppose (ii) is satisfied. Let $e : M \to I$ be an injective envelope of $M$. Since $I$ is injective, there exists an $A$-linear mapping $\varphi : E \to I$ extending $e$. But $\varphi$ maps $E_n$ into $I_n$ for every $n$, hence induces homomorphisms gr^{a}(\varphi) : \operatorname{gr}^{a}(E) \to \operatorname{gr}^{a}(I) \text{ and } \varphi_1 : E_1 \to I_1 \text{ rendering the diagram commutative}

$$
\begin{array}{ccc}
\operatorname{gr}^{a}(E) & \xrightarrow{\beta_E} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), E_1) \\
\downarrow \operatorname{gr}^{a}(\varphi) & & \downarrow \operatorname{Homgr}(1, \varphi_1) \\
\operatorname{gr}^{a}(I) & \xrightarrow{\beta_I} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), I_1)
\end{array}
$$

Since $E_1$ and $I_1$ are injective envelopes of the $A/\alpha$-module $M$, the homomorphism $\varphi_1$ is bijective; since $\beta_E$ and $\beta_I$ are bijective, it follows that $\operatorname{gr}^{a}(\varphi)$ is bijective. This implies, by induction on $n$, that $\varphi$ induces a bijection of $E_n$ onto $I_n$ for every $n \geq 1$; hence $\varphi$ is bijective, which entails (i).

#### Lemma 2 {#ac-x-s8-lem-2 .statement}

*Let $A$ be a ring, $\alpha$ an ideal of finite type of $A$, and $M$ an $A$-module each element of which is annihilated by a power of $\alpha$. Let $\widehat{A}$ denote the separated completion of $A$ for the $\alpha$-adic topology.*

a) *There exists on $M$ a unique structure of $\widehat{A}$-module extending the given structure of $A$-module.*

b) *The sub-$\widehat{A}$-modules of $M$ are its sub-$A$-modules, and one has $\operatorname{Hom}_A(M, P) = \operatorname{Hom}_{\widehat{A}}(M, P)$ for every $\widehat{A}$-module $P$.

a) Let us identify $\widehat{A}$ with the projective limit of the rings $A/\alpha^n$, and endow $M$ with the discrete topology. Let $a = (a_n)$ be an element of $\widehat{A}$, and $x$ an element of $M$. Since $x$ is annihilated by a power of $\alpha$, the sequence $(a_n x)$ is stationary; let $ax$ denote its limit. The mapping $(a, x) \mapsto ax$ defines on $M$ a structure of $\widehat{A}$-module extending the given structure of $A$-module.

Conversely, suppose given such a structure on $M$; let $a = (a_n)$ be an element of $\widehat{A}$, $x$ an element of $M$ and $m$ an integer such that $\alpha^m x = 0$. For every integer $n$, $a - a_n$ belongs to $\alpha^n$, which is equal to $\alpha^n \widehat{A}$ (III, § 2, n° 12, cor. 2 of prop. 16); hence one has $ax = a_n x$ for $n \geq m$, whence the assertion of uniqueness.

b) It follows from the preceding that one has $Ax = \widehat{A}x$ for every $x \in M$; the $\widehat{A}$-submodules of $M$ are therefore its $A$-submodules. Finally, let $u$ be an $A$-linear homomorphism of $M$ into a $\widehat{A}$-module $P$. Let $a = (a_n)$ be an element of $\widehat{A}$, $x$ an element of $M$, and $m$ an integer such that $\alpha^m x = 0$; one has $\alpha^m u(x) = 0$. Since $a - a_m$ belongs to $\alpha^m \widehat{A}$, one has

$$
u(ax) = u(a_m x) = a_m u(x) = au(x),
$$

so that $u$ is $\widehat{A}$-linear.

#### Proposition 3 {#ac-x-s8-prop-3 .statement}

*Let $A$ be a noetherian ring, $p$ a prime ideal of $A$, and $e : A/p \to I$ an injective envelope of the $A$-module $A/p$. For every integer $n \geq 0$, let $I_n$ denote the submodule of $I$ consisting of the elements annihilated by $p^n$.*

a) The $A$-module $I$ is the union of the $I_n$. The injection $\Lambda / \mathfrak{p} \to I_1$ extends to an isomorphism of $\kappa(\mathfrak{p})$ onto $I_1$; let us identify $\kappa(\mathfrak{p})$ with $I_1$ by means of this isomorphism. For each integer $n \geqslant 0$, the structure of $\Lambda / \mathfrak{p}$-module of $I_{n+1}/I_n$ arises by restriction of scalars from a unique structure of $\kappa(\mathfrak{p})$-vector space; the canonical homomorphism $\beta_{I,-n}: I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\Lambda/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$ is an isomorphism of finite-dimensional $\kappa(\mathfrak{p})$-vector spaces.

b) There exists a unique structure of $\widehat{A_p}$-module on $I$ inducing its structure of $A$-module. The canonical homomorphism $\widehat{A_p} \longrightarrow \mathrm{End}_A(I)$ is bijective.

According to A, X, p. 20, Example 1, the $A/\mathfrak{p}$-module $\kappa(\mathfrak{p})$ is an injective envelope of $A/\mathfrak{p}$. It therefore follows from Prop. 2 that $I_1$ identifies with $\kappa(\mathfrak{p})$, that $I$ is the union of the $I_m$, and that for each integer $n \geqslant 0$, $\beta_{I,-n}$ is an isomorphism of $A/\mathfrak{p}$-modules. For every nonzero element $a$ of $A/\mathfrak{p}$, the homothety of ratio $a$ is invertible in $\mathrm{Hom}_{A/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$, hence also in $I_{n+1}/I_n$, which completes the proving of a).

Let $s \in A - \mathfrak{p}$. Since the homothety $s_{A/\mathfrak{p}}$ is injective, the trace of $\mathrm{Ker}\, s_I$ on $A/\mathfrak{p}$ is zero, whence it follows that the homothety $s_I$ is injective. Then $s_I$ is a direct factor submodule of $I$ (A, X, p. 19, Cor. 4), hence equal to $I$ since $I$ is indecomposable (No. 1, Prop. 1), so that the homothety $s_I$ is bijective. There therefore exists a unique $A_p$-module structure on $I$ inducing its $A$-module structure; it extends uniquely to a $\widehat{A_p}$-module structure (Lemma 2).

For each integer $n$, one deduces from the canonical ring homomorphism $\Lambda_p \longrightarrow \mathrm{End}_A(I)$ an $A$-linear mapping $\alpha_n : A_p/\mathfrak{p}^n A_p \longrightarrow \mathrm{Hom}_A(I_n, I)$. Consider the commutative diagram with exact rows

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^n A_p & \longrightarrow & 0 \\
& & \downarrow \alpha'_{n+1} & & \downarrow \alpha_{n+1} & & \downarrow \alpha_n & & \\
0 & \longrightarrow & \mathrm{Hom}_A(I_{n+1}/I_n, I_1) & \longrightarrow & \mathrm{Hom}_A(I_{n+1}, I) & \longrightarrow & \mathrm{Hom}_A(I_n, I) & \longrightarrow & 0
\end{array}
$$

where $\alpha'_{n+1}$ is the homomorphism induced by $\alpha_{n+1}$. Consider the canonical $\kappa(\mathfrak{p})$-bilinear mapping

$$
\alpha_{n,-n} : \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p \times I_{n+1}/I_n \longrightarrow I_1
$$

(formula (1)). The linear mapping $I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\kappa(\mathfrak{p})}(\mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p, I_1)$ associated with it on the left identifies with $\beta_{I,-n}$, and that associated with it on the right is $\alpha'_{n+1}$. Since $\beta_{I,-n}$ is bijective by a), the same is true of $\alpha'_{n+1}$; one then deduces from the above diagram, by induction on $n$, that $\alpha_n$ is an isomorphism for every $n$. Since $I$ is the union of the $I_n$, the canonical mapping $\mathrm{End}_A(I) \to \varprojlim \mathrm{Hom}_A(I_n, I)$ is bijective; the ring homomorphism $\widehat{A_p} \to \mathrm{End}_A(I)$, which identifies with the projective limit of the mappings $\alpha_n$, is therefore bijective.

#### Remark {#ac-x-s8-n2-rem-1 .statement}

It follows from the preceding proof that the annihilator of $I_n$ in $\widehat{A_p}$ (resp. in $A_p$) is $\mathfrak{p}^n \widehat{A_p}$ (resp. $\mathfrak{p}^n A_p$). Hence the annihilator of the $A$-module $I_n$ is the inverse image in $A$ of the ideal $\mathfrak{p}^n A_p$, which is sometimes denoted by $\mathfrak{p}^{(n)}$ and is called the $n$th symbolic power of the prime ideal $\mathfrak{p}$.

#### Corollary {#ac-x-s8-n2-cor-1 .statement}

Let J be an injective A-module such that Ass_A(J) = {p}.

a) The canonical mapping J → A_p ⊗_A J is bijective.

b) Let E denote the A/p-module Hom_A(A/p, J). There exists on E a unique structure of κ(p)-vector space extending its structure of A/p-module; the A-module J is isomorphic to I([E:κ(p)]).

Indeed, J is isomorphic to an A-module I^{(c)}, where c is a suitable cardinal (No. 1, th. 1). The corollary follows from the proposition when J = I, and the general case is deduced from it at once.

### 3. Matlis Duality

In this No., we suppose that the ring A is local noetherian.

#### Definition {#ac-x-s8-n3-def-1 .statement}

We say that an A-module I is a Matlis A-module if it is injective, if m_A is its unique associated prime ideal, and if the κ_A-vector space Hom_A(κ_A, I) is of dimension 1.

Let e : κ_A → I be an injective envelope of κ_A (A, X, p. 20, th. 2). The A-module I is a Matlis module, and every Matlis module is isomorphic to I (No. 2, cor. of prop. 3). If A is a discrete valuation ring, with field of fractions K, the A-module K/A is a Matlis module (No. 1, example). If A is an artinian local ring, the A-module A is a Matlis module if and only if A is a Gorenstein ring (§ 3, No. 7, lemma 1).

Let I be a Matlis A-module. For every integer n ≥ 0, let I_n denote the sub-A-module of I consisting of the elements annihilated by m_A^n. By prop. 2 of No. 2, the A-module I is the union of the I_n, the A-module I_1 is of length 1 (that is to say isomorphic to κ_A) and the A-module I is an injective envelope of I_1; moreover, the canonical homomorphism of graded gr(A)-modules

$$
\beta : \operatorname{gr}^{m_A}(I) \longrightarrow \operatorname{Hom}_{\kappa_A}(\operatorname{gr}(A), I_1)
$$

is an isomorphism. By prop. 3 of No. 2, the A-module structure of I extends to a unique $\widehat{A}$-module structure, and the canonical homomorphism $\widehat{A} \to \operatorname{End}_A(I)$ is bijective.

#### Lemma 3 {#ac-x-s8-lem-3 .statement}

Let I be a Matlis A-module. Then:

a) I is a Matlis $\widehat{A}$-module;
b) the A-module I is artinian and a cogenerator (A, X, p. 18, def. 3).

Since the A-module I is injective, the A/m_A^n-module I_n is injective for each n (No. 2, lemma 1, a)). As I_n is the set of elements of I annihilated by m_A^n, the $\widehat{A}$-module I is injective (lemma 1, b)). It is indecomposable over $\widehat{A}$ since it is so over A; as it contains the sub-$\widehat{A}$-module I_1 isomorphic to $\kappa_A$, we have $m_{\widehat{A}} \in \operatorname{Ass}_{\widehat{A}}(I)$, hence $\operatorname{Ass}_{\widehat{A}}(I) = \{ m_{\widehat{A}} \}$ (prop. 1), whence a).

Let us prove now that I is artinian. To every sub-A-module M of I, let us associate the graded ideal $a_M$ of gr(A) defined as follows: an element of gr(A)_n belongs to $(\mathfrak{a}_M)_n$ if it is annihilated by all the linear forms $\beta(x)$, where $x$ runs through $((M \cap I_{n+1}) + I_n)/I_n$. Let $M$ and $N$ be submodules of $I$ such that $N \subset M$; then $\mathfrak{a}_M \subset \mathfrak{a}_N$. Suppose $\mathfrak{a}_M = \mathfrak{a}_N$; we have $(M \cap I_{n+1}) + I_n = (N \cap I_{n+1}) + I_n$ for every $n$ since $\beta$ is an isomorphism. By induction on $n$ we deduce from this that $M \cap I_{n+1} = N \cap I_{n+1}$ for every $n$, whence finally $M = N$.

This being so, let $M_0 \supset M_1 \supset \ldots \supset M_n \supset \ldots$ be a decreasing sequence of sub-A-modules of $I$; the increasing sequence $\mathfrak{a}_{M_0} \subset \mathfrak{a}_{M_1} \subset \ldots$ is stationary, since $\mathrm{gr}(A)$ is a finitely generated $\kappa_A$-algebra. The sequence $(M_i)_{i \geq 0}$ is therefore stationary, which implies that the A-module $I$ is artinian. Finally, the A-module $I$ is a cogenerator by virtue of A, X, p. 18, prop. 12.

Let $M$ be an A-module. Recall (A, VIII, § 4, No. 6) that the socle of $M$ is the sum of the simple submodules of $M$, that is to say the set of elements of $M$ annihilated by $m_A$; it is a $\kappa_A$-vector space, canonically isomorphic to $\mathrm{Hom}_A(\kappa_A, M)$.

#### Lemma 4 {#ac-x-s8-lem-4 .statement}

*Let I be a Matlis A-module and M a $\Lambda$-module. The following conditions are equivalent :*

(i) $M$ is artinian;
(ii) every element of $M$ is annihilated by a power of $m_A$, and the socle of $M$ is of finite dimension over $\kappa_\Lambda$;
(iii) there exist an integer $n \geq 0$ and an injective a-linear mapping of $M$ into $I^n$.

*When these conditions are satisfied, every injective envelope of $M$ is isomorphic to $I^s$, where $s$ is the dimension over $\kappa_A$ of the socle of $M$.*

(iii) $\Rightarrow$ (i): this is clear since the a-module $I$ is artinian (Lemma 3).

(i) $\Rightarrow$ (ii): suppose that $M$ is artinian. Let $x \in M$; the decreasing sequence of submodules $m_A^n x$ of $M$ is stationary. Let $n$ be an integer such that $m_A^{n+1} x = m_A^n x$; Nakayama's lemma implies that $m_A^n x = 0$. On the other hand, the socle of $M$ is artinian as an a-module, hence also as a $\kappa_A$-vector space, which means that it is of finite dimension.

(ii) $\Rightarrow$ (iii): suppose condition (ii) satisfied; let $e : M \to J$ be an injective envelope of $M$. We have $\mathrm{Ass}(M) \subset \{m_A\}$, hence $\mathrm{Ass}(J) \subset \{m_A\}$ (No. 1, Remark 2), and $J$ is isomorphic to $I^{(c)}$ for a cardinal $c$ (No. 1, Theorem 1). Let $x$ be a nonzero element of $J$ annihilated by $m_A$; since the a-module $Ax$ is simple and its intersection with $e(M)$ is not reduced to 0, $x$ belongs to $e(M)$. Thus $e$ induces an isomorphism of the socle of $M$ onto that of $J$; consequently the socle of $M$ is of dimension $c$, which proves (iii) as well as the last assertion.

#### Lemma 5 {#ac-x-s8-lem-5 .statement}

*Every artinian $\widehat{\Lambda}$-module is artinian as a $\Lambda$-module.*

Let $M$ be an artinian $\widehat{\Lambda}$-module; every element of $M$ is annihilated by a power of $m_{\widehat{\Lambda}}$, hence by a power of $m_A$. By Lemma 2 of No. 2, the sub-A-modules of $M$ are its sub-$\widehat{\Lambda}$-modules, hence $M$ is artinian as an A-module.

Let us now fix a Matlis $A$-module I. For every $A$-module $M$, let us denote by $D_A(M)$ the $\widehat{A}$-module
$$
D_A(M) = \operatorname{Hom}_A(M, I)
$$
The $\widehat{A}$-module $D_A(A)$ is canonically identified with $I$, the $\widehat{A}$-module $D_A(I)$ with $\widehat{A}$ ($n^\circ 2$, prop. 3), and the $\widehat{A}$-module $D_A(\kappa_A)$ with $I_1$ (*loc. cit.*).

For every $A$-linear mapping $f : M \to N$, we shall denote by
$$
D_A(f) : D_A(N) \to D_A(M)
$$
the $\widehat{A}$-linear mapping $\operatorname{Hom}_A(f, 1_I)$. Since the $A$-module $I$ is injective, the sequence $(D_A(g), D_A(f))$ is exact for every exact sequence $(f, g)$ of $A$-linear mappings.

We shall apply these definitions to the ring $\widehat{A}$ endowed with the Matlis module I (lemma 3, a)) ; for every $\widehat{A}$-module $P$, $D_{\widehat{A}}(P)$ is therefore the $\widehat{A}$-submodule $\operatorname{Hom}_{\widehat{A}}(P, I)$ of $D_A(P)$. It amounts to the same thing to say that $P$ is artinian as an $A$-module or as a $\widehat{A}$-module (lemma 5) ; if this is the case, one has $D_{\widehat{A}}(P) = D_A(P)$ (*loc. cit.*).

Let $M$ be an $A$-module. For $m \in M$, the mapping $f \mapsto f(m)$ of $D_A(M)$ into $I$ is $\widehat{A}$-linear ; let us denote it by $\alpha_M(m)$. Thus one defines an $A$-linear homomorphism
$$
\alpha_M : M \longrightarrow D_{\widehat{A}}(D_A(M))
$$
We denote by $\widehat{\alpha}_M : \widehat{A} \otimes_A M \longrightarrow D_{\widehat{A}}(D_A(M))$ the $\widehat{A}$-linear mapping deduced from $\alpha_M$.

#### Theorem 2 {#ac-x-s8-thm-2 .statement}

*Let $M$ be an $A$-module.*

a) *In order that $M$ be artinian, it is necessary and sufficient that the $\widehat{A}$-module $D_A(M)$ be of finite type. When this is so, the homomorphism $\alpha_M$ is bijective.*

b) *For $M$ to be of finite type, it is necessary and sufficient that $D_A(M)$ be artinian (as an $A$-module or as a $\widehat{A}$-module). In this case the homomorphism $\widehat{\alpha}_M$ is an isomorphism.*

c) *For $M$ to be of finite length, it is necessary and sufficient that $D_A(M)$ be of finite length (as an $A$-module or as a $\widehat{A}$-module). In this case $\alpha_M$ is an isomorphism of $M$ onto $D_A(D_A(M))$, and one has $\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(M)$.*

Let us first prove that the homomorphism $\alpha_M$ is injective for every $A$-module $M$. Let $m$ be a nonzero element of $M$; its annihilator is contained in $m_A$. There therefore exists a surjective $A$-homomorphism of $Am$ onto $\kappa_A$, and consequently a nonzero homomorphism of $Am$ into $I$. Since $I$ is injective, this extends to a homomorphism $f : M \to I$ such that $f(m) \neq 0$. This proves the injectivity of $\alpha_M$.

Suppose that the $A$-module $M$ is artinian. By lemma 4, there exist an integer $r$ and an injective $A$-linear mapping $f : M \to I^r$. The homomorphism $D_A(f) : D_A(I^r) \to D_A(M)$ is then surjective; since $D_A(I^r)$ is identified with $\widehat{A}^r$, this proves that the $\widehat{A}$-module $D_A(M)$ is of finite type. Similarly, if $M$ is of finite type, there exist an integer $n$ and a surjective homomorphism $u : A^n \to M$; the homomorphism $D_A(u) : D_A(M) \to I^n$ is injective, so that $D_A(M)$ is artinian (as an $A$-module or as a $\widehat{A}$-module).

Suppose that $M$ is artinian. There exist an integer $r$ and an injective $A$-linear mapping $f : M \to I^r$; since $I$ is artinian (lemma 3), the $A$-module $\operatorname{Coker}(f)$ is also so, and one can find an integer $s$ and an exact sequence of $A$-modules

$$
0 \to M \xrightarrow{f} I^r \xrightarrow{g} I^s .
$$

Hence one deduces a commutative diagram with exact rows

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M & \xrightarrow{f} & I^r & \xrightarrow{g} & I^s \\
& & \downarrow{\alpha_M} & & \downarrow{\alpha_{I^r}} & & \downarrow{\alpha_{I^s}} \\
0 & \to & D_{\widehat{A}}(D_A(M)) & \xrightarrow{D_{\widehat{A}}(D_A(f))} & D_{\widehat{A}}(D_A(I^r)) & \xrightarrow{D_{\widehat{A}}(D_A(g))} & D_{\widehat{A}}(D_A(I^s)) .
\end{array}
$$

The $\widehat{A}$-module $D_{\widehat{A}}(D_A(I))$ is identified with $I$ and $\alpha_I$ with the identity mapping; hence $\alpha_{I^r}$ and $\alpha_{I^s}$ are bijective, and analogously so is $\alpha_M$ (A, X, p. 7, Corollary 3).

If the $A$-module $M$ is finitely generated, there exist integers $m$ and $n$ and an exact sequence of $A$-modules

$$
A^m \longrightarrow A^n \longrightarrow M \to 0 ;
$$

from which one deduces a commutative diagram with exact rows

$$
\begin{array}{ccccccccc}
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & \widehat{A} \otimes_A M & \longrightarrow & 0 \\
\downarrow{\widehat{\alpha}_{A^m}} & & \downarrow{\widehat{\alpha}_{A^n}} & & \downarrow{\widehat{\alpha}_M} & & \\
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & D_A(D_A(M)) & \to & 0 .
\end{array}
$$

Since $\widehat{\alpha}_A$ is equal to $1_{\widehat{A}}$, it follows that $\widehat{\alpha}_M$ is an isomorphism.

It remains to prove the equality $\operatorname{long}_A(M) = \operatorname{long}_A(D_A(M))$ when $M$ is of finite length. We may suppose $M \neq 0$; there then exists an exact sequence

$$
0 \to \kappa_A \longrightarrow M \longrightarrow N \to 0 ,
$$

whence one deduces an exact sequence

$$
0 \to D_A(N) \longrightarrow D_A(M) \longrightarrow D_A(\kappa_A) \to 0 .
$$

One has $\operatorname{long}_A(M) = \operatorname{long}_A(N) + 1$ and

$$
\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(D_A(N)) + \operatorname{long}_A(D_A(\kappa_A)) = \operatorname{long}_A(D_A(N)) + 1 ;
$$

one concludes by induction on the integer $\operatorname{long}_A(M)$.

#### Remark {#ac-x-s8-n3-rem-1 .statement}

Suppose the ring $A$ artinian. One has $\operatorname{long}_A(I) = \operatorname{long}_A(D_A(A)) = \operatorname{long}(A)$ (Theorem 2, c)). Let $M$ be a finitely generated $A$-module; it admits an injective envelope isomorphic to $I^s$, where $s$ is the dimension of the socle of $M$ (Lemma 4). Hence one has $\operatorname{long}_A(M) \leq s \operatorname{long}(A)$; for equality to hold, it is necessary and sufficient that $M$ be injective. In particular, for the $A$-module $A$ to be injective, it is necessary and sufficient that its socle be of dimension 1; thus one recovers Lemma 1 of § 3, No. 7.

### 4. Duality of modules of finite length

Let $A$ be a noetherian ring; let $\Omega$ denote the set of its maximal ideals. Generalizing the definition given in the preceding number, we shall say that an $A$-module $J$ is a Matlis $A$-module if it is injective, if its associated prime ideals are the maximal ideals of $A$, and if for every maximal ideal $m$ of $A$ the $A/m$-vector space $\operatorname{Hom}_A(A/m, J)$ is of dimension 1. For every $m \in \Omega$, let us choose an injective envelope $\kappa(m) \to I(m)$ of the $A$-module $\kappa(m)$; the $A$-module $\bigoplus_{m \in \Omega} I(m)$ is a Matlis module, and every Matlis $A$-module is isomorphic to it (No. 1, Theorem 1).

Let us recall (VIII, § 1, No. 5) that one denotes by $Z_0(A)$ the $\mathbf{Z}$-module $\mathbf{Z}^{(\Omega)}$ and by $\varepsilon : Z_0(A) \to \mathbf{Z}$ the linear form which maps each element of the basis $\Omega$ to 1. If $M$ is an $A$-module of finite length, the $A_m$-module $M_m$ is of finite length for every $m \in \Omega$, and is zero except for a finite number of ideals $m \in \Omega$. We put

$$
z_0(M) = \sum_{m \in \Omega} \operatorname{long}_{A_m}(M_m)[m] \text{ in } Z_0(A) ;
$$

one has $\operatorname{long}_A(M) = \varepsilon(z_0(M))$ (*loc. cit.*, example 3). Conversely, an $A$-module $N$ such that $\operatorname{long}_{A_m}(N_m)$ is finite for every $m \in \Omega$, and zero outside a finite subset $I$ of $\Omega$, is of finite length: in fact $N$ is isomorphic to a submodule of $\bigoplus_{m \in I} N_m$ (II, § 3, No. 3, cor. 2 of th. 1), and one has $\operatorname{long}_{A_m}(N_m) = \operatorname{long}_A(N_m)$ since every simple $A_m$-module is isomorphic to $\kappa(m)$, hence simple as an $A$-module.

Let $J$ be a Matlis $A$-module. For every $A$-module $M$, we shall denote by $D_A(M)$, or simply by $D(M)$, the $A$-module $\operatorname{Hom}_A(M, J)$. Let $\alpha_M$ be the homomorphism from $M$ into $D(D(M))$ defined by $\alpha_M(m)(f) = f(m)$ for $m \in M,\ f \in D(M)$.

#### Proposition 4 {#ac-x-s8-prop-4 .statement}

For the a-module M to be of finite length, it is necessary and sufficient that D(M) be of finite length. One then has $z_0(D(M)) = z_0(M)$, $\operatorname{long}_A(M) = \operatorname{long}_A D(M)$, $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$, and the a-linear mapping $\alpha_M$ is bijective.

For every $m \in \Omega$, the $A_m$-module $D(M)_m$ is identified with $\operatorname{Hom}_{A_m}(M_m, J_m)$ (II, § 2, No. 7, prop. 19); the first assertion of the proposition then follows from th. 2, c) and from the characterization of modules of finite length given above. Henceforth suppose M to be of finite length; one has $\operatorname{long}_{A_m}(D(M)_m) = \operatorname{long}_{A_m}(M_m)$ for every $m \in \Omega$ (*loc. cit.*), whence $z_0(D(M)) = z_0(M)$ and $\operatorname{long}_A(D(M)) = \operatorname{long}_A(M)$. Moreover the mapping $(\alpha_M)_m : M_m \to D(D(M))_m$ is identified with the canonical homomorphism $\alpha_{M_m}$, which is bijective (*loc. cit.*); consequently $\alpha_M$ is bijective.

For every $a \in A$ one has $D(a_M) = a_{D(M)}$ and consequently $\operatorname{Ann}_A(M) \subset \operatorname{Ann}_A(D(M))$. Applying this to the a-module D(M), one deduces the opposite inclusion, whence the equality $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$.

#### Example {#ac-x-s8-n4-exa-1 .statement}

Let A be a principal ideal domain, K its field of fractions. *The A-module K/A is a Matlis module*: in fact the canonical mapping from K/A into $\prod_{m \in \Omega} K/A_m$ induces an isomorphism from K/A onto $\bigoplus_{m \in \Omega} K/A_m$ (A, VII, p. 10, th. 2); the assertion then follows from No. 1, example 1. We have moreover already proved in A, VII, § 4, No. 9 that the mapping $\alpha_M$ is bijective for every $A$-module M of finite length when the ring A is principal.

### 5. Dualizing functors

In this number, let $A$ be a fixed noetherian local ring. Suppose given
a) for every $A$-module $M$ of finite length, an $A$-module $T(M)$ ;
b) for every a-linear mapping $f : M \to N$ between $A$-modules of finite length, an a-linear mapping $T(f) : T(N) \to T(M)$,
in such a way that the following conditions are satisfied:
FD 1) The mappings $f \mapsto T(f)$ are a-linear.
FD 2) For every $A$-module $M$ of finite length, one has $T(1_M) = 1_{T(M)}$.
FD 3) For every diagram $M \xrightarrow{f} N \xrightarrow{g} P$ of $A$-modules of finite length and a-linear mappings, one has $T(g \circ f) = T(f) \circ T(g)$.
FD 4) For every exact sequence $M' \xrightarrow{u} M \xrightarrow{v} M''$ of $A$-modules of finite length, the sequence $T(M'') \xrightarrow{T(v)} T(M) \xrightarrow{T(u)} T(M')$ is exact.
FD 5) The $A$-module $T(\kappa_A)$ is of length 1.

From FD 1) and FD 2), one deduces $T(a_M) = a T(1_M) = a 1_{T(M)} = a_{T(M)}$ for every $a \in A$. Taking $M = \{0\}$, one obtains $0_{T(M)} = 1_{T(M)}$, hence $T(\{0\}) = \{0\}$. It follows from this and from FD 4) that for every injective (resp. surjective) linear mapping between $A$-modules of finite length, the mapping $T(f)$ is surjective (resp. injective).

Let $M$ be an $A$-module of finite length. Then $T(M)$ is of finite length and one has $\operatorname{long}_A(T(M)) = \operatorname{long}_A(M)$: this follows in fact from FD 4) and FD 5) and from the fact that every module of finite length admits a composition series whose quotients are isomorphic to $\kappa_A$.

Let $M$ be an $A$-module of finite length, and $(e_\lambda)_{\lambda \in L}$ an orthogonal family of projections of $M$; by FD 3), $(T(e_\lambda))_{\lambda \in L}$ is an orthogonal family of projections of $T(M)$. Hence, if $M$ is the direct sum of a family of submodules $(M_\lambda)_{\lambda \in L}$, and if $p_\lambda$ denotes the projection of $M$ onto $M_\lambda$, the homomorphism
$$
\sum_{\lambda \in L} T(p_\lambda) : \bigoplus_{\lambda \in L} T(M_\lambda) \longrightarrow T(M)
$$
is an isomorphism.

#### Example 1 {#ac-x-s8-n5-exa-1 .statement}

Let $J$ be a Matlis $A$-module. Put $T(M) = \operatorname{Hom}_A(M, J)$ for every $A$-module $M$ of finite length and $T(f) = \operatorname{Hom}_A(f, 1_J)$ for every $A$-linear mapping $f$ between $A$-modules of finite length. Then conditions FD 1) to FD 5) are satisfied. We shall see below (th. 3) that every construction satisfying conditions FD 1) to FD 5) is obtained in this way.

#### Example 2 {#ac-x-s8-n5-exa-2 .statement}

Let $C$ be an injective complex of $A$-modules and $d$ an integer such that $H^i(\operatorname{Homgr}_A(\kappa_A, C))$ is zero for $i \neq d$ and is of length 1 for $i = d$. For every $A$-module $M$ of finite length, one has $H^i(\operatorname{Homgr}_A(M, C)) = 0$ for $i \neq d$; let us argue in fact by induction on the length of $M$, supposed $> 0$; there exists an exact sequence of $A$-modules $0 \to \kappa_A \to M \to N \to 0$, which gives rise to an exact sequence of complexes
$$
0 \to \operatorname{Homgr}_A(N, C) \longrightarrow \operatorname{Homgr}_A(M, C) \longrightarrow \operatorname{Homgr}_A(\kappa_A, C) \longrightarrow 0
$$
and the conclusion follows from the induction hypothesis applied to $N$.

Let $T(M) = H^d(\operatorname{Homgr}_A(M, C))$ for every $A$-module $M$ of finite length, and $T(f) = H^d(\operatorname{Homgr}_A(f, 1_C))$ for every $A$-linear mapping $f$ between $A$-modules of finite length; conditions FD 1) to FD 5) are satisfied.

#### Example 3 {#ac-x-s8-n5-exa-3 .statement}

Let $\Omega$ be an $A$-module and $d$ an integer $\geqslant 0$ such that $\operatorname{Ext}_A^i(\kappa_A, \Omega)$ is zero for $i \neq d$ and has length 1 for $i = d$. Set $T(M) = \operatorname{Ext}_A^d(M, \Omega)$ for every $A$-module $M$ of finite length and $T(f) = \operatorname{Ext}_A^d(f, 1_\Omega)$ for every $A$-linear mapping $f$ between $A$-modules of finite length. Then $\operatorname{Ext}_A^i(M, \Omega) = 0$ for every $A$-module $M$ of finite length and every $i \neq d$, and conditions FD 1) to FD 5) are satisfied: it is enough, in fact, to apply the preceding example to the case where $C$ is the canonical injective resolution of $\Omega$.

#### Example 4 {#ac-x-s8-n5-exa-4 .statement}

If $A$ is a Gorenstein ring, for example a regular ring, one can apply Example 3 by taking $\Omega = A$ and $d = \dim(A)$ (§ 3, No. 7, Prop. 11).

For every integer $n \geqslant 0$, set $I_n = T(A/\mathfrak{m}_A^n)$. For $m \geqslant n$, denote by $p_{mn} : A/\mathfrak{m}_A^m \longrightarrow A/\mathfrak{m}_A^n$ the canonical surjection and by $i_{mn} : T(A/\mathfrak{m}_A^n) \longrightarrow T(A/\mathfrak{m}_A^m)$ the $A$-linear mapping $T(p_{mn})$. It is injective by FD 4), and one has $i_{mn} \circ i_{np} = i_{mp}$ for $m \geqslant n \geqslant p$ by FD 3). Let $I = \varprojlim T(A/\mathfrak{m}_A^n)$ be the inductive limit $A$-module of the system $((I_n), (i_{mn}))$. For $n \geqslant 0$, the canonical mapping $I_n \to I$ is injective; we identify $I_n$ with its image in $I$, so that $I$ is the increasing union of the $I_n$.

Let M be an A-module of finite length, and n an integer $\geqslant 0$ such that $m_A^n M = 0$. For $x \in M$, let us denote by $\varphi_{M,x}^n$ the a-linear mapping of $A/m_A^n$ into M which maps the class of 1 to x. The mapping $T(\varphi_{M,x}^n) : T(M) \to I_n$ is a-linear, and one has $T(\varphi_{M,a x}^n) = a T(\varphi_{M,x}^n)$ for $a \in A$ by FD 1). Hence the mapping $(x, u) \mapsto T(\varphi_{M,x}^n)(u)$ of $M \times T(M)$ into I is A-bilinear. It does not depend on the choice of the integer n: in fact, for every integer $q \geqslant n$ and every element x of M, one has $\varphi_{M,x}^q = \varphi_{M,x}^n \circ p_{q n}$, whence by FD 3) $T(\varphi_{M,x}^q) = i_{q n} \circ T(\varphi_{M,x}^n)$. We deduce an a-linear mapping
$$
\theta_M : T(M) \longrightarrow \operatorname{Hom}_A(M, I)
$$
satisfying $\theta_M(u)(x) = T(\varphi_{M,x})(u)$ for $u \in T(M),\ x \in M$.

#### Theorem 3 {#ac-x-s8-thm-3 .statement}

a) The A-module I is a Matlis module. For every integer $m \geqslant 0$, $I_m$ is the a-submodule of I consisting of the elements annihilated by $m_A^m$.

b) For every A-module M of finite length, the a-linear mapping $\theta_M : T(M) \to \operatorname{Hom}_A(M, I)$ is bijective.

c) For every a-linear mapping $f : M \to N$ between A-modules of finite length, one has $\theta_M \circ T(f) = \operatorname{Hom}_A(f, 1_I) \circ \theta_N$.

Let us prove c). Let n be an integer and M, N A-modules of finite length annihilated by $m_A^n$. Let $f : M \to N$ be an a-linear mapping. For $u$ in $T(N)$ and x in M, one has by FD 3)
$$
\begin{align*}
\theta_M(T(f)(u))(x) &= T(\varphi_{M,x}^n)(T(f)(u)) = T(f \circ \varphi_{M,x}^n)(u) \\
&= T(\varphi_{N,f(x)}^n)(u) = \theta_N(u)(f(x)) = (\theta_N(u) \circ f)(x) .
\end{align*}
$$
This proves c).

Let us prove b). First consider the particular case $M = A/m_A^n$. Then $T(M)$ is equal by definition to $I_n$. If $a$ is an element of A, of class $\bar{a}$ in M, one has $\varphi_{M,\bar{a}}^n = a 1_M$, whence $T(\varphi_{M,\bar{a}}^n) = a 1_{I_n}$; thus $\theta_M : I_n \to \operatorname{Hom}_A(A/m_A^n, I)$ is the canonical isomorphism which sends an element $x$ of $I_n$ to the mapping $\bar{a} \mapsto a x$. This proves b) in this case.

Now suppose given an exact sequence
$$
P \xrightarrow{u} N \xrightarrow{v} M \to 0
$$
of A-modules of finite length annihilated by $m_A^n$. Consider the diagram
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(M) & \xrightarrow{T(v)} & T(N) & \xrightarrow{T(u)} & T(P) \\
   &                & \downarrow{\theta_M} &           & \downarrow{\theta_N} &           & \downarrow{\theta_P} \\
0 & \longrightarrow & \operatorname{Hom}_A(M, I) & \xrightarrow{\operatorname{Hom}(v, 1)} & \operatorname{Hom}_A(N, I) & \xrightarrow{\operatorname{Hom}(u, 1)} & \operatorname{Hom}_A(P, I)
\end{array}
$$

it is commutative by the beginning of the proof, and its rows are exact by FD 4). We deduce that $\theta_M$ is bijective if $\theta_P$ and $\theta_N$ are so. Applying this to a presentation
$$
(A/\mathfrak{m}_A^n)^r \longrightarrow (A/\mathfrak{m}_A^n)^s \longrightarrow M \longrightarrow 0
$$
of the $A/\mathfrak{m}_A^n$-module $M$, we deduce that $\theta_M$ is bijective for every $A$-module of finite length annihilated by $\mathfrak{m}_A^n$, whence b).

Let us prove a). It follows from the foregoing applied to the $A$-module $A/\mathfrak{m}_A^n$ that $I_n$ is the set of elements of $I$ which are annihilated by $\mathfrak{m}_A^n$. By FD 5) the $A$-module $I_1 = T(\kappa_A)$ is isomorphic to $\kappa_A$; by Prop. 2 of No. 2, it is enough for us to prove that, for every integer $n \geqslant 0$, the canonical $A$-linear mapping
$$
\beta : I_{n+1}/I_n \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
is bijective. Now from the exact sequence
$$
0 \longrightarrow \mathfrak{m}_A^n/\mathfrak{m}_A^{n+1} \xrightarrow{u} A/\mathfrak{m}_A^{n+1} \xrightarrow{p_{n+1,n}} A/\mathfrak{m}_A^n \longrightarrow 0,
$$
one deduces an exact sequence
$$
0 \longrightarrow I_n \xrightarrow{i_{n+1,n}} I_{n+1} \xrightarrow{T(u)} T(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}) \longrightarrow 0.
$$
By composing $T(u)$ with $\theta_{\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}}$, one thus obtains a surjective homomorphism
$$
\gamma : I_{n+1} \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
with kernel $I_n$. By c), $\gamma$ is the composite of the arrows $\theta_{I_{n+1}} : I_{n+1} \to \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I)$ and $\mathrm{Hom}(u, 1) : \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I) \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$; since $\theta_{I_{n+1}}$ is the linear mapping associated with the multiplication $A/\mathfrak{m}_A^{n+1} \times I_{n+1} \to I$, the isomorphism $I_{n+1}/I_n \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$ deduced from $\gamma$ coincides with $\beta$, which completes the proof.

#### Example 5 {#ac-x-s8-n5-exa-5 .statement}

Let us take up again the hypotheses and notations of Example 1. Then $T(A/\mathfrak{m}_A^n) = \mathrm{Hom}_A(A/\mathfrak{m}_A^n, J)$ is identified with the submodule $J_n$ of $J$ formed by the elements annihilated by $\mathfrak{m}_A^n$; by passing to the inductive limit one obtains a canonical isomorphism of $I$ onto $J$.

#### Example 6 {#ac-x-s8-n5-exa-6 .statement}

Let us take up again the hypotheses and notations of Example 3. One obtains that $I = \varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, \Omega)$ is a Matlis $A$-module. For every $A$-module of finite length $M$, there is a canonical $A$-isomorphism
$$
0_M : \mathrm{Ext}_A^d(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, I);
$$
moreover this isomorphism is $\mathrm{End}_A(M)$-linear (Theorem 3, c)).

In particular, if the ring $A$ is Gorenstein of dimension $d$, the $A$-module $\varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, A)$ is a Matlis module.

### 6. Change of rings; Macaulay duality

#### Proposition 5 {#ac-x-s8-prop-5 .statement}

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings, such that the residual extension $\kappa_A \to \kappa_B$ induced by $\rho$ is of finite degree. Let $I_A$ be a Matlis $A$-module.

a) Let $I_B$ denote the sub-$B$-module of $\mathrm{Hom}_A(B, I_A)$ formed by the $A$-homomorphisms from $B$ into $I_A$ whose kernel contains a power of $m_B$. Then $I_B$ is a Matlis $B$-module.

b) Let $M$ be a $B$-module. The canonical mapping

$$
\alpha : \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A)) \longrightarrow \mathrm{Hom}_A(M, I_A)
$$

defined by $\alpha(u)(m) = u(m)(1)$ induces a $B$-isomorphism of $D_B(M) = \mathrm{Hom}_B(M, I_B)$ onto the sub-$B$-module $\mathrm{Hom}_A^{cont}(M, I_A)$ of $D_A(M) = \mathrm{Hom}_A(M, I_A)$ consisting of mappings $f : M \to I_A$ such that for every element $m$ of $M$, there exists an integer $n \geqslant 0$ such that $f(m^n_B m) = 0$.

The above condition on $f$ means that $f$ is continuous when $I_A$ is given the discrete topology and $M$ the finest topology inducing on each finitely generated submodule the $m_B$-adic topology, which justifies the notation. Analogously, the condition $g \in I_B$ means that $g$ is continuous when $I_A$ is given the discrete topology and $B$ the $m_B$-adic topology.

Let us prove a). For every $B$-module of finite length $M$, denote by $T(M)$ the $B$-module $\mathrm{Hom}_A(M, I_A)$; for every $B$-linear mapping $f : M \to N$ between $B$-modules of finite length, denote by $T(f) : T(N) \to T(M)$ the $B$-linear mapping $\mathrm{Hom}_A(f, 1_{I_A})$. The verification of conditions FD 1) to FD 4) of No. 5 is immediate. Moreover, for every $B$-module of finite length $N$, one has $\mathrm{long}_A(N_{[A]}) = \mathrm{long}_B(N) \ [\kappa_B : \kappa_A]$; since one has $\mathrm{long}_A(T(M)) = \mathrm{long}_A(M)$ (No. 3, th. 2), one deduces that $\mathrm{long}_B(T(M)) = \mathrm{long}_B(M)$, which implies FD 5). We may therefore apply theorem 3 of No. 5; one has

$$
T(B/m_B^n) = \mathrm{Hom}_A(B/m_B^n, I_A),
$$

so that the Matlis $B$-module $\varprojlim T(B/m_B^n)$ is identified with the sub-$B$-module $I_B$ of $\mathrm{Hom}_A(B, I_A)$, which proves a).

Let us prove b). The mapping $\alpha$ is the inverse of the canonical isomorphism

$$
\beta : \mathrm{Hom}_A(M, 1_A) \longrightarrow \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A))
$$

which associates to $v \in \mathrm{Hom}_A(M, I_A)$ the map $v'$ of $M$ into $\mathrm{Hom}_A(B, I_A)$ such that $v'(m)(b) = v(bm)$ (A, II, p. 74, prop. 1). In order that $v'$ take its values in $I_B$, it is necessary and sufficient that $v$ belong to $\mathrm{Hom}_A^{cont}(M, I_A)$, whence b).

#### Corollary {#ac-x-s8-n6-cor-1 .statement}

a) If the $A$-algebra $B$ is finite, the $B$-module $I_B = \mathrm{Hom}_A(B, I_A)$ is a Matlis $B$-module.

b) If the $B$-module $M$ is artinian, the mapping $\alpha$ is a $B$-isomorphism of $D_B(M)$ onto $D_A(M)$.

Proposition 5 applies in particular when $A$ is a field $k$, in which case one may take $I_A = k$, hence $D_k(M) = \mathrm{Hom}_k^{cont}(M, k)$ ("Macaulay duality"). It will be noted that the assumption $[\kappa_B : k] < +\infty$ is satisfied in particular when the $k$-algebra $B$ is the local ring at a maximal ideal of a $k$-algebra of finite type (A, VIII, App. 3, cor. 1).

More particularly, consider an $\mathbf{N}$-graded $k$-algebra of finite type $S$, such that $S_0$ is a field, of finite degree over $k$. One may apply Proposition 5 to the local ring $S'$ of $S$ at the maximal ideal $S_+ = \bigoplus_{n > 0} S_n$ or, what amounts to the same thing, to its completion $\widehat{S} = \prod_{n \geq 0} S_n$ (III, § 1, No. 3, lemma 2 and § 2, No. 12, example 1). The $S$-module $I_{\widehat{S}} = \mathrm{Hom}_k^{cont}(\widehat{S}, k)$ is then identified with
$$
S^{*gr} = \bigoplus_{n \geq 0} \mathrm{Hom}_k(S_n, k)
$$
for $s \in S$ and $u \in S^{*gr}$, the element $su$ of $S^{*gr}$ is the interior product $s \perp u$ (A, III, p. 156 and p. 157). Take, for example, $S = k[T_1, \ldots, T_d]$, whence $\widehat{S} = k[[T_1, \ldots, T_d]]$. Let $(u_\alpha)_{\alpha \in \mathbf{N}^d}$ be the basis of the $k$-vector space $S^{*gr}$ dual to the basis $(T^\alpha)_{\alpha \in \mathbf{N}^d}$ of $S$. The structure of $S^{*gr}$ as $S$-module is then described by the formulae (A, III, p. 167)

$$
\begin{align*}
T^\beta u_\alpha &= u_\alpha \cdot \beta & \text{if } \alpha \geq \beta , \\
T^\beta u_\alpha &= 0 & \text{otherwise}.
\end{align*}
$$

### 7. Duality of extension modules and torsion products

Let $A$ be a ring, and $P$ and $J$ $A$-modules. For every complex $C$ of $A$-modules, a canonical isomorphism of complexes was constructed in A, X, p. 99, prop. 12
$$
\mu : \mathrm{Homgr}_A(C \otimes_A P, J) \longrightarrow \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J)) .
$$
Let $M$ be an $A$-module, and $(C, p)$ a projective resolution of $M$. Consider the sequence of homomorphisms
$$
\begin{array}{ccccccccc}
\mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\varphi^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))) & \xrightarrow{\mathrm{H}(\mu)^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C \otimes_A P, J)) \\
& \xrightarrow{u} & \mathrm{Homgr}_A(\mathrm{H}(C \otimes_A P), J) & \xrightarrow{v} & \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J) ,
\end{array}
$$

where $\varphi$ is the canonical isomorphism $\varphi(C, \mathrm{Hom}_A(P, J))$ (A, X, p. 100, th. 1), $u$ the canonical homomorphism $\lambda(C \otimes_A P, J)$ (A, X, p. 82), and $v$ is deduced from the canonical isomorphism $\psi(C, P) : \mathrm{Tor}^A(M, P) \longrightarrow \mathrm{H}(C \otimes_A P)$.

Let $(C', p')$ be another projective resolution of $M$. By A, X, p. 49, Corollary to Proposition 3, there exists a homotopism of complexes $\alpha : C' \to C$ such that $p \circ \alpha = p'$. It follows from A, X, p. 103, Proposition 2, that one has $\mathrm{H}(\alpha \otimes 1_P) \circ \psi(C', P) = \psi(C, P)$ and $\varphi(C', R) \circ \mathrm{H}(\mathrm{Homgr}(\alpha, 1_R)) = \varphi(C, R)$ for every A-module $R$. It follows that the graded homomorphism of degree 0

$$
\theta(M, P) : \mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J)
$$

which is the composite of the sequence of homomorphisms above is independent of the choice of the projective resolution $(C, p)$ of $M$. By construction it is $\mathrm{End}_A(J)$-linear.

The definition of the homomorphism $\theta(M, P)$ may be made explicit as follows. Let $p$ be an integer, $v$ an element of $\mathrm{Ext}_A^p(M, \mathrm{Hom}_A(P, J))$, $\tau$ an element of $\mathrm{Tor}_p^A(M, P)$. With the aid of the isomorphism $\varphi(C, \mathrm{Hom}_A(P, J))$, $v$ is represented by a linear mapping $u : C_p \to \mathrm{Hom}_A(P, J)$ such that $u \circ d_C = 0$; analogously, with the aid of $\psi(C, P)$, $\tau$ is represented by an element $\sum c_\mu \otimes p_\mu$ of $C_p \otimes P$ such that $\sum d_C(c_\mu) \otimes p_\mu = 0$. One then has $\theta(M, P)(v)(\tau) = \sum u(c_\mu)(p_\mu)$.

On the other hand, let $v : C \otimes_A \mathrm{Hom}_A(P, J) \longrightarrow \mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)$ be the homomorphism which maps the element $c \otimes h$, for $c \in C_p$, $h \in \mathrm{Hom}_A(P, J)$, to the homomorphism $u \mapsto (-1)^p h(u(c))$. It is graded of degree 0; it is bijective if each module $C_p$ is free of finite type. It is easily verified that this is a morphism of complexes.

Consider the sequence of homomorphisms

$$
\begin{array}{cccccc}
\mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\psi} & \mathrm{H}(C \otimes_A \mathrm{Hom}_A(P, J)) & \xrightarrow{\mathrm{H}(v)} & \mathrm{H}(\mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)) \\
& \xrightarrow{w} & \mathrm{Homgr}_A(\mathrm{H}(\mathrm{Homgr}_A(C, P)), J) & \xrightarrow{t} & \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
\end{array}
$$

where $\psi$ is the canonical isomorphism $\psi(C, \mathrm{Hom}_A(P, J))$, $w$ the canonical homomorphism $\lambda(\mathrm{Homgr}_A(C, P), J)$ (A, X, p. 82), and $t$ is deduced from the canonical isomorphism $\varphi(C, P)$. One sees as above that the composite homomorphism

$$
\rho(M, P) : \mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
$$

is independent of the choice of the resolution $C$; it is $\mathrm{End}_A(J)$-linear. Let $p$ be an integer, $\xi \in \mathrm{Tor}_p^A(M, \mathrm{Hom}_A(P, J))$, $\lambda \in \mathrm{Ext}_A^p(M, P), J)$; if $\xi$ is represented with the aid of $\psi(C, \mathrm{Hom}_A(P, J))$ by an element $\sum c_\mu \otimes u_\mu$ of $C \otimes \mathrm{Hom}_A(P, J)$ such that $\sum d_C(c_\mu) \otimes u_\mu = 0$, and $\lambda$ with the aid of $\varphi(C, P)$ by a homomorphism $\ell : C_p \to P$ such that $\ell \circ d_C = 0$, one has $\rho(M, P)(\xi)(\lambda) = (-1)^p \sum u_\mu(\ell(c_\mu))$.

#### Proposition 6 {#ac-x-s8-prop-6 .statement}

*Suppose the A-module J injective; for every A-module N, put $D(N) = \mathrm{Hom}_A(N, J)$.*

a) The homomorphisms $\theta^i(M, P) : \mathrm{Ext}_A^i(M, D(P)) \longrightarrow D(\mathrm{Tor}_i^A(M, P))$ are bijective.

b) If the ring $A$ is noetherian and the $A$-module $M$ of finite type, the homomorphisms $\rho_i(M, P) : \mathrm{Tor}_i^A(M, D(P)) \longrightarrow D(\mathrm{Ext}_A^i(M, P))$ are bijective.

a) By construction, the homomorphism $\theta(M, P)$ is bijective as soon as $\lambda(C \otimes_A P, J)$ is bijective, which is the case when $J$ is injective (A, X, p. 85, Corollary 2).

b) Choose the resolution $C$ so that each module $C_p$ is free of finite type (A, X, p. 53, Proposition 6). Then the homomorphism $\nu$ is bijective, and the same is true of $\lambda(\mathrm{Homgr}_A(C, P), J)$ since $J$ is injective; hence $\rho(M, P)$ is bijective.

#### Remark 1 {#ac-x-s8-n7-rem-1 .statement}

For every homomorphism $f : N \to N'$ of $A$-modules, let us denote by $D(f) : D(N') \to D(N)$ the homomorphism $\mathrm{Hom}(f, 1_J)$. Let $u : M \to M'$ and $v : P \to P'$ be homomorphisms of $A$-modules. Choose projective resolutions $(C, p)$ of $M$ and $(C', p')$ of $M'$, and a morphism of complexes $\tilde{u} : C \to C'$ such that $p' \circ \tilde{u} = u \circ p$ (A, X, p. 49, Proposition 3). The diagram

$$
\begin{array}{ccc}
\mathrm{Homgr}_A(C' \otimes_A P', J) & \xrightarrow{\mu'} & \mathrm{Homgr}_A(C', \mathrm{Hom}_A(P', J)) \\
\downarrow \mathrm{Hom}(\tilde{u} \otimes v, 1_J) & & \downarrow \mathrm{Hom}(\tilde{u}, \mathrm{Hom}(v, 1)) \\
\mathrm{Homgr}_A(C \otimes_A P, J) & \xrightarrow{\mu} & \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))
\end{array}
$$

where $\mu$ and $\mu'$ are the canonical homomorphisms, is commutative; one then deduces from A, X, p. 103, Proposition 2 a commutative diagram

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P')) & \xrightarrow{\theta^i(M', P')} & D(\mathrm{Tor}_i^A(M', P')) \\
\downarrow \mathrm{Ext}^i(u, D(v)) & & \downarrow D(\mathrm{Tor}_i(u, v)) \\
\mathrm{Ext}_A^i(M, D(P)) & \xrightarrow{\theta^i(M, P)} & D(\mathrm{Tor}_i^A(M, P))
\end{array}
$$

Let $w : P'' \to P$ be a homomorphism of $A$-modules; one obtains analogously a commutative diagram

$$
\begin{array}{ccc}
\mathrm{Tor}_i^A(M, D(P)) & \xrightarrow{\rho_i(M, P)} & D(\mathrm{Ext}_A^i(M, P)) \\
\downarrow \mathrm{Tor}_i(u, D(w)) & & \downarrow D(\mathrm{Ext}^i(u, w)) \\
\mathrm{Tor}_i^A(M', D(P'')) & \xrightarrow{\rho_i(M', P'')} & D(\mathrm{Ext}_A^i(M', P''))
\end{array}
$$

#### Remark 2 {#ac-x-s8-n7-rem-2 .statement}

Let

$$(\mathcal{E})$$
$$0 \to M' \xrightarrow{j} M \xrightarrow{q} M'' \to 0$$

be an exact sequence of $A$-modules. The homomorphism $L(q) : L(M) \to L(M'')$ induced on the canonical free resolutions is surjective, and the complex $Ker\,L(q)$ defines a projective resolution of $M'$. Applying Proposition 3 of A, X, p. 104 to the exact sequence $0 \to Ker\,L(q) \to L(M) \to L(M'') \to 0$, one obtains commutative diagrams

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P)) & \xrightarrow{\theta^i(M', P)} & D(\mathrm{Tor}_i^A(M', P)) \\
\downarrow & & \downarrow \\
\delta^i(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\partial_{i+1}(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M'', D(P)) & \xrightarrow{\theta^{i+1}(M'', P)} & D(\mathrm{Tor}_{i+1}^A(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\partial_{i+1}(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\delta^i(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_i^A(M', D(P)) & \xrightarrow{\rho_i(M', P)} & D(\mathrm{Ext}_A^i(M', P))
\end{array}
$$

Let

$$(\mathcal{F})$$
$$0 \to P' \to P \to P'' \to 0$$

be an exact sequence of $A$-modules; since the $A$-module $J$ is injective, one deduces from it an exact sequence

$$(\mathcal{D}(\mathcal{F}))$$
$$0 \to D(P'') \to D(P) \to D(P') \to 0.$$

Applying A, X, p. 104, Proposition 3 and p. 106, Proposition 4 to the exact sequences $(\mathcal{F})$ and $(\mathcal{D}(\mathcal{F}))$, one obtains analogously commutative diagrams

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M, D(P')) & \xrightarrow{\theta^i(M, P')} & D(\mathrm{Tor}_i^A(M, P')) \\
\downarrow & & \downarrow \\
\delta^i(M, D(\mathcal{F})) & & (-1)^{i+1}D(\partial_{i+1}(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M, D(P'')) & \xrightarrow{\theta^{i+1}(M, P'')} & D(\mathrm{Tor}_{i+1}^A(M, P''))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^{\mathbf{A}}(M, D(P')) & \xrightarrow{\rho_{i+1}(M, P')} & D(\mathrm{Ext}_{\Lambda}^{i+1}(M, P')) \\
\downarrow & & \downarrow \\
\partial_{i+1}(M, D(\mathcal{F})) & & (-1)^i D(\delta^i(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i}^{\mathbf{A}}(M, P'') & \xrightarrow{\rho_{i}(M, P'')} & D(\mathrm{Ext}_{\Lambda}^{i}(M, P''))
\end{array}
$$

## EXERCISES {#ac-x-s8-exercises}

See the [exercises for § 8](exercises/s8/).
