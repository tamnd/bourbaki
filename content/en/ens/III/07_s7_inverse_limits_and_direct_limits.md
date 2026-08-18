---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 7
section_title: Inverse limits and direct limits
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 191-211, 251-254
pdf_pages: 0197-0217, 0257-0260
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS
      page: 191
      pdf_page: 197
    - "no": 2
      title: INVERSE SYSTEMS OF MAPPINGS
      page: 192
      pdf_page: 198
    - "no": 3
      title: DOUBLE INVERSE LIMIT
      page: 196
      pdf_page: 202
    - "no": 4
      title: CONDITIONS FOR AN INVERSE LIMIT TO BE NON-EMPTY
      page: 198
      pdf_page: 204
    - "no": 5
      title: DIRECT LIMITS
      page: 202
      pdf_page: 208
    - "no": 6
      title: DIRECT SYSTEMS OF MAPPINGS
      page: 204
      pdf_page: 210
    - "no": 7
      title: DOUBLE DIRECT LIMIT. PRODUCT OF DIRECT LIMITS
      page: 209
      pdf_page: 215
statements: 34
exercises: 9
errata:
    - says: no. 2, Proposition 2, Corollary 2
      read: no. 2, Proposition 1, Corollary 2
      why: The fact cited on page 197 is that the maps of an inverse system compose, h to the lambda nu being h to the lambda mu after h to the mu nu, and that is Corollary 2 of Proposition 1 of no. 2, the corollary on three inverse systems. Proposition 2 of that no. prints one corollary and it carries no number.
content_sha256: 3203bbc4a92310057bd8d756d11de83e7fba92da7a7a4944a0823379e9b3ec20
---

## 7. INVERSE LIMITS AND DIRECT LIMITS

### 1. INVERSE LIMITS

Let $I$ be a preordered set and let $(E_\alpha)_{\alpha\in I}$ be a family of sets indexed by $I$. For each pair $(\alpha,\beta)$ of elements of $I$ such that $\alpha\leq\beta$, let $f_{\alpha\beta}$ be a mapping of $E_\beta$ into $E_\alpha$. Suppose that the $f_{\alpha\beta}$ satisfy the following conditions :

$(\mathrm{LP}_I)$ *The relations $\alpha\leq\beta\leq\gamma$ imply $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$.*

$(\mathrm{LP}_{II})$ *For each $\alpha\in I$, $f_{\alpha\alpha}$ is the identity mapping of $E_\alpha$.*

Let $G=\prod_{\alpha\in I}E_\alpha$ be the *product* of the family of sets $(E_\alpha)_{\alpha\in I}$, and let $E$ denote the subset of $G$ consisting of all $x$ which satisfy each of the relations

(1)

$$\operatorname{pr}_{\alpha}x=f_{\alpha\beta}(\operatorname{pr}_{\beta}x)$$

for each pair of indices $(\alpha,\beta)$ such that $\alpha\leq\beta$. $E$ is said to be the *inverse limit of the family* $(E_\alpha)_{\alpha\in I}$ *with respect to the family of mappings* $(f_{\alpha\beta})$, and we write $E=\underset{\longleftarrow}{\lim}\,(E_\alpha,f_{\alpha\beta})$ or simply $E=\underset{\longleftarrow}{\lim}\,E_\alpha$ when there is no risk of ambiguity. By abuse of language, the pair $((E_\alpha),(f_{\alpha\beta}))$ (usually denoted by $(E_{\alpha\beta},f_{\alpha\beta})$) is called an *inverse system of sets*, relative to the index set $I$. The *restriction* $f_\alpha$ of the projection $\operatorname{pr}_\alpha$ to $E$ is called the *canonical mapping* of $E$ into $E_\alpha$, and we have the relation

(2)

$$f_\alpha=f_{\alpha\beta}\circ f_\beta$$

whenever $\alpha\leq\beta$; this is merely a transcription of the relations (1) which define $E$.

*Examples*

#### Example 1 {#ens-iii-s7-n1-exa-1 .statement tag=03TF}

Suppose that the order relation on $I$ is the relation of *equality*. Then the only pairs $(\alpha,\beta)$ such that $\alpha\leq\beta$ are the pairs $(\alpha,\alpha)$ where $\alpha\in I$; and since $f_{\alpha\alpha}$ is the identity mapping, the relation (1) is satisfied for *all* $x\in G$; in other words, $\underset{\longleftarrow}{\lim}\,E_\alpha$ is then the *product* $\prod_{\alpha\in I}E_\alpha$.

#### Example 2 {#ens-iii-s7-n1-exa-2 .statement tag=03TG}

Suppose that $I$ is *right directed*, that $E_\alpha$ is the same set $F$ for all $\alpha\in I$, and that $f_{\alpha\beta}$ is the identity mapping of $F$ onto itself whenever $\alpha\leq\beta$. Then $E=\underset{\longleftarrow}{\lim}\,E_\alpha$ is the *diagonal* $\Delta$ of the product $\prod_{\alpha\in I}E_\alpha=F^I$. Indeed, it is clear that each $x\in\Delta$ satisfies the relations (1). Conversely, let $x$ be an element of $E$, and let us show that for each pair of indices

$(\alpha, \beta)$ we have $\mathrm{pr}_\alpha x = \mathrm{pr}_\beta x$. By hypothesis, there exists an index $\gamma \in I$ such that $\alpha \leqslant \gamma$ and $\beta \leqslant \gamma$; hence by (1) we have $\mathrm{pr}_\alpha x = f_{\alpha\gamma}(\mathrm{pr}_\gamma x) = \mathrm{pr}_\gamma x$, and similarly $\mathrm{pr}_\beta x = \mathrm{pr}_\gamma x$, which proves our assertion.

It should be noted that $E = \varprojlim E_\alpha$ can be *empty* even when all the $E_\alpha$ are non-empty and all the mappings $f_{\alpha\beta}$ are *surjective* (Exercise 4; see no. 4).

¶ It is clear that for each subset J of I the pair consisting of the subfamily $(E_\alpha)_{\alpha \in J}$ and the family $(f_{\alpha\beta})$, where $\alpha \in J$, $\beta \in J$, and $\alpha \leqslant \beta$, is again an inverse system of sets relative to J; it is said to be obtained by *restricting* the index set to J. Let E and E' respectively denote the inverse limits of the families $(E_\alpha)_{\alpha \in I}$ and $(E_\alpha)_{\alpha \in J}$. For each $x \in E$ the element

$$g(x) = (f_\alpha(x))_{\alpha \in J} \tag{3}$$

belongs to E' by virtue of (2); the mapping $g : E \to E'$ so defined is called *canonical*. If J' is a subset of J, and E'' the inverse limit of the family $(E_\alpha)_{\alpha \in J'}$, and if $g' : E' \to E''$ and $g'' : E \to E''$ are the canonical mappings, then by definition we have

$$g'' = g' \circ g. \tag{4}$$

### 2. INVERSE SYSTEMS OF MAPPINGS

#### Proposition 1 {#ens-iii-s7-prop-1 .statement tag=03OC}

*Let* I *be an ordered set, let* $(E_\alpha, f_{\alpha\beta})$ *be an inverse system of sets relative to* I, *let* $E = \varprojlim E_\alpha$ *be its inverse limit, and for each* $\alpha \in I$ *let*

$$f_\alpha : E \to E_\alpha$$

*be the canonical mapping. For each* $\alpha \in I$, *let* $u_\alpha$ *be a mapping of a set* F *into* $E_\alpha$ *such that*

$$f_{\alpha\beta} \circ u_\beta = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta. \tag{5}$$

*Then :*

(a) *there exists a unique mapping* $u$ *of* F *into* E *such that*

$$u_\alpha = f_\alpha \circ u \qquad \textit{for all } \alpha \in I;\tag{6}$$

(b) *the mapping* $u$ *is injective if and only if, for each pair of distinct elements* $y$, $z$ *of* F, *there exists* $\alpha \in I$ *such that* $u_\alpha(y) \neq u_\alpha(z)$.

For the relation $u_\alpha = f_\alpha \circ u$ means that for each $y \in F$ we have

$$\mathrm{pr}_\alpha(u(y)) = u_\alpha(y);$$

the element $u(y) \in \prod_{\alpha \in I} E_\alpha$ is uniquely determined by $u(y) = (u_\alpha(y))_{\alpha \in I}$. It remains to be shown that $u(y) \in E$ for all $y \in F$, in other words, that

$$\mathrm{pr}_\alpha(u(y)) = f_{\alpha\beta}(\mathrm{pr}_\beta(u(y)))$$

whenever $\alpha \leqslant \beta$. But this can be written in the form

$$u_\alpha(y) = f_{\alpha\beta}(u_\beta(y))$$

and therefore follows from (5). The second part of the Proposition follows immediately from the definitions.

#### Corollary 1 {#ens-iii-s7-prop-1-cor-1 .statement tag=03RN}

*Let* $(E_\alpha, f_{\alpha\beta})$ *and* $(F_\alpha, g_{\alpha\beta})$ *be two inverse systems of sets relative to the same index set* I; *let* $E = \varprojlim E_\alpha$, $F = \varprojlim F_\alpha$, *and let* $f_\alpha$ *(resp.* $g_\alpha$*) be the canonical mapping of* E *into* $E_\alpha$ *(resp. of* F *into* $F_\alpha$*) for each* $\alpha \in I$, *For each* $\alpha \in I$, *let* $u_\alpha$ *be a mapping of* E *into* $F_\alpha$ *such that the diagram*

$$\begin{array}{ccc} E_\beta & \overset{u_\beta}{\longrightarrow} & F_\beta \\ {\scriptstyle f_{\alpha\beta}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\alpha\beta}} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*is commutative* [^1] *whenever* $\alpha \leqslant \beta$. *Then there exists a unique mapping* $u : E \to F$ *such that for each* $\alpha \in I$ *the diagram*

$$\begin{array}{ccc} E & \overset{u}{\longrightarrow} & F \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*is commutative.*

Put $v_\alpha = u_\alpha \circ f_\alpha$. If $\alpha \leqslant \beta$, we have, by (2),

$$g_{\alpha\beta} \circ v_\beta = g_{\alpha\beta} \circ u_\beta \circ f_\beta = u_\alpha \circ f_{\alpha\beta} \circ f_\beta = u_\alpha \circ f_\alpha = v_\alpha,$$

