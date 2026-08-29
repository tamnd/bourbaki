---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 3
section_title: Résolutions
lang: en
source: alg-x-fr
book_pages: A X.46-A X.61, A X.178-A X.184
pdf_pages: 0052-0067, 0184-0190
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement de morphismes de complexes
      page: 46
      pdf_page: 52
    - "no": 2
      title: Résolutions
      page: 48
      pdf_page: 54
    - "no": 3
      title: La résolution libre canonique
      page: 50
      pdf_page: 56
    - "no": 4
      title: La résolution injective canonique
      page: 52
      pdf_page: 58
    - "no": 5
      title: Résolutions de type fini
      page: 53
      pdf_page: 59
    - "no": 6
      title: ' Résolutions projectives minimales'
      page: 54
      pdf_page: 60
    - "no": 7
      title: Résolutions graduées
      page: 56
      pdf_page: 62
    - "no": 8
      title: La résolution standard
      page: 57
      pdf_page: 63
    - "no": 9
      title: Résolutions et groupes de Grothendieck
      page: 58
      pdf_page: 64
statements: 29
exercises: 19
content_sha256: a1b2e48f6dae81d4cf5b709be2d47f83208c48b5e620837f8b9559aaa92197bf
translated_from: content/fr/alg/X/03_s3_resolutions.md
source_lang: fr
translation_method: machine
source_content_sha256: 5ebb6c8a429b73fb0e96f7c1b840436916f3f85cfd822df95c442238a2791ff1
translation_model: gpt-5.4
translation_run: translate-en-mt-931dafce
glossary_version: 34
glossary_terms_sha256: 3518ae3f83c8958a673714008e91f72c2230f18cbae54da64b716f0d71e46fb9
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. RESOLUTIONS

We retain the conventions of the preceding paragraph.

### 1. Extension of morphisms of complexes

#### Lemma 1 {#alg-x-s3-lem-1 .statement}

Consider a diagram of A-modules and homomorphisms

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
f' \downarrow & & f \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f \downarrow & & k'' \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

such that $f \circ \alpha' = \beta \circ f', \alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta', \text{and } f = k'' \circ \alpha + \beta \circ k \text{ and where } M' \text{ is projective. There exists an A-homomorphism } k': M' \to N' \text{ such that } f' = k \circ \alpha' + \beta' \circ k'.$

In fact, put $g = f' - k \circ \alpha'$; we have
$$
\beta \circ g = \beta \circ f' - \beta \circ k \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = k'' \circ \alpha \circ \alpha' = 0.
$$
This implies $\mathrm{Im}\ (g) \subset \mathrm{Ker}\ (\beta) = \mathrm{Im}\ (\beta')$. Since $M'$ is projective, there therefore exists an A-homomorphism $k': M' \to N'$ such that $\beta' \circ k' = g$, whence the lemma.

#### Lemma 2 {#alg-x-s3-lem-2 .statement}

If in the commutative diagram of A-modules and homomorphisms

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
& \downarrow u & \downarrow u'' \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
& \downarrow & \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

one has $\alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta'$ and if $M'$ is projective, there exists an A-homomorphism $u': M' \to N'$ such that $\beta' \circ u' = u \circ \alpha'$.

It is enough to put $k'' = u'', k = -u, f = 0, f' = 0$ and $u' = k'$ in Lemma 1.

Lemma 1 bis. — Consider a diagram of A-modules and homomorphisms

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
k' \downarrow & & k \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f' \downarrow & & f \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

such that $f \circ \alpha' = \beta \circ f'$, $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha'$, $\beta \circ \beta' = 0$, and $f' = k \circ \alpha' + \beta' \circ k'$ and where $N''$ is injective. There exists an $A$-homomorphism $k'' : M'' \to N''$ such that $f = k'' \circ \alpha + \beta \circ k$.

In fact, put $g = f - \beta \circ k$, we have
$$
g \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = \beta \circ f' - \beta \circ k \circ \alpha' = \beta \circ \beta' \circ k' = 0 .
$$
This implies $\mathrm{Ker}\, g \supset \mathrm{Im}\, \alpha' = \mathrm{Ker}\, \alpha$. Since $N''$ is injective, there therefore exists (X, p. 16, remark) an $A$-homomorphism $k' : M'' \to N''$ such that $g = k'' \circ \alpha$, whence the lemma.

Lemma 2 bis. — If, in the commutative diagram of $A$-modules and homomorphisms

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \xrightarrow{\alpha} M'' \\
u' \downarrow & & u \downarrow \\
N' & \xrightarrow{\beta'} & N \xrightarrow{\beta} N''
\end{array}
$$

one has $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha', \beta \circ \beta' = 0$ and if $N''$ is injective, there exists an $A$-homomorphism $u'' : M'' \to N''$ such that $u'' \circ \alpha = \beta \circ u$.
It is enough to put $u' = k', u = -k, f = 0, f' = 0$ and $k'' = u''$ in Lemma 1 bis.

#### Proposition 1 {#alg-x-s3-prop-1 .statement}

Let $(P, d_P)$ and $(E, d_E)$ be two complexes of $A$-modules and $r$ an integer.

a) Let $(u_i : P_i \to E_i)_{i \leq r}$ be a family of homomorphisms such that $d_E \circ u_i = u_{i-1} \circ d_P$ for $i \leq r$. Suppose that $P_i$ is projective for $i > r$ and that $H_i(E) = 0$ for $i \geq r$. Then the family of the $u_i$ extends to a morphism of complexes from $P$ into $E$; two such extensions are homotopic.

b) Let $(u^i : P^i \to E^i)_{i \leq r}$ be a family of homomorphisms such that $u^i \circ d_P = d_E \circ u^{i-1}$ for $i \leq r$. Suppose that $E^i$ is injective for $i > r$ and that $H^i(P) = 0$ for $i \geq r$. Then the family of the $u^i$ extends to a morphism of complexes from $P$ into $E$; two such extensions are homotopic.

Let us prove a). The existence of an extension $v$ of the family $(u_i)_{i \leq r}$ follows at once from Lemma 2 by induction. Let $v'$ be another extension; put $f = v' - v$, and construct by induction on the integer $n$ a homomorphism $k_n : P_n \to E_{n+1}$ such that $f_n = d_E \circ k_n + k_{n-1} \circ d_P$. For $i \leq r$, take $k_i = 0$. Let $n \geq r$ and suppose that the $k_i$ have been constructed for $i \leq n$. Consider then the diagram

