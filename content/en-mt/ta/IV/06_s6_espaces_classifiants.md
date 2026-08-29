---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 6
section_title: Espaces classifiants
lang: en
source: ta-i-iv-fr
book_pages: TA IV.437-TA IV.454, TA IV.477-TA IV.480
pdf_pages: 0453-0470, 0493-0496
extraction: native
subsections:
    - "no": 1
      title: Prolongement des homotopies
      page: 437
      pdf_page: 453
    - "no": 2
      title: Espaces fibrés localement triviaux de base $B\times \mathbf{I}$
      page: 440
      pdf_page: 456
    - "no": 3
      title: Espaces fibrés principaux de base $B\times \mathbf{I}$
      page: 443
      pdf_page: 459
    - "no": 4
      title: Espaces fibrés universels
      page: 446
      pdf_page: 462
    - "no": 5
      title: Espace classifiant pour un groupe discret
      page: 449
      pdf_page: 465
statements: 32
exercises: 9
content_sha256: b015eaffc395a390ad89b5be3071d4a836f54b19acf3405ffc848c6477ed66de
translated_from: content/fr/ta/IV/06_s6_espaces_classifiants.md
source_lang: fr
translation_method: machine
source_content_sha256: 07449d365571676c544d1619988ed7e8c13e4b70374afbf038ed0d746cfaa9f5
translation_model: gpt-5.4
translation_run: translate-en-mt-56604f7a
glossary_version: 34
glossary_terms_sha256: cb58b1aad9e3fe796e60c0e37ca8b90b04a841672cf1a517f72151ea538ba0e4
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. CLASSIFYING SPACES

### 1. Extension of homotopies

#### Proposition 1 {#ta-iv-s6-prop-1 .statement tag=023V}

Let $X'$ be a normal topological space, let X be a subspace of $X'$, let A be a closed subspace of $X'$ contained in X, and let U be a neighbourhood of A in X.

Let us denote by $i_A$ the canonical injection of A into X$,i_U$ the canonical injection of U into X; let $j_A$ and $j_U$ denote the corresponding injections of Cyl($i_A$) and Cyl($i_U$) into $X\times \mathbf{I}$.

There exists a continuous mapping $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) such that $j_U\circ$ $r(x) =x$ for every point $x\in j_A$(Cyl($i_A$)).

Let $U'$ be an open set of $X'$ such that $A\subset X\cap U'\subset U$. By definition of a normal space (TG, IX, p. 41), there exists an open neighbourhood $V'$ of A in $X'$ such that $A\subset V'\subset \overline{V'}\subset U'$ and a continuous function $\varphi ': X'\rightarrow \mathbf{I}$ which is equal to 1 at every point of A and to 0 at every point of $\complement V'$. Put $\varphi =\varphi '|X$ and $V = X\cap V'$. Let us also denote by $\alpha : U\times \mathbf{I}\rightarrow$ Cyl($i_U$) and $\beta : X\rightarrow$ Cyl($i_U$) the canonical mappings (III, p. 238).

Let $r$ be the mapping of $X\times \mathbf{I}$ into Cyl($i_U$) defined by

$\alpha (x,1-(1-t)\varphi (x))$ for $(x, t)\in U\times \mathbf{I}$,

$$
r(x, t) =
$$

$\beta (x)$ otherwise.

The mapping $r$ is continuous on $U\times \mathbf{I}$. For every point $(x, t)\in U\times \mathbf{I}$ such that $x\notin V$, we have $\varphi (x) = 0$, whence $r(x, t) =\alpha (x,1) =\beta (x)$. It follows that the mappings $r$ and $\beta \circ$ pr$_1$ coincide on $(X-V)\times \mathbf{I}$, which implies that $r$ is continuous on this subspace. Since U and the interior of X-V cover X, the mapping $r$ is continuous.

Let $y$ be a point of Cyl($i_A$) ; put $(x, t) =j_A(y)$. If $x\in$ A, $\varphi (x) = 1$ and $r(x, t) =\alpha (x, t)$, whence $j_U(r(x, t)) = (x, t)$. Otherwise, $t= 1$ and one has $r(x, t) =\alpha (x,1)$ if $x\in U$ and $r(x, t) =\beta (x)$ otherwise ; hence $j_U(r(x, t)) = (x, t)$ in this case. This entails that $j_U\circ r$ maps every point of $j_A$(Cyl($i_A$)) to itself, whence the proposition.

#### Corollary 1 {#ta-iv-s6-prop-1-cor-1 .statement tag=023W}

Let X be a normal topological space, let $f$ be a continuous mapping of X into a topological space Z. Let A be a closed subspace of X, let U be a neighbourhood of A in X and let $\sigma : U\times$ $\mathbf{I}\rightarrow Z$ be a homotopy whose term is the mapping $f|U$. There exists a homotopy $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ whose term is the mapping $f$ and which coincides with $\sigma$ in $A\times \mathbf{I}$.

Put $X'= X$ and let $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) be the continuous mapping given by Prop. 1. With the notations introduced in the proof of this proposition, there exists a unique continuous mapping F: Cyl($i_U$)$\rightarrow Z$ such that $F(\alpha (x, t)) =\sigma (x, t)$ for $(x, t)\in U\times \mathbf{I}$ and $F(\beta (x)) =f(x)$ for $x\in$ X (III, p. 238, Prop. 4). The mapping $F\circ r: X\times \mathbf{I}\rightarrow$ Z is a homotopy ; its term maps a point $x\in$ X to $F(r(x,1)) = F(\beta (x)) =f(x)$. If $(x, t)\in A\times \mathbf{I}$, $F(r(x, t)) = F(\alpha (x, t)) =\sigma (x, t)$, therefore this homotopy coincides with $\sigma$ on $A\times \mathbf{I}$.

#### Corollary 2 {#ta-iv-s6-prop-1-cor-2 .statement tag=023X}

Let X be a normal topological space, let A be a closed subspace of X and let U be a neighbourhood of A in X. Let $f$ and $f'$ be continuous homotopic mappings of U into a topological space Z. If $f$ possesses a continuous extension to X, the same is true of the mapping $f'|A$.

Let F be a continuous mapping of X into Z such that $F|U =f$. Let us choose a homotopy $\sigma : A\times \mathbf{I}\rightarrow Z$ joining $f'$ to $f$. By Cor. 1, there exists a homotopy $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ with term F which extends $\sigma$. The origin of $\widetilde{\sigma}$ is then a continuous mapping of X into Z which coincides with $f'$ on A.

#### Corollary 3 {#ta-iv-s6-prop-1-cor-3 .statement tag=023Y}

Let X be a normal topological space, let A be a closed subspace of X and let U be a neighbourhood of A in X. Let Z be a topological space homotopic to a point and let $g: U\rightarrow$ Z be a continuous mapping. There exists a continuous mapping $\widetilde{g}: X\rightarrow Z$ which coincides with $g$ on A.

Since Z is homotopic to a point, the mapping $g$ is homotopic to a constant mapping $f$. The mapping $f$ extends continuously to X ; the assertion therefore follows from Cor. 2.

#### Corollary 4 {#ta-iv-s6-prop-1-cor-4 .statement tag=023Z}

Let X be a paracompact topological space, let A be a closed subspace of X. Let $n$ be an integer $\geqslant 0$ and let V be an open subset of $\mathbf{R}^n$. Let $f: X\rightarrow V$ be a continuous mapping and let $\sigma : A\times \mathbf{I}\rightarrow V$ be a homotopy with terminal map $f|A$. There exists a homotopy $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ with terminal map $f$ which extends $\sigma$.

Let us denote by $i_A$ the canonical injection of A into X, by $\alpha_A: A\times \mathbf{I}\rightarrow$ Cyl($i_A$) and $\beta_A: X\rightarrow$ Cyl($i_A$) the canonical mappings, and also by $j_A:$ Cyl($i_A$)$\rightarrow$ $X\times \mathbf{I}$ the canonical injection. Since A is closed in X, $j_A$ defines a homeomorphism of Cyl($i_A$) onto the closed subspace $(A\times \mathbf{I})\cup (X\times \{1\})$ of $X\times \mathbf{I}$. Let $\widetilde{\sigma}_0$ be the unique mapping of Cyl($i_A$) into V such that $\widetilde{\sigma}_0\circ \alpha_A=\sigma$ and $\widetilde{\sigma}_0\circ \beta_A=f$; it is continuous (III, p. 238, prop. 4).

Since X is paracompact and $\mathbf{I}$ is compact, the space $X\times \mathbf{I}$ is paracompact (TG, I, p. 70, prop. 17), hence normal (TG, IX, p. 49, prop. 4). There therefore exists a continuous mapping $k: X\times \mathbf{I}\rightarrow \mathbf{R}^n$ such that $k\circ j_A=\widetilde{\sigma}_0$ (TG, IX, p. 45, corollary).

The set U of points $x\in$ X such that $k(x, t)\in$ V for all $t\in \mathbf{I}$ is open in X (IV, p. 439, lemma 1). Hence it is a neighbourhood of A. By corollary 1, applied to the mapping $f$ and to the homotopy $k|U\times \mathbf{I}$, there exists a homotopy $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ with initial map $f$ which coincides with $k$, hence with $\sigma$, on $A\times \mathbf{I}$.

#### Lemma 1 {#ta-iv-s6-lem-1 .statement tag=0240}

Let Z be a topological space, K a compact topological space and W an open subset of $Z\times K$. The set U of points $z\in Z$ such that $\{z\} \times K$ is contained in W is open in Z.

The first projection pr$_1: Z\times K\rightarrow Z$ is proper (TG, I, p. 77, cor. 5), hence closed. Consequently, $\complement U =$ pr$_1(\complement W)$ is closed in Z and U is open.

#### Corollary 5 {#ta-iv-s6-lem-1-cor-5 .statement tag=0241}

Let $X'$ be a normal topological space, let X be a subspace of $X'$, let A be a closed subspace of $X'$ contained in X, and let U be a neighbourhood of A in X.

Let Y and Z be topological spaces; let $f: X\times  \{1\} \times Y\rightarrow$ $X\times  \{1\} \times Z$ be an $X\times  \{1\}$-morphism and let $g: U\times \mathbf{I}\times Y\rightarrow U\times \mathbf{I}\times Z$ be a $U\times \mathbf{I}$-morphism which coincides with $f$ on $U\times  \{1\} \times Y$.

There then exists an $X\times \mathbf{I}$-morphism $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ which coincides with $f$ on $X\times  \{1\} \times Y$ and with $g$ on $A\times \mathbf{I}\times Y$.

Moreover, if $f$ and $g$ are homeomorphisms, one can choose a homeomorphism $h$ having the required properties.

Let $U'$ be an open neighbourhood of A in $X'$ such that $U'\cap X\subset U$. Since the space $X'$ is normal, there exists an open neighbourhood $V'$ of A in $X'$ such that $A\subset V'\subset \overline{V'}\subset U'$ (TG, IX, p. 41). Replacing U by $\overline{V'}\cap X$ if necessary, we may thus suppose that U is closed in X. Let us then take up again the notation of Prop. 1 and of its proof; let $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) be a continuous mapping such that $j_U\circ r(x) =x$ for every point $x\in j_A$(Cyl($i_A$)).