and we may therefore apply Proposition 1 to the mappings $v_\alpha$; hence the

existence and uniqueness of a mapping $u:E\to F$ such that

$$
g_\alpha\circ u=v_\alpha=u_\alpha\circ f_\alpha
$$

for each $\alpha\in I$.

¶ A family of mappings $u_\alpha:E_\alpha\to F_\alpha$ which satisfies the conditions of Corollary 1 is called an *inverse system of mappings* of $(E_\alpha,f_{\alpha\beta})$ into $(F_\alpha,g_{\alpha\beta})$. The mapping $u$ defined in Corollary 1 is called the *inverse limit* of the family $(u_\alpha)$ and is written $u=\underset{\leftarrow}{\lim}\,u_\alpha$ when there is no risk of confusion.

#### Corollary 2 {#ens-iii-s7-prop-1-cor-2 .statement tag=03RO}

Let $(E_\alpha,f_{\alpha\beta})$, $(F_\alpha,g_{\alpha\beta})$, $(G_\alpha,h_{\alpha\beta})$ be three *inverse systems of sets relative to the same index set* $I$; let $E=\underset{\leftarrow}{\lim}\,E_\alpha$, $F=\underset{\leftarrow}{\lim}\,F_\alpha$, $G=\underset{\leftarrow}{\lim}\,G_\alpha$, and let $f_\alpha$ (resp. $g_\alpha,h_\alpha$) be the *canonical mapping* of $E$ (resp. $F,G$) *into* $E_\alpha$ (resp. $F_\alpha,G_\alpha$). If $(u_\alpha)$ and $(v_\alpha)$ are *two inverse systems of mappings*, $u_\alpha:E_\alpha\to F_\alpha$, $v_\alpha:F_\alpha\to G_\alpha$, then the *composite mappings* $v_\alpha\circ u_\alpha:E_\alpha\to G_\alpha$ form an *inverse system of mappings*, and we have

(7)

$$
\underset{\leftarrow}{\lim}\,(v_\alpha\circ u_\alpha)
=
\left(\underset{\leftarrow}{\lim}\,v_\alpha\right)\circ
\left(\underset{\leftarrow}{\lim}\,u_\alpha\right).
$$

For if we put $w_\alpha=v_\alpha\circ u_\alpha$, then if $\alpha\leq\beta$ we have

$$
w_\alpha\circ f_{\alpha\beta}
=v_\alpha\circ(u_\alpha\circ f_{\alpha\beta})
=v_\alpha\circ(g_{\alpha\beta}\circ v_\beta)
=(h_{\alpha\beta}\circ v_\beta)\circ u_\beta
=h_{\alpha\beta}\circ w_\beta,
$$

which shows that $(w_\alpha)$ is an inverse system of mappings. Furthermore, if $u=\underset{\leftarrow}{\lim}\,u_\alpha$ and $v=\underset{\leftarrow}{\lim}\,v_\alpha$, then $h_\alpha\circ(v\circ u)=(v_\alpha\circ g_\alpha)\circ u=(v_\alpha\circ u_\alpha)\circ f_\alpha$ for each $\alpha\in I$, and therefore, by the uniqueness of the inverse limit, we have $v\circ u=\underset{\leftarrow}{\lim}\,w_\alpha$.

¶ Let $(E_\alpha,f_{\alpha\beta})$ be an inverse system of sets, and for each $\alpha\in I$ let $M_\alpha$ be a subset of $E_\alpha$. If $f_{\alpha\beta}(M_\beta)\subset M_\alpha$ whenever $\alpha\leq\beta$, the $M_\alpha$ are said to form an *inverse system of subsets* of the $E_\alpha$. Let $g_{\alpha\beta}$ be the mapping of $M_\beta$ into $M_\alpha$ (where $\alpha\leq\beta$) whose graph is the same as that of the restriction of $f_{\alpha\beta}$ to $M_\beta$. Then it is clear that $(M_\alpha,g_{\alpha\beta})$ is an inverse system of sets and that

(8)

$$
\underset{\leftarrow}{\lim}\,M_\alpha
=
\left(\underset{\leftarrow}{\lim}\,E_\alpha\right)\cap\prod_{\alpha\in I}M_\alpha.
$$

#### Proposition 2 {#ens-iii-s7-prop-2 .statement tag=03RP}

Let $(E_\alpha,f_{\alpha\beta})$ and $(E'_\alpha,f'_{\alpha\beta})$ be two *inverse systems of sets relative to* $I$, and let $u_\alpha$ be a mapping of $E_\alpha$ into $E'_\alpha$ for each $\alpha\in I$, such that the $u_\alpha$ form an *inverse system of mappings*. Let $u=\underset{\leftarrow}{\lim}\,u_\alpha$. Then for each $x'=(x'_\alpha)\in E'=\underset{\leftarrow}{\lim}\,E'_\alpha$, the $\bar u_\alpha^{-1}(x'_\alpha)$ form an *inverse system of subsets* of the $E_\alpha$, and $\bar u^{-1}(x')=\underset{\leftarrow}{\lim}\,\bar u_\alpha^{-1}(x'_\alpha)$.

For if $\alpha \leqslant \beta$ and $x_\beta \in \overset{-1}{u_\beta}(x'_\beta)$, we have

$$u_\alpha(f_{\alpha\beta}(x_\beta)) = f'_{\alpha\beta}(u_\beta(x_\beta)) = f'_{\alpha\beta}(x'_\beta) = x'_\alpha,$$

from which the first assertion follows; and to say that $x = (x_\alpha) \in \mathrm{E} = \varprojlim \mathrm{E}_\alpha$ is such that $u(x) = x'$ means, by definition, that $u_\alpha(x_\alpha) = x'_\alpha$ for each $\alpha \in \mathrm{I}$.

#### Corollary {#ens-iii-s7-n2-cor-1 .statement tag=03OD}

*If $u_\alpha$ is injective* (resp. *bijective*) *for each $\alpha \in \mathrm{I}$, then $u$ is injective* (resp. *bijective*).

With the notation of Proposition 2, the images $u_\alpha(\mathrm{E}_\alpha)$ also form an inverse system of subsets of the $\mathrm{E}'_\alpha$, and we have

(9) $$u(\mathrm{E}) \subset \varprojlim u_\alpha(\mathrm{E}_\alpha);$$

but the two sides of this relation are *not necessarily equal* (Exercise 4).

#### Proposition 3 {#ens-iii-s7-prop-3 .statement tag=03OE}

*Let $\mathrm{I}$ be a preordered set, let $(\mathrm{E}_\alpha, f_{\alpha\beta})$ be an inverse system of sets relative to $\mathrm{I}$, and let $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$. Let $\mathrm{J}$ be a cofinal subset of $\mathrm{I}$ such that $\mathrm{J}$ is right directed, and let $\mathrm{E}'$ be the inverse limit of the inverse system of sets obtained from $(\mathrm{E}_\alpha, f_{\alpha\beta})$ by restricting the index set to $\mathrm{J}$. Then the canonical mapping $g$ of $\mathrm{E}$ into $\mathrm{E}'$* (no. 1, *formula* (3)) *is bijective*.

For each $\alpha \in \mathrm{J}$, let $f'_\alpha$ be the canonical mapping $\mathrm{E}' \to \mathrm{E}_\alpha$. Then, by (2) and (5), $g$ is the unique mapping of $\mathrm{E}$ into $\mathrm{E}'$ such that $f_\alpha = f'_\alpha \circ g$ for all $\alpha \in \mathrm{J}$ (Proposition 1). We shall show that $g$ is injective by using the criterion of Proposition 1. If $x$, $y$ are distinct elements of $\mathrm{E}$, then by definition there exists $\alpha \in \mathrm{I}$ such that $f_\alpha(x) \neq f_\alpha(y)$; since $\mathrm{J}$ is cofinal in $\mathrm{I}$, there exists $\lambda \in \mathrm{J}$ such that $\alpha \leqslant \lambda$; since $f_{\alpha\lambda}(f_\lambda(x)) \neq f_{\alpha\lambda}(f_\lambda(y))$, we have $f_\lambda(x) \neq f_\lambda(y)$. It remains to be shown that $g$ is surjective. Let $x' = (x'_\lambda)_{\lambda \in \mathrm{J}}$ be an element of $\mathrm{E}'$. For each $\alpha \in \mathrm{I}$ there exists $\lambda \in \mathrm{J}$ such that $\alpha \leqslant \lambda$, and the element $f_{\alpha\lambda}(x'_\lambda)$ does not depend on the index $\lambda \in \mathrm{J}$ such that $\alpha \leqslant \lambda$; for if $\mu \in \mathrm{J}$ is such that $\alpha \leqslant \mu$, there exists $\nu \in \mathrm{J}$ such that $\lambda \leqslant \nu$ and $\mu \leqslant \nu$, hence $f_{\alpha\lambda}(x'_\lambda) = f_{\alpha\lambda}(f_{\lambda\nu}(x'_\nu)) = f_{\alpha\nu}(x'_\nu)$, and similarly $f_{\alpha\mu}(x'_\mu) = f_{\alpha\nu}(x'_\nu)$. Let $x_\alpha$ be the common value of the $f_{\alpha\lambda}(x'_\lambda)$ for the $\lambda \in \mathrm{J}$ such that $\alpha \leqslant \lambda$, and let $x = (x_\alpha)_{\alpha \in \mathrm{I}}$. Then $x \in \mathrm{E}$, because if $\alpha \leqslant \beta$ and if $\lambda \in \mathrm{J}$ is such that $\beta \leqslant \lambda$, we have

$$f_{\alpha\beta}(x_\beta) = f_{\alpha\beta}(f_{\beta\lambda}(x'_\lambda)) = f_{\alpha\lambda}(x'_\lambda) = x_\alpha.$$

Finally, we have $x'_\lambda = f_{\lambda\lambda}(x'_\lambda)$ for all $\lambda \in \mathrm{J}$, hence $x_\lambda = x'_\lambda$ for all $\lambda \in \mathrm{J}$; in other words, $f(x_\lambda) = x'_\lambda$, so that $g(x) = x'$. Therefore $g$ is surjective and the proof is complete.

In particular, if $\mathrm{I}$ has a *greatest element* $\omega$, we may take $\mathrm{J} = \{\omega\}$, so that $\varprojlim \mathrm{E}_\alpha$ is canonically identified with $\mathrm{E}_\omega$.