$$
\begin{array}{cccccc}
P_{n+1} & \xrightarrow{d_P} & P_n & \xrightarrow{d_P} & P_{n-1} \\
f_{n+1} \downarrow & & & & k_{n-1} \downarrow \\
E_{n+2} & \xrightarrow{d_E} & E_{n+1} & \xrightarrow{d_E} & E_n .
\end{array}
$$

The hypotheses of Lemma 1 are satisfied; there therefore exists an $A$-homomorphism $k_{n+1} : P_{n+1} \to E_{n+2}$ such that $f_{n+1} = d_E \circ k_{n+1} + k_n \circ d_P$, whence a).

The proof of b) is analogous, via Lemmas 1 bis and 2 bis.

### 2. Resolutions

In the sequel, a module will always be identified with the complex of which it is the component of degree zero and all of whose other components are zero.

#### Definition 1 {#alg-x-s3-def-1 .statement}

Let $M$ be an $A$-module. A left resolution of $M$ is a pair $(P,p)$ where $P$ is a complex zero on the right and $p:P\to M$ is a homomorphism. A right resolution of $M$ is a pair $(e,E)$ where $E$ is a complex zero on the left and $e:M\to E$ a homomorphism.

The length of the resolution $(P,p)$ (resp. $(e,E)$) is called the length of the complex $P$ (resp. $E$). If $(P,p)$ and $(P',p')$ (resp. $(e,E)$ and $(e',E')$) are two left (resp. right) resolutions of $M$, a morphism of complexes $f:P\to P'$ such that $p'\circ f=p$ (resp. $g:E\to E'$ such that $g\circ e=e'$) is called a morphism of resolutions.

#### Proposition 2 {#alg-x-s3-prop-2 .statement}

Let $P$ be a complex zero on the right and $p:P\to M$ a morphism.
For $(P,p)$ to be a left resolution of $M$, it is necessary and sufficient that the sequence

(1)

$$
\cdots\longrightarrow P_n\xrightarrow{d_P}P_{n-1}\longrightarrow\cdots\longrightarrow P_1\xrightarrow{d_P}P_0\xrightarrow{p}M\longrightarrow0
$$

be exact.

In fact, to say that $p:P\to M$ is a homomorphism means that $H_i(P)=0$ for $i>0$ and that $p_0$ induces an isomorphism of $\operatorname{Coker}(d_P:P_1\to P_0)$ onto $M$.

Similarly:

**Proposition 2bis.** — Let $E$ be a complex null on the left and $e:M\to E$ a morphism.
In order that $(e,E)$ be a right resolution of $M$, it is necessary and sufficient that the sequence

(1 bis)

$$
0\longrightarrow M\xrightarrow{e_0}E^0\xrightarrow{d_E}E^1\longrightarrow\cdots\longrightarrow E^n\xrightarrow{d_E}E^{n+1}\longrightarrow\cdots
$$

be exact.

By abuse of language, one often says that sequence (1) (resp. (1 bis)) is a left (resp. right) resolution of $M$.

#### Definition 2 {#alg-x-s3-def-2 .statement}

A projective resolution (resp. free, resp. flat) of the $A$-module $M$ is a left resolution $(P,p)$ of $M$ such that the complex $P$ is projective (resp. free, resp. flat) (X, p. 25). An injective resolution of $M$ is a right resolution $(e,E)$ of $M$ such that the complex $E$ is injective (loc. cit.).

#### Example 1 {#alg-x-s3-n2-exa-1 .statement}

Suppose that the ring $A$ is principal; let $M$ be an $A$-module and $(x_i)_{i\in I}$ a generating family of $M$. Denote by $L_0$ the free module $A^{(I)}$, by $(e_i)$ its canonical basis, and define $p:L_0\to M$ by $p(e_i)=x_i$. The morphism $p$ is surjective and its kernel $L_1$ is a free $A$-module by VII, § 3, Corollary 2 to Theorem 1; hence the exact sequence

$$
0\longrightarrow L_1\longrightarrow L_0\xrightarrow{p}M\longrightarrow0
$$

is a free resolution of $M$ of length 1. If $I$ is finite, $L_0$ and $L_1$ are of finite type.

#### Example 2 {#alg-x-s3-n2-exa-2 .statement}

Suppose A commutative; let E be an A-module and u an endomorphism of E. Denote by $E_u$ the $A[X]$-module obtained by endowing E with the structure defined by

$$
(p, x) \mapsto p(u)(x) \quad \text{for} \quad p \in A[X] \quad \text{and} \quad x \in E.
$$

By III, p. 106, one has an exact sequence:

$$
0 \to A[X] \otimes_A E \xrightarrow{\psi} A[X] \otimes_A E \xrightarrow{\varphi} E_u \to 0
$$

where $\varphi(p \otimes x) = p.x$ and $\psi(p \otimes x) = Xp \otimes x - p \otimes u(x)$ for $p \in A[X]$ and $x \in E$. This exact sequence is a resolution of length 1 of $E_u$, free (resp. projective, resp. of finite type) if E is a free (resp. projective, resp. of finite type) A-module.

#### Example 3 {#alg-x-s3-n2-exa-3 .statement}

If A is principal, the exact sequence

$$
0 \to A \to K \to K/A \to 0
$$

is an injective resolution of length 1 of the A-module $A_s$ (X, p. 18, Example 1).

#### Proposition 3 {#alg-x-s3-prop-3 .statement}

Let $f : M' \to M$ be a homomorphism of A-modules, $p' : P' \to M'$ a morphism into $M'$ of a complex null on the right and projective $P'$, and $p : P \to M$ a left resolution of M. There exists a morphism of complexes $\tilde{f} : P' \to P$, and only one up to homotopy, such that $p \circ \tilde{f} = f \circ p'$.

Let us consider the complex $\overline{P}$ defined as follows: $\overline{P}_n = P_n$ for $n \neq -1$, $\overline{P}_{-1} = M$, $d_{\overline{P},n} = d_{P,n}$ for $n \neq 0, -1$, $d_{\overline{P},0} = p_0$, $d_{\overline{P},-1} = 0$, and the complex $\overline{P}'$ defined analogously. Applying to the complexes $\overline{P}$ and $\overline{P}'$ Prop. 1 a) with $r = 0$, $u_i = 0$ for $i < -1$ and $u_{-1} = f$, we obtain Prop. 3.

#### Corollary {#alg-x-s3-n2-cor-1 .statement}

