---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 4
section_title: Théorie de la descente
lang: en
source: ta-i-iv-fr
book_pages: TA IV.382-TA IV.405, TA IV.462-TA IV.463
pdf_pages: 0398-0421, 0478-0479
extraction: native
subsections:
    - "no": 1
      title: Données de descente
      page: 382
      pdf_page: 398
    - "no": 2
      title: Données de descente effectives
      page: 384
      pdf_page: 400
    - "no": 3
      title: Descente de morphismes
      page: 387
      pdf_page: 403
    - "no": 4
      title: 'Descente : cas des espaces étalés'
      page: 388
      pdf_page: 404
    - "no": 5
      title: 'Descente : cas des revêtements'
      page: 390
      pdf_page: 406
    - "no": 6
      title: Descente de groupoïdes
      page: 394
      pdf_page: 410
    - "no": 7
      title: Descente par une application étale et surjective
      page: 399
      pdf_page: 415
    - "no": 8
      title: Groupoïde de Poincaré d’un espace quotient
      page: 402
      pdf_page: 418
statements: 29
exercises: 7
content_sha256: a9cfa1530684da37c0beb2dba5cd1ad16832230c665fd22fc8bc4f1c1f58d3a3
translated_from: content/fr/ta/IV/04_s4_theorie_de_la_descente.md
source_lang: fr
translation_method: machine
source_content_sha256: 426b9763b4b18b5eb0a9925025a7e53d8ed98667d5b656984d09078aa3d796af
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-6f41c41b
glossary_version: 34
glossary_terms_sha256: 1dda6eecfd1e3142e943edd73dbff3fe62d413a86a6561ed87744225c1a337f5
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. THEORY OF DESCENT

### 1. Descent data

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. Let $(Z, p)$ be an X-space.

#### Definition 1 {#ta-iv-s4-def-1 .statement tag=0227}

A descent data relative to $f$ on the X-space $(Z, p)$ is called a continuous mapping $\tau : Z\times_YX\rightarrow Z$ satisfying the following two properties:

(i) For every pair $(x, x')\in X\times_YX$, the mapping $z\mapsto \tau (z, x')$ induces by restriction a bijection $\tau_{x,x'}$ of $Z_x$ onto $Z_{x'}$;

(ii) For every triplet $(x, x', x'')$ of points of X such that $f(x) =$ $f(x') =f(x'')$, one has

$$
\tau_{x,x''}=\tau_{x',x''}\circ \tau_{x,x'}
$$

If $\tau$ is a descent data on $(Z, p)$, the family $(\tau_{x,x'})$, for $(x, x')\in X\times_YX$, is thus a law of operation (on the right) of the groupoid $X\times_YX$ on the X-space $(Z, p)$ (II, p. 167). In particular, one has $\tau_{x,x}=$ Id$_{Z_x}$ for every $x\in X$, which is also written $\tau (z, p(z)) =z$ for every $z\in Z$. Conversely, given a law of operation (on the right) of the groupoid $X\times_YX$ on $(Z, p)$, the map from $Z\times_YX$ into Z defined by $(z, x)\mapsto z\cdot (p(z), x)$ verifies the relations (i) and (ii) of the definition.

Let X and Y be topological spaces, $f: X\rightarrow Y$ a continuous mapping and let $(Z, p)$ be an X-space. If $\tau$ is a descent data relative to $f$ on $(Z, p)$, the relation $R_{\tau}(z_1, z_2)$ defined by « $f(p(z_1)) =$ $f(p(z_2))$ and $\tau (z_1, p(z_2)) =z_2$ » is the equivalence relation in Z deduced from the operation of the groupoid $X\times_YX$ defined by $\tau$; it is compatible with the mapping $f\circ p$. It is said that this is the equivalence relation associated with the descent data $\tau$. The canonical bijection $(z_1, z_2)\mapsto (z_1, p(z_2))$ of the graph Γ of the equivalence relation $R_{\tau}$ onto $Z\times_YX$ is a homeomorphism, the reciprocal homeomorphism applies an element $(z_1, x_2)\in Z\times_YX$ to $(z_1, \tau (z_1, x_2))$.

Conversely, let R be an equivalence relation in Z compatible with the mapping $f\circ p: Z\rightarrow Y$ and let Γ be the graph of R. Suppose moreover that the mapping $p_2: (z_1, z_2)\mapsto (z_1, p(z_2))$ defines a homeo-morphism of Γ onto $Z\times_YX$. The mapping $\tau : Z\times_YX\rightarrow Z$ given by pr$_2\circ p^{-1}_2$ is continuous; it is a descent data relative to $f$ on $(Z, p)$ and the relation R is the equivalence relation associated with $\tau$.

#### Example 1 {#ta-iv-s4-n1-exa-1 .statement tag=0228}

Let X and Y be topological spaces, let $f: X\rightarrow Y$ be a continuous mapping and let $(T, q)$ be a Y-space. Put $Z = X\times_YT$. The mapping $\tau$ from $Z\times_YX$ into Z which associates with $((x, t), x')$ the element $(x', t)$ is a descent datum relative to $f$ on the X-space $(X\times_YT$, pr$_1)$, called the canonical descent datum. For $z_1= (x_1, t_1)$ and $z_2= (x_2, t_2)\in Z$, the relation $R_{\tau}\{z_1, z_2\}$ is equivalent to $t_1=t_2$.

#### Example 2 {#ta-iv-s4-n1-exa-2 .statement tag=0229}

Let Y be a topological space, $(V_i)_{i\in I}$ a family of subsets of Y, and for each $i\in I$, let $(Z_i, p_i)$ be a $V_i$-space. Let X denote the sum topological space of the family $(V_i)_{i\in I}$ and $(Z, p)$ the X-space sum of the family $(Z_i)_{i\in I}$. Let $f: X\rightarrow Y$ be the canonical mapping.

The space $X\times_YX$ is then identified with the sum space of the family $(V_i\cap$ $V_j)_{(i,j)\in I\times I}($I, p. 4, Example 5). Let $\tau$ be a descent datum relative to $f$ on $(Z, p)$. For each pair $(i, j)\in I\times I$, define a continuous mapping $\tau_{i,j}:\overset{-1}{p_{i}}(V_i\cap V_j)\rightarrow \overset{-1}{p_{j}}(V_i\cap V_j)$ by $z\mapsto \tau (z,(p_i(z), j))$. The family $(\tau_{i,j})$ satisfies the following properties:

(i) For each $i\in I$, one has $\tau_{i,i}=$ Id$_{Z_i}$;

(ii) For each pair $(i, j)\in I\times I,\tau_{i,j}$ is an isomorphism of $(V_i\cap V_j)$-spaces ;

(iii) For each triple $(i, j, k)\in I\times I\times I$ and each $z\in \overset{-1}{p_{i}}(V_i\cap V_j\cap V_k)$, one has $\tau_{j,k}(\tau_{i,j}(z)) =\tau_{i,k}(z)$.

Conversely, every family $(\tau_{i,j})$ possessing the above properties arises from a unique descent datum relative to $f$ on $(Z, p)$.

### 2. Effective descent data

Let X and Y be topological spaces, $f: X\rightarrow Y$ a continuous mapping and $(Z, p)$ an X-space. Let $\tau$ be a descent datum relative to $f$ on $(Z, p)$, let $R_{\tau}$ be the associated equivalence relation and let $g: Z\rightarrow Z/R_{\tau}$ be the canonical mapping. Since the relation $R_{\tau}$ is compatible with the mapping $f\circ p$, there exists a unique continuous mapping $q: Z/R_{\tau}\rightarrow Y$ such that the diagram

Z $^gZ/R_{\tau}$

$$
pq \tag{1}
$$

X $^f$ Y

let it be a commutative square. The Y-space $(Z/R_{\tau}, q)$ is called the quotient space of $(Z, p)$ by the descent datum $\tau$. Let us denote by $h: Z\rightarrow X\times_Y$ $(Z/R_{\tau})$ the mapping defined by $h(z) = (p(z), g(z))$ for $z\in Z$. It is continuous. Let $(x, u)\in X\times_Y(Z/R_{\tau})$ and let $z\in Z$ be such that $g(z) =u$; then we have $(z, x)\in Z\times_YX$ and the point $z'=\tau (z, x)$ is the unique element of Z such that $h(z') = (x, u)$; consequently, the mapping $h$ is bijective.

One says that the descent datum $\tau$ relative to $f$ on $(Z, p)$ is effective if diagram (1) is a cartesian square, that is to say, if the continuous bijection $h$ is a homeomorphism. In order that the descent datum $\tau$ be effective, it is necessary and sufficient that the sets $\overset{-1}{p}(U)\cap V$, where U is an open subset of X and V an open subset of Z saturated for $R_{\tau}$, constitute a basis of the topology of Z. In particular, the condition for a descent datum relative to $f$ to be effective is of a local nature on Y.