*Remarks*

#### Remark 1 {#ens-iii-s7-n2-rem-1 .statement tag=03TH}

For each $\alpha \in I$ put $E'_\alpha = f_\alpha(E)$. Then the sets $E'_\alpha$ form an *inverse system of subsets* of the $E_\alpha$ by reason of (2), and it is immediately clear that $\varprojlim E'_\alpha = E = \varprojlim E_\alpha$. The mapping $f'_{\alpha\beta} : E'_\beta \to E'_\alpha$ (where $\alpha \leqslant \beta$), whose graph is the same as that of the restriction of $f_{\alpha\beta}$ to $E_\beta$, is *surjective*, and we have

$$(10) \qquad E'_\alpha = f_\alpha(E) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(E_\beta)$$

for all $\alpha \in I$.

#### Remark 2 {#ens-iii-s7-n2-rem-2 .statement tag=03TI}

Let I be a (*right*) *directed* ordered set, let $(E_\alpha, f_{\alpha\beta})$ be an inverse system of sets relative to I, and for each $\alpha \in I$ let $u_\alpha : F \to E_\alpha$ be a mapping such that the family $(u_\alpha)$ satisfies formula (5). Consider the inverse system $(F_\alpha, i_{\alpha\beta})$ indexed by I, where $F_\alpha = F$ for all $\alpha \in I$ and $i_{\alpha\beta}$ is the identity mapping of F. Then (no. 1, Example 2) F is canonically identified with $\varprojlim F_\alpha$. If we consider $u_\alpha$ as a mapping of $F_\alpha$ into $E_\alpha$, then $(u_\alpha)$ is an inverse system of mappings, and the mapping $u : F \to E$ defined by (6) is identified with the inverse limit of this system of mappings. Hence, by abuse of language, we write $u = \varprojlim u_\alpha$.

#### Remark 3 {#ens-iii-s7-n2-rem-3 .statement tag=03TJ}

Let I be an ordered set and let $(E_\alpha, f_{\alpha\beta})$ be an inverse system of sets relative to I. For each finite subset J of I, let $F_J$ be the inverse limit of the (finite) inverse system obtained from $(E_\alpha, f_{\alpha\beta})$ by restricting the index set to J. If J and K are any two finite subsets of I such that $J \subset K$, let $g_{JK}$ denote the canonical mapping (3) of $F_K$ into $F_J$. Then the relation (4) shows that $(F_J, g_{JK})$ is an *inverse system* of sets relative to the *directed* set (with respect to the relation $\subset$) $\mathfrak{F}(I)$ of finite subsets of I. Next, for each $J \in \mathfrak{F}(I)$ let $h_J : E \to F_J$ be the canonical mapping (3). By virtue of (4) and with the abuse of language mentioned in Remark (2), $(h_J)$ is an *inverse system* of mappings. Put $h = \varprojlim h_J : E \to F = \varprojlim F_J$, and let us show that $h$ is a *bijection* (called *canonical*). Indeed, let $y = (y_J) \in F$. By definition we have $y_J = (x_{\alpha, J})_{\alpha \in J}$, where $x_{\alpha, J} \in E_\alpha$ for all $\alpha \in J$. If $J \subset K$, then by definition of the mapping $g_{JK}$ and because $y_J = g_{JK}(y_K)$, we have $x_{\alpha, J} = x_{\alpha, K}$ for all $\alpha \in J$. Hence, given $\alpha \in I$, there is a unique element $x_\alpha \in E_\alpha$ such that $x_\alpha = x_{\alpha, J}$ for all finite subsets J of I which contain $\alpha$. If $\alpha \leqslant \beta$, there is a finite subset J of I which contains both $\alpha$ and $\beta$; hence $x_\alpha = f_{\alpha\beta}(x_\beta)$ by definition. Consequently $x = (x_\alpha)$ is the unique element of E such that $h(x) = y$.

### 3. DOUBLE INVERSE LIMIT

Let I, L be two preordered sets, and $I \times L$ their product (§ 1, no. 4). Consider an inverse system of sets $(E^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ relative to the index set $I \times L$.

We have

(11) $\qquad f^{\lambda\nu}_{\alpha\gamma} = f^{\lambda\mu}_{\alpha\beta} \circ f^{\mu\nu}_{\beta\gamma}$ whenever $\alpha \leqslant \beta \leqslant \gamma$ and $\lambda \leqslant \mu \leqslant \nu$.

Let E or $\lim \mathrm{E}^{\lambda}_{\alpha}$ denote the inverse limit of this inverse system.

For each $\lambda \in \mathrm{L}$ put $g^{\lambda}_{\alpha\beta} = f^{\lambda\lambda}_{\alpha\beta} : \mathrm{E}^{\lambda}_{\beta} \to \mathrm{E}^{\lambda}_{\alpha}$. It follows from (11) that

(12) $\qquad g^{\lambda}_{\alpha\gamma} = g^{\lambda}_{\alpha\beta} \circ g^{\lambda}_{\beta\gamma}$ whenever $\alpha \leqslant \beta \leqslant \gamma$,

so that $(\mathrm{E}^{\lambda}_{\alpha}, g^{\lambda}_{\alpha\beta})$ is an inverse system of sets relative to I. Let $\mathrm{F}^{\lambda} = \lim \mathrm{E}^{\lambda}_{\alpha}$ denote its inverse limit. For fixed $\lambda \leqslant \mu$ in L it follows from (11) that the $h^{\lambda\mu}_{\alpha} = f^{\lambda\mu}_{\alpha\alpha} : \mathrm{E}^{\mu}_{\alpha} \to \mathrm{E}^{\lambda}_{\alpha}$ form an inverse system of mappings, whose inverse limit we denote by $h^{\lambda\mu} = \lim h^{\lambda\mu}_{\alpha} : \mathrm{F}^{\mu} \to \mathrm{F}^{\lambda}$. If $\lambda \leqslant \mu \leqslant \nu$ in L, we have

(13) $$h^{\lambda\nu} = h^{\lambda\mu} \circ h^{\mu\nu}$$

(no. 2, Proposition 2, Corollary 2); hence $(\mathrm{F}^{\lambda}, h^{\lambda\mu})$ is an inverse system of sets relative to L. Let $\mathrm{F} = \lim \mathrm{F}^{\lambda}$ be its inverse limit. We shall define a *canonical bijection* $\mathrm{F} \to \mathrm{E}$. To do this we note that F is by definition a subset of $\prod_{\lambda \in \mathrm{L}} \mathrm{F}^{\lambda}$, and $\mathrm{F}^{\lambda}$ is a subset of $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$; hence F may be canonically identified with a subset of $\prod_{(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}} \mathrm{E}^{\lambda}_{\alpha} = \mathrm{G}$ (Chapter II, § 5, no. 5, Proposition 7). For each $z \in \mathrm{G}$, let $\mathrm{pr}^{\lambda}(z)$ denote the element $(\mathrm{pr}^{\lambda}_{\alpha}(z))_{\alpha \in \mathrm{I}}$ of $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$. Then $z \in \mathrm{F}$ if and only if

(14) $\qquad \mathrm{pr}^{\lambda}(z) = h^{\lambda\mu}(\mathrm{pr}^{\mu}(z))$ whenever $\lambda \leqslant \mu$ in L

and $\mathrm{pr}^{\lambda}(z) \in \mathrm{F}^{\lambda}$ for all $\lambda \in \mathrm{L}$; that is to say, whenever $\alpha \leqslant \beta$ in I we have

(15) $$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\lambda}_{\alpha\beta}(\mathrm{pr}^{\lambda}_{\beta}(z)).$$

But $h^{\lambda\mu}(\mathrm{pr}^{\mu}(z)) = (f^{\mu\lambda}_{\alpha\alpha}(\mathrm{pr}^{\mu}_{\alpha}(z))_{\alpha \in \mathrm{I}}$; it therefore follows from (14) and (15) that if $\alpha \leqslant \beta$ and $\lambda \leqslant \mu$, we have

$$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\mu}_{\alpha\alpha}(f^{\mu\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z))) = f^{\lambda\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z)),$$

which implies that $z \in \mathrm{E}$. The converse is obvious, and we have therefore proved

#### Proposition 4 {#ens-iii-s7-prop-4 .statement tag=03OF}

*If* $(\mathrm{E}^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ *is an inverse system of sets relative to a product* $\mathrm{I} \times \mathrm{L}$ *of preordered sets, then (up to a canonical bijection) we have*

$$(16) \qquad \varprojlim_{\alpha,\lambda} \mathrm{E}^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

#### Corollary 1 {#ens-iii-s7-prop-4-cor-1 .statement tag=03OG}

*Let* $(\mathrm{E}'^\lambda_\alpha, f'^{\mu\lambda}_{\alpha\beta})$ *be another inverse system of sets relative to* $\mathrm{I} \times \mathrm{L}$, *and for each* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *let* $u^\lambda_\alpha$ *be a mapping of* $\mathrm{E}^\lambda_\alpha$ *into* $\mathrm{E}'^\lambda_\alpha$ *such that the* $u^\lambda_\alpha$ *form an inverse system of mappings. Then*

$$(17) \qquad \varprojlim_{\alpha,\lambda} u^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha u^\lambda_\alpha).$$

The verification is similar to that of Proposition 4.

#### Corollary 2 {#ens-iii-s7-prop-4-cor-2 .statement tag=03OH}

*Let* $(\mathrm{E}^\lambda_\alpha, f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$ *be a family of inverse systems of sets relative to* I. *If* $\prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta}$ *denotes the extension to products* (Chapter II, § 5, no. 7, Definition 2) *of the family of mappings* $(f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$, *then* $\left( \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha, \prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta} \right)$ *is an inverse system of sets relative to* I, *and (up to a canonical bijection) we have*

