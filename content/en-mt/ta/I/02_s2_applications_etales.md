---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 2
section_title: Applications étales
lang: en
source: ta-i-iv-fr
book_pages: TA I.25-TA I.42, TA I.140-TA I.141
pdf_pages: 0041-0058, 0156-0157
extraction: native
subsections:
    - "no": 1
      title: Applications séparées
      page: 25
      pdf_page: 41
    - "no": 2
      title: Applications étales
      page: 28
      pdf_page: 44
    - "no": 3
      title: Sections locales des applications étales
      page: 32
      pdf_page: 48
    - "no": 4
      title: Relèvements continus des applications étales
      page: 33
      pdf_page: 49
    - "no": 5
      title: Construction de sections continues d’applications étales
      page: 35
      pdf_page: 51
    - "no": 6
      title: Majoration du cardinal des fibres d’une application étale et séparée
      page: 40
      pdf_page: 56
statements: 47
exercises: 7
content_sha256: 87d728a77058cb1073bd8346d18c7e5ba69f05eb6a61904c13c511f71918bf39
translated_from: content/fr/ta/I/02_s2_applications_etales.md
source_lang: fr
translation_method: machine
source_content_sha256: fdeb72dfbd6bf4e4d9e524bce744200385f12476c65d18d6e4df15e0dab945b5
translation_model: gpt-5.4
translation_run: translate-en-mt-f3f50668
glossary_version: 34
glossary_terms_sha256: e8f2b8a5487dcbaaa8f2acd55ace1df09e5e1ae8f6f226277dd40e490beaf5cb
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. ÉTALE MAPPINGS

### 1. Separated mappings

#### Proposition 1 {#ta-i-s2-prop-1 .statement tag=01MH}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a continuous mapping. The following properties are equivalent:

(i) The diagonal $\Delta_X$ of the fibred product $X\times_YX$ is a closed subspace;

(ii) For every topological space W and every pair of continuous mappings $(g_1, g_2)$ from W into X such that $f\circ g_1=f\circ g_2$, the set of points $w\in W$ such that $g_1(w) =g_2(w)$ is closed in W;

(iii) For every pair $(x_1, x_2)$ of points of X such that $x_1=\not x_2$ and $f(x_1) =f(x_2)$, there exists a neighbourhood $V_1$ of $x_1$ in X and a neighbourhood $V_2$ of $x_2$ in X such that $V_1\cap V_2=\emptyset$.

(i)$\Rightarrow$(ii) : Let $g_1,g_2$ be continuous mappings from W into X such that $f\circ g_1=f\circ g_2$, and let $g: W\rightarrow X\times_YX$ be the mapping deduced from $g_1$ and $g_2$. The set of points $w\in W$ such that $g_1(w) =g_2(w)$ is $\overset{-1}{g}(\Delta_X)$. Since $g$ is continuous, it is therefore closed if the diagonal $\Delta_X$ is closed.

(ii)$\Rightarrow$(i) : The diagonal $\Delta_X$ is the set of points $z\in X\times_YX$ such that pr$_1(z) =$ pr$_2(z)$. It follows from (ii) applied to $W = X\times_YX$ and to the pair of mappings (pr$_1$, pr$_2$) that the diagonal $\Delta_X$ is closed in $X\times_YX$.

(i)$\Leftrightarrow$(iii) : Let $(x_1, x_2)$ be a point of $X\times_YX$ and let $V_1$ and $V_2$ be neighbourhoods of $x_1$ and $x_2$ respectively. The condition $V_1\cap V_2=\emptyset$ is equivalent to the condition $(V_1\times V_2)\cap \Delta_X=\emptyset$, that is, to $(V_1\times V_2)\cap$ $(X\times_YX)\cap \Delta_X=\emptyset$. Since the sets $(V_1\times V_2)\cap (X\times_YX)$ form a basis of neighbourhoods of $(x_1, x_2)$ in $X\times_YX$, this proves the equivalence of (i) and (iii).

#### Definition 1 {#ta-i-s2-def-1 .statement tag=01MI}

Let X and Y be topological spaces. A continuous mapping $f: X\rightarrow Y$ is said to be separated if it satisfies the equivalent conditions of proposition 1.

#### Proposition 2 {#ta-i-s2-prop-2 .statement tag=01MJ}

Let X, Y, Z be topological spaces and let $f: X\rightarrow Y$ and $g: Y\rightarrow Z$ be continuous mappings.

a) If $f$ and $g$ are separated, then $g\circ f$ is separated.

b) If $g\circ f$ is separated, then $f$ is separated.

c) Suppose moreover that the mapping $f$ is proper and surjective. Then, if $g\circ f$ is separated, $g$ is separated.

Consider, in $X\times X$, the subspaces $\Delta_X$ (diagonal), $X\times_YX$ and $X\times_ZX$. These are respectively the sets of points $u$ of $X\times X$ such that pr$_1(u) =$ pr$_2(u),f\circ$pr$_1(u) =f\circ$pr$_2(u),g\circ f\circ$pr$_1(u) =g\circ f\circ$pr$_2(u)$. If $g\circ f$ is separated, $\Delta_X$ is closed in $X\times_ZX$, hence also in $X\times_YX$, whence b).

By prop. 1, (ii), applied to $W = X\times_ZX,g_1=f\circ$ pr$_1$ and $g_2=f\circ$ pr$_2,X\times_YX$ is closed in $X\times_ZX$ if $g$ is separated. If moreover $f$ is separated, $\Delta_X$ is closed in $X\times_YX$ (prop. 1, (i)), hence in $X\times_ZX$, whence a).

Finally, let us prove c). The mapping $(f, f): X\times X\rightarrow Y\times Y$ is proper (TG, I, p. 73, prop. 4). The subspace $X\times_ZX$ is the inverse image of $Y\times_ZY$ by $(f, f)$ ; by TG, I, p. 72, prop. 3, the mapping $u: X\times_Z$ $X\rightarrow Y\times_ZY$ deduced from $(f, f)$ is proper. Since $g\circ f$ is separated, the diagonal $\Delta_X$ is closed in $X\times_ZX$. Consequently, $u(\Delta_X)$ is closed in $Y\times_ZY$. Since $f$ is surjective, $u(\Delta_X)$ is the diagonal of $Y\times_ZY$. This shows that $g$ is separated.

#### Remark 1 {#ta-i-s2-n1-rem-1 .statement tag=01MK}

An injective continuous mapping is separated.