#### Example 1 {#ta-iv-s4-n2-exa-1 .statement tag=022A}

Let X and Y be topological spaces and $f: X\rightarrow Y$ a continuous mapping. Let $(T, q)$ be a Y-space. Let Z be the X-space $X\times_YT$, endowed with the mapping pr$_1$; let us denote by $\tau$ its canonical descent datum relative to $f$ (IV, p. 383, Example 1). The subsets of Z of the form $X\times_YV$, where V is an open subset of T, are open in Z and saturated for the relation $R_{\tau}($loc. cit.). By definition of the product topology, the sets $U\times_Y$ pr$^{-1}_2(V)$, where U is open in X and V is open in T, form a basis of the topology of $X\times_YZ$. Consequently, the canonical descent datum on a fibred product $X\times_YT$ is effective.

The canonical mapping $Z/R_{\tau}\rightarrow T$ is injective and continuous. It is not, however, necessarily surjective, nor strict (IV, p. 462, exerc. 1).

#### Example 2 {#ta-iv-s4-n2-exa-2 .statement tag=022B}

Let us take up again the notation of Example 2 (IV, p. 383). The topological space $Z/R_{\tau}$ is then the topological space obtained by gluing the spaces $Z_i$ along the $\overset{-1}{p_{i}}(V_i\cap V_j)$ by means of the bijections $\tau_{i,j}$ (TG, I, p. 16). Consequently, if for every $i\in I$, the set $V_i$ is open (resp. closed) in Y, the set $g(Z_i)$ is open (resp. closed) in $Z/R_{\tau}$ and the restriction of $g$ to $Z_i$ induces a homeomorphism of $Z_i$ onto $g(Z_i)$ (TG, I, p. 17, Prop. 9). The space Z is the sum space of the spaces $Z_i$; the space $X\times_Y(Z/R_{\tau})$ is the sum space of the spaces $V_i\times_Y$ $(Z/R_{\tau}) =g(Z_i)$. The mapping $h$ is identified with the sum mapping of the mappings $g|Z_i: Z_i\rightarrow g(Z_i)$. It is therefore a homeomorphism, which shows that the descent datum $\tau$ is effective.

Without a particular assumption on the subsets $V_i$, it is not always true that the restriction of $g$ to $Z_i$ induces a homeomorphism of $Z_i$ onto its image; in this case, the descent datum $\tau$ is not effective (IV, p. 462, exerc. 2).

#### Proposition 1 {#ta-iv-s4-prop-1 .statement tag=022C}

Let X and Y be topological spaces, let $f: X\rightarrow Y$ be a continuous mapping. Suppose that every point of Y possesses a neighbourhood above which there exists a continuous section of the mapping $f$. Then every descent datum relative to $f$ on an X-space is effective.

Let $(Z, p)$ be an X-space and let $\tau$ be a descent datum relative to $f$ on $(Z, p)$. The assertion that $\tau$ is an effective descent datum is local in Y, which allows us to suppose that the mapping $f$ possesses a continuous section $s$. Let $g: Z\rightarrow Z/R_{\tau}$ and $q: Z/R_{\tau}\rightarrow Y$ denote the canonical mappings, and let $h: Z\rightarrow X\times_Y(Z/R_{\tau})$ be the mapping given by $z\mapsto (p(z), g(z))$. The mapping $h$ is bijective and continuous; it is enough to prove that it is a homeomorphism.

The mapping from Z into Z which, to $z$, associates $\tau (z, s(f(p(z))))$ is continuous and maps every element of Z to the unique element $z'$ of Z which is equivalent to it for the relation $R_{\tau}$ and such that $p(z')$ belongs to the image of $s$. It therefore defines, by passing to the quotient, a continuous mapping $t: Z/R_{\tau}\rightarrow Z$ which is a section of the mapping $g$. In particular, one has $f\circ p\circ t=q\circ g\circ t=q$.

For every $(x, u)\in X\times_Y(Z/R_{\tau})$, one has $f(p(t(u))) =f(x)$; let us then put $h'(x, u) =\tau (t(u), x)$. The resulting mapping $h'$ from $X\times_Y(Z/R_{\tau})$ into Z is continuous. For every $(x, u)\in X\times_Y(Z/R_{\tau})$, one has