$$(18) \qquad \varprojlim_\alpha \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha = \prod_{\lambda \in \mathrm{L}} (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

Consider the double inverse system $(\mathrm{E}^\lambda_\alpha, g^{\lambda\mu}_{\alpha\beta})$ relative to $\mathrm{I} \times \mathrm{L}$, where the order relation on L is equality (no. 1, Example 1), and apply Proposition 4.

### 4. CONDITIONS FOR AN INVERSE LIMIT TO BE NON-EMPTY

In this subsection we shall give the two most frequently used sufficient conditions for an inverse limit to be non-empty (see also Exercise 5).

#### Proposition 5 {#ens-iii-s7-prop-5 .statement tag=03OI}

*Let* $(\mathrm{E}_\alpha, f_{\alpha\beta})$ *be an inverse system of sets relative to a* directed *set* I *which has a* countable *cofinal subset, and suppose furthermore that the* $f_{\alpha\beta}$ *are* surjective. *Then, if* $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$, *the canonical mapping* $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ *is surjective for each* $\alpha \in \mathrm{I}$ *(and, a fortiori,* E *is not empty provided that none of the* $\mathrm{E}_\alpha$ *is empty).*

Let $(\alpha_n)$ be a sequence of elements of I which form a cofinal subset of I. Since I is directed, we can define a sequence $(\beta_n)$ of elements of I inductively by the conditions $\beta_0 = \alpha_0, \beta_n \geqslant \beta_i$ for $i < n$ and $\beta_n \geqslant \alpha_n$. Clearly the sequence $(\beta_n)$ is increasing and forms a cofinal subset of I. In view of Proposition 1 of no. 1 and the relations $f_\alpha = f_{\alpha\beta_n} \circ f_{\beta_n}$ for

$\alpha \leqslant \beta_n$, we need only prove the Proposition for the case $\mathrm{I} = \mathbf{N}$. Moreover, it is clear that it suffices to prove that $f_0$ is surjective. Let $x_0 \in \mathrm{E}_0$. Define $x_n \in \mathrm{E}_n$ (for $n \geqslant 1$) inductively to be an element of the set $\overset{-1}{f}_{n-1,n}(x_{n-1})$, which is possible because the latter set is non-empty by hypothesis. We then show by induction on $n - m$ that $x_m = f_{mn}(x_n)$ for $m \leqslant n$, and it follows that $x = (x_n)$ belongs to E.

The second criterion concerns inverse systems $(\mathrm{E}_\alpha, f_{\alpha\beta})$ relative to an index set I such that for each $\alpha \in \mathrm{I}$ we are given a set $\mathfrak{S}_\alpha$ of subsets of $\mathrm{E}_\alpha$ which satisfy the following conditions :

(i)  *Every intersection of sets belonging to $\mathfrak{S}_\alpha$ also belongs to $\mathfrak{S}_\alpha$.*

It follows in particular (by considering the intersection of the empty family) that $\mathrm{E}_\alpha \in \mathfrak{S}_\alpha$.

(ii)  *If a set of subsets $\mathfrak{F} \subset \mathfrak{S}_\alpha$ is such that every finite intersection of sets belonging to $\mathfrak{F}$ is non-empty, then $\bigcap\limits_{\mathbf{M} \in \mathfrak{F}} \mathrm{M}$ is non-empty.*

In view of (i), it is clear that (ii) is equivalent to the following condition :

(ii)′  *If $\mathfrak{G} \subset \mathfrak{S}_\alpha$ is left directed (with respect to inclusion) and does not contain the empty set, then $\bigcap\limits_{\mathbf{M} \in \mathfrak{G}} \mathrm{M}$ is non-empty.*

#### Theorem 1 {#ens-iii-s7-thm-1 .statement tag=03RQ}

*Suppose that I is directed, that the sets $\mathfrak{S}_\alpha$ satisfy conditions* (i) *and* (ii), *and that the inverse system $(\mathrm{E}_\alpha, f_{\alpha\beta})$ has the following properties:*

(iii)  *For each pair of indices $\alpha$, $\beta$ such that $\alpha \leqslant \beta$, and each $x_\alpha \in \mathrm{E}_\alpha$, we have $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$.*

(iv)  *For each pair of indices $\alpha$, $\beta$ such that $\alpha \leqslant \beta$, and each $\mathrm{M}_\beta \in \mathfrak{S}_\beta$, we have $f_{\alpha\beta}(\mathrm{M}_\beta) \in \mathfrak{S}_\alpha$.*

*Let $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$ and let $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ be the canonical mapping for each $\alpha \in \mathrm{I}$. Then:*

(a)  *For each $\alpha \in \mathrm{I}$ we have*

$$(19) \qquad f_\alpha(\mathrm{E}) = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

(b)  *If $\mathrm{E}_\alpha$ is non-empty for each $\alpha \in \mathrm{I}$, then E is non-empty.*

Let $\Sigma$ be the set of families $\mathfrak{A} = (\mathrm{A}_\alpha)_{\alpha \in \mathrm{I}}$ which satisfy the following conditions :

$$(20) \qquad \mathrm{A}_\alpha \neq \emptyset \quad \textit{and} \quad \mathrm{A}_\alpha \in \mathfrak{S}_\alpha \quad \textit{for all} \quad \alpha \in \mathrm{I};$$

$$(21) \qquad f_{\alpha\beta}(\mathrm{A}_\beta) \subset \mathrm{A}_\alpha \quad \textit{whenever} \quad \alpha \leqslant \beta.$$

If $\mathfrak{A} = (A_\alpha)$ and $\mathfrak{A}' = (A'_\alpha)$ are any two elements of $\Sigma$, let the relation $\mathfrak{A} \leqslant \mathfrak{A}'$ mean that $A_\alpha \supset A'_\alpha$ for all $\alpha$. Clearly $\Sigma$ is *ordered* by this relation.

(1) Let us first show that the ordered set $\Sigma$ is *inductive*. Let L be a totally ordered set and let $\lambda \to \mathfrak{A}^\lambda = (A^\lambda_\alpha)_{\alpha \in I}$ be a strictly increasing mapping of L into $\Sigma$. For each $\alpha \in I$, put $B_\alpha = \bigcap_{\lambda \in L} A^\lambda_\alpha$. Then it is immediately seen that the family $\mathfrak{B} = (B_\alpha)_{\alpha \in I}$ satisfies (21); by reason of (i) and (ii), it also satisfies (20), hence belongs to $\Sigma$; and it is clear that $\mathfrak{B}$ is an upper bound of the set of the $\mathfrak{A}^\lambda$.

(2) Let $\mathfrak{A} = (A_\alpha)$ be a *maximal* element of $\Sigma$. We shall show that $A_\alpha = f_{\alpha\beta}(A_\beta)$ whenever $\alpha \leqslant \beta$. Let $A'_\alpha = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(A_\beta)$ for all $\alpha \in I$, and let us show that $\mathfrak{A}' = (A'_\alpha)$ belongs to $\Sigma$. Note first that if $\alpha \leqslant \beta \leqslant \gamma$, we have $f_{\alpha\gamma}(A_\gamma) = f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) \subset f_{\alpha\beta}(A_\beta)$ by (21); moreover, $f_{\alpha\beta}(A_\beta) \in \mathfrak{S}_\alpha$ by (iv), and $f_{\alpha\beta}(A_\beta) \neq \emptyset$ by (20). Hence conditions (i) and (ii) show that $\mathfrak{A}'$ satisfies (20). Also, if $\alpha \leqslant \beta$, we have

$$f_{\alpha\beta}(A'_\beta) \subset \bigcap_{\gamma \geqslant \beta} f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) = \bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma);$$

and for each $\delta \geqslant \alpha$ there exists $\gamma \in I$ such that $\gamma \geqslant \delta$ and $\gamma \geqslant \beta$, so that $f_{\alpha\gamma}(A_\gamma) \subset f_{\alpha\delta}(A_\delta)$ and consequently

$$\bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma) = \bigcap_{\delta \geqslant \alpha} f_{\alpha\delta}(A_\delta) = A'_\alpha.$$

Hence $\mathfrak{A}'$ satisfies (21) and therefore belongs to $\Sigma$. Since $A'_\alpha \subset A_\alpha$ for all $\alpha$, the maximality of $\mathfrak{A}$ in $\Sigma$ implies $\mathfrak{A}' = \mathfrak{A}$, and our assertion is proved.

(3) We shall establish next that if $\mathfrak{A} = (A_\alpha)$ is a *maximal* element of $\Sigma$, then each of the $A_\alpha$ *consists of a single element*. Let $x_\alpha \in A_\alpha$. For each $\beta \geqslant \alpha$, put $B_\beta = A_\beta \cap \overset{-1}{f}_{\alpha\beta}(x_\alpha)$; if $\beta$ is not $\geqslant \alpha$, put $B_\beta = A_\beta$; then we shall see that $\mathfrak{B} = (B_\beta)$ belongs to $\Sigma$. If $\beta$ is not $\geqslant \alpha$, the relation $\beta \leqslant \gamma$ implies $f_{\beta\gamma}(B_\gamma) \subset f_{\beta\gamma}(A_\gamma) \subset A_\beta = B_\beta$. If, on the other hand, $\alpha \leqslant \beta \leqslant \gamma$, then since

$$\overset{-1}{f}_{\alpha\gamma}(x_\alpha) = \overset{-1}{f}_{\beta\gamma}(\overset{-1}{f}_{\alpha\beta}(x_\alpha)),$$

we have

$$f_{\beta\gamma}(\overset{-1}{f}_{\alpha\gamma}(x_\alpha)) \subset \overset{-1}{f}_{\alpha\beta}(x_\alpha),$$

and since $f_{\beta\gamma}(A_\gamma) \subset A_\beta$, we again have $f_{\beta\gamma}(B_\gamma) \subset B_\beta$, so that the family $\mathfrak{B}$ satisfies (21). Since $A_\alpha = f_{\alpha\beta}(A_\beta)$ whenever $\alpha \leqslant \beta$ by part (2) of the

proof, it is clear that $\mathrm{B}_\beta \neq \emptyset$ for all $\beta \in \mathrm{I}$. Finally, by virtue of (i) and (iii), we have $\mathrm{B}_\beta \in \mathfrak{S}_\beta$ for all $\beta \in \mathrm{I}$, and hence $\mathfrak{B} \in \Sigma$. Since $\mathrm{B}_\beta \subset \mathrm{A}_\beta$ for all $\beta \in \mathrm{I}$, the maximality of $\mathfrak{A}$ implies that $\mathrm{B}_\beta = \mathrm{A}_\beta$ for all $\beta$, and in particular $\mathrm{A}_\alpha = \{x_\alpha\}$.

(4) We are now in a position to prove Theorem 1. Let us start with (a). We have

$$f_\alpha(\mathrm{E}) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

Conversely, let

$$x_\alpha \in \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta),$$

and put

$$\mathrm{B}_\beta = \overset{-1}{f}_{\alpha\beta}(x_\alpha)$$

