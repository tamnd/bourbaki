---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 1
section_title: Applications linéaires compactes
lang: en
source: ts-iii-v-fr
book_pages: TS III.2-TS III.23, TS III.103-TS III.118
pdf_pages: 0016-0037, 0117-0132
extraction: native
subsections:
    - "no": 1
      title: Applications linéaires compactes
      page: 2
      pdf_page: 16
    - "no": 2
      title: Applications linéaires compactes et topologies faibles
      page: 6
      pdf_page: 20
    - "no": 3
      title: Transposition
      page: 8
      pdf_page: 22
    - "no": 4
      title: Le théorème de Leray–Schauder
      page: 10
      pdf_page: 24
    - "no": 5
      title: Sous-espaces invariants par un opérateur compact
      page: 12
      pdf_page: 26
    - "no": 6
      title: Espaces d’approximation
      page: 14
      pdf_page: 28
    - "no": 7
      title: Exemples d’espaces d’approximation
      page: 20
      pdf_page: 34
statements: 57
exercises: 37
content_sha256: 92b75882bce16b6824c3479ff9597eedf1b6caa70b690c86dad0dce89c28a961
translated_from: content/fr/ts/III/01_s1_applications_lineaires_compactes.md
source_lang: fr
translation_method: machine
source_content_sha256: b8cdeaecabfbb6543419f53f92ca3d724ec2830149e855a9c428a3a8e4ef0d6e
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-d216dbc4
glossary_version: 34
glossary_terms_sha256: 10d4ccc5ef7065d9651ff40351cc989c6d25497094fc4ee640add0d7deafeac7
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. COMPACT LINEAR MAPPINGS

### 1. Compact linear mappings

#### Definition 1 {#ts-iii-s1-def-1 .statement tag=02NY}

Let E be a topological vector space and F a separated topological vector space. A linear mapping $u$ from E into F is said to be compact if there exists a neighbourhood V of 0 in E such that $u(V)$ is a relatively compact subset of F.

We denote by $\mathscr{L}^c(E; F)$ the set of compact linear mappings from E into F; we also denote by $\mathscr{L}^c(F)$ the set $\mathscr{L}^c(F; F)$.

#### Remark 1 {#ts-iii-s1-n1-rem-1 .statement tag=02NZ}

A neighbourhood of 0 in E absorbs every bounded subset of E; the image of a bounded subset of E by a compact linear mapping from E into F is therefore a relatively compact subset of F.

#### Remark 2 {#ts-iii-s1-n1-rem-2 .statement tag=02O0}

Let E be a seminormed space and let B be the unit ball of E. In order that a linear mapping $u$ from E into a separated topological vector space F be compact, it is necessary and sufficient that $u(B)$ be a relatively compact subset of F.

#### Remark 3 {#ts-iii-s1-n1-rem-3 .statement tag=02O1}

Let F be a separated topological vector space. In order that a vector subspace E of F be of finite dimension, it is necessary and sufficient that the canonical injection of E into F be compact (EVT, I, p. 15, th. 3).

#### Remark 4 {#ts-iii-s1-n1-rem-4 .statement tag=02O2}

For every topological vector space E over the field $\mathbf{R}$, we denote by $E_{(\mathbf{C})}$ the complexified topological vector space of E (EVT, II, p. 65). We identify E with a real topological vector subspace of $E_{(\mathbf{C})}$ by the mapping $x\mapsto 1\otimes x$; the real topological vector space underlying $E_{(\mathbf{C})}$ is then the topological direct sum of E and $iE$.

Let $u$ be a linear mapping from E into a separated topological vector space F over $\mathbf{R}$. Let $u_{(\mathbf{C})}$ denote the $\mathbf{C}$-linear mapping from $E_{(\mathbf{C})}$ into $F_{(\mathbf{C})}$ which extends $u$. The sets of the form $V +iV$, where V is a neighbourhood of 0 in E, form a fundamental system of neighbourhoods of 0 in $E_{(\mathbf{C})}$. In order that the set $u_{(\mathbf{C})}(V +iV) =u(V) +iu(V)$ be relatively compact in $F_{(\mathbf{C})}$, it is necessary and sufficient that $u(V)$ be relatively compact in F. Consequently, in order that the $\mathbf{C}$-linear mapping $u_{(\mathbf{C})}$ be compact, it is necessary and sufficient that the $\mathbf{R}$-linear mapping $u$ be so.

In the same order of ideas, when $v$ is a continuous $\mathbf{C}$-linear mapping from $E_{(\mathbf{C})}$ into a $\mathbf{C}$-topological vector space G, in order that $v$ be compact it is necessary and sufficient that its restriction to E be compact.

#### Remark 5 {#ts-iii-s1-n1-rem-5 .statement tag=02O3}

Let E be a topological vector space, F a separated topological vector space. Let $F_1$ be a closed vector subspace of F and let $j$ be the canonical injection of $F_1$ into F. In order that a linear mapping $u$ from E into $F_1$ be compact, it is necessary and sufficient that the linear mapping $j\circ u$ from E into F be so.

#### Remark 6 {#ts-iii-s1-n1-rem-6 .statement tag=02O4}

Let $(G_i)_{i\in I}$ be a family of separated topological vector spaces, and for every $i\in I$, let $u_i$ be a compact linear mapping from a topological vector space E into $G_i$. If the set I is finite, or if E is a seminormed space, the linear mapping $x\mapsto (u_i(x))_{i\in I}$ from E into $\prod_{i\in I}G_i$ is compact (remark 2 and TG, I, p. 63, th. 3).

#### Proposition 1 {#ts-iii-s1-prop-1 .statement tag=02O5}

Let E be a topological vector space and F a separated topological vector space.

a) Every compact linear mapping from E into F is continuous ;

b) Every continuous linear mapping of finite rank from E into F is compact;

c) The set $\mathscr{L}^c(E; F)$ of compact linear mappings from E into F is a vector subspace of $\mathscr{L}(E; F)$.

Let us prove a). Let $v: E\rightarrow F$ be a compact linear mapping and U a neighbourhood of 0 in F. Choose a neighbourhood V of 0 in E such that $v(V)$ is relatively compact in F. Then $v(V)$ is bounded and there exists therefore a real number $\lambda  >0$ such that the set $v(\lambda V)$ is contained in U; consequently, $v$ is continuous.

Let $u: E\rightarrow F$ be a continuous linear mapping of finite rank. Since the image $u(E)$ of $u$ is separated and of finite dimension, there exists a compact neighbourhood A of 0 in $u(E)$. The set $V =\overset{-1}{u}(A)$ is a neighbourhood of 0 in E and we have $u(V)\subset A$, hence the linear mapping $u$ is compact. This proves assertion b).

Let $u_1$ and $u_2$ be compact linear mappings of E into F. Let $V_1$ and $V_2$ be neighbourhoods of 0 in E such that the sets $u_1(V_1)$ and $u_2(V_2)$ are relatively compact in F. Put $V = V_1\cap V_2$ and $u=u_1+u_2$. Then $u(V)$ is contained in $u_1(V_1) +u_2(V_2)$, hence is relatively compact in F, and the linear mapping $u$ is compact. It is immediate that $\mathscr{L}^c(E; F)$ is stable under homothety. This proves that $\mathscr{L}^c(E; F)$ is a vector subspace of $\mathscr{L}(E; F)$, whence assertion c).

#### Proposition 2 {#ts-iii-s1-prop-2 .statement tag=02O6}

Let E be a semi-normed space and F a separated topological vector space. Suppose that every closed bounded subset of F is complete. Then the vector subspace $\mathscr{L}^c(E; F)$ of $\mathscr{L}(E; F)$ is closed for the topology of bounded convergence.

