---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 11
section_title: Grothendieck Groups
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.183-A VIII.210
pdf_pages: 0200-0227
extraction: native
subsections:
    - "no": 1
      title: Additive Functions of Modules
      page: 183
      pdf_page: 200
    - "no": 2
      title: The Grothendieck Group of an Additive Set of Modules
      page: 186
      pdf_page: 203
    - "no": 3
      title: Using Composition Series
      page: 189
      pdf_page: 206
    - "no": 4
      title: The Grothendieck Group R(A)
      page: 191
      pdf_page: 208
    - "no": 5
      title: Change of Rings
      page: 193
      pdf_page: 210
    - "no": 6
      title: The Grothendieck Group $R_K(A)$
      page: 194
      pdf_page: 211
    - "no": 7
      title: Multiplicative Structure on $K(\mathscr{C})$
      page: 196
      pdf_page: 213
    - "no": 8
      title: The Grothendieck Group $K_0(A)$
      page: 199
      pdf_page: 216
    - "no": 9
      title: The Grothendieck Group $K_0(A)$ of an Artinian Ring
      page: 200
      pdf_page: 217
    - "no": 10
      title: Change of Rings for $K_0(A)$
      page: 201
      pdf_page: 218
    - "no": 11
      title: Frobenius Reciprocity
      page: 202
      pdf_page: 219
    - "no": 12
      title: The Case of Simple Rings
      page: 204
      pdf_page: 221
statements: 36
exercises: 14
content_sha256: 22144ede4a5a2a95481142745763f478695c7ee2c260a4f16db28ffbaa72102e
---

## § 11. GROTHENDIECK GROUPS

### 1. Additive Functions of Modules

Let A be a ring, and let $\mathscr{C}$ be a set of classes of A-modules (VIII, p. 51); we say that an A-module is of type $\mathscr{C}$ if its class belongs to $\mathscr{C}$.

#### Definition 1 {#alg-viii-s11-def-1 .statement}

We say that the set $\mathscr{C}$ of classes of A-modules is additive if every zero module is of type $\mathscr{C}$ and the direct sum of two modules of type $\mathscr{C}$ is of type $\mathscr{C}$. We say that $\mathscr{C}$ is hereditary if it is additive and the submodules and quotient modules of a module of type $\mathscr{C}$ are of type $\mathscr{C}$.

#### Example 1 {#alg-viii-s11-n1-exa-1 .statement}

The set of classes of A-modules of finite length is hereditary (II, §1, No. 10, p. 212, Proposition 16).

#### Example 2 {#alg-viii-s11-n1-exa-2 .statement}

The set of classes of finitely generated A-modules is additive. If the ring A is Noetherian, then this set is hereditary (VIII, p. 3, Proposition 3 and VIII, p. 7, Proposition 4).

#### Example 3 {#alg-viii-s11-n1-exa-3 .statement}

The set of classes of finitely generated projective A-modules is additive but generally not hereditary.

#### Definition 2 {#alg-viii-s11-def-2 .statement}

Let $\varphi$ be a mapping from $\mathscr{C}$ to an abelian group G (written additively); set $\varphi (E) =\varphi$(cl(E)) for every A-module E of type $\mathscr{C}$. We say that $\varphi$ is an additive function of modules (resp. a weakly additive function of modules) if we have $\varphi (E) =\varphi (E') +\varphi (E'')$ for every exact sequence (resp. for every split exact sequence)

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

of modules of type $\mathscr{C}$.

#### Example 4 {#alg-viii-s11-n1-exa-4 .statement}

Let $\mathscr{C}$ be the set of classes of A-modules of finite length. The mapping long$_A:\mathscr{C}\rightarrow \mathbf{Z}$ that sends a class of A-modules of finite length to its length is an additive function of modules (II, §1, No. 10, p. 213, Corollary 3). The results of this subsection are a generalization of the results on modules of finite length established in II, §1, No. 10, p. 212–214.

In the remainder of this subsection, we consider an additive set $\mathscr{C}$ of A-modules and an additive mapping $\varphi$ from $\mathscr{C}$ to an abelian group G.

Let E and $E'$ be modules of type $\mathscr{C}$; then $E\oplus E'$ is of type $\mathscr{C}$, and there exists a split exact sequence (II, §1, No. 9, p. 210)

$$
0\longrightarrow E\longrightarrow E\oplus E'\longrightarrow E'\longrightarrow 0
$$

from this, we deduce (1) $\varphi (E\oplus E') =\varphi (E) +\varphi (E')$. In particular, we have $\varphi (0) = 0$.

#### Proposition 1 {#alg-viii-s11-prop-1 .statement}

Suppose that $\mathscr{C}$ is hereditary. Let E and F be A-modules and $u: E\rightarrow F$ a linear mapping.

a) If E or F is of type $\mathscr{C}$, then so is the image of $u$.

b) If E is of type $\mathscr{C}$, then so is the kernel of $u$, and we have (2) $\varphi (E) =\varphi$(Ker $u) +\varphi$(Im $u)$.

c) If F is of type $\mathscr{C}$, then so is the cokernel of $u$, and we have (3) $\varphi (F) =\varphi$(Im $u) +\varphi$(Coker $u)$.

The proposition follows from the existence of exact sequences

$0\longrightarrow$ Ker $u\longrightarrow E\longrightarrow$ Im $u\longrightarrow 0$,

$0\longrightarrow$ Im $u\longrightarrow F\longrightarrow$ Coker $u\longrightarrow 0$.

#### Corollary {#alg-viii-s11-n1-cor-1 .statement}

Let $(E_i)_{0\leqslant i\leqslant n}$ be a finite sequence of modules of type $\mathscr{C}$. If there exists an exact sequence

0 // $E_0^{u_0}$ // $E_1^{u_1}$ /$/\cdots$ // $E_{n-1}^{u_{n-1}}$ // $E_n$ // $0$,

then we have (4) $\sum_{i=0}^n(-1)^i\varphi (E_i) = 0$.

Let us prove the corollary by induction on $n$; the cases $n= 0$ and $n= 1$ are trivial. So let $n\geqslant 1$, and let

$$
0\longrightarrow E_0\longrightarrow^{u_0}E_1\longrightarrow  \cdots  \longrightarrow^{u_1}E_{n-1}\longrightarrow^{u_{n-1}}E_n-^u-\rightarrow^{^n}E_{n+1}\longrightarrow 0
$$

be an exact sequence of modules of type $\mathscr{C}$. By Proposition 1, the kernel F of $u_n$ is a module of type $\mathscr{C}$, and we have (5) $\varphi (F) =\varphi (E_n)-\varphi (E_{n+1})$.

Moreover, we have an exact sequence

$$
0\longrightarrow E_0\longrightarrow E_1\longrightarrow E_2\longrightarrow  \cdots  \longrightarrow E_{n-1}\longrightarrow F\longrightarrow 0
$$

and the induction hypothesis gives the relation

$$
n\sum_{i=0}^{-1}(-1)^i\varphi (E_i) + (-1)^n\varphi (F) = 0 \tag{6}
$$

We then immediately deduce from (5) and (6) that $\sum^n_{i=0}^{+1}(-1)^i\varphi (E_i) = 0$, and the corollary follows.

#### Proposition 2 {#alg-viii-s11-prop-2 .statement}

Suppose that the set $\mathscr{C}$ is hereditary. Let E be an A-module, and let M and N be submodules of E.

a) If the modules M and N are of type $\mathscr{C}$, then so are the modules $M\cap N$ and M + N, and we have

$$
\varphi (M + N) +\varphi (M\cap N) =\varphi (M) +\varphi (N)
$$

b) If the modules $E/M$ and $E/N$ are of type $\mathscr{C}$, then so are the modules $E/(M\cap N)$ and $E/(M + N)$, and we have

$$
\varphi (E/(M + N)) +\varphi (E/(M\cap N)) =\varphi (E/M) +\varphi (E/N)
$$

Assertions a) and b) follow from the existence of the exact sequences

$$
0\rightarrow M\cap N\rightarrow M\oplus N\rightarrow M + N\rightarrow 0
$$

and

$$
0\rightarrow E/(M\cap N)\rightarrow (E/M)\oplus (E/N)\rightarrow E/(M + N)\rightarrow 0
$$

(II, §1, No. 7, p. 207, Proposition 10).

#### Proposition 3 {#alg-viii-s11-prop-3 .statement}

Suppose that $\mathscr{C}$ is hereditary. Let E be a module of type $\mathscr{C}$ and $(E_i)_{0\leqslant i\leqslant n}$ a composition series of E (I, §4, No. 7, p. 41). For $1\leqslant i\leqslant n$, the module $E_{i-1}/E_i$ is of type $\mathscr{C}$, and we have

$$
\varphi (E) =\sum_{i=1}^n\varphi (E_{i-1}/E_i)
$$

