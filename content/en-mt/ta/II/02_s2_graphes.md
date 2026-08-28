---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 2
section_title: Graphes
lang: en
source: ta-i-iv-fr
book_pages: TA II.155-TA II.159, TA II.219-TA II.223
pdf_pages: 0171-0175, 0235-0239
extraction: native
subsections:
    - "no": 1
      title: Définition d’un graphe
      page: 155
      pdf_page: 171
    - "no": 2
      title: Orientation d’un graphe
      page: 156
      pdf_page: 172
    - "no": 3
      title: Graphes orientés et carquois
      page: 156
      pdf_page: 172
    - "no": 4
      title: Arbres
      page: 157
      pdf_page: 173
statements: 5
exercises: 12
content_sha256: 2b453f333fdb6d905983651acfc36b7060a9577a4763b395fc05b04e8eb89f0d
translated_from: content/fr/ta/II/02_s2_graphes.md
source_lang: fr
translation_method: machine
source_content_sha256: d6f6affb4b67a412593d410b6a23b13fedad0ca0e860213e6a9b2b8045d76375
translation_model: gpt-5.4
translation_run: translate-en-mt-49a43b8a
glossary_version: 34
glossary_terms_sha256: ae360287c63d2841b1c4bbdbdd7c1c23feb1a3c636769ec08b102e74b7efa51b
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. GRAPHS

### 1. Definition of a graph

#### Definition 1 {#ta-ii-s2-def-1 .statement tag=01SU}

A graph[^1] is a quiver $(S,F, o, t)$ endowed with an involution of F, denoted by $f\mapsto \overline{f}$, without fixed point and such that $t(\overline{f}) =o(f)$ for every $f\in F$.

The quiver $(S,F, o, t)$ is said to underlie this graph. For every arrow $f$ of this quiver, one has, by definition, $\overline{f}=f,\overline{f}=\not f$ and $t(\overline{f}) =$ $o(f)$. Applying this last relation to the arrow $\overline{f}$, one obtains the equality $o(\overline{f}) =t(f)$. The arrow $\overline{f}$ is called the arrow opposite to $f$.

A pair of opposite arrows of the graph is called an edge of the graph. Each of the two arrows belonging to this pair is called an orientation of this edge. For this reason, the arrows of a graph are also called the oriented edges of the graph.

If G and $G'$ are graphs, a graph morphism of G into $G'$ is a quiver morphism $\varphi : G\rightarrow G'$ such that $\varphi (f) =\varphi (\overline{f})$ for every arrow $f$ of G.

