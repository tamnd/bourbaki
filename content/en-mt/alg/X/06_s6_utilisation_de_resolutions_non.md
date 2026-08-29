---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 6
section_title: Utilisation de résolutions non canoniques
lang: en
source: alg-x-fr
book_pages: A X.100-A X.113, A X.189-A X.197
pdf_pages: 0106-0119, 0195-0203
extraction: ocr
subsections:
    - "no": 1
      title: Calcul des modules $\mathrm{Tor}^A(P, M)$ et $\mathrm{Ext}_A(M, N)$
      page: 100
      pdf_page: 106
    - "no": 2
      title: Calcul des applications $\mathrm{Tor}^A(g, f)$ et $\mathrm{Ext}_A(f, h)$
      page: 103
      pdf_page: 109
    - "no": 3
      title: Calcul des homomorphismes de liaison
      page: 104
      pdf_page: 110
    - "no": 4
      title: Finitude des modules d’extensions et de torsion
      page: 107
      pdf_page: 113
    - "no": 5
      title: Les homomorphismes $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ et $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$
      page: 108
      pdf_page: 114
    - "no": 6
      title: Les homomorphismes $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ et $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$
      page: 109
      pdf_page: 115
    - "no": 7
      title: Les homomorphismes $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ et $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$
      page: 110
      pdf_page: 116
    - "no": 8
      title: 'Application : homologie et cohomologie des groupes'
      page: 111
      pdf_page: 117
statements: 30
exercises: 18
content_sha256: 0c26e4c195513eda20c41eed9f564bfc5605c3675b50f3a3af22c634208610bd
translated_from: content/fr/alg/X/06_s6_utilisation_de_resolutions_non.md
source_lang: fr
translation_method: machine
source_content_sha256: 908be744602e152c7d063ad7bc7de7071838f03e3a57fb041dfa7346f158a9b6
translation_model: gpt-5.4
translation_run: translate-en-mt-0e9b7016
glossary_version: 34
glossary_terms_sha256: 4a1b90b402f82c8484d11095b6c4eb590c6a9d800a6cfebfed28f5dbd78ce0fb
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. USE OF NONCANONICAL RESOLUTIONS

We retain the conventions of § 4.

### 1. Calculation of the modules $\mathrm{Tor}^A(P, M)$ and $\mathrm{Ext}_A(M, N)$

Let $M, N$ be left $A$-modules, $P$ a right $A$-module. Let moreover $a : R \to M$ be a left resolution of $M$, $b : S \to P$ a left resolution of $P$ and $c : N \to E$ a right resolution of $N$.

By $X$, p. 49, prop. 3 and 3 bis, there exist morphisms of complexes $\alpha : L(M) \to R$, $\beta : L(P) \to S$, $\gamma : E \to I(N)$ such that $a \circ \alpha = p_M$, $b \circ \beta = p_P$, $\gamma \circ C = e_N$, and the homotopy classes of $\alpha, \beta, \gamma$ depend only on the given resolutions. By $X$, p. 64, prop. 3 and $X$, p. 84, prop. 3, the homotopy classes of the morphisms

$$
\beta \otimes \alpha : L(P) \otimes_A L(M) \to S \otimes_A R,
$$
$$
\mathrm{Homgr}_A(\alpha, \gamma) : \mathrm{Homgr}_A(R, E) \to \mathrm{Homgr}_A(L(M), I(N))
$$

depend only on the given resolutions, whence by passing to homology graded $k$-homomorphisms of degree 0

$$
\psi(S, R) : \mathrm{Tor}^A(P, M) \to H(S \otimes_A R),
$$
$$
\varphi(R, E) : H(\mathrm{Homgr}_A(R, E)) \to \mathrm{Ext}_A(M, N),
$$

independent of the choice of $\alpha, \beta, \gamma$.

For example, taking for $a, b, c$ the identity mappings of $M, P, N$ respectively, one finds the homomorphisms $\psi(P, M) : \mathrm{Tor}^A(P, M) \to P \otimes_A M$ and $\varphi(M, N) : \mathrm{Hom}_A(M, N) \to \mathrm{Ext}_A(M, N)$ introduced in $X$, p. 68, remark 2) and $X$, p. 87, remark 2).

#### Theorem 1 {#alg-x-s6-thm-1 .statement}

a) If one of the resolutions $R$ or $S$ is flat, then $\psi(S, R)$ is an isomorphism of graded $k$-modules.

b) If $R$ is projective or if $E$ is injective, $\varphi(R, E)$ is an isomorphism of graded $k$-modules.

a) Suppose for example $\mathbf R$ flat, and choose $\alpha$ and $\beta$ as above. The homomorphism $\beta\otimes\alpha$ is the composite of the morphisms

$$
L(P)\otimes_A L(M)\xrightarrow{1_{L(P)}\otimes\alpha}L(P)\otimes_A\mathbf R\xrightarrow{\beta\otimes1_{\mathbf R}}S\otimes_A\mathbf R.
$$

Since $L(P)$ (resp. $\mathbf R$) is flat and $\alpha$ (resp. $\beta$) is a homomorphism, $1_{L(P)}\otimes\alpha$ (resp. $\beta\otimes1_{\mathbf R}$) is one, by prop. 4 of X, p. 67. Therefore $\beta\otimes\alpha$ is a homomorphism and $\psi(S,R)=H(\beta\otimes\alpha)$ is bijective.

b) One reasons analogously, using prop. 4 of X, p. 86.

#### Corollary {#alg-x-s6-n1-cor-1 .statement}

If $R$ is a flat resolution of $M$, the homomorphism

$$
\psi(P,R):\operatorname{Tor}^A(P,M)\longrightarrow H(P\otimes_A R)
$$

is bijective. If $R$ is a projective resolution of $M$, the homomorphism

$$
\varphi(R,N):H(\operatorname{Homgr}_A(R,N))\longrightarrow \operatorname{Ext}_A(M,N)
$$

