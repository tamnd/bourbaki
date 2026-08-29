---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 3
section_title: Groupoïde de Poincaré
lang: en
source: ta-i-iv-fr
book_pages: TA III.289-TA III.300, TA III.334
pdf_pages: 0305-0316, 0350-0350
extraction: native
subsections:
    - "no": 1
      title: Groupoïde de Poincaré
      page: 289
      pdf_page: 305
    - "no": 2
      title: Fonctorialité du groupoïde de Poincaré
      page: 293
      pdf_page: 309
    - "no": 3
      title: Lacets librement homotopes
      page: 299
      pdf_page: 315
statements: 27
exercises: 2
content_sha256: ee54037fd61f5c94a013c52d01e32e0a8d06665295d56ff2380aa432000f2116
translated_from: content/fr/ta/III/03_s3_groupoide_de_poincare.md
source_lang: fr
translation_method: machine
source_content_sha256: 12c1892f9c178bcdfcd252546024bfd78e4e9843611e8f358057b6b5d6375e69
translation_model: gpt-5.4
translation_run: translate-en-mt-d88036bd
glossary_version: 34
glossary_terms_sha256: e99239d484a95a3328a672ef0fc614c4901bf7d2d2b7a5b7cc8b595873b936f3
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. POINCARÉ GROUPOID

### 1. Poincaré groupoid

#### Definition 1 {#ta-iii-s3-def-1 .statement tag=01YE}

Let X be a topological space, let $c_0$ and $c_1$ be paths in X and $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ a homotopy joining $c_0$ to $c_1$. One says that $\sigma$ is a strict homotopy if the mappings $s\mapsto \sigma (0, s)$ and $s\mapsto \sigma (1, s)$ are constant.

One says that paths $c_0$ and $c_1$ in X are strictly homotopic if there exists a strict homotopy joining $c_0$ to $c_1$.

Two strictly homotopic paths have the same origin and the same end.

#### Example {#ta-iii-s3-n1-exa-1 .statement tag=01YF}

Let $c$ be a path in X and let $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ be a continuous mapping such that $\varphi (0) = 0$ and $\varphi (1) = 1$. The paths $c$ and $c\circ \varphi$ are strictly homotopic. In fact, the mapping $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ defined by $\sigma (t, s) =c((1-s)t+s\varphi (t))$ is a strict homotopy joining $c$ to $c\circ \varphi$.

Let X be a topological space. Recall (cf. III, p. 257) that Λ(X) denotes the topological space $\mathscr{C}_c(\mathbf{I}; X)$ of paths in X and that for $x$, $y\in X$, $\Lambda_{x,y}(X)$ is the subspace of Λ(X) formed by the paths with origin $x$ and end $y$. The family of sets $\Lambda_{x,y}(X)$, for $x,y\in X$, is a partition of the space of paths in X. By the canonical bijection (III, p. 257, remark 2) of $\mathscr{C}(\mathbf{I}\times \mathbf{I}; X)$ onto $\mathscr{C}(\mathbf{I}; \Lambda (X))$, strict homotopies correspond to paths $c:\mathbf{I}\rightarrow \Lambda (X)$ whose image is contained in a subspace of the form $\Lambda_{x,y}(X)$. The relation “the paths $c_0$ and $c_1$ are strictly homotopic” is therefore an equivalence relation in Λ(X) (III, p. 259, prop. 5) and the equivalence classes for this relation are the arcwise connected components of the subspaces $\Lambda_{x,y}(X)$ of the space of paths in X. One denotes by $\varpi_{x,y}(X)$ the set $\pi_0(\Lambda_{x,y}(X))$ and calls every element of $\varpi_{x,y}(X)$ a class of paths joining $x$ to $y$.

#### Definition 2 {#ta-iii-s3-def-2 .statement tag=01YG}

One calls the space of loops of X, and denotes by Ω(X), the subspace of Λ(X) consisting of loops (III, p. 256, def. 1) in X.

One denotes by $\Omega_x(X)$ the set $\Lambda_{x,x}(X)$. The elements of $\Omega_x(X)$ are called loops in X at $x$ and the elements of $\varpi_{x,x}(X)$ are called classes of loops in X at $x$. The constant mapping $e_x:\mathbf{I}\rightarrow X$ with image $x$ is a loop, called the constant loop at $x$; its strict homotopy class is denoted by $\varepsilon_x$. The mapping $x\mapsto e_x$ of X into Λ(X) is continuous (III, p. 257, prop. 1).