Put also $f'=$ pr$_3\circ f$ and $g'=$ pr$_3\circ g$. Since $f'$ and $g'$ coincide on $U\times  \{1\} \times Y$, there exists a unique mapping

$\varphi :$ Cyl($i_U$)$\times Y\rightarrow$ Cyl($i_U$)$\times Z$

such that $\varphi (\alpha (x, t), y) = (\alpha (x, t), g'(x, t, y))$ for $(x, t, y)\in U\times \mathbf{I}\times Y$ and $\varphi (\beta (x), y) = (\beta (x), f'(x,1, y))$ for $(x, y)\in X\times Y$. Since U is closed in X, the canonical surjection $\pi$ of $(U\times \mathbf{I})\cup X$ onto Cyl($i_U$) is universally strict (III, p. 239, remark 2). Since the mapping $\varphi \circ (\pi \times$ Id$_Y)$ is continuous, the mapping $\varphi$ is continuous. It is therefore a morphism of Cyl($i_U$)-spaces, and even an isomorphism if $f$ and $g$ are homeomorphisms.

Let then $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ be the mapping $r^*(\varphi )$ deduced from $\varphi$ by the base change $r$. It is given by $h(x, t, y) =$ $(x, t$, pr$_2(\varphi (r(x, t), y)))$ for $(x, t, y)\in X\times \mathbf{I}\times Y$. It is a morphism of $X\times \mathbf{I}$-spaces, and even an isomorphism if $\varphi$ is one. For $(x, t, y)\in$ $A\times \mathbf{I}\times Y$, one has $r(x, t) = (x, t)$, whence