$$
h(h'(x, u)) = (p(h'(x, u)), g(h'(x, u)))
$$

$$
= (p(\tau (t(u), x)), g(\tau (t(u), x)))
$$

$$
= (x, u)
$$

because $\tau (t(u), x)$ is equivalent to $t(u)$ for the relation $R_{\tau}$. This proves that the mapping $h\circ h'$ is the identity mapping of $X\times_Y(Z/R_{\tau})$. For $z\in Z$, one then has $t(g(z)) =\tau (z, s(f(p(z)))$ and $f(p(t(g(z)))) =f(p(z))$, whence $z=\tau (t(g(z)), p(z))$, by definition of the equivalence relation $R_{\tau}$. Thus one has $h'(h(z)) =z$ and $h'\circ h=$ Id$_Z$. The mapping $h$ is therefore a homeomorphism, which was to be proved.

#### Proposition 2 {#ta-iv-s4-prop-2 .statement tag=022D}

Let $f: X\rightarrow$ Y be a continuous mapping, let $(Z, p)$ be an X-space and let $\tau$ be a descent datum relative to $f$ on Z. The equivalence relation $R_{\tau}$ is closed if $f$ is proper; it is open if $f$ is open.

The mapping $\widetilde{\tau}: Z\times_YX\rightarrow$ X $\times_Y$ Z defined by $(z, x)\mapsto$ $(p(z), \tau (z, x))$ is a homeomorphism, with inverse mapping $(x, z)\mapsto (\tau (z, x), p(z))$. We have $\tau$ = pr$_2\circ \widetilde{\tau}$, where pr$_2: X\times_YZ\rightarrow$ Z is the second projection. If $f$ is proper, pr$_2$ is proper; if $f$ is open, pr$_2$ is open (I, p. 17, prop. 8). It follows that $\tau$ is proper (resp. open) if $f$ is. The saturation of a subset A of Z with respect to the relation $R_{\tau}$ is the image of $A\times_YX$ under $\tau$. Consequently, if $f$ is proper, the saturation of a closed subset is closed; if $f$ is open, the saturation of an open subset is open.

### 3. Descent of morphisms

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Let $(Z, p)$ and $(Z', p')$ be X-spaces endowed with descent data relative to $f$, denoted respectively by $\tau$ and $\tau '$. One says that an X-morphism $\varphi : Z\rightarrow Z'$ is compatible with the descent data $\tau$ and $\tau '$ if one has

$$
\tau '(\varphi (z), x) =\varphi (\tau (z, x))
$$

for every $(z, x)\in Z\times_YX$. It amounts to the same to say that the images under $\varphi$ of two equivalent points with respect to the relation $R_{\tau}$ are equivalent with respect to the relation $R_{\tau'}$. Such a morphism $\varphi$ defines, by passing to the quotients, a continuous mapping $\overline{\varphi}: Z/R_{\tau}\rightarrow Z'/R_{\tau'}$; it is a Y-morphism of spaces.

Let us denote by $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ the set of X-morphisms of Z into $Z'$ which are compatible with the descent data $\tau$ and $\tau '$.

#### Proposition 3 {#ta-iv-s4-prop-3 .statement tag=022E}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a continuous mapping. Let $(Z, p)$ and $(Z', p')$ be X-spaces endowed with descent data relative to $f$, denoted respectively by $\tau$ and $\tau '$. If the descent datum $\tau '$ is effective, the mapping $\varphi \mapsto \overline{\varphi}$ is a bijection of $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ onto $\mathscr{C}_Y(Z/R_{\tau}; Z'/R_{\tau'})$.

For every X-morphism $\varphi$ of Z into $Z'$ compatible with the descent data, the mapping $\overline{\varphi}$ is a Y-morphism. Conversely, let $g: Z\rightarrow Z/R_{\tau}$ and $g': Z'\rightarrow Z'/R_{\tau'}$ denote the canonical mappings, and let $\psi : Z/R_{\tau}\rightarrow Z'/R_{\tau'}$ be a Y-morphism. The mappings $p: Z\rightarrow X$ and $\psi \circ g: Z\rightarrow Z'/R_{\tau'}$ are Y-morphisms. The hypothesis that the descent datum $\tau '$ is effective means that the diagram

$$
{Z'}^{g'}Z'/R_{\tau'}
$$

$p'q'$

X $^f$ Y

is a cartesian square. Hence there exists a unique continuous mapping $\varphi : Z\rightarrow Z'$ such that $p'\circ \varphi =p$ and $g'\circ \varphi =\psi \circ g$. The first equality means that $\varphi$ is an X-morphism, the second equality means that $\varphi$ is compatible with the descent data and that $\overline{\varphi}=\psi$, whence the proposition.

### 4. Descent: case of spread spaces

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. Let T and $T'$ be Y-spaces; endow the X-spaces $X\times_YT$ and $X\times_YT'$ with their canonical descent data and denote by $\mathscr{C}_f(X\times_YT; X\times_YT')$ the set of X-morphisms of $X\times_YT$ into $X\times_YT'$ which are compatible with these descent data. For every Y-morphism $\varphi : T\rightarrow T'$, the X-morphism $f^*(\varphi ): (x, t)\mapsto$ $(x, \varphi (t))$ of $X\times_YT$ into $X\times_YT'$ is compatible with the canonical descent data. We shall denote by $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ the resulting mapping.

#### Proposition 4 {#ta-iv-s4-prop-4 .statement tag=022F}

Suppose that the mapping $f$ is strict and surjective and that T is a spread Y-space. Then the mapping $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ is bijective.

Let $\tau$ (resp. $\tau '$) denote the equivalence relation on $X\times_YT$ (resp. on $X\times_YT'$) associated with the canonical descent datum. Since the mapping $f$ is surjective, the projection pr$_2: X\times_YT\rightarrow T$ is surjective and the canonical mapping $(X\times_YT)/R_{\tau}\rightarrow T$ is bijective. In particular, the mapping $f^*$ is injective. Let us prove that it is surjective. Let $\varphi : X\times_YT\rightarrow X\times_YT'$ be an X-morphism compatible with the canonical descent data. Then for $(x, t)\in X\times_YT$, one has $\varphi (x, t) = (x, \varphi (t))$, where $\overline{\varphi}$ is a mapping of T into $T'$.

By definition of $\overline{\varphi}$, the mapping $\overline{\varphi}\circ$ pr$_2: X\times_YT\rightarrow T'$ is equal to pr$_2\circ \varphi$, and is therefore continuous. Since the mapping $f$ is surjective and strict and T is a spread Y-space, the projection pr$_2: X\times_YT\rightarrow T$ is strict (I, p. 32, remark 3). By proposition 9 of I, p. 18, the mapping $\overline{\varphi}$ is therefore continuous. It is a Y-morphism such that $f^*(\overline{\varphi}) =\varphi$, which proves the proposition.

#### Corollary {#ta-iv-s4-n4-cor-1 .statement tag=022G}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a strict and surjective mapping. Let T and $T'$ be spread Y-spaces. If there exists an X-isomorphism $X\times_YT\rightarrow X\times_YT'$ compatible with the canonical descent data, the Y-spaces T and $T'$ are isomorphic.

Let $\psi : X\times_YT\rightarrow X\times_YT'$ be an X-isomorphism of spread spaces. By proposition 4, there exists a unique morphism of Y-spaces $\varphi : T\rightarrow T'$ such that $\psi =f^*(\varphi )$. Since $f$ is surjective, the mapping $\varphi$ is bijective. It then follows from cor. 2 of I, p. 30 that $\varphi$ is an isomorphism, since the Y-spaces T and $T'$ are spread.

#### Proposition 5 {#ta-iv-s4-prop-5 .statement tag=022H}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. Suppose that the mapping $f$ is proper and separated, or else open. Every descent datum relative to $f$ on a spread X-space is effective. Moreover, if $f$ is surjective, the quotient space is a spread Y-space.

Let $(Z, p)$ be an X-étalé space and let $\tau$ be a descent datum relative to $f$ on $(Z, p)$. Let us denote by $R_{\tau}$ the equivalence relation in Z associated with $\tau$, let $g: Z\rightarrow Z/R_{\tau}$ be the canonical surjection and let $h$ denote the mapping of Z into $X\times_Y(Z/R_{\tau})$ defined by $z\mapsto (p(z), g(z))$. It is continuous and bijective; let us prove that it is a homeomorphism.

a) Suppose first that the mapping $f$ is open.

Let $z_0$ be a point of Z; put $x_0=p(z_0)$. Since $p$ is étale, there exists a neighbourhood U of $x_0$ in X and a continuous section $s: U\rightarrow Z$ of $p$ over U such that $s(x_0) =z_0$. The mapping $p\times p: Z\times_YZ\rightarrow$ $X\times_YX$ is étale, and the mappings of $U\times_YU$ into $Z\times_YZ$ defined by $(x, x')\mapsto (s(x), s(x'))$ and $(x, x')\mapsto (s(x), \tau (s(x), x'))$ are continuous sections of it over $U\times_YY$. Since they coincide at every point of $U\times_YU$ of the form $(x, x)$, they therefore coincide on an open neighbourhood V of $\Delta_U$ contained in $U\times_YU$. Let $U_0$ be a neighbourhood of $x_0$ in X such that $U_0\times_YU_0$ is contained in V. Let $(x, u)$ be a point of $U_0\times_Yg(s(U_0))$; let $x'\in U_0$ be such that $u=g(s(x'))$. We have therefore $s(x) =\tau (s(x'), x)$, whence $R_{\tau}\{s(x), s(x')\}$ and $(x, u) = (x, g(s(x'))) =$ $(x, g(s(x))) =h(s(x))$.

Since the mapping $g$ is open (IV, p. 386, prop. 2), the set $U_0\times_Yg(s(U_0))$ is an open subset of $X\times_Y(Z/R_{\tau})$ on which the mapping $h^{-1}$ is equal to the continuous mapping $s\circ$ pr$_1$. The mapping $h$ is therefore a homeomorphism.

b) Suppose now that the mapping $f$ is proper and separated.

Let $z_0$ be a point of Z; put $x_0=p(z_0)$ and $y_0=f(x_0)$. The mapping $s$ given by $x\mapsto \tau (z_0, x)$ is a section of $p$ over $\overset{-1}{f}(y_0)$.

The set $\overset{-1}{f}(y_0)$ is compact (TG, I, p. 75, Theorem 1 and I, p. 26, Remark 2), and two distinct points of $\overset{-1}{f}(y_0)$ have disjoint neighbourhoods in X, since $f$ is separated (I, p. 25, Proposition 1). By Theorem 2 of I, p. 37, there therefore exists a neighbourhood $U_0$ of $\overset{-1}{f}(y_0)$ in X and a section $s_0$ of $p$ over $U_0$ extending $s$. The set $s_0(U_0)$ is an open set of Z, since $p$ is étale (I, p. 30, Corollary 3), and contains the saturated set of $\{z_0\}$ for the relation $R_{\tau}$. The mapping $g$ is closed (IV, p. 386, Proposition 2). There then exists an open set V of $Z/R_{\tau}$ such that $W =\overset{-1}{g}(V)\cap \overset{-1}{p}(U_0)$ is a neighbourhood of $z_0$ contained in $s_0(U_0)$ (I, p. 75, Lemma).

Let now $(x, u)\in U_0\times_YV$, and let $z$ be the unique point of Z such that $h(z) = (x, u)$; by definition, one has $z\in W$. Since $W\subset s_0(U_0)$, one has $z=s_0(p(x))$. This shows that the restriction of $h^{-1}$ to the open set $U_0\times_YV$ of $X\times_Y(Z/R_{\tau})$ is equal to $s_0\circ p\circ$ pr$_1$. Consequently, $h$ is a homeomorphism.

Thus we have shown that the descent datum $\tau$ is effective. The mapping $f$ is universally strict (I, p. 20, corollary). Under the assumption that $f$ is surjective, it then follows from Proposition 8 of I, p. 31 that $q: Z/R_{\tau}\rightarrow Y$ is étale.

### 5. Descent: case of coverings

Let X, Y be topological spaces, and let $f: X\rightarrow Y$ be a surjective continuous mapping. Let $(Z, p)$ be a covering of X, and let $\tau$ be a descent datum relative to $f$ on Z.

If $f$ is proper and separated (resp. if $f$ is open), the descent datum $\tau$ is effective and the Y-space $Z/R_{\tau}$ is an étale space (IV, p. 389, Proposition 5). It is even a covering of Y if $f$ has a continuous section in a neighbourhood of each point (I, p. 72, Proposition 3) or if Z is a locally finite covering of X (I, p. 77, Corollary 4). This number is devoted to bringing out other conditions under which $Z/R_{\tau}$ is a covering of Y.

Let us first prove a lemma.

#### Lemma 1 {#ta-iv-s4-lem-1 .statement tag=022I}

Let B, $B'$ be topological spaces, and let $f: B'\rightarrow B$ be a continuous mapping. If the fibred square $B'\times_BB'$ is locally connected, the topological space $B'$ is locally connected.

Let $a$ be a point of $B'$ and let V be a neighbourhood of $a$. Suppose that the fibre square $B'\times_BB'$ is locally connected and let W be a connected neighbourhood of $(a, a)$ in $B'\times_BB'$ which is contained in $V\times V$. Put U = pr$_1(W)$. The set U is contained in V, and is connected since the image of a connected set under a continuous mapping is connected. If $\Delta_{B'}$ denotes the diagonal of $B'\times_BB'$, the mapping pr$_1|\Delta_{B'}: \Delta_{B'}\rightarrow B'$ is a homeomorphism. Since U contains pr$_1(W\cap \Delta_{B'})$ and $W\cap \Delta_{B'}$ is a neighbourhood of $(a, a)$ in $\Delta_{B'}$, U is a neighbourhood of $a$ in $B'$. This proves the lemma.

