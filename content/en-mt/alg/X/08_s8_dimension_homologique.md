---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 8
section_title: Dimension homologique
lang: en
source: alg-x-fr
book_pages: A X.134-A X.146, A X.202-A X.206
pdf_pages: 0140-0152, 0208-0212
extraction: ocr
subsections:
    - "no": 1
      title: Dimension projective d’un module
      page: 134
      pdf_page: 140
    - "no": 2
      title: L’homomorphisme $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$
      page: 137
      pdf_page: 143
    - "no": 3
      title: Dimension homologique d’un anneau
      page: 138
      pdf_page: 144
    - "no": 4
      title: Anneaux de dimension homologique 0
      page: 140
      pdf_page: 146
    - "no": 5
      title: Anneaux de dimension homologique 1
      page: 140
      pdf_page: 146
    - "no": 6
      title: Dimension homologique des anneaux de polynômes
      page: 141
      pdf_page: 147
    - "no": 7
      title: Dimension homologique des modules gradués
      page: 143
      pdf_page: 149
statements: 34
exercises: 22
content_sha256: a43e5824a369fc7cb54f0cf634d6c6c6ca549a1893ead639ca49ac83f5b3a298
translated_from: content/fr/alg/X/08_s8_dimension_homologique.md
source_lang: fr
translation_method: machine
source_content_sha256: 01423d7f9d05c6000bce1884bf08ce49ac1e4be4045d9ae6bb8edef4dbad7463
translation_model: laguna-s-2.1-free, hy3-free
translation_run: translate-en-mt-e117ae35
glossary_version: 34
glossary_terms_sha256: 44c97967687f9cad418a5d554b6a20aa8f0ff3376c394b7238ace34727c7514d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 8. HOMOLOGICAL DIMENSION

In this section, we adopt the conventions of § 5.

### 1. Projective Dimension of a Module

#### Definition 1 {#alg-x-s8-def-1 .statement}

*Let $M$ be an $A$-module. The projective dimension of $M$, denoted by $\mathrm{dp}_A(M)$, is the greatest lower bound in $\overline{\mathbf{Z}}$ of the lengths of projective resolutions of $M$* (X, p. 48).

We thus have $\mathrm{dp}_A(0) = -\infty$, $\mathrm{dp}_A(M) \geq 0$ if $M \neq 0$. For $M$ to be projective, it is necessary and sufficient that $\mathrm{dp}_A(M) \leq 0$.

#### Lemma 1 {#alg-x-s8-lem-1 .statement}

*If $\mathrm{dp}_A(M) < n < +\infty$, then $\mathrm{Ext}_A^n(M, N) = 0$ for every $A$-module $N$ and $\mathrm{Tor}_n^A(P, M) = 0$ for every righthand $A$-module $P$.
This follows immediately from the fact that $M$ has a projective resolution of length $< n$ and from X, p. 100, Theorem 1.*

#### Proposition 1 {#alg-x-s8-prop-1 .statement}

*Let $M$ be an $A$-module and $n$ an integer $\geq 0$. The following conditions are equivalent* :
(i) $\mathrm{dp}_A(M) \leq n$ (*i.e.* (def. 1), $M$ has a projective resolution of length $\leq n$);
(ii) $\mathrm{Ext}_A^r(M, N) = 0$ for every $A$-module $N$ and every integer $r > n$;
(iii) $\mathrm{Ext}_A^{n+1}(M, N) = 0$ for every $A$-module $N$;
(iv) *for every exact sequence*
$$
0 \to K \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$
*où les $P_i$ sont projectifs, $K$ is projective*.

(i) ⇒ (ii): this follows from Lemma 1.
(ii) ⇒ (iii): this is trivial.
(iii) ⇒ (iv): in the situation of (iv), for every $A$-module $N$ there is an isomorphism of $\mathrm{Ext}_A^1(K, N)$ onto $\mathrm{Ext}_A^{n+1}(M, N)$ (X, p. 128, Corollary 4); if (iii) holds, then
$$
\mathrm{Ext}_A^1(K, N) = 0
$$
for every $N$ and $K$ is projective (X, p. 93, Proposition 10).
(iv) ⇒ (i): consider the exact sequence (X, p. 50)
$$
0 \to Z_{n-1}(M) \to L_{n-1}(M) \to \ldots \to L_0(M) \to M \to 0 .
$$
If (iv) holds, then $Z_{n-1}(M)$ is projective and $M$ has a projective resolution of length $\leq n$.

#### Corollary 1 {#alg-x-s8-prop-1-cor-1 .statement}

Let $(M_i)_{i \in E}$ be a family of $A$-modules. We have
$$
\mathrm{dp}_A \left( \bigoplus_{i \in E} M_i \right) = \sup_{i \in E} \mathrm{dp}_A(M_i) .
$$
This follows from the equivalence of conditions (i) and (iii) of Proposition 1 and Proposition 7 of X, p. 89.

In the following statement, we agree that $\pm \infty + 1 = \pm \infty - 1 = \pm \infty$.

#### Corollary 2 {#alg-x-s8-prop-1-cor-2 .statement}

Let
$$
0 \to M' \to M \to M'' \to 0
$$
be an exact sequence of $A$-modules.

a) We have
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$
Equality occurs as soon as $\mathrm{dp}_A(M'') \neq \mathrm{dp}_A(M') + 1$.

b) We have
$$
\mathrm{dp}_A(M'') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M') + 1) .
$$
Equality occurs as soon as $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M')$.