Let X be a topological space and let $x,y,z$ be points of X. By passing to arcwise connected components, one deduces from the continuous mapping $c\mapsto \overline{c}$ of $\Lambda_{x,y}(X)$ into $\Lambda_{y,x}(X)$ (III, p. 258, corollary) a mapping of $\varpi_{x,y}(X)$ into $\varpi_{y,x}(X)$ which is denoted by $\gamma \mapsto \overline{\gamma}$. If $\gamma \in$ $\varpi_{x,y}(X),\overline{\gamma}$ is called the inverse of the path class $\gamma$.

Analogously, if one identifies the sets $\pi_0(\Lambda_{x,y}(X))\times \pi_0(\Lambda_{y,z}(X))$ and $\pi_0(\Lambda_{x,y}(X)\times \Lambda_{y,z}(X))$ (III, p. 260, Prop. 6), one deduces from the continuous mapping $(c, d)\mapsto c*d$ of $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ into $\Lambda_{x,z}(X)$ (III, p. 258, corollary), by passing to arcwise connected components, a mapping $C_{x,y,z}:\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$. For $\gamma \in \varpi_{x,y}(X)$ and $\delta \in \varpi_{y,z}(X)$, the strict homotopy class $C_{x,y,z}(\gamma , \delta )$ is denoted by $\gamma \delta$. It is called the composite of the composable path classes $\gamma$ and $\delta$.

One has $\overline{\overline{\gamma}}=\gamma$ and $\overline{\gamma \delta}=\delta  \gamma$.

#### Proposition 1 {#ta-iii-s3-prop-1 .statement tag=01YH}

Let X be a topological space, let $x,y,z,u$ be points of X, and let $\gamma_1\in \varpi_{x,y}(X),\gamma_2\in \varpi_{y,z}(X),\gamma_3\in \varpi_{z,u}(X)$ be path classes. One has

$$
\varepsilon_x\gamma_1=\gamma_1\varepsilon_y=\gamma_1 \tag{1}
$$

$$
\gamma_1\overline{\gamma}_1=\varepsilon_x,\overline{\gamma}_1\gamma_1=\varepsilon_y \tag{2}
$$

$$
(\gamma_1\gamma_2)\gamma_3=\gamma_1(\gamma_2\gamma_3) \tag{3}
$$

Let $c_1\in \Lambda_{x,y}(X),c_2\in \Lambda_{y,z}(X),c_3\in \Lambda_{z,u}(X)$ be representatives of $\gamma_1,\gamma_2$ and $\gamma_3$ respectively. Let $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ be the function defined by

$t/2$ for $0\leqslant t\leqslant 1/2$,

(4) $\varphi (t) =t-1/4$ for $1/2\leqslant t\leqslant 3/4$,

$2t-1$ for $3/4\leqslant t\leqslant 1$.

The function $\varphi$ is affine on each of the three intervals $[0,1/2]$, $[1/2,3/4]$ and $[3/4,1]$; it is therefore continuous. One has $\varphi (0) = 0$ and $\varphi (1) = 1$. It follows from formula (1) of III, p. 256 defining the juxtaposition of paths that

$$
c_1*(c_2*c_3) = ((c_1*c_2)*c_3)\circ \varphi
$$

By the example of III, p. 289, the paths $c_1*(c_2*c_3)$ and $(c_1*c_2)*c_3$ are strictly homotopic, whence equality (3).

Analogously, the function $\psi :\mathbf{I}\rightarrow \mathbf{I}$ defined by

$2t$ for $0\leqslant t\leqslant 1/2$,

$$
\psi (t) = \tag{5}
$$

1 for $1/2\leqslant t\leqslant 1$

is continuous and satisfies $\psi (0) = 0,\psi (1) = 1$. The equality $\gamma_1\varepsilon_y=\gamma_1$ then follows from the fact that

$$
c_1*e_y=c_1\circ \psi
$$

and the equality $\varepsilon_x\gamma_1=\gamma_1$ is proved analogously, whence (1).

The mapping $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ defined by

$c_1(2ts)$ for $0\leqslant t\leqslant 1/2$,

$$
\sigma (t, s) = \tag{6}
$$

$c_1(2(1-t)s)$ for $1/2\leqslant t\leqslant 1$

is continuous; it is a strict homotopy joining the path $e_x$ to the path $c_1*\overline{c_1}$, whence the first equality in (2). The second results from the first and from the fact that, for every path $c$, one has $c=\overline{\overline{c}}$.

#### Remark 1 {#ta-iii-s3-n1-rem-1 .statement tag=01YI}

Let X be a topological space. Let $n$ be an integer $\geqslant 1$ and let $(c_1, . . . , c_n)$ be a sequence of paths in X such that $c_i$ and $c_{i+1}$ are juxtaposable for $1\leqslant i\leqslant n-1$ (such a sequence is called a sequence of juxtaposable paths). Let us denote by $c$ the path

$$
c_1*(c_2*(\cdots  *(c_{n-1}*c_n). . .))
$$