#### Remark 2 {#ta-i-s2-n1-rem-2 .statement tag=01ML}

For a topological space X to be separated (TG, I, p. 52, def. 1), it is necessary and sufficient that the mapping of X into a space reduced to a point be separated. In this case, every continuous mapping of X into a topological space is separated (prop. 1, (iii)).

Let $f: X\rightarrow$ Y be a continuous and separated mapping. For every point $y$ of Y, the fibre $\overset{-1}{f}(y)$ is a separated topological space (loc. cit.). There exist nevertheless continuous mappings which are not separated but all of whose fibres are separated topological spaces (I, p. 140, exerc. 1).

#### Remark 3 {#ta-i-s2-n1-rem-3 .statement tag=01MM}

Let $f: X\rightarrow Y$ be a continuous and separated mapping. If the space Y is separated, the space X is separated. This follows from remark 2 and proposition 2 applied with a space Z reduced to a point.

#### Remark 4 {#ta-i-s2-n1-rem-4 .statement tag=01MN}

Let $f: X\rightarrow Y$ be a continuous and separated mapping, $y$ a point

of Y and A a finite subset of $\overset{-1}{f}(y)$. Let us show that there exists a family $(V_a)_{a\in A}$ of pairwise disjoint sets such that for each $a\in A$, the set $V_a$ is a neighbourhood of $a$ in X. For this, for each subset $\{a, b\}$ of A with two elements, let us choose a neighbourhood $V_{(a,b)}$ of $a$ and a neighbourhood $V_{(b,a)}$ of $b$ in X such that $V_{(a,b)}\cap V_{(b,a)}=\emptyset$ (prop. 1, (iii)). Let $V_a$ denote the intersection of the family consisting of X and the sets $V_{(a,b)}$ for $b\in A,b=\not a$. The set $V_a$ is a neighbourhood of $a$ in X, and if $a,b$ are two distinct elements of A, the set $V_a\cap V_b$ is contained in $V_{(a,b)}\cap V_{(b,a)}$, hence is empty.

#### Remark 5 {#ta-i-s2-n1-rem-5 .statement tag=01MO}

Let Y be a topological space. Let $(A_i)_{i\in I}$ be a family of subsets of Y and let X be the sum space of the family $(A_i)_{i\in I}$. The canonical mapping of X into Y is separated.

#### Proposition 3 {#ta-i-s2-prop-3 .statement tag=01MP}

Let $f: X\rightarrow Y$ be a continuous and separated mapping. Every continuous section of $f$ induces a homeomorphism of Y onto a closed subset of X.

Let $s: Y\rightarrow X$ be a continuous section of $f$. The mapping $s$ induces a homeomorphism of Y onto the subspace $s(Y)$ of X (TG, I, p. 22, prop. 9). The identity mapping of X and the mapping $s\circ f$ are continuous and one has $f\circ$ Id$_X=f\circ (s\circ f)$. Since the mapping $f$ is separated, the set $s(Y)$, which is the set of points $x$ of X such that $x=s\circ f(x)$, is closed in X (prop. 1, (ii)).

#### Proposition 4 {#ta-i-s2-prop-4 .statement tag=01MQ}

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

be a cartesian square. If the mapping $p$ is separated, the same is true of $p'$. Conversely, if $p'$ is separated and if $f$ is universally strict and surjective, then $p$ is separated.

Consider the square

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

$q'q$

${B'}^f$ B

where the mapping $\varphi$ is induced by the mapping $f'\times f': X'\times X'\rightarrow X\times X$. Recall (I, p. 13, example 1) that this square is cartesian and that one has $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$.

If the mapping $p$ is separated, the set $\Delta_X$ is closed in $X\times_BX$; consequently, $\Delta_{X'}$ is a closed subset of $X'\times_{B'}X'$, which proves that the mapping $p'$ is separated.

If the mapping $f$ is surjective, the mapping $\varphi$ is surjective (I, p. 10, cor.) ; if $f$ is universally strict, $\varphi$ is strict (I, p. 20, def. 6). Suppose the mapping $p'$ separated. Then $\Delta_{X'}$ is closed in $X'\times_{B'}X'$. Since $\Delta_{X'}=\overset{-1}{\varphi}(\Delta_X)$ and since $\varphi$ is surjective and strict, $\Delta_X$ is closed in $X\times_BX$, which proves that the mapping $p$ is separated.

#### Proposition 5 {#ta-i-s2-prop-5 .statement tag=01MR}

Let X, Y, Z be topological spaces and let $f: X\rightarrow Y,g: Y\rightarrow Z$ be continuous mappings. Suppose the mapping $g$ separated and the mapping $g\circ f$ proper. Then the mapping $f$ is proper.

Consider the following cartesian square:

$X\times_ZY^{pr_2}$ Y

pr$_1g$

X $^{g\circ f}Z$.

Let $s: X\rightarrow X\times_ZY$ be the mapping $x\mapsto (x, f(x))$. It is a continuous section of pr$_1: X\times_ZY\rightarrow X$. By prop. 4, the mapping pr$_1$ is separated; it follows that the mapping $s$ is proper (I, p. 27, prop. 3 and TG, I, p. 72, prop. 2). On the other hand, the mapping pr$_2$ is proper (I, p. 17, prop. 8). Hence the mapping $f$, which is equal to pr$_2\circ s$, is proper (TG, I, p. 73, prop. 5).

### 2. Etale mappings

#### Definition 2 {#ta-i-s2-def-2 .statement tag=01MS}

Let E and B be topological spaces, let $p: E\rightarrow B$ be a mapping and let $x$ be a point of E. One says that the mapping $p$ is topologically etale at $x$ if there exists a neighbourhood U of $x$ in E and a neighbourhood V of $p(x)$ in B such that $p$ induces a homeomorphism of U onto V.

One says that the mapping $p$ is topologically etale if it is topologically etale at every point $x$ of E.

When no confusion is possible, cf. example 3 below, one shall say etale instead of topologically etale. Instead of saying that $p: E\rightarrow B$ is an etale mapping, one also says that the B-space $(E, p)$ is an etale B-space, or simply that E is a space spread over B, when no doubt is possible as to the mapping $p$.

#### Remark 1 {#ta-i-s2-n2-rem-1 .statement tag=01MT}

The set of points of E at which a mapping $p: E\rightarrow B$ is etale is an open set U of E, and the restriction of $p$ to U is an etale mapping of U into B.

#### Remark 2 {#ta-i-s2-n2-rem-2 .statement tag=01MU}