Let $u$ be an element of $\mathscr{L}(E; F)$ adhering to $\mathscr{L}^c(E; F)$ for the topology of bounded convergence. Denote by B the unit ball of E and by V a neighbourhood of 0 in F. Choose a neighbourhood W of 0 in F such that $W + W\subset V$. By hypothesis there exists an element $v$ of $\mathscr{L}^c(E; F)$ such that $(u-v)(B)\subset W$. The set $v(B)$ being relatively compact in F, there exists a finite subset M of F such that $v(B)\subset M + W$, whence $u(B)\subset M + V$. Since this holds for every V, the set $u(B)$ is precompact in F, hence its closure is also so (TG, II, prop. 1, p. 30). Since the latter is closed and bounded, it is complete by the hypothesis made on F, and consequently is compact (TG, II, cor., p. 30). It follows that $u(B)$ is relatively compact. This proves that $u$ belongs to $\mathscr{L}^c(E; F)$.

If F is locally convex, the hypothesis of the proposition means that F is quasi-complete (EVT, III, p. 8, déf. 6).

#### Corollary {#ts-iii-s1-n1-cor-1 .statement tag=02O7}

Let E and F be Banach spaces. The set $\mathscr{L}^c(E; F)$ is a closed vector subspace of the Banach space $\mathscr{L}(E; F)$. It contains the closure of the space $\mathscr{L}^f(E; F)$ of continuous linear mappings of finite rank from E into F.

This follows from Propositions 1 and 2.

There exist Banach spaces E and F such that $\mathscr{L}^f(E; F)$ is not dense in $\mathscr{L}^c(E; F) ($cf. Remark 6 of III, p. 16 and Theorem 4 of III, p. 19, b)).

#### Proposition 3 {#ts-iii-s1-prop-3 .statement tag=02O8}

Let $E_1$, E, F, $F_1$ be topological vector spaces, F and $F_1$ being supposed separated. Let $v: E_1\rightarrow E,u: E\rightarrow F$ and $w: F\rightarrow F_1$ be linear mappings. If $v$ and $w$ are continuous and $u$ is compact, then $w\circ u\circ v$ is compact.

By hypothesis, there exists a neighbourhood V of 0 in E such that $u(V)$ is relatively compact in F. Put $U =\overset{-1}{v}(V)$. Then U is a neighbourhood of 0 in $E_1$ and its image by $w\circ u\circ v$ is contained in $w(u$(V)), hence is relatively compact in $F_1$. Consequently, the linear mapping $w\circ u\circ v$ is compact.

Let E be a separated topological vector space; according to Props. 1 and 3, $\mathscr{L}^c(E)$ is a two-sided ideal of the algebra $\mathscr{L}(E)$. When E is a Banach space, $\mathscr{L}(E)$ is a Banach algebra and $\mathscr{L}^c(E)$ is a closed two-sided ideal of $\mathscr{L}(E)$ (cor. to Prop. 2). It is a proper ideal if E is of infinite dimension (cf. Remark 3, p. 2).

#### Corollary {#ts-iii-s1-n1-cor-2 .statement tag=02O9}

Let E be a Hilbert space. The space $\mathscr{L}^c(E)$ is a closed self-adjoint two-sided ideal of $\mathscr{L}(E)$. In particular, it is a star-algebra.

In fact, the space $\mathscr{L}^c(E)$ is a closed, hence self-adjoint, two-sided ideal of $\mathscr{L}(E)$ (Lemma 15 of I, p. 122).

#### Proposition 4 {#ts-iii-s1-prop-4 .statement tag=02OA}

Let E be a topological vector space, $\widehat{E}$ its separated completion and $j$ the canonical mapping of E into $\widehat{E}$. Let $u$ be a compact linear mapping of E into a separated topological vector space F. Then there exists a unique compact linear mapping $v$ of $\widehat{E}$ into F such that $u=v\circ j$.

Identify F with a topological vector subspace of $\widehat{F}$ and denote by $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ the unique continuous linear mapping such that $\widehat{u}\circ j$ coincides with $u$ on E. Since $u$ is compact, there exist a neighbourhood V of 0 in E and a compact subset A of F such that $u(V)\subset A$. We have $\widehat{u}(j(V))\subset A$, whence $\widehat{u}(j(V))\subset A$. Now $j(V)$ is a neighbourhood of 0 in $\widehat{E}$ (TG, III, p. 24, Prop. 7). It follows that the image of $\widehat{u}$ is contained in F and the continuous linear mapping $v:\widehat{E}\rightarrow F$ deduced from $\widehat{u}$ by passing to the subspace is compact. Since $j(E)$ is dense in $\widehat{E}$, the mapping $v$ is the unique continuous linear mapping of $\widehat{E}$ into F such that $u=v\circ j$.

#### Proposition 5 {#ts-iii-s1-prop-5 .statement tag=02OB}

Let E be a locally convex space, F a separated topological vector space and $u$ a compact linear mapping of E into F. Then there exist a Banach space G, a continuous linear mapping $v$ of E into G and a compact linear mapping $w$ of G into F such that $u=w\circ v$.

Let V be a neighbourhood of 0 in E such that $u(V)$ is relatively compact in F. Let $p$ be a continuous seminorm on E such that V contains the unit ball of $p$ (EVT, II, p. 26, cor.). Denote by $E_p$ the seminormed space obtained by endowing E with the seminorm $p$. The mapping $u$ is a compact linear mapping of $E_p$ into F. The separated completion G of $E_p$ is a Banach space. Denote by $v$ the canonical linear mapping of $E_p$ into G. According to Prop. 4, there exists a compact linear mapping $w: G\rightarrow F$ such that $u=w\circ v$. On the other hand, $v$ is a continuous mapping of E into G because the topology of E is finer than that of $E_p$.

### 2. Compact linear mappings and weak topologies

Let E be a locally convex space, $E'$ its dual. Recall that the topology $\sigma (E,E')$ on E is called the weak topology on E (EVT, IV, p. 4). In this number, $E_{\sigma}$ denotes the space E endowed with the weak topology.

#### Proposition 6 {#ts-iii-s1-prop-6 .statement tag=02OC}

