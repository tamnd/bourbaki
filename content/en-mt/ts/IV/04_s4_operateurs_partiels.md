---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 4
section_title: Opérateurs partiels
lang: en
source: ts-iii-v-fr
book_pages: TS IV.224-TS IV.261, TS IV.344-TS IV.352
pdf_pages: 0237-0274, 0357-0365
extraction: native
subsections:
    - "no": 1
      title: Opérateurs partiels
      page: 224
      pdf_page: 237
    - "no": 2
      title: Opérateurs fermés, fermables et à domaine dense
      page: 227
      pdf_page: 240
    - "no": 3
      title: Exemples d’opérateurs partiels
      page: 231
      pdf_page: 244
    - "no": 4
      title: Adjoint
      page: 235
      pdf_page: 248
    - "no": 5
      title: Critères élémentaires pour les opérateurs auto-adjoints
      page: 239
      pdf_page: 252
    - "no": 6
      title: Opérateurs différentiels
      page: 242
      pdf_page: 255
    - "no": 7
      title: Spectre et résolvante
      page: 243
      pdf_page: 256
    - "no": 8
      title: Pseudo-spectre
      page: 250
      pdf_page: 263
    - "no": 9
      title: Opérateurs de multiplication
      page: 252
      pdf_page: 265
    - "no": 10
      title: Extensions auto-adjointes d’un opérateur symétrique
      page: 255
      pdf_page: 268
statements: 74
exercises: 24
content_sha256: 0dde724b75a1681dcc83ba3a9f7f0d845b34c1b80f481582d556c63070e9f580
translated_from: content/fr/ts/IV/04_s4_operateurs_partiels.md
source_lang: fr
translation_method: machine
source_content_sha256: 3cd17fd996cfdeaafc25ba263abdd60eec21307e4dac7a13cf5fd093c75b9e9d
translation_model: gpt-5.4
translation_run: translate-en-mt-9b860916
glossary_version: 34
glossary_terms_sha256: b7d515ffd63fdd397da83f079e71984b8569457c0e3cb5dac126269372ab1ed3
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. PARTIAL OPERATORS

### 1. Partial operators

In this number, K is a commutative field.

We recall (E, II, §3, p. 9–10) that a graph[^1] is a set all of whose elements are pairs. If A and B are sets, a correspondence between A and B is a triplet $(\Gamma ,A,B)$, where Γ is a graph contained in $A\times B$; its set of definition (also called its domain) is pr$_1$(Γ), and the set of its values is pr$_2(\Gamma )$. A correspondence is a function (E, II, p. 13, def. 9) if its graph is functional and if its initial set coincides with its set of definition. Every subset of a functional graph is a functional graph.

#### Definition 1 {#ts-iv-s4-def-1 .statement tag=032J}

Let E and F be vector spaces over K. A partial operator $u$ from E into F is a correspondence $(\Gamma ,E,F)$ between E and F satisfying the following conditions:

(i) The graph Γ is a vector subspace of $E\times F$;

(ii) The graph Γ is functional.

If E = F, one says that $u$ is a partial operator on E.

Let $u$ be a partial operator from E into F. The graph Γ of the correspondence $u$ is called the graph of the partial operator $u$, and is also denoted by $\Gamma_u$. We denote by $\mathscr{P}(E; F)$ the set of partial operators from E into F; we write simply $\mathscr{P}(E) =\mathscr{P}(E; E)$.

To give a partial operator from E into F amounts to giving a vector subspace D of E and a linear mapping $u$ from D into F, the associated partial operator being the correspondence $(\Gamma ,E,F)$ where $\Gamma \subset D\times F$ is the graph of $u$.

The domain of definition of a partial operator $u$ is called simply the domain of $u$, and denoted by dom($u$).

Every linear mapping $u$ from E into F is a partial operator from E into F.

If $D\subset E$ is a vector subspace, we shall denote by $1_D$ the partial operator with domain D which is the identity mapping on D, that is, the correspondence $(\Delta_D,E,E)$ where $\Delta_D$ is the diagonal of $D\times D$ (E, II, p. 13, def. 8). We shall denote by $0_D$ the partial operator with domain D which is zero on D, that is, the correspondence $(D\times  \{0\},E,F)$.

Two partial operators $u= (\Gamma ,E,F)$ and $u'= (\Gamma ',E,F)$ from E into F are equal if and only if dom($u$) $=$ dom($u'$) and if the linear mappings $u$ and $u'$ from dom($u$) into F coincide.

Following E, II, §3, the following notions are defined:

(i) Let $u$ be a partial operator from E into F; let D be its domain and $u: D\rightarrow F$ the associated linear mapping. The image of a subset A of E by $u$ is the subset $u(A\cap D)$ of F; it is denoted simply by $u(A)$. The inverse image by $u$ of a subset B of F by $u$ is the subset $\overset{-1}{u}(B)$ of D.

If A (resp. B) is a vector subspace of E (resp. of F), then its image by $u$ (resp. its inverse image) is a vector subspace of F (resp. of E).

The image of $u$ is the vector subspace $u(D)$ of F, also denoted by Im($u$). One says that $u$ is a surjective partial operator if Im($u$) $= F$. The kernel of $u$ is the vector subspace $\overset{-1}{u}(\{0\})$ of E, also denoted by Ker($u$). The kernel of $u$ is reduced to 0 if and only if the linear mapping $u$ from dom($u$) into F is injective. One then says that $u$ is injective. If $u$ is injective and surjective, one says that it is bijective.

(ii) If E, F and G are K-vector spaces and $u= (\Gamma ,E,F)$, $v= (\Gamma ',F,G)$ are partial operators from E into F and from F into G, respectively, the composite correspondence $v\circ u= (\Gamma '\circ \Gamma ,E,G)$ is a partial operator from E into G. Its domain is $\overset{-1}{u}$(dom($v$)). If H is a K-vector space and $w= (\Gamma '',G,H)$ a partial operator from G into H, one has $w\circ (v\circ u) = (w\circ v)\circ u$. One will sometimes write $vu$ instead of $v\circ u$.

(iii) In particular, for every partial operator $u$ from E into F and every $a\in K$, the partial operators $au= (a1_F)\circ u$ and $ua=u\circ (a1_E)$ are defined. They are equal if $a\not = 0$, or if the domain of $u$ is equal to E; one has $u0 = 0_E$ and $0u= 0_{dom(u)}$.

Let E be a vector space. From what precedes, the set $\mathscr{P}$(E), endowed with the law of composition defined by $(u, v)\mapsto u\circ v$, is a unital associative magma (A, I, p. 4, Def. 5 and A, I, p. 12, Def. 2) with identity element $1_E$. For every $n\in \mathbf{N}$, one denotes by $u^n$ the composite $\overset{n}{\circ}u$ (A, I, p. 13).

Moreover, one defines the following notions:

(i) If $u= (\Gamma ,E,F)$ is a partial operator from E into F, and if G is a subspace of E, the reduction of $u$ to G is the partial operator $(\Gamma \cap (G\times F),E,F)$ from E into F. Its domain is dom($u$)$\cap G$; one will sometimes denote it by $u|G$, when no confusion with the restriction of $u$ to the subspace G is to be feared.

(ii) Let $v$ be an injective partial operator from F into E. Then the inverse correspondence $v^{-1}= (\Gamma^{-1},E,F)$ of $v$ is a partial operator such that dom($v^{-1}$) $=$ Im($v$). One says that $v^{-1}$ is the inverse partial operator of $v$. One has the equalities $v\circ v^{-1}= 1_{dom(v^{-1})}$ in $\mathscr{P}(E)$ and $v^{-1}\circ v= 1_{dom(v)}$ in $\mathscr{P}(F)$. The partial operator $v^{-1}$ is injective and one has $(v^{-1})^{-1}=v$.

(iii) Let E, F and G be vector spaces. Let $u$ (resp. $v$) be an injective partial operator from E into F (resp. from F into G). Then the partial operator $v\circ u$ is injective and $(v\circ u)^{-1}=u^{-1}\circ v^{-1}$.

(iv) If $u$ and $v$ are partial operators from E into F, one says that $v$ is an extension of $u$, and one writes $u\subset v$, if the graph of $u$ is contained in the graph of $v$. This implies that dom($u$)$\subset$ dom($v$) and that $u$ is the restriction of $v$ to dom($u$). The relation “ $u\subset v$ ” is an order relation in $\mathscr{P}(E; F)$. For example, one has $au\subset ua$ for every $a\in K$ and every $u\in \mathscr{P}(E; F)$.

(v) Let E be a vector space over K and $(F_i)_{i\in I}$ a family of vector spaces over K. For $i\in I$, let $u_i$ be a partial operator from E into $F_i$. The product partial operator of the $u_i$ is the partial operator from E into the product vector space of the spaces $F_i$ whose domain is the intersection D of the spaces dom($u_i$) and which associates to $x\in D$ the family $(u_i(x))_{i\in I}$. It is denoted by $(u_i)_{i\in I}$.

(vi) Let $A : F\times F\rightarrow F$ be the linear mapping $(x, y)\mapsto x+y$. Let $u$ and $v$ be partial operators from E into F. The sum $u+v$ is the partial operator $A\circ (u, v)$ from E into F. Its domain is dom($u$)$\cap$ dom($v$). For $u,v,w$ in $\mathscr{P}(E; F)$, one has $(u+v) +w=u+ (v+w)$.

Let G be a vector space over K. For every $u$ and $v$ in $\mathscr{P}(E; F)$ and every $w\in \mathscr{P}(F; G)$, one has $w\circ u+w\circ v\subset w\circ (u+v)$. In general, there is no equality in this formula (exercise 1 of IV, p. 344), but this is the case when the domain of $w$ is equal to F. For $w\in \mathscr{P}(G; E)$, one has $u\circ w+v\circ w= (u+v)\circ w$.

(vii) Let L be an extension of the field K. Let E and F be vector spaces over K and $E_{(L)}= L\otimes_KE, F_{(L)}= L\otimes_KF$ the L-vector spaces obtained by extension of scalars from K to L (A, II, p. 82). For every partial operator $u$ from E into F, let $u_{(L)}$ denote the partial operator from $E_{(L)}$ into $F_{(L)}$ whose graph is the vector subspace $L\otimes_K\Gamma_u$ of $E_{(L)}\times F_{(L)}$; its domain is $L\otimes_K$ dom($u$), and it coincides on this with the unique linear mapping sending $1\otimes x$ to $1\otimes u(x)$ for every $x\in$ dom($u$).

Let $v$ be a partial operator from E into F. One has $u\subset v$ if and only if $u_{(L)}\subset v_{(L)}$.

(viii) Let $E_1, F_1, E_2, F_2$ be K-vector spaces. Let $u$ (resp. $v$) be a partial operator from $E_1$ into $F_1$ (resp. from $E_2$ into $F_2$). Let $u\otimes v$ denote the partial operator from $E_1\otimes F_1$ into $E_2\otimes F_2$ with domain dom($u$)$\otimes$dom($v$) such that $(u\otimes v)(x\otimes y) =u(x)\otimes v(y)$ for every $(x, y)\in E_1\times E_2$.

### 2. Closed operators, closable operators, and operators with dense domain

In this No., K denotes a commutative topological field (TG, III, p. 54).

#### Definition 2 {#ts-iv-s4-def-2 .statement tag=032K}

Let E and F be topological vector spaces over K (EVT, I, p. 1, def. 1). Let $u\in \mathscr{P}(E; F)$ be a partial operator from E into F.

One says that $u$ is an operator with dense domain if the domain of $u$ is dense in E.

One says that $u$ is closed if the graph of $u$ is closed in the topological vector space $E\times F$. One says that $u$ is closable if it possesses a closed extension.

Let E, F and G be topological vector spaces over K. Every extension of an operator $u\in \mathscr{P}(E; F)$ with dense domain has dense domain. Moreover, if $v\in \mathscr{L}(E; F)$, then $u+v$ is an operator with dense domain. If $v: F\rightarrow G$ (resp. $w: G\rightarrow E$) is an isomorphism of topological vector spaces, then $v\circ u$ (resp $u\circ w$) is an operator with dense domain.

#### Example {#ts-iv-s4-n2-exa-1 .statement tag=032L}

Let E and F be topological vector spaces over K.

1) Suppose the space F separated. Let $u$ be a linear mapping from E into F. If $u$ is continuous, then the partial operator $u$ is closed (TG, I, p. 53, Corollary 2). Suppose moreover that K is a non-discrete valued field and that E and F are metrisable complete topological vector spaces over K. By the closed graph theorem (EVT, I, p. 19, Corollary 5), the partial operator defined by $u$ is then closed if and only if $u$ is continuous.

2) Suppose the space E separated. Let $v$ be an injective continuous linear mapping from F into E. The partial operator $v^{-1}\in \mathscr{P}(E; F) ($cf. IV, p. 226) is then closed, since its graph is the image of the graph of $v$, which is closed, under the isomorphism of topological vector spaces from $F\times E$ onto $E\times F$ defined by $(y, x)\mapsto (x, y)$.

#### Proposition 1 {#ts-iv-s4-prop-1 .statement tag=032M}

Let E and F be topological vector spaces over K. A partial operator $u$ of E into F is closable if and only if the closure of the graph $\Gamma_u$ of $u$ in $E\times F$ is a functional graph. There then exists a unique partial operator $v$ of E into F whose graph is $\overline{\Gamma}_u$, and it is the smallest closed extension of $u$.

If the closure of the graph of $u$ in $E\times F$ is a functional graph, it is the graph of a partial operator, and this is a closed extension of $u$, so that $u$ is closable. Conversely, suppose that $u\subset w$ with $w$ closed. The closure $\overline{\Gamma}_u$ of the graph of $u$ in $E\times F$ is contained in $\Gamma_w$, hence $\Gamma_u$ is a functional graph.

The last assertion follows from the fact that if $w$ is a closed extension of $u$, then the graph of $w$ contains $\overline{\Gamma}_u$.

#### Definition 3 {#ts-iv-s4-def-3 .statement tag=032N}

Let E and F be topological vector spaces over K. Let $u$ be a closable operator of E into F. The closed operator whose graph is $\Gamma_u$ is called the closure of $u$. It is denoted by $\overline{u}$.

#### Remark {#ts-iv-s4-n2-rem-1 .statement tag=032O}

Let E and F be topological vector spaces over K. Let $u$ be a closable operator of E into F. The domain of the closure of $u$ is contained in the closure of the domain of $u$ in E. In general, it is distinct from it (exercise 1 of IV, p. 344, b)).

If $u\in \mathscr{P}(E; F)$ is closable and dom($u$) $= E$, then $u=\overline{u}$ is closed, since then dom($\overline{u}$) $=$ dom($u$).

#### Proposition 2 {#ts-iv-s4-prop-2 .statement tag=032P}