An etale mapping is continuous and open (TG, I, p. 33, prop. 5) ; in particular, the image of an etale mapping is open. Conversely, if $p: E\rightarrow B$ is a continuous and open mapping, and if every point $x$ of E possesses a neighbourhood V such that the mapping $p|V$ is injective, the mapping $p$ is etale. The fibres of an etale mapping are discrete.

#### Example 1 {#ta-i-s2-n2-exa-1 .statement tag=01MV}

Let B be a topological space and $(U_i)_{i\in I}$ a family of subsets of B. Let E denote the sum space of the family $(U_i)_{i\in I}$ and $p: E\rightarrow B$ the mapping deduced from the canonical injections of the $U_i$ into B. In order that the mapping $p$ be etale, it is necessary and sufficient that the $U_i,i\in I$, all be open.

#### Example 2 {#ta-i-s2-n2-exa-2 .statement tag=01MW}

Let U be an open set of $\mathbf{C}$. In order that a holomorphic function $f: U\rightarrow \mathbf{C}$ be an etale mapping, it is necessary and sufficient that its derivative nowhere vanish.

#### Example 3 {#ta-i-s2-n2-exa-3 .statement tag=01MX}

An etale morphism of varieties (VAR, R, 5.7.8) is a topologically etale mapping, but there exist morphisms of real varieties which are topologically etale and which are not etale morphisms. This is the case, for example, of the mapping $x\mapsto x^3$ of $\mathbf{R}$ into $\mathbf{R}$. However, a morphism of complex analytic varieties which is topologically etale is an etale morphism (I, p. 141, exerc. 6).

#### Proposition 6 {#ta-i-s2-prop-6 .statement tag=01MY}

Let X, Y, Z be topological spaces and let $f: X\rightarrow Y,g: Y\rightarrow Z$ be mappings.

a) Suppose that $f$ and $g$ are etale; then $g\circ f$ is etale.

b) Suppose that $g$ is étale, $f$ is continuous and $g\circ f$ is open. Then $f$ is open.

c) Suppose that $g\circ f$ and $g$ are étale and that $f$ is continuous. The mapping $f$ is then étale.

d) Suppose that $g\circ f$ is étale and that the mapping $f$ is continuous and open; then $f$ is étale and $g$ is étale at every point of $f(X)$.

Let us prove a). Suppose the mappings $f$ and $g$ are étale. Then they are continuous and open, hence the mapping $g\circ f$ is continuous and open. Let $x$ be a point of X. There exists a neighbourhood W of $f(x)$ in Y such that the mapping $g|W$ is injective, and a neighbourhood V of $x$

in X, contained in $\overset{-1}{f}(W)$, such that the mapping $f|V$ is injective; the mapping $(g\circ f)|V$ is then injective. This proves that the mapping $g\circ f$ is étale (remark 2).

Let us prove b). Let $x$ be a point of X and W an open neighbourhood of $f(x)$ such that $g$ induces a homeomorphism of W onto the open set $g(W)$. Let V be a neighbourhood of $x$ such that $f(V)$ is contained in W; then $g\circ f(V)$ is a neighbourhood of $g\circ f(x)$, hence $f(V)$ is a neighbourhood of $f(x)$ in the open set W, and also in Y. This proves that the mapping $f$ is open (TG, I, p. 33, prop. 5).

Let us prove c). By b$),f$ is open. Let $x$ be a point of X. Since $g\circ f$ is étale, there exists a neighbourhood V of $x$ in X such that $g\circ f|V$ is injective. Thus, $f|V$ is injective and $f$ is étale (I, p. 29, remark 2).

Let us prove d). Let $x$ be a point of X and put $y=f(x)$. There exists an open neighbourhood V of $x$ such that $g\circ f$ induces a homeomorphism of V onto the open set $g\circ f(V)$. Since the mapping $f$ is open, $f(V)$ is an open neighbourhood of $y$. The mapping $f|V: V\rightarrow f(V)$ deduced from $f$ by passing to subspaces is continuous, open and bijective; hence it is a homeomorphism, so that $f$ is étale at $x$. Moreover, the mapping $g$ induces a homeomorphism of $f(V)$ onto $g\circ f(V)$, hence is étale at $y$.

#### Corollary 1 {#ta-i-s2-prop-6-cor-1 .statement tag=01MZ}

Let B be a topological space. A B-morphism of one étalé B-space into another is étale.

This follows from assertion c) of prop. 6.

#### Corollary 2 {#ta-i-s2-prop-6-cor-2 .statement tag=01N0}

Let B be a topological space; a bijective B-morphism of one étalé B-space into another is a B-isomorphism.

By corollary 1, such a morphism is étale; it is therefore open (I, p. 29, remark 2). If it is bijective, it is a B-isomorphism.

#### Corollary 3 {#ta-i-s2-prop-6-cor-3 .statement tag=01N1}

Let $p: E\rightarrow B$ be an étale mapping. Every continuous section of $p$ induces a homeomorphism of B onto an open subset of E.

In fact, such a section is étale (corollary 1), hence open.

#### Corollary 4 {#ta-i-s2-prop-6-cor-4 .statement tag=01N2}

Let $p: E\rightarrow B$ be an étale and separated mapping. Suppose that E is connected and that $p$ admits a section. Then $p$ is a homeomorphism.

Let $s$ be a section of $p$; since $p$ is étale, the image of $s$ is open in E (Corollary 3); it is also closed, since $p$ is separated (I, p. 27, Prop. 3). Since E is connected, we have $s(B) = E$ and $p$ is a homeomorphism.

#### Proposition 7 {#ta-i-s2-prop-7 .statement tag=01N3}

Let $p: E\rightarrow B$ be a continuous mapping. In order that the mapping $p$ be étale, it is necessary and sufficient that it be open and that the diagonal $\Delta_E$ of $E\times_BE$ be open in $E\times_BE$.

Suppose first that the mapping $p$ is étale. Then it is open and every point of E possesses a neighbourhood V such that $p|V$ is injective, which amounts to saying that one has $(V\times V)\cap (E\times_BE)\subset \Delta_E$. Hence $\Delta_E$ is an open subset of $E\times_BE$.

Conversely, suppose that $p$ is an open mapping and that $\Delta_E$ is an open subset of $E\times_BE$. Let $x$ be a point of E. Let V be an open neighbourhood of $x$ in E such that $(V\times V)\cap (E\times_BE)$ is contained in $\Delta_E$. Then $p|V$ is injective. By Remark 2, I, p. 29, the mapping $p$ is étale.