Since $\mathscr{C}$ is hereditary, the modules $E_0/E_1$ and $E_1$ are of type $\mathscr{C}$, and we have $\varphi (E) =\varphi (E_0/E_1) +\varphi (E_1)$. Since the sequence $(E_{i+1})_{0\leqslant i\leqslant n-1}$ is a composition series of $E_1$, Proposition 3 follows by induction on $n$.

### 2. The Grothendieck Group of an Additive Set of Modules

Let A be a ring. In this subsection, we consider an additive set $\mathscr{C}$ of classes of A-modules; we identify $\mathscr{C}$ with the canonical basis of the free abelian group $\mathbf{Z}_{(\mathscr{C})}$. For any exact sequence

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

of modules of type $\mathscr{C}$, we denote by $r_{\mathscr{E}}$ the element cl(E) $-$ cl(E$')-$ cl(E$'')$ of $\mathbf{Z}_{(\mathscr{C})}$. Let R be the subgroup of $\mathbf{Z}_{(\mathscr{C})}$ generated by the elements of the form $r_{\mathscr{E}}$; the quotient group $\mathbf{Z}^{(\mathscr{C})}/R$ is called the Grothendieck group of $\mathscr{C}$ and is denoted by $K(\mathscr{C})$. For a module E of type $\mathscr{C}$, we denote the image of cl(E) in $K(\mathscr{C})$ by $[E]_{\mathscr{C}}$ (or sometimes [E] when there is ambiguity about $\mathscr{C})$. We then have the following universal property.

#### Proposition 4 {#alg-viii-s11-prop-4 .statement}

a) The mapping $E\mapsto [E]_{\mathscr{C}}$ from $\mathscr{C}$ to $K(\mathscr{C})$ is additive.

b) Let G be an abelian group, and let $\varphi :\mathscr{C}\rightarrow G$ be an additive function of modules. There exists a unique homomorphism $u: K(\mathscr{C})\rightarrow G$ such that we have $\varphi (E) =u([E]_{\mathscr{C}})$ for every module E of type $\mathscr{C}$.

Assertion a) is obvious. Let us prove b). There exists a homomorphism $u_':\mathbf{Z}_{(\mathscr{C})}\rightarrow G$ that extends $\varphi$. Since $\varphi$ is additive, we have $u_'(r$ ) = 0 for every exact sequence $(\mathscr{E})$ of modules of type $\mathscr{C}$; therefore, R is contained in$^{\mathscr{E}}$ the kernel of $u'$. Consequently, when passing to the quotient, $u'$ defines a homomorphism $u$ from $K(\mathscr{C})$ to G, and it is clear that we have $\varphi (E) =u([E]_{\mathscr{C}})$ for every A-module of type $\mathscr{C}$. The group $K(\mathscr{C})$ is generated by the set of elements $[E]_{\mathscr{C}}$ for E running through $\mathscr{C}$; the uniqueness of $u$ follows.

Let $\mathscr{C}$ and $\mathscr{D}$ be additive sets of classes of A-modules such that $\mathscr{C}\subset \mathscr{D}$. Since the mapping $E\mapsto [E]_{\mathscr{D}}$ fromn$\mathscr{C}$ to the Grothendieck groupnK($\mathscr{D})$ is additive, there exists a homomorphism $\gamma_{\mathscr{D},\mathscr{C}}: K(\mathscr{C})\rightarrow K(\mathscr{D})$, called

canonical, characterized by the formula $\gamma_{\mathscr{D},\mathscr{C}}([E]_{\mathscr{C}}) = [E]_{\mathscr{D}}$ for every module E of type $\mathscr{C}$. It is not always injective (VIII, p. 210, Exercise 13).

#### Example {#alg-viii-s11-n2-exa-1 .statement}

$*$ Let A be a Noetherian commutative ring, and let Σ be its spectrum. For any integer $n\geqslant 0$, denote by $\mathscr{C}^{\geqslant n}$ the set of classes of finitely generated A-modules with support of codimension $\geqslant n$ in Σ. Set $K(n,A) =$ $K(\mathscr{C}^{\geqslant n})$ and $\gamma_n=\gamma_{\mathscr{C}^{\geqslant n},\mathscr{C}^{\geqslant n+1}}$. We have a sequence of homomorphisms

$$
\gamma_n: K(n+ 1,A)\longrightarrow K(n,A)
$$

We can prove (AC, VIII, §1, n$^o5$, p. 13, proposition 10) that in $K(n,A)$, the elements $[A/\mathfrak{p}]_{\mathscr{C}_n}$, where $\mathfrak{p}$ runs through the set of elements of Σ of height $n$, form a basis of a $\mathbf{Z}$-module supplementary to the image of $\gamma_n$. More precisely, for every module E of type $\mathscr{C}^{\geqslant n}$, we have

$[E]_{\mathscr{C}^{\geqslant n}}\equiv \sum$ long$_{A_{\mathfrak{p}}}(E_{\mathfrak{p}})\cdot [A/\mathfrak{p}]_{\mathscr{C}^{\geqslant n}}$ (mod Im $\gamma_n).*$

$\{\mathfrak{p}\in Σ|$ht($\mathfrak{p})=n\}$

The group $K(\mathscr{C})$ is generated by the elements of the form $[E]_{\mathscr{C}}$ with $E\in \mathscr{C}$, and we have $[E\oplus E']_{\mathscr{C}}= [E]_{\mathscr{C}}+ [E']_{\mathscr{C}}$ by relation (1) (VIII, p. 184). Every element of $K(\mathscr{C})$ is therefore of the form $[E]_{\mathscr{C}}-[F]_{\mathscr{C}}$, where E and F belong to $\mathscr{C}$.

An element of $K(\mathscr{C})$ is called effective if it is of the form $[E]_{\mathscr{C}}$ for an A-module E of type $\mathscr{C}$. The set of effective elements of $K(\mathscr{C})$ is denoted by $K(\mathscr{C})^+$; it is a submonoid of $K(\mathscr{C})$, and $K(\mathscr{C})$ can be identified with the group of differences of $K(\mathscr{C})^+$ (I, §2, No. 4, p. 20).

#### Proposition 5 {#alg-viii-s11-prop-5 .statement}

Let E and F be modules of type $\mathscr{C}$. The equality

$[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ holds if and only if there exist exact sequences of modules of type $\mathscr{C}$

$$
(\mathscr{E})0\longrightarrow L\longrightarrow P\longrightarrow M\longrightarrow 0
$$

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

such that $E\oplus Q$ is isomorphic to $F\oplus P$.

The stated condition is sufficient because it implies the relations

$$
[P]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[Q]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[E]_{\mathscr{C}}+[Q]_{\mathscr{C}}= [F]_{\mathscr{C}}+[P]_{\mathscr{C}}
$$

which give $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$.

Now suppose that we have $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$. By the construction of the group $K(\mathscr{C})$, there exist two finite families of exact sequences of modules of type $\mathscr{C}$

$$
(\mathscr{G}_i)0\longrightarrow G'_i\longrightarrow G_i\longrightarrow G''_i\longrightarrow 0
$$

for $i\in I$ and

$$
(\mathscr{H}_j)0\longrightarrow H'_j\longrightarrow H_j\longrightarrow H''_j\longrightarrow 0
$$

for $j\in J$ such that in $\mathbf{Z}_{(\mathscr{C})}$, we have

cl(E) $-$ cl(F) $=\sum_{j\in J}r_{\mathscr{H}_j}-\sum_{i\in I}r_{\mathscr{G}_i}$.

More explicitly, this relation can be written as (7) cl(E) $+\sum_{i\in I}$ cl(G$_i) +\sum_{j\in J}$ cl(H$'_j) +\sum_{j\in J}$ cl(H$''_j)$

= cl(F) $+\sum_{i\in I}$ cl(G$'_i) +\sum_{i\in I}$ cl(G$''_i) +\sum_{j\in J}$ cl(H$_j)$.

Set $G =\bigoplus_{i\in I}G_i, G'=\bigoplus_{i\in I}G'_i$, etc. By passing to the direct sums, we obtain the exact sequences $(\mathscr{G})$ 0 // $G_'^p$ // G $^q$ // $G_{''}$ // $0$,

$(\mathscr{H})$ 0 // $H_'^r$ // H $^s$ // $H_{''}$ // 0 consisting of modules of type $\mathscr{C}$.

Next, let $M_1, . . . ,M_m,N_1, . . . ,N_n$ be A-modules of type $\mathscr{C}$. If we have $\sum^m_{i=1}$ cl(M$_i) =\sum^n_{j=1}$ cl(N$_j)$ in the group $\mathbf{Z}_{(\mathscr{C})}$, then we have $m=n$ and there exists a permutation $\sigma \in \mathfrak{S}_m$ such that cl(M$_i) =$ cl(N$_{\sigma(i)})$ for every $1\leqslant i\leqslant m$ (I, §7, No. 9, p. 95, Proposition 11). Consequently, the modules $\bigoplus^m_{i=1}M_i$ and $\bigoplus^n_{j=1}N_j$ are isomorphic. In particular, from (7), we deduce the existence of an isomorphism from $E\oplus Q$ to $F\oplus P$, where we have set

$$
P = G'\oplus G''\oplus H,Q = G\oplus H'\oplus H''
$$

We also set

$$
L = G'\oplus H',M = G''\oplus H''
$$

The modules L, M, P, Q are of type $\mathscr{C}$, and the sequence $(\mathscr{E})$ 0 // L $^{\lambda}$ // P $^µ$ // M // $0$,

where we define $\lambda$ and $µ$ by

$$
\lambda (g', h') = (g',0, r(h')),µ(g', g'', h) = (g'', s(h))
$$

is exact. We construct an exact sequence $(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0$ in the same way; this concludes the proof.

The set $\mathscr{C}$ is a commutative monoid for the law of composition $(E,E')\mapsto$ cl(E$\oplus E')$. We sometimes denote the group of differences of the commutative monoid $\mathscr{C}$ (I, §2, No. 4, p. 20) by $K'(\mathscr{C})$ and call it the Grothendieck group of $\mathscr{C}$ for direct sums. For any module E of type $\mathscr{C}$, we denote the image of cl(E) in $K'(\mathscr{C})$ by $[E]'_{\mathscr{C}}$.

#### Proposition 6 {#alg-viii-s11-prop-6 .statement}

a) The mapping $E\mapsto [E]'_{\mathscr{C}}$ from $\mathscr{C}$ to $K'(\mathscr{C})$ is a weakly additive function of modules.

b) Let G be an abelian group, and let $\varphi :\mathscr{C}\rightarrow G$ be a weakly additive function of modules. There exists a unique group homomorphism $u: K'(\mathscr{C})\rightarrow$ G such that we have $\varphi (E) =u([E]'_{\mathscr{C}})$ for every module E of type $\mathscr{C}$.

c) Let E and F be modules of type $\mathscr{C}$. We have $[E]'_{\mathscr{C}}= [F]'_{\mathscr{C}}$ if and only if there exists a module M of type $\mathscr{C}$ such that $E\oplus M$ is isomorphic to $F\oplus M$.