Let $(P, p)$ and $(P', p')$ be two projective resolutions of M. There exists a morphism, and only one up to homotopy, $\alpha : P' \to P$ such that $p \circ \alpha = p'$.

In fact, there exists a morphism $\alpha : P' \to P$ (resp. $\beta : P \to P'$) such that $p \circ \alpha = p'$ (resp. $p' \circ \beta = p$). Since $p \circ \alpha \circ \beta = p$ (resp. $p' \circ \beta \circ \alpha = p'$), $\alpha \circ \beta$ is homotopic to $1_P$ (resp. $\beta \circ \alpha$ is homotopic to $1_{P'}$).

PROPOSITION 3 bis. — Let $g : N \to N'$ be a homomorphism of a-modules, $e' : N' \to E'$ a morphism from $N'$ into a left zero and injective complex $E'$, and $e : N \to E$ a right resolution of N. There exists a morphism of complexes $\tilde{g} : E \to E'$, and only one up to homotopy, such that $\tilde{g} \circ e = e' \circ g$.

This is proved like Prop. 3 with the aid of Prop. 1 b).

#### Corollary {#alg-x-s3-n2-cor-2 .statement}

Let $(e, E)$ and $(e', E')$ be two injective resolutions of N; there exists a morphism $\alpha : E \to E'$ and only one up to homotopy such that $\alpha \circ e = e'$.

### 3. The canonical free resolution

For every a-module M, let us denote by L_0(M) the free a-module A^{(M)} with basis M, by (e_m)_{m \in M} its canonical basis, and by $p_M : L_0(M) \to M$ the homomorphism such that
$$
p_M(e_m) = m , \quad m \in M .
$$
Put $Z_0(M) = \mathrm{Ker}\, p_M$ and let $i_M : Z_0(M) \to L_0(M)$ be the canonical injection. We have an exact sequence
$$
(1) \qquad 0 \longrightarrow Z_0(M) \xrightarrow{i_M} L_0(M) \xrightarrow{p_M} M \longrightarrow 0 .
$$
A graded module L(M) is defined by putting $L_n(M) = 0$ for $n < 0$ and, by induction on the integer $n > 0$
$$
(2) \qquad L_n(M) = L_0(Z_{n-1}(M)) ; \qquad Z_n(M) = Z_0(Z_{n-1}(M)) .
$$
A-homomorphisms $d_n^M : L_n(M) \to L_{n-1}(M)$ are defined by
$$
(3) \qquad \left\{ \begin{array}{ll}
d_n^M = 0 , & n \leqslant 0 , \\
d_1^M = i_M \circ p_{Z_0(M)} , \\
d_n^M = i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} , & n > 1 .
\end{array} \right.
$$
By construction we have an exact sequence
$$
\longrightarrow L_n(M) \xrightarrow{d_n^M} L_{n-1}(M) \longrightarrow \cdots \longrightarrow L_0(M) \xrightarrow{p_M} M \longrightarrow 0 ,
$$
so that, if $p_M$ is extended to a morphism of complexes
$$
p_M : (L(M), d^M) \to M ,
$$
we obtain a free resolution of M, called the canonical free resolution of M.

Let $f : M \to N$ be an A-homomorphism of a-modules. Denote by
$$
L_0(f) : L_0(M) \to L_0(N)
$$
the unique A-homomorphism such that $L_0(f)(e_m) = e_{f(m)}$ for every $m \in M$. One has
$$
(4) \qquad p_N \circ L_0(f) = f \circ p_M .
$$
It follows that $L_0(f)$ induces an A-homomorphism $Z_0(f) : Z_0(M) \to Z_0(N)$ and one has
$$
(5) \qquad i_N \circ Z_0(f) = L_0(f) \circ i_M .
$$
Put $L_n(f) = 0$, for $n < 0$ and define by induction on the integer $n > 0$, homomorphisms $L_n(f) : L_n(M) \to L_n(N)$ and $Z_n(f) : Z_n(M) \to Z_n(N)$ by
$$
(6) \qquad \left\{ \begin{array}{l}
L_n(f) = L_0(Z_{n-1}(f)) \\
Z_n(f) = Z_0(Z_{n-1}(f)) .
\end{array} \right.
$$

#### Proposition 4 {#alg-x-s3-prop-4 .statement}

$L(f) : L(M) \to L(N)$ is a morphism of complexes of a-modules; one has $p_M \circ L(f) = f \circ p_N$.

It is a matter of proving, for every integer $n > 0$, the formula

$$
d_n^N \circ L_n(f) = L_{n-1}(f) \circ d_n^M .
$$

One has first

$$
\begin{align*}
d_1^N \circ L_1(f) &= i_N \circ p_{Z_0(N)} \circ L_0(Z_0(f)) & \text{(by (3) and (6))} \\
&= i_N \circ Z_0(f) \circ p_{Z_0(M)} & \text{(by (4))} \\
&= L_0(f) \circ i_M \circ p_{Z_0(M)} & \text{(by (5))} \\
&= L_0(f) \circ d_1^M & \text{(by (3))} .
\end{align*}
$$

When $n > 1$, one has successively

$$
\begin{align*}
d_n^N \circ L_n(f) &= i_{Z_{n-2}(N)} \circ p_{Z_{n-1}(N)} \circ L_0(Z_{n-1}(f)) & \text{(by (3) and (6))} \\
&= i_{Z_{n-2}(N)} \circ Z_{n-1}(f) \circ p_{Z_{n-1}(M)} & \text{(by (4))} \\
&= i_{Z_{n-2}(N)} \circ Z_0(Z_{n-2}(f)) \circ p_{Z_{n-1}(M)} & \text{(by (6))} \\
&= L_0(Z_{n-2}(f)) \circ i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} & \text{(by (5))} \\
&= L_{n-1}(f) \circ d_n^M & \text{(by (3) and (6))} .
\end{align*}
$$

One has at once

(7)
$$
L(1_M) = 1_{L(M)} .
$$

On the other hand, if $g : N \to P$ is an A-homomorphism of a-modules, one has

(8)
$$
L(g \circ f) = L(g) \circ L(f) .
$$

In fact, for $m \in M$, one has
$$
L_0(g \circ f)(e_m) = e_{g \circ f(m)} = L_0(g)(e_{f(m)}) = L_0(g) \circ L_0(f)(e_m) ,
$$
hence $L_0(g \circ f) = L(g) \circ L(f)$; consequently $Z_0(g \circ f) = Z_0(g) \circ Z_0(f)$; whence at once $L_n(g \circ f) = L_n(g) \circ L_n(f)$, for $n \geqslant 0$, by induction on $n$, whence (8).

#### Remark {#alg-x-s3-n3-rem-1 .statement}

If $f, g \in \mathrm{Hom}_A(M, N)$, one does not have $L(f + g) = L(f) + L(g)$. However these two morphisms are homotopic according to X, p. 49, prop. 3.

Let $M$ be a right a-module; denote by $A^\circ$ the opposite ring of $A$, by $M^\circ$ the underlying $A^\circ$-module of $M$, by $L(M^\circ)$ its canonical free resolution. This is denoted by $L(M)$, and the underlying A-complex $L(M^\circ)^\circ$ of $L(M^\circ)$ is called the canonical free resolution of $M$. Thus one has

$$
L(M^\circ) = L(M)^\circ .
$$

### 4. The canonical injective resolution

Let $F$ be the $A$-module $\operatorname{Hom}_{\mathbf Z}(A,\mathbf Q/\mathbf Z)$; for every $A$-module $M$, put $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ and denote by $e_M:M\longrightarrow I^0(M)$ the homomorphism which to $m\in M$ associates the family $(\varphi(m))_{\varphi\in\operatorname{Hom}_A(M,F)}$. According to X, p. 19, cor. 2, $I^0(M)$ is an injective $A$-module and $e_M$ is injective. Put $K^0(M)=\operatorname{Coker}e_M$ and denote by $q_M:I^0(M)\longrightarrow K^0(M)$ the canonical projection. Thus one has an exact sequence

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{q_M} K^0(M)\longrightarrow 0.
$$

A graded $A$-module $I(M)$ is defined by putting $I^n(M)=0$ for $n<0$ and, by recurrence on the integer $n>0$,

(9)
$$
I^n(M)=I^0(K^{n-1}(M)),\qquad K^n(M)=K^0(K^{n+1}(M)).
$$

$A$-homomorphisms $\delta_M^n:I^n(M)\longrightarrow I^{n+1}(M)$ are defined by

(10)
$$
\left\{
\begin{aligned}
\delta_M^n&=0, && n<0,\\
\delta_M^0&=\epsilon_{K^0(M)}\circ q_M,\\
\delta_M^n&=\epsilon_{K^n(M)}\circ q_{K^{n-1}(M)}, && n>0.
\end{aligned}
\right.
$$

By construction one has an exact sequence

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{\delta_M^0}\cdots\longrightarrow I^n(M)\xrightarrow{\delta_M^n}I^{n+1}(M)\longrightarrow\cdots,
$$

so that, if $e_M$ is extended to a morphism of complexes

$$
e_M:M\longrightarrow (I(M),\delta_M),
$$

one obtains an injective resolution of $M$, called the canonical injective resolution of $M$.

Let $f:M\longrightarrow N$ be a homomorphism of $A$-modules. Let $I^0(f)$ denote the homomorphism from $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ into $I^0(N)=F^{\operatorname{Hom}_A(N,F)}$ which maps the family $(x_\varphi)_{\varphi\in\operatorname{Hom}_A(M,F)}$ to the family $(x_{\psi\circ f})_{\psi\in\operatorname{Hom}_A(N,F)}$. One has:

(11)
$$
I^0(f)\circ e_M=e_N\circ f.
$$

It follows that $I^0(f)$ induces a homomorphism $K^0(f):K^0(M)\longrightarrow K^0(N)$ and one has

(12)
$$
K^0(f)\circ q_M=q_N\circ K^0(f).
$$

Put $I^n(f)=0$ for $n<0$ and define, by recurrence on the integer $n>0$, homomorphisms $I^n(f):I^n(M)\longrightarrow I^n(N)$ and $K^n(f):K^n(M)\longrightarrow K^n(N)$ by:

(13)
$$
\left\{
\begin{aligned}
I^n(f)&=I^0(K^{n-1}(f)),\\
K^n(f)&=K^0(K^{n-1}(f)).
\end{aligned}
\right.
$$

#### Proposition 5 {#alg-x-s3-prop-5 .statement}

I(f) : I(M) → I(N) is a morphism of complexes of A-modules; one has I(f) ◦ e_M = e_N ◦ f.
This is proved in a manner analogous to Prop. 4.

One has
(14)
$$
I(1_M) = 1_{I(M)}
$$
and for every homomorphism $g : N \to P$ of A-modules
(15)
$$
I(g \circ f) = I(g) \circ I(f) .
$$

#### Remark {#alg-x-s3-n4-rem-1 .statement}

If $f, g \in \mathrm{Hom}_A(M, N)$, one does not have $I(f + g) = I(f) + I(g)$. However, these two morphisms are homotopic by X, p. 49, prop. 3 bis.

If M is a right A-module, one puts $I(M) = I(M^\circ)^\circ$; this is called the canonical injective resolution of M, and one has
$$
I(M^\circ) = I(M)^\circ .
$$

### 5. Resolutions of finite type

In particular, it follows from the two preceding numbers that every A-module possesses injective resolutions, free resolutions (hence also projective or flat resolutions). In certain cases, one can be more precise:

Suppose $A$ left noetherian and let $M$ be an $A$-module. Let us construct by induction sequences $(L_n)_{n \geq 0}$, $(Z_n)_{n \geq 0}$, $(d_n)_{n \geq 1}$ where, for every $n \geq 0$, $L_n$ is a finitely generated free $A$-module, $Z_n$ a submodule of $L_n$ and $d_{n+1} : L_{n+1} \to L_n$ a homomorphism. For this, choose a finite generating family $(m_i)_{i \in I_0}$ of $M$, put $L_0 = A^{(I_0)}$, define $p : L_0 \to M$ by $p(e_i) = m_i$ and put $Z_0 = \mathrm{Ker}\,(p)$. For $n \geq 0$, $L_n$ and $Z_n$ having been constructed, $Z_n$ is finitely generated since contained in $L_n$; choose a finite generating family $(x_{n,i})_{i \in I_{n+1}}$ of $Z_n$; put $L_{n+1} = A^{(I_{n+1})}$, define $d_{n+1}$ by $d_{n+1}(e_i) = x_{n,i}$ and put $Z_{n+1} = \mathrm{Ker}\,(d_{n+1})$.

By construction one has an exact sequence
$$
\cdots \longrightarrow L_{n+1} \xrightarrow{d_{n+1}} L_n \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{p} M \longrightarrow 0 ,
$$
whence:

#### Proposition 6 {#alg-x-s3-prop-6 .statement}

When $A$ is left noetherian, every finitely generated $A$-module $M$ possesses a free resolution $p : L \to M$ such that $L_n$ is finitely generated for every integer n.
More generally:

#### Proposition 7 {#alg-x-s3-prop-7 .statement}

Let $C$ be an $A$-complex and let $a \in \mathbf{Z}$ be such that $H_n(C) = 0$ for $n < a$.
a) There exists a free $A$-complex $L$ such that $L_n = 0$ for $n < a$ and a homologism $f : L \to C$.

b) Suppose $A$ left noetherian and the $A$-modules $H_n(C)$, $n\in \mathbf{Z}$, finitely generated.
There exists a free $A$-complex $L$ such that $L_n=0$ for $n<a$ and that $L_n$ is a finitely generated $A$-module for every $n$, and a homomorphism $f:L\to C$.

Let $C'$ be the subcomplex of $C$ such that $C'_n=C_n$ for $n>a$, $C'_a=Z_a(C)$, $C'_n=0$ for $n<a$; then the canonical injection of $C'$ into $C$ is a homomorphism. Replacing $C$ by $C'$, one may therefore suppose that $C_n=0$ for $n<a$. The statement then results from repeated application of the following lemma, for $r=a,a+1,\ldots$ :

#### Lemma 3 {#alg-x-s3-lem-3 .statement}

Let $C$ be a complex and let $r\in \mathbf{Z}$. There exists a complex $C'$ and a homomorphism $f:C'\to C$ such that $f_n:C'_n\to C_n$ is an isomorphism for $n<r$ and such that $C'_r$ is a free $A$-module. If $A$ is noetherian and the $A$-modules $H_r(C)$ and $C_{r-1}$ are of finite type, one can require that $C'_r$ be of finite type.

a) Let first $h:M\to C_r$ be a homomorphism of $A$-modules; let $d=(d_n)$ denote the differential of $C$. Let $N$ be the submodule of $M\times C_{r+1}$ formed by the pairs $(m,x)$ such that $h(m)=d_{r+1}(x)$; define a complex $(C',d')$ by $C'_n=C_n$ for $n\ne r,r+1$, $C'_r=M$, $C'_{r+1}=N$, $d'_n=d_n$ for $n\ne r,r+1$, $d'_r=h$, $d'_{r+1}(m,x)=m$ for $(m,x)\in N$ and $d'_{r+2}(y)=(0,d_{r+2}(y))$ for $y\in C_{r+2}$. Also consider the morphism of complexes $f:C'\to C$ such that $f_n=1_{C_n}$ for $n\ne r,r+1$, $f_r=h$, $f_{r+1}(m,x)=x$.

