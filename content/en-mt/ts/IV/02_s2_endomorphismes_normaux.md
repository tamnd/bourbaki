---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 2
section_title: Endomorphismes normaux
lang: en
source: ts-iii-v-fr
book_pages: TS IV.179-TS IV.195, TS IV.319-TS IV.330
pdf_pages: 0192-0208, 0332-0343
extraction: native
subsections:
    - "no": 1
      title: Compléments sur les espaces $L^p(X, \mu)$
      page: 179
      pdf_page: 192
    - "no": 2
      title: Image essentielle d’une fonction mesurable
      page: 181
      pdf_page: 194
    - "no": 3
      title: Fonctions universellement mesurables
      page: 182
      pdf_page: 195
    - "no": 4
      title: L’algèbre stellaire $L^{\infty}(X, \mu)$
      page: 185
      pdf_page: 198
    - "no": 5
      title: Endomorphismes de multiplication
      page: 186
      pdf_page: 199
    - "no": 6
      title: Mesures spectrales
      page: 190
      pdf_page: 203
    - "no": 7
      title: Algèbres stellaires commutatives d’endomorphismes d’un espace hilbertien
      page: 191
      pdf_page: 204
    - "no": 8
      title: Continuité du calcul fonctionnel
      page: 194
      pdf_page: 207
statements: 32
exercises: 28
content_sha256: 0067987d155820404a75f619ade4cf9674a5866210669997c73b0916f3d2e730
translated_from: content/fr/ts/IV/02_s2_endomorphismes_normaux.md
source_lang: fr
translation_method: machine
source_content_sha256: 599ff9259cb84424a17e1f017fdd2fb6a18f4e62275c59892bbbafb68a6beda5
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-e63f706a
glossary_version: 34
glossary_terms_sha256: 054dd3fb40cd70a3eeb7527141a4eec962f29bf9df84b3ce83754e1f39cfab34
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. NORMAL ENDOMORPHISMS

In this paragraph, the Hilbert spaces considered are complex, unless otherwise mentioned.

### 1. Complements on the spaces $L^p(X, \mu)$

#### Proposition 1 {#ts-iv-s2-prop-1 .statement tag=02YO}

Let X be a locally compact topological space. Let $\mu$ be a positive measure on X and let $p\in [1,+\infty [$. Let $(X_i)_{i\in I}$ be a locally countable family (INT, IV, p. 190, § 5, n$^o9$, def. 7) of pairwise disjoint locally compact subsets of X such that the complement of the union of the $X_i$ is locally $\mu$-negligible. Let $\varphi_i$ be the characteristic function of $X_i$ and $\mu_i$ the measure induced by $\mu$ on $X_i$ (INT, IV, p. 186, §5, n$^o7$, def. 4).

a) The mapping $p_i:f\mapsto f \varphi_i$ is a projector of $\mathscr{L}^p(X, \mu)$ and defines by passing to the quotients a projector $\widetilde{p}_i$ of $L^p(X, \mu)$. The latter is an orthoprojector of $L^2(X, \mu)$ if $p= 2$;

b) The mapping $f\mapsto f|X_i$ induces an isometric isomorphism of the image of $p_i$ onto the space $\mathscr{L}^p(X_i, \mu_i)$ and defines by passing to the quotients an isometric isomorphism of the image of $\widetilde{p}_i$ onto $L^p(X_i, \mu_i)$, through which these two spaces are identified;

c) The sum of the spaces $L^p(X_i, \mu_i)$ is total in the space $L^p(X, \mu)$. In the case $p= 2$, the space $L^2(X, \mu)$ is the Hilbert sum of the spaces $L^2(X_i, \mu_i)$.

Assertion a) is elementary. Assertion b) results from the scholium of INT, V, p. 84, § 7, n$^o1$.

Let $q\in ]1,+\infty ]$ be the conjugate exponent of $p$. We identify the dual of $L^p(X, \mu)$ with $L^q(X, \mu)$ (INT, V, p. 61, § 5, n$^o8$, th. 4). Let $f$ be a function in $\mathscr{L}^q(X, \mu)$ whose class $\widetilde{f}$ in $L^q(X, \mu)$ satisfies $\langle \widetilde{f} ,\widetilde{p}_i(\varphi )\rangle = 0$ for all $i\in I$ and all $\varphi \in L^p(X, \mu)$. Since the image of $p_i$ contains $\mathscr{K}(X_i)$, it follows that the measure $(f|X_i)\cdot \mu_i$ on $X_i$ is zero, which means that the restriction of $f$ to $X_i$ is locally $\mu_i$-negligible on $X_i$ (INT, V, p. 46, § 5, n$^o3$, cor. 2). Since the complement in X of the union of the $X_i$ is locally $\mu$-negligible, we conclude that the function $f$ is locally $\mu$-negligible on X (INT, IV, p. 190, § 5, n$^o9$ and p. 172, n$^o2$, prop. 5). The class of $f$ is then zero in $L^q(X, \mu)$ (using INT, V, p. 8, § 1, n$^o3$, lemma 1 and the corollary of proposition 9 when $p\not = 1$). By the Hahn–Banach theorem (EVT, II, p. 46, cor. 1), the first part of the assertion c) follows.

If $p= 2$, the image of $p_i$ is orthogonal to that of $p_j$ for all $i\not =j$, since $X_i$ and $X_j$ are then disjoint, whence the last assertion.

#### Proposition 2 {#ts-iv-s2-prop-2 .statement tag=02YP}

