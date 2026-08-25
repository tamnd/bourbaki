---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 0
section_title: Graphs
appendix: true
lang: en
source: lie-iv-vi
pdf_pages: 0040-0043
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS
      page: 0
      pdf_page: 40
    - "no": 2
      title: CONNECTED COMPONENTS OF A GRAPH
      page: 0
      pdf_page: 40
    - "no": 3
      title: FORESTS AND TREES
      page: 0
      pdf_page: 42
statements: 6
exercises: 0
content_sha256: eac22a0040474678cfb62df408ef3ef6cb1dc27c07113e0e6b8e5da22b5af9c4
---

## APPENDIX
# GRAPHS

### 1. DEFINITIONS

#### Definition 1 {#lie-iv-a0-def-1 .statement}

*A combinatorial graph (or simply a graph, if there is no risk of confusion) is a pair* $(\mathbf{A}, S)$, *where S is a set and A is a subset of $\mathfrak{P}(S)$ consisting of sets with two elements.*

Let $\Gamma = (\mathbf{A}, S)$ be a graph. The elements of $\mathbf{A}$ are called the *edges* and those of S the *vertices* of $\Gamma$; two vertices are said to be *joined* if $\{x, y\}$ is an edge. A vertex is called *terminal* if it is joined to at most one vertex, and a *ramification point* if it is joined to at least three vertices.

In accordance with the general definitions (*Sets R*, §8), an *isomorphism* from the graph $\Gamma$ to a graph $\Gamma' = (\mathbf{A}', S')$ is a bijection from S to S' that takes $\mathbf{A}$ to $\mathbf{A}'$. A graph $\Gamma' = (\mathbf{A}', S')$ is called a *subgraph* of $\Gamma$ if $S' \subset S$ and $\mathbf{A}' \subset \mathbf{A}$; $\Gamma$ is called a *full subgraph* of $\Gamma$ if $S' \subset S$ and $\mathbf{A}' = \mathbf{A} \cap \mathfrak{P}(S)$. It is clear that every subset of S is the set of vertices of exactly one full subgraph of $\Gamma$.

To make the arguments easier to follow, we represent a graph by a diagram having points corresponding to the vertices, two points being joined by a line if and only if the vertices they represent are joined in the graph. For example, the diagram