is bijective. If $E$ is an injective resolution of $N$, the homomorphism

$$
\varphi(M,E):H(\operatorname{Homgr}_A(M,E))\longrightarrow \operatorname{Ext}_A(M,N)
$$

is bijective.

#### Remark {#alg-x-s6-n1-rem-1 .statement}

The diagram of $k$-modules

$$
\begin{array}{ccc}
\operatorname{Tor}^A(P,M)&\xrightarrow{\psi(S,R)}&H(S\otimes_A R)\\
\downarrow{\sigma_{P,M}}&&\downarrow{H(\sigma(S,R))}\\
\operatorname{Tor}^{A^\circ}(M^\circ,P^\circ)&\xrightarrow{\psi(R^\circ,S^\circ)}&H(R^\circ\otimes_{A^\circ}S^\circ),
\end{array}
$$

where $\sigma_{P,M}$ and $\sigma(S,R)$ are the *commutation isomorphisms* (X, p. 71 and 63), is commutative: it is obtained in fact, by passing to homology, from the commutative diagram of complexes

$$
\begin{array}{ccc}
L(P)\otimes_A L(M)&\xrightarrow{\beta\otimes\alpha}&S\otimes_A R\\
\downarrow{\sigma(L(P),L(M))}&&\downarrow{\sigma(S,R)}\\
L(M^\circ)\otimes_{A^\circ}L(P^\circ)&\xrightarrow{\alpha\otimes\beta}&R^\circ\otimes_{A^\circ}S^\circ
\end{array}
$$

("the morphisms $\psi$ are compatible with the commutation isomorphisms").

Analogously, let $a_1:R_1\to M$, $b_1:S_1\to P$, $c_1:N\to E_1$ be morphisms of complexes, where $R_1$ and $S_1$ are projective and right zero and $E_1$ injective and left zero. By X, p. 49, prop. 3 and 3 bis, there exist morphisms of complexes

$$
\alpha_1:R_1\to L(M),\qquad \beta_1:S_1\to L(P),\qquad \gamma_1:I(N)\to E_1
$$

such that $p_M \circ \alpha_1 = a_1, p_P \circ \beta_1 = b_1, \gamma_1 \circ e_N = c_1$, whence morphisms of complexes

$$
\beta_1 \otimes \alpha_1 : S_1 \otimes_A R_1 \to L(P) \otimes_A L(M),
$$

$$
\operatorname{Homgr}_A (\alpha_1, \gamma_1) : \operatorname{Homgr}_A (L(M), l(N)) \to \operatorname{Homgr}_A (R_1, E_1),
$$

and by passing to homology, *graded k-linear mappings of degree* 0:

$$
\psi'(S_1, R_1) : H(S_1 \otimes_A R_1) \to \operatorname{Tor}^A (P, M)
$$
$$
\varphi'(R_1, E_1) : \operatorname{Ext}_A (M, N) \to H(\operatorname{Homgr}_A (R_1, E_1))
$$

which one verifies, as above, to be independent of the choice of $\alpha_1, \beta_1, \gamma_1$.

#### Proposition 1 {#alg-x-s6-prop-1 .statement}

*If* $a_1, b_1, c_1$ *are homologisms,* $\psi'(S_1, R_1)$ *and* $\varphi'(R_1, E_1)$ *are the reciprocal bijections of the bijections* $\psi(S_1, R_1)$ *and* $\varphi(R_1, E_1)$ *respectively.*

In fact, $f = (\beta \otimes \alpha) \circ (\beta_1 \otimes \alpha_1)$ is a morphism of the complex $S_1 \otimes_A R_1$ into itself, and one has $(h_1 \circ \alpha_1) \circ f = f$. By X, p. 49, prop. 3 and 3 *bis*, $f$ is a homotopism, hence $H(f) = 1$ and

$$
\psi(S_1, R_1) \circ \psi'(B_1, R_1) = H(\beta \otimes \alpha) \circ H(\beta_1 \otimes \alpha_1) = H(f) = 1;
$$

analogously $\psi'(S_1, R_1) \circ \psi(S_1, R_1) = 1$. One reasons in an analogous manner for the mappings $\varphi$ and $\varphi'$.

#### Example 1 {#alg-x-s6-n1-exa-1 .statement}

Let $a$ be an element of $A$ such that the mapping $\varphi : x \mapsto xa$ of $A$ into itself is injective (*"* $a$ is not a right zero divisor *"*). Using the resolution

$$
0 \to A_s \xrightarrow{\varphi} A_s \to A/Aa \to 0
$$

one sees that for every right $A$-module $M$, one has

$$
\operatorname{Tor}_i^A (M, A/Aa) = 0 \quad \text{for } i > 1
$$

and that the $k$-module $\operatorname{Tor}_1^A (M, A/Aa)$ is isomorphic to $\operatorname{Ker} (a_M)$.

Analogously, for every left $A$-module $M$, one has

$$
\operatorname{Ext}_A^i (A/Aa, M) = 0 \quad \text{for } i > 1
$$

and the $k$-module $\operatorname{Ext}_A^1 (A/Aa, M)$ is isomorphic to $M/aM$.

#### Example 2 {#alg-x-s6-n1-exa-2 .statement}

Suppose that $A$ is an integral domain; let $K$ be the field of fractions of $A$ and $M$ an $A$-module. Using the flat resolution

$$
0 \to A \to K \to K/A \to 0
$$

(X, p. 9, *example* 5), we see that $\operatorname{Tor}_i^A (K/A, M) = 0$ for $i > 1$; moreover, in view of II, p. 116, prop. 26, (ii), the $A$-module $\operatorname{Tor}_1^A (K, A, M)$ is isomorphic to the torsion submodule of $M$.

#### Example 3 {#alg-x-s6-n1-exa-3 .statement}