Let X be a locally compact space countable at infinity. Let $\mu$ be a positive measure on X. For all $p\in [1,+\infty [$, the space $L^p(X, \mu)$ is of countable type.

Let $(U_n)_{n\in\mathbf{N}}$ be a sequence of relatively compact open subsets of X whose union is equal to X and which satisfy $U_n\subset U_{n+1}$ for all $n\in \mathbf{N}$ (TG, I, p. 68, prop. 15). For all $n\in \mathbf{N}$, the space $\mathscr{K}(X,\overline{U}_n)$ identifies with a closed subspace of the Banach space $\mathscr{C}(U_n)$ (INT, III, p. 40, § 1, n$^o1$); since this latter space is of countable type (TG, X, p. 25, corollary), the same is true of $\mathscr{K}(X,\overline{U}_n)$ (TG, IX, p. 19, cor., (i)). Let $\mathscr{F}_n$ be a countable dense subset of $\mathscr{K}(X,\overline{U}_n)$.

Let $f\in \mathscr{L}^p(X, \mu)$ and let $\varepsilon  >0$. There exists an integer $n\in \mathbf{N}$ such that $\int_{X-U_n}|f|^p< \varepsilon /2$, and there exists $g\in \mathscr{F}_n$ such that $\int_{\overline{U}_n}|f-g|^p< \varepsilon /2$. The union of the classes in $L^p(X, \mu)$ of the elements of the sets $\mathscr{F}_n$ is therefore dense in $L^p(X, \mu)$, which concludes the proof (TG, IX, p. 18, prop. 12).

### 2. Essential image of a measurable function

In this number, X denotes a locally compact topological space, and $\mu$ a positive measure on X.

#### Definition 1 {#ts-iv-s2-def-1 .statement tag=02YQ}

Let Y be a topological space. For every measurable function $g$ from X into Y, the $\mu$-essential image of $g$ is the subset of the $y\in Y$ such that, for every open neighbourhood U of $y$, the set $\overset{-1}{g}(U)$ is not locally $\mu$-negligible in X (INT, IV, p. 172, § 5, n$^o2$, def. 3).

#### Lemma 1 {#ts-iv-s2-lem-1 .statement tag=02YR}

Let $g$ be a $\mu$-measurable function from X into a topological space Y, and S its $\mu$-essential image. The set of elements $x\in X$ such that $g(x)$ does not belong to S is locally $\mu$-negligible in X.

Let $Z =\overset{-1}{g}(Y$ - S) be the set in question.

First suppose that X is compact and $g$ continuous. In this case, the image measure $g(\mu)$ is defined (INT, V, p. 69, § 6, n$^o1$, def. 1) since $\mu$ is a bounded measure. It follows from the definitions that the $\mu$-essential image of $g$ is the support of the measure $g(\mu) ($cf. INT, V, p. 70, § 6, n$^o2$, cor. 2), whence $\mu(Z) =g(\mu)(Y$ - S) = 0 (INT, IV, p. 118, § 2, n$^o2$, prop. 5).

Now consider the general case. Let C be a compact subset of X, and let $\varepsilon  >0$ be a real number. Since $g$ is measurable, there exists a compact subset $C_1\subset C$ such that $\mu(C$- $C_1)\leqslant \varepsilon$ and such that $g|C_1$ is continuous (INT, IV, p. 169, § 5, n$^o1$, prop. 1). One then has

$\mu(Z\cap C)\leqslant \mu(C$ - $C_1) +\mu(Z\cap C_1)\leqslant \varepsilon +\mu(Z\cap C_1)$.

Let $\mu_1$ be the measure induced by $\mu$ on $C_1$ (INT, IV, p. 186, § 5, n$^o7$, def. 4). Let $S_1$ be the $\mu_1$-essential image of $g|C_1$. One has $Z\cap C_1\subset$ $(g|C_1)^{-1}(Y$ - $S_1)$. By the first case, the set $Z\cap C_1$ is therefore $\mu_1$-negligible, and consequently $\mu$-negligible (INT, IV, p. 187, § 5, n$^o7$, lemma 2, (i)). The above inequality becomes $\mu(Z\cap C)\leqslant \varepsilon$; since $\varepsilon$ and C are arbitrary, the set Z is locally $\mu$-negligible (INT, IV, p. 172, § 5, n$^o2$, prop. 5).

#### Lemma 2 {#ts-iv-s2-lem-2 .statement tag=02YS}

Let $g$ be a continuous function from X into $\mathbf{C}$. The $\mu$-essential image of $g$ is the closure of the image under $g$ of the support of $\mu$.

Let Y be the support of $\mu$. If $z\in \mathbf{C}$ is not adherent to $g$(Y), there exists an open neighbourhood U of $z$ such that the open set $\overset{-1}{g}(U)$ does not meet Y and is therefore locally $\mu$-negligible; this means that $z$ does not belong to the $\mu$-essential image of $g$.

Conversely, if $z\in \mathbf{C}$ is adherent to $g$(Y), then for every open neighbourhood U of $z$, the set $\overset{-1}{g}(U)$ is an open set in X which meets Y. It is therefore not $\mu$-negligible, and since it is open, it is not locally $\mu$-negligible (INT, IV, p. 172, § 5, n$^o2$, Cor. 2). Hence $z$ belongs to the $\mu$-essential image of $g$.

#### Lemma 3 {#ts-iv-s2-lem-3 .statement tag=02YT}

Let $g$ be a continuous function from X into $\mathbf{C}$ and S its $\mu$-essential image. Suppose that S is not empty and that $0\notin S$; denote by $\delta$ the distance from 0 to S. Then $\delta  >0$.

Put $h(x) = 1/g(x)$ if $g(x)\not = 0$ and $h(x) = 0$ otherwise. The function $h$ belongs to $\mathscr{L}^{\infty}(X, \mu)$. Let $\widetilde{h}$ be the class of $h$ in $L^{\infty}(X, \mu)$. Then we have the formula $\delta^{-1}=\|\widetilde{h}\|_{\infty}$.

Let U be an open neighbourhood of 0 such that the open set $Z =\overset{-1}{g}(U)$ is locally $\mu$-negligible, hence negligible (INT, IV, p. 172, § 5, n$^o2$, Cor. 2). Let Y be the support of $\mu$; we have $Y\subset X$ - Z. The restriction of the function $h$ to X - Z is continuous and bounded; therefore $h\in \mathscr{L}^{\infty}(X, \mu)$ and the norm of $\widetilde{h}$ in $\mathscr{L}^{\infty}(X, \mu)$ is equal to the norm of its restriction to X - Z. Moreover, for every $\alpha \in \mathbf{R}_+$, the set of $x\in X$ - Z such that $|h(x)|> \alpha$ is an open set in X - Z; therefore it is locally $\mu$-negligible if and only if it does not meet Y (INT, IV, loc. cit. and INT, III, p. 66, § 3, n$^o2$, Def. 1). Consequently, we have

$\|\widetilde{h}\|_{\infty}=$ sup$_{x\in Y}\frac{1}{|g(x)|}$,

whence

$\|\widetilde{h}1\|=$ inf$_{\infty x\in Y}|g(x)|=$ inf$_{\lambda\in g(Y)}|\lambda |=$ inf$_{\lambda\in\overline{g(Y)}}|\lambda |$

which is equal to $\delta$ by the preceding lemma.

### 3. Universally measurable functions

In this No., X is a locally compact topological space. We recall (INT, V, p. 28, § 3, No$^o4$, def. 2) that a mapping $f$ of X into a topological space Y is universally measurable if it is $\mu$-measurable for every positive measure $\mu$ on X. For this, it is enough that $f$ be $\mu$-measurable for every positive measure $\mu$ with compact support on X (INT, V, p. 28, § 4, No$^o3$, prop. 6).

#### Lemma 4 {#ts-iv-s2-lem-4 .statement tag=02YU}

Let Y and Z be locally compact topological spaces, $f: X\rightarrow Y$ and $g: Y\rightarrow Z$ universally measurable mappings. The mapping $g\circ f: X\rightarrow Z$ is universally measurable.

Let $\mu$ be a positive measure with compact support on X and let C be its support. The restriction of $f$ to C is $(\mu|$C)-proper. The mapping $g$ is measurable with respect to the image measure $(f|C)(\mu|C)$, hence the mapping $(g\circ f)|C =g\circ (f|C)$ is $(\mu|$C)-measurable. Consequently, the mapping $g\circ f$ is $\mu$-measurable. The lemma follows.

We denote by $\mathscr{L}_u(X)$ the vector space of complex-valued functions which are universally measurable on X, and by $\mathscr{L}_u^{\infty}(X)$ the subspace of functions $f\in \mathscr{L}_u(X)$ which are bounded on X. For $f\in \mathscr{L}_u^{\infty}$(X), we put $\|f\|_{\infty}=$ sup$_{x\in X}|f(x)|$.

#### Proposition 3 {#ts-iv-s2-prop-3 .statement tag=02YV}

a) The set $\mathscr{L}_u(X)$ is an involutive subalgebra of the involutive algebra of functions from X into $\mathbf{C}$;

b) The set $\mathscr{L}_u^{\infty}(X)$ is a subalgebra of $\mathscr{L}_u(X)$ and the mapping defined by $f\mapsto  \|f\|_{\infty}$ is a norm on $\mathscr{L}_u^{\infty}(X)$ for which $\mathscr{L}_u^{\infty}(X)$ is a unital stellar algebra;