if $\beta \geqslant \alpha$, and $\mathrm{B}_\beta = \mathrm{E}_\beta$ otherwise. By the definition of $x_\alpha$, the $\mathrm{B}_\beta$ are non-empty, and we have $\mathrm{B}_\beta \in \mathfrak{S}_\beta$ for all $\beta \in \mathrm{I}$ by virtue of (iii) and (i); moreover, it is evident that $f_{\beta\gamma}(\mathrm{B}_\gamma) \subset \mathrm{B}_\beta$ whenever $\beta \leqslant \gamma$. Hence $\mathfrak{B} = (\mathrm{B}_\beta) \in \Sigma$. Let $\mathfrak{A} = (\mathrm{A}_\alpha)$ be a maximal element of $\Sigma$ such that $\mathfrak{A} \geqslant \mathfrak{B}$ (the existence of $\mathfrak{A}$ follows from (1) and §2, no. 4, Theorem 2, Corollary 1). Since, by (3), $\mathrm{A}_\beta$ is of the form $\{y_\beta\}$ for all $\beta \in \mathrm{I}$, it follows that $y = (y_\beta)$ belongs to E, and $f_\alpha(y) = y_\alpha = x_\alpha$ by definition.

Finally, (a) implies (b). We may as well assume that I is not empty (otherwise there is nothing to prove). The hypothesis that the $\mathrm{E}_\alpha$ are non-empty implies that $f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$ for all $\beta \geqslant \alpha$. Since the $f_{\alpha\beta}(\mathrm{E}_\beta)$, for fixed $\alpha$ and variable $\beta \geqslant \alpha$, form a left directed set of subsets of $\mathrm{E}_\alpha$ belonging to $\mathfrak{S}_\alpha$, condition (ii)$'$ proves that

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset.$$

Hence $f_\alpha(\mathrm{E}) \neq \emptyset$ by (a), and *a fortiori* $\mathrm{E} \neq \emptyset$. Q.E.D.

#### Remark {#ens-iii-s7-n4-rem-1 .statement tag=03OJ}

Suppose that condition (iii) in Theorem 1 is replaced by the following weaker condition :

(iii)$'$ *For each* $\alpha \in \mathrm{I}$ *and each non-empty set* $\mathrm{M}_\alpha \in \mathfrak{S}_\alpha$ *there exists* $x_\alpha \in \mathrm{M}_\alpha$ *such that* $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ *for each* $\beta \geqslant \alpha$.

Then the conclusion (b) of Theorem 1 remains valid; the proofs of parts (1) and (2) of Theorem 1 remain unchanged and the proof of part (3) remains valid provided that we are careful to take $x_\alpha \in \mathrm{A}_\alpha$ such that $\overset{-1}{f}_{\alpha\beta}(x_\alpha)$ belongs to $\mathfrak{S}_\beta$ for all $\beta \geqslant \alpha$. Finally, the proof of (4) shows that if

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$$

and if we choose an $x_\alpha$ in this set such that $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ whenever $\beta \geqslant \alpha$, there exists $y \in E$ such that $f_\alpha(y) = x_\alpha$, which proves our assertion.

*Examples*

#### Example 1 {#ens-iii-s7-n4-exa-1 .statement tag=03TK}

If the $E_\alpha$ are *finite* sets, Theorem 1 can be applied by taking $\mathfrak{S}_\alpha$ to be the set of *all* subsets of $E_\alpha$. \* This example is generalized in *General Topology* to the situation in which the $E_\alpha$ are *compact* topological spaces, the $f_{\alpha\beta}$ *continuous* maps, and $\mathfrak{S}_\alpha$ the set of *closed* subsets of $E_\alpha$ (*General Topology*, Chapter I, § 9, no. 6). \*

#### Example 2 {#ens-iii-s7-n4-exa-2 .statement tag=03TL}

Let A be a ring with an identity element, and for each $\alpha \in I$ let $T_\alpha$ be an *Artinian* left A-module. Let $E_\alpha$ be a *homogeneous space* for $T_\alpha$ on which $T_\alpha$ operates faithfully (so that $E_\alpha$ is an *affine space* attached to $T_\alpha$). For $\beta \geqslant \alpha$, suppose that $f_{\alpha\beta} : E_\beta \to E_\alpha$ is an *affine mapping*. Take $\mathfrak{S}_\alpha$ to be the set consisting of the empty set and the *affine linear varieties* in $E_\alpha$. Then condition (i) is trivially satisfied, and (ii) follows from the fact that $T_\alpha$ is Artinian; for this implies that there exists a minimal element in the set of finite intersections of sets $M \in \mathfrak{F}$, and this minimal element must be equal to $\bigcap_{M \in \mathfrak{F}} M$. Finally, since $f_{\alpha\beta}$ is affine, conditions (iii) and (iv) are trivially satisfied. \*

### 5. DIRECT LIMITS

Let I be a (*right*) *directed* preordered set and let $(E_\alpha)_{\alpha \in I}$ be a family of sets indexed by I. For each pair $(\alpha, \beta)$ of elements of I such that $\alpha \leqslant \beta$, let $f_{\beta\alpha}$ be a *mapping of* $E_\alpha$ *into* $E_\beta$. Suppose that the $f_{\beta\alpha}$ satisfy the following conditions :

(LI$_\mathrm{I}$)  *The relations* $\alpha \leqslant \beta \leqslant \gamma$ *imply* $f_{\gamma\alpha} = f_{\gamma\beta} \circ f_{\beta\alpha}$.
(LI$_\mathrm{II}$)  *For each* $\alpha \in I, f_{\alpha\alpha}$ *is the identity mapping of* $E_\alpha$.

Let G be the set which is the *sum* of the family of sets $(E_\alpha)_{\alpha \in I}$ (Chapter II, § 4, no. 8); by abuse of language, we shall identify the $E_\alpha$ with their canonical images in G, and for each $x \in G$ we shall denote by $\lambda(x)$ the unique index $\alpha \in I$ such that $x \in E_\alpha$. Let $R\{x, y\}$ denote the following relation between two elements $x$, $y$ of G : "there exists an element $\gamma \in I$ such that $\gamma \geqslant \alpha = \lambda(x)$ and $\gamma \geqslant \beta = \lambda(y)$ for which $f_{\gamma\alpha}(x) = f_{\gamma\beta}(y)$". Then R is an *equivalence relation on* G. It is clear that R is reflexive and symmetric on G. To show that R is transitive, let $x \in E_\alpha, y \in E_\beta, z \in E_\gamma$, and suppose that there exist $\lambda \in I$ such that $\lambda \geqslant \alpha$, $\lambda \geqslant \beta$ and $f_{\lambda\alpha}(x) = f_{\lambda\beta}(y)$, and $\mu \in I$ such that $\mu \geqslant \beta$, $\mu \geqslant \gamma$, and $f_{\mu\beta}(y) = f_{\mu\gamma}(z)$. Since I is a directed set, there exists $\nu \in I$ such that $\nu \geqslant \lambda$ and $\nu \geqslant \mu$;

by $(\mathrm{LI_I})$ we then have

$$f_{\nu\alpha}(x) = f_{\nu\lambda}(f_{\lambda\alpha}(x)) = f_{\nu\lambda}(f_{\lambda\beta}(y)) = f_{\nu\beta}(y)$$
$$= f_{\nu\mu}(f_{\mu\beta}(y)) = f_{\nu\mu}(f_{\mu\gamma}(z)) = f_{\nu\gamma}(z),$$

which establishes our assertion. The quotient set $\mathrm{E} = \mathrm{G/R}$ is called the *direct limit of the family* $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ *with respect to the family of mappings* $(f_{\beta\alpha})$, and is written $\mathrm{E} = \varinjlim (\mathrm{E}_\alpha, f_{\beta\alpha})$, or simply $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ when there is no risk of ambiguity. By abuse of language, the pair $((\mathrm{E}_\alpha), (f_{\beta\alpha}))$ (which is usually written $(\mathrm{E}_\alpha, f_{\beta\alpha})$) is called a *direct system of sets*, relative to the directed set I.

¶ Clearly E is not empty provided at least one of the $\mathrm{E}_\alpha$ is not empty. We denote by $f_\alpha$ the restriction to $\mathrm{E}_\alpha$ of the canonical mapping $f$ of G onto $\mathrm{E} = \mathrm{G/R}$; $f_\alpha$ is called the *canonical mapping* of $\mathrm{E}_\alpha$ into E. If $\alpha \leqslant \beta$, we have the relation

(22) $$f_\beta \circ f_{\beta\alpha} = f_\alpha$$

since for each $x \in \mathrm{E}_\alpha$ we have $f_{\beta\beta}(f_{\beta\alpha}(x)) = f_{\beta\alpha}(x)$ by $(\mathrm{LI_I})$; and therefore the elements $x \in \mathrm{E}_\alpha$ and $f_{\beta\alpha}(x) \in \mathrm{E}_\beta$ are congruent mod R.

*Examples*

#### Example 1 {#ens-iii-s7-n5-exa-1 .statement tag=03TM}

Let A, B be two sets, and let $(\mathrm{V}_\alpha)_{\alpha \in \mathrm{I}}$ be a family of subsets of A whose index set I is directed, and such that the relation $\alpha \leqslant \beta$ implies $\mathrm{V}_\beta \subset \mathrm{V}_\alpha$. Let $\mathrm{E}_\alpha$ denote the set of all mappings of $\mathrm{V}_\alpha$ into B, and for each pair of indices $(\alpha, \beta)$ such that $\alpha \leqslant \beta$ let $f_{\beta\alpha}$ be the mapping of $\mathrm{E}_\alpha$ into $\mathrm{E}_\beta$ which sends each function $u \in \mathrm{E}_\alpha$ to its *restriction* to $\mathrm{V}_\beta$. It is obvious that the conditions $(\mathrm{LI_I})$ and $(\mathrm{LI_{II}})$ are satisfied, and the set $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ is called the set of *germs of mappings* of the $\mathrm{V}_\alpha$ into B. \* The most frequent case is that in which $(\mathrm{V}_\alpha)$ is the family of *neighbourhoods* of a subset of a topological space A (*General Topology*, Chapter I, §6, no. 10). \*

#### Example 2 {#ens-iii-s7-n5-exa-2 .statement tag=03TN}