Suppose that $A$ is a local noetherian ring, let $m$ denote its maximal ideal, and put $\kappa = A/m$. Let $M$ be a finitely generated $A$-module and $P$ a minimal projective resolution of $M$ (X, p. 54). For every $n \geqslant 0$, the $\kappa$-vector spaces $\mathrm{Tor}_n^A(\kappa, M)$ and $\mathrm{Ext}_A^n(M, \kappa)$ are finite-dimensional, of dimension equal to the rank of the free $A$-module $P_n$; in fact, the complexes $\kappa \otimes_A P$ and $\mathrm{Homgr}_A(P, \kappa)$ have zero differential.

### 2. Computation of the mappings $\mathrm{Tor}^A(g, f)$ and $\mathrm{Ext}_A(f, h)$

Let $f : M \to M', h : N' \to N$ be homomorphisms of left $A$-modules, $g : P \to P'$ a homomorphism of right $A$-modules, $a : R \to M, a' : R' \to M'$, $b : S \to P, b' : S' \to P'$, left resolutions of $M, M', P, P'$, respectively, $c : N \to E, c' : N' \to E'$ right resolutions of $N$ and $N'$, $\tilde{f} : R \to R', \tilde{g} : S \to S', \tilde{h} : E' \to E$ morphisms of complexes such that

$$
a' \circ \tilde{f} = f \circ a, \quad b' \circ \tilde{g} = g \circ b, \quad \tilde{h} \circ c' = c \circ h .
$$

#### Proposition 2 {#alg-x-s6-prop-2 .statement}

*The following two diagrams are commutative*:

$$
\begin{array}{ccc}
\mathrm{Tor}^A(P, M) & \xrightarrow{\psi(S, R)} & \mathrm{H}(S \otimes_A R) \\
\mathrm{Tor}^A(g, f) \downarrow & & \downarrow \mathrm{H}(\tilde{g} \otimes \tilde{f}) \\
\mathrm{Tor}^A(P', M') & \xrightarrow{\psi(S', R')} & \mathrm{H}(S' \otimes_A R') ,
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R', E')) & \xrightarrow{\varphi(R', E')} & \mathrm{Ext}_A(M', N') \\
\mathrm{H}(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \downarrow & & \downarrow \mathrm{Ext}_A(f, h) \\
\mathrm{H}(\mathrm{Homgr}_A(R, E)) & \xrightarrow{\varphi(R, E)} & \mathrm{Ext}_A(M, N) .
\end{array}
$$

Let $\alpha : L(M) \to R, \alpha' : L(M') \to R', \gamma : L(P) \to S, \gamma' : L(P') \to S'$ be morphisms of complexes such that

$$
a \circ \alpha = p_M, \quad a' \circ \alpha' = p_{M'}, \quad b \circ \gamma = p_P, \quad b' \circ \gamma' = p_{P'} .
$$

By definition, $\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R)$ is equal to

$$
\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \mathrm{H}(\gamma \otimes \alpha) = \mathrm{H}((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) ,
$$

whereas $\psi(S', R') \circ \mathrm{Tor}^A(g, f)$ is equal to

$$
\mathrm{H}(\gamma' \otimes \alpha') \circ \mathrm{H}(L(g) \otimes L(f)) = \mathrm{H}((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))) .
$$

On the other hand, $\alpha' \circ L(f)$ and $\tilde{f} \circ \alpha$ are two morphisms from $L(M)$ into $R'$ such that $a' \circ (\alpha' \circ L(f)) = p_{M'} \circ L(f) = f \circ p_M = f \circ a \circ \alpha = a' \circ (\tilde{f} \circ \alpha)$. By X, p. 49, prop. 3, $\alpha' \circ L(f)$ and $\tilde{f} \circ \alpha$ are homotopic; analogously $\gamma' \circ L(g)$ and $\tilde{g} \circ \gamma$ are homotopic, and consequently so are $(\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))$ and $(\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)$ by prop. 3 of X, p. 64. Therefore

$$
H(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R) = H((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) = H((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f)))
$$
$$
= \psi(S', R') \circ \mathrm{Tor}^A(g, f) .
$$

One reasons analogously for the second diagram.

#### Remark {#alg-x-s6-n2-rem-1 .statement}

Similarly, consider commutative diagrams of morphisms of complexes

$$
\begin{array}{ccc}
R_1 & \xrightarrow{a_1} & M \\
\tilde{f} \downarrow & & \downarrow f \\
R'_1 & \xrightarrow{a'_1} & M'
\end{array}
$$
$$
\begin{array}{ccc}
S_1 & \xrightarrow{b_1} & P \\
\tilde{g} \downarrow & & g \downarrow \\
S'_1 & \xrightarrow{b'_1} & P'
\end{array}
$$
$$
\begin{array}{ccc}
N' & \xrightarrow{c'_1} & E' \\
h \downarrow & & \tilde{h} \downarrow \\
N & \xrightarrow{c_1} & E_1
\end{array}
$$

where the complexes $R_1, R'_1, S_1, S'_1$ are projective and zero on the right and where the complexes $E_1, E'_1$ are injective and zero on the left. Then

$$
\mathrm{Tor}^A(g, f) \circ \psi'(S_1, R_1) = \psi'(S'_1, R'_1) \circ H(\tilde{g} \otimes \tilde{f})
$$
$$
\varphi'(R_1, E_1) \circ \mathrm{Ext}_A(f, h) = H(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \circ \varphi'(R'_1, E'_1)
$$

as is proved analogously to prop. 2.

### 3. Calculation of the connecting homomorphisms

Let us consider a commutative diagram

(1)
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & R' & \xrightarrow{\tilde{u}} & R & \xrightarrow{\tilde{v}} & R'' & \longrightarrow & 0 \\
& & a' \downarrow & & a \downarrow & & a'' \downarrow & & \\
0 & \longrightarrow & M' & \xrightarrow{u} & M & \xrightarrow{v} & M'' & \longrightarrow & 0
\end{array}
$$

(2)