b) The complex $\operatorname{Ker}f$ is zero in degree $\ne r,r+1$ and the differential $d'_{r+1}$ induces an isomorphism of $\operatorname{Ker}f_{r+1}$ onto $\operatorname{Ker}f_r$, hence $H(\operatorname{Ker}f)=0$.

c) When the composite mapping $M\xrightarrow{h}C_r\to C_r/B_r(C)$ is surjective, one sees analogously that $H(\operatorname{Coker}f)=0$, and $f$ is then a homomorphism (X, p. 31, cor. 2).

d) When $A$ is assumed noetherian and the $A$-modules $H_r(C)$ and $C_{r-1}$ are of finite type, then $C_r/B_r(C)$ is of finite type, by virtue of the exact sequence (X, p. 25)

$$
0\to H_r(C)\to C_r/B_r(C)\to C_{r-1}\ ;
$$

there then exists a free $A$-module of finite type $M$ and a homomorphism $h:M\to C_r$ such that the condition of c) is satisfied; in the general case, there exists a free module $M$ and a surjective homomorphism $h:M\to C_r$. This completes the proof.

### 6.  Minimal projective resolutions

Let $M$ be an $A$-module and let

$$
(P)\qquad \cdots \longrightarrow F_n \xrightarrow{d_n} F_{n-1}\longrightarrow \cdots \longrightarrow F_0\xrightarrow{d_0} M\longrightarrow 0
$$