#### Proposition 8 {#ta-i-s2-prop-8 .statement tag=01N4}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. If the mapping $p$ is étale, the mapping $p'$ is étale. Conversely, if the mapping $p'$ is étale and the mapping $f$ is universally strict and surjective, the mapping $p$ is étale.

Suppose that the mapping $p$ is étale. It is in particular open and $p'$ is open (I, p. 17, Prop. 8). Consider then the cartesian square (I, p. 13, Example 1)

$$
E'\times_{B'}{E'}^{\varphi}E\times_BE
$$

$q'q$

${B'}^fB$. One has $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ (loc. cit.). Moreover, the diagonal $\Delta_E$ is open in $E\times_BE$ (Prop. 7), hence the diagonal $\Delta_{E'}$ is open in $E'\times_{B'}E'$. This proves that the mapping $p'$ is étale (loc. cit.).

Suppose now that the mapping $f$ is surjective and universally strict and that the mapping $p'$ is étale. Then $p'$ is open, hence $p$ is open (I, p. 21, Prop. 11, a)). On the other hand $\Delta_{E'}$ is an open subset of $E'\times_{B'}E'$. Since $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ and the mapping $\varphi$ is surjective and strict (I, p. 20, Def. 6), $\Delta_E$ is open in $E\times_BE$. By Prop. 7, the mapping $p$ is étale.

#### Corollary {#ta-i-s2-n2-cor-1 .statement tag=01N5}

Let B be a topological space. The fibre product of two étale B-spaces is an étale B-space.

Let $(E, p)$ and $(E', p')$ be étale B-spaces. The mapping pr$_1: E\times_B$ $E'\rightarrow E$ is étale (prop. 8), hence the mapping $p\circ$ pr$_1: E\times_BE'\rightarrow B$ is étale (prop. 6, a)).

#### Remark 3 {#ta-i-s2-n2-rem-3 .statement tag=01N6}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. If the mapping $p$ is étale and if the mapping $f$ is strict, the mapping $f'$ is strict. In fact, under these hypotheses, every point of E possesses an open neighbourhood U such that $p$ induces a homeomorphism of U onto the open set $p(U)$. The mapping $p'$ then induces

a homeomorphism of $(\overset{-1}{f}')(U)$ onto $\overset{-1}{f}(p(U))$. The mapping $f$ induces

a strict mapping of $\overset{-1}{f}(p(U))$ onto $p(U)$ (I, p. 20) and the mapping

$f'$ therefore induces a strict mapping of $(\overset{-1}{f}')(U)$ into U. It follows that the mapping $f'$ is strict ( I, p. 23, corollary 2).

### 3. Local sections of étale mappings

Let E and B be sets, A a subset of B and $p: E\rightarrow B$ a mapping. A section of $p$ over A (or on A) is a mapping $s: A\rightarrow E$ such that $p\circ s$ is the canonical injection of A into B. To give a section $s$ of $p$ over A amounts to giving a section of the mapping $p_A:\overset{-1}{p}(A)\rightarrow A$ deduced from $p$. If $s$ is a section of $p$ over A and if $A'$ is a subset of A, the restriction $s'$ of $s$ to $A'$ is a section of $p$ over $A'$. One then says that $s$ is an extension of $s'$ to A.

When E and B are topological spaces and $p: E\rightarrow$ B a continuous mapping, the set $\mathscr{C}_B(A; E)$ (I, p. 2) of continuous sections of $p$ over A is also denoted by $\mathscr{S}(A;p)$ or $\mathscr{S}(A; E)$. Let $s$ be a continuous section of $p$ over A. The mapping $s$ induces a homeomorphism of A onto $s(A)$, and $p$ induces the reciprocal homeomorphism. By definition 2, I, p. 28, we therefore have:

#### Proposition 9 {#ta-i-s2-prop-9 .statement tag=01N7}

Let $p: E\rightarrow B$ be a continuous mapping. In order that the mapping $p$ be étale, it is necessary and sufficient that every point of E possess an open neighbourhood which is the image of a continuous section of $p$ over an open subset of B.

#### Remark 1 {#ta-i-s2-n3-rem-1 .statement tag=01N8}

Let $p: E\rightarrow B$ be a continuous and open mapping. In order that an open set U of E be the image of a continuous section of $p$ over an open set of B, it is necessary and sufficient that the restriction of $p$ to U be injective.

#### Remark 2 {#ta-i-s2-n3-rem-2 .statement tag=01N9}

Let $p: E\rightarrow$ B be a continuous mapping. Suppose that every point of B possesses an open neighbourhood V such that there exists a continuous section of $p$ over V. Such a mapping $p$ is not necessarily étale, nor even open. It is nevertheless surjective and universally strict (I, p. 20, corollary).

### 4. Continuous liftings of étale mappings

Let $p: E\rightarrow B$ and $f: Z\rightarrow B$ be continuous mappings. A continuous lifting of $f$ to E means a continuous mapping $g: Z\rightarrow E$ such that $p\circ g=f$. The set of continuous liftings of $f$ to E is none other than $\mathscr{C}_B(Z; E)$. It is also identified with the set $\mathscr{S}(Z; Z\times_BE)$ of continuous sections of the projection of the Z-space $(Z\times_BE$, pr$_1)$.

If T is a subset of Z, a continuous lifting of $f$ to E defined on T means a continuous lifting of $f|T$ to E:

$$
\begin{array}{ccc}
 &  & E\\
 & \nearrow & \Big\downarrow{\scriptstyle p}\\
T\subset Z & \xrightarrow{\ f\ } & B.
\end{array}
$$

#### Proposition 10 {#ta-i-s2-prop-10 .statement tag=01NA}

Let E, B and Z be topological spaces, $p: E\rightarrow B$ an étale mapping and $f: Z\rightarrow B$ a continuous mapping.

Let $z\in Z$ and $x\in E$ be points such that $f(z) =p(x)$. There exists a neighbourhood W of $z$ in Z and a continuous lifting $g$ of $f$ to E, defined on W, such that $g(z) =x$.

There exists an open neighbourhood V of $p(x)$ in B and a continuous section $s$ of $p$ over V such that $s(p(x)) =x$ (prop. 9). The set

$W =\overset{-1}{f}(V)$ is an open neighbourhood of $z$ and the mapping $g=s\circ (f|W)$ is a continuous lifting of $f$ to E, defined on W and such that $g(z) =x$.

#### Proposition 11 {#ta-i-s2-prop-11 .statement tag=01NB}

Let E, B and Z be topological spaces, $p: E\rightarrow B$ and $f: Z\rightarrow B$ continuous mappings. Let $g$ and $g'$ be continuous liftings of $f$ to E. Let W be the set of points of Z where $g$ and $g'$ coincide.

a) If the mapping $p$ is separated, W is closed.