Let $K =\mathbf{R}$ and let E and F be topological vector spaces over $\mathbf{R}$. Let $u$ be a partial operator of E into F. Then $u$ has dense domain (resp. is closed, is closable) if and only if $u_{(\mathbf{C})}$ has dense domain (resp. is closed, is closable).

Suppose that the domain of $u$ is dense in E. Every neighbourhood of 0 in $E_{(\mathbf{C})}$ contains a neighbourhood of the form $V +iV$ (TVS, II, p. 65), where V is a neighbourhood of 0 in E, and therefore contains an element of the domain of $u_{(\mathbf{C})}$; this partial operator therefore has dense domain. The converse is also true since the mapping of $E_{(\mathbf{C})}$ into E which associates $x$ to $x+iy$ for every $(x, y)\in E\times E$ is continuous and surjective.

The graph of $u_{(\mathbf{C})}$ identifies with the complexified topological vector space of the graph of $u$. It is therefore closed in $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$ if the graph of $u$ is closed in $E\times E$. Conversely, one has $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$ in $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$; since $E\times E$ is closed in $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$, the partial operator $u$ is closed when $u_{(\mathbf{C})}$ is.

A partial operator $v$ from E into F is an extension of $u$ if and only if $v_{(\mathbf{C})}$ is an extension of $u_{(\mathbf{C})}$, hence the partial operator $u_{(\mathbf{C})}$ is closable if $u$ is closable. Conversely, if $u_{(\mathbf{C})}$ is closable, the partial operator $u$ is also, since $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$, which is then a functional graph (prop. 1).

#### Lemma 1 {#ts-iv-s4-lem-1 .statement tag=032Q}

Let E, F and G be topological vector spaces over K. Let $u$ be a closed operator from E into F.

a) For every $v\in \mathscr{L}(E; F)$, the partial operator $u+v$ is closed.

b) For every $v\in \mathscr{L}(G; E)$, the partial operator $u\circ v$ is closed.

Let us prove a). Let $\gamma$ be the mapping $(x, y)\mapsto (x, y-v(x))$ of $E\times F$ into itself; it is continuous. For every $(x, y)\in E\times F$, one has $\gamma (x, y)\in \Gamma_u$ if and only if $x\in$ dom($u$) and $y=u(x) +v(x)$, that is to say that $\overset{-1}{\gamma}(\Gamma_u) = \Gamma_{u+v}$. The assertion follows.

Let us prove b). The mapping $\eta = (v,1_F)$ of $G\times F$ into $E\times F$ is continuous; for every $(z, y)\in G\times F$, one has $\eta (z, y) = (v(z), y)$, hence $\overset{-1}{\eta}(\Gamma_u) = \Gamma_{u\circ v}$. The assertion follows.

Let E and F be topological vector spaces over K, F being separated. Let $a\in K$. If $u\in \mathscr{P}(E; F)$ is closable, the same is true of $au$. If $a\not = 0$, one has $\overline{au}=au$, and $u$ is closed if and only if $au$ is. If $a= 0$, the closure of $au$ is $0_{\overline{dom(u)}}$, and $au$ is equal to $0_{dom(\overline{u})}$; it may therefore happen that $u$ is closed but that $au$ is not.

#### Proposition 3 {#ts-iv-s4-prop-3 .statement tag=032R}

Let E and F be topological vector spaces over K, F being separated. Let $u$ be a closed partial operator from E into F. The kernel of $u$ is a closed subspace of E.

In fact, the kernel of $u$ is the inverse image of the closed subspace $\Gamma_u\cap (E\times  \{0\})$ of $E\times F$ by the continuous linear mapping $x\mapsto (x,0)$ of E into $E\times F$.

In the rest of this No., it is assumed that K is a non-discrete valued field.

#### Definition 4 {#ts-iv-s4-def-4 .statement tag=032S}

Let E and F be normed spaces over K and let $u$ be a partial operator from E into F. For $x$ in dom($u$), one writes

$$
\|x\|_u= (\|x\|^2_E+\|u(x)\|^2_F)^{1/2}
$$

The mapping $x\mapsto  \|x\|_u$ resulting is a norm on dom($u$). The normed space thus obtained is denoted by $E_u$.

#### Remark {#ts-iv-s4-n2-rem-2 .statement tag=032T}

Let E and F be normed spaces over K and let $u$ be a partial operator from E into F.

1) The canonical injection of $E_u$ into E is continuous since one has $\|x\|\leqslant \|x\|_u$ for every $x\in E$. In particular, every subspace of dom($u$) which is closed in E is closed in $E_u$.

2) If E and F are Hilbert spaces, then the space $E_u$ is a prehilbertian space, since the norm on $E_u$ arises from the positive Hermitian form

$$
(x, y)\mapsto (x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

on dom($u$).

#### Proposition 4 {#ts-iv-s4-prop-4 .statement tag=032U}

Let E and F be Banach spaces (resp. Hilbert spaces), and let $u$ be a partial operator from E into F. Then $u$ is closed if and only if the normed space $E_u$ is a Banach space (resp. a Hilbert space).

It is enough to treat the case of Banach spaces. The norm of $E_u$ is obtained, by transport of structure by means of the bijective linear mapping $(x, y)\mapsto x$ of $\Gamma_u$ onto dom($u$), from the norm obtained by restriction to the subspace $\Gamma_u$ of the norm $(x, y)\mapsto (\|x\|^2_E+\|y\|^2_F)^{1/2}$ on the Banach space $E\oplus F$. Thus the space $E_u$ is a Banach space if and only if the subspace $\Gamma_u$ of $E\oplus F$ is closed.

If $u$ and $v$ are partial operators from E into F and from F into G, respectively, and if $u$ is closed, then the partial operator $v\circ u$ is not closed in general, even if $v$ is continuous (exercise 1 of IV, p. 344, c)). One nevertheless has the following sufficient condition:

#### Lemma 2 {#ts-iv-s4-lem-2 .statement tag=032V}

Let E, F and G be normed spaces over K, F being a Banach space. Let $u$ be a closed partial operator from E into F and let $v\in \mathscr{L}(F; G)$. If there exists $C\in \mathbf{R}_+$ such that

$$
\|u(x)\|\leqslant C(\|x\|+\|(v\circ u)(x)\|)
$$

for every $x\in$ dom($v\circ u$) $=$ dom($u$), that is to say, if the linear mapping $x\mapsto u(x)$ from $E_{v\circ u}$ into F is continuous, then $v\circ u$ is closed.

Let us write $w=v\circ u$. Let $(x_n, w(x_n))_{n\in\mathbf{N}}$ be a sequence in the graph of $w$ which converges in $E\times G$. Let $x$ be the limit of the sequence $(x_n)$. The hypothesis implies that the sequence $(u(x_n))_{n\in\mathbf{N}}$ is then a Cauchy sequence in F; it converges to an element $y$ of F. Since $u$ is closed, one has therefore $x\in$ dom($u$) and $y=u(x)$. Then $w(x_n) =v(u(x_n))$ tends to $v(y) =$ $v(u(x))$ since $v$ is continuous, hence the graph of $w$ is closed.

Let $u$ be a closed partial operator on a Banach space E and F a subspace of dom($u$). If F is dense in the Banach space $E_u$, then the restriction of $u$ to F is closable, and its closure is equal to $u$. One then says that F is a core for $u$.

### 3. Examples of partial operators

In this No., $K =\mathbf{R}$ or $\mathbf{C}$.

#### Example 1 {#ts-iv-s4-n3-exa-1 .statement tag=032W}

Let X be a locally compact topological space and let $\mu$ be a positive measure on X. Let $p_1$ and $p_2$ be fixed elements of $[1,+\infty [$.

Let $g$ be a $\mu$-measurable function on X with values in K. Let D denote the subspace of $\mathscr{L}_K^{p_1}(X, \mu)$ formed by the functions $f$ in $\mathscr{L}_K^{p_1}(X, \mu)$ such that $gf\in \mathscr{L}_K^{p_2}(X, \mu)$. The linear mapping from D into $\mathscr{L}_K^{p_2}(X, \mu)$ defined by $f\mapsto gf$ determines a partial operator from $\mathscr{L}_K^{p_1}(X, \mu)$ into $\mathscr{L}_K^{p_2}(X, \mu)$, which is denoted by $m_g$.

The vector subspace of $\mu$-negligible functions in $\mathscr{L}_K^{p_1}(X, \mu)$ is contained in D, and the image under $m_g$ of a $\mu$-negligible function is again $\mu$-negligible. We shall denote by $\widetilde{m}_g$ the partial operator from $L^{p_1}_K(X, \mu)$ into $L^{p_2}_K(X, \mu)$ deduced from $m_g$ by passing to quotients. It is said to be the multiplication operator by $g$ from $L^{p_1}_K(X, \mu)$ into $L^{p_2}_K(X, \mu)$. Functions $g_1$ and $g_2$ which are locally equal $\mu$-almost everywhere define the same multiplication operator.

#### Proposition 5 {#ts-iv-s4-prop-5 .statement tag=032X}

The multiplication operator $\widetilde{m}_g$ from $L^{p_1}_K(X, \mu)$ into $L^{p_2}_K(X, \mu)$ is a closed operator with dense domain.

Let us first prove that the partial operator $\widetilde{m}_g$ is closed. Let $(f_n, h_n)_{n\in\mathbf{N}}$ be a sequence in $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ such that the sequence $(f_{\widetilde{n}},\widetilde{h}_n)$ of the classes of $f_n$ and $h_n$ belongs to the graph of $\widetilde{m}_g$ and converges in $L^{p_1}_K(X, \mu)\times L^{p_2}_K(X, \mu)$ when $n$ tends to infinity. Let $(f, h)$ be a pair in $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ such that the pair $(\widetilde{f} ,\widetilde{h})$ of their classes is the limit of $(\widetilde{f}_n,\widetilde{h}_n)$.

There exists a sequence $(f_{n_k})_{k\in\mathbf{N}}$ extracted from the sequence $(f_n)_n$ such that $f_{n_k}(x)$ converges to $f(x)$ for $\mu$-almost every $x$ (INT, IV, p. 131, § 3, n$^o4$, th. 3). This implies that $h_{n_k}(x) =g(x)f_{n_k}(x)$ converges $\mu$-almost everywhere to $g(x)f(x)$. Moreover the sequence $(h_{n_k})$ converges to $h$ in the space $\mathscr{L}_K^{p_2}(X, \mu)$. The functions $h$ and $gf$ are therefore equal $\mu$-almost everywhere (loc. cit.). Thus $\widetilde{f}$ belong to the domain of $\widetilde{m}_g$ and $\widetilde{h}=\widetilde{m}_g(\widetilde{f})$. This proves that $\widetilde{m}_g$ is closed.

Let us prove that the domain of $\widetilde{m}_g$ is dense in $L^{p_1}_K(X, \mu)$. It is enough to verify that the classes of functions $f\in \mathscr{K}(X; K)$ belong to the closure of the domain of $\widetilde{m}_g$ in $L^{p_1}_K(X, \mu)$. Let $f\in \mathscr{K}(X; K)$ and let $\widetilde{f}$ be its class in $L^{p_1}_K(X, \mu)$. For every integer $n\in \mathbf{N}$, let $\varphi_n$ denote the characteristic function of the set of elements $x\in X$ such that $|g(x)|\leqslant n$, and put $f_n=f \varphi_n$. Then $|gf_n|\leqslant n|f|$, which belong to $\mathscr{L}_K^{p_2}(X, \mu)$, hence $f_n$ belong to the domain of $\widetilde{m}_g$. For every element $x$ of X, the sequence $(f_n(x))_{n\in\mathbf{N}}$ converges to $f(x)$ when $n\rightarrow +\infty$; moreover, one has $|f_n|\leqslant |f|$, which belong to $\mathscr{L}_K^{p_1}(X, \mu)$. By Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6), the sequence of classes of $f_n$ converges to $\widetilde{f}$ in $L^{p_1}_K(X, \mu)$. Thus, the class of $f$ belong to the closure of the domain of $\widetilde{m}_g$.

In the following proposition, it is supposed that $p_1=p_2= 2$.

#### Proposition 6 {#ts-iv-s4-prop-6 .statement tag=032Y}

a) Let $g'$ be a $\mu$-measurable function on X such that $|g|\leqslant |g'|$. One has dom($\widetilde{m}_{g'}$)$\subset$ dom($\widetilde{m}_g$) and dom($\widetilde{m}_{g'}$) is a core of the partial operator $\widetilde{m}_g$;

b) Let F be a subspace of $\mathscr{L}_K^2(X, \mu)$ whose intersection with $\mathscr{K}(X; K)$ is dense in $\mathscr{K}(X; K)$ and whose image G in $L^2_K(X, \mu)$ is contained in dom($\widetilde{m}_g$). If $|g|^2$ is locally $\mu$-integrable, then $\mathscr{K}(X; K)$ is contained in the domain of $\widetilde{m}_g$ and G is a core of $m_g$.

