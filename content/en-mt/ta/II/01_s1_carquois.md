---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 1
section_title: Carquois
lang: en
source: ta-i-iv-fr
book_pages: TA II.151-TA II.155, TA II.215-TA II.218
pdf_pages: 0167-0171, 0231-0234
extraction: native
subsections:
    - "no": 1
      title: Définition d’un carquois
      page: 151
      pdf_page: 167
    - "no": 2
      title: Sous-carquois
      page: 152
      pdf_page: 168
    - "no": 3
      title: Morphismes de carquois
      page: 152
      pdf_page: 168
    - "no": 4
      title: Produits de carquois
      page: 153
      pdf_page: 169
    - "no": 5
      title: Chemins et lacets dans un carquois
      page: 154
      pdf_page: 170
    - "no": 6
      title: Composantes connexes d’un carquois
      page: 154
      pdf_page: 170
statements: 2
exercises: 10
content_sha256: efe28e60038f2693e1a5ba938564c626f052607bb9c4dbb84cfc0a6a0a6620d5
translated_from: content/fr/ta/II/01_s1_carquois.md
source_lang: fr
translation_method: machine
source_content_sha256: b9239c711495a6203933aa065daeb8861e4db7597cdf677411c7d806e8a8c0fb
translation_model: gpt-5.4
translation_run: translate-en-mt-5f46b4e3
glossary_version: 34
glossary_terms_sha256: a39a39383b59d7b52ac09228256ad6a4590e10051edec2b460c31fd7f4a8347f
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. QUIVERS

Its monument, superb among monuments,

Which bristles, above a wall of dry bricks, its crest of towers like a quiver of arrows...

Victor Hugo, La Légende des siècles

### 1. Definition of a quiver

#### Definition 1 {#ta-ii-s1-def-1 .statement tag=01SS}

A quiver is a quadruple $(S,F, o, t)$, where S and F are sets and $o,t$ are mappings of F into S.

Let $C = (S,F, o, t)$ be a quiver. The elements of S are called the vertices of C. The elements of F are called the arrows of C. Let $f$ be an arrow of C; the vertex $o(f)$ is called the origin or the source of $f$, the vertex $t(f)$ is called the end, or the target, of $f$; one also says that $f$ joins the vertex $o(f)$ to the vertex $t(f)$. The mappings $o$ and $t$ are called respectively the source and target mappings, or origin and end, of the quiver C.

© N. Bourbaki and Springer-Verlag Berlin Heidelberg 2   016

N. Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_2  151

When C is a quiver, Som(C), Fl(C), $o_C$ and $t_C$ will denote respectively the set of vertices, the set of arrows, the source mapping and the target mapping of C. Let $a$ and $b$ be vertices of C; the set of arrows of C joining $a$ to $b$ is denoted by Fl$_{a,b}(C)$, or again $C_{a,b}$.

To make the arguments easier to understand, one may represent a quiver by a diagram composed of points and arrowed lines corresponding respectively to the vertices and the arrows. The diagram:

$$
f_1g
$$

$\bullet \bullet \bullet k$

$abc$

$f_2h$

represents a quiver whose vertices are $a,b,c$, whose arrows are $f_1, f_2, g, h, k$, and whose source and target mappings are given by

$$
o(f_1) =o(f_2) =ao(g) =bo(h) =co(k) =c
$$

$$
t(f_1) =t(f_2) =bt(g) =ct(h) =bt(k) =c
$$

### 2. Subquivers

Let C and $C'$ be quivers. One says that $C'$ is a subquiver of C if one has Som(C$'$)$\subset$ Som(C), Fl(C$'$)$\subset$ Fl(C) and if the mappings $o_{C'}$ and $t_{C'}$ coincide on Fl(C$'$) with the mappings $o_C$ and $t_C$. If, moreover, every arrow of C whose source and target belong to Som(C$'$) is an arrow of $C'$, one says that $C'$ is a full subquiver of C.

Let C be a quiver and let $(C_i)_{i\in I}$ be a family of subquivers of C. The intersection of the family $(C_i)_{i\in I}$ is defined to be, and is denoted by $\bigcap_{i\in I}C_i$, the subquiver of C whose set of vertices is $\bigcap_{i\in I}$ Som(C$_i$) and whose set of arrows is $\bigcap_{i\in I}$ Fl(C$_i$).

### 3. Morphisms of quivers

Let C and $C'$ be quivers. A quiver morphism of C into $C'$ is a pair $(u, v)$, where $u:$ Som(C) $\rightarrow$ Som(C$'$) and $v:$ Fl(C) $\rightarrow$ Fl(C$'$) are mappings such that $o_{C'}\circ v=u\circ o_C$ and $t_{C'}\circ v=u\circ t_C$.

Let $\varphi = (u, v)$ be a quiver morphism of C into $C'$. The mappings $u$ and $v$ are denoted by Som($\varphi$ ) and Fl($\varphi$ ). If $a$ is a vertex of C, we shall denote by abuse $\varphi (a)$ the image of a vertex $a$ of C, and we shall say that $\varphi (a)$ is the image of $a$ under $\varphi$. Analogously, if $f$ is an arrow of C, we shall denote by abuse $\varphi (f)$ the arrow $v(f)$ of $C'$ and we shall say that it is the image of $f$ under $\varphi$.