and by $c'$ the path defined by $c'(t) =c_i(nt-i+ 1)$ for $1\leqslant i\leqslant n$ and $t\in [\frac{i-1}{n},\frac{i}{n}]$. The paths $c$ and $c'$ have the same image and are strictly homotopic: one is the composite of the other with a homeomorphism of $\mathbf{I}$ leaving 0 and 1 fixed (cf. III, p. 289, example). We shall sometimes denote by $c_1*c_2* \cdots  *c_n$ the path $c'$.

There exists a unique oriented graph $\varpi (X)$ whose set of vertices is X and whose set of arrows joining a point $x$ to a point $y$ is $\varpi_{x,y}(X)$, and in which the mappings $C_{x,y,z}$ define a law of composition. By proposition $1,\varpi (X)$ is a groupoid (II, p. 162, def. 4). For every $x\in X$, the identity element at the vertex $x$ of this groupoid is the class of the constant loop with image $x$. The inverse of an arrow $\gamma$ is the arrow $\overline{\gamma}$, which we shall also denote by $\gamma^{-1}$. In particular, the law of composition $C_{x,x,x}$ endows, for every $x\in X$, the set $\varpi_{x,x}(X)$ with a group structure; this group is denoted by $\pi_1(X, x)$.

#### Definition 3 {#ta-iii-s3-def-3 .statement tag=01YJ}

Let X be a topological space. The groupoid $\varpi (X)$ is called the Poincaré groupoid, or fundamental groupoid, of the space X. Let $x$ be a point of X; the group $\pi_1(X, x)$ of classes of loops at $x$ is called the Poincaré group, or fundamental group, of the space X at the point $x$.

Let $\mathscr{U}$ be a set of subsets of X whose interiors cover X. The classes of paths in X whose image is contained in one of the subsets belonging to $\mathscr{U}$ generate the groupoid $\varpi (X)$ (lemma 4 of III, p. 272).

The orbits of the groupoid $\varpi (X)$ (II, p. 162) coincide with the arcwise connected components of the space X. In particular (loc. cit.), one has:

#### Proposition 2 {#ta-iii-s3-prop-2 .statement tag=01YK}

Let X be a topological space.

a) If the space X is arcwise connected, the groups $\pi_1(X, x)$ and $\pi_1(X, y)$ are isomorphic for all points $x$ and $y$ of X.

b) Let $x$ be a point of X; the following conditions are equivalent:

(i) The group $\pi_1(X, x)$ is trivial;

(ii) Two paths with origin $x$ in X which have the same end

are strictly homotopic;

(iii) Every loop with origin $x$ in X is strictly homotopic

to the constant loop with image $x$.

More precisely, let X be an arcwise connected topological space and let $x$ and $y$ be points of X. For every element $\delta$ of $\varpi_{x,y}(X)$, the mapping $u_{\delta}:\gamma \mapsto \delta \gamma \delta^{-1}$ of $\pi_1(X, y)$ into $\pi_1(X, x)$ is a group isomorphism whose inverse isomorphism is $u_{\delta^{-1}}$. For $\delta \in \varpi_{x,y}(X)$ and $\gamma \in \pi_1(X, y)$, we set $^{\delta}\gamma =u_{\delta}(\gamma )$. When $x=y$, one has $^{\delta}\gamma =$ Int($\delta$ )$(\gamma )$, i.e. $u_{\delta}=$ Int($\delta$ ).

Let $x,y,z$ be points of X. For $\delta \in \varpi_{x,y}(X)$ and $\eta \in \varpi_{y,z}(X)$, one has $u_{\delta \eta}=u_{\delta}\circ u_{\eta}$, which may also be written $^{\delta \eta}\gamma =^{\delta}(^{\eta}\gamma )$ for $\gamma \in \pi_1(X, z)$.

Let $x,y$ be points of X and let $\delta ,\delta '$ be elements of $\varpi_{x,y}(X)$. One has