Let E be a locally convex space, F a separated locally convex space, $u: E\rightarrow F$ a compact linear mapping and B a bounded subset of E. The restriction of $u$ to B is a continuous mapping of the set B, endowed with the topology induced by $\sigma (E,E')$, into the space F.

The mapping $u$ is a continuous linear mapping of E into F, and also of $E_{\sigma}$ into $F_{\sigma}$. Its restriction to B is therefore a continuous mapping of the set B, endowed with the topology induced by $\sigma (E,E')$, into the space $F_{\sigma}$. Now the set $u(B)$ is contained in a compact subset C of F (remark 1 of III, p. 2) and the space $F_{\sigma}$ is separated, so that the topologies induced on C by those of F and of $F_{\sigma}$ coincide. The proposition follows.

#### Corollary {#ts-iii-s1-n2-cor-1 .statement tag=02OD}

Let $(x_n)_{n\in\mathbf{N}}$ be a sequence of points of E, which converges to a point $x$ of E for the weakened topology. The sequence $(u(x_n))_{n\in\mathbf{N}}$ converges in F to $u(x)$.

Indeed, the set consisting of the point $x$ and the points of the sequence $(x_n)_{n\in\mathbf{N}}$ is a bounded subset of E (EVT, III, p. 3, cor. of prop. 2).

#### Proposition 7 {#ts-iii-s1-prop-7 .statement tag=02OE}

Let E be a semi-normed space, $E'$ its dual, B the unit ball of $E'$ and $u$ a linear mapping of $E'$ into a locally convex separated space F. If the restriction of $u$ to B endowed with the topology induced by $\sigma (E',E)$ is continuous, then $u(B)$ is a compact subset of F and $u$ is a compact linear mapping of the strong dual $E'_b$ of E into F.

Indeed the set B, endowed with the topology induced by $\sigma (E',E)$, is compact (EVT, III, p. 17, cor. 2).

#### Corollary 1 {#ts-iii-s1-prop-7-cor-1 .statement tag=02OF}

Let E be a semi-normed space of countable type, let $E'$ be its dual and let B be the unit ball of $E'$. Let $u$ be a linear mapping of $E'$ into a locally convex separated space F. Suppose that for every sequence $(x_n)_{n\in\mathbf{N}}$ of elements of B which converges for $\sigma (E',E)$ to 0, the sequence $(u(x_n))_{n\in\mathbf{N}}$ converges to 0 in F. Then, $u(B)$ is a compact subset of F and $u$ is a compact linear mapping of the strong dual $E'_b$ of E into F.

Indeed, the topology induced on B by $\sigma (E',E)$ is metrisable (EVT, III, p. 19, cor. 2). The assumption of the corollary therefore implies that the restriction of $u$ to B is a continuous mapping of B into F, when B is endowed with the topology $\sigma (E',E)$, and the corollary follows from the preceding proposition.

#### Corollary 2 {#ts-iii-s1-prop-7-cor-2 .statement tag=02OG}

Let E be a semi-normed space and $\mathfrak{S}$ a set of precompact subsets of E whose union is dense in E. Let us denote by $E'_b$ the strong dual of E and by $E'_{\mathfrak{S}}$ the dual of E endowed with the $\mathfrak{S}$-topology. The space $E'_{\mathfrak{S}}$ is separated and the identical mapping of $E'_b$ into $E'_{\mathfrak{S}}$ is compact.

The space $E'_{\mathfrak{S}}$ is separated according to TG, X, p. 8, prop. 7; on the unit ball of $E'$, the $\mathfrak{S}$-topology coincides with the weak topology $\sigma (E',E)$ (EVT, III, p. 17, prop. 5), whence the corollary.

#### Example {#ts-iii-s1-n2-exa-1 .statement tag=02OH}

Let E be a semi-normed space. The identical mapping of $E'_b$ into the space $E'$, endowed with the weak topology, the topology of compact convergence or the topology of precompact convergence, is compact.

#### Proposition 8 {#ts-iii-s1-prop-8 .statement tag=02OI}

Let E be a reflexive Banach space, B its unit ball, F a locally convex separated space and $u: E\rightarrow F$ a linear mapping. The following conditions are equivalent :

(i) The linear mapping $u$ is compact ;

(ii) The set $u(B)$ is a compact subset of F ;

(iii) The restriction of $u$ to B is a continuous mapping of the set B, endowed with the topology induced by $\sigma (E,E')$, into F ;

(iv) For every sequence $(x_n)_{n\in\mathbf{N}}$ of points of B which converges to 0 for the topology $\sigma (E,E')$, the sequence $(u(x_n))_{n\in\mathbf{N}}$ converges to 0 in F ;

(v) From every infinite sequence of points of $u(B)$, one can extract a sequence which converges in F ;

(vi) Every infinite sequence of points of $u(B)$ has an adherence value in F.

Since E is a reflexive space, B is a compact subset of $E_{\sigma}$ (TVS, IV, p. 17, prop. 6), hence (iii) implies (ii). Condition (ii) implies (i) by definition, and condition (i) implies (iii) by prop. 6. It is also elementary that (iii) implies (iv) and that (v) implies (vi).

We shall now prove that (iv) implies (v). Let $(x_n)$ be an infinite sequence of points of B. Since B is a compact subset of $E_{\sigma}$, there exists, by the theorem of $\breve{S}$mulian (TVS, IV, p. 36, th. 2), a sequence $(y_n)$, extracted from the sequence $(x_n)$, which converges in $E_{\sigma}$ to a limit $y$. The sequence $(y_n-y)$ is bounded in $E_{\sigma}$, hence in E (TVS, IV, p. 1, prop. 1); it is therefore contained in a homothetic set of B. If condition (iv) is satisfied, the sequence $(u(y_n-y))$ converges to 0 in F, and $(u(y_n))$, which is a sequence extracted from $(u(x_n))$, converges to $u(y)$. This proves that (iv) implies (v).

To conclude, let us prove that (vi) implies (ii). Let $j: F\rightarrow \widehat{F}$ be the canonical injection of F into its completion. Under hypothesis (vi), $u(B)$ is a precompact subset of F (TVS, IV, p. 32, prop. 1), hence $j(u(B))$ is a relatively compact subset of $\widehat{F}$ (TG, II, n$^{\circ}2$, p. 29) and $j\circ u$ is a compact linear mapping. By the equivalence already proved of conditions (i) and (ii), $j(u(B))$ is a compact subset of $\widehat{F}$. Consequently, $u(B)$ is a compact subset of F.

### 3. Transpose

Let E be a locally convex space and $E'$ its dual. Recall that one denotes by $E'_b$ and $E'_c$ the locally convex spaces obtained by endowing the vector space $E'$ with the topology of bounded convergence and that of compact convergence respectively (TVS, III, p. 14). The space $E'_b$ is also called the strong dual of E (loc. cit., example 4).

#### Proposition 9 {#ts-iii-s1-prop-9 .statement tag=02OJ}

Let E be a locally convex space, F a separated locally convex space and $u$ a continuous linear mapping of E into F.

a) If the mapping $u$ is compact, then its transpose $^tu$ is a compact linear mapping of $F'_c$ into $E'_c$ and a continuous linear mapping of $F'_c$ into $E'_b$;

b) Suppose that the space E is a semi-normed space and that the space F is quasi-complete. If the transpose $^tu$ is a continuous mapping of $F'_c$ into $E'_b$, then the linear mapping $u$ is compact.

Suppose first that the linear mapping $u$ is compact. Then there exists a neighbourhood V of 0 in E whose image under $u$ is contained in a compact subset C of F. By definition (TVS, II, p. 47, def. 2 and p. 68, def. 1), the polar $C^{\circ}$ of C is a neighbourhood of 0 in $F'_c$ and one has $^tu(C^{\circ})\subset V^{\circ}$. Now $V^{\circ}$ is an equicontinuous subset of $E'$, closed for the weak topology, hence compact in $E'_c$ (TVS, III, p. 17, cor. 2 and prop. 5). This proves that $^tu$ is a compact linear mapping of $F'_c$ into $E'_c$.

Retain the preceding hypotheses and let U be a neighbourhood of 0 in $E'_b$. It contains the polar $A^{\circ}$ of a bounded subset A of E. Since the linear mapping $u$ is compact, the set $u(A)$ is relatively compact in F (remark 1 of III, p. 2), and $(^tu)^{-1}(A^{\circ}) =u(A)^{\circ}$ is a neighbourhood of 0 in $F'_c$. This proves that $^tu$ is a continuous linear mapping of $F'_c$ into $E'_b$.

Let us now place ourselves under the assumptions of b) and denote by B the unit ball of E. The polar $B^{\circ}$ of B is the unit ball of $E'_b$ and one has $(^tu)^{-1}(B^{\circ}) =u(B)^{\circ}$. If $^tu$ is a continuous mapping of $F'_c$ into $E'_b$, the set $u(B)^{\circ}$ is therefore a neighbourhood of 0 in $F'_c$; it therefore contains the polar $C^{\circ}$ of a compact subset C of F. By the bipolar theorem (EVT, II, p. 49, cor. 3), the set $u(B)$ is contained in the closed convex envelope of $C\cup  \{0\}$; this is compact because the space F is quasi-complete (EVT, III, p. 8). This proves that the linear mapping $u$ is compact.

#### Corollary 1 (Schauder) {#ts-iii-s1-prop-9-cor-1 .statement tag=02OK}

Let E be a seminormed space, F a Banach space, $E'$ and $F'$ their respective strong duals, and $u$ a continuous linear mapping of E into F. The following properties are equivalent:

(i) The linear mapping $u$ of E into F is compact;

(ii) The linear mapping $^tu$ of $F'$ into $E'$ is compact;

(iii) The linear mapping $^tu$ of $F'_c$ into $E'$ is continuous.

The equivalence of (i) and (iii) results from prop. 9, a) and b); the implication (iii)$\Rightarrow$(ii) follows from the fact that the identity mapping of $F'$ into $F'_c$ is compact (cor. of prop. 7 of III, p. 7).