Assertion a) is obvious. Assertion b) follows from (I, §2, No. 4, p. 19, Theorem 1) and assertion c) from (I, §2, No. 4, p. 18, Proposition 6).

Since the mapping $E\mapsto [E]_{\mathscr{C}}$ from $\mathscr{C}$ to $K(\mathscr{C})$ is a weakly additive function of modules, we can deduce a homomorphism $u: K'(\mathscr{C})\rightarrow K(\mathscr{C})$ from it. This homomorphism is surjective but is not always an isomorphism (VIII, p. 191, Remark 2).

Let $R_'$ be the subgroup of $\mathbf{Z}_{(\mathscr{C})}$ generated by the elements of the form $r_{\mathscr{E}}$, where $\mathscr{E}$ is a split exact sequence of A-modules of type $\mathscr{C}$, that is, by the elements of the form cl(E$'\oplus E'')-$ cl(E$')-$ cl(E$'')$, where $E'$ and $E''$ are modules of type $\mathscr{C}$. The canonical mapping from $\mathscr{C}$ to the quotient group $\mathbf{Z}^{(\mathscr{C})}/R'$ extends to a group homomorphism $v: K'(\mathscr{C})\rightarrow \mathbf{Z}^{(\mathscr{C})}/R'$. This is an isomorphism. Indeed, the canonical mapping from $\mathscr{C}$ to $K'(\mathscr{C})$ extends to a group homomorphism from $\mathbf{Z}^{(\mathscr{C})}$ to $K'(\mathscr{C})$ whose kernel contains $R'$, and therefore to a homomorphism $v':\mathbf{Z}^{(\mathscr{C})}/R'\rightarrow K'(\mathscr{C})$ by passing to the quotient; it is clear that $v$ and $v'$ are inverse bijections.

An element of $K'(\mathscr{C})$ is called effective if it is of the form $[E]'_{\mathscr{C}}$ for an A-module E of type $\mathscr{C}$. The set of effective elements of $K'(\mathscr{C})$ is denoted by $K'(\mathscr{C})^+$.

### 3. Using Composition Series

Let A be a ring. Let E be an A-module of finite length and S a simple A-module. By the Jordan–Hölder theorem (I, §4, No. 7, p. 43, Theorem 6), the number of quotients of a Jordan–Hölder series of E that are isomorphic to S does not depend on the sequence. We denote it by $`_S(E)$ and call it the multiplicity of S in E. The support of the A-module E is the set of classes of simple A-modules S such that $`_S(E)\not= 0$. When E is semisimple and has finite length, the integer $`_S(E)$ is the length [E : S] of the isotypical component of E of type S (VIII, p. 72), and the notion of support coincides with that introduced in VIII, p. 66.

#### Lemma 1 {#alg-viii-s11-lem-1 .statement}

Let E, $E'$, and $E''$ be A-modules of finite length and

0 // $E_'^i$ // E $^p$ // $E_{''}$ // 0

an exact sequence. We have $`_S(E) =`_S(E') +`_S(E'')$.

Let $Σ'$ and $Σ''$ be Jordan–Hölder series of $i(E')$ and $E/i(E')$, respectively. There exists a Jordan–Hölder series Σ of E whose sequence of quotients can be obtained by juxtaposing the sequence of quotients of Σ and that of $Σ'$ (I, §4, No. 8, p. 44).

#### Proposition 7 {#alg-viii-s11-prop-7 .statement}

Let $\mathscr{C}$ be a hereditary set of classes of modules such that every module of type $\mathscr{C}$ has finite length. Let $\mathscr{S}$ be the set of classes of simple modules belonging to $\mathscr{C}$. Then the family $([S]_{\mathscr{C}})_{S\in\mathscr{S}}$ is a basis of the $\mathbf{Z}$-module $K(\mathscr{C})$, and we have

$$
[E]_{\mathscr{C}}=_S\sum_{\in\mathscr{S}}`_S(E)[S]_{\mathscr{C}} \tag{8}
$$

for every module E of type $\mathscr{C}$.

Formula (8) follows from Proposition 3 applied to a Jordan–Hölder series of E. By Lemma 1, for every element S of $\mathscr{S}$, there exists a $\mathbf{Z}$-linear mapping $\varphi_S$ from $K(\mathscr{C})$ to $\mathbf{Z}$ such that $\varphi_S([E]_{\mathscr{C}}) =`_S(E)$ for every module E of type $\mathscr{C}$. In particular, we have $\varphi_S([S]_{\mathscr{C}}) = 1$ and $\varphi_S([S']_{\mathscr{C}}) = 0$ for every $S'\not= S$ in $\mathscr{S}$. It follows that the elements of the form $[S]_{\mathscr{C}}$ (for $S\in \mathscr{S})$ are linearly independent over $\mathbf{Z}$; these elements generate $K(\mathscr{C})$ by formula (8).

#### Corollary {#alg-viii-s11-n3-cor-1 .statement}

Let E and F be semisimple modules of type $\mathscr{C}$. The module E is isomorphic to F if and only if we have $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ in $K(\mathscr{C})$.

Indeed, we have $[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}`_S(E)[S]_{\mathscr{C}}$ and an analogous formula for F, and E is isomorphic to F if and only if we have $`_S(E) =`_S(F)$ for every $S\in \mathscr{S}$ (VIII, p. 72).

#### Remark {#alg-viii-s11-n3-rem-1 .statement}

The set $K(\mathscr{C})^+$ is the submonoid of $K(\mathscr{C})$ generated by the family

$$
([S]_{\mathscr{C}})_{S\in\mathscr{S}}
$$

### 4. The Grothendieck Group R(A)

Let A be a ring. Let $\mathscr{F}(A)$ be the set of classes of finitely generated A-modules (VIII, p. 51). The classes of the A-modules of finite length form a subset $\mathscr{L}\mathscr{F}(A)$ of $\mathscr{F}(A)$; we have seen that $\mathscr{L}\mathscr{F}(A)$ is a hereditary set of classes of modules. We denote the Grothendieck group associated with $\mathscr{L}\mathscr{F}(A)$ by R(A) and the image in R(A) of the class of an A-module E of finite length by [E].

The results of Subsection 3 imply the following:

a) Let $\mathscr{S}(A)$ be the set of classes of simple A-modules. The family

$([S])_{S\in\mathscr{S}(A)}$ is a basis of the $\mathbf{Z}$-module R(A).

b) Let E and F be semisimple A-modules of finite length. Then E and F are isomorphic if and only if we have [E] = [F] in R(A).

c) Let E be an A-module of finite length and $(E_i)_{0\leqslant i\leqslant n}$ a Jordan–Hölder series of E. Set $F =\bigoplus^n_{i=1}(E_{i-1}/E_i)$. Then F is a semisimple A-module of finite length, and we have [E] = [F] in R(A).

d) Let $`: R(A)\rightarrow \mathbf{Z}$ be the homomorphism characterized by $`([S]) = 1$ for every simple A-module S. We then have $`([E]) =\sum_{S\in\mathscr{S}(A)}`_S(E) =$ long$_A(E)$ for every A-module E of finite length.

If D is a field, then the homomorphism $`: R(D)\rightarrow \mathbf{Z}$ is an isomorphism.

#### Remark 1 {#alg-viii-s11-n4-rem-1 .statement}

Let $\mathscr{S}\mathscr{S}(A)$ be the hereditary set of classes of semisimple A-modules of finite length. By Proposition 7 of VIII, p. 190, the Grothendieck group $K(\mathscr{S}\mathscr{S}(A))$ is a free $\mathbf{Z}$-module whose elements $[S]_{\mathscr{S}\mathscr{S}(A)}$ (for $S\in \mathscr{S}(A))$

form a basis. The canonical homomorphism $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ (VIII, p. 186) is therefore an isomorphism.

#### Remark 2 {#alg-viii-s11-n4-rem-2 .statement}

Let $K'(\mathscr{L}\mathscr{F}(A))$ be the Grothendieck group of $\mathscr{L}\mathscr{F}(A)$ for direct sums (VIII, p. 188). The Krull–Remak–Schmidt theorem (VIII, p. 37) implies that $K'(\mathscr{L}\mathscr{F}(A))$ is a free $\mathbf{Z}$-module with basis the set of classes of indecomposable A-modules of finite length, while $K(\mathscr{L}\mathscr{F}(A))$ admits the set of classes of simple A-modules as a basis.

#### Remark 3 {#alg-viii-s11-n4-rem-3 .statement}

Let E be an A-module of finite length. By c), there exists a semisimple A-module $E'$ of finite length such that $[E] = [E']$, and by b), such a module is defined up to an isomorphism; we sometimes call it a semisimplification of E.