(7) $u_{\delta'}=u_{\delta}\circ$ Int($\delta^{-1}\delta '$) $=$ Int($\delta '\delta^{-1}$)$\circ u_{\delta}$.

#### Remark 2 {#ta-iii-s3-n1-rem-2 .statement tag=01YL}

Let X be a topological space and let C be an arcwise connected component of X. If $x$ and $y$ are points of C, the topological space $\Lambda_{x,y}(C)$ is identified with the topological space $\Lambda_{x,y}(X)$, so that the set $\varpi_{x,y}(C)$ is identified with the set $\varpi_{x,y}(X)$. Thus, the fundamental groupoid $\varpi (C)$ is identified with the full subgroupoid of $\varpi (X)$ having C as set of points. In particular, for every point $x$ of C, the group $\pi_1(C, x)$ is identified with the group $\pi_1(X, x)$.

#### Remark 3 {#ta-iii-s3-n1-rem-3 .statement tag=01YM}

Let X be a topological space and let $x,y,z$ be points of X. The mapping $(c, d)\mapsto c*d$ of $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ into $\Lambda_{x,z}(X)$ is continuous (III, p. 258, corollary of Prop. 2). It should be noted that the composition mapping $\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$ deduced from it is not necessarily continuous when the sets $\varpi_{x,y}(X),\varpi_{y,z}(X)$ and $\varpi_{x,z}(X)$ are endowed with the quotient topologies (cf. TG, I, p. 35 and III, p. 259). However, for every $\gamma_0\in \varpi_{x,y}(X)$ and every $\delta_0\in \varpi_{y,z}(X)$, the partial mappings $\gamma \mapsto \gamma \delta_0$ of $\varpi_{x,y}(X)$ into $\varpi_{x,z}(X)$ and $\delta \mapsto \gamma_0\delta$ of $\varpi_{y,z}(X)$ into $\varpi_{x,z}(X)$ are homeomorphisms. In fact, let $c_0\in \Lambda_{x,y}(X)$ be a path of class $\gamma_0$. The mapping $d\mapsto c_0*d$ is a continuous mapping of $\Lambda_{y,z}(X)$ into $\Lambda_{x,z}(X)$. The mapping $\delta \mapsto \gamma_0\delta$ is deduced from it by passing to quotients, and is therefore continuous. The same holds for the mapping $\delta '\mapsto \gamma_0^{-1}\delta '$ of $\varpi_{x,z}(X)$ into $\varpi_{y,z}(X)$. Since these two mappings are inverse to one another, they are homeomorphisms. One reasons analogously for the mapping $\gamma \mapsto \gamma \delta_0$. See also IV, p. 374.

### 2. Functoriality of the Poincaré groupoid

Let X, Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. The mapping $c\mapsto f\circ c$ is a continuous mapping, denoted $\Lambda (f)$, of Λ(X) = $\mathscr{C}_c(\mathbf{I}; X)$ into Λ(Y) = $\mathscr{C}_c(\mathbf{I}; Y)$ (I, p. 132, lemma). By passing to subsets it defines continuous mappings

$$
\Lambda_x(f): \Lambda_x(X)\rightarrow \Lambda_{f(x)}(Y)
$$

for $x\in X$,

$$
\Lambda_{x,y}(f): \Lambda_{x,y}(X)\rightarrow \Lambda_{f(x),f(y)}(Y)
$$

for $x,y\in X$ and

$$
\Omega (f): \Omega (X)\rightarrow \Omega (Y)
$$

For $x\in X$, the mapping $\Lambda_{x,x}(f)$ is also denoted $\Omega_x(f)$. By passing to path-connected components (III, p. 290), one deduces from the mapping $\Lambda_{x,y}(f)$ a mapping

$$
\varpi_{x,y}(f):\varpi_{x,y}(X)\rightarrow \varpi_{f(x),f(y)}(Y)
$$

Let $x,y,z$ be points of X and let $c\in \Lambda_{x,y}(X),d\in \Lambda_{y,z}(X)$ be paths; by definition of the juxtaposition of paths, one has

$$
f\circ (c*d) = (f\circ c)*(f\circ d)
$$

By passing to strict homotopy classes, one obtains the relation

$$
\varpi_{x,z}(f)(\gamma \delta ) = (\varpi_{x,y}(f)(\gamma ))(\varpi_{y,z}(f)(\delta ))
$$

for every $\gamma \in \varpi_{x,y}(X)$ and every $\delta \in \varpi_{y,z}(X)$. Thus, the continuous mapping $f$ and the mappings $\varpi_{x,y}(f)$, for $x$ and $y\in$ X, define a morphism of the groupoid $\varpi (X)$ into the groupoid $\varpi (Y)$ (II, p. 161, def. 3). It is denoted by $\varpi (f)$ and is called the morphism of Poincaré groupoids deduced from the continuous mapping $f$. In particular, if $x$ is a point of X, the mapping $\varpi_{x,x}(f)$ is a homomorphism of the group $\pi_1(X, x)$ into the group $\pi_1(X, f(x))$; this homomorphism is also denoted by $\pi_1(f, x)$.

#### Remark 1 {#ta-iii-s3-n2-rem-1 .statement tag=01YN}

The homomorphism $\varpi_{x,y}(f)$ is continuous if one endows the sets $\varpi_{x,y}(X)$ and $\varpi_{f(x),f(y)}(Y)$ with the quotient topology of the topology of compact convergence on $\mathscr{C}_c(\mathbf{I}; X)$ and $\mathscr{C}_c(\mathbf{I}; Y)$.

To simplify the notation, if $x,y\in X$ and $\gamma \in \varpi_{x,y}(X)$, we shall sometimes write $f_*(\gamma )$ for the element $\varpi_{x,y}(f)(\gamma )$ of $\varpi_{f(x),f(y)}(Y)$.

Let X, Y, Z be topological spaces, let $f: X\rightarrow Y,g: Y\rightarrow Z$ be continuous mappings. For every path $c$ in X, one has $(g\circ f)\circ c=$ $g\circ (f\circ c)$. It follows that one has

$$
\varpi (g\circ f) =\varpi (g)\circ \varpi (f)
$$

Let X and Y be topological spaces, let $f_0$ and $f_1$ be continuous mappings of X into Y, and let $\sigma : X\times \mathbf{I}\rightarrow Y$ be a homotopy joining $f_0$ to $f_1$. Since the mapping $(c, t)\mapsto c(t)$ of $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ into X (III, p. 257, prop. 1) is continuous, the same is true of the mapping of $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}\times \mathbf{I}$ into Y given by $(c, t, s)\mapsto \sigma (c(t), s)$. Consequently, the mapping $\Sigma : (c, s)\mapsto \sigma (c(\cdot ), s)$ is a continuous mapping of $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ into $\mathscr{C}_c(\mathbf{I}; Y)$ (loc. cit.). The mapping Σ is a homotopy joining the mapping $\Lambda (f_0)$ to the mapping $\Lambda (f_1)$. By restriction to the loop spaces, the mapping Σ induces a homotopy $\Omega (X)\times \mathbf{I}\rightarrow \Omega (Y)$ joining $\Omega (f_0)$ to $\Omega (f_1)$. Let $x$ be a point of X; suppose that the homotopy $\sigma$ is a homotopy pointed at $x$, and put $y=f_0(x) =f_1(x)$. The mapping Σ then induces a continuous mapping of $\Omega_x(X)\times \mathbf{I}$ into $\Omega_y(Y)$ which is a homotopy pointed at $e_x$, joining the mapping $\Omega_x(f_0)$ to the mapping $\Omega_x(f_1)$.