$h(x, t, y) = (x, t$, pr$_2(\varphi (x, t, y))) = (x, t, g'(x, t, y)) =g(x, t, y)$,

which proves that $h$ coincides with $g$ on $A\times \mathbf{I}\times Y$. Analogously, for $x\in X$ and $y\in Y$, we have $r(x,1) = (x,1)$, hence

$h(x,1, y) = (x,1$, pr$_2(\varphi (x,1, y))) = (x,1, f'(x,1, y)) =f(x,1, y)$

so that $h$ coincides with $f$ on $X\times  \{1\} \times Y$. The corollary is thus proved.

### 2. Locally trivial fibre spaces with base $B\times \mathbf{I}$

#### Proposition 2 {#ta-iv-s6-prop-2 .statement tag=0242}

Let B be a paracompact topological space and let $(E, p)$ be a locally trivial fibre space over $B\times \mathbf{I}$. Put $E_1=\overset{-1}{p}(B\times \{1\})$ and denote by $p_1: E_1\rightarrow B$ the mapping pr$_1\circ p|E_1$. Then the $B\times \mathbf{I}$-spaces $(E, p)$ and $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ are isomorphic.

Let us first prove two lemmas.

#### Lemma 2 {#ta-iv-s6-lem-2 .statement tag=0243}

Let $\alpha ,\beta ,\gamma$ be real numbers such that $\alpha \leqslant \beta \leqslant \gamma$, let B be a topological space and let $p: E\rightarrow B\times [\alpha , \gamma ]$ be a continuous mapping. Put $B_0= B\times [\alpha , \beta ]$, $B_1= B\times [\beta , \gamma ]$, $E_0=\overset{-1}{p}(B_0)$, $E_1=$ $\overset{-1}{p}(B_1)$ and denote by $p_0: E_0\rightarrow B_0,p_1: E_1\rightarrow B_1$ the mappings deduced from $p$. If $(E_0, p_0)$ and $(E_1, p_1)$ are trivializable fibre spaces, the same is true of $(E, p)$.

Let $g_0: E_0\rightarrow B_0\times F_0$ and $g_1: E_1\rightarrow B_1\times F_1$ be trivializations of $E_0$ and $E_1$ respectively. Let $g'_0$ and $g'_1$ denote the trivializations of the $B\times  \{\beta \}$-fibered space $\overset{-1}{p}(B\times  \{\beta \})$ deduced from $g_0$ and $g_1$ by restriction. The mapping $h=g'_0\circ (g'_1)^{-1}$ is a $B\times  \{\beta \}$-isomorphism of $B\times  \{\beta \} \times F_1$ onto $B\times  \{\beta \} \times F_0$. Define a continuous mapping $h'$ of $B\times F_1$ into $F_0$ by putting $h'(a, y) =$ pr$_3\circ h(a, \beta , y)$ for $(a, y)\in B\times F_1$. For $(a, t, y)\in B\times [\beta , \gamma ]\times F_1$, put $H(a, t, y) = (a, t, h'(a, y))$. The mapping H resulting is a $(B\times [\beta , \gamma ])$-isomorphism of $B\times [\beta , \gamma ]\times F_1$ onto $B\times [\beta , \gamma ]\times F_0$, and one has $g_0|\overset{-1}{p}(B\times  \{\beta \}) = H\circ g_1|\overset{-1}{p}(B\times  \{\beta \})$. There therefore exists a continuous mapping $g: E\rightarrow B\times [\alpha , \gamma ]\times F_0$ such that $g|E_0=g_0$ and $g|E_1= H\circ g_1$. The mapping $g$ is an isomorphism of $B\times [\alpha , \gamma ]$-spaces, hence E is trivializable.

#### Lemma 3 {#ta-iv-s6-lem-3 .statement tag=0244}

Let B be a topological space and let $(E, p)$ be a locally trivial $B\times \mathbf{I}$-fibered space. Every point $a$ of B possesses a neighbourhood V such that the $V\times \mathbf{I}$-space $E_{V\times\mathbf{I}}$ is trivializable.

Let $a$ be a point of B; for every point $t$ of $\mathbf{I}$, there exists an open neighbourhood $W_t$ of $t$ in $\mathbf{I}$ and a neighbourhood $V_t$ of $a$ in B such that E is trivializable over $V_t\times W_t$. There then exist an integer $n >0$ and, for every integer $i$ such that 1 $\leqslant i\leqslant n$, a point $t_i$ of $\mathbf{I}$ such that the interval $[\frac{i-1}{n},\frac{i}{n}]$ is contained in $W_{t_i}($III, p. 272, lemma 4). Put $V =\cap_{1\leqslant i\leqslant n}V_{t_i}$. The fibered space E is trivializable over $V\times$ $[\frac{i-1}{n},\frac{i}{n}]$ for every integer $i$ such that $1\leqslant i\leqslant n$. Lemma 3 then follows from Lemma 2 by induction on $n$.

Let us now prove the proposition. By lemma 3, there exists an open covering $(U_j)_{j\in J}$ of B such that, for every $j\in J$, E is trivializable over $U_j\times \mathbf{I}$. Since the space B is paracompact, we may suppose the covering $(U_j)_{j\in J}$ locally finite (TG, IX, p. 49) and choose a covering $(A_j)_{j\in J}$ of B where, for every $j\in J$, the set $A_j$ is closed in B and contained in $U_j$ (TG, IX, p. 49, prop. 4 and p. 48, cor. 1).

For every open subset U of B, let us denote by $\mathscr{F}(U)$ the set of $U\times \mathbf{I}$-isomorphisms of $\overset{-1}{p}(U\times \mathbf{I})$ onto $\overset{-1}{p_{1}}(U)\times \mathbf{I}$ which induce the identical mapping of $\overset{-1}{p}(U\times  \{1\})$ onto $\overset{-1}{p_{1}}(U)\times  \{1\}$. For every pair $(V,U)$ of open sets of B such that $U\subset V$, let us denote by $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ the mapping which, to a $(V\times \mathbf{I})$-isomorphism $g:\overset{-1}{p}(V\times \mathbf{I})\rightarrow \overset{-1}{p_{0}}(V)\times \mathbf{I}$, associates the $(U\times \mathbf{I})$-isomorphism deduced from $g$ by passing to the subspaces. The pair $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ is a sheaf on B (I, p. 45, example 4). To prove the proposition, it is enough to prove that the sheaf $\mathscr{F}$ is soft (I, p. 64).

Let $j\in J$, let A be a closed subset of $A_j$, let V be an open set in B such that $A\subset V\subset U_j$, and let $g$ be an element of $\mathscr{F}(V)$. There exists an open neighbourhood W of A such that $\overline{W}\subset V$, for a paracompact space is normal (TG, IX, p. 49, prop. 4). We shall prove that there exists an element $g'$ of $\mathscr{F}(U_j)$ such that $g'|W =g|W$. Corollary 2 (I, p. 65) of prop. 6 then implies that the sheaf $\mathscr{F}$ is soft.

Since the $B\times \mathbf{I}$-space E is trivializable over $U_j\times \mathbf{I}$, we may suppose that $\overset{-1}{p}(U_j\times \mathbf{I}) = U_j\times \mathbf{I}\times F$, where F is a topological space. The element $g$ of $\mathscr{F}(V)$ is then a $V\times \mathbf{I}$-isomorphism of $V\times \mathbf{I}\times F$ onto itself which induces the identical mapping of $V\times$ $\{1\}\times F$. Apply cor. 5 of IV, p. 439, to the spaces $X'= X$, $X = U_j$, A = W, U = V, and Y = Z = F, to the mapping $g: V\times \mathbf{I}\times F\rightarrow V\times \mathbf{I}\times F$ and to the identical mapping of $U_j\times  \{1\} \times F$. There therefore exists a $U_j\times \mathbf{I}$-isomorphism $g'$ of $U_j\times \mathbf{I}\times F$ onto itself which induces the identical mapping of $U_j\times  \{1\} \times F$ and which coincides with $g$ on $\overline{W}\times \mathbf{I}\times F$, and a fortiori on $W\times \mathbf{I}\times F$. Hence the proposition.

#### Corollary 1 {#ta-iv-s6-lem-3-cor-1 .statement tag=0245}

Let B be a paracompact topological space and let $(E, p)$ be a locally trivial fibre space over $B\times \mathbf{I}$ (I, p. 71, Corollary 2). For $t\in \mathbf{I}$, let us denote by $(E_t, p_t)$ the locally trivial fibre space over B $i^*_tE$, where $i_t: B\rightarrow B\times  \{t\}$ is the mapping $b\mapsto (b, t)$. The locally trivial fibre spaces over B $E_0$ and $E_t$ are isomorphic for every $t\in \mathbf{I}$.

#### Corollary 2 {#ta-iv-s6-lem-3-cor-2 .statement tag=0246}

Let B and $B'$ be topological spaces, and let E be a locally trivial fibre space over B. Let $f_0$ and $f_1$ be continuous mappings of $B'$ into B. Suppose that the space $B'$ is paracompact. If the mappings $f_0$ and $f_1$ are homotopic, the locally trivial fibre spaces over $B'$ $f_0^*E$ and $f_1^*E$ are isomorphic.

Let $\sigma : B'\times \mathbf{I}\rightarrow B$ be a homotopy joining $f_0$ to $f_1$ and let us denote by $E'$ the space over $B'\times \mathbf{I}$ $\sigma^*E$; this is a locally trivial fibre space. Let us denote by $i_0$ and $i_1$ the mappings of $B'$ into $B'\times \mathbf{I}$ given by $x\mapsto (x,0)$ and $x\mapsto (x,1)$. By Cor. 1, the fibre spaces over $B'$ $i^*_0E'$ and $i^*_1E'$ are isomorphic. Since $\sigma \circ i_0=f_0$, the space over $B'$ $i^*_0E'$ is identified with $f_0^*E$; analogously, the space over $B'$ $i^*_1E'$ is identified with $f_1^*E$. Consequently, the fibre spaces over $B'$ $f_0^*E$ and $f_1^*E$ are isomorphic, as was to be proved.

#### Corollary 3 {#ta-iv-s6-lem-3-cor-3 .statement tag=0247}

Let B be a paracompact topological space. If B is homotopic to a point, every locally trivial fibre space with base B is trivializable.

#### Corollary 4 {#ta-iv-s6-lem-3-cor-4 .statement tag=0248}

Let B and $B'$ be topological spaces, let $(E, p)$ be a locally trivial fibre space over B, let $f$ be a continuous mapping of $B'$ into B, let $\sigma : B'\times \mathbf{I}\rightarrow B$ be a homotopy starting from $f$, and let $\widetilde{f}$ be a continuous lifting of $f$ to E. If the space $B'$ is paracompact, there exists a homotopy $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow E$ starting from $\widetilde{f}$ which is a lifting of $\sigma$ to E.

Let $(E', p')$ be the $B'\times \mathbf{I}$-space deduced from $(E, p)$ by base change by the mapping $\sigma : B'\times \mathbf{I}\rightarrow B$. It is a locally trivial fibre space (I, p. 71, Corollary 2), and the mapping $s: B'\times  \{0\} \rightarrow E'$ defined by $s((a,0)) = ((a,0),\widetilde{f}(a))$ for $a\in B'$ is a continuous section of $p'$ over $B'\times  \{0\}$. By Proposition 2, there exists a continuous section $\widetilde{s}$ of $p'$ extending $s$. The mapping $\widetilde{\sigma}=$ pr$_2\circ \widetilde{s}$ has the required property.

### 3. Principal fibre spaces with base $B\times \mathbf{I}$

Let G be a topological group. We shall see that Proposition 2 and its corollaries remain valid when, in each statement, one replaces “locally trivial fibre space” by “principal fibre space with group G”.

#### Lemma 4 {#ta-iv-s6-lem-4 .statement tag=0249}

Let B be a topological space, let G be a topological group and let E, $E'$ be principal fibre spaces with group G and base B. Let F denote the topological space G endowed with the left operation of $G\times G$ given by $(g, g')\cdot f=g'f g^{-1}$, and let $M = (E\times_BE')\times^{G\times G}F$ denote the locally trivial fibre space with fibre type F and base B associated with it.