#### Proposition 8 {#alg-viii-s11-prop-8 .statement}

Let A be a principal ideal domain that is not a field, and let L be its field of fractions. There exists an isomorphism $\varphi : R(A)\rightarrow L^*/A^*$ such that we have

$$
\varphi ([A/aA]) =aA^* \tag{9}
$$

for every $a\not= 0$ in A.

Let P be a system of representatives consisting of irreducible elements of A (VII, §1, No. 3, p. 3). The maximal ideals of A are the ideals $pA$ for $p\in P$; every simple A-module is therefore isomorphic to a unique module $A/pA$. Moreover (VII, §1, No. 3, p. 4, Theorem 2), the abelian group $L^*/A^*$ is free and has the family $(pA^*)_{p\in P}$ as a basis. Hence there exists an isomorphism $\varphi$ from R(A) to $L^*/A^*$ characterized by $\varphi ([A/pA]) =pA^*$ for every $p\in P$.

Let $a\not= 0$ in A. There exist an integer $r\geqslant 0$, elements $p_1, . . . , p_r$ of P, and an element $u$ of $A^*$ such that we have $a=up_1\cdots p_r$. The module $A/aA$ admits the composition series defined by

$$
E_0= A/aA,E_i= (p_1\cdots p_iA)/aA(1\leqslant i\leqslant r)
$$

and the module $E_{i-1}/E_i= (p_1\cdots p_{i-1}A)/(p_1\cdots p_iA)$ is isomorphic to $A/p_iA$. We therefore have (VIII, p. 185, Proposition 3)

$$
\varphi ([A/aA]) =\prod_{i=1}^r\varphi ([A/p_iA]) =p_1\cdots p_rA^*=aA^*
$$

#### Remark 4 {#alg-viii-s11-n4-rem-4 .statement}

We keep the assumptions and notation of Proposition 8. Let E be an A-module of finite length, and let $a_1A, . . . , a_nA$ be its invariant factors (VII, §4, No. 5, p. 20). Since E is isomorphic to $\bigoplus_i^n_{=1}A/a_iA$, we have

$$
\varphi ([E]) =\prod_{i=1}^n\varphi ([A/a_iA]) =a_1\cdots a_nA^* \tag{10}
$$

$5)*$ Let A be a Dedekind ring that is not a field (Comm. Alg., VIII, §2, No. 1). By reasoning as in Proposition 8, we can prove the existence of an isomorphism $\varphi$ from R(A) to the group of fractional ideals of A, characterized by $\varphi ([A/\mathfrak{a}]) =\mathfrak{a}$ for every nonzero ideal $\mathfrak{a}$ of $A.*$

Proposition 8 will be used, for example, in the following two cases:

a) Suppose that we have $A =\mathbf{Z}$. The $\mathbf{Z}$-modules of finite length are simply the finite abelian groups. Since $\mathbf{Q}^*$ is the direct product of $\mathbf{Z}^*=$ $\{1,-1\}$ and $\mathbf{Q}^*_+$, we can deduce from Proposition 8 an isomorphism $\varphi '$ from $R(\mathbf{Z})$ to $\mathbf{Q}^*_+$ given by

$\varphi '([G]) =$ Card(G) for every finite abelian group G.

b) Suppose that A is the polynomial ring K[T] in one variable T with coefficients in a commutative field K. Let E be a finite-dimensional vector space over K and $u$ an endomorphism of E. As in VII, §5, No. 1, p. 29, denote by $E_u$ the A-module with underlying additive group E and external law $(p, x)\mapsto p(u)x$. The A-module $E_u$ has finite length. Conversely, every simple A-module is finite-dimensional over K (VII, §4, No. 8, p. 25, Remark 4). Consequently, every A-module of finite length is finite-dimensional over K, hence of the form $E_u$. Moreover (VII, §5, No. 3, p. 32, Corollary 1), the product of the invariant factors of $E_u$ is equal to the characteristic polynomial $\chi_u$ of $u$. Consequently, Proposition 8 gives an isomorphism

$$
\varphi : R(K[T])\rightarrow K(T)^*/K^*
$$

characterized by $\varphi ([E_u]) =\chi_uK^*$ (cf. formula (10)).

### 5. Change of Rings

Let A and B be rings, and let $f: A\rightarrow B$ be a ring homomorphism. Let $\mathscr{C}$ be an additive set of A-modules and $\mathscr{D}$ an additive set of B-modules.

First, suppose that for every B-module M of type $\mathscr{D}$, the A-module $f_*(M)$ obtained by restricting the ring of scalars to A is of type $\mathscr{C}$. Then the mapping from $\mathscr{D}$ to $K(\mathscr{C})$ that sends M to $[f_*(M)]_{\mathscr{C}}$ is an additive function of modules; from it, we deduce a group homomorphism

$$
f_*: K(\mathscr{D})\longrightarrow K(\mathscr{C})
$$

We define a group homomorphism $f_*: K'(\mathscr{D})\rightarrow K'(\mathscr{C})$ likewise.

We now suppose that for every A-module E of type $\mathscr{C}$, the B-module $f^*(E)$ derived from E by extension of scalars via $f$ (II, §5, No. 1, p. 277) is of type $\mathscr{D}$. The mapping from $\mathscr{C}$ to $K'(\mathscr{D})$ that sends an element E of $\mathscr{C}$

to $[f^*(E)]'_{\mathscr{D}}$ is a weakly additive function of modules; it therefore induces a group homomorphism $f^*: K'(\mathscr{C})\rightarrow K'(\mathscr{D})$.

Suppose, furthermore, that for every exact sequence

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

of A-modules of type $\mathscr{C}$, the sequence of B-modules of type $\mathscr{D}$

$$
0\longrightarrow B\otimes_AE'\longrightarrow B\otimes_AE\longrightarrow B\otimes_AE''\longrightarrow 0
$$

is exact. This holds, in particular, in the following cases:

a) The homomorphism $f$ makes B into a projective A-module (II, §3, No. 6, p. 251, Proposition 5 and II, §3, No. 7, p. 257, Corollary $6)*$or, more

generally, a flat (X, §1, n$^o3$, p. 8, définition 1) A-module$*$.

b) $*$The set $\mathscr{C}$ is a set of classes of projective or, more generally, flat (X,

§4, n$^o5$, p. 72, corollaire 2) A-modules$*$.

The mapping from $\mathscr{C}$ to $K(\mathscr{D})$ that sends E to $[f^*(E)]_{\mathscr{D}}$ is then additive. It therefore induces a group homomorphism $f^*: K(\mathscr{C})\rightarrow K(\mathscr{D})$.

### 6. The Grothendieck Group $R_K(A)$