where the first row (1) is an exact sequence of complexes of left A-modules, the second row (2) is an exact sequence of left A-modules, and the vertical arrows are left resolutions.

#### Proposition 3 {#alg-x-s6-prop-3 .statement}

a) Let $P$ be an A-module, $b : S \to P$ a left resolution of $P$; suppose that the sequence of complexes of k-modules

(3)
$$
0 \to S \otimes_A R' \xrightarrow{1_S \otimes \tilde{u}} S \otimes_A R \xrightarrow{1_S \otimes \tilde{v}} S \otimes_A R'' \to 0
$$

is exact. Then the following diagram is commutative:

$$
\begin{array}{ccc}
\operatorname{Tor}^{A}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}^{A}(P,M')\\
\Big\downarrow\vcenter{\rlap{$\psi(S,R'')$}}&&\Big\downarrow\vcenter{\rlap{$\psi(S,R')$}}\\
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R').
\end{array}
$$

b) Let $N$ be a left $A$-module, $c:N\to E$ a right resolution of $N$; suppose that the sequence of complexes of $k$-modules

(4)

$$
0\longrightarrow \operatorname{Homgr}_A(R'',E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{\imath},1)}
\operatorname{Homgr}_A(R,E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{u},1)}
\operatorname{Homgr}'_A(R',E)\longrightarrow 0
$$

is exact. Then the following diagram is commutative:

$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(R',E))
&\xrightarrow{\delta((4))}
&H(\operatorname{Homgr}_A(R'',E))
\\
\Big\downarrow\vcenter{\rlap{$\varphi(R',E)$}}
&&
\Big\downarrow\vcenter{\rlap{$\varphi(R'',E)$}}
\\
\operatorname{Ext}_A(M',N)
&\xrightarrow{\partial((2),N)}
&\operatorname{Ext}_A(M'',N).
\end{array}
$$

Let us prove a), for example. Let $\beta:L(P)\to S$ be a morphism of complexes such that
$t\circ\beta=p_P$; let us consider the diagram of $k$-complexes

$$
\begin{array}{ccccccccc}
0&\longrightarrow&S\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&S\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&S\otimes_A R''&\longrightarrow&0\\
&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_{R'}$}}&&\\
0&\longrightarrow&L(P)\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&L(P)\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&L(P)\otimes_A R''&\longrightarrow&0\\
&&\Big\downarrow\vcenter{\rlap{$1\otimes a'$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a''$}}&&\\
0&\longrightarrow&L(P)\otimes_A M'&\xrightarrow{1\otimes u}&L(P)\otimes_A M&\xrightarrow{1\otimes v}&L(P)\otimes_A M''&\longrightarrow&0.
\end{array}
$$

This is a commutative diagram with exact rows (by the hypothesis for the first row, and by the fact that $L(P)$ is flat for the other two). We therefore have a commutative diagram (X, p. 31, prop. 2, and X, p. 72, def. 2)

$$
\begin{array}{ccc}
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R')\\
\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}&&\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}\\
H(L(P)\otimes_A R'')&\longrightarrow&H(L(P)\otimes_A R')\\
\Big\downarrow\vcenter{\rlap{$H(1\otimes a'')$}}&&\Big\downarrow\vcenter{\rlap{$H(1\otimes a')$}}\\
H(L(P)\otimes_A M'')&\longrightarrow&H(L(P)\otimes_A M')\\
\Big\uparrow\vcenter{\rlap{$\psi_P(M'')$}}&&\Big\uparrow\vcenter{\rlap{$\psi_P(M')$}}\\
\operatorname{Tor}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}(P,M').
\end{array}
$$

By X, p. 67, prop. 4, H(1 ⊗ a'') and H(1 ⊗ a') are bijective; on the other hand, by definition of the homomorphisms ψ, we have H(β ⊗ 1) ◦ ψ(L(P), R'') = ψ(S, R'') and H(1 ⊗ a'') ◦ ψ(L(P), R'') = ψ(L(P), M'') = ψ_p(M''), therefore

$$
ψ(S, R'') = H(β ⊗ 1) ◦ H(1 ⊗ a'')^{-1} ◦ ψ_p(M'');
$$

analogously, $ψ(S, R') = H(β ⊗ 1) ◦ H(1 ⊗ a')^{-1} ◦ ψ_p(M')$, and the required assertion $\partial((3)) ◦ ψ(S, R'') = ψ(S, R') ◦ \partial(P, (2))$ follows from the commutativity of the preceding diagram.

#### Remark 1 {#alg-x-s6-n3-rem-1 .statement}

Using the commutation isomorphisms, one deduces from a) the analogous statement obtained by exchanging the roles of the two arguments of the tensor product.

#### Remark 2 {#alg-x-s6-n3-rem-2 .statement}

With the notation of a), suppose either that S is flat, or that R, R', R'' are flat; then on the one hand sequence (3) is exact (X, p. 72, cor. 2) and one may apply prop. 3; on the other hand $ψ(S, R')$ is bijective (th. 1), therefore

$$
\partial(P, (2)) = ψ(S, R')^{-1} ◦ \partial((3)) ◦ ψ(S, R'').
$$

#### Remark 3 {#alg-x-s6-n3-rem-3 .statement}

With the notation of b), suppose either that E is injective, or that R, R', R'' are projective; then on the one hand sequence (4) is exact (X, p. 83, prop. 2) and one may apply prop. 3; on the other hand, $φ(R', E)$ is bijective (th. 1) ; therefore

$$
δ((2), N) = φ(R'', E) ◦ \partial((4)) ◦ φ(R', E)^{-1}.
$$

Let us now consider a commutative diagram

(5)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & N' & \xrightarrow{r} & N & \xrightarrow{s} & N'' & \rightarrow & 0 \\
   &           & c'   &         &   &         & c''   &         &
\end{array}
$$

(6)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & E' & \xrightarrow{\tilde{r}} & E & \xrightarrow{\tilde{s}} & E'' & \rightarrow & 0
\end{array}
$$

whose first row (5) is an exact sequence of left A-modules, the second row (6) an exact sequence of complexes of left A-modules, and in which the vertical arrows are right resolutions. Reasoning as in Prop. 3, one proves the following proposition:

#### Proposition 4 {#alg-x-s6-prop-4 .statement}

Let M be a left A-module, $a : R \to M$ a left resolution of M such that the sequence

(7)
$$
0 \rightarrow \mathrm{Homgr}_A(R, E') \xrightarrow{\mathrm{Homgr}(\tilde{s}, 1)} \mathrm{Homgr}_A(R, E) \xrightarrow{\mathrm{Homgr}(\tilde{r}, 1)} \mathrm{Homgr}_A(R, E'') \rightarrow 0
$$

is exact. Then the following diagram is commutative.

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R, E'')) & \xrightarrow{\partial((7))} & \mathrm{H}(\mathrm{Homgr}_A(R, E')) \\
\varphi(R, E'') \downarrow & & \downarrow \varphi(R, E') \\
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, (5))} & \mathrm{Ext}_A(M, N')
\end{array}
$$

#### Remark 4 {#alg-x-s6-n3-rem-4 .statement}

If R is projective or if E, E', E'' are injective, the sequence (7) is exact ($\lambda$, p. 83, Prop. 2); moreover, $\varphi(R, E'')$ is bijective (Th. 1); hence

$$
\delta(M, (5)) = \varphi(R, E') \circ \partial((7)) \circ \varphi(R, E'')^{-1}.
$$

#### Remark 5 {#alg-x-s6-n3-rem-5 .statement}

We leave it to the reader to state and prove the propositions analogous to Props. 3 and 4 and concerning the homomorphisms $\psi_1$ and $\varphi_1$.

### 4. Finiteness of extension and torsion modules

Let M be a left A-module, I a filtered preordered set, $(N_i, u_{ji})$ an inductive system of left A-modules relative to I, $N = \lim N_i$ its inductive limit, $u_i : N_i \to N,\ i \in I$, the canonical mapping. Then $(\mathrm{Ext}_A(M, N_i), \mathrm{Ext}_A(l_M, u_{ji}))$ is an inductive system of $k$-modules and $(\mathrm{Ext}_A(l_M, u_i))$ an inductive system of mappings, whose inductive limit is a homomorphism of graded $k$-modules, called *canonical*

$$
\lim_{i \in I} \mathrm{Ext}_A(M, N_i) \to \mathrm{Ext}_A(M, \lim_{i \in I} N_i).
$$

#### Proposition 5 {#alg-x-s6-prop-5 .statement}

*If A is left noetherian and if M is a finitely generated A-module, the canonical homomorphism (8) is bijective.*

For let (X, p. 53, Prop. 6) $p : L \to M$ be a free resolution of M such that $L_n$ is of finite type for each $n$. The canonical morphism of $k$-complexes

$$
u : \lim \mathrm{Homgr}_A(L, N_i) \to \mathrm{Homgr}_A(L, \lim N_i)
$$

is bijective, hence so also is the homomorphism

$$
\lim \mathrm{H}(\mathrm{Homgr}_A(L, N_i)) \to \mathrm{H}(\mathrm{Homgr}_A(L, \lim N_i))
$$

deduced from the homomorphisms $\mathrm{H}(\mathrm{Homgr}(l, u_i))$ (X, p. 28, Prop. 1). One then concludes by Prop. 2 (X, p. 103) and Th. 1 (X, p. 100).

#### Proposition 6 {#alg-x-s6-prop-6 .statement}

*Let B be a ring and N an (A, B)-bimodule, which is a noetherian B-module (resp. of finite length).

a) Suppose A right noetherian and let M be a finitely generated right A-module. Then the B-modules (X, p. 81) $\mathrm{Tor}_n^A(M, N)$ are noetherian (resp. of finite length).

b) Suppose A left noetherian and let M be a finitely generated left A-module. Then the B-modules (X, p. 98) $\mathrm{Ext}_A^n(M, N)$ are noetherian (resp. of finite length).

Choose a free resolution $p : L \to M$ such that each of the A-modules $L_n$ is of finite type (X, p. 53, Prop. 6), and let C be the complex of B-modules $L \otimes_A N$ in case $a$, $\mathrm{Homgr}_A(L, N)$ in case $b$. Each of the B-modules $C_n$ is isomorphic to a product of a finite number of copies of N, hence is noetherian (resp. of finite length); the same is therefore true of the modules $\mathrm{H}_n(C)$. But, by X, p. 100, Th. 1, these are isomorphic to the $\mathrm{Tor}_n^A(M, N)$ in case $a$, to the $\mathrm{Ext}_A^{-n}(M, N)$ in case $b$.

#### Corollary {#alg-x-s6-n4-cor-1 .statement}

Let $\rho : A \to B$ be a homomorphism of noetherian commutative rings, $M$ a finitely generated $A$-module, $N$ a $B$-module. If $N$ is a finitely generated $B$-module (resp. of finite length), the same is true of the $B$-modules $\operatorname{Tor}^{A}_{n}(M,N)$ and $\operatorname{Ext}^{n}_{A}(M,N)$.

### 5. The homomorphisms $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ and $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$

Let $B$ be a ring, $N$ a $(B,A)$-bimodule, $M$ a left $B$-module, $P$ a
right $B$-module, $Q$ a left $A$-module.
By X, p. 62, one has a homomorphism

$$
\gamma_{1} : H(L(P) \otimes_{B} N) \otimes_{A} Q \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,;
$$

moreover (X, p. 69, Prop. 5), one has isomorphisms

$$
\psi_{1}(N) : \operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to H(L(P) \otimes_{B} N) \otimes_{A} Q \,,
$$

$$
\psi_{1}(N \otimes_{A} Q) : \operatorname{Tor}^{B}(P,N \otimes_{A} Q) \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,.
$$

The graded homomorphism of degree 0, called *canonical*

(9)

$$
\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)
$$

is defined as the composite $\psi_{P}(N \otimes_{A} Q)^{-1} \circ \gamma_{1} \circ (\psi_{P}(N) \otimes 1_{Q})$.

Analogously, from the canonical morphism of complexes

$$
\alpha : \operatorname{Homgr}_{B}(L(M),N) \otimes_{A} Q \to \operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)
$$

one deduces a homomorphism $H(\alpha)$; one has the canonical homomorphism (X, p. 62)

$$
\gamma_{2} : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \,,
$$

and the isomorphisms (X, p. 88, prop. 5)

$$
\varphi_{M}(N) : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N) \otimes_{A} Q \,,
$$

$$
\varphi_{M}(N \otimes_{A} Q) : H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q) \,.
$$

The graded homomorphism of degree 0, called *canonical*

(10)

$$
\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)
$$

is defined as the composite

$$
\varphi_{M}(N \otimes_{A} Q) \circ H(\alpha) \circ (\varphi_{M}(N) \otimes 1_{Q})^{-1} \,.
$$

#### Proposition 7 {#alg-x-s6-prop-7 .statement}

a) If the $A$-module $Q$ is flat, homomorphism (9) is bijective.
b) If the $A$-module $Q$ is finitely generated projective, homomorphism (10) is bijective.

c) If the $A$-module $Q$ is flat, the ring $B$ noetherian and the $B$-module $M$ finitely generated, homomorphism (10) is bijective.

a) If $Q$ is flat, $\gamma_1$ is bijective ($X$, p. 66, cor. 2).

b) If $Q$ is finitely generated projective, it is flat, hence $\gamma_2$ is bijective, and moreover $\alpha$ is bijective (II, p. 75, prop. 2, a)).