To conclude, let us prove that condition (ii) implies (i). Suppose that the linear mapping $^tu: F'\rightarrow E'$ is compact. It results from the implication (i)$\Rightarrow$(ii), applied to $^tu$, that $^{tt}u$ is a compact linear mapping of $E''$ into $F''$. Let us denote by $v$ the canonical linear mapping of E into $E''$; it is continuous. Since F is identified with a closed vector subspace of $F''$ and since $u$ coincides with $^t(^tu)\circ v$ on E, it results from remark 5 of III, p. 3 that the linear mapping $u$ is compact.

#### Corollary 2 {#ts-iii-s1-prop-9-cor-2 .statement tag=02OL}

Let E be a seminormed space and F a Banach space of countable type. Let $u$ be a continuous linear mapping of E into F. Suppose that for every sequence $(y_n)$ of elements of $F'$ converging weakly to 0, the sequence $(^tu(y_n))$ converges strongly to 0 in $E'$. Then the linear mapping $u$ is compact.

Let us denote by $B'$ the unit ball of $F'$, endowed with the topology induced by the topology $\sigma (F',F)$. Since F is a Banach space of countable type, $B'$ is a compact metrisable space (EVT, III, p. 19, cor. 2). Under the assumption made, the restriction of $^tu$ to $B'$ is a continuous mapping of $B'$ into $E'$ and $^tu(B')$ is a compact subset of $E'$. By cor. 1, the linear mapping $u$ is compact.

#### Remark {#ts-iii-s1-n3-rem-1 .statement tag=02OM}

Let E and F be separated locally convex spaces. The transpose of a compact linear mapping of E into F is not always a compact linear mapping of $F'_b$ into $E'_b($cf. III, p. 108, exercise 15).

### 4. The Leray-Schauder theorem

The following theorem will be proved in TA, to appear.

#### Theorem 1 (Brouwer) {#ts-iii-s1-thm-1 .statement tag=02ON}

Let B be a nonempty compact convex subset of a finite-dimensional normed vector space. Every continuous mapping of B into B has a fixed point.

We shall deduce from it the following result.

#### Theorem 2 (Leray-Schauder) {#ts-iii-s1-thm-2 .statement tag=02OO}

Let X be a nonempty compact topological space, homeomorphic to a convex subset of a locally convex space. Every continuous mapping of X into X has a fixed point.

One may suppose that X is a convex subset of a locally convex space E. Let N be the closure of $\{0\}$ in E and $\pi : E\rightarrow E/N$ the canonical surjection. Since X is a separated space, the restriction of $\pi$ to X is injective; since X is compact, it therefore defines a homeomorphism of X onto a nonempty compact convex subset of the separated locally convex space $E/N$. This allows us to suppose that the space E is separated.

Let $f: X\rightarrow X$ be a continuous mapping. The mapping $h: X\rightarrow E$ defined by $h(x) =f(x)-x$ is continuous; since X is compact, the image $h(X)$ is closed. It is therefore enough to prove that 0 adheres to $h$(X), that is to say that for every convex open neighbourhood U of 0 in E, there exists a point $b$ of X such that $f(b)-b\in U$.

Let U be a convex neighbourhood of 0 in E. For every $a\in X$, let $V_a$ denote the set of elements $x$ of X such that $f(x)-f(a)\in U$. It is open in X and contains $a$. Since X is compact and nonempty, there exists a nonempty finite subset A of X such that the sets $V_a$, for $a\in A$, cover X. Let $(\varphi_a)_{a\in A}$ be a continuous partition of unity subordinate to the covering $(V_a)_{a\in A}$ (TG, IX, p. 43, prop. 1 and p. 47, th. 3). Let F denote the vector subspace of E generated by $f(A)$. For every $x\in F\cap X$, put

$$
g(x) =\sum_{a\in A}\varphi_a(x)f(a)
$$

This defines a continuous mapping $g: F\cap X\rightarrow E$. Its image is contained in the convex envelope of $f$(A), hence in $F\cap X$. Since the set $F\cap X$ is a nonempty compact convex subset of a finite-dimensional vector space, the mapping $g$ has a fixed point $b\in F\cap X$ by Theorem 1. We have

$$
f(b)-b=f(b)-g(b) =\sum_{a\in A}\varphi_a(b) (f(b)-f(a))
$$

For every $a\in$ A such that $\varphi_a(b)\not = 0$, one has $b\in V_a$ so that $f(b)-f(a)\in U$. Since U is convex, it follows that $f(b)-b\in U$, which completes the proof.

### 5. Invariant subspaces under a compact operator

The following theorem is to be compared with Schur’s Lemma (A, VIII, p. 43, cor. and V, p. 386, prop. 6) and Corollary 4 of I, p. 26.

#### Theorem 3 {#ts-iii-s1-thm-3 .statement tag=02OP}

Let E be a separated locally convex space over $\mathbf{C}$ and A a subset of $\mathscr{L}(E)$. Make the following assumptions:

(i) There exists no closed vector subspace of E, distinct from $\{0\}$ and E, which is stable under A;

(ii) The set A contains a nonzero compact endomorphism. Then the commutant of A is reduced to the homotheties.

Replacing A by the unital subalgebra of $\mathscr{L}(E)$ generated by A, one is reduced to the case where A is a unital subalgebra of $\mathscr{L}(E)$. Let then $h$ be a nonzero compact endomorphism of E belonging to A.

#### Lemma 1 {#ts-iii-s1-lem-1 .statement tag=02OQ}

There exists an element $a$ of A such that the kernel of $ha-1_E$ is not reduced to 0.

There exists an element $x_0$ of E such that $h(x_0)\not = 0$. Let V be a closed neighbourhood of $h(x_0)$ not containing 0. Since the endomorphism $h$ is compact, one can choose a convex open neighbourhood U of $x_0$ such that $h(U)$ is a relatively compact subset of V. The closure C of $h(U)$ is therefore a compact convex subset of E; since it is contained in V, it does not contain 0.

Let $y$ be a point of C. Let $Ay$ denote the set of images of $y$ under the elements of A. It is a vector subspace of E stable under A; it is nonzero since it contains $y$. By assumption (i) of the theorem, the set $Ay$ is dense in E. There therefore exists an element $b$ of A such that $b(y)\in U$. Since the set C is compact, there exists a

$-1$