c) The algebra $\mathscr{L}_u(X)$ contains $\mathscr{C}(X)$ and $\mathscr{L}_u^{\infty}(X)$ contains $\mathscr{C}_b(X)$;

d) Every Borel function from X into $\mathbf{C}$ (TG, IX, p. 61, def. 5) belongs to $\mathscr{L}_u(X)$;

e) For every sequence $(f_n)_{n\in\mathbf{N}}$ in $\mathscr{L}_u(X)$ which converges simply to a function $f$ from X into $\mathbf{C}$, one has $f\in \mathscr{L}_u(X)$.

Assertions a) and c) follow from the definitions (cf. INT, IV, p. 175, § 5, No$^o3$, cor. 3). Assertion d) is a consequence of INT, IV, p. 179, § 5, No$^o5$, th. 4, since the inverse image under a Borel function of every Borel subset of $\mathbf{C}$ is a Borel subset of X, which is universally measurable (INT, V, p. 28, § 3, No$^o4$). Finally, assertion e) follows from Egoroff's theorem (INT, IV, p. 175, § 5, No$^o4$, th. 2).

To prove assertion b), it is enough to remark that e) implies, a fortiori, that a uniform limit of universally measurable functions is universally measurable.

There may exist universally measurable functions on X which are not Borel. In fact, if X is metrisable, the characteristic function of a Souslin subset of X is universally measurable (cf. INT, IV, p. 171, § 5, No$^o1$, cor. 2); now, in every uncountable Polish space, there exists a Souslin subset which is not Borel ("Souslin's theorem"; this follows from TG, IX, p. 120, exercise 8 and from the fact that for every uncountable Polish space X, there exists a Borel bijection $X\rightarrow \mathbf{N}^{\mathbf{N}}$ whose inverse is Borel).

#### Lemma 5 {#ts-iv-s2-lem-5 .statement tag=02YW}

Let $\mu$ be a positive measure on X. Let $g$ be a $\mu$-measurable function from X into $\mathbf{C}$, and let S be its $\mu$-essential image. For every function $f\in \mathscr{L}_u(S)$, the mapping $h$ from X into $\mathbf{C}$ such that $h(x) = 0$ if $g(x)\notin S$ and $h(x) =f(g(x))$ if $g(x)\in S$ is $\mu$-measurable.

Let $x\in X$ and let U be a relatively compact open neighbourhood of $x$. The set N = U - $(U\cap \overset{-1}{g}(S))$ is $(\mu|$U)-negligible. For every integer $n\geqslant 1$, let $V_n$ be an open set such that $N\subset V_n\subset U$ and $\mu(V_n-N)<1/n$ (INT, IV, p. 116, § 1, n$^o4$, prop. 19).

The restriction $\widetilde{g}$ of $g$ to U- $V_n$ is $\mu|(U$- $V_n$)-proper, and its image is contained in S. Since $f$ is universally measurable, the mapping $x\mapsto f(g(x))$ from U - $V_n$ into $\mathbf{C}$ is measurable with respect to the measure $\mu|(U$ - $V_n)$ (INT, V, p. 71, § 6, n$^o2$, prop. 3). The mapping $h_n$ from X into $\mathbf{C}$ such that $h_n(x) = 0$ if $x \notin U$ - $V_n$ and $h_n(x) =f(g(x))$ if $x\in U$ - $V_n$ is therefore $\mu$-measurable (INT, IV, p. 193, § 5, n$^o10$, prop. 16).

Since $h_n(x)\rightarrow h(x)$ for $\mu$-almost all $x\in U$, the restriction of $h$ to U is $\mu$-measurable (INT, IV, p. 175, § 5, n$^o4$, th. 2). It follows that $h$ is $\mu$-measurable by the localisation principle (INT, IV, p. 171, § 4, n$^o2$, prop. 4).

#### Remark {#ts-iv-s2-n3-rem-1 .statement tag=02YX}

Under the hypotheses of the lemma, let us denote by abuse of language the function $h$ defined in the lemma by $f\circ g$.

If $g=g_1$ locally $\mu$-almost everywhere on X, the functions $g$ and $g_1$ have the same $\mu$-essential image and one has $f\circ g=f\circ g_1$.

If $g$ is a $\mu$-measurable function defined $\mu$-almost on X, one also denotes by $f\circ g$ the function $f\circ g_1$ where $g_1$ is a $\mu$-measurable function defined on X equal to $g$ locally $\mu$-almost everywhere.

### 4. The star algebra $L^{\infty}(X, \mu)$

Let X be a locally compact topological space and let $\mu$ be a positive measure on X. We consider the commutative star algebra $L^{\infty}(X, \mu)$ (Example 4 of I, p. 103).

#### Lemma 6 {#ts-iv-s2-lem-6 .statement tag=02YY}

Let $g\in \mathscr{L}^{\infty}(X, \mu)$. The spectrum of the class of $g$ in $L^{\infty}(X, \mu)$ is equal to the $\mu$-essential image of $g$.

Let us denote by $\widetilde{g}$ the class of $g$ in $L^{\infty}(X, \mu)$ and by S the $\mu$-essential image of $g$. Let $z\in \mathbf{C}-$ S. By definition, there exists an open neighbourhood U of $z$ such that $Y =\overset{-1}{g}(U)$ is locally $\mu$-negligible. The function $h$ defined by $h(x) = (g(x)-z)^{-1}$ if $x \notin Y$, and $h(x) = 0$ if $x\in Y$, then belong to $\mathscr{L}^{\infty}(X, \mu)$. Its class $\widetilde{h}$ in $L^{\infty}(X, \mu)$ satisfies $(\widetilde{g}-z)\widetilde{h}= 1$, since $(g(x)-z)h(x) = 1$ for every $x$ not belonging to the locally $\mu$-negligible set Y. Hence $z\in \mathbf{C}-$ Sp($\widetilde{g}$).

Conversely, let $z\in \mathbf{C}-$ Sp($\widetilde{g}$). Let $h\in \mathscr{L}^{\infty}(X, \mu)$ be a function whose class is the inverse of $\widetilde{g}-z$ in $L^{\infty}(X, \mu)$. There exists a real number $M>0$ such that $|h(x)|\leqslant M$ locally $\mu$-almost everywhere, and moreover one has $(g(x)-z)h(x) = 1$ locally $\mu$-almost everywhere. Let U be the open ball with center $z$ and radius $M^{-1}$ in $\mathbf{C}$; then $\overset{-1}{g}(U)$ is contained in the locally $\mu$-negligible set