![Diagram of a graph with vertices a, b, c, d, e and edges {a, b}, {b, c}, {c, d}, {c, e}](https://i.imgur.com/3Q5z5QG.png)

represents a graph whose vertices are $a, b, c, d, e$ and whose edges are $\{a, b\}, \{b, c\}, \{c, d\}$ and $\{c, e\}$.

### 2. CONNECTED COMPONENTS OF A GRAPH

Let $\Gamma = (\mathbf{A}, S)$ be a graph. If $a$ and $b$ are two vertices, a *path* joining $a$ and $b$ is a sequence $(x_0, \ldots, x_n)$ of vertices of $\Gamma$ with $x_0 = a, x_n = b$, the vertices $x_i$ and $x_{i+1}$ being joined for $0 \leq i < n$; the integer $n \geq 0$ is the *length* of the path. The path $(x_0, \ldots, x_n)$ is said to be injective if $x_i \neq x_j$ if $i \neq j$. If a path $(x_0, \ldots, x_n)$ joining $a$ and $b$ is of minimal length among such paths, it is necessarily injective; for if not, there would exist $i$ and $j$ with $0 \leq i < j \leq n$ and $x_i = x_j$ and then the sequence

$$
(x_0, \ldots, x_i, x_{j+1}, \ldots, x_n)
$$

would be a path of length $< n$ joining $a$ and $b$.

The relation "there exists a path joining $a$ and $b$" between two vertices $a$ and $b$ of $\Gamma$ is an equivalence relation $R$ on the set $S$ of vertices. The equivalence classes of $R$ are called the *connected components* of $\Gamma$; and $\Gamma$ is said to be *connected* if $S$ has at most one connected component, that is if any two vertices of $\Gamma$ can be joined by at least one path.

#### Proposition 1 {#lie-iv-a0-prop-1 .statement}

*Let $\Gamma = (A, S)$ be a graph and $(S_\alpha)_{\alpha \in L}$ its family of connected components. Denote by $\Gamma_\alpha$ the full subgraph of $\Gamma$ having $S_\alpha$ as its set of vertices.*

(i) *For any $\alpha$ in $L$, the graph $\Gamma_\alpha$ is connected.*
(ii) *If $\Gamma' = (A', S')$ is a connected subgraph of $\Gamma$, there exists $\alpha$ in $L$ such that $\Gamma' \subset \Gamma_\alpha$.*
(iii) *If $\alpha \neq \beta$, no element of $S_\alpha$ is joined in $\Gamma$ to any element of $S_\beta$ (equivalently, every edge of $\Gamma$ is an edge of one of the $\Gamma_\alpha$).*
(iv) *Let $(S'_\lambda)_{\lambda \in M}$ be a partition of $S$ such that, if $\lambda \neq \mu$, no element of $S'_\lambda$ is joined in $\Gamma$ to any element of $S'_\mu$; then each of the sets $S'_\lambda$ is a union of connected components of $\Gamma$.*

(i) Let $\alpha$ be in $L$ and $a$ and $b$ be in $S_\alpha$. Then there exists a path $c = (x_0, \ldots, x_n)$ joining $a$ and $b$ in $\Gamma$. For any $i$ with $0 \leq i \leq n$, the path $(x_0, \ldots, x_i)$ joins $a$ to $x_i$ in $\Gamma$, so $x_i \in S_\alpha$. Thus, $c$ is a path *in* $\Gamma_\alpha$ joining $a$ and $b$. It follows that $\Gamma_\alpha$ is connected.

(ii) Let $\Gamma' = (A', S')$ be a non-empty connected subgraph of $\Gamma$, let $a$ be an element of $S'$ and let $S_\alpha$ be the connected component of $S$ containing $a$. For any $b$ in $S'$, there exists a path $c$ joining $a$ and $b$ in $\Gamma'$, and *a fortiori* in $\Gamma$. It follows that $S' \subset S_\alpha$.

(iii) Given distinct elements $\alpha$ and $\beta$ of $L$, and vertices $a \in S_\alpha$ and $b \in S_\beta$, there is no path joining $a$ and $b$, and in particular no edge joining $a$ and $b$.

(iv) Let $a$ be in $S'_\lambda$ and let $S_\alpha$ be the connected component of $\Gamma$ containing $a$. Then, for any $b$ in $S_\alpha$, there exists a path $(x_0, \ldots, x_n)$ joining $a$ and $b$ in $\Gamma$. If $i$ is an integer such that $0 \leq i < n$ and if $x_i \in S'_\lambda$, then $x_{i+1} \in S'_\lambda$ since $x_i$ is joined to $x_{i+1}$. It follows by induction that $x_i \in S'_\lambda$ for $0 \leq i \leq n$, and in particular that $b = x_n$ is in $S'_\lambda$. Thus, $S_\alpha \subset S'_\lambda$.

#### Corollary 1 {#lie-iv-a0-prop-1-cor-1 .statement}

*A graph $\Gamma = (A, S)$ is connected if and only if there does not exist a partition $(S', S'')$ of $S$ into two non-empty subsets such that no element of $S'$ is joined in $\Gamma$ to any element of $S''$.*

Suppose that $\Gamma$ is not connected and let $S'$ be one of its connected components. The set $S'' = S - S'$ is non-empty by Prop. 1, (i) and no element of $S'$ is joined to any element of $S''$ by Prop. 1, (iii).

Suppose now that $\Gamma$ is connected and let $(S', S'')$ be a partition with the stated property. By Prop. 1, (iv), the set $S'$ contains at least one connected component, so $S' = S$ and $S'' = \varnothing$, a contradiction.

#### Corollary 2 {#lie-iv-a0-prop-1-cor-2 .statement}

*A subset $S'$ of $S$ is a union of connected components if and only if no vertex belonging to $S'$ is joined to any vertex belonging to $S - S'$.*

The condition is sufficient by Prop. 1, (iv). It is necessary by Prop. 1, (iii).

### 3. FORESTS AND TREES

Let $\Gamma = (A, S)$ be a graph. A *circuit* of $\Gamma$ is a sequence

$$
(x_1, \ldots, x_n)
$$

of distinct vertices of $\Gamma$ such that $n \geq 3$, $x_i$ is joined to $x_{i+1}$ for $1 \leq i < n$ and $x_n$ is joined to $x_1$. $\Gamma$ is called a *forest* if there is no circuit in $\Gamma$; every subgraph of $\Gamma$ is then also a forest. A connected forest is called a *tree*; the connected components of a forest are thus trees.

#### Proposition 2 {#lie-iv-a0-prop-2 .statement}

*Let $\Gamma = (A, S)$ be a forest having only a finite number of vertices.*

(i) *If $\Gamma$ has at least one vertex, it has a terminal vertex.*
(ii) *If $\Gamma$ has at least two vertices, there is a partition $(S', S'')$ of its set of vertices into two non-empty subsets such that two distinct vertices that both belong to $S'$ or both belong to $S''$ are never joined.*

Suppose that $\Gamma$ has at least one vertex and let $(x_0, \ldots, x_n)$ be an injective path of maximal length in $\Gamma$. The vertex $x_0$ cannot be joined to a vertex $y$ distinct from $x_0, x_1, \ldots, x_n$, since otherwise there would exist an injective path in $\Gamma$ of length $n + 1$, namely $(y, x_0, \ldots, x_n)$. The vertex $x_0$ is not joined to any vertex $x_i$ with $2 \leq i \leq n$, since otherwise $(x_0, x_1, \ldots, x_i)$ would be a circuit in the forest $\Gamma$. Thus, $x_0$ is terminal.

We shall prove (ii) by induction of the number $m$ of vertices of $\Gamma$, the case $m = 2$ being trivial. Suppose then that $m \geq 3$ and that assertion (ii) is proved for graphs with $m - 1$ vertices. Let $a$ be a terminal vertex of $\Gamma$ (cf. (i)). We apply the induction hypothesis to the full subgraph of $\Gamma$ whose vertices are the vertices $x \neq a$ of $\Gamma$. Thus, there exist two non-empty disjoint subsets $S'_1$ and $S''_1$ of $S$ with $S'_1 \cup S''_1 = S - \{a\}$, and such that two distinct vertices in $S'_1$ (resp. $S''_1$) are never joined. Since $a$ is joined to at most one vertex of $\Gamma$, we can suppose for example that it is not joined to any vertex in $S'_1$. The partition $(S'_1, S''_1 \cup \{a\})$ then has the required property. Q.E.D.

For any integer $n \geq 1$, denote by $A_n$ the graph whose vertices are the integers $1, 2, \ldots, n$ and whose edges are the pairs $\{i, j\}$ with $i - j = \pm 1$:

$$
\begin{array}{cccccc}
1 & 2 & 3 & n-1 & n \\
\circ & \circ & \circ & \cdots & \circ
\end{array}
$$

A graph $\Gamma$ is said to be a chain of length $m \geq 0$ if it is isomorphic to $A_{m+1}$. This is equivalent to the existence in $\Gamma$ of an injective path $(x_0, \ldots, x_m)$ containing all the vertices, the vertices $x_i$ and $x_j$ not being joined if $|i - j| > 1$.

#### Proposition 3 {#lie-iv-a0-prop-3 .statement}

*A graph is a chain if and only if its number of vertices is finite and non-zero and it is a tree with no ramification point.*

Suppose that the graph $\Gamma$ is a chain $(x_0, \ldots, x_m)$ with the properties listed before the statement of Prop. 3. It is clear that any vertex of $\Gamma$ is joined to at most two vertices. If $i < j$ the path $(x_i, \ldots, x_j)$ extracted from the path $(x_0, \ldots, x_m)$ joins $x_i$ to $x_j$; thus, $\Gamma$ is connected. Finally, let $(x_{p_1}, \ldots, x_{p_n})$ be a circuit in $\Gamma$, and let $p_k$ be the smallest of the distinct integers $p_1, \ldots, p_n$. There exist distinct indices $i$ and $j$ such that $x_{p_k}$ is joined to $x_{p_i}$ and $x_{p_j}$: this follows from the definition of a circuit. Since $p_k < p_i$ and $p_k < p_j$, we necessarily have $p_i = p_j = p_k + 1$, which is a contradiction since $p_1, \ldots, p_n$ are distinct. Thus, there is no circuit in $\Gamma$.

Conversely, let $\Gamma$ be a tree with no ramification point and with a finite non-zero number of vertices, and let $(x_0, \ldots, x_m)$ be an injective path of maximal length in $\Gamma$. Denote by $T$ the set of vertices other than $x_0, \ldots, x_m$. A vertex $b \in T$ cannot be joined to any vertex $x_i$, for we would have either

a) $i = 0$, but then $(b, x_0, \ldots, x_m)$ would be an injective path of length $m + 1$ in $\Gamma$, or
b) $i = m$, but then $(x_0, \ldots, x_m, b)$ would be an injective path of length $m + 1$ in $\Gamma$, or
c) $0 < i < m$, but then $x_i$ would be joined to three distinct vertices $x_{i-1}$, $x_{i+1}$ and $b$.

Since $\Gamma$ is connected, $T$ is empty by Cor. 1 of Prop. 1. Moreover, if there were $i, j$ with $j - i > 1$ and $x_i, x_j$ joined, there would be a circuit $(x_i, x_{i+1}, \ldots, x_j)$ in $\Gamma$. Thus, $\Gamma$ is a chain. Q.E.D.