c) Under the hypotheses of c), $\gamma_2$ is bijective since $Q$ is flat. Moreover ($X$, p. 53, prop. 6), there exists a resolution $L$ of $M$ such that each $L_n$ is finitely generated free; let $u : L(M) \to L$ be a homotopism ($X$, p. 49, cor. to prop. 3); in the commutative diagram,

$$
\begin{array}{ccc}
\mathrm{Homgr}_B(L(M), N) \otimes_A Q & \xrightarrow{\alpha} & \mathrm{Homgr}_B(L(M), N \otimes_A Q) \\
\uparrow & & \uparrow \\
\mathrm{Homgr}_B(L, N) \otimes_A Q & \xrightarrow{\bar{\alpha}} & \mathrm{Homgr}_B(L, N \otimes_A Q).
\end{array}
$$

the vertical arrows deduced from $u$ are homotopisms ($X$, p. 64, prop. 3 and p. 83, prop. 3) and $\bar{\alpha}$ is bijective (II, p. 75, prop. 2 (ii)); hence $H(\alpha)$ is bijective, and homomorphism (10) is bijective.

### 6. The homomorphisms $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ and $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$

Let us retain the preceding notations, and suppose that $N$ is flat over $A$. Then the morphism $N \otimes_A L(Q) \xrightarrow{1 \otimes p_Q} N \otimes_A Q$ is a homologism ($X$, p. 67, prop. 4), whence homomorphisms

$$
\psi(P, N \otimes_A L(Q)) : \mathrm{Tor}^B(P, N \otimes_A Q) \to H(P \otimes_B N \otimes_A L(Q))
$$
$$
\varphi(N \otimes_A L(Q), M) : H(\mathrm{Homgr}_B(N \otimes_A L(Q), M)) \to \mathrm{Ext}_B(N \otimes_A Q, M).
$$

Using then the *isomorphisms*

$$
\overline{\psi}_Q(P \otimes_B N) : \mathrm{Tor}^A(P \otimes_B N, Q) \to H(P \otimes_B N \otimes_A L(Q)),
$$
$$
\beta : \mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M)) \to \mathrm{Homgr}_B(N \otimes_A L(Q), M),
$$
$$
\varphi_Q(\mathrm{Hom}_B(N, M)) : H(\mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M))) \to \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)),
$$

one deduces from them graded homomorphisms of degree 0 called *canonical*:

(11) $$ \mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q) $$
(12) $$ \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M). $$

#### Proposition 8 {#alg-x-s6-prop-8 .statement}

*a)* If $N$ is flat over $A$ and over $B$, homomorphism (11) is bijective.

*b)* If $N$ is flat over $A$ and projective over $B$, homomorphism (12) is bijective.

Indeed $N \otimes_A L(Q)$ is isomorphic to a direct sum of copies of $N$, hence is a flat (resp. projective) $B$-module when the $B$-module $N$ is flat (resp. projective); one then applies Theorem 1 (X, p. 100).

### 7. The homomorphisms $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ and $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$

In this No., we suppose that $A$ is *commutative*; given a ring homomorphism $\rho : A \to B$ such that $\rho(A)$ is contained in the center of $B$ and two $A$-modules $E$ and $F$. There is a canonical isomorphism of complexes of $A$-modules

$$
u : B \otimes_A (L(E) \otimes_A L(F)) \to (L(E) \otimes_A B) \otimes_B (B \otimes_A L(F));
$$

on the other hand, since $L(E) \otimes_A B$ and $B \otimes_A L(F)$ are *free* $B$-complexes, there is a canonical homomorphism of graded $A$-modules (X, p. 102)

$$
\psi'(L(E) \otimes_A B, B \otimes_A L(F)) : H((L(E) \otimes_A B) \otimes_B (B \otimes_A L(F)))
$$
$$
\to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

finally, there is a homomorphism (X, p. 62)

$$
\gamma : B \otimes_A \mathrm{Tor}^A(E, F) \to H(B \otimes_A L(E) \otimes_A L(F)).
$$

The *canonical* homomorphism of graded $B$-modules

(13)
$$
B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