$$
\overset{-1}{h}(]M,+\infty [)\cup  \{x\in X|(g(x)-z)h(x)\not = 1\}
$$

therefore $z\in \mathbf{C}-$ S. The lemma is proved.

#### Proposition 4 {#ts-iv-s2-prop-4 .statement tag=02YZ}

Let $g\in \mathscr{L}^{\infty}(X, \mu)$. Denote by $\widetilde{g}$ the class of $g$ in $L^{\infty}(X, \mu)$ and by S the spectrum of $\widetilde{g}$. The mapping $f\mapsto f\circ g$ (remark, p. 184) is the functional calculus mapping of $\mathscr{C}(S)$ into $L^{\infty}(X, \mu)$ associated with $\widetilde{g}$.

Let $f\in \mathscr{C}(S)$. The function $h=f\circ g$ is $\mu$-measurable (Lemma 5 of IV, p. 184) and bounded. Denote by $f\widetilde{\circ}g$ its class in $L^{\infty}(X, \mu)$. The mapping $f\mapsto f\widetilde{\circ}g$ is a continuous morphism of involutive algebras with unit of $\mathscr{C}(S)$ into $L^{\infty}(X, \mu)$. Since $g(x)$ belongs to S locally $\mu$-almost everywhere (Lemma 1 of IV, p. 181 and Lemma 6), this morphism associates with the identity mapping of S the class $\widetilde{g}$ of the function $g$. It therefore coincides with the functional calculus mapping of $\widetilde{g}$ (Prop. 7 of I, p. 111).

### 5. Multiplication Endomorphisms

Let X be a locally compact topological space and let $\mu$ be a positive measure on X. Let $p\in [1,+\infty [$.

Let $g\in \mathscr{L}^{\infty}(X, \mu)$. Denote by $m_g$ the mapping $f\mapsto g\cdot f$ of $\mathscr{L}^p(X, \mu)$ into itself. The mapping $m_g$ is linear and continuous since

$$
N_p(m_g(f))\leqslant N_{\infty}(g)N_p(f) \tag{1}
$$

for every function $f\in \mathscr{L}^p(X, \mu)$. In particular, the function $m_g(f)$ is $\mu$-negligible if $f$ is $\mu$-negligible. The mapping $m_g$ therefore induces, by passing to quotients, an endomorphism of $L^p(X, \mu)$, which will be denoted by $\widetilde{m}_g$.

#### Lemma 7 {#ts-iv-s2-lem-7 .statement tag=02Z0}

Let $g\in \mathscr{L}^{\infty}(X, \mu)$. The endomorphism $\widetilde{m}_g$ of $L^p(X, \mu)$ is injective if and only if the set of $x\in X$ such that $g(x) = 0$ is locally $\mu$-negligible.

Let A denote the set of $x\in X$ such that $g(x) = 0$.

Suppose that A is locally $\mu$-negligible. Let $f\in \mathscr{L}^p(X, \mu)$ and $\widetilde{f}$ its class in $L^p(X, \mu)$. Suppose that $\widetilde{m}_g(\widetilde{f}) = 0$. By definition, this is the case if and only if the function $f g$ is $\mu$-negligible, so that the set B of $x\in X$ such that $f(x)g(x)\not = 0$ is $\mu$-negligible. The function $f$ is zero outside $A\cup B$, hence is $\mu$-negligible. This implies that the endomorphism $\widetilde{m}_g$ is injective.

Conversely, suppose that A is not locally $\mu$-negligible. Let C be a compact subset of X such that $A\cap C$ is not $\mu$-negligible, and let $\varphi$ be the characteristic function of $A\cap C$. The class of the function $\varphi$ in $L^p(X, \mu)$ is not zero, but that of $m_g(\varphi )$ is, hence $m_g$ is not injective.

Since the product of a locally $\mu$-negligible function and a $\mu$-negligible function is $\mu$-negligible, the endomorphism $\widetilde{m}_g$ depends only on the class of $g$ in $L^{\infty}(X, \mu)$. For $\widetilde{g}\in L^{\infty}(X, \mu)$, one also denotes by $\widetilde{m}_g$ the endomorphism $\widetilde{m}_g$ of $L^p(X, \mu)$ for every function $g\in \mathscr{L}^{\infty}(X, \mu\widetilde{)}$ whose class is $\widetilde{g}$. One says that $\widetilde{m}_g$ is the endomorphism of multiplication by $\widetilde{g}$ in $L^p(X, \mu)$.

#### Proposition 5 {#ts-iv-s2-prop-5 .statement tag=02Z1}

Let $p\in [1,+\infty [$. The map $m:g\mapsto \widetilde{m}_g$ of $L^{\infty}(X, \mu)$ into $\mathscr{L}(L^p(X, \mu))$ is an isometric morphism of unital Banach algebras.

For $a,b$ in $\mathbf{C}$ and $g_1,g_2$ in $L^{\infty}(X, \mu)$, one verifies at once that $\widetilde{m}_{ag_1+bg_2}=a\widetilde{m}g_1+b\widetilde{m}_{g_2}$, hence the mapping $\widetilde{m}$ is linear. Moreover, one has $\widetilde{m}_1= 1_{L^p(X,\mu)}$ and $\widetilde{m}_{g_1g_2}=\widetilde{m}_{g_1}\widetilde{m}_{g_2}$, hence the mapping $\widetilde{m}$ is a unital algebra morphism of $L^{\infty}(X, \mu)$ into $\mathscr{L}(L^p(X, \mu))$.

Formula (1) above proves that $\widetilde{m}$ has norm $\leqslant 1$.

Let $g\in \mathscr{L}^{\infty}(X, \mu)$ and $\widetilde{g}$ its class in $L^{\infty}(X, \mu)$. Let $\varepsilon  >$ 0. The set Y of the $x\in X$ such that $|g(x)|>\|\widetilde{g}\|_{\infty}-\varepsilon$ is not locally $\mu$-negligible. There therefore exists a compact subset C of X such that $\mu(Y\cap C)>0$. Let $\varphi$ be the characteristic function of $Y\cap C$. Since

$$
\|\widetilde{m}_{\widetilde{g}}(\varphi )\|_p=(\int_X|\varphi g|^pd\mu)^{1/p}\geqslant (\int_Y|\varphi g|^pd\mu)^{1/p}
$$

$$
\geqslant (\|\widetilde{g}\|_{\infty}-\varepsilon )\mu(Y\cap C)^{1/p}= (\|\widetilde{g}\|_{\infty}-\varepsilon )\|\varphi \|_p
$$

it follows that $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}-\varepsilon$. Since $\varepsilon$ is arbitrary, one deduces that $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}$, which proves that $\widetilde{m}$ is isometric.

#### Lemma 8 {#ts-iv-s2-lem-8 .statement tag=02Z2}

Let $(g_n)$ be a bounded sequence in $\mathscr{L}^{\infty}(X, \mu)$ converging pointwise $\mu$-almost everywhere. Let $\widetilde{m}\in L^{\infty}(X, \mu)$ be the class of its limit. Then $\widetilde{m}_{g_n}$ converges to $\widetilde{m}_{\widetilde{g}}$ in the space $\mathscr{L}(L^p(X, \mu))$ endowed with the topology of simple convergence.

Let $f\in \mathscr{L}^p(X, \mu)$. The sequence $(g_nf)$ is bounded in $\mathscr{L}^p(X, \mu)$ and converges pointwise $\mu$-almost everywhere to $gf$. By Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6), the sequence $(g_nf)$ converges to $gf$ in $\mathscr{L}^p(X, \mu)$, and the assertion follows.

We shall now consider the case where $p= 2$.

#### Proposition 6 {#ts-iv-s2-prop-6 .statement tag=02Z3}

The mapping $m:g\mapsto \widetilde{m}_g$ is an isometric unital morphism of the involutive algebra $L^{\infty}(X, \mu)$ into the involutive algebra $\mathscr{L}(L^2(X, \mu))$.

In particular, for every $g\in L^{\infty}(X, \mu)$, the multiplication endomorphism $\widetilde{m}_g$ is normal; it is hermitian if and only if $g$ is locally $\mu$-almost everywhere real-valued.

By Prop. 5, the mapping $\widetilde{m}$ is an injective isometric morphism of unital Banach algebras of $L^{\infty}(X, \mu)$ into $\mathscr{L}(L^2(X, \mu))$. Let $g\in \mathscr{L}^{\infty}(X, \mu)$. For $f_1$ and $f_2\in \mathscr{L}^2(X, \mu)$, one has

$$
\langle f_1|\widetilde{m}_g(f_2)\rangle =\int_X\overline{f_1(x)}g(x)f_2(x)d\mu(x) =\langle \widetilde{m}_{\overline{g}}(f_1)|f_2\rangle
$$

whence it follows that $\widetilde{m}^*_g=\widetilde{m}_{\overline{g}}$, which proves that $m$ is an involutive morphism. The final assertions follow from this (cf. I, p. 106, Prop. 5).

#### Corollary {#ts-iv-s2-n5-cor-1 .statement tag=02Z4}

Let $g\in L^{\infty}(X, \mu)$.

a) The spectrum of $\widetilde{m}_g$ in $\mathscr{L}(L^2(X, \mu))$ is the μ-essential image of $g$;