Suppose that, for each $\alpha \in \mathrm{I}$, $\mathrm{E}_\alpha$ is the same set F and that whenever $\alpha \leqslant \beta$, $f_{\beta\alpha}$ is the identity mapping of F onto itself. Then there exists a *canonical bijection* of $\varinjlim \mathrm{E}_\alpha$ onto F. In order to define $\varinjlim \mathrm{E}_\alpha$, we have to form the set G which is the sum of the family $(\mathrm{E}_\alpha)$; G is therefore the union of a family $(\mathrm{G}_\alpha)$ of mutually disjoint sets, and for each $\alpha \in \mathrm{I}$ there is a canonical bijection $h_\alpha : \mathrm{F} \to \mathrm{G}_\alpha$. We have next to consider the equivalence relation R on G corresponding to the partition $(\mathrm{P}_y)_{y \in \mathrm{F}}$, where $\mathrm{P}_y$ is the set of all $h_\alpha(y)$ as $\alpha$ runs through I. Clearly $y \to \mathrm{P}_y$ is a bijection whose inverse is the bijection required. We shall identify F with $\varinjlim \mathrm{E}_\alpha$ by means of this canonical bijection.

#### Lemma 1 {#ens-iii-s7-lem-1 .statement tag=03OK}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *be a direct system of sets,* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *its direct limit, and for each* $\alpha \in \mathrm{I}$ *let* $f_\alpha \colon \mathrm{E}_\alpha \to \mathrm{E}$ *the canonical mapping.*