#### Proposition 3 {#ta-iii-s3-prop-3 .statement tag=01YO}

Let X and Y be topological spaces, $f_0$ and $f_1$ continuous mappings of X into Y, and let $\sigma : X\times \mathbf{I}\rightarrow$ Y be a homotopy joining $f_0$ to $f_1$. Let $x$ be a point of X; put $y_0=f_0(x)$, $y_1=f_1(x)$, and denote by $\delta \in \varpi_{y_0,y_1}(Y)$ the class of the path $d$ defined by $d(t) =\sigma (x, t)$ for $t\in \mathbf{I}$. For every $\gamma \in \pi_1(X, x)$, one has $(f_1)_*(\gamma ) =$ $\delta^{-1}((f_0)_*(\gamma ))\delta$.

Let $c$ be a loop in X at $x$ and let $\gamma$ be its strict homotopy class. Put $\gamma_0= (f_0)_*(\gamma )$ and $\gamma_1= (f_1)_*(\gamma )$; these are the strict homotopy classes of $f_0\circ c$ and $f_1\circ c$. For $(t, s)\in \mathbf{I}\times \mathbf{I}$, put $\varphi (t, s) =\sigma (c(t), s)$. For every $t\in \mathbf{I}$, one has $\varphi (t,0) = (f_0\circ c)(t),\varphi (t,1) = (f_1\circ c)(t)$ and $\varphi (0, t) =\varphi (1, t) =d(t)$. The relation $\gamma_0\delta =\delta \gamma_1$ therefore follows from the following lemma.

#### Lemma 1 {#ta-iii-s3-lem-1 .statement tag=01YP}

Let Y be a topological space and let $\varphi :\mathbf{I}\times \mathbf{I}\rightarrow Y$ be a continuous mapping. For $t\in \mathbf{I}$, put $c_0(t) =\varphi (t,0),c_1(t) =\varphi (t,1)$, $d_0(t) =\varphi (0, t)$ and $d_1(t) =\varphi (1, t)$. The paths $c_0*d_1$ and $d_0*c_1$ are strictly homotopic.

Let $c$ denote the path in $\mathbf{I}\times \mathbf{I}$ obtained by juxtaposing the paths $t\mapsto (t,0)$ and $t\mapsto (1, t)$; let $d$ denote the path in $\mathbf{I}\times \mathbf{I}$ obtained by juxtaposing the paths $t\mapsto (0, t)$ and $t\mapsto (t,1)$. The paths $c$ and $d$ have the same origin $(0,0)$ and the same end $(1,1)$. The mapping $(t, s)\mapsto$ $(1-s)c(t)+sd(t)$ of $\mathbf{I}\times \mathbf{I}$ into $\mathbf{I}\times \mathbf{I}$ is a strict homotopy joining $c$ to $d$. One has $c_0*d_1=\varphi \circ c$ and $d_0*c_1=\varphi \circ d$; these two paths are therefore strictly homotopic.