Let G and $G'$ be graphs; one says that $G'$ is a subgraph of G if it is a subquiver thereof and if the involution of Fl(G$'$) is the restriction of that of Fl(G).

### 2. Orientation of a graph

Let G be a graph. An orientation of G is a subset A of the set of arrows of G such that $A\cap \overline{A}=\emptyset$ and $A\cup \overline{A}=$ Fl(G).

A graph endowed with an orientation is called an oriented graph.

Let G be an oriented graph and let A be its orientation; an oriented subgraph of G is a subgraph $G'$ of G endowed with the orientation $A'=$ Fl(G$'$)$\cap A$.

Let $(G,A)$ and $(G',A')$ be oriented graphs. An oriented graph morphism of $(G,A)$ into $(G',A')$ is a graph morphism $\varphi : G\rightarrow G'$ such that Fl($\varphi$ )$(A)\subset A'$.

### 3. Oriented graphs and quivers

Let G be a graph, $(S,F, o, t)$ the underlying quiver, and A an orientation of G. Then $(S,A, o|A, t|A)$ is a quiver, called the quiver associated with the oriented graph $(G,A)$.

Conversely, let $C = (S,F, o, t)$ be a quiver. Put $\widetilde{F} = F\times \{-1,1\}$ and let $\widetilde{o},\widetilde{t}$ be the mappings of $\widetilde{F}$ into S defined by

$$
\widetilde{o}(f,1) =o(f)\widetilde{o}(f,-1) =t(f)
$$

$$
\widetilde{t}(f,1) =t(f)\widetilde{t}(f,-1) =o(f)
$$

for $f\in F$. Then $\widetilde{C} = (S,\widetilde{F},\widetilde{o},\widetilde{t})$, endowed with the involution $(f, \varepsilon )\mapsto (f,-\varepsilon )$ of $\widetilde{F}$, is a graph, called the graph associated with the quiver C. The set $A = F\times  \{1\}$ is an orientation of this graph. One says that $(\widetilde{C},A)$ is the oriented graph associated with the quiver C.

If $f$ is an arrow of C, one also says that $(f,1)$ is the oriented edge of $\widetilde{C}$ associated with $f$ and that the pair $\{(f,1),(f,-1)\}$ is the edge of $\widetilde{C}$ associated with $f$.

If $C'$ is a subquiver of C, the oriented graph $\widetilde{C}'$ is an oriented subgraph of $\widetilde{C}$.

There exists a unique quiver morphism $\varphi$ from C into the underlying quiver of $\widetilde{C}$ such that $\varphi (f) = (f,1)$ for every arrow $f$ of G; it is an isomorphism of C onto the quiver associated with the directed graph $(\widetilde{C},A)$.

### 4. Trees

When one speaks of paths, or connected components, of a graph, one means the paths or connected components of the underlying quiver. Two vertices of a graph belong to the same connected component if and only if there exists a path joining them.

Let G be a graph. If $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ is a path in G, the sequence $\overline{c}= (a_n, f_n, . . . , a_1, f_1, a_0)$ is a path in G, called the opposite path to $c$. Let $c$ and $c'$ be juxtaposed paths in G; then $\overline{c'}$ and $\overline{c}$ are juxtaposed, and one has $\overline{c*c'}=\overline{c'}*\overline{c}$.

A path $c$ in G is said to be without backtracking if there exists no pair of consecutive arrows of $c$ which are opposite. Let $c= (a_0, f_1, . . . , f_n, a_n)$ be a path in G joining $a_0$ and $a_n$. If, for an integer $i$ such that $1\leqslant i < n$, the arrows $f_i$ and $f_{i+1}$ are opposite, the path $(a_0, f_1, . . . , a_{i-1}, f_{i+2}, . . . , f_n, a_n)$ is a path in G joining $a_0$ to $a_n$ whose length is strictly less than that of the path $c$. By induction, there therefore exists a path without backtracking in G which joins $a_0$ to $a_n$.

#### Definition 2 {#ta-ii-s2-def-2 .statement tag=01SV}

A forest is a graph in which every loop without backtracking is a constant loop. A tree is a connected forest.

#### Proposition 1 {#ta-ii-s2-prop-1 .statement tag=01SW}

Let G be a graph. Every forest of G is contained in a maximal forest of G; in particular, there exists a maximal forest of G.

In order that a forest of G be maximal, it is necessary and sufficient that the set of its vertices be equal to the set of vertices of G and that its connected components be those of G.

Let $A_0$ be a forest of G. The set of forests of G, endowed with the order relation “A is a subgraph of B”, is inductive. Consequently there exists a maximal forest of G of which $A_0$ is a subgraph (E, III, p. 21, Cor. 1).

The subgraph of G whose set of vertices is Som(G) and whose set of arrows is empty is a forest of G. There therefore exists a maximal forest of G.

Let A be a maximal forest of G. Let us prove that A and G have the same set of vertices. The subgraph of G whose set of vertices is Som(G) and whose set of arrows is Fl(A) is a forest and has A as a subgraph. Hence Som(A) = Som(G).

Let us now prove that A and G have the same connected components. Since an arrow of A is an arrow of G, every connected component of A is contained in a connected component of G. Since A and G have the same set of vertices, it is sufficient to prove that two vertices of G which are in the same connected component of G are in the same connected component of A. If this is not the case, the relation $R_A$, “being in the same connected component of A”, is strictly finer than the relation $R_G$, and there exist two vertices of G which are not in the same connected component of A but which are nevertheless joined by an arrow $f$ of G. Let B be the oriented subgraph of G whose set of vertices is Som(G) and whose set of arrows is Fl(A) $\cup  \{f, f\}$; let us prove that B is a forest of G. Let $c= (a_0, f_1, . . . , f_n, a_n)$ be a non-constant loop without backtracking in B of minimal length. Since A is a forest, the loop $c$ is not a loop in A. Let $i$ (resp. $j$) be the smallest (resp. the largest) integer of $\{0, . . . , n\}$ such that $a_0$ and $a_i$ (resp. $a_j$ and $a_n$) are not in the same connected component of A. This means that the arrows $f_i$ and $f_{j+1}$ are oriented arrows of B associated with the edge $\{f, f\}$ and that they are opposite. Since the loop $c$ is without backtracking, $f_{i+1}=\not\overline{f_i}$, hence $i=\not j$ and the path $(a_i, f_{i+1}, a_{i+1}, . . . , f_j, a_j)$ is a non-constant loop without backtracking in B of length $< n$, contrary to the assumption that $c$ is of minimal length. It follows that B is a forest. This contradicts the assumption that A is a maximal forest of G.

Let now A be a forest of G such that Som(A) = Som(G) and $\pi_0(A) =\pi_0(G)$; let us prove that it is a maximal forest of G. It is enough to prove that, if $f\notin$ Fl(A), the subgraph B of G with set of vertices Som(G) and set of arrows Fl(A) $\cup  \{f, f\}$ is not a forest. By hypothesis, the points $o(f)$ and $t(f)$ are in the same connected component of A; there therefore exists a path $c$ without backtracking in A joining $o(f)$ to $t(f)$. Then the path $c*\overline{f}$ is a nonconstant loop without backtracking in B, which shows that B is not an oriented forest.

#### Corollary {#ta-ii-s2-n4-cor-1 .statement tag=01SX}

A maximal forest of a connected graph is a maximal tree in it.

#### Remark 1 {#ta-ii-s2-n4-rem-1 .statement tag=01SY}

In LIE, IV, p. 33, appendix, the notion of a combinatorial graph was defined as a pair $(A,S)$, where S is a set and A a subset of $\mathfrak{P}(S)$ consisting of sets with two elements; the elements of S are called vertices, those of A edges, and two vertices $x$ and $y\in S$ are said to be joined if $\{x, y\}$ is an edge.

To such a combinatorial graph $\Gamma  = (A,S)$, one associates a graph G whose set of vertices is S and whose set of arrows $\widetilde{A}$ is the subset of $S^2$ consisting of pairs of joined vertices, the origin mapping and the end mapping coinciding with the first and second projection of $S^2$ onto S, and the involution $f\mapsto \overline{f}$ being given by the restriction to $\widetilde{A}$ of the mapping $(x, y)\mapsto (y, x)$ of $S^2$ into itself. The mapping which associates with an edge $\{f, f\}$ of G the set $\{o(f), t(f)\}$ is a bijection of the set of edges of G onto that of the edges of the combinatorial graph Γ.

Conversely, every graph such that the origin and the end of every arrow are distinct, and such that an arrow is determined by its origin and its end, is of this form.

The reader will verify that the notions of connectedness, tree, and forest for a combinatorial graph coincide with the corresponding notions for the graph associated with it.

## EXERCISES {#ta-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: Care will be taken not to confuse the notion of graph introduced here with that of E, II, §3, n$^o1$.