Let us prove a). If $f\in \mathscr{L}_K^2(X, \mu)$ belong to the domain of $m_{g'}$, so that $f g'\in \mathscr{L}_K^2(X, \mu)$, the assumption implies that $f g\in \mathscr{L}_K^2(X, \mu)$, whence the result.

Let us prove that dom($\widetilde{m}_{g'}$) is a core of $\widetilde{m}_g$, that is to say that the domain of $\widetilde{m}_{g'}$ is dense in the Hilbert space $E_{\widetilde{m}_g}$. Let $h\in \mathscr{L}_K^2(X, \mu)$

whose class $\widetilde{h}$ belong to $E_{\widetilde{m}_g}$ and is orthogonal to dom($\widetilde{m}_{g'}$). This means that

$$
(\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh h'(1 +|g|^2)d\mu= 0
$$

for every function $h'\in \mathscr{L}_K^2(X, \mu)$ whose class $\widetilde{h}'$ belongs to dom($\widetilde{m}_{g'}$).

Let C be a compact subset of X and let $\varphi$ be its characteristic function. Let $n\in \mathbf{N}$. Denote by $\varphi_n$ the characteristic function of the $\mu$-integrable set $C_n$ of the $x\in C$ such that $|h(x)|\leqslant n$ and put $h'_n=\varphi_nh$. The class of $h'_n$ belongs to the domain of $\widetilde{m}_{g'}$ since $|g'h'_n|\leqslant n\varphi$; hence

$$
0 =\int_X\overline{h}h'_n(1 +|g|^2)d\mu=\int_X|h|^2\varphi_n(1 +|g|^2)d\mu
$$

This implies that $h$ is zero for $\mu$-almost every $x\in C_n$ and therefore, since $n$ is arbitrary, that $h$ is zero for $\mu$-almost every $x\in C$. It follows finally that $h$ is zero $\mu$-almost everywhere, since C is arbitrary and $h$ is moderate (INT, V, p. 9, § 1, n$^o3$, cor.).

Let us now consider assertion b). Since $|g|^2$ is locally $\mu$-integrable, the function $f g$ belongs to $\mathscr{L}_K^2(X, \mu)$ if $f\in \mathscr{K}(X; K)$, hence $\mathscr{K}(X; K)$ is contained in the domain of $\widetilde{m}_g$.

Let $h\in \mathscr{L}_K^2(X, \mu)$ whose class $\widetilde{h}$ belongs to $E_{m_g}$ and is orthogonal to G. One then has

$$
0 = (\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh\overline{h}'(1 +|g|^2)d\mu
$$

for every $h'\in F$ of class $\widetilde{h}'$. In view of the assumption on F, this means that the measure $h(1 +|g|^2)\cdot \mu$ is zero, hence that $h$ is zero $\mu$-almost everywhere since $h$ is moderate.

Let $p$ be a real number $\geqslant 1$. Let $h$ be an element of $\mathscr{L}_K^{\infty}(X, \mu)$. The multiplication operator $\widetilde{m}_h$ by $h$ is an endomorphism of $L^p_K(X, \mu)$(IV, p. 186, No.$^o5$). Suppose that the set Y of the $x\in X$ such that $h(x) = 0$ is locally $\mu$-negligible. Then the endomorphism $\widetilde{m}_h$ is injective (Lemma 7 of IV, p. 186). Let us denote by $h^{-1}$ the function on X equal to 0 on Y and to $x\mapsto 1/h(x)$ on X- Y. The reciprocal partial operator $\widetilde{m}^{-1}_h$ is the multiplication operator by $h^{-1}$ from $L^p_K(X, \mu)$ into $L^p_K(X, \mu)$, that is to say, $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$. In fact, the image of $\widetilde{m}_h$ is the space of classes of functions $g\in \mathscr{L}_K^p(X, \mu)$ of the form $g=hf$ for $f\in \mathscr{L}_K^p(X, \mu)$. This condition is equivalent to $g(x)/h(x) =f(x)$ for every $x\in X$- Y and $g(x) = 0$ if $x\in Y$. This implies that the domain of $\widetilde{m}^{-1}_h$ in $L^p_K(X, \mu)$ is the domain of $\widetilde{m}_{h^{-1}}$, and that the equality $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$ is valid.

In what follows, we shall sometimes denote simply by $m_h$ the partial multiplication operator by $h$ from $L^{p^1}_K(X, \mu)$ into $L^{p_2}_K(X, \mu)$.

#### Example 2 {#ts-iv-s4-n3-exa-2 .statement tag=032Z}

Let E be a Hilbert space over K and $B = (e_i)_{i\in I}$ an orthonormal basis of E. Let $(\lambda_i)_{i\in I}$ be a family of elements of K. Let D be the vector subspace of E consisting of the elements $x\in E$ such that the family $(\lambda_i\langle e_i|x\rangle )_{i\in I}$ is square-summable in K. The space D is dense in E since it contains the vector $e_i$ for every $i\in I$. The partial operator $u$ with domain D given by

$$
x\mapsto \sum_{i\in I}\lambda_i\langle e_i|x\rangle e_i
$$

is called a diagonal partial operator in the basis B, and $(\lambda_i)_{i\in I}$ is called the family of eigenvalues of $u$.

The operator $u$ is closed. In fact, let $(x_n, u(x_n))_{n\in\mathbf{N}}$ be a sequence of elements of the graph of $u$ which converges in $E\times E$, and let $(x, y)$ be its limit. Then $\langle e_i|x_n\rangle  \rightarrow  \langle e_i|x\rangle$ for every $i\in I$ and

$$
\langle e_i|u(x_n)\rangle =\lambda_i\langle e_i|x_n\rangle  \rightarrow  \langle e_i|y\rangle
$$

for every $i\in I$. Consequently, $\lambda_i\langle e_i|x\rangle =\langle e_i|y\rangle$ for every $i\in I$, which proves that $x\in D$ and $u(x) =y$, that is to say that $u$ is closed.

This example is in fact a particular case of the preceding one, applied to the topological space X = I endowed with the discrete topology and the counting measure $\mu$, since E identifies with the space $\ell^2(I) = L^2(I, \mu)$ by the mapping $x\mapsto (\langle e_i|x\rangle )_{i\in I}$ (EVT, V, p. 23, cor. 2) and $u$ then identifies with the multiplication operator $m_{\lambda}$, where $\lambda$ is the function $i\mapsto \lambda_i$.

#### Example 3 {#ts-iv-s4-n3-exa-3 .statement tag=0330}

The set $\mathbf{N}_{\mathbf{R}}=\mathbf{N}\cup  \{\infty , \omega \}$ is endowed with the total ordering described in VAR, R2, p. 10, such that $n <\infty < \omega$ for every $n\in \mathbf{N}$. Let $r\in \mathbf{N}_{\mathbf{R}}$. Let $n\in \mathbf{N}$ and let U be an open subset of $\mathbf{R}^n$. Let $k\in \mathbf{N}$ be such that $k\leqslant r$. Let $(n_{\alpha})_{|\alpha|\leqslant k}$ be a family of elements of $\mathscr{C}^r$(U), where the multi-indices considered belong to $\mathbf{N}^n$. The family $(n_{\alpha})$ defines a scalar differential operator D of order $\leqslant k$ on U (cf. VAR, R2, 14.1.6, 14.1.4). For every integer $m$ such that $k\leqslant m\leqslant r$, the differential operator D defines a linear mapping of $C^m(U)$ into $C^{m-k}(U)$ which sends $f\in C^m(U)$ to

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}(f)
$$

The same formula defines a continuous linear mapping of $\mathscr{D}(U)$ into $\mathscr{D}'(U)$ (def. 2 of IV, p. 208).

#### Definition 5 {#ts-iv-s4-def-5 .statement tag=0331}

Let E be a vector subspace of $\mathscr{D}'(U)$ containing $\mathscr{D}(U)$. A differential operator associated with D on E is any partial operator on E which is an extension of the partial operator with domain $\mathscr{D}(U)$ defined by $\varphi \mapsto D(\varphi )$.

Suppose for example that the coefficients $n_{\alpha}$ are bounded functions on U. Let $\mu$ be the Lebesgue measure on U. If $p$ is an element of $[1,+\infty [$, one can then define on $L^p(U)$ a differential operator associated with D whose domain is the Sobolev space $W^{k,p}(U)$ (No. 14 of IV, p. 221), since in this case one has $n_{\alpha}\partial^{\alpha}(f)\in L^p(U)$ for every $f\in W^{k,p}(U)$ and every $|\alpha |\leqslant k$.

### 4. Adjoint

In this No., K is one of the fields $\mathbf{R}$ or $\mathbf{C}$, and E and F denote Hilbert spaces over K.

Let $u$ be an operator with dense domain from E into F. Let D denote the domain of $u$. For $y\in F$, let $\lambda_y$ be the linear form on D such that $\lambda_y(x) =\langle y|u(x)\rangle$ for every $x\in D$. We denote by $D^*$ the set of vectors $y\in F$ such that $\lambda_y$ is continuous on D. It is a vector subspace of F. Let $y\in D^*$; since D is dense in E, the linear form $\lambda_y$ extends in a unique way to a continuous linear form on E, which we again denote by $\lambda_y$. By EVT, V, p. 15, Theorem 3, there exists a unique element $u^*(y)$ in E such that $\lambda_y(x) =\langle u^*(y)|x\rangle$ for every $x\in E$. The mapping $y\mapsto u^*(y)$ is linear from $D^*$ into E.

#### Definition 6 {#ts-iv-s4-def-6 .statement tag=0332}

The partial operator from F into E with domain $D^*$ defined by $y\mapsto u^*(y)$ is called the adjoint of $u$. It is denoted by $u^*$.

#### Remark {#ts-iv-s4-n4-rem-9 .statement tag=0333}

Thus $y\in D^*$ if and only if there exists $c\in \mathbf{R}_+$ such that $|\langle y|u(x)\rangle |\leqslant c\|x\|$ for every $x\in D$. The element $u^*(y)$ is then characterised by the relation

$$
\langle y|u(x)\rangle =\langle u^*(y)|x\rangle \tag{1}
$$

for every $x\in D$. We then have $|\langle y|u(x)\rangle |\leqslant \|u^*(y)\| \|x\|$ for every $x\in D$.

In the case where $u$ is a continuous linear mapping from E into F, its adjoint in the sense of the preceding definition coincides with the adjoint defined in EVT, V, p. 38, Definition 1, since $D^*$ is equal to F in this case.

Let $v\in \mathscr{P}(E; F)$ be such that $u\subset v$. Then $v^*\subset u^*$.

Let $v\in \mathscr{P}(E; F)$ be such that $u+v$ has dense domain. Then the partial operator $v$ has dense domain and we have $u^*+v^*\subset (u+v)^*$. In general, there is no equality (exercise 9 of IV, p. 347). If $v\in \mathscr{L}(E; F)$, then $u+v$ has dense domain and $(u+v)^*=u^*+v^*$. This is so, for example, if F = E and if $v=\lambda 1_E$ where $\lambda \in K$.

Let G be a Hilbert space over K and let $v\in \mathscr{P}(F; G)$ be an operator with dense domain. If $v\circ u$ has dense domain, then $u^*\circ v^*\subset (v\circ u)^*$. In general, there is no equality (loc. cit.). If $u$ (resp. $v$) is an isomorphism, then $v\circ u$ has dense domain and we have $(v\circ u)^*=u^*\circ v^*$. This is so, for example, if E = F (resp. F = G) and $u=\lambda 1_E$ (resp. $v=\lambda 1_F$) where $\lambda \in K^*$.

Let $s$ denote the isometric isomorphism of Hilbert spaces from $E\oplus F$ into $F\oplus E$ defined by $s(x, y) = (-y, x)$ for every $(x, y)\in E\oplus F$.

#### Proposition 7 {#ts-iv-s4-prop-7 .statement tag=0334}

Let $u$ be a partial operator with dense domain from E into F.

a) The graph of $u^*$ is equal to $s(\Gamma^{\circ}_u) =s(\Gamma_u)^{\circ}$;

b) The partial operator $u^*$ is closed;

c) The kernel of $u^*$ is the orthogonal of the image of $u$.

Let us put $W =s(\Gamma_u)^{\circ}$. Since the linear mapping $s$ is unitary, we have $W =s(\Gamma^{\circ}_u)$.

We have $(y, x)\in W$ if and only if

$$
\langle (y, x)|(-u(x'), x')\rangle = 0
$$

for all $x'\in$ dom($u$), that is to say, if

$$
\langle y|u(x')\rangle =\langle x|x'\rangle
$$

for all $x'\in$ dom($u$). When $y\in$ dom($u^*$) and $x=u^*(y)$, this property holds (cf. formula (1), p. 236). Conversely, if this condition is satisfied, it follows that $|\langle y|u(x')\rangle |\leqslant \|x\| \|x'\|$ for all $x'\in$ dom($u$), whence it follows that $y$ belong to dom($u^*$); one then has $u^*(y) =x$. Hence $W = \Gamma_{u^*}$.

The operator $u^*$ is closed, because the space $s(\Gamma_u)^{\circ}$ is closed in $F\oplus E$.

Let us prove assertion c). If $y$ is orthogonal to the image of $u$, the linear form $\lambda_y:x\mapsto  \langle y|u(x)\rangle$ on D is zero, hence $y\in$ dom($u^*$) and $u^*(y) = 0$. Conversely, let $y\in$ dom($u^*$). Then $u^*(y) = 0$ if and only if $y$ is orthogonal to $u(x)$ for all $x\in D$ (formula (1), p. 236).

#### Proposition 8 {#ts-iv-s4-prop-8 .statement tag=0335}

Let $u$ be an operator with dense domain from E into F. Then $u^*$ has dense domain if and only if $u$ is closable. When this is so, the closure $\overline{u}$ of $u$ is equal to $u^{**}$, and the adjoint of $\overline{u}$ is equal to $u^*$.

By Prop. 7, the partial operator $u^*$ is closed. Suppose that the domain $D^*$ of $u^*$ is dense in F. Let $u^{**}$ be the adjoint of $u^*$; it is a closed partial operator from E into F. Let us prove that $u\subset u^{**}$, which will imply that $u$ is closable. Let $x\in$ dom($u$). By definition of $u^*$, the linear forms on $D^*$ given by $y\mapsto  \langle x|u^*(y)\rangle$ and $y\mapsto  \langle u(x)|y\rangle$ are equal; hence $x\in$ dom($u^{**}$) and $u^{**}(x) =u(x)$, whence the assertion.

Conversely, suppose that $u$ is closable; one has $\Gamma_{\overline{u}}=\overline{\Gamma}_u$ (Prop. 1 of IV, p. 228). Let $y\in F$ be a vector orthogonal to dom($u^*$). The element $(y,0)$ of $F\oplus E$ then belongs to the orthogonal complement of the graph of $u^*$. But, by Prop. 7, a), one has

$$
\Gamma^{\circ}_{u^*}= (s(\Gamma_u)^{\circ})^{\circ}=s(\Gamma_u) =s(\Gamma_u)
$$

It follows therefore that $(0, y)\in \Gamma_{\overline{u}}$, whence $y=\overline{u}(0) = 0$. Since the orthogonal complement of dom($u^*$) is reduced to 0, the space dom($u^*$) is dense in F.

Finally, Prop. 7, applied to $u^*$, implies that

$$
\Gamma_{u^{**}}=s^{-1}(\Gamma^{\circ}_{u^*}) =s^{-1}(s(\Gamma^{\circ \circ}_u)) =\overline{\Gamma}_u
$$

hence $u^{**}=\overline{u}$, then $\overline{u}^*= (u^*)^{**}=\overline{u^*}=u^*$ since $u^*$ is closed.

#### Corollary {#ts-iv-s4-n4-cor-1 .statement tag=0336}

If $u$ is a closed partial operator with dense domain from E into F, then $u^*$ has dense domain and one has $u^{**}=u$.

#### Definition 7 {#ts-iv-s4-def-7 .statement tag=0337}

Let $u$ be a partial operator on E. One says that $u$ is symmetric if $u$ has dense domain and if $u^*$ is an extension of $u$. One says that $u$ is self-adjoint if $u$ has dense domain and $u^*=u$. One says that $u$ is essentially self-adjoint if it is closable and if the closure $\overline{u}$ of $u$ is self-adjoint.

One says that $u$ is a partial operator bounded below if $u$ is symmetric and if there exists a real number $c$ such that $\langle x|u(x)\rangle \geqslant c\|x\|^2$ for every $x$ belonging to the domain of $u$. One then says that $c$ is a lower bound of $u$. If $c= 0$, one also says that $u$ is a positive partial operator.

We denote by $\mathscr{A}(E)$ the set of self-adjoint partial operators on E.

#### Remark 1 {#ts-iv-s4-n4-rem-1 .statement tag=0338}

For an operator $u$ with dense domain on E to be symmetric, it is necessary and sufficient that one have

$$
\langle x|u(y)\rangle =\langle u(x)|y\rangle \tag{2}
$$

for every $(x, y)\in$ dom($u$)$^2$. This formula in fact shows that the domain of $u$ is contained in that of $u^*$, and then that $u^*$ and $u$ coincide on the domain of $u$. In particular, it follows that $\langle x|u(x)\rangle  \in \mathbf{R}$ for every $x\in$ dom($u$).

As will be seen in different examples, formula (2) can often be verified by a straightforward calculus. On the other hand, the exact determination of the domain of the adjoint, which alone makes it possible to know whether or not a symmetric operator is self-adjoint, may be very delicate.

#### Remark 2 {#ts-iv-s4-n4-rem-2 .statement tag=0339}

A self-adjoint partial operator $u$ is essentially self-adjoint (cf. prop. 8).

#### Remark 3 {#ts-iv-s4-n4-rem-3 .statement tag=033A}

Let $u$ be a symmetric partial operator on E. The operator $u$ is closable (prop. 7, b)). It satisfies dom($u$)$\subset$ dom($u^*$), and $u$ is self-adjoint if and only if dom($u$) $=$ dom($u^*$). Moreover, the closure $\overline{u}$ of $u$ is symmetric since $\overline{u}\subset u^*=\overline{u}^*$ (prop. 8).

#### Remark 4 {#ts-iv-s4-n4-rem-4 .statement tag=033B}

Suppose $K =\mathbf{C}$. Let $u\in \mathscr{P}(E; E)$ be a partial operator with dense domain. The condition $\langle x|u(x)\rangle  \in \mathbf{R}$ for every $x\in$ dom($u$) implies that $u$ is symmetric (EVT, V, p. 2, remark); in particular, if $\langle x|u(x)\rangle  \in \mathbf{R}_+$ for every $x\in$ dom($u$), then $u$ is positive.

#### Remark 5 {#ts-iv-s4-n4-rem-5 .statement tag=033C}

Let $u$ and $v$ be symmetric partial operators on E. If $u$ is self-adjoint and if $u\subset v$, then $v\subset v^*\subset u^*=u$, hence $u=v$.

#### Remark 6 {#ts-iv-s4-n4-rem-6 .statement tag=033D}

An essentially self-adjoint partial operator $u$ is symmetric, since $u\subset \overline{u}$ implies $\overline{u}=\overline{u}^*\subset u^*$, hence $u\subset u^*$.

#### Remark 7 {#ts-iv-s4-n4-rem-7 .statement tag=033E}

Let $u$ and $v$ be symmetric partial operators on E. If $u+v$ has dense domain, for example if $u$ or $v$ belong to $\mathscr{L}$ (E), then $u+v$ is symmetric. In general, the partial operator $u+v$ is not self-adjoint, even if $u$ and $v$ are (exercise 9 of IV, p. 347).

#### Remark 8 {#ts-iv-s4-n4-rem-8 .statement tag=033F}

Let $u$ be a symmetric partial operator on E. A real number $c$ is a lower bound of $u$ if and only if the operator $u-c\cdot 1_E$ is positive.

#### Lemma 3 {#ts-iv-s4-lem-3 .statement tag=033G}

Suppose that $K =\mathbf{R}$. Let $u$ be a partial operator with dense domain from E into F.

a) The adjoint of $u_{(\mathbf{C})}$ is $(u^*)_{(\mathbf{C})}$;

b) Suppose that E = F; the partial operator $u$ is symmetric (resp. self-adjoint) if and only if the partial operator $u_{(\mathbf{C})}$ is symmetric (resp. self-adjoint).

Let us prove a). Let $y\in F_{(\mathbf{C})}$ and write $y=y_1+iy_2$ with $y_1,y_2\in F$. For all $(x_1, x_2)\in E\times E$, we have

$$
\langle u_{(\mathbf{C})}(x_1+ix_2)|y\rangle =\langle u(x_1)|y_1\rangle +i\langle u(x_1)|y_2\rangle
$$

$$
-i\langle u(x_2)|y_1\rangle +\langle u(x_2)|y_2\rangle
$$

If $y\in$ dom($u^*$)$_{(\mathbf{C})}$, it follows that $y\in$ dom(($u_{(\mathbf{C})}$)$^*$) and that $u^*_{(\mathbf{C})}(y) = (u_{(\mathbf{C})})^*(y)$, hence $u^*_{(\mathbf{C})}\subset (u_{(\mathbf{C})})^*$.

Conversely, suppose that $y$ belongs to dom(($u_{(\mathbf{C})}$)$^*$). Taking $x_2= 0$ (resp. $x_1= 0$) in the above formula, we verify that $y_1\in$ dom($u^*$) (resp. that $y_2\in$ dom($u^*$)), whence $y\in$ dom($u^*$)$_{(\mathbf{C})}$.

Assertion a) implies that $u_{(\mathbf{C})}$ is symmetric (resp. self-adjoint) if $u$ is.

