---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 10
section_title: Cohomologie locale, dualité de Grothendieck
lang: en
source: ac-x-fr
pdf_pages: 0141-0150, 0178-0180
extraction: ocr
subsections:
    - "no": 1
      title: Cohomologie locale
      page: 0
      pdf_page: 141
    - "no": 2
      title: Cohomologie locale sur un anneau de Macaulay
      page: 145
      pdf_page: 144
    - "no": 3
      title: Dualité de Grothendieck sur un anneau de Macaulay
      page: 147
      pdf_page: 146
statements: 20
exercises: 11
content_sha256: 5249772d053544eedc1734bed7c660da3174e2c1d5383a26977e65276609f491
translated_from: content/fr/ac/X/10_s10_cohomologie_locale_dualite_de.md
source_lang: fr
translation_method: machine
source_content_sha256: e8bae18987bec37ceb60f14d75f74c46d0c21bd1844866f4cb791e7a520a550f
translation_model: gpt-5.4
translation_run: translate-en-mt-aef7963f
glossary_version: 34
glossary_terms_sha256: 5c3e402cd5fe2210d83c169a3fb624d3a1ae7624e6c39e7afbc5df84f03b9864
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 10. LOCAL COHOMOLOGY, GROTHENDIECK DUALITY

### 1. Local cohomology

In this No., we consider a local noetherian ring $A$. Recall (VIII, § 3, No. 3, Lemma 2) that the ideals of definition of $A$ are the ideals of $A$ distinct from $A$ containing a power of $m_A$, or again the ideals $a \subset m_A$ such that $A/a$ is of finite length. We denote by $\mathscr{D}$ the set of ideals of definition of $A$, endowed with the order relation opposite to inclusion; it is filtering to the right.

Let $M$ be an $A$-module. To every ideal of definition $a$ of $A$ let us associate the graded $A$-module $\mathrm{Ext}_A(A/a, M)$; if $a$ and $b$ are ideals of definition with $a \subset b$, let $p_{ab} : A/a \to A/b$ denote the canonical mapping and consider the $A$-linear mapping $\mathrm{Ext}(p_{ab}, 1_M) : \mathrm{Ext}_A(A/b, M) \longrightarrow \mathrm{Ext}_A(A/a, M)$. Thus one obtains an inductive system of graded $A$-modules and graded $A$-linear mappings of degree 0 relative to the ordered set $\mathscr{D}$. The graded $A$-module $\varprojlim_{a \in \mathscr{D}} \mathrm{Ext}_A(A/a, M)$ is called the *local cohomology module* of $M$, and is denoted by $H_A(M)$.

The ideals $m_A^n$ for $n \geq 1$ form a cofinal subset of $\mathscr{D}$; hence there is a canonical isomorphism of graded modules $\varprojlim_n \mathrm{Ext}_A(A/m_A^n, M) \longrightarrow H_A(M)$. It follows that every element of $H_A(M)$ is annihilated by a power of $m_A$.

#### Remark 1 {#ac-x-s10-n1-rem-1 .statement}

Let $X$ be the topological space $\mathrm{Spec}(A)$, $\mathcal{O}_X$ the structural sheaf of rings and $\widetilde{M}$ the $\mathcal{O}_X$-module associated with $M$. The graded $A$-module $H_A(M)$ is identified with the module $H_{\{m_A\}}(X, \widetilde{M})$ of cohomology with support in the closed point $m_A$ of $X$.

For every homomorphism $f : M \to N$ of $A$-modules, the mappings $\mathrm{Ext}_A(1_{A/a}, f) : \mathrm{Ext}_A(A/a, M) \longrightarrow \mathrm{Ext}_A(A/a, N)$ form an inductive system of graded linear mappings. By passing to the inductive limit, one obtains a graded homomorphism $H_A(f) : H_A(M) \to H_A(N)$. For every sequence $M \xrightarrow{f} N \xrightarrow{g} P$ of $A$-modules and homomorphisms, one has $H_A(g \circ f) = H_A(g) \circ H_A(f)$. Let