finite family $(b_1, . . . , b_n)$ of elements of A such that the sets $b_i(U)$ cover C. There exists a continuous partition of unity $(\varphi_1, . . . , \varphi_n)$ on C subordinate to this covering (TG, IX, p. 47, th. 3). Define a mapping $f: C\rightarrow E$ by putting

$$
f(x) =\sum_{i=1}^n\varphi_i(x)b_i(x)
$$

for every $x\in C$; it is a continuous mapping. Since U is convex and $b_i(x)$ belongs to U when $\varphi_i(x)$ is not zero, we have $f(C)\subset U$ and $h(f(C))\subset C$. By Leray-Schauder's theorem (Theorem 2 of III, p. 11), there exists an element $x\in C$ such that $h(f(x)) =x$. Put then

$$
a=\sum_{i=1}^n\varphi_i(x)b_i
$$

We have $h(a(x)) =h(f(x)) =x$ and $x$ is nonzero since 0 does not belong to C, hence the kernel of $ha-1_E$ is nonzero.

Let us complete the proof of Theorem 3. Let $a$ be an element of A such that the kernel T of $ha-1_E$ is nonzero (Lemma 1). Let $i$ denote the canonical injection of T into E. The linear mapping $i$ is equal to $h\circ a\circ i$, and is therefore compact. Hence the dimension of T is finite (Remark 3 of III, p. 2). Let $u$ be an element of $\mathscr{L}(E)$ which commutes with A. Since $u$ commutes with $h\circ a$, we have $u(T)\subset T$. Since T is of nonzero finite dimension over the algebraically closed field $\mathbf{C}$, the endomorphism of T induced by $u$ has an eigenvalue $\lambda$.

Put F = Ker($u-\lambda 1_E$). It is a closed nonzero vector subspace of E; it is stable under A, since $u$ commutes with the elements of A. By assumption (i), we have F = E, whence $u=\lambda 1_E$.

#### Corollary 1 {#ts-iii-s1-thm-3-cor-1 .statement tag=02OR}

Let us retain the assumptions of Theorem 3 and suppose moreover that the elements of A are pairwise permutable. Then E is of dimension 1 over $\mathbf{C}$.

By assumption (ii) of Theorem 3, the space E is not zero. It therefore contains a vector subspace F of dimension 1. This subspace is closed because E is assumed separated. By Theorem 3, every element of A is a homothety, and therefore stabilizes F. It then follows from assumption (i) of Theorem 3 that F is equal to E.

#### Corollary 2 (Lomonosov) {#ts-iii-s1-thm-3-cor-2 .statement tag=02OS}

Let E be a separated locally convex space of dimension at least 2 over the field $\mathbf{C}$ and $u$ an endomorphism of E. Suppose that there exists a compact endomorphism $h\not = 0$ of E permutable with $u$. Then there exists a closed vector subspace F of E, distinct from $\{0\}$ and from E, such that $u(F)\subset F$.

In fact, Corollary 1 shows that the set $A =\{u, h\}$ cannot satisfy assumption (i) of Theorem 3.

#### Corollary 3 {#ts-iii-s1-thm-3-cor-3 .statement tag=02OT}

Let E be a separated locally convex space over the field $\mathbf{C}$ and $u$ a compact endomorphism of E. If E is of dimension at least 2, there exists a closed vector subspace F of E, distinct from $\{0\}$ and from E, such that $u(F)\subset F$.

The case $u= 0$ is immediate. The case $u\not = 0$ follows from Cor. 2 by taking $h=u$.

### 6. Approximation spaces

Given locally convex spaces E and F, let us recall (EVT, III, p. 14, Example 2) that $\mathscr{L}_{pc}(E; F)$ denotes the locally convex space obtained by endowing $\mathscr{L}(E; F)$ with the topology of precompact convergence. We also denote by $\mathscr{L}_{pc}(E)$ the locally convex space $\mathscr{L}_{pc}(E; E)$. When the locally convex space E is separated and quasi-complete (EVT, III, p. 8, def. 6), the topology of precompact convergence on $\mathscr{L}(E; F)$ coincides with the topology of compact convergence, since the closure of a precompact subset of E is compact (EVT, III, p. 8).

#### Definition 2 {#ts-iii-s1-def-2 .statement tag=02OU}

A locally convex space E is said to have the approximation property, or again to be an approximation space, if the identity mapping $1_E$ of E is adherent in the space $\mathscr{L}_{pc}(E)$ to the set $\mathscr{L}^f(E)$ of continuous finite-rank endomorphisms of E.

In particular, every finite-dimensional locally convex space is an approximation space.

#### Remark 1 {#ts-iii-s1-n6-rem-1 .statement tag=02OV}

In order that the topological direct sum of locally convex spaces E and F be an approximation space, it is necessary and sufficient that E and F be approximation spaces.

#### Remark 2 {#ts-iii-s1-n6-rem-2 .statement tag=02OW}

Let E be a locally convex space. Let N be the closure of $\{0\}$ in E and P an algebraic supplementary subspace of N in E. Then P is a topological supplementary subspace of N in E, and is isomorphic to the locally convex space $E/N$. The space N is an approximation space. By Remark 1, in order that E be an approximation space, it is necessary and sufficient that the separated locally convex space $E/N$ be one.

#### Remark 3 {#ts-iii-s1-n6-rem-3 .statement tag=02OX}

Let E be a locally convex space, A an equicontinuous subset of $\mathscr{L}^f(E)$ and T a total subset of E. If $1_E$ is adherent to A for the topology of simple convergence in T, then $1_E$ is adherent to A in $\mathscr{L}_{pc}(E)$ (EVT, III, p. 16, Proposition 4 and p. 17, Proposition 5), and E is an approximation space.

#### Remark 4 {#ts-iii-s1-n6-rem-4 .statement tag=02OY}

Let E be a locally convex space over $\mathbf{C}$. Let us denote by $E_0$ the locally convex space over $\mathbf{R}$ underlying E. In order that E be an approximation space, it is necessary and sufficient that $E_0$ be one. In fact, the condition is necessary; let us prove that it is sufficient. Suppose therefore that $E_0$ is an approximation space. Let C be a precompact subset of E and U a balanced convex neighbourhood of 0 in E. Put $C'= C\cup iC$. There exists a continuous $\mathbf{R}$-linear mapping $u$ of finite rank from $E_0$ into $E_0$ such that $x-u(x)$ belongs to U for every $x\in C'$. Put $v(x) =\frac{1}{2}(u(x)-iu(ix))$ for every $x$ in E. Thus one defines a continuous $\mathbf{C}$-linear mapping of finite rank from E into E. For every $x\in C$, we have $x\in C',ix\in C'$ and $x-v(x) =\frac{1}{2}(x-u(x))-\frac{i}{2}(ix-u(ix))$, so that $x-v(x)$ belongs to U. This proves that E is an approximation space.

#### Remark 5 {#ts-iii-s1-n6-rem-5 .statement tag=02OZ}

Let E be a locally convex space over $\mathbf{R}$. In order that the complexified locally convex space $E_{(\mathbf{C})}$ of E be an approximation space, it is necessary and sufficient that E be one. This follows from remarks 1 and 4, since the underlying real locally convex space of $E_{(\mathbf{C})}$ is isomorphic to $E\times E$.

#### Proposition 10 {#ts-iii-s1-prop-10 .statement tag=02P0}

Let E be a Hilbert space. Then E is an approximation space.

The set A of orthogonal projections of finite rank in E is equicontinuous. Let $n\geqslant 1$ be an integer and $(x_1, . . . , x_n)$ a family of elements of E. Let V denote the vector subspace generated by the $x_i$ and $p_V$ the orthogonal projection with image V. We have $p_V(x_i) =x_i$ for $1\leqslant i\leqslant n$. It follows that $1_E$ is adherent to A for the topology of simple convergence, and hence that E is an approximation space (remark 3).