c) We have
$$
\mathrm{dp}_A(M') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M'') - 1) .
$$
Equality occurs as soon as $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M'')$.

Let us prove for example a), the proofs of b) and c) being analogous.
If N is an arbitrary a-module and n an integer $\geq 0$, we have an exact sequence
$$
\mathrm{Ext}_A^{n+1}(M'', N) \to \mathrm{Ext}_A^{n+1}(M, N) \to \mathrm{Ext}_A^{n+1}(M', N) \to \mathrm{Ext}_A^{n+2}(M'', N)
$$
$$
\to \mathrm{Ext}_A^{n+2}(M, N) .
$$
If $\mathrm{dp}_A(M'), \mathrm{dp}_A(M'') \leq n$, then $\mathrm{Ext}_A^{n+1}(M', N) = 0$ and $\mathrm{Ext}_A^{n+1}(M'', N) = 0$ (prop. 1), hence $\mathrm{Ext}_A^{n+1}(M, N) = 0$ and $\mathrm{dp}_A(M) \leq n$ (prop. 1), so that
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$

If $\mathrm{dp}_A(M)<\sup\bigl(\mathrm{dp}_A(M'),\mathrm{dp}_A(M'')\bigr)$, then necessarily $\mathrm{dp}_A(M)<+\infty$. For every $n>\mathrm{dp}_A(M)$ and every a-module N, we have

$$
\operatorname{Ext}_A^{n+1}(M',N)\ne0\Longleftrightarrow\operatorname{Ext}_A^{n+2}(M'',N)\ne0,
$$

by the preceding exact sequence; by prop. 1, this immediately implies $\mathrm{dp}_A(M'')=\mathrm{dp}_A(M')+1$, since one of the quantities $\mathrm{dp}_A(M')$, $\mathrm{dp}_A(M'')$ is $>\mathrm{dp}_A(M)$.

**Example.** — Let $a$ be an element of A which is neither invertible nor a right zero divisor.
Then $\mathrm{dp}_A(A/Aa)=1$.

Indeed, by the exact sequence $0\longrightarrow A_s\xrightarrow{\varphi} A_s\longrightarrow A/Aa\longrightarrow0$, where $\varphi(x)=xa$, we have $\mathrm{dp}_A(A/Aa)\leq1$. If $\mathrm{dp}_A(A/Aa)<1$, then $A/Aa$ is projective, and there exists an a-linear mapping $\psi:A_s\longrightarrow A_s$ such that $\psi\circ\varphi=\mathrm{Id}$; this implies

$$
1=\psi(\varphi(1))=\psi(a)=a.\psi(1)
$$

and $a$ is invertible.

#### Proposition 2 {#alg-x-s8-prop-2 .statement}

Assume A left noetherian. Let M be a finitely generated a-module and n an integer $\geq0$. The following conditions are equivalent:

(i) $\mathrm{dp}_A(M)\leq n$.

(i bis) M possesses a projective resolution P of length $\leq n$ such that $P_i$ is a finitely generated a-module for each $i$.

(ii) $\operatorname{Ext}_A^r(M,N)=0$ for every finitely generated a-module N and every integer $r>n$.

(iii) $\operatorname{Ext}_A^{n+1}(M,N)=0$ for every finitely generated a-module N.

(iv) $\operatorname{Tor}^A_r(P,M)=0$ for every right a-module P and every $r>n$.

(v) $\operatorname{Tor}^A_{n+1}(A/a,M)=0$ for every finitely generated right ideal $a$ of A.

(i bis) $\Rightarrow$ (i) : this is trivial.

(i) $\Rightarrow$ (ii) : this follows from Lemma 1.

(ii) $\Rightarrow$ (iii) : this is trivial.

(iii) $\Rightarrow$ (i) : by (iii) and X, p. 107, prop. 5, we have $\operatorname{Ext}_A^{n+1}(M,N)=0$ for every a-module N, whence (i) by prop. 1.

(i) $\Rightarrow$ (iv) : this follows from Lemma 1.

(iv) $\Rightarrow$ (v) : this is trivial.

(v) $\Rightarrow$ (i bis) : let (L,d) be a free resolution of M such that $L_r$ is finitely generated for all $r$ (X, p. 53, prop. 6). Set $K=\mathrm{Z}_{n-1}(L)$; then K is finitely generated as a submodule of $L_{n-1}$ and we have an exact sequence

$$
0\longrightarrow K\longrightarrow L_{n-1}\longrightarrow L_{n-2}\longrightarrow\cdots\longrightarrow L_1\longrightarrow L_0\longrightarrow M\longrightarrow0.
\tag{1}
$$

By (v) and X, p. 131, cor. 3, we have $\operatorname{Tor}^A_1(A/a,K)=0$ for every finitely generated right ideal $a$ of A. By th. 2 of X, p. 74, the a-module K is flat; since it is finitely generated, hence of finite presentation (X, p. 10, prop. 5), it is projective (X, p. 13, cor.), so (1) is a projective resolution of M.

#### Corollary {#alg-x-s8-n1-cor-1 .statement}

Suppose $A$ left noetherian and let $\mathcal{C}_0$ (resp. $\mathcal{C}$) be the set of classes of $A$-modules projective of finite type (resp. of $A$-modules of finite projective dimension and of finite type). Then the homomorphism of Grothendieck groups $K(\mathcal{C}_0) \to K(\mathcal{C})$ is bijective.

This follows from X, p. 58, th. 1 (note that $\mathcal{C}_0$ and $\mathcal{C}$ are left exact by cor. 2).

### 2. The homomorphism $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$

Let $M$ a left $A$-module, $P$ a right $A$-module, $n$ an integer $\geqslant 0$. The mapping $k$-bilinéaire (X, p. 129)

$$
c_{P;M,A_s} : \operatorname{Ext}_A^n(M, A) \times \operatorname{Tor}_n^A(P, M) \to P \otimes_A A
$$

corresponds to a mapping $k$-linéaire

(2)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_k(\operatorname{Ext}_A^n(M, A), P);
$$

moreover, if one equips $\operatorname{Ext}_A^n(M, A)$ with the structure of right $A$-module coming from the bimodule structure of $A$, the image of (2) consists of mappings $A$-linéaires, as is immediately verified; this yields a $k$-homomorphisme, called canonical

(3)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P).
$$

#### Proposition 3 {#alg-x-s8-prop-3 .statement}

a) If $\mathrm{dp}_A(M) \leqslant n$, the canonical homomorphism (3) is injective.
b) If $\mathrm{dp}_A(M) \leqslant n$, if $A$ is left noetherian and if $M$ is of finite type, the canonical homomorphism (3) is bijective.

We argue by induction on $n$. If $n = 0$, $M$ is projective, the homomorphism (3) reduces to the canonical homomorphism $P \otimes_A M \to \operatorname{Hom}_A(M^*, P)$ of II, p. 77, and the proposition follows from loc. cit., corollary. If $n > 0$, let

(4)
$$
0 \to N \to L \to M \to 0
$$

be an exact sequence of $A$-modules where $L$ is free (and of finite type in case b); then $\mathrm{dp}_A(N) \leqslant n - 1$ (X, p. 135, cor. 2, c)) and $N$ is of finite type in case b.