$$
\begin{array}{ccccccccc}
0 & \to & M & \xrightarrow{f} & N & \xrightarrow{g} & P & \to & 0
\end{array}
$$

be an exact sequence of $A$-modules. By $\Lambda$, X, p. 90, Prop. 8, the connecting homomorphisms of the extension modules $\mathrm{Ext}_A(A/a, P) \longrightarrow \mathrm{Ext}_A(A/a, M)$ form an inductive system of $A$-linear mappings, graded of (ascending) degree +1. By passing to the inductive limit, one deduces an $A$-homomorphism $\partial(\mathscr{E}) : H_A(P) \to H_A(M)$, graded of degree +1, which makes exact the sequence of homomorphisms

$$
\ldots \longrightarrow H_A^{n-1}(P) \xrightarrow{\partial^{n-1}(\mathscr{E})} H_A^n(M) \xrightarrow{H_A^n(f)} H_A^n(N) \xrightarrow{H_A^n(g)} H_A^n(P) \xrightarrow{\partial^n(\mathscr{E})} H_A^{n+1}(M) \longrightarrow \ldots
$$

Let M be an a-module. For every ideal $\alpha$ of A, the A-module $\mathrm{Hom}_A(A/\alpha, M)$ is canonically identified with the submodule of M consisting of the elements annihilated by $\alpha$. Thus $H_A^0(M)$ is identified with the submodule of M consisting of the elements $m$ which are annihilated by a power of $\mathfrak{m}_A$, that is to say such that $\mathrm{long}_A(Am) < +\infty$. In particular one has $H_A^0(M) = M$ when M is artinian.

#### Example 1 {#ac-x-s10-n1-exa-1 .statement}

If M is injective, the A-module $H_A^i(M)$ is zero for $i > 0$ and injective for $i = 0$ (§ 8, No. 2, lemma 1, c)).

#### Example 2 {#ac-x-s10-n1-exa-2 .statement}

If $H_A^0(M) = M$ (for example if M is artinian), $H_A^i(M)$ is zero for $i > 0$. Let in fact (I, e) be an injective envelope of M. The submodule $H_A^0(I)$ of I is injective (example 1) and contains $e(M)$, hence is equal to I. Put $N = \mathrm{Coker}\,e$ and consider the exact sequence $0 \to M \xrightarrow{e} I \xrightarrow{p} N \to 0$. Since $I = H_A^0(I)$, one has $N = H_A^0(N)$ and the homomorphism $H_A^0(p)$ is surjective. Since $H_A^i(I)$ is zero for $i > 0$ (example 1), $H_A^1(M)$ is zero and $H_A^i(M)$ is isomorphic to $H_A^{i-1}(N)$ for $i > 1$; one concludes by reasoning by induction on the integer $i$.

#### Example 3 {#ac-x-s10-n1-exa-3 .statement}

Let $\Omega$ be a dualizing A-module. For $i \neq \dim(A)$, one has $\mathrm{Ext}_A^i(A/\alpha, \Omega) = 0$ for every ideal of definition $\alpha$ of A (§ 8, No. 5, example 3), whence $H_A^i(\Omega) = 0$; for $i = \dim(A)$, the A-module $H_A^i(\Omega)$, which is isomorphic to $\varprojlim \mathrm{Ext}_A^i(A/\mathfrak{m}_A^n, \Omega)$, is a Matlis module (*loc. cit.*, example 6).

#### Example 4 {#ac-x-s10-n1-exa-4 .statement}

Let A be a noetherian local integral ring; let K denote its field of fractions, and suppose that $A \neq K$. It is an injective A-module (A, X, p. 18, example 1), so that the module $H_A(K)$ is zero (example 1). From the exact sequence $0 \to A \to K \to K/A \to 0$, one obtains for every $i$ an isomorphism $H_A^i(K/\Lambda) \to H_A^{i+1}(A)$.

More generally, for every torsion-free A-module M and every integer $i$, one deduces from the exact sequence