a resolution of $M$. One says that $(P)$ is a minimal projective resolution if, for every $n\geq 0$, the homomorphism $\delta_n:P_n\to \operatorname{Im}(d_n)$ induced by $d_n$ is a projective cover (VIII, § 8, No. 5).

#### Proposition 8 {#alg-x-s3-prop-8 .statement}

Let $M$ be an $A$-module, $P$ and $P'$ two minimal projective resolutions of $M$, and $f:P\to P'$ a morphism of resolutions. Then $f$ is an isomorphism.
In particular, two minimal projective resolutions of $M$ are isomorphic.

Put $\widetilde P_n=P_n$ for $n\ne-1$ and $\widetilde P_{-1}=M$; define $\widetilde P'_n$ analogously and put $f_{-1}=1_M$. We shall prove by induction starting from $-1$ that $f_n:\widetilde P_n\to\widetilde P'_n$ is an isomorphism for every $n$. This is evident for $n=-1$; suppose that $f_n$ and $f_{n-1}$ are isomorphisms. It follows from the commutativity of the diagram

$$
\begin{array}{ccc}
P_n & \xrightarrow{\ d_n\ } & P_{n-1}\\
{\scriptstyle f_n}\downarrow && \downarrow{\scriptstyle f_{n-1}}\\
P'_n & \xrightarrow{\ d'_n\ } & P'_{n-1}
\end{array}
$$

that $f_n$ induces an isomorphism $g_n$ of $\operatorname{Ker}d_n$ onto $\operatorname{Ker}d'_n$. It then follows from the commutativity of the diagram

$$
\begin{array}{ccc}
P_{n+1} & \xrightarrow{\ \delta_{n+1}\ } & \operatorname{Ker}d_n\\
{\scriptstyle f_{n+1}}\downarrow && \downarrow{\scriptstyle g_n}\\
P'_{n+1} & \xrightarrow{\ \delta'_{n+1}\ } & \operatorname{Ker}d'_n
\end{array}
$$

and from VIII, *loc. cit*., that $f_{n+1}$ is an isomorphism.

#### Corollary {#alg-x-s3-n6-cor-1 .statement}

*Let $M$ be an $A$-module, $P$ and $P'$ two projective resolutions of $M$; suppose that $P$ is minimal. Let $f:P\to P'$ and $g:P'\to P$ be two morphisms of resolutions. Then $f$ is injective, $g$ is surjective, and $P'$ is the direct sum of the subcomplexes $\operatorname{Im}f$ and $\operatorname{Ker}g$. Moreover $\operatorname{Ker}g$ has zero homology.*