b) If the mapping $p$ is étale, W is open.

Let us denote by $h$ the continuous mapping $(g, g'): Z\rightarrow E\times E$. The image of $h$ is contained in $E\times_BE$ since $p\circ g=f=p\circ g'$ and the set W of points of Z where $g$ and $g'$ coincide is the inverse image under $h$ of the diagonal $\Delta_E$.

If the mapping $p$ is étale, the diagonal $\Delta_E$ is open in $E\times_BE$ (I, p. 31, prop. 7), therefore the set W is open in Z.

If the mapping $p$ is separated, the diagonal $\Delta_E$ is closed in $E\times_BE$ (I, p. 25, def. 1) and the set W is closed in Z.

#### Corollary 1 {#ta-i-s2-prop-11-cor-1 .statement tag=01NC}

If the space Z is connected and if the mapping $p$ is étale and separated, continuous liftings of $f$ to E which coincide at one point are equal.

#### Corollary 2 {#ta-i-s2-prop-11-cor-2 .statement tag=01ND}

Let $p: E\rightarrow B$ be an étale and separated mapping. If the space E is connected, the group Aut$_B(E)$ operates freely on E.

In fact, if $f: E\rightarrow E$ is a B-morphism, the set of points where $f$ and Id$_E$ coincide is equal to E or to the empty set by Cor. 1.

#### Corollary 3 {#ta-i-s2-prop-11-cor-3 .statement tag=01NE}

Let E, B and Z be topological spaces, let $p: E\rightarrow B$ be an étale and separated mapping, and let $f: Z\rightarrow B$ be a continuous mapping. For $i= 1$, 2, let $U_i$ be an open subset ( resp. closed subset) of Z and $g_i: U_i\rightarrow E$ a continuous lifting of $f$ defined on $U_i$. Suppose that the intersection $U_1\cap U_2$ is connected and that there exists a point $z$ of $U_1\cap U_2$ such that $g_1(z) =g_2(z)$. Then there exists a continuous lifting of $f$ defined on $U_1\cup U_2$ which extends $g_1$ and $g_2$.

By Corollary 1, the restrictions of $g_1$ and $g_2$ to $U_1\cap U_2$ are equal. The mapping $g: U_1\cup U_2\rightarrow E$ defined by $g(z) =g_i(z)$ for $z\in U_i(i= 1$, 2) is a continuous lifting of $f$ defined on $U_1\cup U_2$ (TG, I, p. 19, Prop. 4).

In the preceding results, the particular case where Z = B and $f=$ Id$_B$ is important: the continuous liftings of $f$ are then the continuous sections of $p$.

#### Proposition 12 {#ta-i-s2-prop-12 .statement tag=01NF}

Let $p: E\rightarrow B$ be an étale mapping. In order that the mapping $p$ be separated, it is necessary and sufficient that for every open subset V of B and every pair $(s, s')$ of continuous sections of $p$ over V, the set of points where $s$ and $s'$ coincide be closed in V.

The condition is necessary (Proposition 11, I, p. 34). Let us prove that it is sufficient. Let $b$ be a point of B, let $x$ and $x'$ be two distinct points of E such that $p(x) =p(x') =b$. Let V be an open neighbourhood of $b$ and $s,s'$ continuous sections of $p$ over V such that $s(V)$ and $s'(V)$ are open neighbourhoods of $x$ and $x'$ respectively (Prop. 9). By hypothesis, the set W of points $x\in V$ such that $s(x)=\not s'(x)$ is open in V, hence in B. The sets $s(W)$ and $s'(W)$ are open neighbourhoods of $x$ and $x'$ respectively; they are disjoint by construction. This proves that the mapping $p$ is separated (I, p. 25, Definition 1).

### 5. Construction of continuous sections of étale mappings

#### Theorem 1 {#ta-i-s2-thm-1 .statement tag=01NG}

Let X, Y, Z be topological spaces, let $f: Z\rightarrow$ $X\times Y$ be an étale and separated mapping, and let $y_0$ be a point of Y. Let $s: X\times Y\rightarrow Z$ be a section of $f$. Suppose that the restriction of $s$ to $X\times  \{y_0\}$ is continuous, as are analogously the restrictions of $s$ to $\{x\} \times Y$ for every $x\in X$. If the space Y is connected and locally connected (TG, I, p. 84, def. 4), the mapping $s$ is continuous.

#### Lemma {#ta-i-s2-n5-lem-1 .statement tag=01NH}

Let U be an open set of X, let V be a connected open set of Y, and let $(x_1, y_1)\in U\times V$. Suppose that the restriction of $s$ to $U\times  \{y_1\}$ is continuous. Let $\sigma$ be a continuous section of $f$ over $U\times V$ such that $\sigma (x_1, y_1) =s(x_1, y_1)$. There exists a neighbourhood $U'$ of $x_1$ such that $s=\sigma$ on $U'\times V$. In particular, $s$ is continuous in a neighbourhood of $(x_1, y_1)$.

Since the restriction of $s$ to $U\times  \{y_1\}$ is continuous and the mapping $f$ is étale, there exists a neighbourhood $U'$ of $x_1$ such that $s(x, y_1) =\sigma (x, y_1)$ for every $x\in U'($I, p. 34, prop. 11, b)). Let $x\in U'$; since the restriction of $s$ to $\{x\} \times V$ is continuous and the mapping $f$ is étale and separated, it follows from Corollary 1, I, p. 34, that $\sigma (x, y) =s(x, y)$ for every $y\in V$. Thus $s$ and $\sigma$ coincide on $U'\times V$.

We now prove the theorem. First let us prove that the mapping $s$ is continuous in a neighbourhood of every point of $X\times  \{y_0\}$. Let $x_0\in$ X; one can choose an open neighbourhood U of $x_0$ in X, a connected open neighbourhood V of $y_0$ in Y, and a continuous section $\sigma : U\times V\rightarrow Z$ of $f$ such that $\sigma (x_0, y_0) =s(x_0, y_0)$. By the above lemma, $s$ is continuous in a neighbourhood of $(x_0, y_0)$.