Let K be a commutative field and A a K-algebra. The set of classes of A-modules that are finite-dimensional vector spaces over K is hereditary. The corresponding Grothendieck group is denoted by $R_K(A)$. It is a free $\mathbf{Z}$-module with basis the family $([S])_{S\in\mathscr{S}}$, where $\mathscr{S}$ is the set of classes of simple A-modules that are finite-dimensional over K. There exists a homomorphism

dim$: R_K(A)\longrightarrow \mathbf{Z}$

characterized by dim([E]) = [E : K] for every A-module E that is finite-dimensional over K. When A = K, it is an isomorphism. The submonoid of effective elements is denoted by $R_K(A)^+$.

#### Lemma 2 {#alg-viii-s11-lem-2 .statement}

Let M and $M'$ be A-modules that are finite-dimensional vector spaces over K. The supports (VIII, p. 190) of M and $M'$ are disjoint if and only if there exists an $a\in A$ such that $a_M= 0_M$ and $a_{M'}= 1_{M'}$.

Suppose that there exists an $a\in A$ such that $a_M= 0_M$ and $a_{M'}= 1_{M'}$. Let S be a simple A-module. If cl(S) belongs to the support $\mathscr{S}_M$ of M, then the A-module S is isomorphic to one of the quotients of a Jordan–Hölder series of M and we have $a_S= 0_S$. Likewise, if cl(S) belongs to the support $\mathscr{S}_{M'}$ of M’, then we have $a_S= 1_S$. It follows that $\mathscr{S}_M$ and $\mathscr{S}_{M'}$ are disjoint.

Conversely, suppose that the sets $\mathscr{S}_M$ and $\mathscr{S}_{M'}$ are disjoint. They are finite because M and $M'$ are finite-dimensional over K. Every simple A-module S whose class belongs to $\mathscr{S}_M\cup \mathscr{S}_{M'}$ is finite-dimensional over K and a fortiori over the field End$_A(S)$. By Corollary 1 of Proposition 4 (VIII, p. 83), there exists an element $b\in A$ such that we have $b_S= 0_S$ (resp. $b_S= 1_S)$ for every simple A-module S whose class belongs to $\mathscr{S}_M$ (resp. $\mathscr{S}_{M'})$. Let $(M_i)_{0\leqslant i\leqslant n}$ be a Jordan–Hölder series of M. By the above, we have $bM_i\subset M_{i+1}$ for $0\leqslant i < n$ and therefore $(b^n)_M= 0_M$. The existence of a natural number $m$ such that $((1-b)^m)_{M'}= 0_{M'}$ is proved in the same way. Set $P(X) = 1-(1-X^n)^m$ and $a= P(b)$. The polynomial P(X) is a multiple of $X^n$, so we have $a_M= 0_M$, while the polynomial $1-P(X)$ is a multiple of $(1-X)^m$, so we have $a_{M'}= 1_{M'}$. This concludes the proof.

Let L be an extension of K. If M is an A-module that is finite-dimensional over K, then $M_{(L)}$ is an $A_{(L)}$-module that is finite-dimensional over L. Moreover, for every exact sequence

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

of A-modules, the sequence of $A_{(L)}$-modules

$$
0\longrightarrow M'_{(L)}\longrightarrow M_{(L)}\longrightarrow M''_{(L)}\longrightarrow 0
$$

deduced from it by extension of scalars is exact (II, §7, No. 7, p. 308, Proposition 14). Hence there exists a unique ring homomorphism $u: R_K(A)\rightarrow$ $R_L(A_{(L)})$ such that $u([M]) = [M_{(L)}]$ for every A-module M that is finite-dimensional over K (No. 5).

#### Theorem 1 {#alg-viii-s11-thm-1 .statement}

The homomorphism $u: R_K(A)\rightarrow R_L(A_{(L)})$ defined above is injective. Let $\xi$ be an element of $R_K(A)$. Then $\xi$ is effective if and only if $u(\xi )$ is.

#### Lemma 3 {#alg-viii-s11-lem-3 .statement}

Let S and T be two nonisomorphic simple A-modules that are finite-dimensional over K. The supports of the $A_{(L)}$-modules $S_{(L)}$ and $T_{(L)}$ are disjoint.

By Lemma 2, there exists an element $a\in A$ such that $a_S= 0$ and $a_T= 1$. The element $1\otimes a$ of $A_{(L)}$ acts as 0 on $S_{(L)}$ and as 1 on $T_{(L)}$. By Lemma 2, the supports of the $A_{(L)}$-modules $S_{(L)}$ and $T_{(L)}$ are disjoint.

Let us prove Theorem 1. Let $\mathscr{S}$ be the set of classes of simple A-modules that are finite-dimensional over K. The family $([S])_{S\in\mathscr{S}}$ is a basis of the $\mathbf{Z}$-module $R_K(A)$. Let $S\in \mathscr{S}$. The $A_{(L)}$-module $S_{(L)}$ is not zero, so its support is not empty. Let $S'$ be an element of this support. By Lemma 1 of VIII, p. 190, there exists a homomorphism $f_{S'}: R_L(A_{(L)})\rightarrow \mathbf{Z}$ such that $f_{S'}([E]) =`_{S'}(E)$ for every $A_{(L)}$-module E that is finite-dimensional over L. We have $f_{S'}([S_{(L)}])\not= 0$ by construction and $f([T_{(L)}]) = 0$ for every $T\in \mathscr{S}\{S\}$ by Lemma 3. We have therefore proved that the elements of $R_L(A_{(L)})$ of the form $[S_{(L)}]$ for $S\in \mathscr{S}$ are linearly independent over $\mathbf{Z}$. It follows that the homomorphism $u$ is injective.

Let $S\in \mathscr{S}$, and let $S'$ be an element of the support of $S_{(L)}$. For every $\xi \in R_K$(A), the coordinate of $\xi$ of index [S] in the basis $([S])_{S\in\mathscr{S}}$ is $f_{S'}(u(\xi ))/[S_{(L)}: S']$. It follows that if $u(\xi )$ is effective, then so is $\xi$.

### 7. Multiplicative Structure on $K(\mathscr{C})$

Let K be a commutative ring and A a bigebra over the ring K (III, §11, No. 4, p. 585), with coproduct $c$ and counit $\gamma$. Unless stated otherwise, the tensor products are over K. Let E and F be (left) A-modules. The tensor product $E\otimes F$ is endowed with an $(A\otimes$ A)-module structure characterized by the formula

$$
(a\otimes b)(x\otimes y) =ax\otimes by \tag{11}
$$

for $a, b\in A,x\in E$, and $y\in F$. Using the homomorphism $c: A\rightarrow A\otimes A$, we deduce from this $(A\otimes$ A)-module an A-module $c_*(E\otimes F)$ (II, §1, No. 13, p. 221). More precisely, let $a\in A$; if $c(a) =\sum_ia_i\otimes b_i$, then we have

$$
a(x\otimes y) =\sum_ia_ix\otimes b_iy \tag{12}
$$

for $x\in E$ and $y\in F$. By abuse of notation, we also denote the resulting A-module by $E\otimes F$. It follows immediately from the coassociativity of $c$ that the canonical isomorphism of K-modules

$$
\varphi : (E\otimes F)\otimes G\longrightarrow E\otimes (F\otimes G)
$$

is A-linear for all A-modules E, F, and G. Likewise, if the bigebra A is cocommutative, then the canonical isomorphism from $E\otimes F$ to $F\otimes E$ is A-linear. Finally, let $K_{\gamma}$ be the A-module with underlying group K and external law $(a, x)\mapsto \gamma (a)x$. The canonical isomorphism from $K\otimes E$ (resp. $E\otimes K)$ to E is an isomorphism of A-modules from $K_{\gamma}\otimes E$ (resp. $E\otimes K_{\gamma})$ to E.

#### Proposition 9 {#alg-viii-s11-prop-9 .statement}

Let K be a commutative ring, A a bigebra over K with counit $\gamma$, and $\mathscr{C}$ an additive set of classes of A-modules with the following properties:

(i) Every A-module of type $\mathscr{C}$ is a projective $(*$or, more generally, flat$*)$ K-module.

(ii) If the A-modules E and F are of type $\mathscr{C}$, then so is the A-module $E\otimes F$.

(iii) The A-module $K_{\gamma}$ defined above is of type $\mathscr{C}$. Then there exists a unique ring structure on the additive group $K(\mathscr{C})$ whose multiplication satisfies

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}
$$

for all A-modules E and F of type $\mathscr{C}$. The unit element of $K(\mathscr{C})$ is $[K_{\gamma}]_{\mathscr{C}}$. If the bigebra A is cocommutative, then the ring $K(\mathscr{C})$ is commutative.

Endowed with the law of composition given by $(E,F)\mapsto$ cl(E $\otimes F)$, the set $\mathscr{C}$ is a monoid with unit element cl(K$_{\gamma})$. Consequently, $\mathbf{Z}^{(\mathscr{C})}$ is canonically endowed with the structure of a ring with multiplication characterized by the formula