$$
0 \to M \to K \otimes_A M \to (K/A) \otimes_A M \to 0
$$

an isomorphism $H_A^i((K/A) \otimes_A M) \to H_A^{i+1}(M)$.

#### Example 5 {#ac-x-s10-n1-exa-5 .statement}

Let us retain the hypotheses of the preceding example and suppose moreover that $\dim(A) = 1$. Let N be a torsion A-module; since every nonzero ideal of A distinct from A is an ideal of definition (VIII, § 1, No. 3, prop. 6, e)), one has $H_A^0(N) = N$, and consequently $H_A^i(N) = 0$ for $i > 0$ (example 2).

Let M be an A-module; let $T(M)$ denote its torsion submodule. Consider the long exact local cohomology sequence associated with the exact sequence

$$
0 \to T(M) \to M \to M/T(M) \to 0 ;
$$

in view of the foregoing, one deduces from it canonical isomorphisms $T(M) \to H_A^0(M)$ and $H_A^1(M) \to H_A^1(M/T(M))$. Since the canonical homomorphism $(K/A) \otimes_A M \to (K/A) \otimes_A (M/T(M))$ is bijective, one finally obtains *canonical isomorphisms*

$$
H_A^0(M) \to T(M) , \qquad H_A^1(M) \to (K/A) \otimes_A M .
$$

#### Proposition 1 {#ac-x-s10-prop-1 .statement}

Let $A$ be a noetherian local ring and $M$ a finitely generated $A$-module.

a) The $A$-module $H_A(M)$ is artinian, and zero in degree $> \dim(M)$.

b) Let $p = \operatorname{prof}_A(M)$. We have $H_A^i(M) = 0$ for $i < p$, and $H_A^p(M) \neq 0$ if $M$ is nonzero.

Let us prove a) by induction on $\dim(M)$. The case where $\dim(M) \leq 0$ follows from Example 2 above. Suppose $\dim(M) > 0$ and first take $M$ of the form $A/\mathfrak{p}$, where $\mathfrak{p}$ is a prime ideal of $A$ distinct from $\mathfrak{m}_A$. Let $x$ be an element of $\mathfrak{m}_A - \mathfrak{p}$; we have an exact sequence $0 \to M \xrightarrow{xM} M \longrightarrow M/xM \to 0$, with $\dim(M/xM) = \dim(M) - 1$. Hence we deduce an exact sequence of local cohomology

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

Every element of $H_A^i(M)$ is annihilated by a power of $\mathfrak{m}_A$; to prove that this module is artinian, it is enough therefore to prove that the socle of $H_A^i(M)$ is of finite dimension over $\kappa_A$ (§ 8, No. 3, Lemma 3). By the induction hypothesis, the kernel $N$ of the homothety of ratio $x$ in $H_A^i(M)$ is artinian; since $x$ belongs to $\mathfrak{m}_A$, the socle of $H_A^i(M)$ identifies with that of $N$, and is therefore of finite dimension. If $i > \dim(M)$, we have $H_A^{i-1}(M/xM) = 0$ by the induction hypothesis, so that the homothety of ratio $x$ is injective in $H_A^i(M)$; since every element of $H_A^i(M)$ is annihilated by a power of $x$, we deduce that $H_A^i(M) = 0$, whence a) in the case considered.

Let us pass to the general case. The $A$-module $M$ admits a composition series $(M_j)_{0 \leq j \leq n}$ such that each quotient $M_j/M_{j+1}$ is isomorphic to $A/\mathfrak{p}_j$, where $\mathfrak{p}_j$ is a prime ideal of $A$ (IV, § 1, No. 4, Theorem 1). Let us prove by induction on $n$ that $M$ satisfies a). The case $n = 0$ is trivial. The exact sequence $0 \to M_1 \to M \to A/\mathfrak{p}_0 \to 0$ yields an exact sequence of local cohomology

$$
H_A^i(M_1) \longrightarrow H_A^i(M) \longrightarrow H_A^i(A/\mathfrak{p}_0)
$$