Let us now prove that the mapping $s$ is continuous at every point of $X\times Y$. For $x_0\in X$, let us denote by $C(x_0)$ the set of points $y\in$ Y such that $s$ is continuous in a neighbourhood of $(x_0, y)$. The set $C(x_0)$ is open in Y by definition, and contains $y_0$ by what precedes.

Let us prove that it is closed in Y. Consider a point $y_1$ of Y adherent to $C(x_0)$, an open neighbourhood U of $x_0$ in X, an open neighbourhood V of $y_1$ in Y, and a continuous section $\sigma : U\times V\rightarrow Z$ of $f$ such that $\sigma (x_0, y_1) =s(x_0, y_1)$. Since the restriction of $s$ to $\{x_0\} \times V$ is continuous and $f$ is étale, there exists an open neighbourhood $V'$ of $y_1$ in Y such that $\sigma (x_0, y) =s(x_0, y)$ for every $y\in V'$ (prop. 11 of I, p. 34). Since Y is locally connected, we may suppose that $V'$ is connected. Since $y_1$ is adherent to $C(x_0)$, the set $C(x_0)\cap V'$ is not empty; let $y_2$ be a point of $C(x_0)\cap V'$. By the lemma applied to $(x_0, y_2)$, there exists a neighbourhood $U'$ of $x_0$ contained in U such that $s=\sigma$ over $U'\times V'$. This proves that $C(x_0)$ is closed, for $U'\times V'$ is a neighbourhood of $(x_0, y_1)$. Since Y is connected, we have $C(x_0) = Y$, and this for every $x_0\in X$, whence the theorem.

#### Corollary 1 {#ta-i-s2-thm-1-cor-1 .statement tag=01NI}

Let X, Y, E, B be topological spaces. Let $p: E\rightarrow B$ be an étale and separated mapping, let $h: X\times Y\rightarrow B$ be a continuous mapping and let $y_0$ be a point of Y. Let $g: X\times Y\rightarrow E$ be a mapping such that $p\circ g=h$. Suppose that the restrictions of $g$ to $X\times  \{y_0\}$ on the one hand and, for every $x\in X$, to $\{x\} \times Y$ on the other hand, are continuous. If the space Y is connected and locally connected, the mapping $g$ is continuous.

Let us denote by Z the fibre product $(X\times Y)\times_BE$ and by $f: Z\rightarrow X\times Y,h': Z\rightarrow E$ the canonical projections. The mapping $f$ is étale (I, p. 31, prop. 8) and separated (I, p. 27, prop. 4). The mapping $s: X\times Y\rightarrow$ Z defined by $s(x, y) = ((x, y), g(x, y))$ is a section of $f$ satisfying the hypotheses of theorem 1. It is therefore continuous, as is $g=h'\circ s$.

#### Remark {#ta-i-s2-n5-rem-1 .statement tag=01NJ}

If, in theorem 1, it is not supposed that the space Y is locally connected, the conclusion of the theorem is no longer necessarily true (I, p. 141, exerc. 7).

#### Theorem 2 {#ta-i-s2-thm-2 .statement tag=01NK}

Let B be a topological space and A a subspace of B. Make one of the following hypotheses:

(i) A admits a fundamental system of paracompact neighbourhoods;

(ii) B is paracompact and A closed;

(iii) B is metrizable;

(iv) A is compact and two distinct points of A possess disjoint neighbourhoods in B.

Then every continuous section over A of an étale mapping $p: E\rightarrow B$ extends to a continuous section of $p$ over a neighbourhood of A.

Consider the following property (PCV) of the pair $(B,A)$:

(PCV) For every covering $(U_i)_{i\in I}$ of A by open subsets

of B, there exists a neighbourhood V of A and a locally

finite family $(F_j)_{j\in J}$ of closed subsets of V covering V, such that

each of the $F_j$ is contained in one of the $U_i$.

Theorem 2 follows from Lemmas 1 and 3 below.

#### Lemma 1 {#ta-i-s2-lem-1 .statement tag=01NL}

Each of properties (i) to (iv) of theorem 2 implies property (PCV).

Let $(U_i)_{i\in I}$ be an open covering of A by open sets of B. Under hypothesis (i), there exists a paracompact neighbourhood V of A contained in the union of the $U_i$, an open covering $(U'_j)_{j\in J}$ of the space V, locally finite and finer than the covering $(V\cap U_i)_{i\in I}$, and an open covering $(U''_j)_{j\in J}$ of the space V such that for every $j\in J$, the closure $F_j$ of $U''_j$ in V is contained in $U'_j$ (TG, IX, p. 49, prop. 4 and p. 48, cor. 1 to th. 3). Hence property (PCV) in this case.

Condition (ii) implies condition (i) by Corollary 2 of TG, IX, p. 50. Analogously, condition (iii) implies condition (i): in fact, if B is metrisable, every neighbourhood of A is metrisable, hence paracompact (TG, IX, p. 51, th. 4).

Lastly, suppose that condition (iv) is satisfied, and let us show that property (PCV) holds. Since A is compact, it is enough to consider the case of a finite covering $(U_i)_{0\leqslant i\leqslant n}$. We then construct by induction open sets $V_0, . . . ,V_n$ of B satisfying the following conditions for $0\leqslant i\leqslant n:$

$$
\alpha )A\subset V_0\cup  \cdots  \cup V_i\cup U_{i+1}\cup  \cdots  \cup U_n
$$

$$
\beta )\overline{V_i}\cap A\subset U_i
$$

Suppose that $V_0, . . . ,V_{r-1}$ have been constructed satisfying the above conditions for $0\leqslant i\leqslant r-1$, and let us construct $V_r$. The sets K = $A\cap \complement U_r$ and $L = A\cap \complement (V_0\cup \cdots \cup V_{r-1}\cup U_{r+1}\cup \cdots \cup U_n)$ are closed in A, hence compact. By virtue of $(\alpha )$, they are disjoint. By hypothesis, for every point $a$ of L and every point $b$ of K, there exist disjoint neighbourhoods of $a$ and $b$ in B. By Lemma 2 below, there exist disjoint open sets $V_r$ and W in B such that $L\subset V_r$ and $K\subset W$. From the inclusions $L\subset V_r$ and $A\subset V_0\cup  \cdots  \cup V_{r-1}\cup U_r\cup  \cdots  \cup U_n$ and from the definition of L, it follows that $(\alpha )$ holds for $i=r$. On the other hand, we have $\overline{V_r}\cap K =\emptyset$, hence $\overline{V_r}\cap A\subset U_r$.