Conversely, suppose that $u_{(\mathbf{C})}$ is symmetric. The relation $\langle u(x)|y\rangle =\langle x|u(y)\rangle$ for all $(x, y)\in$ dom($u_{(\mathbf{C})}$)$\times$ dom($u_{(\mathbf{C})}$) implies that $u$ is symmetric on taking $x$ and $y$ in the subspace dom($u$) of dom($u_{(\mathbf{C})}$). If $u_{(\mathbf{C})}$ is self-adjoint, what precedes proves that $u$ is symmetric; since dom($u^*$) $=$ dom($u^*_{(\mathbf{C})}$)$\cap F$, assertion a) implies that dom($u^*$) $=$ dom($u_{(\mathbf{C})}$)$\cap F =$ dom($u$), therefore $u$ is self-adjoint.

### 5. Elementary Criteria for Self-Adjoint Operators

#### Proposition 9 {#ts-iv-s4-prop-9 .statement tag=033H}

Let $v\in \mathscr{L}(F; E)$ be an injective continuous linear mapping of F into E whose image is dense in E. The adjoint of $v$ is an injective continuous linear mapping of E into F and one has $(v^*)^{-1}= (v^{-1})^*$. In particular, if E = F, the endomorphism $v$ is hermitian if and only if the partial operator $v^{-1}$ is self-adjoint.

The partial operator $v^{-1}$ is a closed operator with dense domain from E into F (Example 2 of IV, p. 228), and the adjoint $v^*$ of $v$ is a continuous linear mapping from E into F; it is injective, since the image of $v$ is dense in E (EVT, V, p. 41, prop. 4). Let $s$ (resp. $s'$) be the isometric isomorphism $(x, y)\mapsto (-y, x)$ of $E\oplus F$ onto $F\oplus E$ (resp. the isometric isomorphism $(y, x)\mapsto (-x, y)$ of $F\oplus E$ onto $E\oplus F$), and let $\iota$ (resp. $\iota '$) be the isometric isomorphism $(y, x)\mapsto (x, y)$ of $F\oplus E$ onto $E\oplus F$ (resp. the isometric isomorphism $(x, y)\mapsto (y, x)$ of $E\oplus F$ onto $F\oplus E$). Then $s\circ \iota =-\iota '\circ s'$, whence

$$
\Gamma_{(v^{-1})^*}=s(\Gamma_{v^{-1}})^{\circ}=s(\iota (\Gamma_v))^{\circ}=-\iota '(s'(\Gamma_v))^{\circ}=-\iota '(\Gamma_{v^*}) = \Gamma_{(v^*)^{-1}}
$$

by prop. 7 of IV, p. 236. The proposition follows.

#### Proposition 10 (Hellinger–Toeplitz) {#ts-iv-s4-prop-10 .statement tag=033I}

Let $u$ be a symmetric partial operator on the Hilbert space E. If the domain of $u$ is equal to E, then $u\in \mathscr{L}(E)$ and $u$ is hermitian.

In fact, the partial operator $u$ is closable (prop. 8 of IV, p. 237), and therefore closed since its domain is E (IV, p. 228, Remark). We then conclude by invoking EVT, I, p. 19, cor. 5.

#### Corollary {#ts-iv-s4-n5-cor-1 .statement tag=033J}

Let $u$ be a symmetric partial operator on E. If the partial operator $u$ induces a bijective linear mapping of dom($u$) onto E, then $u$ is self-adjoint.

In fact, the inverse partial operator $u^{-1}$ of $u$ is symmetric with domain E (prop. 9), hence $u^{-1}$ is a self-adjoint element of $\mathscr{L}(E)$ (prop. 10), and $u$ is therefore hermitian (prop. 9).

#### Proposition 11 {#ts-iv-s4-prop-11 .statement tag=033K}

Let $u$ be a symmetric partial operator on E, and let $\lambda \in \mathbf{C}$. If $u+\lambda 1_E$ and $u+\lambda 1_E$ are surjective, then $u$ is self-adjoint.

It is enough to prove that dom($u^*$)$\subset$ dom($u$). Let $x\in$ dom($u^*$). By hypothesis there exists $y\in$ dom($u$) such that $u(y) +\lambda y=u^*(x) +\lambda x$. Let us prove that $y=x$. For every $z\in$ dom($u$), we have

$$
\langle (u+\lambda 1_E)(z)|x\rangle =\langle z|(u^*+\overline{\lambda}1_E)(x)\rangle
$$

$$
=\langle z|(u+\overline{\lambda}1_E)(y)\rangle =\langle (u+\lambda 1_E)(z)|y\rangle
$$

since $u$ is symmetric. Since the operator $u+\lambda 1_E$ is surjective, we indeed have $y=x$, hence $x\in$ dom($u$).

We shall see later (cf. prop. 17 of IV, p. 248) that if $\lambda \in \mathbf{C}-\mathbf{R}$, then the converse is true.

#### Proposition 12 {#ts-iv-s4-prop-12 .statement tag=033L}

Let $u$ be a closed operator with dense domain from E into F. The partial operator $u^*\circ u$ on E is self-adjoint and positive. Its domain is a core for $u$.

Let us denote by $v$ the partial operator $1_E+u^*\circ u$. Its domain is dom($u^*\circ u$), which is contained in dom($u$). For all $x\in$ dom($u$) and $y\in$ dom($v$), one has $u(y)\in$ dom($u^*$) and

$$
\langle x|v(y)\rangle =\langle x|y\rangle +\langle x|(u^*\circ u)(y)\rangle =\langle x|y\rangle +\langle u(x)|u(y)\rangle \tag{3}
$$

$$
\langle y|v(y)\rangle =\|y\|^2+\|u(y)\|^2 \tag{4}
$$

Formula (4) implies that the partial operator $v$ is injective. Moreover, by prop. 7 of IV, p. 236, a), one has $F\oplus E = \Gamma_{u^*}\oplus s(\Gamma_u)$. Let $x\in E$. There exist $y'\in$ dom($u^*$) and $x'\in$ dom($u$) such that

$$
(0, x) = (y', u^*(y')) + (-u(x'), x') = (y'-u(x'), x'+u^*(y'))
$$

Hence one has $y'=u(x')$, whence $x'\in$ dom($u^*\circ u$) $=$ dom($v$) and

$$
x=x'+u^*(y') =x'+ (u^*\circ u)(x') =v(x')
$$

The partial operator $v$ on E is therefore surjective, and induces a bijective linear mapping of dom($v$) onto E.

Let $x\in E$ be orthogonal to dom($v$). Write $x=v(x')$ where $x'\in$ dom($v$). By formula (4), one obtains

$$
0 =\langle x'|x\rangle =\langle x'|v(x')\rangle =\|x'\|^2+\|u(x')\|^2
$$

whence $x'= 0$, and then $x= 0$. The domain of $v$ is therefore dense in E.

The partial operator $v$ has dense domain; it is bijective and formula (3) shows that it is symmetric. One concludes that $v$ is self-adjoint by applying the corollary to proposition 10. Consequently, $u^*\circ u=v-1_E$ is self-adjoint. Moreover, the formula

$$
\langle x|(u^*\circ u)(x)\rangle =\|u(x)\|^2
$$

for all $x\in$ dom($u^*\circ u$) implies that $u^*\circ u$ is positive.

Finally, let $y\in E_u$ be orthogonal to dom($u^*\circ u$). There exists an element $x$ in the domain of $u^*\circ u$ such that $y=v(x) =x+ (u^*\circ u)(x)$. One then has $0 = (x|y)_u=\langle y|y\rangle$, whence $y= 0$.

### 6. Differential operators

Let $n\in \mathbf{N}$ and U be an open set in $\mathbf{R}^n$. We endow $\mathbf{R}^n$ and U with the Lebesgue measure denoted by $\mu$.

Let $k\in \mathbf{N}$ and $h\in \mathbf{N}$ be such that $h\geqslant k$. Let D be a scalar differential operator on U of order $\leqslant k$, with coefficients $(n_{\alpha})_{|\alpha|\leqslant k}$ of class $C^h$ on U. Suppose that for every $\alpha$ such that $|\alpha |\leqslant k$ and every $\beta$ such that $0\leqslant \beta \leqslant \alpha$, the function $\partial^{\beta}n_{\alpha}$ is bounded on U.

Let $^tD$ be the scalar differential operator on U transpose of D (VAR, R2, 14.3.2); it is of order $\leqslant k$ and of class $C^{h-k}$; for $\varphi \in \mathscr{D}$(U), one has

$$
^tD(\varphi ) =\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\partial^{\alpha}(\overline{n}_{\alpha}\varphi )
$$

(loc. cit.); in particular, the coefficients of $^tD$ are bounded on U.

We denote by $D_-$ the partial operator on $L^2(U)$ with domain $\mathscr{D}(U)$ defined by

$$
\varphi \mapsto D(\varphi ) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}\varphi \tag{5}
$$

Let $H_D$ be the space of $f\in L^2(U)$ such that the distribution

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}f
$$

belongs to $L^2(U)$; we denote by $D_+$ the partial operator with domain $H_D$ defined by $f\mapsto D(f)$.

Since one has $\partial^{\alpha}f\in L^2(U)$ if $f\in H^k(U)$ and $|\alpha |\leqslant k$, the Sobolev space $H^k(U)$ is contained in $H_D$; in general, these spaces are distinct.

One has $D_-\subset D_+$, and these are differential operators associated with D on $L^2(U)$ (def. 5 of IV, p. 235).

#### Proposition 13 {#ts-iv-s4-prop-13 .statement tag=033M}

Let $u$ be a partial operator on $L^2(U)$. If $D_-\subset u\subset D_+$, then $u$ is closable and $(^tD)_-\subset u^*\subset (^tD)_+$.

Let $\varphi$ and $\psi$ belong to $\mathscr{D}(U)$. Then one has

$$
\langle \varphi |D(\psi )\rangle =\sum_{|\alpha|\leqslant}\int_{kU}n_{\alpha}\varphi  \partial^{\alpha}\psi  d\mu
$$

$$
=\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}\varphi )|\psi \rangle =\langle^tD(\varphi )|\psi \rangle
$$

