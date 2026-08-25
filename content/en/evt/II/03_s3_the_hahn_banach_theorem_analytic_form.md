---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 3
section_title: The Hahn-Banach Theorem (analytic form)
lang: en
source: evt-i-v
book_pages: TVS II.21-TVS II.23, TVS II.72-TVS II.74
pdf_pages: 0058-0060, 0109-0111
extraction: ocr
subsections:
    - "no": 1
      title: Extension of positive linear forms
      page: 21
      pdf_page: 58
    - "no": 2
      title: The Hahn-Banach theorem (analytic form)
      page: 22
      pdf_page: 59
statements: 6
exercises: 8
content_sha256: a5147d86c2ae43411a7a8933f6c307748cadd54639ce8c502a03286da01e0e92
---

## § 3. THE HAHN-BANACH THEOREM (ANALYTIC FORM)

### 1. Extension of positive linear forms

#### Proposition 1 {#evt-ii-s3-prop-1 .statement}

— Let E be a preordered vector space and V be a vector subspace of E such that every element of E is bounded above by an element of V. Given a linear form f on V that is positive for the preordered vector space structure of V (induced by that of E) there exists a non-empty set $S_f$ of positive linear forms on E, each being an extension of f. If $h \in S_f$ then the values $h(a)$ for $a \in E$ lie in the interval $[\alpha', \alpha'']$, where

$$
\alpha' = \sup_{z \in V, z \leq a} f(z), \quad \alpha'' = \inf_{y \in V, y \geq a} f(y).
$$

I. Special case.

Suppose firstly that $E = V + \mathbf{R}a$. Since the proposition is trivial if $a \in V$, we confine ourselves to the case $a \notin V$. The conditions on V imply that the set $A''$ of $y \in V$ such that $a \leq y$ is not empty; similarly the set $A'$ of $z \in V$ such that $-z \geq -a$ (\emph{i.e.} $z \leq a$) is not empty. For $y \in A''$ and $z \in A'$, we have $z \leq a \leq y$, and thus by hypothesis $f(z) \leq f(y)$. Thus $\alpha', \alpha''$ are finite and $\alpha' \leq \alpha''$. Any linear form $f_1$ on E that extends $f$ is completely determined by $f_1(a)$ and for all $\lambda \in \mathbf{R}$ and all $x \in V$, we have

$$
f_1(x + \lambda a) = f(x) + \lambda f_1(a).
$$

Thus $f_1$ is positive if and only if the relations

$$
x \in V, \quad \lambda \in \mathbf{R}, \quad x + \lambda a \geq 0
$$

imply

$$
f(x) + \lambda f_1(a) \geq 0.
$$

As $f(\mu x) = \mu f(x)$ and the relations $x \geq 0$ and $\mu x \geq 0$ are equivalent for $\mu > 0$, it is sufficient to show that (2) implies (3) in the particular cases $\lambda = 0, \lambda = 1$ and $\lambda = -1$. For $\lambda = 0$, the fact that (2) implies (3) follows from the hypothesis that $f$ is positive. For $\lambda = 1$, to say that (2) implies (3) means that for $-x \in A'$, we have $f_1(a) \geq f(-x)$, \emph{i.e.} $f_1(a) \geq \alpha'$; for $\lambda = -1$, (2) implies (3), means that for $x \in A''$, we have $f(x) \geq f_1(a)$, \emph{i.e.} $f_1(a) \leq \alpha''$. The proposition is therefore proved in this case.

II. General case.

Let $\mathfrak{F}$ be the set of pairs $(W, g)$ where $W$ is a vector subspace of $E$ containing $V$ and $g$ is a positive linear form on $W$ which is an extension of $f$. We order $\mathfrak{F}$ putting $(W, g) \leq (W', g')$ if $W \subset W'$ and if $g'$ is an extension of $g$. Clearly $\mathfrak{F}$ is inductive and by th. 2 of S, III, § 2.4, there is a maximal element $(W_0, g_0)$. Suppose $W_0 \neq E$. Then there exists a vector $b \notin W_0$, and, if $W_1 = W_0 + \mathbf{R}b$, the special case above shows that there exists a positive linear form on $W_1$ which is an extension of $g_0$; this contradicts the hypothesis that $(W_0, g_0)$ is maximal. Thus $W_0 = E$, and the first part of the proposition is proved. When $a \in V$, the second assertion is obviously true with $\alpha' = \alpha'' = f(a)$; if, on the contrary, $a \notin V$ and one puts $V_1 = V + \mathbf{R}a$, the second assertion follows from the special case I of the proof.

#### Corollary {#evt-ii-s3-n1-cor-1 .statement}

In a topological vector space $E$ with a compatible preorder structure, let $P$ be the set of elements $\geq 0$ in $E$. Let $V$ be a vector subspace of $E$ containing at least one interior point $x_0$ of $P$. Then every positive linear form on $V$ can be extended to a positive linear form on $E$.

By prop. 1 it is sufficient to show that for every $x \in E$, there exists $x' \in V$ such that $x' - x \in P$. Now let $U$ be a neighbourhood of $0$ in $E$ such that $x_0 + U \subset P$. Then $x + x_0 + U \subset x + P$, and, hence there exists $\varepsilon$ such that $0 < \varepsilon < 1$ and the point $y = x_0 + (1 - \varepsilon)x$ belongs to $x + P$; then every point of the form $x + \lambda(y - x)$ belongs to $x + P$ for $\lambda > 0$. If we take $\lambda = 1/\varepsilon$, then $x + \lambda(y - x) = \lambda x_0 \in V$, from which the conclusion follows.

The conclusion of the corollary is not necessarily valid if one does not assume that $V$ contains an interior point of $P$, even if $E$ is of finite dimension and if $P \cap V$ contains points interior in $V$ (II, p. 91, exerc. 25, b)).