#### Proposition 6 {#ta-iv-s4-prop-6 .statement tag=022J}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. Suppose that the mapping $f$ is proper, separated and surjective, and make one of the following assumptions:

(i) The fibres of $f$ are locally connected and the fibre square $B'\times_BB'$ is locally connected.

(ii) The fibres of $f$ are finite, the diagonal $\Delta_{B'}$ of $B'\times_BB'$ is open in $B'\times_BB'$ and $B'\times_BB'-\Delta_{B'}$ is a locally connected space.

Then, if $(E', p')$ is a covering, $(E, p)$ is a covering.

Since the mapping $f$ is universally strict (I, p. 20, corollary), the mapping $p$ is étale (I, p. 31, prop. 8) and separated (I, p. 27, prop. 4). We shall suppose, which is permissible, that $E'= B'\times_BE$.

Let $a$ be a point of B; it is a question of proving that the point $a$ has a neighbourhood W such that the W-space $(E_W, p_W)$ is a covering

which is trivializable. Put $B'_a$ = $\overset{-1}{f}(a)$ and denote by $E'_a$ = $(^-{p'}^1)(E_a)$. The mapping $t_a: E'_a\rightarrow B'_a\times E_a$ defined by $t_a(y) = (p'(y), f'(y))$ is a $B'_a$-isomorphism (I, p. 9, prop. 4), hence $E'_a$ is a trivializable covering of $B'_a$ and $t_a$ is a trivialization of this covering.

Let us prove that there exists a neighbourhood $V'$ of $B'_a$ in $B'$ and a continuous trivialization $t$ of the covering $(E'_{V'}, p_{V'})$ extending $t_a$. Under assumption (ii), $B'_a$ is finite and its points have pairwise disjoint open neighbourhoods over which the covering $E'$ is trivializable, whence the assertion in this case. Under assumption (i), $B'_a$ is locally connected, and so is $B'($IV, p. 390, lemma 1); since the mapping $f$ is proper and separated, $B'_a$ is compact and two distinct points have disjoint neighbourhoods in $B'$, so that the pair $(B',B'_a)$ satisfies property (PCV) ( I, p. 37, lemma 1). The assertion therefore follows from Cor. 2 of I, p. 90.

As $f$ is proper, there exists a neighbourhood V of $a$ in B such that $V'$ contains $\overset{-1}{f}(V)$ (lemma, I, p. 75). We may thus suppose that

$$
V'=\overset{-1}{f}(V)
$$

Let us endow the $V'$-spaces $V'\times E_a$ and $E'_{V'}= V'\times_BE$ with their canonical descent data relative to $f_V: V'\rightarrow V$. We shall now prove that, after shrinking V and $V'$, the isomorphism of $V'$-spaces $t: E'_{V'}\rightarrow$ $V'\times E_a$ which we have just defined is compatible with the descent data, that is to say that one has $t(b'_1, x) =t(b'_2, x)$ if $(b'_1, b'_2)\in V'\times_VV'$ and $x\in E_{f(b'_1)}$. Let $\widetilde{t}$ denote the mapping pr$_2\circ t: E'_{V'}\rightarrow E_a$.