(13) cl(E) cl(F) = cl(E $\otimes F)$

and unit element cl(K$_{\gamma})$ (III, §2, No. 6, p. 446).

Given an A-module F of type $\mathscr{C}$ and an exact sequence

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

of A-modules of type $\mathscr{C}$, the sequence

$$
(\mathscr{E}\otimes F)0\longrightarrow E'\otimes F\longrightarrow E\otimes F\longrightarrow E''\otimes F\longrightarrow 0
$$

deduced from $(\mathscr{E})$ is exact because F is projective $(*$or, more generally, flat$*)$ over K (II, §3, No. 6, p. 251, Proposition 5 and II, §3, No. 7, p. 257, Corollary 6). In the notation of No. 2, we then have

(14) $r_{\mathscr{E}\otimes F}=r_{\mathscr{E}}$ cl(F) $$. It follows that the subgroup R of $\mathbf{Z}_{(\mathscr{C})}$ generated by the elements of the form $r$ is a right ideal of the ring $\mathbf{Z}_{(\mathscr{C})}$, and one proves likewise that it is a left ideal of$^{\mathscr{E}}\mathbf{Z}^{(\mathscr{C})}$. By definition, $K(\mathscr{C})$ is the quotient group $\mathbf{Z}^{(\mathscr{C})}/R$; hence there exists a unique ring structure on $K(\mathscr{C})$ whose multiplication satisfies $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}$ for all A-modules E and F of type $\mathscr{C}$. Its unit element is $[K_{\gamma}]$.

When the bigebra A is cocommutative, the monoid $\mathscr{C}$ is commutative; it follows that the ring $\mathbf{Z}^{(\mathscr{C})}$ and the quotient ring $K(\mathscr{C})$ are commutative.

#### Remark {#alg-viii-s11-n7-rem-1 .statement}

Under only assumptions (i) and (ii) of Proposition 9, the Grothendieck group $K'(\mathscr{C})$ for direct sums (VIII, p. 188) has a unique ring structure whose multiplication satisfies $[E]'_{\mathscr{C}}[F]'_{\mathscr{C}}= [E\otimes F]'_{\mathscr{C}}$. Its unit element is $[K_{\gamma}]'_{\mathscr{C}}$. The ring $K'(\mathscr{C})$ is commutative if the bigebra A is cocommutative. The proof is analogous to that of Proposition 9 because the group $K'(\mathscr{C})$ can be identified with $\mathbf{Z}_{(\mathscr{C})}/R_'$, where $R_'$ is the subgroup of $\mathbf{Z}_{(\mathscr{C})}$ generated by the elements of the form cl(E$'\oplus E'')-$ cl(E$')-$ cl(E$'')$ (loc. cit.).

Under assumptions (i), (ii), and (iii) of Proposition 9, the ring $K(\mathscr{C})$ is called the Grothendieck ring of $\mathscr{C}$. These conditions are, in particular, satisfied when K is a field and $\mathscr{C}$ is the set of classes of A-modules that are finite-dimensional over K. Consequently, we have the following.

#### Corollary {#alg-viii-s11-n7-cor-1 .statement}

Let A be a bigebra with counit $\gamma$ over a commutative field K. Then there exists a unique ring structure on the additive group $R_K(A)$ whose multiplication satisfies

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_KF]_{\mathscr{C}}
$$

for all A-modules E and F that are finite-dimensional over K. The unit element of $R_K(A)$ is $[K_{\gamma}]_{\mathscr{C}}$. If the bigebra A is cocommutative, then the ring $R_K(A)$ is commutative.

#### Example 1 {#alg-viii-s11-n7-exa-1 .statement}

Let K be a commutative field. Let G be a group, and let K[G] be the algebra of the group G. We identify G with its canonical image in K[G] (III, §2, No. 6, p. 446).

We endow K[G] with the structure of a bigebra with coproduct $c$ and counit $\gamma$ given by

$$
c(g) =g\otimes g ,\gamma (g) = 1(g\in G) \tag{15}
$$

Let E and F be K[G]-modules; by formula (12), the K[G]-module structure on $E\otimes F$ is given by

$$
g(x\otimes y) =gx\otimes gy(g\in G, x\in E, y\in F) \tag{16}
$$

The K[G]-module $K_{\gamma}$ is the vector space K endowed with the action of G defined by $g\lambda =\lambda$ for $g\in G$ and $\lambda \in K$.

The ring $R_K(K[G])$ is also denoted by $R_K(G)$. It is commutative; its multiplication is given by $[E] [F] = [E\otimes_KF]$, and the unit element of $R_K(G)$ is $[K_{\gamma}]$.

#### Example 2 {#alg-viii-s11-n7-exa-2 .statement}

Let $\mathfrak{g}$ be a Lie algebra over a commutative field K and $U(\mathfrak{g})$ its enveloping algebra; we identify $\mathfrak{g}$ with its canonical image in $U(\mathfrak{g}) ($Lie, I, §2, No. 7, p. 39, Corollary 2). We endow $U(\mathfrak{g})$ with the structure of a bigebra with coproduct $c$ and counit $\gamma$ given by

$$
c(\xi ) =\xi \otimes 1 + 1\otimes \xi ,\gamma (\xi ) = 0 \tag{17}
$$

for $\xi \in \mathfrak{g}($Lie, II, §1, No. 4, p. 115).

Let E and F be $U(\mathfrak{g}$)-modules; by formula (17), the $U(\mathfrak{g}$)-module structure on $E\otimes F$ is characterized by

$$
\xi (x\otimes y) =\xi x\otimes y+x\otimes \xi y \tag{18}
$$

for $\xi \in \mathfrak{g},x\in E$, and $y\in F$.

The Grothendieck ring $R_K(U(\mathfrak{g}))$ is also denoted by $\mathscr{R}(\mathfrak{g})$ in Lie, VIII,

§7, No. 6, p. $139.*$

Let A be a commutative ring. We can view A as a bigebra that is cocommutative over itself, with coproduct the natural isomorphism from A to $A\otimes_AA$ and counit Id$_A$ (III, §11, No. 4, p. 585). By Proposition 9, we obtain the following result.

#### Proposition 10 {#alg-viii-s11-prop-10 .statement}

Let A be a commutative ring, and let $\mathscr{C}$ be an additive set of classes of A-modules satisfying the following three conditions:

(i) Every A-module of type $\mathscr{C}$ is projective $(*$or, more generally, flat$*)$.

(ii) If E and F are A-modules of type $\mathscr{C}$, then the A-module $E\otimes_AF$ is also of type $\mathscr{C}$.

(iii) The A-module A is of type $\mathscr{C}$. Then there exists a unique ring structure on the additive group $K(\mathscr{C})$ satisfying $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_AF]_{\mathscr{C}}$ for every pair E, F of A-modules of type $\mathscr{C}$. The unit element of $K(\mathscr{C})$ is $[A]_{\mathscr{C}}$.

### 8. The Grothendieck Group $K_0(A)$

Let A be a ring. The set $\mathscr{P}(A)$ of classes of finitely generated projective A-modules is additive; we denote the Grothendieck group $K(\mathscr{P}(A))$ by $K_0(A)$.

For the law of composition $(E,E')\mapsto$ cl(E $\oplus E')$, the set $\mathscr{P}(A)$ is a commutative monoid. Moreover, every exact sequence of projective A-modules

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

splits (II, §2, No. 2, p. 231, Proposition 4), so that E is isomorphic to $E'\oplus E''$. The mapping $E\mapsto [E]$ from $\mathscr{P}(A)$ to $K_0(A)$ therefore defines an isomorphism from the group of differences of the monoid $\mathscr{P}(A)$ to $K_0(A)$ (VIII, p. 188).

For every finitely generated projective module P, there exists a finitely generated projective module $P'$ such that $P\oplus P'$ is free (II, §2, No. 2, p. 232, Corollary 1). Let E and F be finitely generated projective A-modules; by I, §2, No. 4, p. 18, Proposition 6, we have [E] = [F] in $K_0(A)$ if and only if there exists a finitely generated free A-module L such that the A-modules $E\oplus L$ and $F\oplus L$ are isomorphic. We then say that E and F are stably isomorphic; this does not necessarily imply that E and F are isomorphic (VIII, p. 207, Exercise 2 and VIII, p. 210, Exercise 14).

When the ring A is commutative, there exists a commutative ring structure on the additive group $K_0(A)$ whose multiplication is characterized by the formula $[E]_{\mathscr{P}(A)}[F]_{\mathscr{P}(A)}= [E\otimes_AF]_{\mathscr{P}(A)}$ (VIII, p. 199, Proposition 10).

#### Remark {#alg-viii-s11-n8-rem-1 .statement}