The set $M =\bigcup_{0\leqslant i\leqslant n}(V_i\cap \complement U_i)$ is closed and does not meet A by $(\beta )$. By $(\alpha )$, the set $V =((\bigcup_{0\leqslant i\leqslant n}\overline{V_i})-$ M is a neighbourhood of A in B. For $i= 0, . . . , n$, put $F_i= V\cap \overline{V_i}:$ this is a closed subset of V, contained in $U_i$. The family $(F_i)_{0\leqslant i\leqslant n}$ is a covering of V, whence property (PCV).

#### Lemma 2 {#ta-i-s2-lem-2 .statement tag=01NM}

Let B be a topological space, and let K and L be quasi-compact subsets of B. Suppose that for every point $a$ of K and every point $b$ of L, there exist disjoint neighbourhoods of $a$ and $b$ in B. Then there exist two disjoint open sets U and V in B such that $K\subset U$ and $L\subset V$.

Let $a$ be a point of K. For every $b\in L$, let $U_{a,b}$ and $V_{a,b}$ be disjoint open neighbourhoods of $a$ and of $b$. For fixed $a$, the family $(V_{a,b})_{b\in L}$ is an open covering of L. Since this space is quasi-compact, there exists a finite family $T_a\subset L$ such that the union $V_b$ of the $V_{a,b}$ for $b\in T_a$ contains L. The intersection $U_a$ of the $U_{a,b}$ for $b\in T_a$ is an open neighbourhood of $a$, since $T_a$ is finite; moreover, $U_a$ and $V_a$ are disjoint. The $(U_a)_{a\in A}$ form an open covering of K. Since K is quasi-compact, there exists a finite family $S\subset K$ such that $U =\bigcup_{a\in S}U_a$ contains K. Then $V =\bigcap_{a\in S}V_a$ is an open subset of B which contains L. The lemma is proved.

#### Lemma 3 {#ta-i-s2-lem-3 .statement tag=01NN}

Let B be a topological space and A a subspace of B such that the pair $(B,A)$ satisfies property (PCV) of I, p. 37. Then every continuous section over A of an étale mapping $p: E\rightarrow B$ extends to a continuous section of $p$ over a neighbourhood of A.

Let $p: E\rightarrow B$ be an étale mapping and $s: A\rightarrow E$ a continuous section of $p$ over A. For every point $a$ of A, there exists an open neighbourhood $U_a$ of $a$ and a continuous section $s_a: U_a\rightarrow E$ which coincides with $s$ on $U_a\cap A$ (I, p. 34, Prop. 10 and I, p. 34, Prop. 11). The family $(U_a)_{a\in A}$ is a covering of A by open subsets of B. Let V be a neighbourhood of A in B, let $(F_j)_{j\in J}$ be a locally finite family of closed subsets of V covering V, and let $a: J\rightarrow A$ be a mapping such that $F_j$ is contained in $U_{a(j)}$ for every $j\in J$ (property (PCV)). Let $s_j$ denote the restriction of $s_{a(j)}$ to $F_j$. Let W be the set of points $b\in V$ satisfying $s_j(b) =s_k(b)$ for every pair $(j, k)\in J\times J$ such that $b\in F_j\cap F_k$. One defines a section $s': W\rightarrow E$ by $s'(b) =s_j(b)$ if $b\in F_j$. We have $A\subset W$ and $s'|A =s$. The section $s'$ is continuous by Prop. 4 of I, p. 19.

It remains to prove that W is a neighbourhood of A in B. For every pair $(j, k)\in J\times J$, let $T_{jk}$ denote the set of points $b\in F_j\cap F_k$ such that $s_j(b)=\not s_k(b)$. The set $T_{jk}$ is closed in $F_j\cap F_k$ (Prop. 11, b) of I, p. 34), hence in V, and the sets $T_{jk}$ form a locally finite family of subsets of V. The union T of the family $(T_{jk})$ is therefore a closed set of V (TG, I, p. 6, Prop. 4). Now W is, by definition, the complement of T in V. It is therefore a neighbourhood of A in V and consequently in B.

### 6. Upper bound for the cardinal of the fibres of an étale and separated mapping

#### Theorem 3 {#ta-i-s2-thm-3 .statement tag=01NO}

Let E and B be topological spaces and let $p: E\rightarrow B$ be an étale and separated mapping. Suppose that E is connected and that B is locally connected. Let $\mathscr{W}$ be a basis for the topology of B. Then, for every point $a$ of B, one has Card(E$_a$)$\leqslant$ sup(Card($\mathscr{W}$), Card($\mathbf{N}$)).

Since the space B is locally connected, its topology has a basis $\mathscr{W}'$ consisting of connected open sets, for example the connected components of the open sets of $\mathscr{W}$ (TG, I, p. 85, Prop. 11). By virtue of Lemma 4 below, there exists a basis $\mathscr{V}$ for the topology of B consisting of connected open sets and such that Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

#### Lemma 4 {#ta-i-s2-lem-4 .statement tag=01NP}

Let B be a topological space, and let $\mathscr{W}$ and $\mathscr{W}'$ be bases for the topology of B. There exists a subset $\mathscr{V}$ of $\mathscr{W}'$ which is a basis for the topology of B and such that Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

Let $\mathscr{A}\subset \mathscr{W}\times \mathscr{W}$ be the set of pairs $(W_1,W_2)$ for which there exists $W'\in \mathscr{W}'$ such that $W_1\subset W'\subset W_2$; let $\varphi :\mathscr{A}\rightarrow \mathscr{W}'$ be a mapping such that one has $W_1\subset \varphi (W_1,W_2)\subset W_2$ for every pair $(W_1,W_2)\in \mathscr{A}$, and let $\mathscr{V}\subset \mathscr{W}'$ be the image of $\varphi$. One has

Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{A}$)$\leqslant$ Card($\mathscr{W}\times \mathscr{W}$)

(E, III, p. 25, Prop. 3). Let us prove that $\mathscr{V}$ is a basis for the topology of B. Let $x$ be a point of B and U a neighbourhood of $x$. By hypothesis, $x$ has a neighbourhood $W_2\in \mathscr{W}$ contained in U, a neighbourhood $W'\in \mathscr{W}'$ contained in $W_2$ and a neighbourhood $W_1\in \mathscr{W}$ contained in $W'$. Thus $W_1\subset W'\subset W_2\subset U$. Then $(W_1,W_2)\in \mathscr{A}$ and $\varphi (W_1,W_2)$ is a neighbourhood of $x$ contained in U. By Prop. 3 of TG, I, p. 5, the set $\mathscr{V}$ is a basis for the topology of B.