The sheaf $\mathscr{S}$ on B of sections of M is isomorphic to the sheaf on B of isomorphisms of principal fibre spaces from E onto $E'$.

Let us denote by $p,p'$ and $q$ the projections of the B-spaces E, $E'$ and M. For $(x, x')\in E\times_BE'$ and $f\in F$, let $[x, x', f]$ denote the class in M of the element $((x, x'), f)\in (E\times_BE')\times F$. Let $\mathscr{M}$ denote the sheaf on B of isomorphisms of principal fibre spaces from E onto $E'$; its sections over an open set U of B are the isomorphisms of principal fibre spaces from $E_U$ onto $E'_U$.

Let $e$ denote the identity element of G. Let U be an open set of B and let $\varphi : E_U\rightarrow E'_U$ be an isomorphism of principal fibre spaces with group G and base U. The mapping from $E_U$ into $(E\times_BE')\times^{G\times G}F$ defined by $x\mapsto [x, \varphi (x), e]$ is continuous. For $g\in G$ and $x\in E_U$, it sends $x\cdot g$ to $[x\cdot g, \varphi (x\cdot g), e] = [x, \varphi (x), geg^{-1}] = [x, \varphi (x), e]$. There therefore exists a unique continuous mapping $\alpha_U(\varphi ): U\rightarrow M$ such that $\alpha_U(\varphi )(p(x)) = [x, \varphi (x), e]$ for every $x\in E_U$; we have $\alpha_U(\varphi )\in \mathscr{S}(U)$.

It is immediate that the mappings $\alpha_U$ define a morphism of sheaves $\alpha$ from $\mathscr{M}$ into $\mathscr{S}$.

#### Lemma 5 {#ta-iv-s6-lem-5 .statement tag=024A}

The morphism of sheaves $\alpha$ is an isomorphism.

Suppose first that the principal fibre spaces E and $E'$ are both trivializable; choose sections $i: B\rightarrow E$ and $i': B\rightarrow E'$ of them. Then there exists a unique continuous mapping $\theta$ from M into $B\times G$ such that one has