is defined as the composite $\psi'(L(E) \otimes_A B, B \otimes_A L(F)) \circ H(u) \circ \gamma$.

#### Proposition 9 {#alg-x-s6-prop-9 .statement}

*If $B$ is flat over $A$, homomorphism (13) is bijective.*
Indeed $\psi'(L(E) \otimes_A B, B \otimes_A L(F))$ is bijective (X, p. 102, prop. 1) and $\gamma$ is bijective (X, p. 66, cor. 2).

Suppose $B$ *flat* over $A$. Substituting $E$ for $Q$, $B$ for $N$ and $B \otimes_A F$ for $M$ in homomorphism (12), we obtain a homomorphism

$$
\mathrm{Ext}_A(E, B \otimes_A F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)
$$

which is bijective by Proposition 8. Substituting $E$ for $M$, $F$ for $N$, $A$ for $B$, $B$ for $Q$, in homomorphism (10), and interchanging the factors in the tensor products, we obtain a homomorphism of $B$-modules

$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_A(E, B \otimes_A F),
$$

whence by composition a homomorphism called *canonical*

(14)
$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F).
$$

#### Proposition 10 {#alg-x-s6-prop-10 .statement}

Homomorphism (14) is bijective in the following cases:
a) B is a finitely generated projective A-module;
b) B is a flat A-module, A is noetherian, and E is a finitely generated A-module.
This follows from Proposition 7 (X, p. 108).

### 8. Application: homology and cohomology of groups

Let G be a group, $\mathbf{Z}^{(G)}$ its algebra over $\mathbf{Z}$ (III, p. 19). Recall (cf. III, p. 20, example) that if M is a commutative group, it comes to the same thing to give an action of G on M (that is to say a homomorphism $\tau : G \to \mathrm{Aut}(M)$), or a structure of left $\mathbf{Z}^{(G)}$-module on the additive group M. In particular, we shall consider the group $\mathbf{Z}$ as a left $\mathbf{Z}^{(G)}$-module by endowing it with the trivial action.

#### Definition 1 {#alg-x-s6-def-1 .statement}

Let M be a left $\mathbf{Z}^{(G)}$-module (resp. right), n an integer $\geqslant 0$. The group $\mathrm{Ext}_{\mathbf{Z}^{(G)}}^n(\mathbf{Z}, M)$ (resp. $\mathrm{Tor}_n^{\mathbf{Z}^{(G)}}(M, \mathbf{Z})$) is denoted by $H^n(G, M)$ (resp. $H_n(G, M)$) and is called the nth cohomology group (resp. homology group) of G with coefficients in M.

The standard resolution (X, p. 58) $B(\mathbf{Z}^{(G)}, \mathbf{Z})$ is a free resolution of the $\mathbf{Z}^{(G)}$-module $\mathbf{Z}$; it follows that the groups $H^n(G, M)$ (resp. $H_n(G, M)$) identify with the homology groups of the complex:

$$
\mathrm{Hom}_{\mathbf{Z}^{(G)}}(B(\mathbf{Z}^{(G)}, \mathbf{Z}), M) \quad (\text{resp. } M \otimes_{\mathbf{Z}^{(G)}} B(\mathbf{Z}^{(G)}, \mathbf{Z})) .
$$

Using the canonical isomorphism of $(\mathbf{Z}^{(G)})^{\otimes n}$ onto $\mathbf{Z}^{(G^n)}$ (III, p. 36) and the properties of extension of scalars (II, p. 82), one concludes that $H^n(G, M)$ is canonically isomorphic to the homology group of ascending degree $n$ of the complex $C(G, M)$ defined as follows: $C^n(G, M) = 0$ for $n < 0$; for $n \geqslant 0$, $C^n(G, M)$ is the $\mathbf{Z}$-module of mappings of $G^n$ into M; for $n \geqslant 0$, the differential $d^n : C^n(G, M) \to C^{n+1}(G, M)$ is given by

$$
(d^n f)(g_0, ..., g_n) = g_0 \cdot f(g_1, ..., g_n) + \sum_{i=0}^{n-1} (-1)^{i+1} f(g_0, ..., g_i g_{i+1}, ..., g_n)
$$
$$
+ (-1)^{n+1} f(g_0, ..., g_{n-1})
$$

for any $f$ in $C^n(G, M)$ and $g_0, ..., g_n$ in G.

Analogously, $H_n(G, M)$ identifies with the homology group of degree $n$ of the complex $C'(G, M)$, where $C'_n(G, M) = M \otimes_{\mathbf{Z}} \mathbf{Z}^{(G^n)}$ for $n \geqslant 0$, $C'_n(G, M) = 0$ for $n < 0$, the differential $d_n : C'_n(G, M) \to C'_{n-1}(G, M)$ being defined by:

$$
d_n(m \otimes e_{g_1, ..., g_n}) = m \cdot g_1 \otimes e_{g_2, ..., g_n} + \sum_{i=1}^{n-1} (-1)^i m \otimes e_{g_1, ..., g_i g_{i+1}, ..., g_n}
$$
$$
+ (-1)^n m \otimes e_{g_1, ..., g_{n-1}}
$$

for any $n \geqslant 1$, $m$ in M and $g_1, ..., g_n$ in G.

#### Example 1 {#alg-x-s6-n8-exa-1 .statement}

It follows directly from the definition that $H^0(G, M)$ is isomorphic to the submodule of elements of $M$ invariant under the action of $G$, and $H_0(G, M)$ to the quotient module of $M$ by the submodule generated by the elements $m.g-m$ for $m\in M$, $g\in G$.

#### Example 2 {#alg-x-s6-n8-exa-2 .statement}

It follows from the preceding that $H^1(G, M)$ is isomorphic to the $\mathbf{Z}$-module $Z^1(G, M)/B^1(G, M)$, where $Z^1(G, M)$ is the $\mathbf{Z}$-module of mappings $f$ of $G$ into $M$ satisfying:

$$
f(g_1,g_2)=g_1.f(g_2)+f(g_1)\quad\text{for all }g_1,g_2\text{ in }G,
$$

and $B^1(G, M)$ is the sub-$\mathbf{Z}$-module of $Z^1(G, M)$ consisting of the $f$ for which there exists an element $m$ of $M$ such that:

$$
f(g)=g.m-m\quad\text{for every }g\in G.
$$

One sometimes says that $Z^1(G, M)$ is the $\mathbf{Z}$-module of crossed homomorphisms of $G$ into $M$, and $B^1(G, M)$ the submodule of principal crossed homomorphisms.

Let us denote by $\iota:G\to \operatorname{Aut}(M)$ the homomorphism deduced from the action of $G$; consider the external semidirect product $M\times_{\iota}G$ and the extension $\xi_{\iota}:M\times_{\iota}G\to G$ (I, p. 64). Let $e:G\to M\times_{\iota}G$ be a mapping such that $\rho\circ e=1_G$; one has $e=(f,1_G)$, where $f\in C^1(G,M)$. In order that $e$ be a homomorphism (that is to say, a section of the extension $\xi_{\iota}$), it is necessary and sufficient that $f\in Z^1(G,M)$. In order that two sections of $\xi_{\iota}$ be conjugate by an element of $i(M)$, it is necessary and sufficient that the corresponding crossed homomorphisms have the same class in $H^1(G,M)$.

When $G$ operates trivially on $M$, one has $B^1(G,M)=0$ and $H^1(G,M)$ is isomorphic to the $\mathbf{Z}$-module of group homomorphisms of $G$ into $M$.

#### Example 3 {#alg-x-s6-n8-exa-3 .statement}

Analogously $H^2(G,M)$ is isomorphic to the $\mathbf{Z}$-module $Z^2(G,M)/B^2(G,M)$, where $Z^2(G,M)$ is the $\mathbf{Z}$-module of mappings $f$ of $G\times G$ into $M$, satisfying:

$$
g_1.f(g_2,g_3)-f(g_1g_2,g_3)+f(g_1,g_2g_3)-f(g_1,g_2)=0
$$

whatever $g_1,g_2,g_3$ in $G$ may be, and $B^2(G,M)$ is the sub-$\mathbf{Z}$-module of $Z^2(G,M)$ consisting of the $f$ for which there exists a mapping $h$ of $G$ into $M$ such that:

$$
f(g_1,g_2)=g_1.h(g_2)-h(g_1g_2)+h(g_1)
$$

whatever $g_1,g_2$ in $G$ may be.

Thus one recovers the definition of the group $H^2(G,M)$ given in VIII, App. II; in particular there exists a canonical isomorphism of $H^2(G,M)$ onto the group of extension classes of $G$ by $M$ (loc. cit.).

#### Example 4 {#alg-x-s6-n8-exa-4 .statement}

Let $M$ be a $\mathbf{Z}$-module, considered as a right $\mathbf{Z}^{(G)}$-module by making $G$ operate trivially. The group $H_1(G,M)$ is isomorphic to the quotient of $M\otimes_{\mathbf{Z}}\mathbf{Z}^{(G)}$ by the sub-$\mathbf{Z}$-module generated by the elements $m\otimes(e_{g_1g_2}-e_{g_1}-e_{g_2})$ for $m$ in $M$, $g_1,g_2$ in $G$; it follows easily that $H_1(G,M)$ is isomorphic to $M\otimes_{\mathbf{Z}}(G/(G,G))$.

Let us denote by $\sigma$ the anti-automorphism of $\mathbf{Z}^{(G)}$ defined by $\sigma(e_g) = e_{g^{-1}}$ for $g \in G$. Every left $\mathbf{Z}^{(G)}$-module may be considered as a right $\mathbf{Z}^{(G)}$-module by means of $\sigma$, and conversely. This makes it possible, for example, to define the groups $H_q(G, M)$ for a left $\mathbf{Z}^{(G)}$-module $M$, by setting $H_q(G, M) = H_q(G, \sigma_*(M)) = \mathrm{Tor}_q^{\mathbf{Z}^{(G)}}(\mathbf{Z}, M)$.

#### Lemma 1 {#alg-x-s6-lem-1 .statement}

*Let $M$ be a $\mathbf{Z}$-module; let $M^G$ denote the group $\mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, M)$ endowed with its natural structure of left $\mathbf{Z}^{(G)}$-module. Then:*

$$
H^i(G, M^G) = 0 \quad \text{for} \quad i \geqslant 1 .
$$

It follows indeed from Prop. 8, b) (X, p. 109), applied with $A = N = \mathbf{Z}^{(G)}$ and $B = Q = \mathbf{Z}$, that one has a canonical isomorphism:

$$
\mathrm{Ext}_{\mathbf{Z}^{(G)}}(\mathbf{Z}, M^G) \to \mathrm{Ext}_{\mathbf{Z}}(\mathbf{Z}, M)
$$

whence the lemma.

#### Proposition 11 {#alg-x-s6-prop-11 .statement}

*Let $L$ be a finite-degree galois extension of a commutative field $K$, with galois group $G$.
a) *One has* $H^i(G, L) = 0$ *for* $i \geqslant 1$.
b) *One has* $H^1(G, L^*) = 0$.
c) *The group* $H^2(G, L^*)$ *is canonically isomorphic to the group* $\mathrm{Br}(K, L)$ *(VIII, § 13)*.

The normal basis theorem (V, §10, No. 9, Theorem 6) shows that $L$ is isomorphic as a $\mathbf{Z}^{(G)}$-module to $K^G = \mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, K)$; assertion a) then follows from Lemma 1. In view of Example 2, assertion b) follows from V, §10, No. 5, Corollary 1 to Proposition 9: finally, assertion c) was proved in VIII, §13.

## EXERCISES {#alg-x-s6-exercises}

See the [exercises for § 6](exercises/s6/).