Let $\theta \in \operatorname{Ext}_A^1(M, N)$ be the class associated with the exact sequence (4) (X, p. 117, déf. 1). Denote
$$
u_n : \operatorname{Ext}_A^{n-1}(N, A) \to \operatorname{Ext}_A^n(M, A) \qquad v_n : \operatorname{Tor}_n^A(P, M) \to \operatorname{Tor}_{n-1}^A(P, N)
$$
the mappings defined by $u_n(\alpha) = \alpha \circ \theta$ and $v_n(\beta) = \theta \circ \beta$. We have
$$
(\alpha \circ \theta) \circ \beta = \alpha \circ (\theta \circ \beta)
$$

for all $\alpha\in\operatorname{Ext}_A^{n-1}(N,A)$, $\beta\in\operatorname{Tor}_n^A(P,M)$ (X, p. 129, prop. 6), so that the diagram

$$
\begin{array}{ccc}
\operatorname{Tor}_n^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)\\
\downarrow v_n&&\downarrow\operatorname{Hom}(u_n,1)\\
\operatorname{Tor}_{n-1}^A(P,N)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P),
\end{array}
\tag{5}
$$

where the horizontal arrows are the canonical homomorphisms, is commutative.

If $n=1$, we thus have a commutative diagram:

$$
\begin{array}{ccccc}
0&&&&0\\
\downarrow&&&&\downarrow\\
\operatorname{Tor}_1^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^1(M,A),P)\\
\downarrow v_1&&&&\downarrow\operatorname{Hom}(u_1,1)\\
P\otimes_A N&\longrightarrow&\operatorname{Hom}_A(N^*,P)\\
\downarrow&&&&\downarrow\\
P\otimes_A L&\longrightarrow&\operatorname{Hom}_A(L^*,P)
\end{array}
$$

where the columns are exact; this yields the result in this case. If $n\geq 2$, the mappings $u_n$ and $v_n$ are bijective (X, p. 128, cor. 4 and p. 131, cor. 3). By the induction hypothesis, the canonical homomorphism

$$
\operatorname{Tor}_{n-1}^A(P,N)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P)
$$

is injective (resp. bijective); the diagram (5) shows that the same holds for the canonical homomorphism $\operatorname{Tor}_n^A(P,M)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)$, which completes the proof.

### 3. Homological dimension of a ring

#### Definition 2 {#alg-x-s8-def-2 .statement}

We call the homological dimension of $A$ and denote by $\operatorname{dh}(A)$ the supremum in $\mathbf{Z}$ of the set of integers $n$ for which there exist two $A$-modules M and N such that $\operatorname{Ext}_A^n(M,N)\neq 0$.

We have $\operatorname{dh}(0)=-\infty$, $\operatorname{dh}(A)\geq 0$ if $A\neq 0$. We shall see below that $\operatorname{dh}(A)=1$ if $A$ is principal and is not a field, and that, if K is a commutative field

$$
\operatorname{dh}(K[X_1,\ldots,X_n])=n.
$$

#### Proposition 4 {#alg-x-s8-prop-4 .statement}

Let $n$ be an integer $\geq 0$. The following conditions are equivalent:

(i) $\operatorname{dh}(A)\leq n$,

(ii) for every $A$-module M, we have $\mathrm{dp}_A(M)\leq n$,

(ii′) for every finitely generated $A$-module M, we have $\mathrm{dp}_A(M)\leq n$,

(iii) for every exact sequence

$$
0 \to K \to P_{n-1} \to P_{n-2} \to \ldots \to P_0
$$

where the $P_i$ are projective, $K$ is projective,