(i) *Let $(x^{(i)})_{1 \leqslant i \leqslant n}$ be a finite system of elements of* E. *Then there exists* $\alpha \in I$ *and a finite system* $(x_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *of elements of* $E_\alpha$ *such that* $x^{(i)} = f_\alpha(x_\alpha^{(i)})$ *for* $1 \leqslant i \leqslant n$.

(ii) *Let* $(y_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *be a finite system of elements of some* $E_\alpha$. *If* $f_\alpha(y_\alpha^{(i)}) = f_\alpha(y_\alpha^{(j)})$ *for each pair of indices* $(i, j)$, *then there exists* $\beta \geqslant \alpha$ *such that* $f_{\beta\alpha}(y_\alpha^{(i)}) = f_{\beta\alpha}(y_\alpha^{(j)})$ *for each pair* $(i, j)$.

(i) By the definition of E there exists for each $i$ an index $\beta_i \in I$ and an element $z_{\beta_i} \in E_{\beta_i}$ such that $x^{(i)} = f_{\beta_i}(z_{\beta_i})$. Take $\alpha$ such that $\alpha \geqslant \beta_i$ for $1 \leqslant i \leqslant n$, and $x_\alpha^{(i)} = f_{\alpha\beta_i}(z_{\beta_i})$.

(ii) By the definition of E, for each pair $(i, j)$ there exists $\gamma_{ij} \in I$ such that $\gamma_{ij} \geqslant \alpha$ and $f_{\gamma_{ij}\alpha}(y_\alpha^{(i)}) = f_{\gamma_{ij}\alpha}(y_\alpha^{(j)})$. Take $\beta$ such that $\beta \geqslant \gamma_{ij}$ for all pairs $(i, j)$, and use the relations $f_{\beta\alpha} = f_{\beta\gamma_{ij}} \circ f_{\gamma_{ij}\alpha}$.

### 6. DIRECT SYSTEMS OF MAPPINGS

#### Proposition 6 {#ens-iii-s7-prop-6 .statement tag=03RR}

*Let* I *be a directed set, let* $(E_\alpha, f_{\beta\alpha})$ *be a direct system of sets relative to* I, *let* $E = \varinjlim E_\alpha$ *be the direct limit, and for each* $\alpha \in I$ *let*

$$f_\alpha : E_\alpha \to E$$

*be the canonical mapping. For each* $\alpha \in I$, *let* $u_\alpha$ *be a mapping of* $E_\alpha$ *into a set* F *such that*

(23) $$u_\beta \circ f_{\beta\alpha} = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta.$$

*Then:*

(a) *There exists a unique mapping* $u$ *of* E *into* F *such that*

(24) $$u_\alpha = u \circ f_\alpha \qquad \textit{for all } \alpha \in I.$$

(b) $u$ *is surjective if and only if* F *is the union of the sets* $u_\alpha(E_\alpha)$.

(c) $u$ *is injective if and only if for each* $\alpha \in I$ *the relations* $x \in E_\alpha$, $y \in E_\alpha$, $u_\alpha(x) = u_\alpha(y)$ *imply that there exists* $\beta \geqslant \alpha$ *such that* $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$.

(a) With the notation of no. 5, let $v$ be the mapping of G into F which agrees with $u_\alpha$ on $E_\alpha$ for each $\alpha \in I$ (Chapter II, § 4, no. 7, Proposition 8). The hypothesis implies that $v$ is compatible with the equivalence relation R (Chapter II, § 6, no. 5); hence there exists a unique mapping $u$ of $E = G/R$ into F such that $v = u \circ f$ (*loc. cit.*).

(b) Since E is the union of the $f_\alpha(E_\alpha)$, the relation $F = \bigcup_{\alpha \in I} u_\alpha(E_\alpha)$ is clearly necessary and sufficient for $u$ to be surjective.

(c) By Lemma 1 of no. 5 any two elements of $\mathbf{E}$ can always be written in the form $f_\alpha(x)$ and $f_\alpha(y)$, where $x \in \mathrm{E}_\alpha$ and $y \in \mathrm{E}_\alpha$, for a suitable choice of $\alpha \in \mathrm{I}$. It follows also from the lemma that the relation $f_\alpha(x) = f_\alpha(y)$ is equivalent to the existence of $\beta \geqslant \alpha$ such that $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$. Since $u_\alpha(x) = u(f_\alpha(x))$ and $u_\alpha(y) = u(f_\alpha(y))$, this completes the proof.

¶ If the mapping $u$ is *bijective*, it is sometimes said, by abuse of language, that F is the direct limit of the family $(\mathrm{E}_\alpha)$.

#### Remark {#ens-iii-s7-n6-rem-1 .statement tag=03OL}

Suppose that each of the mappings $f_{\beta\alpha}$ is *injective*. Then each of the $f_\alpha$ is *injective*, by the definition of the relation R. In this case we generally identify $\mathrm{E}_\alpha$ and $f_\alpha(\mathrm{E}_\alpha)$ and consider E therefore as the *union* of the $\mathrm{E}_\alpha$. Conversely, let $(\mathrm{F}_\alpha)_{\alpha \in \mathrm{I}}$ be an increasing family of subsets of a set F and suppose that F is the *union* of this family. If $j_{\beta\alpha}$ denotes the canonical injection of $\mathrm{F}_\alpha$ into $\mathrm{F}_\beta$ for $\alpha \leqslant \beta$, then it follows from Proposition 6 that we may identify F with the direct limit of the family $\mathrm{F}_\alpha$ with respect to the family of mappings $(j_{\beta\alpha})$, and the canonical mapping of $\mathrm{F}_\alpha$ into $\varinjlim \mathrm{F}_\alpha$ with the canonical injection of $\mathrm{F}_\alpha$ into F, for each $\alpha \in \mathrm{I}$.

#### Corollary 1 {#ens-iii-s7-prop-6-cor-1 .statement tag=03RS}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *and* $(\mathrm{F}_\alpha, g_{\beta\alpha})$ *be two direct systems of sets relative to the same index set* I; *let* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{F} = \varinjlim \mathrm{F}_\alpha$, *and for each* $\alpha \in \mathrm{I}$ *let* $f_\alpha$ (*resp.* $g_\alpha$) *be the canonical mapping of* $\mathrm{E}_\alpha$ (*resp.* $\mathrm{F}_\alpha$) *into* E (*resp.* F). *For each* $\alpha \in \mathrm{I}$ *let* $u_\alpha$ *be a mapping of* $\mathrm{E}_\alpha$ *into* $\mathrm{F}_\alpha$ *such that, whenever* $\alpha \leqslant \beta$, *the diagram*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_{\beta\alpha}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\beta\alpha}} \\ \mathrm{E}_\beta & \underset{u_\beta}{\longrightarrow} & \mathrm{F}_\beta \end{array}$$

*is commutative. Then there exists a unique mapping* $u : \mathrm{E} \rightarrow \mathrm{F}$ *such that, for each* $\alpha \in \mathrm{I}$, *the diagram*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ \mathrm{E} & \underset{u}{\longrightarrow} & \mathrm{F} \end{array}$$

*is commutative.*

Put $v_\alpha = g_\alpha \circ u_\alpha$. If $\alpha \leqslant \beta$, then by (22) we have

$$v_\beta \circ f_{\beta\alpha} = g_\beta \circ u_\beta \circ f_{\beta\alpha} = g_\beta \circ g_{\beta\alpha} \circ u_\alpha = g_\alpha \circ u_\alpha = v_\alpha.$$

We may therefore apply Proposition 6 to the mappings $v_\alpha$, whence the existence and uniqueness of a mapping $u : \mathrm{E} \to \mathrm{F}$ such that

$$u \circ f_\alpha = v_\alpha = g_\alpha \circ u_\alpha$$

for all $\alpha \in \mathrm{I}$.

¶ A family of mappings $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$ which satisfies the conditions of Corollary 1 is called a *direct system of mappings* of $(\mathrm{E}_\alpha, f_{\beta\alpha})$ into $(\mathrm{F}_\alpha, g_{\beta\alpha})$. The mapping defined in Corollary 1 is called the *direct limit* of the family $(u_\alpha)$ and is written $u = \varinjlim u_\alpha$ when there is no risk of ambiguity.

#### Corollary 2 {#ens-iii-s7-prop-6-cor-2 .statement tag=03RT}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$, $(\mathrm{F}_\alpha, g_{\beta\alpha})$, $(\mathrm{G}_\alpha, h_{\beta\alpha})$ *be three direct systems of sets relative to* I. *Let* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{F} = \varinjlim \mathrm{F}_\alpha$, $\mathrm{G} = \varinjlim \mathrm{G}_\alpha$, *and let* $f_\alpha$ *(resp.* $g_\alpha$, $h_\alpha$*) be the canonical mapping of* $\mathrm{E}_\alpha$ *(resp.* $\mathrm{F}_\alpha$, $\mathrm{G}_\alpha$*) into* E *(resp.* F, G*). If* $(u_\alpha)$ *and* $(v_\alpha)$ *are two direct systems of mappings* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$, $v_\alpha : \mathrm{F}_\alpha \to \mathrm{G}_\alpha$, *then the mappings* $v_\alpha \circ u_\alpha : \mathrm{E}_\alpha \to \mathrm{G}_\alpha$ *form a direct system of mappings, and we have*

(25) $$\varinjlim (v_\alpha \circ u_\alpha) = (\varinjlim v_\alpha) \circ (\varinjlim u_\alpha).$$

For if we put $w_\alpha = v_\alpha \circ u_\alpha$, then for $\alpha \leqslant \beta$ we have

$$h_{\beta\alpha} \circ w_\alpha = (h_{\beta\alpha} \circ v_\alpha) \circ u_\alpha = (v_\beta \circ g_{\beta\alpha}) \circ u_\alpha = v_\beta \circ (u_\beta \circ f_{\beta\alpha}) = w_\beta \circ f_{\beta\alpha},$$

which shows that $(w_\alpha)$ is a direct system of mappings. Furthermore, if $u = \varinjlim u_\alpha$ and $v = \varinjlim v_\alpha$, then for all $\alpha \in \mathrm{I}$ we have

$$(v \circ u) \circ f_\alpha = v \circ (g_\alpha \circ u_\alpha) = h_\alpha \circ (v_\alpha \circ u_\alpha),$$

and by virtue of the uniqueness of the direct limit, we have $v \circ u = \varinjlim w_\alpha$.

#### Proposition 7 {#ens-iii-s7-prop-7 .statement tag=03RU}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *and* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *be two direct systems of sets relative to* I, *and for each* $\alpha \in \mathrm{I}$ *let* $u_\alpha$ *be a mapping of* $\mathrm{E}_\alpha$ *into* $\mathrm{E}'_\alpha$ *such that the* $u_\alpha$ *form a direct system of mappings. Let* $u = \varinjlim u_\alpha$. *If each* $u_\alpha$ *is injective* (resp. *surjective*) *then* $u$ *is injective* (resp. *surjective*).

Let $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$, and let $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$, $f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ be the canonical mappings. Suppose that each $u_\alpha$ is injective. To show that $u$ is injective it is enough, by Proposition 6, to verify that if $x \in \mathrm{E}_\alpha$ and $y \in \mathrm{E}_\alpha$ are such that $f'_\alpha(u_\alpha(x)) = f'_\alpha(u_\alpha(y))$, then there exists $\beta \geqslant \alpha$ such that $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$. Now the hypothesis implies (no. 6, Lemma 1) that there exists $\beta \geqslant \alpha$ such that

$$f'_{\beta\alpha}(u_\alpha(x)) = f'_{\beta\alpha}(u_\alpha(y)), \qquad \text{i.e.,} \qquad u_\beta(f_{\beta\alpha}(x)) = u_\beta(f_{\beta\alpha}(y)),$$

and hence $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ since $u_\beta$ is injective.

Now suppose that the $u_\alpha$ are surjective. Then we have

$$\mathrm{E}' = \bigcup_\alpha f'_\alpha(\mathrm{E}'_\alpha) = \bigcup_\alpha f'_\alpha(u_\alpha(\mathrm{E}_\alpha)) = \bigcup_\alpha u(f_\alpha(\mathrm{E}_\alpha)) = u\Big(\bigcup_\alpha f_\alpha(\mathrm{E}_\alpha)\Big) = u(\mathrm{E}).$$

With the notation of Proposition 7, let $\mathrm{M}_\alpha$ be a subset of $\mathrm{E}_\alpha$ for each $\alpha \in \mathrm{I}$; if we have $f_{\beta\alpha}(\mathrm{M}_\alpha) \in \mathrm{M}_\beta$ whenever $\alpha \leqslant \beta$, the family $(\mathrm{M}_\alpha)_{\alpha \in \mathrm{I}}$ is said to be a *direct system of subsets of the* $\mathrm{E}_\alpha$. Let $g_{\beta\alpha}$ (where $\alpha \leqslant \beta$) be the mapping of $\mathrm{M}_\alpha$ into $\mathrm{M}_\beta$ whose graph is the same as that of the restriction of $f_{\beta\alpha}$ to $\mathrm{M}_\alpha$. Then it is clear that $(\mathrm{M}_\alpha, g_{\beta\alpha})$ is a direct system of sets; and Proposition 7, applied to the canonical injections $j_\alpha : \mathrm{M}_\alpha \to \mathrm{E}_\alpha$, allows us to *identify* $\mathrm{M} = \varinjlim \mathrm{M}_\alpha$ with a subset of E by means of the injection $j = \varinjlim j_\alpha$.

#### Corollary {#ens-iii-s7-n6-cor-1 .statement tag=03ON}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *and* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *be two direct systems of sets, let* $(u_\alpha)$ *be a direct system of mappings* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'_\alpha$, *and let* $u = \varinjlim u_\alpha$.

(i) *Let* $(\mathrm{M}_\alpha)$ *be a direct system of subsets of the* $\mathrm{E}_\alpha$. *Then* $(u_\alpha(\mathrm{M}_\alpha))$ *is a direct system of subsets of the* $\mathrm{E}'_\alpha$, *and we have*

(26) $$\varinjlim u_\alpha(\mathrm{M}_\alpha) = u\,(\varinjlim \mathrm{M}_\alpha).$$

(ii) *Let* $(a'_\alpha)_{\alpha \in \mathbf{I}}$ *be a family such that* $a'_\alpha \in \mathrm{E}'_\alpha$ *for each* $\alpha \in \mathrm{I}$ *and* $f'_{\beta\alpha}(a'_\alpha) = a'_\beta$ *whenever* $\alpha \leqslant \beta$. *Then the sets* $\overset{-1}{u}_\alpha(a'_\alpha)$ *form a direct system of subsets of the* $\mathrm{E}_\alpha$, *and we have*

(27) $$\varinjlim \overset{-1}{u}_\alpha(a'_\alpha) = \overset{-1}{u}(a'),$$

*where* $a'$ *is the unique element of* $\varinjlim \mathrm{E}'_\alpha$ *which is the canonical image of* $a'_\alpha$ *for each* $\alpha \in \mathrm{I}$.

(i) It is evident that the $u_\alpha(\mathrm{M}_\alpha)$ form a direct system of subsets of the $\mathrm{E}'_\alpha$, and we may write $u_\alpha(\mathrm{M}_\alpha) = v_\alpha(\mathrm{M}_\alpha)$, where $v_\alpha$ is the mapping of $\mathrm{M}_\alpha$ onto $u_\alpha(\mathrm{M}_\alpha)$ whose graph is the same as that of the restriction of $u_\alpha$ to $\mathrm{M}_\alpha$. The formula (26) then follows from Proposition 7 because the $v_\alpha$ are surjective.

(ii) Let $\mathrm{N}_\alpha = \overset{-1}{u}_\alpha(a'_\alpha)$. If $\alpha \leqslant \beta$ and $x_\alpha \in \mathrm{N}_\alpha$, then

$$u_\beta(f_{\beta\alpha}(x_\alpha)) = f'_{\beta\alpha}(u_\alpha(x_\alpha) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta;$$

hence $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$, and the $\mathrm{N}_\alpha$ therefore form a direct system of subsets of the $\mathrm{E}_\alpha$. With the notation of the proof of Proposition 7, consider an element $x \in \varinjlim \mathrm{N}_\alpha$. There exists $\alpha \in \mathrm{I}$ and $x_\alpha \in \mathrm{N}_\alpha$ such that $x = f_\alpha(x_\alpha)$, so that $u(x) = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha) = a'$. Conversely, if

$x \in \overset{-1}{u}(a')$ and if $x = f_\alpha(x_\alpha)$ for some $\alpha \in \mathrm{I}$ and some $x_\alpha \in \mathrm{E}_\alpha$, then we have $a' = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha)$. Hence (no. 5, Lemma 1) there exists $\beta \geqslant \alpha$ such that $f'_{\beta\alpha}(u'_\alpha(x_\alpha)) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta$; i.e., $u_\alpha(f_{\beta\alpha}(x_\alpha)) = a'_\beta$, and therefore $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$. Since $x = f_\beta(f_{\beta\alpha}(x_\alpha))$, it follows that $x \in \varinjlim \mathrm{N}_\alpha$.

#### Remark {#ens-iii-s7-n6-rem-2 .statement tag=03OO}

Suppose that, for each $\alpha \in \mathrm{I}$, $u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'$ is a mapping such that the family $(u_\alpha)$ satisfies (23). Consider the direct system $(\mathrm{E}_\alpha, i_{\beta\alpha})$ relative to I, where $\mathrm{E}'_\alpha = \mathrm{E}'$ for all $\alpha \in \mathrm{I}$, and $i_{\beta\alpha}$ is the identity mapping of $\mathrm{E}'$. Then (no. 5, Example 2) $\mathrm{E}'$ can be identified canonically with $\varinjlim \mathrm{E}'_\alpha$. If $u_\alpha$ is considered as a mapping of $\mathrm{E}_\alpha$ into $\mathrm{E}'_\alpha$, then $(u_\alpha)$ is a direct system of mappings, and the mapping $u : \mathrm{E} \to \mathrm{E}'$ defined by (24) is identified with the direct limit of this system of mappings. Hence, by abuse of language, we write $u = \varinjlim u_\alpha$.

If J is a subset of I which is directed (with respect to the induced pre-ordering), it is clear that the pair consisting of the subfamily $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$ and the family $(f_{\beta\alpha})$, where $\alpha \leqslant \beta$ and $\alpha \in \mathrm{J}$ and $\beta \in \mathrm{J}$, is a direct system of sets relative to J; it is said to be obtained by *restricting* the index set to J. Let E, E′ respectively denote the direct limits of the families $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ and $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$, and for each $\alpha \in \mathrm{I}$ let $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$ denote the canonical mapping. Then $(f_\alpha)_{\alpha \in \mathrm{J}}$ is a direct system of mappings, and consequently $g = \varinjlim f_\alpha$ is a mapping of E′ into E, called *canonical*. Moreover, if J′ is a directed subset of J, if E″ is the direct limit of the family $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}'}$, and if

$$g' : \quad \mathrm{E}'' \to \mathrm{E}' \qquad \text{and} \qquad g'' : \mathrm{E}'' \to \mathrm{E}$$

are the canonical mappings, then it follows immediately from Proposition 6 that

(28) $$g'' = g \circ g'.$$

#### Proposition 8 {#ens-iii-s7-prop-8 .statement tag=03OP}

*Let* I *be a directed set, let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *be a direct system of sets relative to* I, *and let* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *be its direct limit. Let* J *be a cofinal subset of* I *and let* E′ *be the direct limit of the direct system of sets obtained from* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *by restricting the index set to* J. *Then the canonical mapping* $g$ *of* E′ *into* E *is bijective.*

J is necessarily a directed set (§ 1, no. 10). We shall use the criteria of Proposition 6 to show that $g$ is bijective. The condition for injectivity follows immediately from the definitions and from Lemma 1 of no. 5. To show that $g$ is surjective, we note that for each $\alpha \in \mathrm{J}$ we have

$$g(\mathrm{E}_\alpha) = f_\alpha(\mathrm{E}_\alpha).$$

Now, for each $\beta \in I$, there exists $\gamma \in J$ such that $\beta \leqslant \gamma$, from which it follows that $g(E_\gamma) \supset g(f_{\gamma\beta}(E_\beta)) = f_\beta(E_\beta)$. E is therefore the union of the sets $g(E_\alpha)$ as $\alpha$ runs through J.

### 7. DOUBLE DIRECT LIMIT. PRODUCT OF DIRECT LIMITS

Let I, L be two directed sets, and let $I \times L$ be their product (§ 1, no. 4) which, with the product preordering, is again a directed set. Consider a direct system of sets $(E^\lambda_\alpha, f^{\mu\lambda}_{\beta\alpha})$ relative to $I \times L$. We have then

$$(29) \qquad f^{\nu\lambda}_{\gamma\alpha} = f^{\mu\nu}_{\gamma\beta} \circ f^{\mu\lambda}_{\beta\alpha}$$

whenever $\alpha \leqslant \beta \leqslant \gamma$ and $\lambda \leqslant \mu \leqslant \nu$.

Let E or $\varinjlim_{\alpha,\lambda} E^\lambda_\alpha$ denote the direct limit of this direct system. For each $\lambda \in L$ put $g^\lambda_{\beta\alpha} = f^{\lambda\lambda}_{\beta\alpha} : E^\lambda_\alpha \to E^\lambda_\beta$. Then from (29) we have

$$(30) \qquad g^\lambda_{\gamma\alpha} = g^\lambda_{\gamma\beta} \circ g^\lambda_{\beta\alpha} \qquad \text{whenever } \alpha \leqslant \beta \leqslant \gamma;$$

in other words, $(E^\lambda_\alpha, g^\lambda_{\beta\alpha})$ is a direct system of sets relative to I. Let $F^\lambda = \varinjlim_\alpha E^\lambda_\alpha$ denote its direct limit. If $\lambda \leqslant \mu$ are fixed elements of L, it follows from (29) that the mappings $h^{\mu\lambda}_\alpha = f^{\lambda\mu}_{\alpha\alpha} : E^\lambda_\alpha \to E^\mu_\alpha$ form a direct system of mappings. Let $h^{\mu\lambda} = \varinjlim_\alpha h^{\mu\lambda}_\alpha : F^\lambda \to F^\mu$ denote the direct limit of this system of mappings. If $\lambda \leqslant \mu \leqslant \nu$ in L, then

$$(31) \qquad h^{\nu\lambda} = h^{\nu\mu} \circ h^{\mu\lambda}$$

(no. 6, Proposition 6, Corollary 2), and therefore $(F^\lambda, h^{\mu\lambda})$ is a direct system of sets relative to L. Let $F = \varinjlim F^\lambda$ be its direct limit. We shall define a *canonical bijection* $E \to F$. For this purpose, let $g^\lambda_\alpha$ denote the canonical mapping $E^\lambda_\alpha \to F^\lambda$, and $h^\lambda$ the canonical mapping $F^\lambda \to F$, and put $u^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha$. If $\alpha \leqslant \beta$ and $\lambda \leqslant \mu$, then we have

$$\begin{aligned} u^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} &= h^\mu \circ g^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu\mu}_{\beta\alpha} \circ f^{\mu\lambda}_{\alpha\alpha} = h^\mu \circ g^\mu_\alpha \circ f^{\mu\lambda}_{\alpha\alpha} \\ &= h^\mu \circ h^{\mu\lambda} \circ g^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha = u^\lambda_\alpha \end{aligned}$$

from (29) and the definition of the $h^{\mu\lambda}$. Hence the $u^\lambda_\alpha$ form a direct system of mappings relative to $I \times L$. Put $u = \varinjlim_{\alpha,\lambda} u^\lambda_\alpha : E \to F$. We shall show that $u$ is bijective by applying the criteria of no. 6, Proposition 6. In the first place, F is the union of the sets $h^\lambda(F^\lambda)$, and each $F^\lambda$ is the

union of the sets $g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)$; hence F is the union of the sets

$$h^\lambda(g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)) = u_\alpha^\lambda(\mathrm{E}_\alpha^\lambda).$$