the $A$-module $H_A^i(M_1)$ is artinian by the induction hypothesis, and the same is true of $H_A^i(A/\mathfrak{p}_0)$ by the cases already treated; consequently $H_A^i(M)$ is artinian. If $i > \dim(M)$, the modules $M_1$ and $A/\mathfrak{p}_0$ are of dimension $< i$; the modules $H_A^i(M_1)$ and $H_A^i(A/\mathfrak{p}_0)$ are therefore zero by the induction hypothesis and the cases already treated, which implies that $H_A^i(M) = 0$.

Suppose $M$ nonzero, and let us prove b) by induction on the integer $p = \operatorname{prof}(M)$. The case $p = 0$ follows from the definition of depth. Suppose $p > 0$ and choose an element $x$ of $\mathfrak{m}_A$ such that the homothety $x_M$ is injective. As above we obtain a local cohomology exact sequence

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

We have $\operatorname{prof}(M/xM) = \operatorname{prof}(M) - 1$ (§ 1, No. 4, prop. 7), whence $H_A^{i-1}(M/xM) = 0$ for $i < p$ by the induction hypothesis, which implies as above that $H_A^i(M) = 0$. In particular $H_A^{p-1}(M)$ is zero, so that the homomorphism $H_A^{p-1}(M/xM) \longrightarrow H_A^p(M)$ is injective; thus $H_A^p(M)$ is nonzero by the induction hypothesis.

It can be shown that the module $H_A^{\dim(M)}(M)$ is nonzero when $M$ is nonzero (exerc. 4; cf. No. 3, cor. of th. 2).

#### Corollary {#ac-x-s10-n1-cor-1 .statement}

**Let $M$ be a nonzero Macaulay $A$-module of finite type. The $A$-module $H_A^i(M)$ is zero for $i \neq \dim(M)$ and nonzero for $i = \dim(M)$.**

#### Remark 2 {#ac-x-s10-n1-rem-2 .statement}

For every ideal of definition $\alpha$ of $A$, the $A$-module $\mathrm{Ext}_A(A/\alpha, M)$ is annihilated by $\alpha$, and $A/\alpha$ identifies with $\widehat{A}/\alpha \widehat{A}$; consequently, the graded $A$-module $\mathrm{Ext}_A(A/\alpha, M)$ identifies with $\widehat{A} \otimes_A \mathrm{Ext}_A(A/\alpha, M)$, hence also with $\mathrm{Ext}_{\widehat{A}}(\widehat{A}/\alpha \widehat{A}, \widehat{A} \otimes_A M)$ (A, X, p. 111, prop. 10). The set of ideals $\alpha \widehat{A}$, for $\alpha \in \mathscr{D}$, contains the powers of $m_{\widehat{A}}$, hence is cofinal in the set of ideals of definition of $\widehat{A}$; we therefore deduce from the foregoing a canonical isomorphism of graded $A$-modules

$$
H_A(M) \longrightarrow H_{\widehat{A}}(\widehat{A} \otimes_A M)
$$

If the $A$-module $M$ is of finite type, the $A$-module $\widehat{A} \otimes_A M$ identifies with the completion $\widehat{M}$ of $M$ (III, § 3, No. 4, th. 3), and we have an isomorphism $H_A(M) \to H_{\widehat{A}}(\widehat{M})$, graded of degree 0.

### 2. Local cohomology on a Macaulay ring

In this number, it is assumed that $A$ is a local Macaulay ring; we put $\dim(A) = d$.

The ideals generated by a sequence of elements of $m_A$ completely secant for $A$ and of length $d = \dim(A)$ form a cofinal subset $\mathscr{D}_{cs}$ in the set $\mathscr{D}$ of ideals of definition of $A$. In fact, let $(x_1, \ldots, x_d)$ be a sequence of elements of $m_A$ completely secant for $A$ (§ 2, Proposition 3); for every integer $n$, the sequence $(x_1^n, \ldots, x_d^n)$ is completely secant for $A$ (A, X, p. 158, Proposition 6, c)), and generates an ideal of definition (VIII, § 3, Corollary to Proposition 3 and Theorem 1) contained in $m_A^n$.