#### Corollary 1 {#ta-iii-s3-lem-1-cor-1 .statement tag=01YQ}

Let X and Y be topological spaces and let $x$ be a point of X. Let $f_0$ and $f_1$ be continuous mappings of X into Y. If there exists a pointed homotopy at $x$ joining $f_0$ to $f_1$, one has $\pi_1(f_0, x) =$ $\pi_1(f_1, x)$.

Let $\sigma$ be a pointed homotopy at $x$ joining $f_0$ to $f_1$. With the notation of Prop. $3,\delta$ is the class of a constant path with image $f_0(x) =$ $f_1(x)$. The assertion follows.

#### Corollary 2 {#ta-iii-s3-lem-1-cor-2 .statement tag=01YR}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a homeomorphism. For every point $x$ of X, the homomorphism

$$
\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))
$$

is an isomorphism.

Let $g$ be a continuous mapping of Y into X, inverse to $f$ up to homotopy. Let $x$ be a point of X. It follows from Prop. 3 applied to the homotopic mappings Id$_X$ and $g\circ f: X\rightarrow X$ that the mapping $\pi_1(g\circ f, x)$ is an isomorphism of the group $\pi_1(X, x)$ onto the group $\pi_1(X, g\circ f(x))$. Since

$$
\pi_1(g\circ f, x) =\pi_1(g, f(x))\circ \pi_1(f, x)
$$

the homomorphism $\pi_1(f, x)$ is injective and the homomorphism $\pi_1(g, f(x))$ is surjective. Since the mapping $g$ is also a homotopy equivalence, the homomorphism $\pi_1(g, f(x))$ is injective; it is therefore an isomorphism. Hence $\pi_1(f, x)$ is an isomorphism.

#### Example {#ta-iii-s3-n2-exa-1 .statement tag=01YS}

Let G be a topological group, let $e$ be its identity element. For every point $g$ of G, the left and right translations, $x\mapsto gx$ and $x\mapsto xg$, are homeomorphisms of G onto itself (TG, III, p. 2) which map $e$ onto $g$. By Corollary 2, they induce isomorphisms of $\pi_1(G, e)$ onto $\pi_1(G, g)$. These isomorphisms are not necessarily equal (IV, p. 459, exerc. 1).

#### Corollary 3 {#ta-iii-s3-lem-1-cor-3 .statement tag=01YT}

Let X be a topological space homotopic to a point. For every point $x$ of X, the group $\pi_1(X, x)$ is reduced to the identity element.

Cor. 3 applies in particular when X is the numerical space of $n$ dimensions $\mathbf{R}^n$ and more generally when X is a subset of the space $\mathbf{R}^n$ which is star-shaped (III, p. 234) with respect to one of its points.

#### Proposition 4 {#ta-iii-s3-prop-4 .statement tag=01YU}

Let X be the product space of a family $(X_j)_{j\in J}$ of topological spaces. The morphism of the groupoid $\varpi (X)$ into the product of the groupoids $\varpi (X_j)$, for $j\in J$, defined by the family of morphisms $(\varpi$(pr$_j$))$_{j\in J}$ is an isomorphism.

Let $\varphi$ denote this morphism of groupoids. The mapping deduced from it by passing to the vertices is the identity mapping $X\rightarrow \prod_jX_j$. Let $x= (x_j)$ and $y= (y_j)$ be two points of X. Let $\varphi_{x,y}$ denote the mapping of $\varpi_{x,y}(X)$ into $\prod_j\varpi_{x_j,y_j}(X_j)$ deduced from $\varphi$. If for every $j\in J,c_j:\mathbf{I}\rightarrow$ $X_j$ is a path joining $x_j$ to $y_j$, the mapping $t\mapsto (c_j(t))$ is a path in X joining $x$ to $y$ (TG, I, p. 25, prop. 1). This proves that $\varphi_{x,y}$ is surjective. Let $c$ and $d$ be two paths in X joining $x$ to $y$. Suppose that for every $j\in J$ there exists a strict homotopy $\sigma_j:\mathbf{I}\times \mathbf{I}\rightarrow X_j$ joining pr$_j\circ c$ to pr$_j\circ d$. Then the mapping $(t, s)\mapsto (\sigma_j(t, s))$ of $\mathbf{I}\times \mathbf{I}$ into X is a strict homotopy joining $c$ to $d($loc. cit.). This proves that $\varphi_{x,y}$ is injective.