b) The endomorphism $\widetilde{m}_g$ is positive if and only if $g$ is locally μ-almost everywhere with positive values;

c) For every function $f\in \mathscr{C}$ (Sp($\widetilde{m}_g$)), one has $f(\widetilde{m}_g) =\widetilde{m}_{f\circ g}$.

Since $\widetilde{m}$ is injective, one has Sp($\widetilde{m}_g$) $=$ Sp($g$) by Prop. 5 of I, p. 106; the result then follows from Lemma 6 of IV, p. 185, from Proposition 4 of IV, p. 185 and from Definition 6 of I, p. 115.

#### Proposition 7 {#ts-iv-s2-prop-7 .statement tag=02Z5}

The image of the morphism $\widetilde{m}$ from $L^{\infty}(X, \mu)$ into $\mathscr{L}(L^2(X, \mu))$ is a maximal commutative subalgebra of the algebra $\mathscr{L}(L^2(X, \mu))$.

It is enough to prove that if $u\in \mathscr{L}(L^2(X, \mu))$ is an endomorphism which commutes with $\widetilde{m}_g$ for every function $g\in \mathscr{L}^{\infty}(X, \mu)$, then $u$ belongs to the image of $\widetilde{m}$. Let $u$ be such an endomorphism.

We denote by $\widetilde{f}$ the class in $L^2(X, \mu)$ of a function $f\in \mathscr{L}^2(X, \mu)$. Let $v$ denote the linear mapping from $\mathscr{L}^2(X, \mu)$ into $L^2(X, \mu)$ defined by $f\mapsto u(\widetilde{f})$. One has $v\circ m_g=\widetilde{m}_g\circ v$ for every $g\in \mathscr{L}^{\infty}(X, \mu)$.

For every μ-measurable subset Y of X, let $\varphi_Y$ denote its characteristic function; the endomorphism $\widetilde{m}_{\varphi_Y}$ is an orthogonal projector of $L^2(X, \mu)$.

Suppose first that X is compact, so that the class of the constant function 1 belongs to $L^2(X, \mu)$. Let $g$ be a function in $\mathscr{L}^2(X, \mu)$ whose class in $L^2(X, \mu)$ is $v(1)$.

Let $c$ be a positive real number and Y the set of $x\in X$ such that $|g(x)|\geqslant c$; this is a μ-measurable set. One has in $L^2(X, \mu)$ the equalities $\varphi_{\widetilde{Y}}g=\widetilde{m}_{\varphi_Y}(v(1)) =v(m_{\varphi_Y}(1)) =v(\varphi_Y)$.

Since moreover $|c\varphi_Y|\leqslant |g\varphi_Y|$, one obtains

$$
c^2\mu(Y) =\int_X(c\varphi_Y)^2d\mu\leqslant \int_X|\varphi_Yg|^2d\mu=\|\widetilde{u}(\varphi_Y)\|^2\leqslant \|u\|^2\mu(Y)
$$

This inequality implies that $\mu(Y) = 0$ if $c >\|u\|$, so that the function $g$ is bounded μ-almost everywhere by $\|u\|$. Finally, for every function $f\in \mathscr{C}$(X), one has

$$
u(\widetilde{f}) =v(m_f(1)) =\widetilde{m}_f(v(1)) =\widetilde{m}_f(\widetilde{g}) =\widetilde{m}_g(\widetilde{f})
$$

whence the equality $u=\widetilde{m}_g$, and in particular $N_{\infty}(g) =\|u\|$.

Let us now consider the general case. There exists a locally countable family $(X_i)_{i\in I}$ of pairwise disjoint compact subsets of X such that Z = X $-\bigcup_{i\in I}X_i$ is locally $\mu$-negligible (INT, IV, p .190, § 5, n$^o9$, prop. 14). Let $\mu_i$ denote the measure induced by $\mu$ on $X_i$ (INT, IV, p. 186, § 5, n$^o7$, def. 4).

By prop. 1 of IV, p. 179, for every $i\in I$, the image $E_i$ of $\widetilde{m}_{\varphi_{Xi}}$ is identified with $L^2(X_i, \mu_i)$ by $f\mapsto f|X_i$. For every function $g\in \mathscr{L}^{\infty}(X, \mu)$, the multiplication endomorphism $\widetilde{m}_g$ commutes with $\widetilde{m}_{\varphi_{Xi}}$, hence leaves $E_i$ stable, and the endomorphism of $E_i$ deduced from $\widetilde{m}_g$ by passing to subspaces coincides with the multiplication endomorphism by $g|X_i$ on $L^2(X_i, \mu_i)$.