Let $\mathscr{V}$ be a basis for the topology of B consisting of nonempty connected open sets and such that Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$. Let $\mathscr{U}$ be the set of open sets U of E such that $p$ induces a homeomorphism of U onto an open set V belonging to $\mathscr{V}$. Every element of $\mathscr{U}$ is a connected nonempty open set. Since the mapping $p$ is étale, by Definition 2 (I, p. 28) and Prop. 3 of TG, I, p. 5, the set $\mathscr{U}$ is a basis for the topology of E. Let us call a caterpillar any finite sequence $(U_0, . . . ,U_n)$ of elements of $\mathscr{U}$ such that for $1\leqslant i\leqslant n,U_{i-1}\cap U_i$ is nonempty and $p(U_{i-1})\cap p(U_i)$ is connected. Let S denote the set of finite sequences of elements of $\mathscr{V}$ and, for every caterpillar $c= (U_0, . . . ,U_n)$, let us denote by $p(c)$ the sequence $(p(U_0), . . . , p(U_n))$.

#### Lemma 5 {#ta-i-s2-lem-5 .statement tag=01NQ}

a) Let $c= (U_0, . . . ,U_n)$ and $c'= (U'_0, . . . ,U'_m)$ be caterpillars such that $U_0= U'_0$ and $p(c) =p(c')$. Then $c=c'$.

b) Let U and $U'$ be elements of $\mathscr{U}$. Then there exists a caterpillar $c= (U_0, . . . ,U_n)$ such that $U_0= U$ and $U_n= U'$.

a) Necessarily, $m=n$. For every integer $i$ such that $0\leqslant i\leqslant n$, put $V_i=p(U_i)$ and let $s_i$ and $s'_i$ denote the continuous sections of $p$ over $V_i$ with respective images $U_i$ and $U'_i$. To prove the equality $c=c'$, we shall prove, by induction on $i$, the equality $s_i=s'_i$ for every integer $i$ such that $0\leqslant i\leqslant n$. By hypothesis, one has $s_0=s'_0$. Let $i$ be such that $1\leqslant i\leqslant n$ and $s_{i-1}=s'_{i-1}$. Since $U_{i-1}\cap U_i$ contains a point $x$, the continuous sections $s_{i-1}$ and $s_i$ coincide at $p(x)$, hence at every point of $V_{i-1}\cap V_i$, since it is connected (Corollary 1 of I, p. 34). The same is true of $s'_{i-1}$ and $s'_i$. For the same reason, $s_i$ and $s'_i$, which coincide on $V_{i-1}\cap V_i$, also coincide on $V_i$, whence the result.

b) If $x$ and $y$ are points of E, we say that a caterpillar $c= (U_0, . . . ,U_n)$ joins $x$ to $y$ if $x\in U_0$ and $y\in U_n$. In the set E, let R be the relation “there exists a caterpillar which joins $x$ to $y$”. The relation R is reflexive since $\mathscr{U}$ is a covering of E. It is obviously symmetric. Let us prove that it is transitive: let $x,y,z$ be three points of E, $(U_0, . . . ,U_n)$ and $(U'_0, . . . ,U'_m)$ caterpillars joining $x$ to $y$ and $y$ to $z$ respectively. Let $U\in \mathscr{U}$ be a neighbourhood of $y$ contained in $U_n\cap U'_0$; we have $p(U_n)\cap p(U) =p(U'_0)\cap p(U) =p(U)$, and, since U is connected , the sequence $(U_0, . . . ,U_n,U,U'_0, . . . ,U'_m)$ is a caterpillar which joins $x$ to $z$. The equivalence classes under R are open, hence also closed. Since E is connected, it follows that any two points of E are always joined by a caterpillar.

Let now U and $U'$ be elements of $\mathscr{U},x$ a point of U and $x'$ a point of $U'$. There exists a caterpillar $(U_2, . . . ,U_{n-2})$ joining $x$ to $x'$. Let $U_1$ and $U_{n-1}$ be open sets of $\mathscr{U}$ such that $x\in U_1,x'\in U_{n-1}$, $U_1\subset U\cap U_2,U_{n-1}\subset U'\cap U_{n-2}$. Put $U_0= U$, $U_n= U'$. Then the sequence $(U_0, . . . ,U_n)$ is a caterpillar.

Let us now prove the theorem. Let U be an element of $\mathscr{U}$ and let C be the set of caterpillars $(U_0, . . . ,U_n)$ such that $U_0= U$. The mapping of C into S which, to a caterpillar $c= (U_0, . . . ,U_n)$ of C, associates the sequence $p(c) = (p(U_0), . . . , p(U_n))$ is injective (lemma 5, a)), hence

(1) Card(C) $\leqslant$ Card(S).

The mapping of C into $\mathscr{U}$ which, to $c= (U_0, . . . ,U_n)\in C$, associates the open set $U_n$ is surjective by the second part of lemma 5, hence (2) Card($\mathscr{U}$)$\leqslant$ Card(C).

For every point $x$ of E, let us choose an open set $U_x$ of $\mathscr{U}$ such that $x\in U_x$. If $x$ and $y$ are distinct points of one and the same fibre $E_a$ of $p$, we have $U_x= U\not_y$ since $p|U_x$ is injective. Hence, for $a\in B$, (3) Card(E$_a$)$\leqslant$ Card($\mathscr{U}$).

Finally, if $\mathscr{V}$ is a finite set, the set S of finite sequences of elements of $\mathscr{V}$ is countable (E, III, p. 49, prop. 1), hence

(4) Card(S) $\leqslant$ Card($\mathbf{N}$).

If $\mathscr{V}$ is infinite, we have

(5) Card(S) = Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2=$ Card($\mathscr{W}$)

by the corollary of E, III, p. 50 and Corollary 1 of E, III, p. 49. The theorem follows from relations (1) to (5) above.

#### Remark {#ta-i-s2-n6-rem-1 .statement tag=01NR}

From the foregoing, if the topology of B admits a countable basis, the same is true of that of E and the fibres of E are countable (cf. TG, I, p. 88, Poincaré-Volterra theorem).

## EXERCISES {#ta-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