(iv) for every exact sequence

$$
I^0 \to I^1 \to \ldots \to I^{n-1} \to N \to 0
$$

where the $I^i$ are injective, $N$ is injective,

(v) every $A$-module possesses an injective resolution of length $\leq n$.

The equivalence of conditions (i), (ii) and (iii) follows from prop. 1. We have obviously (ii) $\Rightarrow$ (ii’). It is therefore enough to proving (ii’) $\Rightarrow$ (iv) $\Rightarrow$ (v) $\Rightarrow$ (i).

(ii’) $\Rightarrow$ (iv): with the notation of (iv), let $K$ be the kernel of $I^0 \to I^1$. By X, p. 128, cor. 4, we have for every $A$-module $M$ an isomorphism $\mathrm{Ext}_A^1(M, N) \to \mathrm{Ext}_A^{n+1}(M, K)$; it then follows from (ii’) that $\mathrm{Ext}_A^1(M, N)$ is zero for every finitely generated $A$-module $M$. By X, p. 93, prop. 11, this implies that $N$ is injective, whence (iv).

(iv) $\Rightarrow$ (v): let $M$ be an $A$-module. Applying (iv) to the exact sequence

$$
0 \to M \to I^0(M) \to I^1(M) \to \ldots \to I^{n-1}(M) \to K^{n-1}(M) \to 0
$$

of X, p. 52, we conclude that $K^{n-1}(M)$ is injective, whence (v).

(v) $\Rightarrow$ (i): this follows from X, p. 100, th. 1.

#### Remarque 1 {#alg-x-s8-n3-rem-1 .statement}

If $\mathrm{dh}(A) \leq n < +\infty$, we have $\mathrm{Tor}_{n+1}^A(P, M) = 0$ for every $A$-module $M$ and every right $A$-module $P$, since $\mathrm{dp}_A(M) \leq n$ (cf. lemma 1).

#### Remarque 2 {#alg-x-s8-n3-rem-2 .statement}

For $\mathrm{dh}(A)$ to be finite, it is necessary and sufficient that $\mathrm{dp}_A(M)$ be finite for every nonzero $A$-module $M$. This indeed follows from the preceding and from X, p. 135, cor. 1.

#### Corollaire {#alg-x-s8-n3-cor-1 .statement}

Suppose $A$ is left noetherian and let $n$ be an integer $> 0$. The following conditions are equivalent:

(i) $\mathrm{dh}(A) \leq n$,

(ii) for every pair of a-modules $M$ and $N$ of finite type, we have $\mathrm{Ext}_A^{n+1}(M, N) = 0$,

(iii) for every left a-module $M$ of finite type and every right a-module $P$ of finite type, we have $\mathrm{Tor}_{n+1}^A(P, M) = 0$.

This follows from Props. 2 and 4.

#### Remark {#alg-x-s8-n3-rem-3 .statement}

By the equivalence of (i) and (iii), we have $\mathrm{dh}(A) = \mathrm{dh}(A^\circ)$ if $A$ is left and right noetherian. This equality is not valid in general (X, p. 204, Exercise 20).

#### Proposition 5 {#alg-x-s8-prop-5 .statement}

Suppose $A$ is left noetherian and of finite homological dimension and let $\mathcal{C}_0$ (resp. $\mathcal{C}$) be the set of equivalence classes of finitely generated projective a-modules (resp. of a-modules). Then the canonical homomorphism of Grothendieck groups $K(\mathcal{C}_0) \to K(\mathcal{C})$ is bijective.

This follows from X, p. 137, Cor.

### 4. Rings of Homological Dimension 0

#### Proposition 6 {#alg-x-s8-prop-6 .statement}

The following conditions are equivalent :
(i) every a-module is projective,
(ii) every a-module is injective,
(iii) every ideal of $A$ is an injective module,
(iv) $\mathrm{dh}(A) \leq 0$,
(v) $A$ is semisimple,
(vi) $A$ is noetherian and every a-module is flat;
(vii) every complex of a-modules is split,
(viii) every exact sequence of a-modules is split.

By Prop. 4, we have (i) ⇔ (ii) ⇔ (iv); by Corollary 1 to Prop. 4, we have (vi) ⇒ (iv). By X, p. 35, Example 4, we have (i) ⇒ (vii); since (ii) ⇒ (iii) and (vii) ⇒ (viii) are trivial and since (viii) ⇒ (i) follows from II, p. 39, Prop. 4, it remains to be shown (iii) ⇒ (v) and (v) ⇒ (vi); the last assertion follows from VIII, § 5, No. 1, Props. 1 and 2; finally, if every ideal of $A$ is injective, it is a direct factor in $A$, hence (iii) ⇒ (v).

### 5. Rings of Homological Dimension 1

#### Proposition 7 {#alg-x-s8-prop-7 .statement}