Let A be a semisimple ring. Every A-module is then semisimple and projective (VIII, p. 138, Proposition 4); we therefore have the equality

$$
\mathscr{L}\mathscr{F}(A) =\mathscr{S}\mathscr{S}(A) =\mathscr{P}(A)
$$

(cf. No. 4 for the definitions of $\mathscr{L}\mathscr{F}(A)$ and $\mathscr{S}\mathscr{S}(A))$. We therefore have $K_0(A) = R(A)$ by the definitions of these Grothendieck groups.

#### Example {#alg-viii-s11-n8-exa-1 .statement}

If every finitely generated projective A-module is free, then the rank defines an isomorphism from $K_0(A)$ to $\mathbf{Z}$. This is, in particular, the case when A is a principal ideal domain (VII, §1, No. 3, p. 15, Corollary 3) or when A is a local ring (VIII, p. 36, Corollary 6).

### 9. The Grothendieck Group $K_0(A)$ of an Artinian Ring

Let A be a left Artinian ring. Let $\mathfrak{r}$ be its radical; it is a nilpotent two-sided ideal of A, and the ring $A/\mathfrak{r}$ is semisimple (VIII, p. 173, Proposition 1). By the corollary of VIII, p. 176, the mapping $P\mapsto$ cl(P$/\mathfrak{r}P)$ is an isomorphism from the monoid $\mathscr{P}(A)$ to the monoid $\mathscr{P}(A/\mathfrak{r})$. We deduce from it a group isomorphism $\gamma$ from $K_0(A)$ to $K_0(A/\mathfrak{r})$ characterized by the relation $\gamma ([P]_{\mathscr{P}(A)}) = [P/\mathfrak{r}P]_{\mathscr{P}(A/\mathfrak{r})}$ for every finitely generated projective A-module P.

Since the ring $A/\mathfrak{r}$ is semisimple, the remark above implies the equality $R(A/\mathfrak{r}) = K_0(A/\mathfrak{r})$. The modules of finite length over the ring $A/\mathfrak{r}$ are simply the semisimple modules of finite length over the ring A (VIII, p. 174, Proposition 2); consequently, we can identify $\mathscr{L}\mathscr{F}(A/\mathfrak{r})$ with $\mathscr{S}\mathscr{S}(A)$ and $R(A/\mathfrak{r})$ with $K(\mathscr{S}\mathscr{S}(A))$. We denote by $\delta$ the homomorphism $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ from $R(A/\mathfrak{r}) = K(\mathscr{S}\mathscr{S}(A))$ to $R(A) = K(\mathscr{L}\mathscr{F}(A))$ (VIII, p. 191, Remark 1); it is an isomorphism. Finally, we have $\mathscr{P}(A)\subset \mathscr{L}\mathscr{F}$(A), and we set $\varepsilon =$ $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{P}(A)}$. We have defined a diagram

$K_0(A)\gamma$ // $K_0(A/\mathfrak{r}) = R(A/\mathfrak{r})$

$^{\varepsilon}$  $^{\delta}$

R(A) .

We denote the (finite) set of classes of simple A-modules by $\mathscr{S}$; for every $\lambda \in \mathscr{S}$, choose a module $S_{\lambda}$ of class $\lambda$ and a projective cover $(P_{\lambda}, u_{\lambda})$ of $S_{\lambda}$ (VIII, p. 175, Proposition 4). It follows from Proposition 6 of VIII, p. 176 that $K_0(A)$ is a free $\mathbf{Z}$-module with basis the family $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$. Moreover, since $S_{\lambda}$ is isomorphic to $P_{\lambda}/\mathfrak{r}P_{\lambda}$ (VIII, p. 176$),\gamma$ transforms the basis $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$ of $K_0(A)$ into the basis $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ of $R(A/\mathfrak{r})$. The isomorphism $\delta$ transforms the basis $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ of $R(A/\mathfrak{r})$ into the basis $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ of R(A).

The Cartan matrix of A is the matrix $(a_{\lambda µ})$ of the homomorphism of $\mathbf{Z}$-modules $\varepsilon : K_0(A)\rightarrow R(A)$ with respect to bases $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$ of $K_0(A)$ and $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ of R(A). By definition, we have (19) $[P_µ] =_{\lambda}\sum_{\in\mathscr{S}}a_{\lambda µ}[S_{\lambda}](µ\in \mathscr{S})$

in the group R(A). In other words, $a_{\lambda µ}$ is the number of quotients isomorphic to $S_{\lambda}$ in a Jordan–Hölder series of the A-module $P_µ$.

Set $\pi =\varepsilon \circ \gamma^{-1}\circ \delta^{-1}$; it is an endomorphism of the group R(A). If M is a finitely generated semisimple A-module and $(P, u)$ a projective cover of M, then we have $\pi ([M]) = [P]$. By formula (19), the matrix of $\pi$ with respect to the basis $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ of R(A) is simply the Cartan matrix of A.

### 10. Change of Rings for $K_0(A)$

Let A and B be rings. Let $f: A\rightarrow B$ be a ring homomorphism. If P is a finitely generated projective A-module, then the B-module $f^*(P) = B\otimes_AP$ is projective and finitely generated (II, §5, No. 2, p. 281, Corollary). The mapping $P\mapsto$ cl($f^*(P))$ is a homomorphism from the monoid $\mathscr{P}(A)$ to the monoid $\mathscr{P}(B)$ and therefore defines a homomorphism $f^*: K_0(A)\rightarrow$

$K_0(B)$ characterized by the relation $f^*([P]_{\mathscr{P}(A)}) = [f^*(P)]_{\mathscr{P}(B)}$ for every finitely generated projective A-module P. If $g: B\rightarrow C$ is a second ring homomorphism, then it follows from the transitivity of the extension of scalars (II, §5, No. 1, p. 278, Proposition 2) that the homomorphisms $(g\circ f)^*$ and $g^*\circ f^*$ from $K_0(A)$ to $K_0(C)$ are equal.

Suppose that $f$ makes B into a finitely generated projective left A-module. Let Q be a finitely generated projective left B-module. Then Q is a direct factor of a finitely generated free B-module that is projective and finitely generated over A. Consequently, the A-module $f_*(Q)$ obtained from Q by restriction of scalars is projective and finitely generated. As above, we deduce a homomorphism $f_*: K_0(B)\rightarrow K_0(A)$ characterized by the relation $f_*([Q]_{\mathscr{P}(B)}) = [f_*(Q)]_{\mathscr{P}(A)}$ for every finitely generated projective B-module Q. If $g: B\rightarrow C$ is a ring homomorphism that makes C into a finitely generated projective B-module, then the homomorphisms $(g\circ f)_*$ and $f_*\circ g_*$ from $K_0(C)$ to $K_0(A)$ are equal.

### 11. Frobenius Reciprocity

Let A be a semisimple ring. Let $f$ be a homomorphism from A to a semisimple ring B. Let S be a simple A-module and T a simple B-module, and let D and E be the centralizers of S and T, respectively. By Schur’s lemma (VIII, p. 47, Corollary), D and E are fields. Let H be the set of A-linear homomorphisms from S to $f_*(T)$. We endow H with an $(E$, D)-bimodule structure with external laws $(e, u)\mapsto e\circ u$ and $(d, u)\mapsto u\circ d$ for $e\in E,u\in H$, $d\in D$.

#### Proposition 11 {#alg-viii-s11-prop-11 .statement}

a) The multiplicity $[f_*(T) : S]$ of the simple A-module S in the semisimple A-module $f_*(T)$ is equal to the dimension of H viewed as a right vector space over D.

b) The multiplicity $[f^*(S) : T]$ is finite and equal to the dimension of H viewed as a left vector space over E.

Assertion a) follows from formula (11) of VIII, p. 72.

The B-module $f^*(S)$ is semisimple and finitely generated, hence has finite length. By formula (12) of loc. cit., we have

(20) $[f^*(S) : T] =$ dim$_E$ Hom$_B(f^*(S),T)$.

Now, in II, §5, No. 1, p. 277–278, formula (2) and Remark 2, we defined an E-linear bijection from Hom$_A(S, f_*(T))$ to Hom$_B(f^*(S),T)$. Assertion b) then follows from formula (20).

Corollary (Frobenius reciprocity). — Suppose that A and B are semisimple algebras that are finite-dimensional over a commutative field K and that $f$ is K-linear. Then the K-vector spaces S, T, D, E, and H are finite-dimensional, and we have the equalities

$$
[f_*(T) : S][D : K] = [f^*(S) : T][E : K] = [H : K] \tag{21}
$$

In particular, when K is algebraically closed, we have D = E = K and

$$
[f_*(T) : S] = [f^*(S) : T] = [H : K] \tag{22}
$$