Next, let $x$, $y$ be two elements of $\mathrm{E}_\alpha^\lambda$ such that $u_\alpha^\lambda(x) = u_\alpha^\lambda(y)$, i.e., $h^\lambda(g_\alpha^\lambda(x)) = h^\lambda(g_\alpha^\lambda(y))$. Then (no. 5, Lemma 1) there exists $\mu \geqslant \lambda$ such that $h^{\mu\lambda}(g_\alpha^\lambda(x)) = h^{\mu\lambda}(g_\alpha^\lambda(y))$, i.e., $g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$; likewise there exists $\beta \geqslant \alpha$ such that $g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$ (no. 5, Lemma 1), i.e., $f_{\beta\alpha}^{\mu\lambda}(x) = f_{\beta\alpha}^{\mu\lambda}(y)$; and this shows (no. 6, Proposition 6) that $u$ is injective. We have therefore proved :

#### Proposition 9 {#ens-iii-s7-prop-9 .statement tag=03RV}

*If* $(\mathrm{E}_\alpha^\lambda, f_{\beta\alpha}^{\mu\lambda})$ *is a direct system of sets relative to a product* $\mathrm{I} \times \mathrm{L}$ *of two directed sets, then (up to a canonical bijection) we have*

(32)
$$\varinjlim_{\alpha,\ \lambda} \mathrm{E}_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} \mathrm{E}_\alpha^\lambda).$$

#### Corollary {#ens-iii-s7-n7-cor-1 .statement tag=03OQ}

*Let* $(\mathrm{E}'^\lambda_\alpha, f'^{\mu\lambda}_{\beta\alpha})$ *be another direct system of sets relative to* $\mathrm{I} \times \mathrm{L}$, *and for each* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *let* $u_\alpha^\lambda$ *be a mapping of* $\mathrm{E}_\alpha^\lambda$ *into* $\mathrm{E}'^\lambda_\alpha$, *such that the* $u_\alpha^\lambda$ *form a direct system of mappings. Then we have*

(33)
$$\varinjlim_{\alpha,\ \lambda} u_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} u_\alpha^\lambda).$$

We leave the verification to the reader.

#### Proposition 10 {#ens-iii-s7-prop-10 .statement tag=03RW}

*Let* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *and* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *be two direct systems of sets, both relative to the same directed set* I. *Let* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$, $\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$, *and let* $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}, f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ *denote the canonical mappings, for each* $\alpha \in \mathrm{I}$. *Then* $(\mathrm{E}_\alpha \times \mathrm{E}'_\alpha, f_{\beta\alpha} \times f'_{\beta\alpha})$ *is a direct systems of sets,* $(f_\alpha \times f'_\alpha)$ *is a direct system of mappings, and* $\varinjlim (f_\alpha \times f'_\alpha)$ *is a bijection*

(34)
$$\varinjlim (\mathrm{E}_\alpha \times \mathrm{E}'_\alpha) \to (\varinjlim \mathrm{E}_\alpha) \times (\varinjlim \mathrm{E}'_\alpha).$$

The first two assertions of the Proposition are immediately verified. To show that $g = \varinjlim (f_\alpha \times f'_\alpha)$ is bijective, we apply Proposition 6 of no. 6. Clearly $\mathrm{E} \times \mathrm{E}'$ is the union of the sets $f_\alpha(\mathrm{E}_\alpha) \times f'_\alpha(\mathrm{E}'_\alpha)$; hence $g$ is surjective. If $(x, x')$ and $(y, y')$ are two elements of $\mathrm{E}_\alpha \times \mathrm{E}'_\alpha$ such that $f_\alpha(x) = f_\alpha(y)$ and $f'_\alpha(x') = f'_\alpha(y')$, then (no. 5, Lemma 1) there exist two elements $\beta$, $\gamma$ of I such that $\beta \geqslant \alpha$, $\gamma \geqslant \alpha$, and $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$, $f'_{\gamma\alpha}(x') = f'_{\gamma\alpha}(y')$; since I is directed, there exists $\delta \in \mathrm{I}$ such that $\delta \geqslant \beta$ and $\delta \geqslant \gamma$; hence $f_{\delta\alpha}(x) = f_{\delta\alpha}(y)$ and $f'_{\delta\alpha}(x') = f'_{\delta\alpha}(y')$. This completes the proof.

The bijection $g$ is called *canonical*.

#### Corollary {#ens-iii-s7-n7-cor-2 .statement tag=03RX}

*Let* $(\mathrm{F}_\alpha, g_{\beta\alpha})$ *and* $(\mathrm{F}'_\alpha, g'_{\beta\alpha})$ *be two direct systems of sets relative to* I, *and for each* $\alpha \in \mathrm{I}$ *let* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$, $u'_\alpha : \mathrm{E}'_\alpha \to \mathrm{F}'_\alpha$ *be mappings such that* $(u_\alpha)$ *and* $(u'_\alpha)$ *are two direct systems of mappings. Then* $(u_\alpha \times u'_\alpha)$ *is a direct system of mappings, and (up to canonical bijections) we have*

(35) $$\varinjlim (u_\alpha \times u'_\alpha) = (\varinjlim u_\alpha) \times (\varinjlim u'_\alpha).$$

We leave the verification to the reader.

### Exercises {#ens-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).

[^1]: This means that $u_\alpha \circ f_{\alpha\beta} = g_{\alpha\beta} \circ u_\beta$.