$$
\theta ([i(b)\cdot g, i'(b)\cdot g', f]) = (b, g'f g^{-1})
$$

for $b\in B,g\in G,g'\in G$ and $f\in$ F; it is an isomorphism of B-spaces. Let $\varphi$ be an isomorphism of principal fibre spaces from E onto $E'$; there exists a unique continuous mapping $\gamma : B\rightarrow G$ such that $\varphi (i(b)) =i'(b)\cdot \gamma (b)$ for $b\in B$. The image of $\varphi$ under the mapping $\alpha_B$ is the mapping $b\mapsto \theta^{-1}(b, \gamma (b))$ from B into M. This implies that $\alpha_B$ is a bijection.

Consequently, $\alpha_U$ is a bijection for every open set U of B such that the principal fibre spaces $E_U$ and $E'_U$ are trivializable. By corollary 2 of I, p. 55, this implies that $\alpha$ is an isomorphism of sheaves.

#### Proposition 3 {#ta-iv-s6-prop-3 .statement tag=024B}

Let G be a topological group, let B be a paracompact topological space and let $(E, p)$ be a principal fibre space of group G and base $B\times \mathbf{I}$. Put $E_1=\overset{-1}{p}(B\times \{1\})$ and let $p_1: E_0\rightarrow B$ be the mapping pr$_1\circ p|E_1$. Then, $(E, p)$ and $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ are isomorphic principal fibre spaces of group G and base $B\times \mathbf{I}$.

Let F be the topological space G endowed with the left operation of the group $G\times G$ given by $(g, g')\cdot f=g'f g^{-1}$. Let $(M, q)$ be the locally trivial fibre space of base $B\times \mathbf{I}$ and fibre type F associated with the principal fibre space $E\times_{B\times\mathbf{I}}(E_1\times \mathbf{I})$ of group $G\times G$. Put $M_1=\overset{-1}{q}(B\times \{1\})$ and $q_1=$ pr$_1\circ p|M_1$; the B-space $(M_1, q_1)$ is identified with the locally trivial fibre space of fibre type F associated with $E_1\times_BE_1$. By lemma 4, where one takes for principal fibre spaces E and $E'$ both equal to $E_1$, the B-space $M_1$ has a section. Since the $B\times \mathbf{I}$-spaces $(M, q)$ and $(M_1\times \mathbf{I}, q_1\times$Id$_{\mathbf{I}})$ are isomorphic (IV, p. 440, prop. 2), the $B\times \mathbf{I}$-space $(M, q)$ has a section, which implies that the principal fibre spaces of group G, E and $E_1\times \mathbf{I}$, are isomorphic.

#### Corollary 1 {#ta-iv-s6-prop-3-cor-1 .statement tag=024C}

Let B be a paracompact topological space, let G be a topological group and let $(E, p)$ be a principal fibre $B\times \mathbf{I}$-space of group G. For $t\in \mathbf{I}$, let $(E_t, p_t)$ denote the principal fibre B-space $i^*_tE$, where $i_t: B\rightarrow B\times  \{t\}$ is the mapping $b\mapsto (b, t)$. The principal fibre B-spaces $E_0$ and $E_t$ are isomorphic for every $t\in \mathbf{I}$.

#### Corollary 2 {#ta-iv-s6-prop-3-cor-2 .statement tag=024D}

Let B and $B'$ be topological spaces, let G be a topological group, and let E be a B-principal fibre space with group G. Let $f_0$ and $f_1$ be continuous mappings of $B'$ into B. Suppose that the space $B'$ is paracompact. If the mappings $f_0$ and $f_1$ are homotopic, the $B'$-principal fibre spaces $f_0^*E$ and $f_1^*E$ are isomorphic.

#### Corollary 3 {#ta-iv-s6-prop-3-cor-3 .statement tag=024E}

Let B be a paracompact topological space and let G be a topological group. If B is homotopic to a point, every principal fibre space with group G is trivialisable.

#### Remark {#ta-iv-s6-n3-rem-1 .statement tag=024F}

An alternative proof of these results would consist in verifying that the isomorphisms of fibre spaces constructed in prop. 2 and its corollaries are isomorphisms of principal fibre spaces.

### 4. Universal Fibre Spaces

Let G be a topological group, let B and $B'$ be topological spaces, and let $(E, p)$ and $(E', p')$ be principal fibre spaces with group G and with bases B and $B'$ respectively.

Let U be an open subset of B and let $f':\overset{-1}{p}(U)\rightarrow E'$ be a continuous mapping which is compatible with the operations of G in $\overset{-1}{p}(U)$ and $E'$ respectively. Then there exists a unique continuous mapping $f: U\rightarrow B'$ such that $f\circ p_U=p'\circ f'$ and the commutative square

$$
E_U^{f'}E'
$$

$p_Up'$

U $^fB'$

is then cartesian (I, p. 94, example (FP)).

For every open subset U of B, let us then denote by $\mathscr{F}(U)$ the set of continuous mappings $g: E_U\rightarrow E'$ which are compatible with the operations of G in $\overset{-1}{p}(U)$ and $E'$ respectively. For every pair $(U,V)$ of open subsets of B such that $U\subset V$, let $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ denote the mapping defined by $r_{UV}(g) =g|E_U$. It is immediately verified that in this way a sheaf $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ on B has been defined. We shall call this sheaf the sheaf on B of morphisms of principal fibre spaces with group G from E into $E'$.

#### Proposition 4 {#ta-iv-s6-prop-4 .statement tag=024G}

If the space B is paracompact and if the space $E'$ is homotopic to a point, the sheaf on B of morphisms of principal fibre spaces with group G from E into $E'$ is a soft sheaf.

There exists an open covering $(U_j)_{j\in J}$ of B such that, for every $j\in J$, the fibre space $E_{U_j}$ is trivialisable. Since the space B is paracompact, we may suppose that the covering $(U_j)_{j\in J}$ is locally finite (TG, IX, p. 49) and choose a covering $(A_j)_{j\in J}$ of B where, for every $j\in J$, the set $A_j$ is closed in B and contained in $U_j$ (TG, IX, p. 49, prop. 4 and p. 48, cor. 1).

By I, p. 65, cor. 2 of prop. 6, it is enough, in order to prove the proposition, to establish the following assertion: let U be an open subset of B such that the principal fibre space $(E_U, p_U)$ is trivialisable, let A be a closed subset of B contained in U, let V be an open neighbourhood of A contained in U, and let $f$ be an element of $\mathscr{F}(V)$; then there exists an open neighbourhood W of A in V and an element $f'$ of $\mathscr{F}(U)$ such that $r_{WU}(f') =r_{WV}(f)$. Let us prove this assertion.

Let W be an open subset of B such that $A\subset W\subset \overline{W}\subset V$. Let $s: U\rightarrow E_U$ be a section of $(E_U, p_U)$. Apply Corollary 3 (IV, p. 438) to the space B, the closed subset $\overline{W}$ and the neighbourhood V of $\overline{W}$, and to the mapping $g=f\circ (s|_V)$ of $E_V$ into $E'$. There then exists a continuous mapping $\widetilde{g}: B\rightarrow E'$ which coincides with $g$ on $\overline{W}$. Put $h=\widetilde{g}|_U$. We have $h|_W=g|_W=f\circ (s|_W)$.

The mapping $H: U\times G\rightarrow E'$ defined by $H(x, g) =h(x)\cdot g$ for $(x, g)\in U\times G$ is continuous and compatible with the operations of G in $U\times G$ and $E'$. Put $f'= H\circ s^{-1}$; this is an element of $\mathscr{F}(U)$. For every $x\in W$, the mappings $f$ and $f'$ coincide at the point $s(x)$, hence at every point of $\overset{-1}{p}(x)$, since they are morphisms of principal fibre spaces. The proposition follows.

#### Theorem 1 {#ta-iv-s6-thm-1 .statement tag=024H}

Let G be a topological group, let $B_u$ be a topological space, and let $(E_u, p_u)$ be a principal fibre space with group G and base $B_u$. Suppose that the space $E_u$ is homotopic to a point.

Let B be a paracompact topological space.

a) Every principal fibre space with group G and base B is isomorphic to a principal fibre space of the form $f^*E_u$, where $f: B\rightarrow B_u$ is a continuous mapping.

b) Let $f_0$ and $f_1$ be continuous mappings of B into $B_u$. In order that $f_0^*E_u$ and $f_1^*E_u$ should be isomorphic principal fibre spaces with group G and base B, it is necessary and sufficient that the mappings $f_0$ and $f_1$ should be homotopic.