In fact, $\alpha=g\circ f$ is an automorphism of $P$ (Prop. 8). Put $\widetilde f=f\circ\alpha^{-1}$.

We have

$$
\operatorname{Im}\widetilde f=\operatorname{Im}f
\quad\text{and}\quad
g\circ\widetilde f=1_P,
$$

which shows that $P'=\operatorname{Im}\widetilde f\oplus\operatorname{Ker}g$. Since the sequence

$$
0\longrightarrow\operatorname{Ker}g\longrightarrow P'
\xrightarrow{\ g\ }P\longrightarrow0
$$

is exact and $g$ is a homomorphism, $\operatorname{Ker}g$ has zero homology.

#### Proposition 9 {#alg-x-s3-prop-9 .statement}

*Let $M$ be an $A$-module and $(P,p)$ a projective resolution of $M$. Let $r$ denote the radical of $A$. Suppose either that $P_n$ is a finitely generated $A$-module for every $n$, or that $r$ is nilpotent. Then a necessary and sufficient condition for $(P,p)$ to be minimal is that the complex $(A/r)\otimes_A P$ have zero differential, in other words that*

$$
d_{n+1}(P_{n+1})\subset rP_n\quad\text{for all }n\geq0.
$$

Suppose that $(P,p)$ is minimal. By VIII, *loc. cit.*, the homomorphism

$$
1\otimes\delta_n:(A/r)\otimes_A P_n\longrightarrow(A/r)\otimes_A\operatorname{Im}d_n
$$

is an isomorphism. It then follows from the exact sequence

$$
0\longrightarrow\operatorname{Im}d_{n+1}
\xrightarrow{\ j_n\ }P_n
\xrightarrow{\ \delta_n\ }\operatorname{Im}d_n
\longrightarrow0
$$

that the homomorphism $1 \otimes j_n : (A/r) \otimes_A \operatorname{Im} d_{n+1} \to (A/r) \otimes_A P_n$ is zero; since $d_{n+1} = j_n \circ \delta_{n+1}$, we deduce that $1_{A/r} \otimes d_{n+1} = 0$ for $n \geqslant 0$.

Conversely, suppose that for every $n \geqslant 1$, $1 \otimes d_n$ is zero, in other words that $\operatorname{Im} d_n = \operatorname{Ker} d_{n-1}$ is contained in $rP_{n-1}$. Since $\delta_{n-1}$ is surjective, it follows from VIII, loc. cit. that $\delta_{n-1}$ is a projective cover for $n \geqslant 1$, hence that $(P, p)$ is minimal.

#### Proposition 10 {#alg-x-s3-prop-10 .statement}

*Suppose that A is a left noetherian local ring, and let M be a finitely generated A-module. Then M possesses a minimal resolution $(P, p)$; for every $n \geqslant 0$, $P_n$ is a finitely generated free module.*

In fact, in the construction carried out in No. 5 (p. 53), one may, by virtue of VIII, loc. cit., take for $(L_0, p)$ a projective cover of M, and for $L_{n+1}$ a projective cover of $\operatorname{Ker} d_n$. The resolution thus obtained is then minimal.

*Remarks. -- 1) Let m denote the maximal ideal of A and put $k = A/m$. Let P be a minimal projective resolution of M, and put $b_n = \dim_k (k \otimes_A P_n)$. Then $P_n$ is a free A-module of rank $b_n$. It follows from the corollary to Prop. 8 that for every other projective resolution $P'$ of M, one has $\dim_k (k \otimes_A P'_n) \geqslant b_n$, and that equality holds if and only if $P'$ is minimal.

2) By Prop. 9, $b_n$ is the dimension over $k$ of $H_n(k \otimes_A P)$, *in other words of $\operatorname{Tor}_n^A(k, M)$*. It is also the dimension over $k$ of $\operatorname{Ext}_A^n(M, k)$ (*cf. X, p. 103, Remark 3*).

### 7. Graded Resolutions

In this number, it is assumed that the ring A is endowed with a grading $(A_n)_{n \in \mathbf{Z}}$, such that $A_n = 0$ for $n < 0$. A graded A-module M is said to be *bounded below* if $M_n = 0$ for $n$ sufficiently small; every graded A-module of finite type is bounded below.

#### Proposition 11 {#alg-x-s3-prop-11 .statement}

*If M is a graded A-module bounded below (resp. if M is a graded A-module of finite type and if A is left noetherian), there exists an exact sequence of graded A-modules unbounded to the left*

$$
\cdots \longrightarrow L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_1 \xrightarrow{d_1} L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

*in which the $L_i$ are graded free and bounded below (resp. graded free and of finite type), and in which the $d_i$ are graded homomorphisms of degree 0.*

If N is a graded A-module bounded below (resp. and of finite type over noetherian A), there exists a graded free A-module bounded below (resp. and of finite type) L and a surjective graded homomorphism $L \to N$ (II, p. 167, *Remark 3*).

This being so, suppose given an exact sequence of graded A-modules and graded homomorphisms of degree 0

$$
L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0,
$$

where the $L_i, i = 0, \ldots, n$, are graded free and bounded below (resp. graded free and of finite type). Then $N = \mathrm{Ker}\, d_n$ is bounded below (resp. of finite type); hence there exist a graded free a-module bounded below (resp. a graded free a-module of finite type) $L_{n+1}$ and a graded homomorphism $d_{n+1} : L_{n+1} \to L_n$ of degree 0, such that $\mathrm{Im}\, d_{n+1} = N$; the sequence

$$
L_{n+1} \xrightarrow{d_{n+1}} L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

is then exact. The proposition then follows from the preceding by induction on $n$.

### 8. The standard resolution

In this No., it is supposed that the ring $A$ is an algebra (associative and unitary) over a commutative ring $k$. For $n \geqslant 0$, let $B_n$ denote the tensor product over $k$ of $(n + 2)$ modules equal to $A$. It is considered as an $(A, A)$-bimodule by endowing it with the structure of left a-module (resp right) deduced from the structure of left a-module (resp right) of the first (resp. of the last) factor of the tensor product.

For $n \geqslant 1$, define bimodule homomorphisms $d_n^i$ (for $0 \leqslant i \leqslant n$) and $d_n$ from $B_n$ into $B_{n-1}$ by the formulas:

$$
d_n^i(x_0 \otimes \ldots \otimes x_{n+1}) = x_0 \otimes \ldots \otimes x_i\, x_{i+1} \otimes \ldots \otimes x_{n+1}, \quad 0 \leqslant i \leqslant n,
$$
$$
d_n = \sum_{i=0}^n (-1)^i d_n^i.
$$

It is clear that
$$
d_{n-1}^i \circ d_n^j = d_{n-1}^{j-1} \circ d_n^i \quad \text{for} \quad i < j
$$
and consequently
$$
d_{n-1} \circ d_n = \sum_{0 \leqslant i < j \leqslant n} (-1)^{i+j} d_{n-1}^i \circ d_n^j + \sum_{0 \leqslant j \leqslant i \leqslant n-1} (-1)^{i+j} d_{n-1}^i \circ d_n^j = 0.
$$

Consequently, if one puts $B_n = 0$ for $n < 0$ and $d_n = 0$ for $n \leqslant 0$, the sequence $(B_n, d_n)$ defines a complex of $(A, A)$-bimodules (X, p. 43), which will be denoted by $B(A)$. For every left a-module $M$, let $B(A, M)$ denote the complex formed by the $B_n \otimes_A M$ and the $d_n \otimes 1_M$, \* in other words the tensor product complex $B(A) \otimes_A M *$; it is a complex of left a-modules.

Define an a-linear mapping $\varepsilon_M$ from $B_0(A, M) = (A \otimes_k A) \otimes_A M$ into $M$ by the formula $\varepsilon_M(a \otimes b \otimes m) = abm$ for $a, b \in A, m \in M$. One has $\varepsilon_M \circ d_1 = 0$, so that the graded homomorphism $\overline{\varepsilon}_M : B(A, M) \to M$, which coincides with $\varepsilon_M$ in degree 0, is a morphism of complexes of a-modules.

#### Proposition 12 {#alg-x-s3-prop-12 .statement}

The mapping $\overline{\varepsilon}_M : B(A, M) \to M$ is a homotopism of complexes of $k$-modules. In particular, the complex $B(A, M)$ is split over $k$, and $(B(A, M), \overline{\varepsilon}_M)$ is a left resolution of the $A$-module $M$.

For $n \geqslant 0$, let us define a $k$-linear mapping $s_n : B_n \to B_{n+1}$ by the formula:

$$
s_n(x_0 \otimes \ldots \otimes x_{n+1}) = 1 \otimes x_0 \otimes \ldots \otimes x_{n+1} \quad \text{for } x_0, \ldots, x_{n+1} \in A .
$$

This is a homomorphism of right $A$-modules, which satisfies the identities:

$$
d_{n+1}^i \circ s_n = s_{n-1} \circ d_n^{i-1} \quad \text{for } n \geqslant 1 , \quad 1 \leqslant i \leqslant n + 1 ,
$$
$$
d_{n+1}^0 \circ s_n = 1_{B_n} \qquad \text{for } n \geqslant 1 ,
$$

and consequently one has

(16)
$$
d_{n+1} \circ s_n + s_{n-1} \circ d_n = 1_{B_n} \quad \text{for } n \geqslant 1 .
$$

Moreover, one has

(17)
$$
d_1 \circ s_0(x_0 \otimes x_1) = x_0 \otimes x_1 - 1 \otimes x_0 x_1 \quad \text{for } x_0, x_1 \in A .
$$

Let $\eta : A \to A \otimes_k A$ denote the mapping defined by $\eta(a) = 1 \otimes a$, and $\overline{\eta} : A \to B(A)$ the morphism of complexes which coincides with $\eta$ in degree 0. It is clear that $\overline{\varepsilon}_A \circ \overline{\eta} = 1_A$; formulas (16) and (17) show that $d \circ s + s \circ d = 1_{B(A)} - \overline{\eta} \circ \overline{\varepsilon}_A$. Putting $\overline{\eta}_M = \overline{\eta} \otimes 1_M$, $d_M = d \otimes 1_M$ and $s_M = s \otimes 1_M$, we deduce that $\overline{\varepsilon}_M \circ \overline{\eta}_M = 1_M$ and $d_M \circ s_M + s_M \circ d_M = 1_{B(A,M)} - \overline{\eta}_M \circ \overline{\varepsilon}_M$. In other words, (X, p. 33, Definition 5), $\overline{\varepsilon}_M$ is a homotopism of complexes of $k$-modules. The other assertions of the proposition follow from this at once.

#### Definition 3 {#alg-x-s3-def-3 .statement}

The left resolution $(B(A, M), \overline{\varepsilon}_M)$ of $M$ is called the standard resolution of the $A$-module $M$.

If $A$ and $M$ are projective $k$-modules (resp. free, resp. flat), the standard resolution $B(A, M)$ is a projective (resp. free, resp. flat) resolution of $M$.

### 9. Resolutions and Grothendieck groups

If $\mathcal{C}$ is a set of classes of $A$-modules, we shall say that a left resolution $(P, p)$ is bounded of type $\mathcal{C}$ if the complex $P$ is bounded of type $\mathcal{C}$ (X, p. 41).

#### Theorem 1 {#alg-x-s3-thm-1 .statement}

Let $\mathcal{C}_0$ and $\mathcal{C}$ be two additive and left exact sets of class of $A$-modules such that $\mathcal{C}_0 \subset \mathcal{C}$ and every $A$-module of type $\mathcal{C}$ possesses a bounded left resolution of type $\mathcal{C}_0$. Then the homomorphism $\alpha : K(\mathcal{C}_0) \to K(\mathcal{C})$ deduced from the inclusion of $\mathcal{C}_0$ in $\mathcal{C}$ is bijective; if $M$ is an $A$-module of type $\mathcal{C}$ and $P$ a bounded left resolution of $M$ of type $\mathcal{C}_0$, one has $\alpha^{-1}([M]_{\mathcal{C}}) = \chi_{\mathcal{C}_0}(P)$ (X, p. 41, example 6).

#### Lemma 4 {#alg-x-s3-lem-4 .statement}

Let $f : M' \to M$ be a homomorphism of $A$-modules of type $\mathcal{C}$, and $p : P \to M$ a bounded left resolution of $P$ of type $\mathcal{C}_0$. There exist a bounded left resolution $p' : P' \to M'$ of type $\mathcal{C}_0$ and a morphism of complexes $u : P' \to P$ such that $p \circ u = f \circ p'$.