(cf. VAR, R2, 14.3.8). Since $\mathscr{D}(U)$ is dense in $L^2(U)$ (prop. 4 of IV, p. 202), this implies that $\varphi \in$ dom($u^*$) and $u^*(\varphi ) =^tD(\varphi )$. Hence one has $(^tD)_-\subset u^*$; in particular, $u^*$ has dense domain and $u$ is closable (prop. 8 of IV, p. 237).

Let $f\in$ dom($u^*$) and $\varphi \in \mathscr{D}(U)$. Since $\mathscr{D}(U)\subset$ dom($u$), the distribution associated with $u^*(f)$ satisfies

$$
\langle u^*(f), \varphi \rangle =\langle \overline{\varphi}|u^*(f)\rangle =\langle u(\overline{\varphi})|f\rangle
$$

Since $D_-\subset u$, $u(\overline{\varphi})$ is calculated by formula (5), whence

$$
\langle u^*(f), \varphi \rangle =\sum_{\alpha}\langle n_{\alpha}\partial^{\alpha}\overline{\varphi}|f\rangle =\sum_{\alpha}\langle \partial^{\alpha}\overline{\varphi}|\overline{n}_{\alpha}f\rangle
$$

$$
=\sum_{\alpha}\langle \overline{n}_{\alpha}f, \partial^{\alpha}\varphi \rangle =\sum_{\alpha}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}f), \varphi \rangle =\langle^tD(f), \varphi \rangle
$$

The distributions $u^*(f)$ and $^tD(f)$ are therefore equal; the distribution $f$ therefore belongs to $H_{_tD}$ and $u^*(f) =^tD(f)$, whence $u^*\subset (^tD)_+$.

#### Remark {#ts-iv-s4-n6-rem-1 .statement tag=033N}

The proposition means that the adjoint of a partial operator $u$ such that $D_-\subset u\subset D_+$ can always be calculated in the sense of distributions: the elements $f$ of the domain of $u^*$ are elements of $L^2(U)$ such that the distribution $^tD(f)$ belongs to $L^2$(U), and one has $u^*(f) =^tD(f)$.

One says that D is formally symmetric if $^tD = D$ as a scalar differential operator. If this is the case, the partial operator $D_-$ is symmetric.

Consider the particular case of the scalar differential operator of order 2 defined by

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

A Laplacian on U is any partial operator $u$, self-adjoint on $L^2$(U), such that $\Delta_-\subset u($cf. VAR, R2, 14.4.3, p. 83). We shall see later (IV, p. 261, example) that there always exists at least one Laplacian on $L^2(U)$; there may exist more than one (exercise 17 of IV, p. 358).

### 7. Spectrum and Resolvent

#### Lemma 4 {#ts-iv-s4-lem-4 .statement tag=033O}

Let E be a complex Banach space and let $u$ be a closed injective partial operator on E such that $u^{-1}\in \mathscr{L}(E)$. Let $v\in \mathscr{L}(E)$ be such that $\|v\|<\|u^{-1}\|^{-1}$. Then the partial operator $u+v$ is injective, one has $(u+v)^{-1}\in \mathscr{L}(E)$, and

$$
(u+v)^{-1}=u^{-1}\circ \sum_{k=0}^{+\infty}(-vu^{-1})^k \tag{6}
$$

where the series is absolutely convergent in $\mathscr{L}(E)$. Moreover, one has

$$
\|(u+v)^{-1}\|\leqslant \|u^{-1}\|_{-1}
$$

$$
1- \|v\| \|u\|
$$

Since $\|v\| \|u^{-1}\|<1$, the series with general term $(-vu^{-1})^k$ is absolutely convergent in $\mathscr{L}$ (E), and its sum is the inverse of the endomorphism $1_E+vu^{-1}$ (prop. 2 of I, p. 22). Consequently, the partial operator $(1_E+vu^{-1})\circ u=u+v($IV, p. 226, rem. vi) is injective and the reciprocal partial operator $(u+v)^{-1}=u^{-1}\circ (1_E+vu^{-1})^{-1}($IV, p. 226, rem. iii) belongs to $\mathscr{L}(E)$. Since

$\|(1_E+vu^{-1})^{-1}\|\leqslant \sum^{+\infty}(\|v\| \|u^{-1}\|)^k=$ 1 $_{-1}$,

$$
1- \|v\| \|u\|
$$

$k=0$

the lemma is proved.

#### Definition 8 {#ts-iv-s4-def-8 .statement tag=033P}

Let $u$ be a closed operator with dense domain on a complex Banach space E. The resolvent set of $u$ is the set of complex numbers $\lambda$ such that the partial operator $\lambda 1_E-u$ is injective and its inverse $(\lambda 1_E-u)^{-1}$ belongs to $\mathscr{L}(E)$.

The spectrum of $u$, denoted by Sp($u$), is the complement of the resolvent set in $\mathbf{C}$.

If $\lambda \in \mathbf{C}-$ Sp($u$), we denote by $R(u, \lambda )\in \mathscr{L}(E)$ the inverse of $\lambda 1_E-u$. The mapping of $\mathbf{C}-$ Sp($u$) into $\mathscr{L}(E)$ which associates $R(u, \lambda )$ to $\lambda$ is called the resolvent of $u$.

#### Remark {#ts-iv-s4-n7-rem-1 .statement tag=033Q}

Let E be a complex Banach space and let $u$ be a closed operator with dense domain on E.

1) If $u\in \mathscr{L}$ (E), its spectrum coincides with the spectrum of the element $u$ of the algebra $\mathscr{L}(E)$(I, p. 2, Definition 1).

2) Let D be the domain of $u$. For every $\lambda \in \mathbf{C}-$ Sp($u$), one has

$$
1_E= (\lambda 1_E-u)\circ R(u, \lambda ),1_D= R(u, \lambda )\circ (\lambda 1_E-u) \tag{7}
$$

Moreover, for $\lambda_1$ and $\lambda_2$ in the resolvent set of $u$, one has

$$
R(u, \lambda_1)-R(u, \lambda_2) = (\lambda_2-\lambda_1)R(u, \lambda_2)\circ R(u, \lambda_1) \tag{8}
$$

$$
R(u, \lambda_1)\circ R(u, \lambda_2) = R(u, \lambda_2)\circ R(u, \lambda_1) \tag{9}
$$

In fact, one has

$$
R(u, \lambda_1)-R(u, \lambda_2) = R(u, \lambda_1)\circ 1_E-1_D\circ R(u, \lambda_2)
$$

Since $1_E= (\lambda_21_E-u)\circ R(u, \lambda_2)$ and $1_D= R(u, \lambda_1)\circ (\lambda_11_E-u)$, one obtains

$$
R(u, \lambda_1)-R(u, \lambda_2) =\lambda_2R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
-R(u, \lambda_1)\circ u\circ R(u, \lambda_2)-\lambda_1R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
+ R(u, \lambda_1)\circ u\circ R(u, \lambda_2)
$$

whence the first formula. By interchanging the roles of $\lambda_1$ and $\lambda_2$, one deduces the second formula.

3) Let $\lambda \in \mathbf{C}$. By the closed graph theorem (EVT, I, p. 19, Corollary 5), if the linear mapping of dom($u$) into E defined by $x\mapsto (\lambda 1_E-u)(x)$ is bijective, then its inverse, whose graph is closed, is continuous from E into E. Therefore $\lambda$ belongs to the resolvent set of $u$ if and only if the mapping $x\mapsto (\lambda 1_E-u)(x)$ of dom($u$) into E is bijective.

4) If $\lambda$ belongs to the spectrum of $u$, one of the following properties holds:

(i) The kernel of $\lambda 1_E-u$ is not reduced to 0; one then says that $\lambda$ is an eigenvalue of $u$, and that the dimension of Ker($\lambda 1_E-u$) is its multiplicity;

(ii) The partial operator $\lambda 1_E-u$ is injective and its image is not dense in E; one then says that $\lambda$ belongs to the residual spectrum of $u$;

(iii) The partial operator $\lambda 1_E-u$ is injective, its image is dense in E, but $\lambda 1_E-u$ is not surjective; one then says that $\lambda$ belongs to the continuous spectrum of $u$.

5) Let $\lambda$ be a complex number belonging to the resolvent set of $u$. The resolvent $R(u, \lambda )$ is an injective linear mapping of E into E; its image is the domain of $u$ and $u=\lambda 1_E-R(u, \lambda )^{-1}($cf. IV, p. 226). Conversely, this property characterizes the resolvent set and the resolvent. Precisely, let $\lambda \in \mathbf{C}$; if there exists a continuous injective linear mapping $w$ of E into E such that $u=\lambda 1_E-w^{-1}$, then $\lambda$ belongs to the resolvent set of $u$ and $w= R(u, \lambda )$.

In particular, if $v$ is a closed operator with dense domain on E, and if $\lambda \in \mathbf{C}$ is a complex number not belonging to Sp($u$)$\cup$ Sp($v$), then the equality $R(u, \lambda ) = R(v, \lambda )$ implies that $u=v$.

6) The spectrum of a closable partial operator $u$ is defined as the spectrum of its closure.

There exist closed operators whose spectrum is empty, or whose spectrum is equal to $\mathbf{C}$ (exercise 12 of IV, p. 347).

Let E be a complex Banach space and $u$ a closed operator with dense domain on E. If F is a complex Banach space and if $v: E\rightarrow F$ is an isomorphism, then one has Sp($v\circ u\circ v^{-1}$) $=$ Sp($u$) and $R(v\circ u\circ v^{-1}, \lambda ) =v\circ R(u, \lambda )\circ v^{-1}$ for every $\lambda  \notin$ Sp($u$).

#### Proposition 14 {#ts-iv-s4-prop-14 .statement tag=033R}

Let E be a complex Banach space. Let $u$ be a closed operator with dense domain on E and U its resolvent set.

a) For every $\lambda \in U$, the open disc in $\mathbf{C}$ with center $\lambda$ and radius $\|R(u, \lambda )\|^{-1}$ is contained in U;

b) The set U is open in $\mathbf{C}$;

c) Suppose that Sp($u$) is not empty. Let $\lambda \in U$ and denote by $\delta$ the distance in $\mathbf{C}$ from $\lambda$ to the spectrum of $u$. One has $\delta  >0$ and $\|R(u, \lambda )\|\geqslant 1/\delta$;

d) The mapping $\lambda \mapsto R(u, \lambda )$ is a holomorphic mapping of U into $\mathscr{L}(E)$. For every integer $k\in \mathbf{N}$ and every $\lambda \in U$, one has

$\frac{\partial^k}{\partial \lambda^k}R(u, \lambda ) = (-1)^kk$!R($u, \lambda$ )$^{k+1}$.

Let $\lambda \in U$. For every $\mu\in \mathbf{C}$ such that $\|(\mu-\lambda )1_E\|<\|R(u, \lambda )\|^{-1}$, lemma 4 applied to the injective partial operator $\lambda 1_E-u$ and to $v= (\mu-\lambda )1_E$ implies that the partial operator $\mu1_E-u=\lambda 1_E-u+v$ is injective and has a continuous inverse. This implies a). According to loc. cit., one also has the formula

$$
R(u, \mu) = R(u, \lambda )\circ \sum_{k\in\mathbf{N}}(\lambda -\mu)^kR(u, \lambda )^k
$$

which implies that the resolvent of $u$ is holomorphic in U.

Assertion b) results at once from a). If Sp($u$) is nonempty, the distance from $\lambda$ to Sp($u$) is strictly positive (TG, IX, p. 13, Prop. 2), whence c).

The last part of assertion d) is proved by induction on $k$, the case $k= 1$ being a consequence of formula (8), p. 245.

#### Proposition 15 {#ts-iv-s4-prop-15 .statement tag=033S}

Let $u$ be a closed operator with dense domain on a complex Banach space E and $\lambda$ a complex number belonging to the resolvent set of $u$.

a) The subset Sp(R($u, \lambda$ ))$-\{0\}$ of $\mathbf{C}$ is the image of the spectrum of $u$ under the mapping $\mu\mapsto (\lambda -\mu)^{-1}$ of $\mathbf{C}-\{\lambda \}$ into $\mathbf{C}^*$;

b) For every $\mu\not =\lambda$ in $\mathbf{C}$, one has

Ker($\mu1_E-u$) $=$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda )$).

Let us prove assertion a). For every $\mu\not =\lambda$, we compute

$$
\mu1_E-u= (\lambda -\mu) ((\lambda -\mu)^{-1}1_E-R(u, \lambda )) (\lambda 1_E-u)
$$

Since $\lambda  \notin$ Sp($u$) and $\mu\not =\lambda$, the linear mapping $(\lambda -\mu)(\lambda 1_E-u)$ is a bijection of dom($u$) onto E. Consequently, this formula implies that $\mu1_E-u$ is a bijection of dom($u$) onto E if and only if $(\lambda -\mu)^{-1}1_E-R(u, \lambda )$ is a bijection of E onto E, which implies the assertion.

Let us prove b). If $\mu\not =\lambda$ and $x\in$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda )$), then $x\in$ dom($u$) and the formula $1_E= (\lambda 1_E-u)\circ R(u, \lambda )$ implies that $x\in$ Ker($\mu1_E-u$). Conversely, if $x\in$ Ker($\mu1_E-u$) and $\mu\not =\lambda$, the formula $1_{dom(u)}= R(u, \lambda )\circ (\lambda 1_E-u)$ implies $R(u, \lambda )(x) = (\lambda -\mu)^{-1}x$.

#### Proposition 16 {#ts-iv-s4-prop-16 .statement tag=033T}

Let $u$ be a closed operator with dense domain on a complex Hilbert space E. The spectrum of $u^*$ is the image of the spectrum of $u$ under complex conjugation and, for every element $\lambda$ of the resolvent set of $u$, one has $R(u, \lambda )^*= R(u^*, \lambda )$. In particular, if $u$ is self-adjoint, the endomorphism $R(u, \lambda )$ is normal for every $\lambda  \notin$ Sp($u$).

Let $\lambda \in \mathbf{C}-$ Sp($u$) be an element of the resolvent set of $u$. One has $u=\lambda 1_E-R(u, \lambda )^{-1}$, hence

$$
u^*=\overline{\lambda}1_E-(R(u, \lambda )^{-1})^*=\overline{\lambda}1_E-(R(u, \lambda )^*)^{-1}
$$

(IV, p. 236 and prop. 9 of IV, p. 239). Applying remark 5, we deduce that $\overline{\lambda}\in \mathbf{C}-$ Sp($u^*$) and that $R(u, \lambda )^*= R(u^*, \lambda )$. Consequently, the spectrum of $u^*$ is contained in the image of Sp($u$) under complex conjugation. We obtain equality by applying this property to $u^*$, since $u^{**}=u$ (cor. to prop. 8 of IV, p. 237). The last assertion then results from formula (9), p. 245.

#### Corollary {#ts-iv-s4-n7-cor-1 .statement tag=033U}

Let $u$ be a self-adjoint partial operator on a complex Hilbert space E. If E is not zero, then the spectrum of $u$ is not empty.