The following conditions are equivalent :
(i) $\mathrm{dh}(A) \leq 1$,
(ii) every submodule of a projective module is projective,
(ii') every ideal of $A$ is projective,
(iii) every quotient of an injective a-module is injective,
(iv) for every projective complex $C$, there exists a homomorphism $\varphi : C \to H(C)$ such that $H(\varphi) = 1_{H(C)}$,
(v) for every injective complex $C$, there exists a homomorphism $\psi : H(C) \to C$ such that $H(\psi) = 1_{H(C)}$.

(i) ⇔ (ii) ⇔ (iii) : this follows from Prop. 4 of X, p. 138.
(ii) ⇒ (iv) : let $C$ be a projective complex. If (ii) is satisfied, the submodule $B(C)$ of $C$ is projective, hence (iv) by X, p. 35, Remark b).
(iii) ⇒ (v) : let $C$ be an injective complex. If (iii) is satisfied, the quotient $B_n(C)$ of $C_{n+1}$ is injective for all $n$, hence (v) by X, p. 35, Remark a).
(iv) ⇒ (ii) : let $P$ be a projective a-module, $M$ a submodule of $P$, and $i : M \to P$ the canonical injection. Let $p : L \to M$ be a surjective homomorphism from a free module $L$ onto $M$. Consider the projective complex $C$ such that $C_1 = L$, $C_0 = P$, $C_i = 0$ for $i \ne 0, 1$, and $d_1 = i \circ p$. If (iv) is satisfied, let $\varphi : C \to H(C)$ be a homomorphism such that $H(\varphi) = 1_{H(C)}$. Since $H_1(C) = \mathrm{Ker}\ p$, $\varphi_1$ is a projector of $L$ onto $\mathrm{Ker}\ p$, so the exact sequence

$$
0 \to \mathrm{Ker}\ p \to L \xrightarrow{p} M \to 0
$$

is split and $M$ is isomorphic to a direct factor of $L$, hence projective.

$(v)\Rightarrow(iii)$ : let $I$ be an injective module, $M$ a quotient of $I$, and $\pi : I \to M$ the canonical projection. Let $i : M \to J$ be an injective homomorphism of $M$ into an injective module $J$. Consider the injective complex $C$ such that $C^0 = I$, $C^1 = J$, $C^i = 0$ for $i \ne 0, 1$, and $d^0 = i \circ \pi$. If (v) is satisfied, let $\psi : H(C) \to C$ be a homomorphism such that $H(\psi) = 1_{H(C)}$. Since

$$
H^1(C) = \operatorname{Coker}i,
$$

$\psi^1$ is a section of the canonical projection $J \to \operatorname{Coker}i$, and $M$ is a direct factor in $J$, hence injective.

$(ii)\Rightarrow(ii')$ : this is trivial.

$(ii')\Rightarrow(ii)$ : this follows from VII, § 3, Corollary 1 to Theorem 1.

#### Example {#alg-x-s8-n5-exa-1 .statement}

If $A$ is principal, then $\operatorname{dh}(A) \leq 1$.

#### Remark {#alg-x-s8-n5-rem-1 .statement}

If $A$ is (commutative) a domain, the preceding conditions are also equivalent to the following :

(iii') : every divisible a-module is injective,

(vi) : every torsion-free a-module is flat and $A$ is noetherian.

Domains satisfying these conditions are called Dedekind rings (cf. X, p. 204, Exercise 12 and AC, VII, § 2, No. 2, Th. 1).

#### Corollary {#alg-x-s8-n5-cor-1 .statement}

Let $A$ be a ring of homological dimension $\leq 1$, $C$ a complex of projective a-modules, $\widetilde{C}$ a complex of projective right a-modules, $C'$ a complex of injective a-modules, $P$ a right a-module, $M$ a left a-module, and $n$ an integer. Then there are split exact sequences

$$
0\to\bigoplus_{p+q=n}H_p(\widetilde C)\otimes_A H_q(C)\xrightarrow{\gamma}H_n(\widetilde C\otimes_A C)\xrightarrow{\alpha}\bigoplus_{p+q=n-1}\operatorname{Tor}_1^A(H_p(\widetilde C),H_q(C))\to0,
$$

$$
0\to\prod_p\operatorname{Ext}_A^1(H_p(C),H^{n-p-1}(C'))\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,C'))\xrightarrow{\lambda}\prod_p\operatorname{Homgr}_A(H_p(C),H^{n-p}(C'))\to0,
$$

$$
0\to P\otimes_A H_n(C)\xrightarrow{\gamma}H_n(P\otimes_A C)\xrightarrow{\alpha}\operatorname{Tor}_1^A(P,H_{n-1}(C))\to0,
$$

$$
0\to\operatorname{Ext}_A^1(H_{n-1}(C),M)\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,M))\xrightarrow{\lambda}\operatorname{Hom}_A(H_n(C),M)\to0.
$$

Since $Z(C)$, $B(C)$, $Z(\widetilde C)$, and $B(\widetilde C)$ are projective and $B(C')$ is injective, this follows from X, p. 78, Cor. 2, p. 96, Cor. 1, and p. 98, Cor. 2.

### 6. Homological Dimension of Polynomial Rings

#### Lemma 2 {#alg-x-s8-lem-2 .statement}

Let $\rho : A\to A'$ be a ring homomorphism, M an a-module, M′ an a′-module. If the a-module $A'_d$ is flat, one has $\mathrm{dp}_A(A'\otimes_A M)\leq\mathrm{dp}_A(M)$. If the a-module $A'_s$ is projective, one has $\mathrm{dp}_A(M')\leq\mathrm{dp}_{A'}(M')$.

The first assertion is clear if $\mathrm{dp}_A(M) = \pm \infty$; if $\mathrm{dp}_A(M) = n \in \mathbf{N}$, there exists an exact sequence of $A$-modules

$$
0 \to P_n \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

where the $P_i$ are projective ; the sequence of $A'$-modules

$$
0 \to A' \otimes_A P_n \to A' \otimes_A P_{n-1} \to \ldots \to A' \otimes_A P_0 \to A' \otimes_A M \to 0
$$

is exact, since $A'_d$ is flat, and the $A'$-modules $A' \otimes_A P_i$ are projective (II, p. 89, Corollary) ; therefore $\mathrm{dp}_{A'}(A' \otimes_A M) \leq n = \mathrm{dp}_A(M)$. The second assertion is clear if $\mathrm{dp}_{A'}(M') = \pm \infty$; if $\mathrm{dp}_{A'}(M') = m \in \mathbf{N}$, there exists an exact sequence of $A'$-modules

$$
0 \to P'_m \to P'_{m-1} \to \ldots \to P'_0 \to M' \to 0 ,
$$

where the $P'_i$ are projective ; the underlying sequence of $A$-modules is exact. Moreover each $P'_i$ is a sub-$A'$-module direct factor of a module ${A'_s}^{(1)}$, hence is a projective $A$-module ; therefore one has $\mathrm{dp}_A(M') \leq m = \mathrm{dp}_{A'}(M')$.

#### Lemma 3 {#alg-x-s8-lem-3 .statement}

*Assume A commutative and let M be an a[X]-module.*
  a) *One has* $\mathrm{dp}_A(M) \leq \mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1$.
  b) *If the homothety* $X_M$ *is injective, one has* $\mathrm{dp}_A(M/XM) \leq \mathrm{dp}_{A[X]}(M)$.
  c) *If* $XM = 0$, *one has* $\mathrm{dp}_A(M) + 1 = \mathrm{dp}_{A[X]}(M)$.
  a) One has an exact sequence of $A[X]$-modules (III, p. 106 and VII, § 5, No. 1)

$$
0 \to A[X] \otimes_A M \to A[X] \otimes_A M \to M \to 0 ;
$$

The assertion *a)* follows from X, p. 135, Corollary 2 and Lemma 2.

*b)* If $\mathrm{dp}_{A[X]}(M) = \pm \infty$, the assertion is trivial. If $M$ is projective and nonzero, then the $A$-module $M/XM$ is identified with $A \otimes_{A[X]} M$, hence is projective, and one has $\mathrm{dp}_A(M/XM) \leq 0 = \mathrm{dp}_{A[X]}(M)$. Let us argue by induction on $\mathrm{dp}_{A[X]}(M) = n$, assumed $> 0$. Consider an exact sequence of $A[X]$-modules $0 \to N \to L \to M \to 0$, where $L$ is a free $A[X]$-module ; applying to the diagram