Let us argue by induction on the length $n$ of $P$, the assertion being trivial when the latter is $< 0$. Consider the mapping $g : M' \times P_0 \to M$ such that

$$
g(x, r') = f(x) - p_0(r')
$$
for $x \in M', r' \in P_0$,

and its kernel $K$; the $A$-module $K$ is of type $\mathcal{C}$ since $g$ is surjective and $M' \times P_0$ and $M$ are of type $\mathcal{C}$. Let $h : P'_0 \to K$ be a surjective homomorphism, where $P'_0$ is of type $\mathcal{C}_0$; let us denote by $p'_0 : P'_0 \to M'$ (resp. $u_0 : P'_0 \to P_0$) the homomorphism composed of $h$ and the projection $K \to M$ (resp. $K \to P_0$); the homomorphism $p'_0$ is surjective and we have a commutative diagram

$$
\begin{array}{ccc}
P'_0 & \xrightarrow{u_0} & P_0 \\
p'_0 \downarrow & & \downarrow p_0 \\
M' & \xrightarrow{f} & M .
\end{array}
$$

It is then enough to apply the induction hypothesis to the homomorphism

$$
\operatorname{Ker} p'_0 \to \operatorname{Ker} p_0
$$

deduced from $u_0$.

#### Lemma 5 {#alg-x-s3-lem-5 .statement}

Consider a commutative diagram

$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \to M'' \to 0
\end{array}
$$

where $(P, p)$ (resp. $(P', p')$) is a left resolution of $M$ (resp. $M'$), and where the bottom horizontal line is an exact sequence. There exists a homologism $p'' : \operatorname{Con}(u) \to M''$.

In fact, the exact sequence (X, p. 37, prop. 7)

$$
0 \to P \xrightarrow{\pi} \operatorname{Con}(u) \xrightarrow{\delta} P'(-1) \to 0
$$

gives an exact homology sequence

$$
\to H_n(P) \to H_n(\operatorname{Con}(u)) \to H_{n-1}(P') \to \cdots
$$
$$
\cdots \to H_1(\operatorname{Con}(u)) \to H_0(P') \xrightarrow{\hat{\partial}} H_0(P) \to H_0(\operatorname{Con}(u)) \to 0 .
$$

By X, p. 38, lemma 3 a), we have $\partial = - H_0(u)$. Since $H_n(P) = 0 = H_n(P')$ for $n > 0$ and $H_0(u) : H_0(P') \to H_0(P)$ is identified with $f : M' \to M$, we conclude that $H_n(\operatorname{Con}(u)) = 0$ for $n > 0$ and that $H_0(\operatorname{Con}(u))$ is isomorphic to $M''$, whence the lemma.

Let us now prove the theorem.

a) Let M be an A-module of type $\mathcal{C}$. For every bounded left resolution $(P, p)$ of M of type $\mathcal{C}_0$, the element $\chi_{\mathcal{C}_0}(P)$ of $K(\mathcal{C}_0)$ depends only on M. In fact, let $(P_1, p_1)$ and $(P_2, p_2)$ be two resolutions of this type. Consider the resolution
$$
(P_1 \times P_2, p_1 \times p_2)
$$
of the A-module $M \times M$ and the homomorphism $\Delta : x \mapsto (x, x)$ of M into $M \times M$. By lemma 4, there exists a bounded left resolution $(Q, q)$ of M of type $\mathcal{C}_0$ and a commutative diagram
$$
\begin{array}{ccc}
Q & \xrightarrow{u} & P_1 \times P_2 \\
q \downarrow & & \downarrow p_1 \times p_2 \\
M & \xrightarrow{\Delta} & M \times M ;
\end{array}
$$
we deduce from this a commutative diagram
$$
\begin{array}{ccc}
Q & \xrightarrow{u \circ pr_i} & P_i \\
q \downarrow & & \downarrow p_i \\
M & \xrightarrow{1_M} & M , \quad i = 1, 2 .
\end{array}
$$
By lemma 5, Con $(u \circ pr_i)$ has zero homology, hence $u \circ pr_i$ is a homologism and $\chi_{\mathcal{C}_0}(Q) = \chi_{\mathcal{C}_0}(P_i)$ (X, p. 41, prop. 10); it follows that $\chi_{\mathcal{C}_0}(P_1) = \chi_{\mathcal{C}_0}(P_2)$ as announced.

b) For every A-module M of type $\mathcal{C}$, let $\varphi(M) \in K(\mathcal{C}_0)$ be the common value of the $\chi_{\mathcal{C}_0}(P)$ for all bounded left resolutions P of M of type $\mathcal{C}_0$. Let us show that the function $\varphi : \mathcal{C} \to K(\mathcal{C}_0)$ is additive. Let therefore
$$
0 \to M' \xrightarrow{f} M \to M'' \to 0
$$
be an exact sequence of A-modules of type $\mathcal{C}$. By Lemma 4, there exists a commutative diagram
$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \xrightarrow{g} M'' \to 0
\end{array}
$$
where $(P, p)$ and $(P', p')$ are bounded left resolutions of type $\mathcal{C}_0$. Then we have
$$
\varphi(M) = \chi_{\mathcal{C}_0}(P) , \qquad \varphi(M') = \chi_{\mathcal{C}_0}(P')
$$
and by Lemma 5
$$
\varphi(M'') = \chi_{\mathcal{C}_0}(\mathrm{Con}\,(u)) = \chi_{\mathcal{C}_0}(P) - \chi_{\mathcal{C}_0}(P') = \varphi(M) - \varphi(M') ;
$$
which was to be proved.

c) Let then $\beta : K(\mathscr{C}) \to K(\mathscr{C}_0)$ be the homomorphism such that, with the preceding notations, we have $\beta([M]_{\mathscr{C}})=\chi_{\mathscr{C}_0}(P)$. Since $p$ is a homomorphism, we have $\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$, hence $\alpha\circ\beta([M]_{\mathscr{C}})=\alpha(\chi_{\mathscr{C}_0}(P))=\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$ and $\alpha\circ\beta=1_{K(\mathscr{C})}$. If $M$ is of type $\mathscr{C}_0$, then $(M,1_M)$ is a resolution of $M$, hence $\varphi(M)=[M]_{\mathscr{C}_0}$ and $\beta\circ\alpha=1_{K(\mathscr{C}_0)}$, which completes the proof.

We shall apply this theorem to modules of "finite projective dimension" in § 8 (X, p. 137).

## EXERCISES {#alg-x-s3-exercises}

See the [exercises for § 3](exercises/s3/).