Other examples of approximation spaces will be given in No.$^o7$ of III, p. 20.

#### Lemma 2 {#ts-iii-s1-lem-2 .statement tag=02P1}

Let E be a locally convex space. Then E is an approximation space if and only if, for every precompact subset C of E and every neighbourhood U of 0 in E, there exist an integer $n\geqslant 0$, elements $e_1, . . . , e_n$ of E, and continuous linear forms $f_1, . . . , f_n$ on E, such that $x-\sum^n_{i=1}f_i(x)e_i$ belongs to U for every $x\in C$.

The definition of the topology of precompact convergence shows that the condition is sufficient. Conversely, suppose that E is an approximation space. Let P be a topological complement in E of the closure of $\{0\}($cf. remark 2). Then the set A of the $u\in \mathscr{L}^f(E)$ such that $u(E)\subset P$ is dense in $\mathscr{L}^f(E)$. Since P is separated, every element $u$ of A is of the form $x\mapsto \sum^n_{i=1}f_i(x)e_i$, where $n\in \mathbf{N},e_1, . . . , e_n$ are elements of E and $f_1, . . . , f_n$ continuous linear forms on E (EVT, I, p. 14, th. 2). This proves that the condition is necessary.

#### Remark 6 {#ts-iii-s1-n6-rem-6 .statement tag=02P2}

There exist Banach spaces which do not possess the approximation property, as was proved by P. Enflo (A counterexample to the approximation problem in Banach spaces, Acta Math. 130 (1973), p. 309–317 ; cf. exercise 25 of III, p. 112). This answered a question of S. Banach (Théorie des opérations linéaires, Monografje Matematyczne I, Warszawa, 1932, remarks on Chapter VI, §1). See also the remark on p. 21.

#### Proposition 11 {#ts-iii-s1-prop-11 .statement tag=02P3}

Let E and F be locally convex spaces. Suppose that E is an approximation space.

a) The set $\mathscr{L}^f(E; F)$ is dense in $\mathscr{L}_{pc}(E; F)$;

b) The set $\mathscr{L}^f(F; E)$ is dense in $\mathscr{L}_{pc}(F; E)$;

c) Let $\mathfrak{S}$ be a set of bounded subsets of F and $u\in \mathscr{L}(F; E)$. Suppose that the image under $u$ of every subset of F belonging to $\mathfrak{S}$ is precompact. Then $u$ is adherent to $\mathscr{L}^f(F; E)$ for the $\mathfrak{S}$-topology (EVT, III, p. 13).

Let $v$ be an element of $\mathscr{L}(E; F)$. The mapping $\varphi :w\mapsto v\circ w$ of $\mathscr{L}_{pc}(E)$ into $\mathscr{L}_{pc}(E; F)$ is continuous (TG, X, p. 5, prop. 3). We have $\varphi (1_E) =v$ and $\varphi (\mathscr{L}^f(E))\subset \mathscr{L}^f(E; F)$, therefore $v$ is adherent to $\mathscr{L}^f(E; F)$ in $\mathscr{L}_{pc}(E; F)$. This proves a).

Analogously, under the assumptions of c), the mapping $\psi :w\mapsto w\circ u$ of $\mathscr{L}_{pc}(E)$ into $\mathscr{L}_{\mathfrak{S}}(F; E)$ is continuous (loc. cit.). We have $\psi (1_E) =u$ and $\psi (\mathscr{L}^f(E))\subset \mathscr{L}^f(F; E)$, therefore $u$ is adherent to $\mathscr{L}^f(F; E)$ in $\mathscr{L}_{\mathfrak{S}}(F; E)$.

The image of a precompact subset of F by a continuous linear mapping of F into E is precompact, therefore b) follows from c).

#### Corollary {#ts-iii-s1-n6-cor-1 .statement tag=02P4}

Let E be a separated approximation space and F a locally convex space. Every compact linear mapping of F into E is adherent to $\mathscr{L}^f(F; E)$ in the space $\mathscr{L}(F; E)$ endowed with the topology of bounded convergence.

This follows from prop. 11, c), for the image of a bounded subset of F by a compact linear mapping of F into E is relatively compact in E (remark 1 of III, p. 2), therefore precompact.

#### Proposition 12 {#ts-iii-s1-prop-12 .statement tag=02P5}

Let E be a locally convex space, I a set, and for each $i\in I$, let $F_i$ be a locally convex space and $v_i: E\rightarrow F_i$ a continuous linear mapping with dense image. Suppose that for every neighbourhood U of 0 in E, there exist $i\in I$ and a neighbourhood V of 0 in $F_i$ such that $\overset{-1}{v_{i}}(V)\subset U$. If the $F_i$ are approximation spaces, then E is also one.

Let A be a precompact subset of E and U a neighbourhood of 0 in E. By hypothesis there exist $i\in I$ and a continuous semi-norm $p$ on $F_i$ such that U contains $(p\circ v_i)^{-1}([0,1])$. Put $F = F_i,v=v_i$ and $B =v$(A), and suppose that F is an approximation space. The set B is precompact in F. There therefore exist (lemma 2) an integer $n\geqslant 1$, elements $y_1, . . . , y_n$ of F and continuous linear forms $f_1, . . . , f_n$ on F, such that one has, for every $y\in B$,

$$
p(y-\sum^nf_j(y)y_j)\leqslant \frac{1}{2}
$$

$j=1$

Since B is bounded (EVT, III, p. 3, prop. 2), there exists a real number $M>0$ such that $|f_j(y)|\leqslant M$ for every $j$ such that $1\leqslant j\leqslant n$ and every $y\in B$. Moreover, since $v(E)$ is dense in F, there exists, for each integer $j$ such that $1\leqslant j\leqslant n$, an element $x_j$ of E such that $p(y_j-v(x_j))\leqslant (2nM)^{-1}$. The linear mapping

$$
u:x\longmapsto \sum_{j=1}^nf_j(v(x))x_j
$$

belongs to $\mathscr{L}^f(E)$. For every $x\in A$, one has

$$
v(x-u(x)) =v(x)-\sum_{j=1}^nf_j(v(x))y_j+\sum_{j=1}^nf_j(v(x))(y_j-v(x_j))
$$

whence $p(v(x-u(x)))\leqslant \frac{1}{2}+\frac{nM}{2nM}= 1$, and therefore $x-u(x)\in U$. The proposition follows.

#### Corollary 1 {#ts-iii-s1-prop-12-cor-1 .statement tag=02P6}

A dense vector subspace of an approximation space is an approximation space.

#### Corollary 2 {#ts-iii-s1-prop-12-cor-2 .statement tag=02P7}

If the separated completion of a locally convex space E is an approximation space, then E is an approximation space.

#### Corollary 3 {#ts-iii-s1-prop-12-cor-3 .statement tag=02P8}

The product of a family of approximation spaces is an approximation space.

Let indeed $(E_i)_{i\in I}$ be a family of approximation spaces. For every finite subset J of I, let us put $E_J=\prod_{i\in J}E_i$ and denote by $v_J$ the canonical mapping of $E =\prod_{i\in I}E_i$ into $E_J$. The locally convex space $E_J$ is an approximation space (Remark 1). The corollary then follows from Prop. 12 applied to the locally convex space E, to the family $(E_J)$ of locally convex spaces, and to the continuous linear mappings $v_J: E\rightarrow E_J$.

#### Corollary 4 {#ts-iii-s1-prop-12-cor-4 .statement tag=02P9}