Suppose that Sp($u$) is empty. Then $u$ is injective and $u^{-1}=-R(u,0)$ is an injective endomorphism of E such that Sp($u^{-1}$)$\subset  \{0\}$ (prop. 15, a)), hence Sp($u^{-1}$) $=\{0\}($I, p. 26, cor. 1). Since $u^{-1}$ is normal (prop. 16), this implies that $u^{-1}$ is zero (I, p. 110, example 1), which is a contradiction.

#### Lemma 5 {#ts-iv-s4-lem-5 .statement tag=033V}

Let E be a complex Hilbert space and let $u$ be a closed partial operator with dense domain on E. Let $\lambda \in \mathbf{C}$. Suppose that there exists a real number $c >0$ such that

(10) $\|u(x)-\lambda x\|\geqslant c\|x\|$ for every $x\in$ dom($u$),

(11) $\|u^*(x)-\lambda x\|\geqslant c\|x\|$ for every $x\in$ dom($u^*$).

Then $\lambda$ belongs to the resolvent set of $u$ and $\|R(u, \lambda )\|\leqslant c^{-1}$.

The assumption implies that $u-\lambda 1_E$ and $u^*-\overline{\lambda}1_E$ are injective. Let F be the image of $u-\lambda 1_E$. The space F is dense in E, since its orthogonal is equal to Ker($u^*-\overline{\lambda}1_E$) (prop. 7, c) of IV, p. 236), which is zero.

Let us prove that the space F is closed. Let $(x_n)_{n\in\mathbf{N}}$ be a sequence in dom($u$) such that the sequence $(u(x_n)-\lambda x_n)_{n\in\mathbf{N}}$ converges to $y\in F$. Inequality (10) implies that the sequence $(x_n)_{n\in\mathbf{N}}$ is a Cauchy sequence in E. Let $x\in E$ be its limit. The sequence $(x_n, u(x_n))$ converges to $(x, y+\lambda x)$ in $E\times E$; since the graph of $u$ is closed, we therefore have $x\in$ dom($u$) and $u(x) =y+\lambda x$, which proves that $y\in F$.

We conclude that F = E. Thus, the partial operator $u-\lambda 1_E$ is bijective, whence $\lambda  \notin$ Sp($u$) (remark 3). Inequality (10) then implies that $\|R(u, \lambda )\|\leqslant c^{-1}$.

#### Proposition 17 {#ts-iv-s4-prop-17 .statement tag=033W}

Let E be a complex Hilbert space and let $u$ be a self-adjoint partial operator on E.

a) The spectrum of $u$ is contained in $\mathbf{R}$;

b) If $u$ is positive, then the spectrum of $u$ is contained in $\mathbf{R}_+$;

c) Suppose that E is nonzero. Let $\lambda  \notin$ Sp($u$) and let $\delta  >0$ be the distance from $\lambda$ to the spectrum of $u$. One has $\|R(u, \lambda )\|=\delta^{-1}$.

Let $(a, b)\in \mathbf{R}\times \mathbf{R}$ and $\lambda =a+ib$. Let $x\in$ dom($u$). Since $u$ is self-adjoint, one has $\langle x|u(x)\rangle  \in \mathbf{R}$, whence

$$
\|u(x)-\lambda x\|^2=\|u(x)\|^2-2a\langle x|u(x)\rangle + (a^2+b^2)\|x\|^2
$$

$$
=\|u(x)-\lambda x\|^2
$$

Suppose that $b\not = 0$. One then obtains

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2+b^2\|x\|^2
$$

$$
\geqslant b^2\|x\|^2
$$

By Lemma 5, one therefore has $\lambda  \notin$ Sp($u$), whence assertion a).

Suppose that $u$ is also positive. If $b= 0$ and $a <0$, one analogously obtains for $x\in$ dom($u$) the inequality

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2\geqslant a^2\|x\|^2
$$

therefore $\lambda  \notin$ Sp($u$) $($loc. cit.$)$, which proves b).

Finally, let us prove c). By Prop. 16, the resolvent $R(u, \lambda )$ is a normal endomorphism of E. Its norm is therefore equal to its spectral radius (Cor. 1 of I, p. 108), whence

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(R(u,\lambda))}|\mu|$

(Th. 1 of I, p. 24). The spectrum of $R(u, \lambda )$ cannot be reduced to $\{0\}$, for in that case one would have $\|R(u, \lambda )\|= 0$, hence the image dom($u$) of $R(u, \lambda )$ would be zero, and E likewise. Prop. 15 therefore implies that

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(u)}\frac{1}{|\lambda-\mu|}=\frac{1}{\delta}$.

#### Corollary {#ts-iv-s4-n7-cor-2 .statement tag=033X}

Let $u$ be a self-adjoint operator on E.

a) The residual spectrum of $u$ is empty;

b) For all $\lambda \not =\mu$ in $\mathbf{C}$, the eigenspaces of $u$ corresponding to $\lambda$ and $\mu$ are orthogonal.

Let us prove a). Let $\lambda$ belong to the spectrum of $u$; it is a real number (Prop. 17). One has Ker($\lambda 1_E-u$) $=$ Im($\lambda 1_E-u$)$^{\circ}$ (Prop. 7 of IV, p. 236), therefore $\lambda$ is not an eigenvalue of $u$ if the partial operator $\lambda 1_E-u$ has dense image. By definition this implies that the residual spectrum of $u$ is empty.

Let us prove b). By the proposition, we may suppose that $\lambda$ and $\mu$ are real. Let $x\in$ dom($u$) be such that $u(x) =\lambda x$ and $y\in$ dom($u$) be such that $u(y) =\mu y$. We then have

$$
\lambda \langle x|y\rangle =\langle u(x)|y\rangle =\langle x|u(y)\rangle =\mu\langle x|y\rangle
$$

whence $\langle x|y\rangle = 0$.

#### Remark {#ts-iv-s4-n7-rem-2 .statement tag=033Y}

If $u$ is a closed symmetric non-self-adjoint operator, its spectrum is not contained in $\mathbf{R}($cf. cor. 10 of IV, p. 257 below), and it is possible that the eigenspaces of $u$ relative to $\lambda$ and $\overline{\lambda}$ are not orthogonal (exercise 11 of IV, p. 347).

### 8. Pseudospectrum

#### Definition 9 {#ts-iv-s4-def-9 .statement tag=033Z}

Let E be a complex Banach space and let $u$ be a closed partial operator on E. Let $\varepsilon$ be a strictly positive real number. The $\varepsilon$-pseudospectrum of $u$ is by definition the union of the spectrum of $u$ and of the set of complex numbers $\lambda$ belonging to the resolvent set of $u$ such that $\|R(u, \lambda )\|> \varepsilon^{-1}$. This set is denoted by PSp$_{\varepsilon}(u)$.

Some authors define the $\varepsilon$-pseudospectrum of $u$ as the set $T_{\varepsilon}(u)$ equal to the union of Sp($u$) and of the set of $\lambda \in \mathbf{C}-$ Sp($u$) such that $\|R(u, \lambda )\|\geqslant \varepsilon^{-1}$. The closure of PSp$_{\varepsilon}(u)$ is contained in $T_{\varepsilon}(u)$, but this inclusion may be strict, even if E is a Hilbert space (cf. exercises 18 of IV, p. 348 and 19 of IV, p. 349).

#### Proposition 18 {#ts-iv-s4-prop-18 .statement tag=0340}

Let E be a complex Banach space and $u$ a closed partial operator on E. Let $\varepsilon \in \mathbf{R}^*_+$. The set PSp$_{\varepsilon}(u)$ is an open subset of $\mathbf{C}$. It is nonempty if E is nonzero.

If E is zero, then PSp$_{\varepsilon}(u)$ is empty. Suppose that E is nonzero. By prop. 14 of IV, p. 246, the set PSp$_{\varepsilon}(u)$ is an open subset of $\mathbf{C}$.

The set PSp$_{\varepsilon}(u)$ is nonempty if the spectrum of $u$ is nonempty. If Sp($u$) is empty, then Liouville's theorem (VAR, R1, p. 29, 3.3.6) implies that the holomorphic function on $\mathbf{C}$ defined by $\lambda \mapsto R(u, \lambda )$ is not bounded, hence there exists $\lambda$ in $\mathbf{C}$ such that $\|R(u, \lambda )\|> \varepsilon^{-1}$.

#### Proposition 19 {#ts-iv-s4-prop-19 .statement tag=0341}

Let E be a complex Banach space and $u$ a closed partial operator on E. One has PSp$_{\varepsilon}(u)\subset$ PSp$_{\delta}(u)$ if $0< \varepsilon  < \delta$ and

$\bigcap_{\varepsilon\in\mathbf{R}^*_+}$ PSp$_{\varepsilon}(u) =$ Sp($u$).

The first assertion results from the definition. For the second, the spectrum of $u$ is contained in PSp$_{\varepsilon}(u)$ for every $\varepsilon  >0$ by definition, and if $\lambda  \notin$ Sp($u$), then $\lambda  \notin$ PSp$_{\varepsilon}(u)$ when $\varepsilon  <\|R(u, \lambda )\|^{-1}$.

#### Proposition 20 {#ts-iv-s4-prop-20 .statement tag=0342}

Let E be a complex Banach space and $u$ a closed partial operator on E. Let $\varepsilon \in \mathbf{R}^*_+$. For every $\lambda \in \mathbf{C}$, the following conditions are equivalent:

(i) One has $\lambda \in$ PSp$_{\varepsilon}(u)$;

(ii) Either $\lambda \in$ Sp($u$), or there exists $x\in$ dom($u$) such that $\|x\|= 1$ and $\|(\lambda 1_E-u)(x)\|< \varepsilon$;

(iii) There exists $v\in \mathscr{L}(E)$ such that $\|v\|< \varepsilon$ and $\lambda \in$ Sp($u+v$).

One may suppose that E is nonzero. Condition (ii) is a reformulation of the definition, and hence of condition (i).

Suppose that condition (i) is satisfied and let us prove (iii). If $\lambda$ belongs to the spectrum of $u$, one can take $v= 0$ in (iii).

Suppose therefore that $\lambda  \notin$ Sp($u$). By definition of PSp$_{\varepsilon}(u)$, there exists $y\in E$ such that $\|y\|= 1$ and $\|R(u, \lambda )y\|> \varepsilon^{-1}$. Put $x= R(u, \lambda )y$. One has $x\not = 0$. By the Hahn–Banach theorem (EVT, II, p. 67, cor. 2), the linear form $\ell$ on $\mathbf{C}x$ such that $\ell (x) = 1$ admits a continuous extension $\ell_1\in E'$ such that $\|\ell_1\|=\|\ell \|$; hence $\|\ell_1\|=\|x\|^{-1}< \varepsilon$. For every $e\in E$, put $v(e) =\ell_1(e)y$. One has $v\in \mathscr{L}(E)$ and $v(x) =y$. It follows that $(u+v)x=u(x) +y=\lambda x$, therefore $\lambda \in$ Sp($u+v$). Since moreover $\|v\|=\|\ell_1\|< \varepsilon$, condition (iii) is satisfied.

Conversely, let $v\in \mathscr{L}(E)$ such that $\|v\|< \varepsilon$ and $\lambda \in$ Sp($u+v$). The partial operator $\lambda 1_E-(u+v)$ is therefore not injective with a continuous inverse; by Lemma 4 of IV, p. 243, applied to the injective partial operator $\lambda 1_E-u$ and to $-v$, one therefore has $\|v\|\geqslant \|R(u, \lambda )\|^{-1}$. It follows that condition (iii) implies (i).

#### Corollary {#ts-iv-s4-n8-cor-1 .statement tag=0343}

Let E be a complex Banach space and $u$ a closed partial operator on E. Let $\varepsilon  >0$.

a) For every $v\in \mathscr{L}(E)$, one has PSp$_{\varepsilon}(u)\subset$ PSp$_{\varepsilon+\|v\|}(u+v)$;

b) Let $\delta  >0$ and let $D_{\delta}$ be the open disk with center 0 and radius $\delta$ in $\mathbf{C}$. One has PSp$_{\varepsilon}(u) + D_{\delta}\subset$ PSp$_{\varepsilon+\delta}(u)$.

Let $\lambda \in$ PSp$_{\varepsilon}(u)$. There exists an endomorphism $w\in \mathscr{L}(E)$ such that $\|w\|< \varepsilon$ and $\lambda \in$ Sp($u+w$) (Prop. 20). Since $u+w= (u+v)+(w-v)$ and $\|w-v\|< \varepsilon +\|v\|$, one has $\lambda \in$ PSp$_{\varepsilon+\|v\|}(u+v) ($loc. cit.).

Let $\mu\in D_{\delta}$; one has $\lambda +\mu\in$ Sp($u+ (w+\mu1_E)$) and $\|w+\mu1_E\|< \varepsilon +\delta$, hence $\lambda +\mu\in$ PSp$_{\varepsilon+\delta}(u) ($loc. cit.).

#### Proposition 21 {#ts-iv-s4-prop-21 .statement tag=0344}

Let E be a complex Banach space and $u$ a closed partial operator on E. Let $\varepsilon \in \mathbf{R}^*_+$. Every bounded connected component of PSp$_{\varepsilon}(u)$ meets the spectrum of $u$.

Let U be a connected component of PSp$_{\varepsilon}(u)$ which does not meet Sp($u$). The set U is open and closed in PSp$_{\varepsilon}(u)$, and its closure U in $\mathbf{C}$ therefore satisfies $U\cap$ PSp$_{\varepsilon}(u) = U$.

Since Sp($u$) is contained in PSp$_{\varepsilon}(u)$ and U does not meet Sp($u$), this equality proves that the set U is disjoint from Sp($u$), hence contained in the resolvent set of $u$. Moreover, it implies that the set $\overline{U}-$ U does not meet PSp$_{\varepsilon}(u)$.

One therefore has $\|R(u, \lambda )\|\leqslant \varepsilon^{-1}$ for every $\lambda$ in $\overline{U}-$ U, whereas $\|R(u, \lambda )\|> \varepsilon^{-1}$ for $\lambda \in U$. If the set U is bounded, its closure $\overline{U}$ is compact and there exists $\lambda_0\in \overline{U}$ such that $\|R(u, \lambda )\|\leqslant \|R(u, \lambda_0)\|$ for $\lambda \in U$. The foregoing implies that $\lambda_0\in U$, which contradicts the maximum principle (VAR, R1, p. 29, 3.3.7) since the resolvent of $u$ is holomorphic in the resolvent set of $u$ (Prop. 14 of IV, p. 246).

### 9. Multiplication operators

Let X be a locally compact space and $\mu$ a positive measure on X. We consider the multiplication operators on $L^2(X, \mu)$; these are closed operators with dense domain (Prop. 5 of IV, p. 232). For every $\mu$-measurable function $g$ on X, we shall denote by $m_g$ the partial operator of multiplication by $g$ on $L^2(X, \mu)$.