Let $\alpha \in \mathscr{D}_{cs}$, and let $\pi : L \to A/\alpha$ be a finite free resolution, zero in degree $> d$ (for example the Koszul complex associated with a completely secant sequence for $A$ generating $\alpha$). Consider the dual $L^* = \mathrm{Homgr}_A(L, A)$ of $L$; since the depth of $A$ is equal to $d$, one has $\mathrm{Ext}_A^i(A/\alpha, A) = 0$ for $i < d$ (§ 1, Corollary 2 to Proposition 2). Since $L^*$ is of length $\leq d$, it follows that $H^i(L^*)$ is zero for $i \neq d$ and that $H^d(L^*)$ is identified with $\mathrm{Ext}_A^d(A/\alpha, A)$ (A, X, p. 100, Theorem 1). Hence there is a homologism

$$
\pi^* : L^*(-d) \longrightarrow \mathrm{Ext}_A^d(A/\alpha, A)
$$

which defines a finite free resolution of $\mathrm{Ext}_A^d(A/\alpha, A)$.

Let $M$ be an $A$-module; consider the canonical isomorphisms (*loc. cit.*)

$$
\varphi(L, M) : H(\mathrm{Homgr}_A(L, M)) \to \mathrm{Ext}_A(A/\alpha, M)
$$
$$
\psi(M, L^*(-d)) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \to H(M \otimes_A L^*)(-d)
$$

Since the complex L is finite free, the canonical morphism of complexes $M \otimes_A L^* \to \mathrm{Homgr}_A(L, M)$ is an isomorphism; it follows that there is an isomorphism of graded A-modules $H(M \otimes_A L^*) \to H(\mathrm{Homgr}_A(L, M))$. By composition of the preceding isomorphisms, one obtains an isomorphism of graded A-modules, called *canonical*,

$$
\tau(L, M) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) \longrightarrow \mathrm{Ext}_A(A/\alpha, M)
$$

which induces for each integer $i$ an isomorphism

$$
\tau^i(L, M) : \mathrm{Tor}_{d-i}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \longrightarrow \mathrm{Ext}_A^i(A/\alpha, M)
$$

For $M = A$, $\tau^d(L, A)$ is the canonical isomorphism of $A \otimes_A \mathrm{Ext}_A^d(A/\alpha, A)$ onto $\mathrm{Ext}_A^d(A/\alpha, A)$.

Let $b$ be an ideal of $\mathcal{D}_{cs}$ contained in $\alpha$. Let $\rho : R \to A/b$ be a finite free resolution of length $\leq d$ and let $p_{ab} : A/b \to A/\alpha$ be the canonical surjection. By A, X, p. 49, Proposition 3, there exists a morphism of complexes $P_{LR} : R \to L$ such that $\pi \circ P_{LR} = p_{ab} \circ \rho$. By Proposition 2 of A, X, p. 103, one has a commutative diagram

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) & \xrightarrow{\mathrm{Tor}(1_M, \mathrm{Ext}^d(p_{ab}, 1_A))} & \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/b, A))(d) \\
\downarrow \psi(L^*(-d), M) & & \downarrow \psi(R^*(-d), M) \\
H(M \otimes_A L^*) & \xrightarrow{H(1_M \otimes^t P_{LR})} & H(M \otimes_A R^*) \\
\downarrow & & \downarrow \\
H(\mathrm{Homgr}_A(L, M)) & \xrightarrow{H(\mathrm{Homgr}(P_{LR}, M))} & H(\mathrm{Homgr}_A(R, M)) \\
\downarrow \varphi(L, M) & & \downarrow \varphi(R, M) \\
\mathrm{Ext}_A(A/\alpha, M) & \xrightarrow{\mathrm{Ext}(p_{ab}, 1_M)} & \mathrm{Ext}_A(A/b, M)
\end{array}
$$