Let C, $C',C''$ be three quivers, let $\varphi = (u, v)$ be a morphism of C into $C'$ and let $\varphi '= (u', v')$ be a morphism of $C'$ into $C''$. Then $(u'\circ u, v'\circ v)$ is a morphism of C into $C''$ which is denoted by $\varphi '\circ \varphi$ and is called the composite of $\varphi '$ and $\varphi$.

Id$_C$ denotes the morphism (Id$_{Som(C)}$, Id$_{Fl(C)}$) of C into itself.

Let $\varphi$ be a quiver morphism of C into $C'$. In order that $\varphi$ be an isomorphism, it is necessary and sufficient that the mappings Som($\varphi$ ) and Fl($\varphi$ ) be bijective (cf. E, IV, p. 6).

Thus, if one calls a quiver structure on sets S and F the datum of two mappings $o, t: F\rightarrow S$, one may take quiver morphisms as morphisms of this structure (E, IV, p. 11).

Let $\varphi$ be a quiver morphism of C into $C'$. There exists a unique subquiver of $C'$ whose sets of vertices and arrows are the images of Som($\varphi$ ) and Fl($\varphi$ ) respectively. It is denoted by $\varphi (C)$ and is called the image of C under $\varphi$. One says that $\varphi$ is injective if the mappings Som($\varphi$ ) and Fl($\varphi$ ) are injective; in this case, $\varphi$ induces an isomorphism of C onto its image.

Let $\varphi$ and $\psi$ be morphisms of quivers from C to $C'$. There exists a unique subquiver of C whose vertices and arrows are respectively the vertices and arrows of C having the same image under $\varphi$ and $\psi$. It is called the equaliser of $\varphi$ and $\psi$.

### 4. Products of quivers

Let $(C_i)_{i\in I}$ be a family of quivers. Put S = $\prod_{i\in I}$ Som(C$_i$), $F =\prod_{i\in I}$ Fl(C$_i$), and let $o$ and $t$ be the mappings $\prod_{i\in I}o_{C_i}$ and $\prod_{i\in I}t_{C_i}$ respectively. The quadruple $C = (S,F, o, t)$ is a quiver, called the product quiver of the family $(C_i)_{i\in I}$.

There exists a unique morphism of quivers pr$_i: C\rightarrow C_i$ such that the mappings Som(pr$_i$) and Fl(pr$_i$) are respectively the projections of index $i$ from Som(C) to Som(C$_i$) and from Fl(C) to Fl(C$_i$).

We have the following universal property: Let $C'$ be a quiver; for every family $(\varphi_i)_{i\in I}$, where, for every $i\in I,\varphi_i: C'\rightarrow C_i$ is a morphism of quivers, there exists a unique morphism of quivers $\varphi : C'\rightarrow C$ such that $\varphi_i=$ pr$_i\circ \varphi$ for every $i\in I$.

### 5. Paths and loops in a quiver

#### Definition 2 {#ta-ii-s1-def-2 .statement tag=01ST}

Let C be a quiver. A path in C is a sequence $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$, where $n$ is an integer $\geqslant 0,a_0, . . . , a_n$ are vertices of C, and where, for $1\leqslant i\leqslant n,f_i$ is an arrow of C joining $a_{i-1}$ to $a_i$. One says that the path $c$ is of length $n$.

Let $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ be a path of length $n$ in C. The vertex $a_0$ is called the origin, or the source, of $c$; the vertex $a_n$ is called the term, or the end, of $c$; one also says that $c$ joins the vertex $a_0$ to the vertex $a_n$. The vertex $a_i$, for $0\leqslant i\leqslant n$, is called the vertex of index $i$; the arrow $f_i$, for $1\leqslant i\leqslant n$, is called the $i$-th arrow, or the arrow of index $i$. A path of length $\geqslant 1$ is determined by the sequence of its arrows.

A path whose origin is equal to the term is called a loop. A path of length 0 is a loop, called constant.

One says that paths

$c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ and $c'= (a'_0, f'_1, a'_1, . . . , a'_{m-1}, f'_m, a'_m)$

in C are juxtaposed if the term $a_n$ of $c$ is the origin $a'_0$ of $c'$. In this case, the sequence $(a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n, f'_1, a'_1, . . . , f'_m, a'_m)$ is a path in C which is denoted by $c*c'$ and is called the juxtaposed path of $c$ and $c'$. It joins the origin of $c$ to the term of $c'$; its length is the sum of the lengths of the paths $c$ and $c'$.

### 6. Connected components of a quiver

Let $C = (S,F, o, t)$ be a quiver. Consider the finest equivalence relation $R_C$ in S such that the relation $R_C\{o(f), t(f)\}$ is satisfied for every arrow $f$ of C. Two vertices $a,b$ of C are equivalent for this relation if and only if there exist an integer $n\geqslant 0$, vertices $a_0, . . . , a_n$ of C and arrows $f_1, . . . , f_n$ of C such that $a_0=a,a_n=b$ and such that, for $1\leqslant i\leqslant n$, the arrow $f_i$ joins either $a_{i-1}$ to $a_i$, or $a_i$ to $a_{i-1}$.

The equivalence classes of this equivalence relation are called the connected components of C. We denote by $\pi_0(C)$ the set of connected components of C. Finally, we say that C is connected if it has at most one connected component.

Let $\varphi : C\rightarrow C'$ be a morphism of quivers. The map Som($\varphi$ ) defines by passing to the quotients a map of $\pi_0(C)$ into $\pi_0(C')$ which we shall denote by $\pi_0(\varphi )$.

## EXERCISES {#ta-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