Since $u$ commutes with $m_{\varphi_{Xi}}$, it likewise leaves the subspace $E_i$ stable. Let $u_i$ denote the endomorphism of $L^2(X_i, \mu_i)$ deduced from $u$ by passing to subspaces.

The map from $\mathscr{L}^{\infty}(X, \mu)$ into $\mathscr{L}^{\infty}(X_i, \mu_i)$ defined by $g\mapsto g|X_i$ being surjective, the hypothesis implies that $u_i$ commutes with $\widetilde{m}_g$ for every function $g\in \mathscr{L}^{\infty}(X_i, \mu_i)$. By the first part of the proof, there exists a function $g_i\in \mathscr{L}^{\infty}(X_i, \mu_i)$ such that $u_i=\widetilde{m}_{g_i}$ and $N_{\infty}(g_i)\leqslant \|u_i\|\leqslant \|u\|$.

The function $g$ on X which coincides with $g_i$ on $X_i$ and which is zero on Z is bounded and $\mu$-measurable (INT, IV, p. 193, § 5, n$^o10$, prop. 16), hence $g\in \mathscr{L}^{\infty}(X, \mu)$. For every $i\in I$, the restriction of $u$ to $E_i$ coincides with that of $\widetilde{m}_g$; therefore one has $u=m_g$ by prop. 1, c) of IV, p. 179.

#### Corollary {#ts-iv-s2-n5-cor-2 .statement tag=02Z6}

Let $u$ be an endomorphism of the Hilbert space $L^2(X, \mu)$ commuting with $\widetilde{m}_g$ for every function $g\in \mathscr{K}(X)$. Then there exists a unique element $f\in L^{\infty}(X, \mu)$ such that $u=\widetilde{m}_f$.

After Prop. 7, it is enough to prove that $u$ commutes with $\widetilde{m}_g$ for every $g\in \mathscr{L}^{\infty}(X, \mu)$. Let $h_1$ and $h_2$ be elements of $\mathscr{L}^2(X, \mu)$ with classes $\widetilde{h}_1$ and $\widetilde{h}_2$ in $L^2(X, \mu)$. Let $k_1$ (resp. $k_2$) be a function in $\mathscr{L}^2(X, \mu)$ whose class is $u(\widetilde{h}_1)$ (resp. $u^*(\widetilde{h}_2)$).

Let us set $h=h_1\overline{k}_2-k_1\overline{h}_2$; then $h\in \mathscr{L}^1(X, \mu)$. Define the measure $\nu =h\cdot \mu$ on X; it is bounded. For every $g\in \mathscr{L}^{\infty}(X, \mu)$, one has

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\langle u^*(\widetilde{h}_2)|\widetilde{m}_g(\widetilde{h}_1)\rangle  - \langle \widetilde{h}_2|\widetilde{m}_g(u(\widetilde{h}_1))\rangle
$$

$$
=\int_Xg\cdot h_1\cdot \overline{k}_2d\mu-\int_Xg\cdot k_1\cdot \overline{h}_2d\mu=\nu (g)
$$

Hence by hypothesis $\nu (g) = 0$ for every function $g\in \mathscr{K}$ (X), that is, $\nu = 0$. Consequently, one obtains

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\nu (g) = 0
$$

for every $g\in \mathscr{L}^{\infty}(X, \mu)$. Since this is the case for all $h_1$ and $h_2$ in $\mathscr{L}^2(X, \mu)$, one has $u\circ \widetilde{m}_g=\widetilde{m}_g\circ u$.

#### Remark {#ts-iv-s2-n5-rem-1 .statement tag=02Z7}

In the sequel, we shall often denote simply by $m_g$ the endomorphism of multiplication by $g$ on $L^p(X, \mu)$.

### 6. Spectral Measures

In this number, we fix a complex Hilbert space E.

Recall that if A is a commutative unital stellar algebra, one denotes by $\mathsf{X}(A)$ the compact topological space of its unital characters (Cor. 1 of I, p. 29) and by $\mathscr{G}_A$ the Gelfand transform of A (Def. 5 of I, p. 7), which is an isometric isomorphism of involutive unital algebras of A onto $\mathscr{C}(\mathsf{X}(A))$ (Theorem 1 of I, p. 108). We shall denote by $\mathscr{H}_A$ the inverse isomorphism.

#### Lemma 9 {#ts-iv-s2-lem-9 .statement tag=02Z8}

Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. For every $x$ and $y$ in E, the mapping $\mu$ of $\mathsf{X}(A)$ into $\mathbf{C}$ defined by $\mu(f) =\langle x|\mathscr{H}_A(f)y\rangle$ for every $f\in \mathscr{C}(\mathsf{X}(A))$ is a bounded measure on the compact space $\mathsf{X}(A)$. It is positive if $x=y$. Its norm is $\leqslant \|x\| \|y\|$, with equality if $x=y$.

The mapping $\mu$ is linear. For every function $f\in \mathscr{C}(\mathsf{X}$(A)), one has

$$
|\mu(f)|\leqslant \|x\| \|y\| \|\mathscr{H}_A(f)\|=\|x\| \|y\| \|f\|
$$

hence $\mu$ is a bounded measure on $\mathsf{X}(A)$ of norm $\leqslant \|x\| \|y\|$.

Suppose that $x=y$. For every positive function $f\in \mathscr{C}(\mathsf{X}$(A)), the element $\mathscr{H}_A(f)$ is a positive element of A (example 1 of I, p. 115), hence a positive element of $\mathscr{L}$ (E), whence $\mu(f) =\langle x|\mathscr{H}_A(f)(x)\rangle \geqslant 0$ (prop. 8 of I, p. 138). This shows that $\mu$ is a positive measure. Since $\mu(1) =\|x\|^2$, the total mass of $\mu$ is $\|x\|^2$ (INT, III, p. 58, § 1, No.$^o8$, cor. 2).

#### Definition 2 {#ts-iv-s2-def-2 .statement tag=02Z9}

Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. For every $x$ and $y$ in E, the linear form $f\mapsto  \langle x|\mathscr{H}_A(f)y\rangle$ on $\mathscr{C}(\mathsf{X}(A))$ is called the spectral measure of $(x, y)$ relative to A. If $x=y$, it is said to be the spectral measure of $x$ relative to A.

#### Remark {#ts-iv-s2-n6-rem-1 .statement tag=02ZA}

Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. For every $x$ and $y$ in E, let $\mu_{x,y}$ denote the spectral measure of $(x, y)$ relative to A. The mapping defined by $(x, y)\mapsto \mu_{x,y}$ of $E\times E$ into $\mathscr{M}^1(\mathsf{X}(A))$ is sesquilinear.

Let $u$ be a normal endomorphism of E and A the unital stellar subalgebra of $\mathscr{L}(E)$ generated by $u$. It is commutative. The space $\mathsf{X}(A)$ is identified with Sp($u$) by the mapping $\chi \mapsto \chi (u)$ (lemma 10 of I, p. 109). The spectral measure $\mu_{x,y}$ of $(x, y)$ relative to A is therefore identified with a measure on Sp($u$), called the spectral measure of $(x, y)$ relative to $u$. For every function $f\in \mathscr{C}$ (Sp($u$)), one then has