It follows first, by taking $\alpha = b$, that the isomorphism $\tau(L, M)$ does not depend on the choice of the resolution L of $A/\alpha$; let us denote it by $\tau_\alpha(M)$. It then follows that the $\tau_\alpha(M)$ for $\alpha \in \mathcal{D}_{cs}$ form an inductive system of isomorphisms. Passing to the inductive limit, and taking account of A, X, p. 70, prop. 8, one obtains for each integer $i$ an *isomorphism of a-modules*

$$
\tau^i(M) : \mathrm{Tor}_{d-i}^A(M, H_A^d(A)) \longrightarrow H_A^i(M)
$$

For $M = A$, $\tau^d(A)$ is the canonical isomorphism of $A \otimes_A H_A^d(A)$ onto $H_A^d(A)$.

#### Remark 1 {#ac-x-s10-n2-rem-1 .statement}

Let $f : M \to N$ be a homomorphism of a-modules. Using A, X, p. 103, prop. 2, one proves that the following diagrams are commutative:

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(M, H_A^d(A)) & \xrightarrow{\tau^i(M)} & H_A^i(M) \\
\downarrow \mathrm{Tor}_{d-i}(f,1) & & \downarrow H^i(f) \\
\mathrm{Tor}_{d-i}^A(N, H_A^d(A)) & \xrightarrow{\tau^i(N)} & H_A^i(N)
\end{array}
$$

#### Remark 2 {#ac-x-s10-n2-rem-2 .statement}

Let
$
(\mathcal{E}) \quad 0 \to M \to N \to P \to 0
$
be an exact sequence of a-modules. Using A, X, p. 104, prop. 3 and p. 106, prop. 4, one proves that the following diagrams are commutative:

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(P, H_A^d(A)) & \xrightarrow{\tau^i(P)} & H_A^i(P) \\
\downarrow \partial_{d-i}(\mathcal{E}, H_A^d(A)) & & \downarrow \partial^i(\mathcal{E}) \\
\mathrm{Tor}_{d-i-1}^A(M, H_A^d(A)) & \xrightarrow{\tau^{i+1}(M)} & H_A^{i+1}(M)
\end{array}
$$

#### Remark 3 {#ac-x-s10-n2-rem-3 .statement}

Consider the isomorphism
$$
\tau^d(M) : M \otimes_A H_A^d(A) \longrightarrow H_A^d(M)
$$
For $x \in M$, let us denote by $f_x$ the mapping $a \mapsto ax$ of A into M. For every $u \in H_A^d(A)$, one has
$$
\tau^d(M)(x \otimes u) = H_A^d(f_x)(u)
$$
This follows in fact from remark 1 applied to the homomorphism $f_x : A \to M$.

### 3. Grothendieck duality over a Macaulay ring

We still suppose that A is a local Macaulay ring, of dimension d. Let $\Omega$ be a dualizing A-module. The A-module $H_A^d(\Omega)$ is a Matlis module (§ 8, No. 5, example 6); in accordance with the notation of § 8, we shall put $D(M) = \mathrm{Hom}_A(M, H_A^d(\Omega))$ for every A-module M.

Consider the isomorphism $\tau^d(\Omega) : \Omega \otimes H_A^d(A) \to H_A^d(\Omega)$ (No. 2). From it one deduces a homomorphism $\omega : H_A^d(A) \to \mathrm{Hom}_A(\Omega, H_A^d(\Omega))$ which associates to an element $u$ of $H_A^d(A)$ the homomorphism $x \mapsto H_A^d(f_x)(u)$ (remark 3 above).

#### Proposition 2 {#ac-x-s10-prop-2 .statement}

*Let A be a local Macaulay ring, of dimension d*, and let $\Omega$ *be a dualizing A-module*. *The homomorphism* $\omega : H_A^d(A) \to D(\Omega)$ *is bijective*.

The homomorphism $\omega$ is the limit of the inductive system of mappings $(\omega_\alpha)_{\alpha \in \mathscr{D}_{cs}}$, where
$$
\omega_\alpha : \mathrm{Ext}_A^d(A/\alpha, A) \longrightarrow \mathrm{Hom}_A(\Omega, \mathrm{Ext}_A^d(A/\alpha, \Omega))
$$