Put $V''= V'\times_VV'$; let us consider it as a $V'$-space by means of the first projection. The mapping $((b'_1, b'_2), x)\mapsto ((b'_1, b'_2),(b'_1, x))$ of $V''\times_VE$ into $V''\times_{V'}E'$ is an isomorphism of $V''$-spaces; this shows that $V''\times_VE$ is a covering of $V''$.

For $i= 1$, 2, define a mapping $u_i: V''\times_VE\rightarrow V''\times E_a$ by setting $u_i(b'_1, b'_2, x) = (b'_1, b'_2,\widetilde{t}(b'_i, x))$; these are trivializations of the covering $V''\times_VE$. Let $W''$ be the set of points $w\in V''$ over which these trivializations $u_1$ and $u_2$ coincide; it contains $B'_a\times B'_a$, as well as the diagonal $\Delta_{V'}$. Let us prove that $W''$ is a neighbourhood of $B'_a\times B'_a$. Under assumption (i), this follows from Cor. 2 of I, p. 80, since $B'\times B'$ is locally connected. Under assumption (ii), $W''$ contains a neighbourhood of $(B'_a\times B'_a)-\Delta_{B'_a}$ in $(B'\times_BB')-\Delta_{B'}$, for this set is locally connected (loc. cit.). As $\Delta_{V'}$ is open in $B'\times_BB',W''$ is a neighbourhood of $B'_a\times B'_a$ in $V''$.

As $f$ is proper, the canonical mapping $f''$ of $B'\times_BB'$ into B is proper, for it is the composite of the projection pr$_1: B'\times_BB'\rightarrow B'$ and the mapping $f$.

By the lemma of I, p. 75, there exists a neighbourhood W of $a$ in V

such that $(f\overset{-1}{''})(W)$ is contained in $W''$; let us put $W'=(\overset{-1}{f}')(W)$; it is a subset of $V'$ and the isomorphism of étale spaces $t: E'_{W'}\rightarrow W'\times E_a$ is compatible with the canonical descent data relative to the mapping $f_W: W'\rightarrow W$. It follows from corollary (IV, p. 388) that the W-étale spaces $E_W$ and $W\times E_a$ are isomorphic. In particular, $E_W$ is a trivializable covering, whence the proposition.

#### Corollary 1 {#ta-iv-s4-prop-6-cor-1 .statement tag=022K}

Let E and B be topological spaces, $p: E\rightarrow B$ a continuous mapping and $(A_i)_{i\in I}$ a locally finite closed covering of B such that for every pair $(i, j)\in I\times I,i=\not j$, the intersection $A_i\cap A_j$ is a locally connected space. Then, in order that the B-space $(E, p)$ be a covering, it is necessary and sufficient that, for every $i\in I$, the $A_i$-space $(\overset{-1}{p}(A_i), p_{A_i})$ be a covering of $A_i$.

The condition is necessary (cf. I, p. 69). Conversely, let $B'$ denote the topological sum of the family $(A_i)_{i\in I}$ and $f: B'\rightarrow B$ the canonical mapping. The mapping $f$ is closed (TG, I, p. 6, prop. 4), separated (I, p. 27, remark 5), with finite fibres, hence proper (TG, I, p. 75, th. 1); it is also surjective. The diagonal $\Delta_{B'}$, being equal to $\bigcup_{i\in I}A_i\times_BA_i$, is open in $B'\times_BB'$. Finally, the space $(B'\times_BB')-\Delta_{B'}$ is homeomorphic to the topological sum of the family $(A_i\cap A_j)$, $(i, j)\in I\times I$, $i=\not j$; it is therefore locally connected. Hypothesis (ii) of proposition 6 is satisfied. If for every $i,\overset{-1}{p}(A_i)$ is a covering of $A_i,E'$ is then a covering of $B'$, hence E is a covering of B.

#### Corollary 2 {#ta-iv-s4-prop-6-cor-2 .statement tag=022L}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a proper, separated and surjective mapping. Assume in addition one of the following hypotheses:

(i) The fibres of $f$, as well as the space $X\times_YX$, are locally connected;

(ii) The fibres of $f$ are finite, the diagonal $\Delta_X$ of $X\times_YX$ is open in $X\times_YX$ and the space $(X\times_YX)-\Delta_X$ is locally connected. Then every descent datum relative to $f$ on a covering of X is effective, and the quotient space is a covering of Y.

Let Z be a covering of X and let $\tau$ be a descent datum relative to $f$ on Z. By proposition 5 (IV, p. 389), the descent datum $\tau$ is effective, in other words the square

Z $Z/R_{\tau}$

X $^f$ Y

is a cartesian square. The hypotheses of proposition 6 (IV, p. 391) are then satisfied. Consequently, $Z/R_{\tau}$ is a covering of Y.

#### Proposition 7 {#ta-iv-s4-prop-7 .statement tag=022M}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous and surjective mapping. Suppose that the space Y is unloopable and that the mapping $f$ is open and has the path-lifting property. Then every descent datum relative to $f$ on a covering of X is effective, and the quotient space is a covering of Y.

Let $(Z, p)$ be a covering of X and let $\tau$ be a descent datum relative to $f$ on Z. Since the mapping $f$ is surjective and open, it follows from prop. 5 of IV, p. 389, that the descent datum $\tau$ is effective. Let $T = Y/R_{\tau}$; it is the quotient Y-space; its projection $q$ is étale (loc. cit.); it is also separated (I, p. 27, prop. 4).

By hypothesis, the mapping $f$ has the path-lifting property, and so does the mapping $p$, since Z is a covering of X (III, p. 302, Corollary 2 of Prop. 3). Hence the same is true of the mapping $p\circ f$, and therefore of the mapping $q$. Consequently (cf. IV, p. 341, Remark 2), T is a covering of Y. The proposition is thus proved.

#### Remark {#ta-iv-s4-n5-rem-1 .statement tag=022N}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a mapping. In order that every descent datum relative to $f$ on a covering of X be effective, and that the quotient space be a covering of Y, it is necessary that $f$ be strict and that $f(X)$ be an open and closed subset of X.

In fact, let us identify the X-space X with $X\times_YY$ and endow it with its canonical descent datum relative to $f$. The quotient space is identified with $f(X)$, endowed with the quotient topology of the topology of X for the equivalence relation defined by $f$. If this is a covering of Y, the space $f(X)$ is then identified with an open and closed subset of Y and the mapping $f$ is strict.

### 6. Descent of groupoids

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. Let $p_1$ and $p_2$ denote the two projections of $X\times_YX$ into X, Coeg($f$) the coequalizer groupoid of the pair $(\varpi (p_1), \varpi (p_2))$ of groupoid morphisms from $\varpi (X\times_YX)$ into $\varpi (X)$, and $\gamma :\varpi (X)\rightarrow$ Coeg($f$) the canonical groupoid morphism (II, p. 199, Def. 2). Since $f\circ p_1=f\circ p_2$, we have $\varpi (f)\circ \varpi (p_1) =\varpi (f)\circ \varpi (p_2)$. It then follows from the universal property of coequalizers (II, p. 199, Prop. 3) that there exists a unique groupoid morphism $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ such that $\varpi (f) =\varpi '(f)\circ \gamma$.

The set of vertices of Coeg($f$) is the quotient set of the set X = Som($\varpi (X)$) by the equivalence relation defined by $f($II, p. 200, Remark 1). It is identified with $f(X)$.

#### Proposition 8 {#ta-iv-s4-prop-8 .statement tag=022O}

Let X and Y be non-empty topological spaces and let $f$ be a continuous mapping of X into Y. Assume that the space X is locally arcwise connected, that the space Y is connected, and that the mapping $f$ is strict and surjective. Then the groupoid Coeg($f$) is transitive.

Let Γ be the quiver whose set of vertices is X and whose set of arrows is the sum set of Fl($\varpi (X)$) and $X\times_YX$, the origin and target mappings being those of $\varpi (X)$ on Fl($\varpi (X)$) and the mappings $p_1$ and $p_2$ on $X\times_YX$. By the definition of the framework of the pair $(\varpi$(pr$_1$)$, \varpi$(pr$_2$)) (II, p. 185, Def. 3) and Remark 2 of II, p. 200, the set of orbits of Coeg($f$) is identified with the set of connected components of the quiver Γ. Since the space X is non-empty, it is enough to prove that the graph Γ is connected.

The connected components of Γ are saturated with respect to the equivalence relation “there exists a path joining $x$ to $x'$”, and therefore are open in X, since X is locally arcwise connected. They are then also closed. They are also saturated with respect to the equivalence relation R defined by $f$. By hypothesis, the mapping $f$ induces a homeomorphism of $X/R$ onto Y, so that the image under $f$ of every connected component of Γ is an open and closed subset of Y, and therefore is equal to Y since the space Y is assumed connected.

Let C be a connected component of Γ, and let $x$ be a point of X. From the preceding, there exists a point $x'\in C$ such that $f(x') =f(x)$. By definition of the quiver Γ, we have $x'\in C$. Thus C = X and the quiver Γ is therefore connected.

#### Proposition 9 {#ta-iv-s4-prop-9 .statement tag=022P}

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Suppose that the space X is locally arcwise connected, that the space Y is simply connected, and that the mapping $f$ is strict and surjective. Then the groupoid $\varpi (Y)$ is generated by the image of $\varpi (X)$ under $\varpi (f)$.

We may suppose that the spaces X and Y are non-empty. Let G denote the subgroupoid of $\varpi (Y)$ generated by the image of $\varpi (X)$ under $\varpi (f)$. Since the mapping $f$ is surjective, the set of vertices of G is equal to Y. By prop. 8, Coeg($f$) is a transitive groupoid. Since $\varpi '(f)$ induces the identity on the vertices, the image of Coeg($f$) under $\varpi '(f)$ is a transitive subgroupoid of $\varpi (Y)$. The image of $\varpi (X)$ under $\gamma$ generates Coeg($f$) (II, p. 200, corollary); since one has $\varpi (f) =$ $\varpi '(f)\circ \gamma$, the groupoid G is transitive.

Let $y_0$ be a point of Y and let H denote the subgroup $G_{y_0}$ of $\pi_1(Y, y_0)$. By Th. 1 of IV, p. 342, there exists a connected covering $(T, p)$ of Y and a point $t_0$ of the fibre $T_{y_0}$ of which H is the stabilizer.

If $x$ is a point of X, the set Fl$_{y_0,f(x)}(G)$ is not empty, since G is transitive. For $u\in$ Fl$_{y_0,f(x)}(G)$, the point $t_0\cdot u$ is a point of the fibre $T_{f(x)}$, independent of $u$ since the group H, the isotropy group of G at $y_0$, fixes $t_0$. Let us denote this point by $\sigma (x)$; let $\sigma : X\rightarrow T$ denote the resulting mapping and $s: X\rightarrow X\times_YT$ the mapping $x\mapsto (x, \sigma (x))$. By construction, the mapping $s$ is compatible with the canonical operations of $\varpi (X)$ in X and $X\times_YT$. It then follows from lemma 1 of III, p. 312 that $s$ is continuous. The mapping $\sigma$ is therefore continuous; moreover it is compatible with the equivalence relation defined by $f$, for $\sigma (x)$ depends only on $f(x)$. Since $f$ is strict and surjective, there exists a unique continuous mapping $\overline{\sigma}: Y\rightarrow T$ such that $\overline{\sigma}\circ f=\sigma$, so that the covering T admits a section. Since T is connected, the mapping $p: T\rightarrow Y$ is a homeomorphism (I, p. 31, cor. 4 of prop. 6), and one has $H =\pi_1(Y, y_0)$, whence $G_{y_0}=\pi_1(Y, y_0)$. Since G is transitive, it follows that $G =\varpi (Y)$.

#### Proposition 10 {#ta-iv-s4-prop-10 .statement tag=022Q}

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Suppose that the space X is simply connected, that the space $X\times_YX$ is locally arcwise connected, and that every descent datum relative to $f$ on a covering of X is effective and the quotient space is a covering of Y. Then the groupoid morphism $\varpi '(f)$ of Coeg($f$) into $\varpi (Y)$ is injective.

Under the hypotheses of the proposition, $f$ is strict ( IV, p. 394, remark); moreover, one may suppose that it is surjective.

#### Lemma 2 {#ta-iv-s4-lem-2 .statement tag=022R}

Let us retain the notation and hypotheses of the proposition. Let T be a set endowed with an operation of the groupoid Coeg($f$) relative to a mapping $q: T\rightarrow Y$. Then there exists a unique topology on T for which $q$ makes T a covering of Y, such that for every class of paths with origin $c$ in X and every point $t$ of T, one has $t\cdot \gamma (c) =t\cdot f_*(c)$. In particular, the operation of Coeg($f$) on T factors through an operation of the groupoid $\varpi (Y)$.

The uniqueness of such a topology on T follows from Lemma 1 (III, p. 312); let us prove its existence. Endow the set $X\times_YT$ with a law of operation of $\varpi (X)$ by putting $(x, t)\cdot u= (x\cdot u, t\cdot \gamma (u))$ for every $(x, t)\in X\times_YT$ and every arrow $u$ with origin $x$ in $\varpi (X)$. Since the space X is simply connected, this law of operation of $\varpi (X)$ is without local monodromy (III, p. 313, Remark). There therefore exists on the set $X\times_YT$ a unique topology which makes the X-space $(X\times_YT$, pr$_1)$ a covering of X and such that the canonical operation of $\varpi (X)$ in this covering coincides with the given operation (III, p. 313, Prop. 3). Let us denote this covering by $(Z, p)$. Let us prove that the mapping $\tau : ((x_1, t), x_2)\mapsto (x_2, t)$ of $Z\times_YX$ into Z is a descent datum on Z relative to the mapping $f$. It is enough to verify that it is continuous, the other conditions of Definition 1 of IV, p. 382, being evident.

The mapping $\tau$ is a lifting of the mapping pr$_2: Z\times_YX\rightarrow X$ to the covering Z of X. Since the space $X\times_YX$ is locally arcwise connected, the space $Z\times_YX$, which is a covering of it, is also locally arcwise connected. By the Corollary (III, p. 269), in order to prove that the mapping $\tau$ is continuous, it is enough to prove that it is arcwise continuous.

Let therefore $\widetilde{c}= ((c, g), c')$ be a path in $Z\times_YX$ and let us prove that the mapping $\tau \circ \widetilde{c}:t\mapsto (c'(t), g(t))$ of $\mathbf{I}$ into Z is continuous. For every $s\in [0,1]$, let us denote by $c_s$ and $c'_s$ the paths in X defined by $t\mapsto c(st)$ and $t\mapsto c'(st)$. For every $s\in [0,1]$, one thus has $c(s) =c(0)\cdot [c_s]$, $c'(s) =c'(0)\cdot [c'_s]$ and $(c, g)(s) = (c(0), g(0))\cdot [c_s]$, where $[u]$ denotes the strict homotopy class of a path $u($III, p. 304, Remark). The mapping $t\mapsto (c_s(t), c'_s(t))$ is a path in $X\times_YX$; by definition of the coequalizer Coeg($f$), one therefore has $\gamma ([c_s]) =\gamma ([c'_s])$ and $g(s) =g(0)\cdot \gamma ([c_s]) =$ $g(0)\cdot \gamma ([c'_s])$. By definition of the operation of $\varpi (X)$ on Z, one therefore has

$$
(\tau \circ \widetilde{c})(s) = (c'(s), g(s)) = (c'(0)\cdot [c'_s], g(0)\cdot \gamma ([c'_s]))
$$

$$
= (c'(0), g(0))\cdot [c'_s] = (\tau \circ \widetilde{c})(0)\cdot [c'_s]
$$

This shows that $\tau \circ \widetilde{c}$ is a continuous lifting to Z of the path $c'($loc. cit.). Consequently, the mapping $\tau$ is arcwise continuous, hence continuous; it is a descent datum relative to $f$ on the X-space Z.

Let $R_{\tau}$ denote the equivalence relation defined by the descent datum $\tau$. Since the mapping $f$ is surjective, the mapping pr$_2: Z\rightarrow T$ induces, by passing to the quotient, a bijection of $Z/R_{\tau}$ onto T. Let us endow T with the topology deduced from that of $Z/R_{\tau}$ by transport of structure, so that $(T, q)$ is a Y-space. By hypothesis, T is therefore a covering of Y and the diagram

Z $^{pr_2}$ T

$pq$

X $^f$ Y

is a cartesian square.

Let $(x, t)$ be a point of Z, $c$ a path with origin $x$ in X, and let $\widetilde{c}$ be the continuous lifting of $c$ to Z with origin $(x, t)$. The path pr$_2\circ \widetilde{c}$ is the lifting with origin $t$ of the path $f\circ c$ in Y, so that $t\cdot \gamma ([c]) =$ $t\cdot [f\circ c] =t\cdot f_*([c])$. This completes the proof of the lemma.

Let us now prove the proposition. Let $u$ and $v$ be two arrows of Coeg($f$) whose images in $\varpi (Y)$ are equal. Since the groupoid morphism $\varpi '(f)$ is the identity on the vertex sets, the arrows $u$ and $v$ have the same origin and the same target. Let us denote by $y$ the origin of $u$; let T be the set of arrows of Coeg($f$) with origin $y$, and let $q: T\rightarrow Y$ be the restriction to T of the target mapping. The groupoid Coeg($f$) operates by composition on the right on the set T, relative to $q$. By lemma 2, the actions of $u$ and $v$ on T are identical. Hence $u=$ $e_y\cdot u=e_y\cdot v=v$. This proves that the groupoid morphism $\varpi '(f)$ is injective.

#### Theorem 1 {#ta-iv-s4-thm-1 .statement tag=022S}

Let X and Y be topological spaces, and let $f: X\rightarrow$ Y be a continuous surjective mapping. Suppose that the spaces X and Y are locally path-connected and semi-locally simply connected. Finally, suppose that one of the following properties is satisfied:

(i) The mapping $f$ is proper, separated, with locally connected fibres, and the space $X\times_YX$ is locally path-connected;

(ii) The mapping $f$ is proper, separated, with finite fibres, the diagonal $\Delta_X$ is open in $X\times_YX$, and its complement is locally connected;

(iii) The mapping $f$ is open and has the path-lifting property. Then the groupoid morphism $\varpi '(f)$ is an isomorphism of the groupoid Coeg($f$) onto the Poincaré groupoid $\varpi (Y)$.

First let us note that under these hypotheses, the mapping $f$ is surjective and strict (I, p. 18, example 2). Moreover, every descent datum relative to $f$ on a covering of X is effective, and the quotient space is a covering of Y; this follows indeed from IV, p. 393, corollary 2 of prop. 4 under hypotheses (i) and (ii), and from prop. 7 of IV, p. 394 under hypothesis (iii). By prop. 10, the groupoid morphism $\varpi '(f)$ is therefore injective and its image is a subgroupoid of $\varpi (Y)$.

By prop. 9 of IV, p. 395, this image is equal to $\varpi (Y)$ under hypotheses (i) and (ii), but also under hypothesis (iii), since the groupoid morphism $\varpi (f)$ is then surjective.

Consequently, $\varpi '(f)$ is an isomorphism.

#### Example {#ta-iv-s4-n6-exa-1 .statement tag=022T}

Here are two examples in which the hypotheses of theorem 1 are satisfied.

1) Let Y be an unlaceable topological space. Let $(A_i)_{i\in I}$ be a locally finite covering of Y by closed sets. Suppose that, for every $i\in I$, the space $A_i$ is unlaceable and that, for every pair $(i, j)\in I\times I$, the space $A_i\cap A_j$ is locally path-connected. One may take for X the sum space of the family $(A_i)_{i\in I}$ and for $f: X\rightarrow Y$ the mapping deduced from the family of canonical injections.

2) Let G be a discrete group operating properly in an unlaceable topological space X, put $Y = X/G$ and let $f: X\rightarrow Y$ be the canonical mapping. It is open (TG, III, p. 10, lemma 2) and has the path-lifting property by virtue of Theorem 4 of III, p. 287. The space Y is unlaceable by IV, p. 349, Prop. 8, b). By hypothesis, the mapping from $G\times X$ into $X\times X$ given by $(g, x)\mapsto (g\cdot x, x)$ is proper, hence strict (I, p. 18, Example 2) and its image is $X\times_YX$. It then follows from III, p. 261, Prop. 8 that $X\times_YX$ is locally path-connected.