#### Proposition 22 {#ts-iv-s4-prop-22 .statement tag=0345}

Let $g$ be a $\mu$-measurable function on X.

a) The spectrum of $m_g$ is the essential $\mu$-image S of $g$;

b) Let $\lambda \in \mathbf{C}-$ Sp($m_g$). The resolvent $R(m_g, \lambda )$ is the multiplication operator $m_h$, where $h$ is the function on X defined by $h(x) = 0$ if $g(x) =\lambda$ and $h(x) = (\lambda -g(x))^{-1}$ otherwise.

Let us prove that $\mathbf{C}-$ S is contained in the resolvent set of $m_g$. Let $\lambda \in \mathbf{C}-$ S. There exists an open neighbourhood U of $\lambda$ such that the subset $Y =\overset{-1}{g}(U)$ of X is locally $\mu$-negligible. The function $k$ defined on X by $k(x) = (\lambda -g(x))^{-1}$ if $x \notin Y$ and $k(x) = 0$ if $x\in Y$ then belong to $\mathscr{L}^{\infty}(X, \mu)$ (Lemma 5 of IV, p. 184); the multiplication operator by $k$ is therefore an endomorphism of $L^2(X, \mu)$.

Since $|gk|\leqslant 1 +|\lambda k|$, we have

$$
|gkf|\leqslant |f|+|\lambda kf|
$$

for $f\in \mathscr{L}^2(X, \mu)$, which implies that the image of $m_k$ is contained in the domain of $m_g$. Conversely, let $f\in \mathscr{L}^2(X, \mu)$ whose class $\widetilde{f}$ belongs to the domain of $m_g$. Outside the locally $\mu$-negligible set Y, we have $f(x) =k(x)(\lambda -g(x))f(x)$, hence $\widetilde{f}$ is in the image of $m_k$. The same formula proves that $\lambda$ belongs to the resolvent set of $m_g$ and that $R(m_g, \lambda ) =m_k$. Since the set Y is locally $\mu$-negligible, the multiplication operator $m_k$ coincides with the operator $m_h$ described in assertion b).

Let us prove conversely that $\mathbf{C}-$ Sp($m_g$) is contained in $\mathbf{C}-$ S. Let $\lambda \in \mathbf{C}-$ Sp($m_g$). Let $M>\|R(m_g, \lambda )\|$ be a real number. Let us denote by Y the set of $x\in X$ such that $|\lambda -g(x)|<M^{-1}$. Let us prove that Y is locally $\mu$-negligible, which will imply that $\lambda$ does not belong to S, and will complete the proof.

Let K be a compact subset of X. Let $\varphi$ be the characteristic function of $Y\cap K$; it is an element of $\mathscr{L}^2(X, \mu)$, and we denote by $\widetilde{\varphi}$ its class in $L^2(X, \mu)$. Let $\psi$ be a function in $\mathscr{L}^2(X, \mu)$ whose class in $L^2(X, \mu)$ is $R(m_g, \lambda )(\widetilde{\varphi})$. We have $R(m_g, \lambda )(\widetilde{\varphi})\in$ dom($m_g$) and $(\lambda -m_g)(R(m_g, \lambda )(\widetilde{\varphi})) =\widetilde{\varphi}$, hence $(\lambda -g(x))\psi (x) = 1$ for $\mu$-almost all $x\in Y\cap K$. This implies

$$
\|R(m_g, \lambda )\|^2\|\widetilde{\varphi}\|^2\geqslant \|R(m_g, \lambda )(\widetilde{\varphi})\|^2\geqslant M^2\mu(Y\cap K) = M^2\|\widetilde{\varphi}\|^2
$$

In view of the choice of M, this means that $\varphi$ is zero $\mu$-almost everywhere. Thus, the set $Y\cap K$ is $\mu$-negligible. Therefore the set Y is locally $\mu$-negligible (INT, IV, p. 172, § 5, n$^o2$, Prop. 5).

#### Proposition 23 {#ts-iv-s4-prop-23 .statement tag=0346}

Let $g$ be a $\mu$-measurable function on X. The adjoint of the multiplication operator $m_g$ is $m_{\overline{g}}$.

For every integer $n\geqslant$ 1, let $\varphi_n$ be the characteristic function of the set of elements $x\in$ X such that $|g(x)|\leqslant n$, and let $\widetilde{\varphi}_n$ be its class in $L^2(X, \mu)$. Let $f\in \mathscr{L}^2(X, \mu)$ be such that its class $\widetilde{f}$ belongs to dom($m^*_g$), and let $\psi$ be a function whose class is $m^*_g(\widetilde{f})$.

For every $h\in \mathscr{L}^2(X, \mu)$ whose class $\widetilde{h}$ belongs to dom($m_g$), we have also $\widetilde{h}\widetilde{\varphi}_n\in$ dom($m_g$), and therefore $\langle \widetilde{f}|m_g(\widetilde{h}\widetilde{\varphi}_n)\rangle =\langle m^*_g(\widetilde{f})|\widetilde{h}\widetilde{\varphi}_n\rangle$. This yields the equality

$$
\int_X\overline{(f g-\psi)}\varphi_nh d\mu= 0
$$

Since the domain of $m_g$ is dense in $L^2(X, \mu)$, it follows that $(f g-\psi )\varphi_n$ is zero $\mu$-almost everywhere. Since $n$ is arbitrary, this means that $m^*_g(\widetilde{f})$ is the class in $L^2(X, \mu)$ of $f g$. In particular, since $m^*_g(\widetilde{f})\in L^2(X, \mu)$, one concludes that $f$ belongs to the domain of $m_{\overline{g}}$ and that $m^*_g(\widetilde{f}) =m_{\overline{g}}(\widetilde{f})$.

The adjoint of $m_g$ is therefore an extension of $m_{\overline{g}}$. Moreover, one has

$$
\langle f|m_g(h)\rangle =\int_X\overline{f}\cdot (gh)d\mu=\int_Xf\overline{g}h d\mu
$$

for every $f\in L^2(X, \mu)$ and $h\in$ dom($m_g$), which proves that the linear form $h\mapsto  \langle f|m_g(h)\rangle$ is continuous whenever $m_{\overline{g}}(f)g$ belongs to $L^2(X, \mu)$. Consequently the domain of $m_{\overline{g}}$ is contained in that of $m^*_g$, which concludes the proof.

#### Corollary {#ts-iv-s4-n9-cor-1 .statement tag=0347}

Let $g$ be a $\mu$-measurable function on X. The multiplication operator $m_g$ on $L^2(X, \mu)$ is self-adjoint (resp. positive ) if and only if the function $g$ is locally $\mu$-almost everywhere real-valued (resp. locally $\mu$-almost everywhere positive).

The first assertion results from the proposition. If $g$ is locally $\mu$-almost everywhere positive, one has $\langle f|m_g(f)\rangle =\int_Xg|f|^2d\mu\geqslant 0$ for every $f\in L^2(X, \mu)$, hence the partial operator $m_g$ is positive.

Conversely, if $m_g$ is positive, then its spectrum is contained in $\mathbf{R}_+$ (prop. 17 of IV, p. 248); since this is the $\mu$-essential image of $g$ (prop. 22, a)), this means that $g$ is locally $\mu$-almost everywhere positive.

#### Lemma 6 {#ts-iv-s4-lem-6 .statement tag=0348}

Let $g_1$ and $g_2$ be $\mu$-measurable functions on X.

a) The partial operator $m_{g_1}+m_{g_2}$ is closable and its closure is the multiplication operator $m_{g_1+g_2}$;

b) One has $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$;

c) Suppose that $g_1$ is bounded. Then one has $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$. Moreover, the domain of $m_{g_2}$ is contained in the domain of $m_{g_1g_2}$, and $m_{g_1}\circ m_{g_2}$ is the restriction of $m_{g_1g_2}$ to dom($m_{g_2}$).

It is elementary that $m_{g_1+g_2}$ is an extension of $m_{g_1}+m_{g_2}$; the latter operator is therefore closable, and $\overline{m_{g_1} + m_{g_2}}\subset m_{g_1+g_2}$.

Let $f\in \mathscr{L}^2(X, \mu)$ be such that the function $h= (g_1+g_2)f$ belongs to $\mathscr{L}^2(X, \mu)$. For every integer $n\geqslant 1$, let $X_n$ denote the set of $x\in X$ such that $|g_1(x)|+|g_2(x)|\leqslant n$, and let $\varphi_n$ be the characteristic function of $X_n$. We have $\varphi_nf\in$ dom($m_{g_1}+m_{g_2}$). Since $(\varphi_nf)(x)$ tends to $f(x)$ for every $x\in X$, and since for every $n\in \mathbf{N}$ one has $|\varphi_nf|\leqslant |f|$ and $|(g_1+g_2)\varphi_nf|\leqslant$ $|(g_1+g_2)f|=|h|$, with $h\in \mathscr{L}^2(X, \mu)$ by hypothesis, Lebesgue's theorem (INT, IV, p. 137, § 3, No.$^o7$, Theorem 6) implies that the sequence of pairs of classes in $L^2(X, \mu)\times L^2(X, \mu)$ of $(\varphi_nf,(g_1+g_2)\varphi_nf)$, which belong to the graph of $m_{g_1}+m_{g_2}$, tends to the pair of classes of $(f, h)$ in $L^2(X, \mu)$. The closure of $m_{g_1}+m_{g_2}$ is therefore indeed equal to $m_{g_1+g_2}$.

It is elementary that $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$. Suppose that $g_1$ is bounded, so that $m_{g_1}$ is a continuous linear mapping on $L^2(X, \mu)$. Then the domain of $m_{g_2}\circ m_{g_1}$ is the set of classes of functions $f\in \mathscr{L}^2(X, \mu)$ such that $g_2(g_1f)\in \mathscr{L}^2(X, \mu)$, that is to say the domain of $m_{g_1g_2}$. Hence $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$.

It is likewise elementary that dom($m_{g_1}\circ m_{g_2}$) $=$ dom($m_{g_2}$) is contained in dom($m_{g_1g_2}$), and that the restriction of $m_{g_1g_2}$ to this space is equal to $m_{g_1}\circ m_{g_2}$.

One must beware of believing that $m_{g_1}\circ m_{g_2}=m_{g_1g_2}$ in general (exercise 10 of IV, p. 347). Nevertheless, one has the following partial result:

#### Proposition 24 {#ts-iv-s4-prop-24 .statement tag=0349}

Let $g$ be a $\mu$-measurable function on X.

a) One has $m_{\overline{g}}\circ m_g=m_{|g|^2}$;

b) For all integers $k, \ell \in \mathbf{N}$, one has $m_{g^k\overline{g}^{\ell}}=m^k_gm^{\ell}_{\overline{g}}$.

One has $m_{\overline{g}}\circ m_g\subset m_{|g|^2}$ by Lemma 6. Conversely, one deduces from the inequality $|g|\leqslant 1 +|g|^2$ that dom($m_{|g|^2}$) $=$ dom($m_{\overline{g}}\circ m_g$), whence the first assertion.

Let $k, \ell \in \mathbf{N}$. We have $m^k_gm^{\ell}_{\overline{g}}\subset m_{g^k\overline{g}^{\ell}}($loc. cit.). The domain of $m^k_gm^{\ell}_{\overline{g}}$ is the set of classes in $L^2(X, \mu)$ of functions $h\in \mathscr{L}^2(X, \mu)$ such that $|g|^jh$ belong to $\mathscr{L}^2(X, \mu)$ for every integer $j$ such that $0\leqslant j\leqslant k+\ell$. The inequalities

$$
|g^jh|\leqslant |h|+|g^{k+\ell}h|
$$

valid for $0\leqslant j\leqslant k+\ell$, show that dom($m^k_gm^{\ell}_{\overline{g}}$) is equal to dom($m_{g^k\overline{g}^{\ell}}$), whence assertion b).

### 10. Self-adjoint extensions of a symmetric operator

In this No., we shall classify the self-adjoint extensions of symmetric operators on a complex Hilbert space, and in particular determine conditions ensuring the existence of a self-adjoint extension of such an operator.

Let E be a complex Hilbert space. For every partial operator $u$ on E, in this No. we shall write $u+i$ and $u-i$ instead of $u+i1_E$ and $u-i1_E$.

Let $u$ be a closed operator with dense domain on E. We recall (cf. definition 4 of IV, p. 230 and proposition 4 of IV, p. 230) that $E_u$ denotes the Hilbert space dom($u$) endowed with the Hermitian form

$$
(x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

We denote by $\|x\|_u$ the norm of an element $x$ of the Hilbert space $E_u$. Every subspace of dom($u$) which is closed in E is closed in $E_u($IV, p. 230, remark 1).

#### Definition 10 {#ts-iv-s4-def-10 .statement tag=034A}

Let $u$ be a closed symmetric operator on a complex Hilbert space E. Let $E_+=$ Ker($u^*-i$) and $E_-=$ Ker($u^*+i$). The pair $(E_+,E_-)$ of subspaces of dom($u^*$) is called the deficiency pair of $u$. The subspaces $E_+$ and $E_-$ are closed subspaces of E (prop. 3 of IV, p. 229). The pair (dim(E$_+$), dim(E$_-$)) of the Hilbert dimensions of these subspaces is called the deficiency index of $u$.

#### Proposition 25 {#ts-iv-s4-prop-25 .statement tag=034B}

Let $u$ be a closed symmetric operator on a complex Hilbert space E. We have

Ker($u^*-i$)$^{\circ}=$ Im($u+i$),

Ker($u^*+i$)$^{\circ}=$ Im($u-i$).

By prop. 7, c) of IV, p. 236, it is enough to prove that the image of $u+i$ (resp. of $u-i$) is closed in E. Since $u$ is symmetric, we have $\langle (u+i)(x)|(u+i)(y)\rangle = (x|y)_u$ for all $x$ and $y$ in dom($u$). The mapping $x\mapsto u(x) +ix$ of $E_u$ into E is therefore isometric. Its image is closed in E (lemma 8 of I, p. 107). Since this is also the image of $u+i$, the latter is closed in E. Analogously, the image of $u-i$ is closed in E.

#### Lemma 7 {#ts-iv-s4-lem-7 .statement tag=034C}

Let $u$ be a closed symmetric operator on a complex Hilbert space E and $v$ a closed symmetric extension of $u$. The domain of $u$ is a closed subspace of the Hilbert space $E_v$.

Since $v$ is an extension of $u$, we have $(x|y)_v= (x|y)_u$ for $x$ and $y$ in dom($u$). The canonical injection of $E_u$ into $E_v$ is therefore isometric, and the conclusion follows (lemma 8 of I, p. 107).

#### Proposition 26 {#ts-iv-s4-prop-26 .statement tag=034D}