associates to an element $u$ of $\mathrm{Ext}_A^d(A/\alpha, A)$ the mapping $x \mapsto f_x \circ u$ (A, X, p. 114). It is therefore enough to prove that each of the mappings $\omega_\alpha$ is bijective.

Let $\alpha$ be an ideal of $\mathscr{D}_{cs}$, generated by a completely secant sequence $x = (x_1, \ldots, x_d)$ for $A$. The Koszul complex $K^\bullet(x, A)$ furnishes a projective resolution of $A/\alpha$; for every $A$-module $M$, the $A$-module $H^d(\mathrm{Homgr}_A(K^\bullet(x, A), M))$ identifies canonically with $M/\alpha M$ (A, X, p. 155). From this one deduces an isomorphism (A, X, p. 100)
$$
\varphi_M : M/\alpha M \longrightarrow \mathrm{Ext}_A^d(A/\alpha, M) .
$$
Let $x \in \Omega$. Taking account of loc. cit., p. 103, prop. 2, one has a commutative diagram

$$
\begin{array}{ccc}
A/\alpha & \xrightarrow{\varphi_A} & \mathrm{Ext}_A^d(A/\alpha, A) \\
\downarrow f_x & & \downarrow \mathrm{Ext}(1_{A/\alpha}, f_x) \\
\Omega/\alpha \Omega & \xrightarrow{\varphi_\Omega} & \mathrm{Ext}_A^d(A/\alpha, \Omega)
\end{array}
$$

where $f_x$ is the homomorphism deduced from $f_x$ by passing to quotients. It follows that if for every $A$-module $M$ one identifies $\mathrm{Ext}_A^d(A/\alpha, M)$ with $M/\alpha M$ by means of $\varphi_M$, the homomorphism $\omega_\alpha$ is identified with the $A$-linear mapping of $A/\alpha$ into $\mathrm{Hom}_A(\Omega, \Omega/\alpha \Omega)$ which sends 1 to the canonical surjection, that is again with the canonical mapping $A/\alpha \longrightarrow \mathrm{End}_{A/\alpha}(\Omega/\alpha \Omega)$. But since the $A/\alpha$-module $\Omega/\alpha \Omega$ is dualizing (§ 9, No. 2, prop. 4), this mapping is bijective (§ 9, No. 4, prop. 6), which proves the proposition.

Let us identify the Matlis bidual $D(D(\Omega))$ with $\widehat{\Omega}$ by the isomorphism $\widehat{\alpha}_\Omega$ (§ 8, No. 3, th. 2, b)).

#### Corollary {#ac-x-s10-n3-cor-1 .statement}

*The homomorphism* $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ *is an isomorphism*.

Let $M$ be an $A$-module, and $i$ an integer. Consider the canonical homomorphisms (§ 8, No. 7)

$$
\rho_{d-i}(M, \Omega) : \mathrm{Tor}^A_{d-i}(M, D(\Omega)) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\theta^{d-i}(M, H^d_A(A)) : \mathrm{Ext}_A^{d-i}(M, D(H^d_A(A))) \longrightarrow D(\mathrm{Tor}^A_{d-i}(M, H^d_A(A))) .
$$

With the aid of the isomorphisms $\omega : H^d_A(A) \to D(\Omega)$, $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ (cor. 1 of prop. 2) and $\tau^i(M) : \mathrm{Tor}^A_{d-i}(M, H^d_A(A)) \to H^i_A(M)$ (No. 2), one deduces from them *canonical homomorphisms of $A$-modules*

$$
\gamma^i(M) : H^i_A(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H^i_A(M)) .
$$

#### Theorem 1 (Grothendieck Duality) {#ac-x-s10-thm-1 .statement}

Let $A$ be a local Macaulay ring, of dimension $d$, and let $\Omega$ be a dualizing $A$-module.