#### Corollary {#ta-iii-s3-n2-cor-1 .statement tag=01YV}

Let $x= (x_j)_{j\in J}$ be a point of X. The mapping

$$
\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)
$$

deduced from the mappings $\pi_1$(pr$_j, x_j$) is a group isomorphism.

This isomorphism is said to be canonical. In the sequel, we shall often identify $\pi_1(X, x)$ with $\prod_{j\in J}\pi_1(X_j, x_j)$ by means of this isomorphism.

#### Remark 2 {#ta-iii-s3-n2-rem-2 .statement tag=01YW}

Let $(X_j)_{j\in J}$ be a family of topological spaces. Let X denote the product topological space $\prod_{j\in J}X_j$ and let $x= (x_j)$ be a point of X.

For every $i\in J$, let $u_i: X_i\rightarrow X$ be the mapping such that, for $z\in X_i$, pr$_i\circ u_i(z) =z$ and, for every $j\in J$ distinct from $i$, pr$_j\circ u_i(z) =$ $x_j$. The mapping $u_i$ is continuous and the mapping $\pi_1(u_i, x_i)$ is identified with the canonical injection of the factor $\pi_1(X_i, x_i)$ into the product group of the family $(\pi_1(X_j, x_j))_{j\in J}($cf. A, I, p. 45).

Suppose that the set J is finite and, for every $j\in J$, let $\gamma_j$ be an element of $\pi_1(X_j, x_j)$. The element $(\gamma_j)$ of $\pi_1(X, x)$ is the composite of the classes of loops $(u_j)_*(\gamma_j),j\in J$, these classes being pairwise permutable.

#### Remark 3 {#ta-iii-s3-n2-rem-3 .statement tag=01YX}

Let $(X_j)_{j\in J}$ be a family of topological spaces. Let X denote the product topological space $\prod_{j\in J}X_j$ and let $x= (x_j)$ be a point of X.

Endow the sets $\pi_1(X, x)$ and $\pi_1(X_j, x_j)$ with the quotient topology of the topology of compact convergence on the spaces $\Lambda_x(X)$ and $\Lambda_{x_j}(X_j)$. The isomorphism $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ is then a homeomorphism. It is continuous (III, p. 294, remark 1). The topology of compact convergence on Λ(X) is generated by the subsets of the form $\mathbf{T}(K,U)$, where K is a compact subset of $\mathbf{I}$ and U an open subset of X. For $j\in J$, let $U_j$ be an open subset of $X_j$, such that $\prod_{j\in J}U_j\subset U$. Then (pr$_j$)$_*(\mathbf{T}(K,U))$ contains $\mathbf{T}(K,U_j)$. This shows that the mappings (pr$_j$)$_*: \Lambda_x(X)\rightarrow \Lambda_{x_j}(X_j)$ are open, and the mappings $\pi_1$(pr$_j, x_j$) are also open. Since they are surjective, the mapping $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ is open (TG, I, p. 34, Prop. 8). Being continuous and bijective, it is a homeomorphism (TG, I, p. 30, example 2).

#### Proposition 5 {#ta-iii-s3-prop-5 .statement tag=01YY}

Let X be a topological space and let $(A_i)_{i\in I}$ be an increasing family of subsets of X, indexed by a filtered ordered set I, such that every quasi-compact subset of X is contained in one of the $A_i$. The canonical groupoid morphism

$\rho :$ lim$\longrightarrow_{i\in I}\varpi (A_i)\rightarrow \varpi (X)$,

induced by the canonical injections of $A_i$ into X, is an isomorphism.

If $i\leqslant j$, let us denote by $\rho_{j,i}$ the groupoid morphism $\varpi (A_i)\rightarrow \varpi (A_j)$ induced by the injection of $A_i$ into $A_j$. Since the mapping induced by $\rho_{j,i}$ by passing to the vertices is the injection $A_i\rightarrow A_j$ and since the $A_i$ cover X, the mapping induced by $\rho$ by passing to the vertices is bijective.

Let $a$ and $b$ be points of X and let $c$ be a path joining $a$ to $b$ in X. The image of $c$ is a quasi-compact subset of X (TG, I, p. 62, Theorem 2), since $\mathbf{I}$ is compact. There therefore exists an element $i\in I$ such that the image of $c$ is contained in $A_i$. Consequently, the mapping induced by $\rho$ by passing to the sets of arrows is surjective.