Since A-module S is simple, it is monogenous, and D is a linear subspace of Hom$_K(S,S)$; hence S and D are finite-dimensional over K. For an analogous reason, T and E are finite-dimensional over K. Finally, H is a linear subspace of Hom$_K(S,T)$; it is therefore also finite-dimensional. Formula (21) then follows from Proposition 11 because the dimension of H over K is equal to [H : D][D : K] and to [H : E][E : K] (II, §1, No. 13, p. 222, Proposition 25). By Theorem 1 of VIII, p. 47, if K is algebraically closed, we have D = E = K. The second part of the corollary then follows from the first.

Let A and B be semisimple algebras that are finite-dimensional over a commutative field K, and let $f$ be a homomorphism of K-algebras from A to B.

Let $\mathscr{S}(A)$ be the set of classes of simple A-modules; for every $\lambda \in \mathscr{S}$ (A), let $S_{\lambda}$ be a module of class $\lambda$ and $D_{\lambda}$ its centralizer. Then $D_{\lambda}$ is an algebra of finite degree over K; we denote this degree by $d_{\lambda}$. We define $\mathscr{S}$(B), $T_µ$, $E_µ$, and $e_µ$ for $µ$ in $\mathscr{S}(B)$ analogously. The Grothendieck group $K_0(A)$ has

the family $([S_{\lambda}])_{\lambda\in\mathscr{S}(A)}$ as a basis, and $K_0(B)$ has $([T_µ])_{µ\in\mathscr{S}(B)}$ as a basis. Let $(a_{µ\lambda})$ be the matrix of $f^*: K_0(A)\rightarrow K_0(B)$ and $(b_{\lambda µ})$ the matrix of $f_*: K_0(B)\rightarrow K_0(A)$ with respect to these bases. By definition, we have

$$
a_{µ\lambda}= [f^*(S_{\lambda}) : T_µ],b_{\lambda µ}= [f_*(T_µ) : S_{\lambda}] \tag{23}
$$

for $\lambda$ in $\mathscr{S}(A)$ and $µ$ in $\mathscr{S}(B)$. We denote the dimension of the vector space Hom$_A(S_{\lambda}, f_*(T_µ))$ over the field K by $h_{\lambda µ}$. By the corollary above, we have

$$
h_{\lambda µ}=e_µa_{µ\lambda}=d_{\lambda}b_{\lambda µ} \tag{24}
$$

When the field K is algebraically closed, we have $d_{\lambda}=e_µ= 1$; consequently, we have

$$
a_{µ\lambda}=b_{\lambda µ}=h_{\lambda µ} \tag{25}
$$

In other words, the matrices of $f_*$ and $f^*$ with respect to the given bases of $K_0(A)$ and $K_0(B)$ are each other’s transposes.

### 12. The Case of Simple Rings

Let A and B be simple rings and $f$ a homomorphism from A to B. Let S be a simple A-module and T a simple B-module. We set

(26) $i(f) = [f^*(S) : T] =$ long$_B(f^*(S))$;

we call the cardinal $i(f)$ the index of $f$. When A is a subring of B and $f$ is the canonical injection of A into B, we write $i(B,A)$ instead of $i(f)$, and we call this cardinal the index of A in B. We define the height $h(f)$ of $f$ analogously:

(27) $h(f) = [f_*(T) : S] =$ long$_A(f_*(T))$.

When A is a subring of B and $f$ the canonical injection of A into B, we write $h(B,A)$ for $h(f)$, and we call it the height of A in B.

The A-module S is monogenous, hence so is the B-module $f^*(S) = B\otimes_AS$. It follows that $i(f)$ is finite and therefore that it is an integer. Let M be an A-module. Denote its length by $\mathfrak{a}$; then M is isomorphic to $S^{(\mathfrak{a})}$. Consequently, the B-module $f_*(M)$ is isomorphic to $f_*(S)^{(\mathfrak{a})}$. By the definition of $i(f)$, we therefore have

(28) long$_B(f^*(M)) =i(f)$ long$_A(M)$.

The $\mathbf{Z}$-modules $K_0(A)$ and $K_0(B)$ are free of dimension 1, with respective bases [S] and [T], and we have

$$
f^*([S]) =i(f)[T] \tag{29}
$$

Let us take, in particular, $M = A_s$; then $f^*(A_s) = B\otimes_AA_s$ is isomorphic to $B_s$ (II, §3, No. 4, p. 249), so

(30) $i(f) =$ long(B)$/$ long(A) $$.

By Wedderburn’s theorem (VIII, p. 120, Theorem 1), there exist integers $m\geqslant$ 1 and $n\geqslant 1$ and fields D and E such that A is isomorphic to $\mathbf{M}_m(D)$ and B to $\mathbf{M}_n(E)$. By formula (30), we have $i(f) =n/m$; in particular, $m$ divides $n$.

Let N be an B-module; denote its length by $\mathfrak{a}$. Then N is isomorphic to $T^{(\mathfrak{a})}$, so the A-module $f_*(N)$ is isomorphic to $f_*(T)^{(\mathfrak{a})}$; by the definition of $h(f)$, we have

(31) long$_A(f_*(N)) =h(f)$ long$_B(N)$.

We have seen (VIII, p. 124, Proposition 5) that $f$ makes B into a free A-module and that all bases of this module have the same cardinal, denoted by $[B : A]_s$ and called the (left) degree of B over A. The A-module $f_*(B_s)$ is isomorphic to $A_s^{[B:A]_s}$, so has length $[B : A]_s$ long(A). By formula (30) and formula (31) applied to the specific case $N = B_s$, we therefore have

$$
[B : A]_s=i(f)h(f) \tag{32}
$$

Now suppose that B is a finitely generated A-module, that is, that $[B : A]_s$ is finite. Then $h(f)$ is finite by formula (32). We defined (VIII, p. 202) a group homomorphism $f_*$ from $K_0(B)$ to $K_0(A)$; we have

$$
f_*([T]) =h(f)[S] \tag{33}
$$

Suppose that A and B are finite-dimensional algebras over a commutative field K and that $f$ is K-linear. As before, there exist integers $m\geqslant 1$ and $n\geqslant 1$, K-algebras D and E that are fields, and K-algebra isomorphisms from A to $\mathbf{M}_m(D)$ and from B to $\mathbf{M}_n(E)$. Set $d= [D : K]$ and $e= [E : K]$. We then have the relations

$_2$ 2 $n^2e$

$$
[A : K] =md ,[B : K] =ne ,[B : A]_s=
$$

$$
m^2d
$$

and, by formulas (30) and (32), the relations

$$
nne
$$

$$
i(f) =,h(f) =
$$

$$
mmd
$$

When the field K is algebraically closed, we have $d=e= 1$ and therefore $i(f) =h(f)$ and $[B : A]_s=i(f)^2$.

Let A, B, and C be simple rings, and let $f: A\rightarrow B$ and $g: B\rightarrow C$ be homomorphisms. Let S be a simple A-module. The C-modules $(g\circ f)^*(S)$ and $g^*(f^*(S))$ are isomorphic; therefore, by formulas (26) and (28), we have

$i(g\circ f) =$ long$_C(g^*(f^*(S))) =i(g)$ long$_B(f^*(S)) =i(g)i(f)$.

We can prove the equality $h(g\circ f) =h(g)h(f)$ likewise. When A is a subring of B and B is a subring of C, and we take the canonical injections for $f$ and $g$, these equalities give

$$
i(C,A) =i(C,B)i(B,A),h(C,A) =h(C,B)h(B,A) \tag{34}
$$

#### Proposition 12 {#alg-viii-s11-prop-12 .statement}

Let B be a simple ring and A a simple subring of B. Suppose that B is a finitely generated left A-module. Let M be a nonzero finitely generated left B-module. Set $A'=$ End$_A(M)$ and $B'=$ End$_B(M)$. Then $B'$ is a subring of $A'$, the rings $A'$ and $B'$ are simple, $A'$ is a finitely generated left $B'$-module, and we have the equalities

$$
i(A',B') =h(B,A),h(A',B') =i(B,A),[A': B']_s= [B : A]_s
$$

By Proposition 4 of VIII, p. 123, the ring $A'$ is simple, M is an $A'$-module of finite length, and we have

long$_A(M) =$ long(A$')$, long$_{A'}(M) =$ long(A)$$. For the same reasons, the ring $B'$ is simple, and we have

long$_B(M) =$ long(B$')$, long$_{B'}(M) =$ long(B)$$. By formulas (31) and (30), we therefore have

$h(B,A) =$ long$_A(M)/$ long$_B(M) =$ long(A$')/$ long(B$') =i(A',B')$; the equality $h(A',B') =i(B,A)$ can be established analogously. From this, we deduce

$$
[A': B']_s=i(A',B')h(A',B') =h(B,A)i(B,A) = [B : A]_s
$$

using formula (32). In particular, $A'$ is a finitely generated left $B'$-module.

### Exercises {#alg-viii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