### 2. The Hahn-Banach theorem (analytic form)

#### Theorem 1 (Hahn-Banach) {#evt-ii-s3-thm-1 .statement}

Let $p$ be a sub-linear function on a vector space $E$. Let $V$ be a vector subspace of $E$ and $f$ a linear form on $V$ such that, for all $y \in V$, we have $f(y) \leq p(y)$. Then there exists a linear form $h$ on $E$ that is an extension of $f$ and such that $h(x) \leq p(x)$ for $x \in E$.

The set of pairs $(x, a)$ such that $p(x) \leq a$ is a convex subset $P$ of the vector space $E_1 = E \times \mathbf{R}$ (II, p. 17, prop. 19), and it is clearly a pointed cone. Let $V_1$ be the subspace $V \times \mathbf{R}$ of $E_1$ and $g(y, a) = -f(y) + a$ for each point $(y, a) \in V_1$. Then $g$ is a positive linear form for the preorder structure on $V_1$ defined by $P \cap V_1$; for if $(y, a) \in P \cap V_1$, then $a \geq p(y) \geq f(y)$, therefore $g(y, a) \geq 0$. Next let $(x, a) \in E_1$; we show that $(x, a)$ is less than a point of $V_1$ for the preorder defined by $P$. If $(x', a') \in V_1$ then $(x, a) \leq (x', a')$ if, and only if, $p(x' - x) \leq a' - a$, taking $a' \geq p(-x) + a$, we see that $(0, a')$ of $V_1$ satisfies the requirements. Thus we can apply prop. I of II, p. 21; there is a linear form $u$ on $E_1$ extending $g$ and positive for the preorder defined by $P$. Therefore $u(0, 1) = g(0, 1) = 1$ and $u$ is of the form $u(x, a) = -h(x) + a$, where $h$ is a linear form on $E$ that extends $f$; further, for all $x \in E$ and all $a \geq p(x)$, we have $h(x) \leq a$, therefore $h(x) \leq p(x)$. Q.E.D.

#### Corollary 1 {#evt-ii-s3-thm-1-cor-1 .statement}

— Let $p$ be a semi-norm on the vector space $E$. Let $V$ be a vector subspace of $E$ and $f$ a linear form on $V$ such that $|f(y)| \leq p(y)$ for all $y \in V$. Then there exists a linear form $h$ defined on $E$ which is an extension of $f$ and is such that $|h(x)| \leq p(x)$ for $x \in E$.

For a semi-norm $q$ and a linear form $g$ on $E$, the relation $g \leq q$ is the same as $|g| \leq q$. The corollary follows from th. 1.

#### Corollary 2 {#evt-ii-s3-thm-1-cor-2 .statement}

— Let $p$ be a semi-norm on the vector space $E$. Given a point $x_0 \in E$, there exists a linear form $f$ defined over $E$, such that $f(x_0) = p(x_0)$ and that $|f(x)| \leq p(x)$ for all $x \in E$.

Apply cor. 1 to the vector subspace, $V$, generated by $x_0$ and to the linear form $\xi x_0 \mapsto \xi p(x_0)$ defined over $V$.

#### Corollary 3 {#evt-ii-s3-thm-1-cor-3 .statement}

— Let $V$ be a vector subspace of the normed space $E$ and let $f$ be a continuous linear form over $V$; then there exists a continuous linear form $h$ defined over $E$ which extends $f$ and is of the same norm (GT, X, § 3.2).

Apply cor. 1, taking $p(x) = \|f\| \cdot \|x\|$, which gives $\|h\| \leq \|f\|$; but clearly $\|h\| \geq \|f\|$, and the corollary follows.

The conclusion of cor. 3 is not necessarily valid for continuous linear mappings of a normed space into an arbitrary normed space (IV, p. 55, exerc. 16, c) and V, p. 65, exerc. 22).

### Exercises {#evt-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