$$
\begin{array}{ccc}
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0 \\
& & \downarrow \quad \downarrow \quad \downarrow \\
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0
\end{array}
$$

Proposition 2 of X, p. 4, one sees that $X_N$ is injective and that one has the exact sequence

$$
0 \to N/XN \to L/XL \to M/XM \to 0 .
$$

Since $L$ is free over $A[X]$, $L/XL$ is free over $A$ and one has

$$
\mathrm{dp}_{A[X]}(N) = n - 1 , \quad \mathrm{dp}_A(M/XM) \leq 1 + \mathrm{dp}_A(N/XN) ;
$$

since $\mathrm{dp}_A(N/XN) \leq n - 1$ by the induction hypothesis, one deduces $\mathrm{dp}_A(M/XM) \leq n$, which was to be proved.

c) The assertion is trivial if $\mathrm{dp}_{A[X]}(M) = \pm \infty$, and also if $\mathrm{dp}_{A[X]}(M) = 0$ (which is impossible since $XM = 0$). We may therefore suppose $\mathrm{dp}_{A[X]}(M) = n > 0$. Considering as above an exact sequence $0 \to N \to L \to M \to 0$, where $L$ is a free $A[X]$-module, we obtain an exact sequence of $A$-modules

$$
0 \to M \to N/XN \to L/XL \to M \to 0 .
$$

By b), we have $\mathrm{dp}_A(N/XN) \leq \mathrm{dp}_{A[X]}(N) = \mathrm{dp}_{A[X]}(M) - 1 = n - 1$; since $\mathrm{dp}_A(L/XL) = 0$, we deduce from the preceding exact sequence, applying $X$ twice, p. 135, cor. 2, that $\mathrm{dp}_A(M) \leq n - 1$. But, by a), we have

$$
\mathrm{dp}_A(M) \geq \mathrm{dp}_{A[X]}(M) - 1 = n - 1 ,
$$

whence c).

#### Theorem 1 {#alg-x-s8-thm-1 .statement}

*Suppose $A$ commutative. Then*

$$
dh(A[X]) = dh(A) + 1 .
$$

For every $A[X]$-module $M$, we have (*lemma 3*)

$$
\mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1 \leq dh(A) + 1
$$

therefore $dh(A[X]) \leq dh(A) + 1$; conversely, if $M$ is an $A$-module, let $\overline{M}$ be the $A[X]$-module obtained by equipping $M$ with the structure for which $XM = 0$, then (*lemma 3*)

$$
\mathrm{dp}_A(M) = \mathrm{dp}_{A[X]}(\overline{M}) - 1 \leq dh(A[X]) - 1 ,
$$

therefore $dh(A) \leq dh(A[X]) - 1$.

#### Corollary 1 {#alg-x-s8-thm-1-cor-1 .statement}

*Suppose $A$ commutative. We have*

$$
dh(A[X_1, ..., X_n]) = dh(A) + n .
$$