Let $u$ be a closed symmetric operator on a complex Hilbert space E. Let $(E_+,E_-)$ be the deficiency pair of $u$. The spaces $E_+,E_-$ and dom($u$) are closed mutually orthogonal subspaces of $E_{u^*}$ whose Hilbert sum is equal to $E_{u^*}$.

Since $u$ is symmetric, we have $u\subset u^*$, hence the space dom($u$) is closed in $E_{u^*}$ (lemma 7). The subspaces $E_+$ and $E_-$ are closed in E and contained in dom($u^*$), hence closed in $E_{u^*}$.

Let $x\in E_+$. We have $u^*(x) =ix$, whence $\langle x|u(y)\rangle =-i\langle x|y\rangle$ for every $y\in$ dom($u$). Consequently, for every $y\in$ dom($u$), we have

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =i(\langle x|u(y)\rangle  - \langle x|u^*(y)\rangle )= 0
$$

since $u$ is symmetric. The spaces $E_+$ and dom($u$) are therefore orthogonal in $E_{u^*}$. Analogously, $E_-$ and dom($u$) are orthogonal in $E_{u^*}$.

Let $x\in E_+$ and $y\in E_-$. Then

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle  - \langle x|y\rangle = 0
$$

therefore $E_+$ and $E_-$ are orthogonal in $E_{u^*}$.

Let $x\in E_{u^*}$ be orthogonal to the closed subspace dom($u$)$\oplus E_+\oplus E_-$. For every $y\in$ dom($u$), we have $u^*(y) =u(y)$ since $u\subset u^*$, whence

$$
0 = (x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle +\langle u^*(x)|u(y)\rangle
$$

This implies that $z=u^*(x)$ belongs to the domain of $u^*$ and satisfies $u^*(z) =-x$. Let $x_-=z-ix$. This is an element of dom($u^*$) satisfying $u^*(x_-) =-x-iz=-ix_-$. Hence $x_-$ belongs to $E_-$. But, for every $w\in E_-$, we have

$$
-i\langle x_-|w\rangle =-i\langle z|w\rangle +\langle x|w\rangle
$$

$$
=\langle u^*(x)|u^*(w)\rangle +\langle x|w\rangle = (x|w)_{u^*}= 0
$$

Taking $w=x_-$, we deduce that $x_-= 0$, that is to say $z=ix$; since $z=u^*(x)$, we therefore have $x\in E_+$, whence $x$ = 0 since $x$ is orthogonal to $E_+$ in $E_{u^*}$. This completes the proof that the direct sum dom($u$)$\oplus E_+\oplus E_-$ is equal to $E_{u^*}$.

#### Corollary {#ts-iv-s4-n10-cor-1 .statement tag=034E}

Let $u$ be a closed symmetric operator on E. Then $u$ is self-adjoint if and only if the deficiency index of $u$ is equal to $(0,0)$.

In fact, the symmetric operator $u$ is self-adjoint if and only if dom($u^*$) $=$ dom($u$); now the proposition proves that dom($u^*$) is the Hilbert sum of dom($u$) and of the deficiency subspaces of $u$.

Let $u$ be a closed symmetric partial operator. The spectrum of $u$ is contained in $\mathbf{R}$ if and only if $u$ is self-adjoint. In fact, it is known that Sp($u$)$\subset \mathbf{R}$ if $u$ is self-adjoint (Prop. 17 of IV, p. 248); if $u$ is not self-adjoint, one of the subspaces Ker($u^*+i$) or Ker($u^*-i$) is nonzero, hence the image of $u+i$ or of $u-i$ is a proper subspace of E (Prop. 25 of IV, p. 256), so that $i$ or $-i$ belongs to Sp($u$).

#### Definition 11 {#ts-iv-s4-def-11 .statement tag=034F}

Let $u$ be a closed symmetric operator on a complex Hilbert space E. A boundary condition for $u$ is a partially isometric linear mapping (TVS, V, p. 41, Def. 3) of Ker($u^*-i$) into Ker($u^*+i$).

Let $u$ be a closed symmetric operator on a complex Hilbert space E and $b$ a boundary condition for $u$. Let I = Ker($b$)$^{\circ}$ be the initial subspace of $b$. We denote by $u_b$ the reduction of $u^*$ to the subspace of dom($u^*$) which is the direct sum of dom($u$) and of the graph in $E_+\oplus E_-$ of the restriction of $b$ to I. Since $E_{u^*}=$ dom($u$)$\oplus E_+\oplus E_-$ (Prop. 26), the partial operator $u_b$ is well defined.

In other words, the domain of $u_b$ is the space of elements $x\in E$ of the form $x=x_0+y+b(y)$, where $x_0\in$ dom($u$) and $y$ belongs to the initial subspace of $b$. One then has $u_b(x_0+y+b(y)) =u(x_0) +iy-ib(y)$.

#### Theorem 1 (von Neumann) {#ts-iv-s4-thm-1 .statement tag=034G}

Let $u$ be a closed symmetric operator on a complex Hilbert space E and $(E_+,E_-)$ its deficiency pair.

a) For every boundary condition $b$ for $u$, the partial operator $u_b$ is a closed symmetric extension of $u$;

b) The mapping $b\mapsto u_b$ is a bijection of the set of boundary conditions for $u$ onto the set of closed symmetric extensions of $u$;

c) For every boundary condition $b$ for $u$, one has

Im($u_b+i$) $=$ Im($u+i$)$\oplus$ Im($b$)

Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Ker($b$)$^{\circ}$;

d) For every boundary condition $b$ for $u$, the deficiency pair of $u_b$ is (Ker($b$), Ker($b^*$)).

Let $b$ be a boundary condition for $u$ and $I\subset E_+$ its initial subspace. The restriction of $u^*$ to $\Gamma_{b|I}\subset E_+\oplus E_-$ is the continuous linear mapping defined by $x+b(x)\mapsto ix-ib(x)$ for $x\in I$. The graph of $u_b$ is the direct sum of the graph of $u$ and the graph of this linear mapping; it is therefore closed. The closed operator $u_b$ is an extension of $u$ such that $u_b\subset u^*$.

Let $\gamma_1$ and $\eta_1$ be elements of I. Consider the elements

$$
\gamma =\gamma_1+b(\gamma_1),\eta =\eta_1+b(\eta_1)
$$

of the graph $\Gamma_{b|I}$. We calculate

$$
\langle \gamma |u^*(\eta )\rangle =i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )+i(\langle \gamma_1|\eta_1\rangle  - \langle b(\gamma_1)|b(\eta_1)\rangle )
$$

$$
=i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )
$$

since $b$ is isometric on I. It follows that one has

$$
\langle u^*(\gamma )|\eta \rangle =\langle \gamma |u^*(\eta )\rangle \tag{12}
$$

for all $\gamma$ and $\eta$ in $\Gamma_{b|I}$.

Let $x$ and $y$ be elements of dom($u$)$,\gamma$ and $\eta$ elements of $\Gamma_{b|I}$. Then

$$
\langle x+\gamma |u_b(y+\eta )\rangle =\langle x|u(y)\rangle +\langle x|u^*(\eta )\rangle +\langle \gamma |u(y)\rangle +\langle \gamma |u^*(\eta )\rangle
$$

$$
=\langle u(x)|y\rangle +\langle u(x)|\eta \rangle +\langle u^*(\gamma )|y\rangle +\langle u^*(\gamma )|\eta \rangle
$$

$$
=\langle u_b(x+\gamma )|y+\eta \rangle
$$

where we have used the fact that $u$ is symmetric and that $\gamma$ and $\eta$ belong to the domain of $u^*$, as well as formula (12). The operator $u_b$ is therefore a closed symmetric extension of $u$. Assertion a) is proved.

The mapping $b\mapsto u_b$ is injective. In fact, a partially isometric mapping of $E_+$ into $E_-$ is uniquely determined by its initial subspace and by its restriction to the latter. Now the domain of $u_b$ determines the initial subspace I of $b$ and the graph of the restriction of $b$ to I.

Let us prove that the mapping $b\mapsto u_b$ is surjective. Let $w$ be a closed symmetric extension of $u$. One has $w\subset w^*\subset u^*$. The domain of $w$ is therefore a subspace of dom($u^*$) containing dom($u$), and $w$ is the restriction of $u^*$ to this subspace. Let G be the intersection of the domain of $w$ and of $E_+\oplus E_-$. It is a closed subspace of $E_{u^*}$ (lemma 7) and one has dom($w$) $=$ dom($u$)$\oplus G$ by proposition 26.

Let $x\in E_+$ and $y\in E_-$ be such that $x+y\in G$. Since $w$ is symmetric, and is the restriction of $u^*$ to dom($w$), we have

$$
\langle x+y|u^*(x+y)\rangle =\langle u^*(x+y)|x+y\rangle
$$

This equality is equivalent to

$$
\langle x|ix\rangle +\langle x| -iy\rangle +\langle y|ix\rangle +\langle y| -iy\rangle
$$

$$
=\langle ix|x\rangle +\langle ix|y\rangle +\langle -iy|x\rangle +\langle -iy|y\rangle
$$

that is, to $\|x\|^2=\|y\|^2$. In particular, the canonical projection $p_+: G\rightarrow E_+$ is injective and, if I denotes its image, the space G is the graph of an isometric mapping $b_0$ of I into $E_-$. For $x$ in I and $y$ in $E_-$ such that $x+y\in G$, we have

$$
\|x+y\|^2_{u^*}=\|x\|^2_{u^*}+\|y\|^2_{u^*}= 2(\|x\|^2+\|y\|^2)
$$

$$
= 4\|x\|^2= 4\|p_+(x+y)\|^2
$$

Thus, considering G as a closed subspace of the Hilbert space $E_{u^*}$, the mapping $x\mapsto \frac{1}{2}p_+(x)$ of G into I is an isometry. In particular, I is closed in $E_+$ (lemma 8 of I, p. 107). There then exists a unique boundary condition $b$ for $u$ whose initial space is I and which coincides with $b_0$ on I. We have dom($w$) $=$ dom($u_b$), whence $w=u_b$. This establishes assertion b).

Let us prove assertions c) and d). Let $b$ be a boundary condition for $u$ and I its initial subspace. For $x_0\in$ dom($u$) and $y\in I$, we have

$$
u_b(x_0+y+b(y))-i(x_0+y+b(y)) = (u-i)(x_0)-2ib(y)
$$

We have Im($u-i$) $= E^{\circ}_-$ (prop. 25). Since the image of $b$ is contained in $E_-$, this formula shows that Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Im($b$). By loc. cit., we thus have Ker($u^*_b+i$) $= E_-\cap$ Im($b$)$^{\circ}=$ Ker($b^*$).

Analogously, one verifies that Im($u_b+i$) $=$ Im($u+i$)$\oplus I$ and hence (loc. cit.) that Ker($u^*_b-i$) $= I^{\circ}\cap E_+=$ Ker($b$).

#### Corollary 1 {#ts-iv-s4-thm-1-cor-1 .statement tag=034H}

Let $u$ be a closed symmetric operator on a complex Hilbert space E. The mapping $b\mapsto u_b$ induces a bijection of the set of isometries of Ker($u^*-i$) onto Ker($u^*+i$) onto the set of self-adjoint extensions of $u$. In particular, there exists a self-adjoint extension of $u$ if and only if the two components of the deficiency index of $u$ are equal.

This follows from the corollary of proposition 26 and the theorem, together with EVT, V, p. 25, cor. 2.

#### Corollary 2 {#ts-iv-s4-thm-1-cor-2 .statement tag=034I}

Let E be a real Hilbert space. Let $u$ be a closed symmetric operator on E. The partial operator $u_{(\mathbf{C})}$ on $E_{(\mathbf{C})}$ is symmetric and closed, and admits at least one self-adjoint extension.

The partial operator $u_{(\mathbf{C})}$ is closed and symmetric by prop. 2 of IV, p. 228 and lemma 3 of IV, p. 239. The $\mathbf{R}$-linear isomorphism $j$ of $E_{(\mathbf{C})}$ onto $E_{(\mathbf{C})}$ such that $j(z\otimes x) =\overline{z}\otimes x$ for every $z\in \mathbf{C}$ and every $x\in E$ induces an isomorphism of Hilbert spaces of Ker($u^*_{(\mathbf{C})}-i$) onto Ker($u^*_{(\mathbf{C})}+i$), and one can apply corollary 1.

#### Corollary 3 {#ts-iv-s4-thm-1-cor-3 .statement tag=034J}

Let $u$ be a symmetric operator on E. The following conditions are equivalent:

(i) The operator $u$ is essentially self-adjoint;

(ii) The spaces Ker($u^*+i$) and Ker($u^*-i$) are zero;

(iii) The spaces Im($u+i$) and Im($u-i$) are dense in E;

(iv) The partial symmetric operator $u$ has a unique self-adjoint extension.

Conditions (ii) and (iii) are equivalent by prop. 7, c) of IV, p. 236.

The partial operator $u$ is essentially self-adjoint if and only if $\overline{u}$ is self-adjoint, that is to say if Ker($\overline{u}^*-i$) $=$ Ker($\overline{u}^*+i$) $=\{0\}$ (cor. of prop. 26). Since $\overline{u}^*=u^*$ (prop. 8 of IV, p. 237), condition (i) is therefore equivalent to condition (ii). Moreover, the preceding corollary shows that (ii) implies that $u$ has a unique self-adjoint extension, which is condition (iv).

Finally, suppose that $u$ has a unique self-adjoint extension $v$. Then the same is true of $\overline{u}$, since every self-adjoint extension of $\overline{u}$ is one of $u$, hence is equal to $v$. By the preceding corollary, the spaces Ker($\overline{u}^*+i$) and Ker($\overline{u}^*-i$) must be zero, whence condition (ii), using again $\overline{u}^*=u^*$.

#### Example {#ts-iv-s4-n10-exa-1 .statement tag=034K}

Let U be an open set of $\mathbf{R}^n$ endowed with the Lebesgue measure $\mu$. Let Δ be the scalar differential operator

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

on U. Let us denote by $u$ the partial operator on the real Hilbert space $L^2_{\mathbf{R}}(U, \mu)$ with domain $\mathscr{D}_{\mathbf{R}}(U) ($IV, p. 201, remark) defined by $\varphi \mapsto  -\sum^n_{i=1}\partial_i^2\varphi$. One has $u_{(\mathbf{C})}= \Delta_-$, which is a closable partial operator (prop. 13 of IV, p. 242) and symmetric (since Δ is formally symmetric), hence $u$ is closable and symmetric (proposition 2 of IV, p. 228 and lemma 3 of IV, p. 239). By the above corollary, there therefore exists a self-adjoint extension of $u_{(\mathbf{C})}$. It is a Laplacian on U (IV, p. 243).

## EXERCISES {#ts-iv-s4-exercises}

Unless otherwise stated, the Banach spaces and Hilbert spaces below are assumed to be complex.

See the [exercises for § 4](exercises/s4/).

[^1]: Care should be taken not to confuse the notion of graph considered here with that introduced in TA, II, p. 155, def. 1.