### 7. Descent by an étale and surjective mapping

Let X and Y be topological spaces and let $f$ be a continuous mapping from X into Y. We retain the notation of the preceding No.

#### Theorem 2 {#ta-iv-s4-thm-2 .statement tag=022U}

Suppose that every point of Y possesses a neighbourhood above which there exists a continuous section of the mapping $f$. The groupoid morphism $\varpi '(f)$ from Coeg($f$) into $\varpi (Y)$ is an isomorphism.

By hypothesis, there exists a covering $(U_j)_{j\in J}$ of Y by open sets and, for every $j\in J$, a continuous section $s_j$ of $f_{U_j}$.

If $c$ is a path in X, we denote by $[c]$ its strict homotopy class in $\varpi (X)$ and by $\{c\}$ the image of $[c]$ in Coeg($f$) by the groupoid morphism $\varpi '(f)$. If $c$ and $c'$ are two paths in X$,\{c\}$ and $\{c'\}$ are composable in Coeg($f$) if and only if the paths $f\circ c$ and $f\circ c'$ in Y are juxtaposed.

Let $c'$ be a path in Y. By Lemma 4 of III, p. 272, applied

to the compact space $\mathbf{I}$ and to the covering ($(^-{c'}^1)(U_j)$)$_{j\in J}$ of $\mathbf{I}$, there exists an integer $n$ such that, for every integer $k$ satisfying $1\leqslant k\leqslant n$, the image of the interval $[\frac{k-1}{n},\frac{k}{n}]$ by $c'$ is contained in an open set $U_{j(k)}$. For every integer $k,1\leqslant k\leqslant n$, let $c'_k$ be the path in Y defined by $s\mapsto c'(\frac{k+s-1}{n})$; one has $[c'] = [c'_1][c'_2]. . .[c'_n]$ (cf. III, p. 291, remark 1), and $c'$ is the path denoted by $c'_1*c'_2* \cdots  *c'_n$. For every $k\in  \{1, . . . , n\}$, let us denote by $c_k$ the path $s_{j(k)}\circ c'_k$ in X and put $\{c_k\}=\gamma ([c_k])$. Since for every $k$, the paths $c'_{k-1}=f\circ c_{k-1}$ and $c'_k=f\circ c_k$ can be juxtaposed, the sequence $(\{c_1\}, . . . ,\{c_n\})$ is composable in Coeg($f$). By construction,

$$
\varpi '(f)(\{c_1\}. . .\{c_n\}) =\varpi '(f)(\{c_1\}). . . \varpi '(f)(\{c_n\})
$$

$$
=\varpi (f)([c_1]). . . \varpi (f)([c_n])
$$

$$
= [f\circ c_1]. . .[f\circ c_n]
$$

$$
= [c'_1]* \cdots  *[c'_n] = [c']
$$

which proves that the groupoid morphism $\varpi '(f)$ is surjective.

Let $u$ and $v$ be arrows of Coeg($f$). Since the groupoid Coeg($f$) is generated by the image of $\varpi (X)$ (II, p. 200, corollary), there exist finite sequences $(c_1, . . . , c_n)$ and $(d_1, . . . , d_n)$ of paths in X such that one has $u=\{c_1\}. . .\{c_n\}$ and $v=\{d_1\}. . .\{d_n\}$. The paths $(f\circ c_1, . . . , f\circ c_n)$ in Y can then be juxtaposed and one has $\varpi '(f)(u) = [(f\circ c_1)]. . .[(f\circ$ $c_n)]$; analogously, $\varpi '(f)(v) = [(f\circ d_1)]. . .[(f\circ d_n)]$.

Suppose that one has $\varpi '(f)(u) =\varpi '(f)(v)$. There then exists a strict homotopy $\sigma$ joining $(f\circ c_1)* \cdots  *(f\circ c_n)$ to $(f\circ d_1)* \cdots  *(f\circ d_n)$. By lemma 4 of III, p. 272, applied to the compact space $\mathbf{I}\times \mathbf{I}$ and to the covering $(\overset{-1}{\sigma}(U_i))_{i\in I})$ of $\mathbf{I}\times \mathbf{I}$, there exists an integer $m\geqslant 1$ such that, for every pair of integers $(j, k)$ satisfying $1\leqslant j\leqslant m$ and $1\leqslant k\leqslant m$, the image of $[\frac{j-1}{m},\frac{j}{m}]\times [\frac{k-1}{m},\frac{k}{m}]$ by $\sigma$ is contained in an open set $U_{i(j,k)}$ of the covering $(U_i)_{i\in I}$.

Every path $c$ in X is of the form $c_1* \cdots  *c_m$, where $c_k$ is the path $t\mapsto c(\frac{k-1+t}{m})$. Replacing the integers $m$ and $n$ by their product $mn$ if necessary, one may therefore suppose that $m=n$.

For every pair $(j, k)$ of integers of $\{1, . . . , n\}$ and every pair $(s, t)\in$ $\mathbf{I}\times \mathbf{I}$, set

$$
\sigma_{j,k}(s, t) =s_{i(j,k)}\circ \sigma (\frac{s + j- 1}{n},\frac{t + k- 1}{n})
$$

For $t\in \mathbf{I}$, also set $h^0_{j,k}(t) =\sigma_{j,k}(t,0)$, $h^1_{j,k}(t) =\sigma_{j,k}(t,1)$, $v^0_{j,k}(t) =\sigma_{j,k}(0, t)$ and $v_{j,k}^1(t) =\sigma_{j,k}(1, t)$. By lemma 1 of III, p. 295, the paths $h^0_{j,k}*v_{j,k}^1$ and $v_{j,k}^0*h^1_{j,k}$ are strictly homotopic, whence the relation

$$
[h^0_{j,k}][v_{j,k}^1] = [v_{j,k}^0][h^1_{j,k}] \tag{2}
$$

in $\varpi (X)$, for every pair $(j, k)\in  \{1, . . . , n\}^2$. On the other hand, for every pair of integers $(j, k)$, with 2 $\leqslant j\leqslant n$ and 1 $\leqslant k\leqslant n$, one has $f\circ v_{j,k}^0=f\circ v_{j-1,k}^1$, whence the relation

$$
\{v^0_{j,k}\}=\{v_{j-1,k}^1\} \tag{3}
$$

in Coeg($f$). Analogously, for every pair of integers $(j, k)$ such that $1\leqslant j\leqslant n$ and $2\leqslant k\leqslant n$, one has

$$
\{h^0_{j,k}\}=\{h^1_{j,k-1}\} \tag{4}
$$

For $j\in  \{1, . . . , n\}$, the paths $f\circ c_j$ and $f\circ h^0_{j,1}$ coincide. By definition of the coequalizer Coeg($f$), one therefore has $\{c_j\}=\{h^0_{j,1}\}$. Analogously, for every $j\in  \{1, . . . , n\},\{d_j\}=\{h^1_{j,n}\}$. Hence one has the relations

$$
u=\{h^0_{1,1}\}. . .\{h^0_{n,1}\},v=\{h^1_{1,n}\}. . .\{h^1_{n,n}\}
$$

By lemma 3 below, one has

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}\{v_{1,n}^1\}. . .\{v^1_{n,n}\}=\{v_{1,1}^0\}. . .\{v_{n,1}^0\}\{h^1_{n,1}\}. . .\{h^1_{n,n}\}
$$

Since the paths $t\mapsto \sigma (0, t)$ and $t\mapsto \sigma (1, t)$ are constant, one has, for $1\leqslant k\leqslant n,\{v^0_{1,k}\}=e_a$ and $\{v^1_{n,k}\}=e_b$ where $a$ and $b\in Y$ are the origin and the end of the arrows $u$ and $v$ of Coeg($f$). It follows that

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}=\{h^0_{n,1}\}. . .\{h^1_{n,n}\}
$$

that is, $u=v$.

#### Lemma 3 {#ta-iv-s4-lem-3 .statement tag=022V}

Let G be a groupoid and let $p, q$ be integers $\geqslant 1$. For every pair $(j, k)$ of integers such that $0\leqslant j\leqslant p$ and $0\leqslant k\leqslant q$, let $x_{j,k}$ be a vertex of G; for every pair $(j, k)$ such that $1\leqslant j\leqslant p$ and $0\leqslant k\leqslant q$, let $h_{j,k}$ be an arrow of G joining $x_{j-1,k}$ to $x_{j,k}$; for every pair $(j, k)$ such that $0\leqslant j\leqslant p$ and $1\leqslant k\leqslant q$, let $v_{j,k}$ be an arrow of G joining $x_{j,k-1}$ to $x_{j,k}$.

Assume that, for every pair $(j, k)$ of integers such that $1\leqslant j\leqslant p$ and $1\leqslant k\leqslant q$, the arrows $v_{j-1,k}$ and $h_{j,k}$ are composable, analogously the arrows $h_{j,k-1}$ and $v_{j,k}$, and that one has $v_{j-1,k}h_{j,k}=h_{j,k-1}v_{j,k}$. Then,

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q}h_{1,q}h_{2,q}. . . h_{p,q}
$$

Let us first treat the particular case where $q= 1$ and prove the result by induction on $p$. If $p= 1$, the assertion to be proved is true by assumption; suppose it true for $p-1$; one then has

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}=h_{1,0}h_{2,0}. . . h_{p-1,0}v_{p-1,1}h_{p,1}=v_{0,1}h_{1,1}. . . h_{p,1}
$$