$$
\int f d\mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$)

by def. 5 of I, p. 110.

### 7. Commutative stellar algebras of endomorphisms of a Hilbert space

#### Definition 3 {#ts-iv-s2-def-3 .statement tag=02ZB}

Let A be an algebra over $\mathbf{C}$ and E a complex topological vector space. Let $\pi$ be a representation of A in E. An element $x$ of E is said to be a cyclic vector for $\pi$ if the set of elements $\pi (a)x$ for $a\in A$ is total in E.

Let $u\in \mathscr{L}(E)$ be an endomorphism of E. It is said that $x\in E$ is a cyclic vector for $u$ if it is a cyclic vector for the identical representation of the stellar subalgebra generated by $u$ in $\mathscr{L}(E)$.

#### Proposition 8 {#ts-iv-s2-prop-8 .statement tag=02ZC}

Let E be a complex Hilbert space. Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. Let $x$ be an element of E. Put $E_x= A\cdot x$ and let $\mu_x$ denote the spectral measure of $x$ relative to A.

There exists a unique isometric isomorphism $\theta_x$ of $L^2(\mathsf{X}(A), \mu_x)$ onto $E_x$ such that $\theta_x(f) =\mathscr{H}_A(f)(x)$ for every function $f\in \mathscr{C}(\mathsf{X}(A))$. For every element $a\in A$, the space $E_x$ is stable under $a$, and if $a_x$ denotes the endomorphism of $E_x$ deduced from $a$ by passing to subspaces, then one has $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

Let $\widetilde{\theta}_x$ be the linear mapping of $\mathscr{C}(\mathsf{X}(A))$ into $E_x$ defined by

$$
\widetilde{\theta}_x(f) =\mathscr{H}_A(f)(x)
$$

For every function $f\in \mathscr{C}(\mathsf{X}$(A)), one has

$$
\|\widetilde{\theta}_x(f)\|^2=\langle \mathscr{H}_A(f)x|\mathscr{H}_A(f)x\rangle =\langle x|\mathscr{H}_A(|f|^2)x\rangle =\int_{\mathsf{X}(A)}|f|^2d\mu_x
$$

Since $\mathscr{C}(\mathsf{X}(A))$ is dense in $\mathscr{L}^2(\mathsf{X}(A), \mu_x)$, there exists a unique isometric linear mapping of $L^2(\mathsf{X}(A), \mu_x)$ into $E_x$ extending $\widetilde{\theta}_x$; let $\theta_x$ denote it. The mapping $\theta_x$ is surjective since its image is closed (lemma 8 of I, p. 107) and contains $A\cdot x$. It is therefore an isometric isomorphism.

Let $a\in A$. Put $g=\mathscr{G}_A(a)\in \mathscr{C}(\mathsf{X}(A))$. The space $E_x$ is stable under $a$. For $f\in \mathscr{C}(\mathsf{X}$(A)), one has then

$$
\widetilde{\theta}_x(m_g(f)) =\mathscr{H}_A(\mathscr{G}_A(a)f)x= (a\circ \mathscr{H}_A(f))x=a(\widetilde{\theta}_x(f))
$$

and it follows that $\theta_x\circ m_g=a_x\circ \theta_x$.

#### Corollary {#ts-iv-s2-n7-cor-1 .statement tag=02ZD}

Let E be a complex Hilbert space. Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$ admitting a cyclic vector $x$. Let $\mu_x$ be the spectral measure of $x$ relative to A. There exists a unique isometric isomorphism

$$
\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E
$$

such that $\theta_x(f) =\mathscr{H}_A(f)$ for every function $f\in \mathscr{C}(\mathsf{X}(A))$. For every $a$ in A, one has $a\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

In fact, one has then $E_x= E$ and $a_x=a$ for every $a\in A$.

Let E be a complex Hilbert space. Let $x\in E$ and let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. Let $E_x$ denote the closed subspace $A\cdot x$ of E. For every $a\in A$, one has then $a(E_x)\subset E_x$. Let $A_x$ denote the commutative unital stellar subalgebra of $\mathscr{L}(E_x)$ formed by the endomorphisms of $E_x$ deduced from the elements of A by passing to subspaces. The vector $x$ is a cyclic vector for $A_x\subset \mathscr{L}(E_x)$.

#### Proposition 9 {#ts-iv-s2-prop-9 .statement tag=02ZE}

There exists a subset C of E such that E is the Hilbert sum of the spaces $E_x$ for $x\in$ C. If E is of countable type, the set C is countable.

Let $\mathscr{O}$ be the set of subsets C of E such that the subspaces $E_x$ for $x\in C$ are pairwise orthogonal. The set $\mathscr{O}$, ordered by inclusion, is of finite character (E, III, p. 34, Def. 2) since C belongs to $\mathscr{O}$ if and only if the sets formed of two elements of C belong to $\mathscr{O}$. By E, III, p. 35, Theorem 1, there exists a maximal element C of $\mathscr{O}$.

Let F be the closed subspace of E generated by the subspaces $E_x$ for $x\in C$. It is enough to prove that $F^{\circ}$ is reduced to 0 in order to complete the proof of the proposition. Let $y$ be an element of $F^{\circ}$. For every $x\in C$ and every $a$ and $b$ in A, we have $\langle a(y)|b(x)\rangle =\langle y|a^*b(x)\rangle = 0$ since $a^*b(x)$ belongs to $E_x$, hence to F. Since the elements $a(y)$ (resp. $b(x)$) generate a dense subspace of $E_y$ (resp. $E_x$), we therefore have $E_y\subset E^{\circ}_x$. Since C is maximal in $\mathscr{O}$, this means that $E_y$ is reduced to 0, hence that $y= 0$.

Suppose that E is of countable type. Since $E_x$ is nonzero for every nonzero $x\in C$, every set C such that E is the Hilbert sum of the spaces $E_x$ for $x\in C$ is countable.

#### Theorem 1 {#ts-iv-s2-thm-1 .statement tag=02ZF}

Let A be a commutative unital stellar subalgebra of $\mathscr{L}(E)$. There exist a locally compact topological space X, a positive measure $\mu$ on X, an isometric isomorphism $\theta$ of $L^2(X, \mu)$ onto E, and an isometric morphism of stellar algebras $\pi$ of A into $\mathscr{C}_b(X)$ such that for every $a\in A$, one has

$$
a\circ \theta =\theta \circ m_{\pi(a)}
$$

By Prop. 9, there exists a subset C of E such that E is the Hilbert sum of the subspaces $E_x$ for $x\in C$. Let X be the locally compact topological space $\mathsf{X}(A)\times C$, where C is endowed with the discrete topology. There exists a unique measure $\mu$ on X such that $\mu|(\mathsf{X}(A)\times  \{x\})$ is identified with the spectral measure $\mu_x$ of $x$ for every $x\in C$ (INT, III, p. 65, § 2, n$^o1$, Prop. 1); this measure is positive (cf. loc. cit.). One then has a decomposition as Hilbert sum

$$
L^2(X, \mu) =\bigoplus_{x\in C}L^2(\mathsf{X}(A), \mu_x)
$$