In other words, there exists a mapping of $[B,B_u]$ into P(B; G) which associates with the homotopy class of a continuous mapping $f$ of B into $B_u$ the isomorphism class of the principal fibre space $f^*E_u$. This mapping is bijective.

Let E be a principal fibre space with group G and base B. By Prop. 4, the sheaf $\mathscr{F}$ on B of morphisms of principal fibre spaces of E into $E_u$ is soft. Hence $\mathscr{F}(B)$ is not empty, whence a).

Let $f_0$ and $f_1$ be continuous mappings of B into $B_u$. If the mappings $f_0$ and $f_1$ are homotopic, the principal fibre spaces $f_0^*E_u$ and $f_1^*E_u$ are isomorphic (IV, p. 445, corollary 2). Let us prove the converse. For $\alpha \in  \{0,1\}$, let $E_{\alpha}$ denote the principal fibre $B_u$-space $f_{\alpha}^*E_u$, $g_{\alpha}: E_{\alpha}\rightarrow E_u$ the first projection and $p_{\alpha}: E_{\alpha}\rightarrow B$ the second projection. Let $i: E_0\rightarrow E_1$ be an isomorphism of principal fibre spaces. Let $p$ be the mapping $p_0\times$ Id$_{\mathbf{I}}: E_0\times \mathbf{I}\rightarrow B\times \mathbf{I}$.

Since the space $B\times \mathbf{I}$ is paracompact (TG, IX, p. 70, proposition 17), the sheaf $\mathscr{G}$ on $B\times \mathbf{I}$ of morphisms of principal fibre spaces from $E_0\times \mathbf{I}$ into $E_u$ is soft (IV, p. 446, proposition 4). Put $A = B\times  \{0,1\}$, $U = B\times ([0,\frac{1}{2}[\cup ]\frac{1}{2},1])$, and define an element $g$ of $\mathscr{G}(U)$ by setting

$g_0(x)$ for $(x, t)\in E_0\times [0,^1[$,

$g(x, t) =$ 2

$g_1\circ i(x)$ for $(x, t)\in E_0\times ]\frac{1}{2},1]$.

Since the sheaf $\mathscr{G}$ is soft, there exist an element $h\in \mathscr{G}(B\times \mathbf{I})$ and an open neighbourhood V of A in U such that $h|V =g|V$; such an element is a continuous mapping $H: E_0\times \mathbf{I}\rightarrow E_u$, compatible with the operations of G and such that $H(x,0) =g_0(x)$, $H(x,1) =g_1(i(x))$ for every $x\in E_0$. There then exists a mapping $h': B\times \mathbf{I}\rightarrow B_u$ such that $h'(p_0(x), t) =p_u(H(x, t))$ for $x\in E_0$ and $t\in \mathbf{I}$; this mapping is continuous, and it is a homotopy joining $f_0$ to $f_1$.

#### Corollary {#ta-iv-s6-n4-cor-1 .statement tag=024I}

Let G be a topological group, let B and $B'$ be paracompact topological spaces. Let $(E, p)$ and $(E', p')$ be principal fibre spaces with group G and with base B and $B'$ respectively. Suppose that the spaces E and $E'$ are both homotopic to a point. The spaces B and $B'$ are homotopic.