Let E be a locally convex space. If every continuous seminorm on E is majorized by a continuous prehilbertian seminorm, then E is an approximation space.

Let $\mathscr{P}$ be the set of continuous prehilbertian seminorms on E. For each $p\in \mathscr{P}$, the hypothesis implies that the seminormed space $E_p$ obtained by endowing E with the seminorm $p$ is an approximation space (Corollary 2 and Proposition 10), and the identity mapping of E into $E_p$ is continuous. The corollary therefore follows from Proposition 12.

#### Lemma 3 {#ts-iii-s1-lem-3 .statement tag=02PA}

Let E be a metrisable locally convex space and $(x_n)_{n\in\mathbf{N}}$ a sequence of elements of E converging to 0. There exist a sequence $(y_n)_{n\in\mathbf{N}}$ of elements of E converging to 0 and a sequence $(\lambda_n)_{n\in\mathbf{N}}$ of elements of the interval $[0,1]$ converging to 0 such that one has $x_n=\lambda_ny_n$ for every $n\in \mathbf{N}$.

Since E is metrisable, there exists a fundamental system $(V_m)_{m\in\mathbf{N}}$ of balanced neighbourhoods of 0 in E such that $V_0= E$ and $2^{m+1}V_{m+1}\subset V_m$ for every $m\geqslant 0$. Since $(x_n)$ converges to 0, there exists a strictly increasing sequence $(N_m)_{m\in\mathbf{N}}$ of integers such that $N_0= 0$ and such that, for every $m\geqslant 0$, one has $x_n\in V_m$ for $n\geqslant N_m$. For every integer $n\geqslant 0$, there exists a unique integer $m\geqslant 0$ such that $N_m\leqslant n <N_{m+1}$, and one then puts $\lambda_n= 2^{-m}$ and $y_n= 2^mx_n$. The sequence $(\lambda_n)$ thus defined converges to 0. Moreover, since $y_n\in V_m$ for $n\geqslant N_{m+1}$, the sequence $(y_n)$ converges to 0 in E. Finally, one has $x_n=\lambda_ny_n$ for every $n$.

Recall (EVT, II, p. 28) that if E is a vector space and L a convex balanced subset of E, one denotes by $E_L$ the vector subspace of E generated by L, endowed with the seminorm whose unit ball is L. When the set L contains no line, this seminorm is a norm.

#### Lemma 4 {#ts-iii-s1-lem-4 .statement tag=02PB}

Let E be a Fréchet space and A a compact subset of E. There exists a compact convex balanced subset L of E containing A such that the topologies induced on A by those of E and of $E_L$ coincide.

The set A is contained in the closed convex balanced hull of the set of points of a sequence $(x_n)_{n\in\mathbf{N}}$ of elements of E converging to 0 (EVT, IV, p. 24, Cor. 1). Let $(y_n)_{n\in\mathbf{N}}$ and $(\lambda_n)_{n\in\mathbf{N}}$ be sequences satisfying the conclusions of Lemma 3. The closed convex balanced hull L of the points of the sequence $(y_n)$ contains A and is a compact subset of E (EVT, III, p. 8). Hence $E_L$ is a Banach space (EVT, III, p. 8, Cor.). In this Banach space, the norm of $x_n$ is majorized by $\lambda_n$, therefore the sequence $(x_n)$ tends to 0. The closed convex balanced hull $\widetilde{A}$ of the sequence $(x_n)$ in $E_L$ is a compact subset of $E_L$ (EVT, III, p. 8). Since L is a bounded subset of E, the canonical injection of $E_L$ into E is continuous. The topologies induced on $\widetilde{A}$ by those of $E_L$ and of E coincide, and $\widetilde{A}$ is a compact, hence closed, subset of E. Since the set $\widetilde{A}$ is convex, balanced, and contains the sequence $(x_n)$, it contains A. This completes the proof.

#### Theorem 4 {#ts-iii-s1-thm-4 .statement tag=02PC}

Let E be a Fréchet space.

a) Suppose that E is an approximation space. Then, for every semi-normed space F, the space $\mathscr{L}^f(F; E)$ is dense in $\mathscr{L}^c(F; E)$ for the topology of bounded convergence;

b) Conversely, suppose that for every Banach space F, every compact linear mapping of F into E belong to the closure of $\mathscr{L}^f(F; E)$ for the topology of bounded convergence. Then E is an approximation space.

Let F be a semi-normed space. The closure of $\mathscr{L}^f(F; E)$ in $\mathscr{L}(F; E)$ is contained in $\mathscr{L}^c(F; E)$ (Prop. 1 and 2 of III, p. 4). It is equal to $\mathscr{L}^c(F; E)$ if E is an approximation space by Cor. to Prop. 11. This proves assertion a).

Suppose that the hypothesis of b) is satisfied. Let $\varepsilon  >0$ be a real number. Let A be a compact subset of E and $p$ a continuous semi-norm on E. Let L be a compact convex balanced subset of E such that A is a compact subset of the normed space $E_L$ (Lemma 4). The canonical injection $j: E_L\rightarrow E$ is compact and $E_L$ is a Banach space (TVS, III, p. 8, Cor.). Hence by hypothesis there exist an integer $n\geqslant 1$, elements $e_1, . . . , e_n$ of E, and continuous linear forms $\ell_1, . . . , \ell_n$ on $E_L$, such that the mapping $v$ of $E_L$ into E defined by $v(x) =\sum^n_{i=1}\ell_i(x)e_i$ satisfies $p(x-v(x))\leqslant \frac{\varepsilon}{2}$ for $x\in A$. The image of $^tj: E'\rightarrow (E_L)'$ is dense in $(E_L)'$ for the weak topology (TVS, IV, p. 6, Prop. 5). On $(E_L)'$ the topology of compact convergence is compatible with the duality between $(E_L)'$ and $E_L$ (TVS, IV, p. 3, Example). Therefore $^tj(E')$ is dense in $(E_L)'$ for the topology of compact convergence (TVS, IV, p. 1, Prop. 1), and there exist continuous linear forms $f_1, . . . , f_n$ on E such that

$$
|\ell_i(x)-f_i(x)|p(e_i)\leqslant \frac{\varepsilon}{2n}
$$

for $x\in A$ and $1\leqslant i\leqslant n$. The endomorphism $u:x\mapsto \sum^n_{i=1}f_i(x)e_i$ of E belong to $\mathscr{L}^f(E)$, and for every $x\in A$, one has

$$
p(x-u(x))\leqslant p(x-v(x)) +p(v(x)-u(x))\leqslant \frac{\varepsilon}{2}+n\times \frac{\varepsilon}{2n}=\varepsilon
$$

It follows from this that $1_E$ belong to the closure of $\mathscr{L}^f(E)$ for the topology of compact convergence. But the latter coincides with the topology of precompact convergence since E is complete. Hence E is an approximation space.

### 7. Examples of approximation spaces

Recall that every Hilbert space is an approximation space (III, p. 15, Prop. 10). This section gives other examples.

If X is a locally compact space, one denotes by $\mathscr{C}_0(X; K)$, or simply $\mathscr{C}_0$(X), the Banach space of continuous mappings from X into K tending to 0 at infinity, endowed with the norm defined by $\|f\|=$ sup$_{x\in X}|f(x)|$ for $f\in \mathscr{C}_0(X)$. When X is compact, this space coincides with the space $\mathscr{C}(X)$ of continuous mappings from X into K.

#### Lemma 5 {#ts-iii-s1-lem-5 .statement tag=02PD}

Let X be a compact topological space, F a finite subset of $\mathscr{C}(X)$ and $\varepsilon  >0$ a real number.