a) The $A$-module $H_A^d(\Omega)$ is a Matlis module; for every $A$-module $P$, let $D(P)$ denote the Matlis dual $\mathrm{Hom}_A(P, H_A^d(\Omega))$.

b) For every finitely generated $A$-module $M$ and every integer $i$, the canonical homomorphism
$$
\gamma^i(M) : H_A^i(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
is an isomorphism of artinian $A$-modules.

c) For every $A$-module $M$ and every integer $i$, the canonical homomorphism
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H_A^i(M))
$$
is an isomorphism of $\widehat{A}$-modules.

This follows from prop. 6 of § 8, No. 7.

#### Corollary {#ac-x-s10-n3-cor-2 .statement}

Let $A$ be a local Macaulay ring, and $M$ a nonzero finitely generated $A$-module, of dimension $e$. The $A$-module $H_A^e(M)$ is nonzero.

By Remark 2 of No. 1, one may suppose that the local ring $A$ is complete. In this case $A$ has a dualizing module $\Omega$ ($§ 9$, No. 3, Corollary 3 of Proposition 6); if $H_A^e(M)$ is zero, the same is true of its Matlis dual $\mathrm{Ext}_A^{d-e}(M, \Omega)$, which contradicts Proposition 3, b) of $§ 9$, No. 1.

#### Remark 1 {#ac-x-s10-n3-rem-1 .statement}

When the $A$-module $M$ is finitely generated, the $\widehat{A}$-module $\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega})$ is identified with $\widehat{A} \otimes_A \mathrm{Ext}_A^{d-i}(M, \Omega)$ ($A$, X, p. 108, Proposition 7, c)), and $\delta^i(M)$ can also be obtained by composing $D(\gamma^i(M))$ with the biduality isomorphism.

#### Remark 2 {#ac-x-s10-n3-rem-2 .statement}

Let $u : M \to M'$ be a homomorphism of $A$-modules. By Remark 1 of No. 2 and that of $§ 8$, No. 7, the following diagrams are commutative:

$$
\begin{array}{ccc}
H_A^i(M) & \xrightarrow{\gamma^i(M)} & D(\mathrm{Ext}_A^{d-i}(M, \Omega)) \\
\downarrow H_A^i(u) & & \downarrow D(\mathrm{Ext}(u,1)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow \mathrm{Ext}(u,1) & & \downarrow D(H_A^i(u)) \\
\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) & \xrightarrow{\delta^i(M)} & D(H_A^i(M))
\end{array}
$$

#### Remark 3 {#ac-x-s10-n3-rem-3 .statement}

Let

$$(\mathcal{E})$$
$$0 \to M' \to M \to M'' \to 0$$

be an exact sequence of $A$-modules. By Remark 2 of No. 2 and that of § 8, No. 7, the following diagrams are commutative:

$$
\begin{array}{ccc}
H_A^{i-1}(M'') & \xrightarrow{\gamma^{i-1}(M'')} & D(\mathrm{Ext}_A^{d-i+1}(M'', \Omega)) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\delta^d i(\mathcal{E}, \Omega)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\partial^{i-1}(\mathcal{E})) \\
\mathrm{Ext}_A^{d-i+1}(M'', \widehat{\Omega}) & \xrightarrow{\delta^{i-1}(M'')} & D(H_A^{i-1}(M''))
\end{array}
$$

#### Example {#ac-x-s10-n3-exa-1 .statement}

Let $A$ be an integral noetherian local ring of dimension 1; let $K$ denote its field of fractions. Let $\Omega$ be a dualizing $A$-module, and let $M$ be a finitely generated $A$-module. The $A$-modules $H_A^0(M)$ and $H_A^1(M)$ are canonically identified with $T(M)$ and $(K/A) \otimes_A M$ (No. 1, Example 5). With these identifications, the duality isomorphisms

$$\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad , \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))$$

(Theorem 1) are none other than the isomorphisms defined in § 9, No. 6.

Exercises

## EXERCISES {#ac-x-s10-exercises}

See the [exercises for § 10](exercises/s10/).