For there exists a continuous mapping $f: B\rightarrow B'$ such that the principal fibre space E is isomorphic to the principal fibre space $f^*E'$ and a continuous mapping $g: B'\rightarrow B$ such that the principal fibre space $E'$ is isomorphic to the principal fibre space $g^*E$ (Theorem 1, a)). The principal fibre spaces $(g\circ f)^*E$ and E are then isomorphic, therefore the mapping $g\circ f$ is homotopic to the mapping Id$_B$ (Theorem 1, b)). Analogously, the mapping $f\circ g$ is homotopic to the mapping Id$_{B'}$.

Let G be a topological group, let B be a topological space and let E be a principal fibre space with group G and with base B. Suppose that the space E is homotopic to a point. One says that the principal fibre space E is universal for principal fibre spaces with group G and paracompact base, and one says that the space B is a classifying space for G. If two classifying spaces for G are paracompact, they are homotopic. When there exists a classifying space, the study of isomorphism classes of principal fibre spaces with group G and paracompact base may be regarded as a homotopy problem.

#### Example {#ta-iv-s6-n4-exa-1 .statement tag=024J}

Endowed with the mapping $p:\mathbf{R}\rightarrow \mathbf{S}^1,t\mapsto e^{2\pi it}$, and with the operation of $\mathbf{Z}$ by translation, the space $\mathbf{R}$ is a principal covering space with group $\mathbf{Z}$. The space $\mathbf{S}^1$ is thus a classifying space for the group $\mathbf{Z}$.

For every discrete group G, we shall construct in the following number a metrisable space which is a classifying space for G.

### 5. Classifying space for a discrete group

Let G be a topological group; let us denote by $e$ its identity element. Let $G^*$ be the set of mappings $h: [0,1[\rightarrow G$ for which there exists a finite sequence $(t_i)_{0\leqslant i\leqslant n}$ with $0 =t_0< t_1<\cdots < t_n= 1$ such that $h$ is constant on the intervals $[t_{i-1}, t_i[$ for $1\leqslant i\leqslant n$. Such a sequence will be said to be adapted to $h$. For every finite subset of $G^*$, there exists a sequence adapted to each of its elements.

The set $G^*$ is a subgroup of $G^{[0,1[}$. We denote by $e^*$ its identity element; the inverse of an element $h\in G^*$ is the mapping $t\mapsto$ $h(t)^{-1}$, denoted by $h^{-1}$.

Let V be a neighbourhood of $e$ in G. Let $h\in G^*$ and let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to $h$. The set of elements $t\in [0,1[$ such that $h(t)\notin V$ is the union of certain of the intervals $[t_{i-1}, t_i[$; the sum of the lengths $t_i-t_{i-1}$ of these intervals does not depend on the sequence $(t_i)_{0\leqslant i\leqslant n}$ chosen; let us denote it by $p_V(h)$. For every real number $\varepsilon$ such that $\varepsilon  >0$, let us then denote by $V^*_{\varepsilon}$ the set of $h\in G^*$ such that $p_V(h)< \varepsilon$.

#### Proposition 5 {#ta-iv-s6-prop-5 .statement tag=024K}

There exists a unique topology on $G^*$ compatible with its group structure for which the sets $V^*_{\varepsilon}$ form a basis of neighbourhoods of the identity element.

Let us verify that the sets $V_{\varepsilon}^*$ satisfy axioms (GV$'_I$), (GV$'_{II}$) and (GV$'_{III}$) of TG, III, p. 4.

Let V be a neighbourhood of $e$ in G and let $\varepsilon$ be a strictly positive real number. Let W be a neighbourhood of $e$ in G such that $W\cdot W\subset V$. Let $h$ and $h'$ be elements of $G^*$. If $t\in [0,1[$ is such that $h(t)h'(t)\notin V$, one has $h(t)\notin W$ or $h'(t)\notin W$. It follows that $p_V(hh')\leqslant p_W(h)+p_W(h')$. Consequently, $W^*_{\varepsilon /2}\cdot W^*_{\varepsilon /2}\subset V^*_{\varepsilon}$, which proves axiom (GV$'_I$).

Let W be a neighbourhood of $e$ in G such that $W^{-1}\subset V$. Then $(W^*_{\varepsilon})^{-1}=$ $(W^{-1})^*_{\varepsilon}\subset V^*_{\varepsilon}$, whence axiom (GV$'_{II}$).

Let $k$ be an element of $G^*$; since the function $k$ takes only a finite number of values, there exists a neighbourhood W of $e$ in G such that $k(t)Wk(t)^{-1}\subset V$ for all $t\in [0,1[$. Let $h$ then be an element of $G^*$. For $t\in [0,1[$, if $k(t)h(t)k(t)^{-1}\notin$ V, then $h(t)\notin W$. Consequently, $p_V(khk^{-1})\leqslant p_W(h)$. This proves that $kW^*_{\varepsilon}k^{-1}\subset V^*_{\varepsilon}$, whence axiom (GV$'_{III}$).

#### Proposition 6 {#ta-iv-s6-prop-6 .statement tag=024L}

The space $G^*$ is contractible and locally contractible at each of its points.

For $h\in G^*$ and $t\in \mathbf{I}$, let us denote by $\sigma (h, t)$ the mapping of $[0,1[$ into G defined by $\sigma (h, t)(x) =h(x)$ if $0\leqslant x < t$ and $\sigma (h, t) =e$ otherwise.

Let us show that the mapping $\sigma : G^*\times \mathbf{I}\rightarrow G^*$ resulting is continuous. Let in fact $k\in G^*,u\in \mathbf{I}$, let V be a neighbourhood of $e$ in G and let $\varepsilon$ be a strictly positive real number. The element $\sigma (h, t)\sigma (k, u)^{-1}$ of $G^*$ is the mapping $f$ of $[0,1[$ into G defined by

$h(x)k(x)^{-1}$ if $0\leqslant x <$ min($t, u$) ;

$h(x)$ if $u\leqslant x < t$;

$$
f(x) =
$$

$k(x)^{-1}$ if $t\leqslant x < u$;

$e$ otherwise.

Consequently,

$$
p_V(\sigma (h, t)\sigma (k, u)^{-1})\leqslant p_V(hk^{-1}) +|t-u|
$$

in other words, for $\sigma (h, t)\in V^*_{\varepsilon}\sigma (k, u)$, it is enough that one have $|t-u|\leqslant \frac{\varepsilon}{2}$ and $h\in V^*_{\varepsilon /2}k$, which proves the continuity of $\sigma$ at $(k, u)$.

For every $h\in G^*,\sigma (h,0)$ is the constant mapping with image $\{e\}$, whereas $\sigma (h,1) =h$. Moreover, $\sigma (e, t) =e$ for every $t\in \mathbf{I}$. Consequently, $\sigma$ is a pointed homotopy at $e\in G^*$ joining the constant mapping with image $\{e\}$ to the identity mapping of $G^*$. This proves that $G^*$ is contractible at $e^*$.

Moreover, for every neighbourhood V of $e$ in G and every real number $\varepsilon  >0$, one has $\sigma (V^*_{\varepsilon}\times \mathbf{I})\subset V^*_{\varepsilon}$. Hence $V^*_{\varepsilon}$ is also contractible at $e^*\in$ $G^*$, so that $G^*$ is locally contractible at $e^*$.

Since $G^*$ is a topological group, it is contractible and locally contractible at each of its points.

Let $\iota$ be the mapping of G into $G^*$ which associates to $g\in G$ the constant mapping with image $\{g\}$ of $[0,1[$ into G. The mapping $\iota$ is an injective homomorphism of groups. Let V be a neighbourhood of $e$ in G and let $\varepsilon$ be a strictly positive real number. One has $\overset{-1}{\iota}(V^*_{\varepsilon}) = V$ if $\varepsilon \leqslant 1$ and $\overset{-1}{\iota}(V^*_{\varepsilon}) = G$ otherwise. The inverse image of a neighbourhood of the identity element of $G^*$ is a neighbourhood of the identity element of G, whence the continuity of $\iota$. Moreover, $\iota (V) = V^*_1\cap \iota (G)$ for every neighbourhood V of $e$ in G. Hence $\iota$ defines an isomorphism of topological groups of G onto its image.

#### Remark 1 {#ta-iv-s6-n5-rem-1 .statement tag=024M}

If G is a separated topological group, $\iota (G)$ is closed in $G^*$.

Let indeed $h\in G^*$ be such that $h\notin \iota (G)$, let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to $h$, put $\varepsilon =$ min$_{1\leqslant i\leqslant n}(t_i-t_{i-1})$. Let V be a neighbourhood of $e$ in G such that $h(t_i)^{-1}h(t_j)\notin V$, for every pair $(i, j)$ of integers such that $0\leqslant i, j\leqslant n-1$ and $h(t_i)=\not h(t_j)$; there exists one since G is separated. Let W be a neighbourhood of $e$ in G such that $W\cdot W^{-1}\subset V$. Let us prove that then $hW^*_{\varepsilon}$ does not meet $\iota (G)$.

Let us reason by contradiction. Let $f$ be an element of $W^*_{\varepsilon}$ and $g$ an element of G such that $hf$ = $\iota (g)$. We therefore have $f(t) =h(t)^{-1}g$ for all $t\in [0,1[$, so that the sequence $(t_i)$ is also adapted to the function $f$. If the value taken by $f$ on the interval $[t_{i-1}, t_i[$ does not belong to W, then $t_i-t_{i-1}< \varepsilon$, since $f\in W^*_{\varepsilon}$. This inequality being false, by definition of $\varepsilon$, we have $f(t)\in W$ for all $t\in [0,1[$. Let $i$ and $j$ then be elements of $\{0, . . . , n-1\}$ such that $h(t_i)=\not h(t_j)$; we have

$$
h(t_i)^{-1}h(t_j) =f(t_i)g^{-1}gf(t_j)^{-1}=f(t_i)f(t_j)^{-1}\in W\cdot W^{-1}
$$

which contradicts the choice of W. The subgroup $\iota (G)$ of $G^*$ is therefore closed.

Suppose that G is a metrisable topological group and let $d$ be a distance on G which defines its topology. Let $h$ and $h'\in G^*$ and let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to $h$ and $h'$. The real number

$$
\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h'(t_{i-1}))
$$

does not depend on the sequence $(t_i)$ chosen; let us denote it by $d^*(h, h')$.

Let us prove that $d^*$ is a distance on $G^*$. We have $d^*(h, h') =$ $d^*(h', h)$ for $h,h'\in G^*$, and $d^*(h, h) = 0$ for all $h\in G^*$. Conversely, let $h$ and $h'$ be elements of $G^*$ such that $d^*(h, h') = 0$. Let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to $h$ and $h'$. Since

$$
0 =d^*(h, h') =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h'(t_{i-1}))
$$

and all the terms of this sum are positive or zero, we have $d(h(t_{i-1}), h'(t_{i-1})) = 0$ for all $i\in  \{1, . . . , n\}$, whence $h=h'$. Finally, let $h,h',h''$ be elements of $G^*$ and let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to each of them. Then,

$$
d^*(h, h'') =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h''(t_{i-1}))
$$

$$
\leqslant \sum_{i=1}^n(t_i-t_{i-1})(d(h(t_{i-1}), h'(t_{i-1}))+d(h(t_{i-1}), h''(t_{i-1})))
$$

$$
=d^*(h, h') +d^*(h, h'')
$$

therefore $d^*$ satisfies the triangle inequality.

This distance $d^*$ is invariant under right (resp. left) translations if $d$ is.

#### Proposition 7 {#ta-iv-s6-prop-7 .statement tag=024N}

Suppose that G is a metrizable topological group. Then the topological group $G^*$ is metrizable. More precisely, if $d$ is a bounded distance on G which defines its topology, the topology of $G^*$ is defined by the distance $d^*$.

Let $d$ be a distance on G which defines its topology. Then, the mapping $d'$ given by $d'(h, h') =$ inf($d(h, h'),1$) is a bounded distance on G which also defines its topology (TG, IX, p. 3). It is therefore enough to prove that $d^*$ defines the topology of $G^*$ under the assumption that $d$ is bounded.

Let V be a neighbourhood of $e$ in G and let $\varepsilon$ be a strictly positive real number. Let $\delta$ be a strictly positive real number such that V contains the ball $B(e, \delta )$. Let $h\in G^*$ and let $(t_i)_{0\leqslant i\leqslant n}$ be a sequence adapted to $h$. Then,

$$
p_V(h) =\sum_{h(t_ii_-=1_1)\notin V}^n(t_i-t_{i-1})
$$

$$
\leqslant \sum^n(t_i-t_{i-1})\frac{d(h(t_{i-1}), e)}{\delta}
$$

$$
i=1
$$

$d(h(t_{i-1}),e)\geqslant \delta$

$$
\leqslant \frac{d^*(h, e^*)}{\delta}
$$

Consequently, the ball $B(e^*, \varepsilon \delta )$ in $G^*$ is contained in $V_{\varepsilon}^*$.

Conversely, let $\delta$ be a strictly positive real number and let Δ be a strictly positive upper bound for the diameter of G. Let V be a neighbourhood of $e$ in G contained in the ball $B(e, \delta /2)$. For a function $h\in G^*$ and a sequence $(t_i)_{0\leqslant i\leqslant n}$ adapted to $h$, one has

$$
d^*(h, e^*) =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)
$$

= $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)\leqslant \delta /2$

+ $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)>\delta /2$

$\leqslant \frac{\delta}{2}+ \Delta \sum_{i=1}^n(t_i-t_{i-1})$

$h(t_{i-1})\notin V$

$$
\leqslant \frac{\delta}{2}+ \Delta p_V(h)
$$

The preceding inequality implies that, for every element $h$ of $V_{\delta /2\Delta}^*$, one has $d^*(h, e^*)\leqslant \delta$. Consequently, every ball of $G^*$ for the distance $d^*$ contains a neighbourhood of the identity element.

#### Remark 2 {#ta-iv-s6-n5-rem-2 .statement tag=024O}

Let $d$ be a bounded distance which defines the topology of G. When the topological group $G^*$ is endowed with the distance $d^*$, the homomorphism $\iota : G\rightarrow G^*$ is an isometry.

#### Remark 3 {#ta-iv-s6-n5-rem-3 .statement tag=024P}

Suppose that G is a discrete topological group. The subgroup $\iota (G)$ is then a discrete subgroup of $G^*$. In fact, the topology of G is defined by the distance $d$ on G given by $d(g, g') = 1$ if $g=\not g'$ and $d(g, g') = 0$ otherwise. The assertion then follows from the preceding remark.

#### Theorem 2 {#ta-iv-s6-thm-2 .statement tag=024Q}

Let G be a discrete topological group. Let G operate on the right in $G^*$ by $h\cdot g=h\iota (g)$ and let B denote the quotient topological space $G^*/G$.

The space $G^*$ is a principal covering of B with group G; it is simply connected by paths.

The space B is a metrizable topological space, connected by paths, locally contractible, and its Poincaré group at every point is isomorphic to G.

Thus, the space B is a classifying space for the group G.

The group $G^*$ is contractible to its identity element (IV, p. 450, prop. 6). In particular it is connected by paths (III, p. 260) and simply connected by paths (IV, p. 340).

The group $\iota (G)$ is closed in $G^*$ (TG, III, p. 7, prop. 5), hence the space $G^*/G$ is metrisable (TG, III, p. 13, prop. 18 and TG, IX, p. 25, prop. 4). It is also connected by arcs (III, p. 258, prop. 3). Since the group $\iota (G)$ is discrete, it follows from corollary 2 of I, p. 100, that $G^*$ is a principal G-covering of B. The pointed covering $(G^*, e^*)$ is then a universal covering of the space B pointed at the image of $e^*$; the Poincaré group of B (at each of its points) is isomorphic to G.

## EXERCISES {#ta-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