This follows from the theorem by induction on $n$.

#### Corollary 2 {#alg-x-s8-thm-1-cor-2 .statement}

*Let $K$ be a commutative field* (resp. *a principal ideal domain* *or a Dedekind ring* *which is not a field*). *Then* $dh(K[X_1, ..., X_n])$ *is equal to* $n$ (resp. $n + 1$). This follows from the fact that $dh(K) = 0$ (resp. $dh(K) = 1$).

### 7. Homological dimension of graded modules

In this section, we suppose that $A$ is a graded ring with degrees $\geq 0$. We denote by $(A_n)_{n \in \mathbf{Z}}$ its grading; we have therefore $A_n = 0$ for $n < 0$, $A_0$ is a subring of $A$, $J_0 = \bigoplus_{n > 0} A_n$ is a two-sided ideal of $A$ and the graded quotient ring $A/J_0$ is identified with $A_0$.

#### Lemma 4 {#alg-x-s8-lem-4 .statement}

Let $M$ be a graded $A$-module bounded below (X, p. 56). If $A_0 \otimes_A M = 0$, then $M = 0$.

Since $A_0 \otimes_A M$ is isomorphic to $M/J_0 M$, this is none other than ll, p. 171, prop. 6.

#### Lemma 5 {#alg-x-s8-lem-5 .statement}

Let $M$ be a graded $A$-module bounded below, and let
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
be a graded $A$-homomorphism such that $1 \otimes_A s : A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \to A_0 \otimes_A M$ is the canonical isomorphism. Then $s$ is surjective. If $\mathrm{Tor}_1^A(A_0, M) = 0$, $s$ is bijective.

We have an exact sequence
$$
0 \to \mathrm{Ker}\ s \to A \otimes_{A_0} M J_0 M \to M \to \mathrm{Coker}\ s \to 0
$$
and the graded $A$-modules $\mathrm{Ker}\ s$ and $\mathrm{Coker}\ s$ are bounded below. From the exact sequence $A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M \to A_0 \otimes_A \mathrm{Coker}\ s \to 0$, we deduce that $A_0 \otimes_A \mathrm{Coker}\ s = 0$, hence $s$ is surjective (Lemma 4). We then have an exact sequence
$$
\mathrm{Tor}_1^A(A_0, M) \to A_0 \otimes_A \mathrm{Ker}\ s \to A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M .
$$
If $\mathrm{Tor}_1^A(A_0, M) = 0$, then $A_0 \otimes_A \mathrm{Ker}\ s = 0$ and $s$ is injective (Lemma 4).

#### Proposition 8 {#alg-x-s8-prop-8 .statement}

Let $M$ be a graded $A$-module bounded below.

a) The following conditions are equivalent :
(i) $M$ is isomorphic to a graded $A$-module of the form $A \otimes_{A_0} N$, where $N$ is a graded projective $A_0$-module (resp. graded free) ;
(ii) $M$ is a projective $A$-module (resp. graded free) ;
(iii) $M/J_0 M$ is a projective $A_0$-module (resp. graded free) and $\mathrm{Tor}_1^A(A_0, M) = 0$.

b) Assume furthermore that $M$ has a generator system consisting of homogeneous elements of bounded degrees. Then the following conditions are equivalent :
(i) The graded $A$-module $M$ has a finite composition series whose quotients are isomorphic to graded $A$-modules of the form $A \otimes_{A_0} N$, where $N$ is a graded $A_0$-module that is flat ;
(ii) $M$ is a flat $A$-module ;
(iii) $M/J_0 M$ is a flat $A_0$-module and $\mathrm{Tor}_1^A(A_0, M) = 0$.

In each case, there is obviously (i) ⇒ (ii) ⇒ (iii). Therefore, it remains to prove (iii) ⇒ (i).

a) The graded $A$-module $A \otimes_{A_0} M/J_0 M$ is a projective $A$-module since $M/J_0 M$ is a projective $A_0$-module. The canonical homomorphism of $A$-modules
$$
p : M \to M/J_0 M
$$
is surjective ; hence there exists a graded $A$-homomorphism of degree zero
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
such that $p \circ s(a \otimes x) = ax$ for $a \in A$ and $x \in M/J_0 M$.

By Lemma 5, $s$ is an isomorphism of $A$-modules from $A\otimes_{A_0}M/J_0M$ onto $M$, whence (i).

b) By the hypothesis on $M$, there exist integers $a,b$ with $a\leq b$ such that $M$ is generated by $\displaystyle\bigoplus_{a\leq i\leq b}M_i$. We argue by induction on the positive integer $b-a$.

If $b-a=0$, then $M$ is generated by $M_a$ and the canonical $A_0$-homomorphism
$$
M_a\longrightarrow M/J_0M
$$
is bijective; we then deduce from the $A$-homomorphism $A\otimes_{A_0}M_a\longrightarrow M$ defined by the $A$-module structure of $M$ a graded $A$-homomorphism
$$
s:A\otimes_{A_0}M/J_0M\longrightarrow M
$$
satisfying the condition of Lemma 5. Then, by Lemma 5, $s$ is bijective, whence (i).