by the induction hypothesis, whence the relation for $p$.

Let us now prove the result by induction on $q$. It is true for $q= 1$ by what precedes; if it is true for $q-1$, one then has

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q-1}h_{1,q-1}. . . h_{p,q-1}v_{p,q}
$$

From the case $q= 1$, one has

$$
h_{1,q-1}. . . h_{p,q-1}v_{p,q}=v_{0,q}h_{1,q}. . . h_{p,q}
$$

whence the required relation.

#### Example 1 {#ta-iv-s4-n7-exa-1 .statement tag=022W}

The theorem applies when the mapping $f$ is étale and surjective.

#### Example 2 {#ta-iv-s4-n7-exa-2 .statement tag=022X}

It also applies when the space X is the sum space of a family $(V_i)_{i\in I}$ of parts of Y whose interiors cover Y, and when $f$ is the mapping induced by the canonical injections of each of the $V_i$ into Y.

### 8. Poincaré Groupoid of a Quotient Space

Let X be a topological space endowed with a continuous action of a discrete group G; set $Y = X/G$ and denote by $f: X\rightarrow$ Y the canonical mapping. Let $|G|$ denote the groupoid $\varpi (G)$; its set of vertices is G; for $g, g'\in G$, there exists a unique arrow joining $g$ to $g'$ if $g'=g'$, and none otherwise. By passing to the fundamental groupoids, the action $m: G\times X\rightarrow X$ induces a morphism of groupoids $\varpi (m):|G| \times \varpi (X)\rightarrow \varpi (X)$. Let $\varpi (X)/G$ be the coequalizer of the two morphisms of groupoids $\varpi (m)$ and $\varpi$(pr$_2$) from $|G| \times \varpi (X)$ to $\varpi (X)$; let $\beta :\varpi (X)\rightarrow \varpi (X)/G$ denote the canonical morphism of groupoids. We have $f\circ m=f\circ$ pr$_2$, hence $\varpi (f)\circ \varpi (m) =\varpi (f)\circ \varpi$(pr$_2$). By the universal property of coequalizers, there therefore exists a unique morphism of groupoids $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)$ such that $\varpi (f) =\varpi ''(f)\circ \beta$.