(Prop. 1 of IV, p. 179, c) applied to the sets $\mathsf{X}(A)\times  \{x\}$ for $x\in C)$. There therefore exists a unique isometry $\theta : L^2(X, \mu)\rightarrow E$ which coincides with $\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E_x$ on $L^2(\mathsf{X}(A), \mu_x)$ for every $x\in C$.

Let $p: X\rightarrow \mathsf{X}(A)$ be the canonical projection; it is surjective, hence the linear mapping $p^*:\mathscr{C}_b(\mathsf{X}(A))\rightarrow \mathscr{C}(X)$ defined by $f\mapsto f\circ p$ is injective. Let us write $\pi =p^*\circ \mathscr{G}_A$; it is an injective morphism of stellar algebras of A into $\mathscr{C}_b(X)$; it is therefore isometric (Prop. 9 of I, p. 112).

Let $a\in A$. For every $x\in C$, we have $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$. The continuous linear mappings $a\circ \theta$ and $\theta \circ m_{\pi(a)}$ therefore coincide on the subspaces $L^2(\mathsf{X}(A), \mu_x)$, and are consequently equal.

#### Corollary (Spectral Theorem) {#ts-iv-s2-n7-cor-2 .statement tag=02ZG}

Let E be a complex Hilbert space. Let $u\in \mathscr{L}(E)$ be a normal endomorphism of E. There exist a locally compact topological space X, a positive measure $\mu$ on X, an isometric isomorphism $\theta$ of $L^2(X, \mu)$ onto E, and a continuous bounded function $g$ on X such that $u=\theta \circ m_g\circ \theta^{-1}$.

If $u$ admits a cyclic vector $x$, one may take X = Sp($u$) and for $g$ the identity function of X.

It is enough to apply theorem 1 (resp. the corollary of proposition 8) to the involutive subalgebra A of $\mathscr{L}(E)$ generated by $u$, and to put $g=\pi (u)$.

This statement reduces every question concerning a single normal endomorphism of a Hilbert space to a similar question for a multiplication operator, which often simplifies its study (cf. for example exercise 19 of IV, p. 325).

### 8. Continuity of the Functional Calculus

In this number, we consider the continuity properties of the functional calculus with respect to the two variables.

For an involutive algebra A and a normal element $a$ of A, and for a continuous function $f$ on a subset of $\mathbf{C}$ containing Sp$_A(a)$, we denote by $f(a)$ the element obtained by the continuous functional calculus of $a$ applied to the restriction of $f$ to the spectrum of $a$.

#### Proposition 10 {#ts-iv-s2-prop-10 .statement tag=02ZH}

Let A be a unital involutive algebra. Let U be a relatively compact open subset of $\mathbf{C}$. Let $\Omega_n$ denote the set of normal elements of A such that Sp$_A(a)$ is contained in U. The mapping $(f, a)\mapsto f(a)$ of $\mathscr{C}(U)\times \Omega_n$ into A is continuous.

Let $q$ denote the mapping $(f, a)\mapsto f(a)$ of $\mathscr{C}(U)\times \Omega_n$ into A. The set of functional-calculus mappings $f\mapsto f(a)$ for $a\in \Omega_n$ is equicontinuous in $\mathscr{L}(\mathscr{C}(U); A)$, since each is a continuous linear mapping of norm $\leqslant 1$. To prove the assertion, it is therefore enough to verify that, for every $f\in \mathscr{C}$ (U), the mapping of $\Omega_n$ into A defined by $a\mapsto f(a)$ is continuous (TG, X, p. 13, cor. 3).

Let $\mathscr{A}$ be the set of $f\in \mathscr{C}(U)$ such that the mapping $a\mapsto f(a)$ of $\Omega_n$ into A is continuous; it remains to prove that $\mathscr{A}=\mathscr{C}(U)$.

The set $\mathscr{A}$ is a unital involutive subalgebra of $\mathscr{C}(U)$. It contains the identity function of U, and therefore separates points. Consequently, it is dense in $\mathscr{C}(U)$ (TG, X, p. 39, prop. 7). Let us prove that it is closed.

Let $(f_n)$ be a sequence in $\mathscr{A}$ converging to $f\in \mathscr{C}(U)$. Let $\varepsilon  >0$ and choose $n\in \mathbf{N}$ such that $\|f-f_n\|_{\infty}\leqslant \varepsilon /4$. For every $(a_1, a_2)\in \Omega^2_n$ we have

$$
\|f(a_1)-f(a_2)\|\leqslant 2\|f-f_n\|_{\infty}+\|f_n(a_1)-f_n(a_2)\|
$$

$$
\varepsilon
$$

$$
\leqslant +\|f_n(a_1)-f_n(a_2)\|
$$

2

Since $f_n$ belongs to $\mathscr{A}$, there exists a neighbourhood V of $a_1$ in $\Omega_n$ such that $\|f_n(a_1)-f_n(a_2)\|\leqslant \varepsilon /2$ for every $a_2\in$ V. Hence $\|f(a_1)-f(a_2)\|\leqslant \varepsilon$ for every $a_2\in V$. The mapping $a\mapsto f(a)$ is therefore continuous at $a_1$; the assertion is proved.

#### Corollary 1 {#ts-iv-s2-prop-10-cor-1 .statement tag=02ZI}

Let A be a unital star algebra and let $A_n$ be the set of normal elements of A. Endow the space $\mathscr{C}(\mathbf{C})$ with the topology of compact convergence. The mapping $(f, a)\mapsto f(a)$ of $\mathscr{C}(\mathbf{C})\times A_n$ into A is continuous.

Let $(f_0, a_0)\in \mathscr{C}(\mathbf{C})\times A_n$. Let U be a relatively compact neighbourhood of the spectrum of $a_0$. Let V be the set of normal elements $a$ of A such that Sp$_A(a)\subset U$; this is an open neighbourhood of $a_0$ in $A_n$ (I, p. 76, Prop. 10). For every $a\in V$ and every function $f\in \mathscr{C}(\mathbf{C})$, one has $f(a) = (f|U)(a)$. Since the mapping $f\mapsto  \|f|U\|_{\infty}$ is a continuous seminorm on $\mathscr{C}(\mathbf{C})$ endowed with the topology of compact convergence, the continuity of the mapping $(f, a)\mapsto f(a)$ at $(f_0, a_0)$ follows from Prop. 10.

#### Corollary 2 {#ts-iv-s2-prop-10-cor-2 .statement tag=02ZJ}

Let E be a complex Hilbert space and let $\mathscr{L}(E)_n$ be the set of normal endomorphisms of E. Endow the space $\mathscr{C}(\mathbf{C})$ with the topology of compact convergence. The mapping of $\mathscr{C}(\mathbf{C})\times \mathscr{L}(E)_n$ into $\mathscr{L}(E)$ defined by $(f, u)\mapsto f(u)$ is continuous.

## EXERCISES {#ts-iv-s2-exercises}

Unless otherwise stated, in the exercises of this paragraph, E denotes a complex Hilbert space.

See the [exercises for § 2](exercises/s2/).