Let $i\in I$, let $a$ and $b$ be points of $A_i$, let $c,c'$ be paths joining $a$ to $b$ in $A_i$; let $h$ be a strict homotopy joining $c$ to $c'$ in X. Since $\mathbf{I}\times \mathbf{I}$ is compact, $h(\mathbf{I}\times \mathbf{I})$ is a quasi-compact subset of X (loc. cit.) and there exists an element $i\in I$ such that the image of $h$ is contained in $A_i$. The paths $c$ and $c'$ are strictly homotopic in $A_i$; fortiori, the path classes $[c]$ and $[c']$ have the same image in lim$\longrightarrow \varpi (A_i)$. Consequently, $\rho$ is injective.

#### Corollary {#ta-iii-s3-n2-cor-2 .statement tag=01YZ}

Let $a$ be a point of X and let J be the set of $i\in I$ such that $a\in A_i$. The canonical homomorphism

lim$\longrightarrow_{i\in J}\pi_1(A_i, a)\rightarrow \pi_1(X, a)$

is bijective.

#### Remark 4 {#ta-iii-s3-n2-rem-4 .statement tag=01Z0}

The proposition and its corollary apply in particular when $(A_i)_{i\in I}$ is an increasing family of subsets of X indexed by a directed ordered set I such that the interiors of the $A_i$ cover X.

### 3. Freely Homotopic Loops

#### Definition 4 {#ta-iii-s3-def-4 .statement tag=01Z1}

Let X be a topological space and let $c$ and $c'$ be two loops in X. A free homotopy joining $c$ to $c'$ means a homotopy $\sigma$ joining $c$ to $c'$ such that $\sigma (0, s) =\sigma (1, s)$ for every $s\in \mathbf{I}$. One says that $c$ is freely homotopic to $c'$ if there exists a free homotopy joining $c$ to $c'$.

The free homotopies joining $c$ to $c'$ correspond to the paths joining $c$ to $c'$ in the space Ω(X) of loops in X. Consequently, the relation “$c$ is freely homotopic to $c'$” is an equivalence relation in Ω(X) whose equivalence classes are the arcwise connected components of Ω(X).

#### Remark {#ta-iii-s3-n3-rem-1 .statement tag=01Z2}

Let $\varphi$ be the canonical mapping of $\mathbf{R}$ onto $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. 2). The mapping $f\mapsto f\circ \varphi |\mathbf{I}$ is a homeomorphism of $\mathscr{C}_c(\mathbf{T}; X)$ onto Ω(X), whence, by passing to arcwise connected components, a bijection of the set $[\mathbf{T}; X]$ (III, p. 230) onto the set of free homotopy classes of loops in X.

#### Proposition 6 {#ta-iii-s3-prop-6 .statement tag=01Z3}

Let X be an arcwise connected topological space and let $x$ be a point of X.

a) Every loop in X is freely homotopic to a loop at $x$. More precisely, if $c$ is a loop at $y$ and $d$ a path with origin $y$ and end $x,c$ is freely homotopic to the loop $(\overline{d}*c)*d$ at $x$.

b) Two loops in X at $x$ are freely homotopic if and only if their strict homotopy classes are conjugate in the group $\pi_1(X, x)$.

Let us prove a). For every $s\in [0,1]$, let $d_s$ denote the path in X defined by $d_s(t) =d(st)$ for $t\in \mathbf{I}$; its origin is $y$. Since the mapping $(s, t)\mapsto d(st)$ is continuous, the mapping $s\mapsto d_s$ of $\mathbf{I}$ into $\mathscr{C}_c(\mathbf{I}; X)$ is continuous (III, p. 257, prop. 1). The mapping $s\mapsto (\overline{d_s}*c)*d_s$ is then a path in Ω(X) (III, p. 257, prop. 2) joining $(e_y*c)*e_y$ to $(\overline{d}*c)*d$, whence a).

Let $c$ and $c'$ be two loops in X at $x$. If their strict homotopy classes are conjugate in $\pi_1(X, x)$, there exists a loop $d$ at $x$ such that $c'$ is strictly homotopic to the loop $(\overline{d}*c)*d$. It follows from a) that $c$ and $c'$ are freely homotopic. Conversely, suppose that there exists a free homotopy $\varphi$ joining $c$ to $c'$. Put $d(t) =\varphi (0, t)$; one has also $d(t) =\varphi (1, t)$ and $d$ is a loop at $x$. By lemma 1 of III, p. 295, the loops $c*d$ and $d*c'$ are strictly homotopic. The strict homotopy classes of $c$ and $c'$ are therefore conjugate in $\pi_1(X, x)$.

#### Scholium {#ta-iii-s3-n3-sch-1 .statement tag=01Z4}

Let X be an arcwise connected topological space and let $x$ be a point of X. Proposition 6 makes it possible to define a canonical bijection of the set of free homotopy classes of loops in X onto the set of conjugacy classes in $\pi_1(X, x)$.

## EXERCISES {#ta-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