In the general case, let $M^{(a)}$ be the (graded) sub-$A$-module of $M$ generated by $M_a$ and $M'$ the quotient $M/M^{(a)}$. We have an exact sequence
$$
0\longrightarrow M^{(a)}\xrightarrow{f}M\xrightarrow{g}M'\longrightarrow0,
$$
whence, since $\operatorname{Tor}_1^A(A_0,M)=0$ by hypothesis, exact sequences
$$
\tag{6}
\operatorname{Tor}_2^A(A_0,M')\longrightarrow\operatorname{Tor}_1^A(A_0,M^{(a)})\longrightarrow0
$$
$$
\tag{7}
0\longrightarrow\operatorname{Tor}_1^A(A_0,M')\longrightarrow M^{(a)}/J_0M^{(a)}
\xrightarrow{1\otimes f}M/J_0M\xrightarrow{1\otimes g}M'/J_0M'\longrightarrow0.
$$

But the canonical homomorphism $M_a\longrightarrow M^{(a)}/J_0M^{(a)}$ is bijective. It follows that the homomorphism $1\otimes f:M^{(a)}/J_0M^{(a)}\longrightarrow M/J_0M$ is injective and that its image is a direct factor sub-$A_0$-module of $M/J_0M$. It then follows from the exact sequence (7) that $\operatorname{Tor}_1^A(A_0,M')=0$ and that the $A_0$-module $M'/J_0M'$ is flat since isomorphic to a direct factor of $M/J_0M$. By the induction hypothesis (which applies to $M'$ since it is generated by the $M'_i$ for $a<i\leq b$), $M'$ satisfies condition (i), hence is flat. We then deduce from the exact sequence (6) that $\operatorname{Tor}_1^A(A_0,M^{(a)})=0$, but $M^{(a)}/J_0M^{(a)}$ is identified with $M_a$ which is a flat $A_0$-module (as a direct factor submodule of $M/J_0M$) ; by what has already been proved, the graded $A$-module $M^{(a)}$ is isomorphic to $A\otimes_{A_0}M_a$, hence also satisfies (i), which completes the proof.

#### Corollary 1 {#alg-x-s8-prop-8-cor-1 .statement}

Let $M$ be a graded $A$-module of finite type. If the $A_0$-module $M/J_0M$ is projective (resp. graded free, resp. flat) and if $\operatorname{Tor}_1^A(A_0,M)=0$, then the $A$-module $M$ is projective (resp. graded free, resp. flat).

#### Corollary 2 {#alg-x-s8-prop-8-cor-2 .statement}

#### Corollary 3 (Hilbert’s Syzygy Theorem) {#alg-x-s8-prop-8-cor-3 .statement}
*Assume that $A_0$ is a commutative field and that $A$ is generated as an $A_0$-algebra by $n$ homogeneous elements of degrees > 0 and algebraically independent. For every graded $a$-module $M$ bounded below (resp. of finite type), there exists an exact sequence of graded $a$-modules and of degree $0$ homogeneous maps*
$$
0 \to L_n \to L_{n-1} \to \ldots \to L_0 \to M \to 0,
$$
where the $L_i$ are graded free and bounded below (resp. graded free and of finite type).

Indeed, $dh(A) = n$ by Theorem 1 of X, p. 143, and Corollary 2 is applied.

#### Remark {#alg-x-s8-n7-rem-1 .statement}
*Corollary 2 also applies in the following cases:
a) $A_0$ is principal and $A = A_0[X_1, ..., X_{n-1}]$;
b) $A_0$ is a regular local noetherian ring of dimension $r$ and $A = A_0[X_1, ..., X_n, r]$.*

#### Corollary 4 {#alg-x-s8-prop-8-cor-4 .statement}
*Assume that $A_0$ is semisimple. Let $M$ be a graded $a$-module bounded below and let $n$ be an integer $\geq 0$. In order that $\mathrm{dp}_A(M) \leq n$, it is necessary and sufficient that*
$$
\operatorname{Tor}_{n+1}^A(A_0, M) = 0.
$$
If $\mathrm{dp}_A(M) \leq n$, then $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ (X, p. 135, Lemma 1). Conversely, let $\dots \to L_1 \to L_0 \to M \to 0$ be an exact sequence of graded $a$-modules bounded below such that $L_0, \dots, L_{n-1}$ are graded free (X, p. 56, Prop. 11); according to Cor. 3 of X, p. 131, the equality $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ implies $\operatorname{Tor}_1^A(A_0, K) = 0$; since $K/J_0 K$ is a projective $A_0$-module because $A_0$ is semisimple (X, p. 140, Prop. 6), $K$ is projective by Prop. 8 (X, p. 144), and $\mathrm{dp}_A(M) \leq n$.

#### Corollary 5 {#alg-x-s8-prop-8-cor-5 .statement}

*Suppose the ring $A_0$ semisimple. If $\operatorname{Tor}_{n+1}^A(A_0, A_0) = 0$, one has $\mathrm{dp}_A(M) \leq n$ for every graded $A$-module bounded below.

Denote by $A^\circ$ the graded ring opposite to $A$: we have $(A^\circ)_0 = (A_0)^\circ$, so $(A^\circ)_0$ is semisimple (VIII, § 5, No. 1, remark 3). Since $\operatorname{Tor}_{n+1}^{A^\circ}(A_0^\circ, A_0^\circ) = 0$, one has $\mathrm{dp}_A(A_{0s}^\circ) \leq n$ by cor. 4: this implies $\operatorname{Tor}_{n+1}^{A^\circ}(M_0, A_0^\circ) = 0$ for every $A$-module $M$, hence $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ and we apply cor. 4.

## EXERCISES {#alg-x-s8-exercises}

See the [exercises for § 8](exercises/s8/).