There exist a finite subset $X_0\subset X$ and a linear mapping $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ of norm $\leqslant 1$ such that $\|u(f|X_0)-f\|\leqslant \varepsilon$ for every $f\in F$.

Since the set F is an equicontinuous subset of $\mathscr{C}$ (X), there exists a finite covering $(U_i)_{i\in I}$ of X such that, for every $i\in I$ and every $f\in F$, the diameter of $f(U_i)$ is $\leqslant \varepsilon$. For $i$ in I, choose a point $x_i$ of $U_i$, and denote by $X_0$ the finite set of the $x_i$ for $i\in I$.

Let $(\varphi_i)_{i\in I}$ be a continuous partition of unity subordinate to $(U_i)_{i\in I}$ (TG, IX, p. 47, th. 3). Define a linear mapping $u$ of $\mathscr{C}(X_0)$ into $\mathscr{C}(X)$ by putting

$$
u(g) =\sum_{i\in I}g(x_i)\varphi_i
$$

for every $g\in \mathscr{C}(X_0)$. The linear mapping $u$ has norm $\leqslant 1$ and satisfies $\|u(f|X_0)-f\|\leqslant \varepsilon$ for every $f$ in F, whence the assertion.

#### Proposition 13 {#ts-iii-s1-prop-13 .statement tag=02PE}

Let X be a locally compact topological space. The Banach space $\mathscr{C}_0(X)$ is an approximation space.

Suppose first that X is compact. Let $A\subset \mathscr{L}^f(\mathscr{C}(X))$ be the set of mappings of the form $f\mapsto u(f|X_0)$, where $X_0$ is a finite subset of X and $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ is a linear mapping of norm $\leqslant 1$. The set A is equicontinuous. By Lemma 5, the identity mapping of $\mathscr{C}(X)$ belongs to the closure of A for the topology of simple convergence on $\mathscr{C}(X)$. The proposition then results from Remark 3 of III, p. 14.

Pass to the general case. Let Y be the Alexandroff compactification of X and $\omega$ the point at infinity of Y (TG, I, p. 67). Identify $\mathscr{C}_0(X)$ with the set of elements of $\mathscr{C}(Y)$ vanishing at $\omega$. Then $\mathscr{C}(Y)$ is the topological direct sum of $\mathscr{C}_0(X)$ and the vector space of constant mappings on Y. Since $\mathscr{C}(Y)$ is an approximation space by what precedes, the space $\mathscr{C}_0(X)$ is an approximation space (Remark 1 of III, p. 14).

#### Corollary {#ts-iii-s1-n7-cor-1 .statement tag=02PF}

Every commutative star algebra is an approximation space.

In fact, such an algebra is isomorphic to the algebra of continuous functions tending to 0 at infinity on a locally compact space (I, p. 108, th. 1).

#### Remark {#ts-iii-s1-n7-rem-1 .statement tag=02PG}

If E is an infinite-dimensional Hilbert space, the star algebra $\mathscr{L}(E)$ does not have the approximation property (A. Szankowski, $\mathscr{B}(H)$ does not have the approximation property, Acta Math. 147 (1981), p. 89–108).

#### Lemma 6 {#ts-iii-s1-lem-6 .statement tag=02PH}

Let X be a locally compact topological space. Let $\mu$ be a positive measure on X and $p\in [1,+\infty [$. Let F be a finite subset of $L^p_K(X, \mu)$ and $\varepsilon  >0$ a real number.

There exists a finite-rank projector $u$ of $L^p_K(X, \mu)$ of norm $\leqslant 1$ such that $\|u(f)-f\|\leqslant \varepsilon$ for every $f$ in F.

Let $\mathscr{P}$ be the set of finite partitions $\pi = (K_1, . . . ,K_n,H)$ of X, where $n\geqslant 1$ is an integer and $K_1, . . . ,K_n$ are integrable subsets of non-zero measure of X. For every partition $\pi = (K_1, . . . ,K_n,H)\in \mathscr{P}$, one defines an endomorphism $v_{\pi}$ of $\mathscr{L}^p(X, \mu)$ by putting

$$
v_{\pi}(f) =\sum^n\frac{1}{\mu(K_i)}(\int_{K_i}f d\mu)\varphi_{K_i}
$$

$i=1$

for $f\in \mathscr{L}_K^p(X, \mu)$, where $\varphi_{K_i}$ is the characteristic function of $K_i$. The mapping $v_{\pi}$ induces, on passing to quotients, a projector $u_{\pi}$ of $L^p_K(X, \mu)$. It is easily verified that the image of $u_{\pi}$ is the space of classes of functions $f\in \mathscr{L}_K^p(X, \mu)$ such that $f$ vanishes on H and is constant on $K_i$ for $1\leqslant i\leqslant n$.

Let us prove that $\|u_{\pi}\|\leqslant 1$. For $f\in \mathscr{L}_K^p(X, \mu)$, one has

$$
\|u_{\pi}(f)\|^p_p=\sum_{i=1}^n\mu(K_i)^{1-p}|\int_{K_i}f d\mu|^p
$$

By Hölder's inequality (INT, IV, p. 208, § 6, No.$^o4$, Theorem 2), for every $i$ one has the inequality

$$
|\int_{K_i}f d\mu|^p\leqslant \mu(K_i)^{p-1}\int_{K_i}|f|^pd\mu
$$

whence $\|u_{\pi}(f)\|_p\leqslant \|f\|_p$.

Let $\mathscr{E}$ be the set of classes in $L^p_K(X, \mu)$ of integrable functions on X taking only a finite number of values. Since $\mathscr{E}$ is dense in $L^p_K(X, \mu)$ (INT, IV, p. 162, §4, No.$^o10$, Corollary 1), there exists a finite set $F'$ of $\mathscr{E}$ such that every element of F is at distance at most $\varepsilon$ from an element of $F'$. On considering the finite partition $\pi$ formed by the sets of non-zero measure on which the mapping $x\mapsto (f(x))_{f\in F'}$ takes a given value, one sees that there exists an element $\pi$ of $\mathscr{P}$ such that $u_{\pi}(f) =f$ for every $f$ in $F'$. The projector $u_{\pi}$ therefore has the required properties.

#### Proposition 14 {#ts-iii-s1-prop-14 .statement tag=02PI}

Let X be a locally compact topological space, $\mu$ a positive measure on X, and $p\in [1,+\infty ]$. The space $L^p_K(X, \mu)$ is an approximation space.

If $p= +\infty$, then the space $L^{\infty}_{\mathbf{C}}(X, \mu)$ is a commutative stellar algebra (Example 4 of I, p. 103), hence an approximation space (Cor. of Prop. 13), and the same is true of $L^{\infty}_{\mathbf{R}}(X, \mu)$ by Remark 5 of III, p. 15.

Suppose that $p$ is finite. Let $A\subset \mathscr{L}^f(L^p_K(X, \mu))$ be the set of projectors of finite rank and norm $\leqslant 1$. By Lemma 6, the identity mapping of $L^p_K(X, \mu)$ is adherent to A for the topology of simple convergence, and the proposition then follows from Remark 3 of III, p. 14.

## EXERCISES {#ts-iii-s1-exercises}

In Exercises 1 to 5 only, K denotes a complete non-archimedean non-discrete valued field, whose valuation is denoted by $x\mapsto  |x|$. We also denote by $G\subset \mathbf{R}^*_+$ the image of $K^*$ under the mapping $x\mapsto  |x|$. The Banach spaces considered are Banach spaces over K.

See the [exercises for § 1](exercises/s1/).