#### Theorem 3 {#ta-iv-s4-thm-3 .statement tag=022Y}

Let X be a delaceable topological space and let G be a discrete group operating properly in X; let $f: X\rightarrow X/G$ be the canonical surjection. The canonical morphism of groupoids $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (X/G)$ introduced above is an isomorphism.

Let Coeg($f$) denote the coequalizer of the two morphisms of groupoids from $\varpi (X\times_YX)$ to $\varpi (X)$ induced by the projections pr$_1$ and pr$_2$; let $\gamma :\varpi (X)\rightarrow$ Coeg($f$) be the canonical morphism of groupoids. Since the image of the mapping $(m$, pr$_2): G\times X\rightarrow X\times X$ is the subspace $X\times_YX$ of $X\times X$, the two morphisms of groupoids $\gamma \circ \varpi (m)$ and $\gamma \circ \varpi$(pr$_2$), from $|G|\times \varpi (X)$ to Coeg($f$), are equal. By the universal property of $\varpi (X)/G$, there exists a unique morphism of groupoids $\alpha :\varpi (X)/G\rightarrow$ Coeg($f$) such that $\gamma =\alpha \circ \beta$.

Let also $\varpi '(f)$ denote the unique morphism of groupoids from Coeg($f$) to $\varpi (Y)$ such that $\varpi (f) =\varpi '(f)\circ \gamma$. By IV, p. 399, Example 2, the hypotheses of Theorem 1 of IV, p. 398 are satisfied and the morphism $\varpi '(f)$ is an isomorphism. Since

$$
\varpi (f) =\varpi '(f)\circ \gamma =\varpi '(f)\circ \alpha \circ \beta =\varpi ''(f)\circ \beta
$$

we have $\varpi ''(f) =\varpi '(f)\circ \alpha$. Thus, to prove Theorem 3, it is enough to prove that the morphism $\alpha$ is an isomorphism.

#### Lemma 4 {#ta-iv-s4-lem-4 .statement tag=022Z}

For every path $c= (c_1, c_2)$ in $X\times_YX$, we have $\beta ([c_1]) =\beta ([c_2])$.

Let $c$ be such a path.

Let $x\in X$, and let $K_x$ be its stabilizer in G. By TG, III, p. 32, prop. 8, there exists an open neighbourhood $U_x$ of $x$ in X such that $K_x\cdot U_x=$ $U_x,g\cdot U_x\cap U_x$ = $\emptyset$ for every $g\in$ G - $K_x$, and such that the mapping $f$ induces a homeomorphism of $U_x/K_x$ onto an open neighbourhood $V_x$ of $f(x)$ in Y. As X is unlaceable and the restriction of the mapping $f$ to $U_x$ is open and closed, we may further suppose that $U_x$ is connected and that the image of the canonical homomorphism $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ is reduced to the identity element. The open sets $(V_x)_{x\in X}$ thus constructed form an open covering of Y. By lemma 4 of III, p. 272, applied to the compact space $\mathbf{I}$ and to the open sets $(f\circ c_1)^{-1}(V_x)$ for $x\in X$, there exists an integer $n\geqslant 1$ such that for every $i\in  \{1, . . . , n\}$, there exists a point $x_i$ in X such that $c_1([\frac{i-1}{n},\frac{i}{n}])$

is contained in $\overset{-1}{f}(V_{x_i})$. As $f\circ c_1=f\circ c_2,c_2([\frac{i-1}{n},\frac{i}{n}])$ is also

contained in $\overset{-1}{f}(V_{x_i})$.

For $j= 1$ or 2 and for $i\in  \{1, . . . , n\}$, let $c_{j,i}$ denote the path in X defined by $t\mapsto c_j(\frac{i+t-1}{n})$; we have $c_j=c_{j,1}* \cdots  *c_{j,n}($III, p. 291, remark 1). Hence, to prove that $\beta ([c_1]) =\beta ([c_2])$, it is enough to prove that $\beta ([c_{1,i}]) =\beta ([c_{2,i}])$ for every integer $i\in  \{1, . . . , n\}$. Replacing the pair of paths $(c_1, c_2)$ by the pair $(c_{1,i}, c_{2,i})$ if necessary, we thus suppose that there exists $x\in X$ such that $(f\circ c_1)([0,1])\subset V_x$.

The inverse image of $V_x$ by $f$ is the disjoint union of the connected components $g\cdot U_x$, where $g$ runs through a system of representatives in G of $G/K_x$. For $i= 1$ or 2, let $g_i$ be an element of G such that the point $x_i=$ $g_i\cdot c_i(0)$ belongs to $U_x$. The image of the path $g_i\cdot c_i$ is then contained in $U_x$. By definition of the groupoid $\varpi (X)/G$, we have $\beta ([g_i\cdot c_i]) =\beta ([c_i])$, which makes it possible to suppose that the images of the paths $c_1$ and $c_2$ are contained in $U_x$ and that $g_1=g_2=e$.

For $s= 0$ or 1, let $d_s$ be a path in $U_x$ joining $x$ to $c_1(s)$ and let $g_s$ be an element of $K_x$ such that $g_s\cdot c_2(s) =c_1(s)$. The paths $d_0*c_1*\overline{d_1}$ and $d_0*(g_0\cdot c_2)*(g_0g_1^{-1}\cdot \overline{d_1})$ are loops at $x$ in $U_x$. They are therefore strictly homotopic in X to the constant loop at $x$, because the image of the canonical homomorphism $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ reduces to the identity element. Their classes have in particular the same image under the groupoid morphism $\beta$, whence

$$
\beta ([d_0])\beta ([c_1])\beta ([d_1])^{-1}=\beta ([d_0])\beta ([g_0\cdot c_2])\beta ([g_0g_1^{-1}\cdot d_1])^{-1}
$$

Since $\beta ([g\cdot c]) =\beta ([c])$ for every element $g\in G$ and every path $c$ in X, it follows that $\beta ([c_1]) =\beta ([c_2])$, as was to be proved.

By the lemma, the two groupoid morphisms $\beta \circ \varpi$(pr$_1$) and $\beta \circ \varpi$(pr$_2$) of $\varpi (X\times_YX)$ into Coeg($f$) are equal. By the universal property of the coequaliser, there therefore exists a unique groupoid morphism $\alpha ':$ Coeg($f$)$\rightarrow \varpi (X)/G$ such that $\beta =\alpha '\circ \gamma$. The morphism $\alpha '\circ \alpha$ is the unique groupoid morphism $\varphi$ of $\varpi (X)/G$ into itself such that $\varphi \circ \beta =\beta$; hence $\alpha '\circ \alpha$ = Id$_{\varpi(X)/G}$. Analogously, $\alpha \circ \alpha '=$ Id$_{Coeg(f)}$. Consequently, $\alpha$ is an isomorphism.

## EXERCISES {#ta-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
