---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Semisimple Modules
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.55-A VIII.75
pdf_pages: 0072-0092
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules
      page: 55
      pdf_page: 72
    - "no": 2
      title: The homomorphism $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$
      page: 57
      pdf_page: 74
    - "no": 3
      title: Some Operations on Modules
      page: 58
      pdf_page: 75
    - "no": 4
      title: Isotypical Modules
      page: 61
      pdf_page: 78
    - "no": 5
      title: Description of an Isotypical Module
      page: 62
      pdf_page: 79
    - "no": 6
      title: Isotypical Components of a Module
      page: 65
      pdf_page: 82
    - "no": 7
      title: Description of a Semisimple Module
      page: 69
      pdf_page: 86
    - "no": 8
      title: Multiplicities and Lengths in Semisimple Modules
      page: 71
      pdf_page: 88
statements: 43
exercises: 8
content_sha256: 7c129df3e6bb57216018bf396d3ebcfea307672b0f7b39a7d0b5865974a0a165
---

## § 4. SEMISIMPLE MODULES

### 1. Semisimple Modules

#### Definition 1 {#alg-viii-s4-def-1 .statement tag=0040}

A module is called semisimple if it is the direct sum of a family of simple modules.[^1].

A multimodule is called semisimple if it is the direct sum of a family of simple multimodules (cf. I, §4, No. 4, p. 37, Definition 7).

An A-module M is semisimple if and only if it is semisimple when viewed as a module over its ring of homotheties $A_M$.

#### Example 1 {#alg-viii-s4-n1-exa-1 .statement tag=0041}

A module reduced to 0 and a simple module are semisimple modules.

#### Example 2 {#alg-viii-s4-n1-exa-2 .statement tag=0042}

If A is a field, then every A-module is semisimple by Theorem 1 of II, §7, No. 1, p. 292. This shows that, in general, a semisimple module decomposes in several ways into a direct sum of simple submodules (see, however, Corollary 2 of VIII, p. 68).

#### Example 3 {#alg-viii-s4-n1-exa-3 .statement tag=0043}

Let A be a principal ideal domain, and let P be a system of representatives consisting of irreducible elements of A (VII, §1, No. 3, p. 3). Let M be an A-module, and, for every $\pi \in P$, let $M(\pi )$ be the set of $x\in M$ such that $\pi x= 0$. By VII, §2, No. 2, p. 9, the A-module M is semisimple if and only if it is the sum of the submodules $M(\pi )$; it is then the direct sum of these submodules. This example will be generalized further on (VIII, p. 65).

Let $A_1$ and $A_2$ be algebras over a commutative ring K. In III, §4, No. 3, p. 466, we introduced the notion of left bimodule over the algebras $A_1$ and $A_2$ and showed that this notion is equivalent to that of a left module over the ring $A_1\otimes_KA_2$. We say that M is a simple (resp. semisimple, finitely generated) bimodule if it is a simple (resp. semisimple, finitely generated) module over the ring $A_1\otimes_KA_2$.

#### Theorem 1 {#alg-viii-s4-thm-1 .statement tag=0044}

Let M be a module that is the (not necessarily direct) sum of a family $(S_i)_{i\in I}$ of simple submodules, and let N be a submodule of M. There exists a subset J of I such that M is the direct sum of the family consisting of N and the modules $S_j$ for $j$ running through J.

Let $\mathscr{S}$ be the set of subsets $I'$ of I such that the sum of the family consisting of the modules N and $S_i$ for $i$ in $I'$ is direct. The set $\mathscr{S}$ is of finite character: a subset J of I belongs to $\mathscr{S}$ if and only if the same holds for every finite subset of J. Hence, the set $\mathscr{S}$ has a maximal element J (Set Theory, III, §4, No. 5, p. 171). Set $N'= N +\sum_{j\in J}S_j$. Let $i$ be in I J. Since J is maximal in $\mathscr{S}$, the set $J\cup  \{i\}$ does not belong to $\mathscr{S}$, so that $S_i\cap N'\not= 0$. Since $S_i$ is a simple module, we have $S_i\cap N'= S_i$. We therefore have $S_i\subset N'$ for every $i\in I$, whence $N'= M$. This completes the proof.

#### Corollary 1 {#alg-viii-s4-thm-1-cor-1 .statement tag=0045}

Every module that is the sum of a family of simple modules is semisimple.

It suffices to apply Theorem 1 to the case N = 0.

#### Corollary 2 {#alg-viii-s4-thm-1-cor-2 .statement tag=0046}

A module M is semisimple if and only if every submodule of M is a direct factor.

The condition is necessary by Theorem 1.

Conversely, suppose that every submodule of M admits a supplement. Let $M'$ be the sum of the simple submodules of M, and let $M''$ be a supplement of $M'$ in M. Suppose that we have $M'\not= M$ and therefore $M''\not= 0$. Let N be a nonzero monogenous submodule of $M''$. By Proposition 3 of VIII, p. 49, there exists a maximal submodule P of N. Let Q be a submodule supplementary to P in M. Then $N\cap Q$ is a submodule of N, supplementary to P in N, hence isomorphic to $N/P$ (II, §1, No. 9, p. 210, Proposition 13). Consequently, $N\cap Q$ is a simple submodule of $M''$, contrary to the definition of $M'$.

We therefore have $M'= M$, and the module M is semisimple by Corollary 1.

#### Corollary 3 {#alg-viii-s4-thm-1-cor-3 .statement tag=0047}

Let M be a semisimple module and N a submodule of M. The modules N and $M/N$ are semisimple. More precisely, if M is the direct sum of a family $(S_i)_{i\in I}$ of simple modules, then there exists a subset J of I such that $M/N$ is isomorphic to $\bigoplus_{j\in J}S_j$ and N to $\bigoplus_{i\in I J}S_i$.

Choose J as in Theorem 1. The module $N'=\bigoplus_{j\in J}S_j$ is supplementary to N in M; it is therefore isomorphic to $M/N$. Moreover, the submodules N and $\bigoplus_{i\in I J}S_i$ of M are both supplementary to $N'$ and therefore isomorphic to $M/N'$.

#### Corollary 4 {#alg-viii-s4-thm-1-cor-4 .statement tag=0048}

Let M be a semisimple module. Then M is simple if and only if the endomorphism ring E of M is a field.

If M is simple, then E is a field by the corollary of Proposition 2 of VIII, p. 47.

If E is a field, then the module M is indecomposable (VIII, p. 31, Proposition 4, a)). Since it is moreover semisimple, it is simple.

#### Remark {#alg-viii-s4-n1-rem-1 .statement tag=0049}

Let K be an algebraically closed commutative field and A a K-algebra. Let M be a semisimple A-module that is a finite-dimensional vector space over the field K. Then M is simple if and only if every endomorphism of the A-module M is of the form $x\mapsto \alpha x$ with $\alpha$ in K: this is necessary by Theorem 1 of VIII, p. 47, and sufficient by Corollary 4 above.

### 2. The homomorphism $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$

Let A be a ring, M an A-module, and $(N_i)_{i\in I}$ a family of A-modules. With any element $(u_i)$ of $\bigoplus_i$ Hom$_A(M,N_i)$, we associate the element $m\mapsto (u_i(m))$ of Hom$_A(M,\bigoplus_iN_i)$. We thus define a canonical homomorphism

$\varphi :\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_AM,\bigoplus_iN_i$.

It is clear that $\varphi$ is injective. Let $u$ be an element of Hom$_A(M,\bigoplus_iN_i)$. Then $u$ belongs to the image of $\varphi$ if and only if the set of indices $i$ such that pr$_i\circ u\not= 0$ is finite. This condition is automatically satisfied when the module M is finitely generated.

Consequently, if the module M is finitely generated, then the homomorphism $\varphi$ is bijective.

### 3. Some Operations on Modules

Let A and B be rings, and let P be an $(A$, B)-bimodule (II, §1, No. 14, p. 225). We will define two procedures, one to go from a left B-module to a left A-module, the other to go from a left A-module to a left B-module.

3.1. The operation $\mathscr{T}$. — Let V be a left B-module. Denote the left A-module $P\otimes_BV$ (II, §3, No. 4, p. 247) by $\mathscr{T}(V)$. The law of action on $\mathscr{T}(V)$ is given by the formula

$$
a(p\otimes v) = (ap)\otimes v \tag{1}
$$

for $a\in A,p\in P$, and $v\in V$.

Let $V'$ be a left B-module. For every B-linear mapping $g$ from V to $V'$, the mapping $1_P\otimes g$ from $\mathscr{T}(V)$ to $\mathscr{T}(V')$ is A-linear; we denote it by $\mathscr{T}(g)$. The mapping $g\mapsto \mathscr{T}(g)$ from Hom$_B(V,V')$ to Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$ is $\mathbf{Z}$-linear, and we have (2) $\mathscr{T}(1_V) = 1_{\mathscr{T}(V)},\mathscr{T}(g'\circ g) =\mathscr{T}(g')\circ \mathscr{T}(g)$

if $V, V', V''$ are left B-modules and $g: V\rightarrow V',g': V'\rightarrow V''$ are B-linear mappings. Since the tensor product commutes with direct sums, if V is the direct sum of a family of submodules $(V_i)_{i\in I}$, then we can identify the A-module $\mathscr{T}(V)$ with $\bigoplus_i\mathscr{T}(V_i)$.

3.2. The operation $\mathscr{H}$. — Let M be a left A-module. Denote the left B-module Hom$_A(P,M)$ (II, §1, No. 14, p. 225) by $\mathscr{H}(M)$. The law of action on $\mathscr{H}(M)$ is given by the formula

$$
(bf)(p) =f(pb) \tag{3}
$$

for $b\in B,f\in$ Hom$_A(P,M)$, and $p\in P$.

Let $M'$ be a left A-module. For every A-linear mapping $g$ from M to $M'$, the mapping Hom$_A(1_P, g)$ from $\mathscr{H}(M)$ to $\mathscr{H}(M')$ is B-linear; we denote it by $\mathscr{H}(g)$. The mapping $g\mapsto \mathscr{H}(g)$ from Hom$_A(M,M')$ to Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))$ is $\mathbf{Z}$-linear, and we have

$$
\mathscr{H}(1_M) = 1_{\mathscr{H}(M)},\mathscr{H}(g'\circ g) =\mathscr{H}(g')\circ \mathscr{H}(g) \tag{4}
$$

if $M, M', M''$ are left A-modules and $g: M\rightarrow M',g': M'\rightarrow M''$ are A-linear mappings. Suppose, moreover, that P is a finitely generated A-module; if M is the direct sum of a family of submodules $(M_i)_i$, then we can identify $\mathscr{H}(M)$ with $\bigoplus_i\mathscr{H}(M_i)$ by VIII, p. 57. 3.3. Relations Between $\mathscr{T}$ and $\mathscr{H}$. — By Proposition 1 of II, §4, No. 1, p. 268, for every left A-module M and every left B-module V, there exists a unique group isomorphism (5) $\gamma :$ Hom$_A(\mathscr{T}(V),M)\longrightarrow$ Hom$_B(V,\mathscr{H}(M))$

characterized by the relation (6) $(\gamma (h)(v))(p) =h(p\otimes v)$ for $h\in$ Hom$_A(\mathscr{T}(V),M),v\in V$, and $p\in P$. The isomorphism $\gamma$ is called the adjunction isomorphism.

Let M be a left A-module. The A-module $\mathscr{T}(\mathscr{H}(M))$ is simply the A-module $P\otimes_B$ Hom$_A(P,M)$. By applying the above to the B-module $\mathscr{H}$ (M), we see that the mapping

$\alpha_M=\gamma^{-1}$(Id$_{\mathscr{H}(M)}) :\mathscr{T}(\mathscr{H}(M))\longrightarrow M$

is the unique mapping satisfying (7) $\alpha_M(p\otimes f) =f(p)$ for $p\in P$ and $f\in$ Hom$_A(P,M)$. We say that $\alpha_M$ is the canonical A-linear mapping from $\mathscr{T}(\mathscr{H}(M))$ to M. For every A-linear mapping $g: M\rightarrow M'$, we have a commutative diagram

$\mathscr{T}(\mathscr{H}(M))^{\alpha_M}$ // M

(I) $\mathscr{T}_{(\mathscr{H}(g))}g$

$\mathscr{T}(\mathscr{H}(M_'))^{\alpha_{M'}}$ // $M_'$.

The inverse

$\gamma^{-1}:$ Hom$_B(V,\mathscr{H}(M))\longrightarrow$ Hom$_A(\mathscr{T}(V),M)$ of the adjunction isomorphism coincides with the mapping $h\mapsto \alpha_M\circ \mathscr{T}(h)$. Indeed, by (6) and (7), we have the relations

$$
\gamma^{-1}(h)(p\otimes v) = (h(v))(p) =\alpha_M(p\otimes h(v)) =\alpha_M\circ \mathscr{T}(h)(p\otimes v)
$$

for all $h\in$ Hom$_B(V,\mathscr{H}$ (M)), $v\in V$, and $p\in P$.

Let V be a B-module. The B-module $\mathscr{H}(\mathscr{T}(V))$ is simply the B-module Hom$_A(P,P\otimes_BV)$. By applying (5) to the A-module $\mathscr{T}$ (V), we see that the B-linear mapping $\beta_V=\gamma$(Id$_{\mathscr{T}(V)})$ from V to $\mathscr{H}(\mathscr{T}(V))$ is characterized by the relation (8) $\beta_V(v)(p) =p\otimes v$ for $p\in P$ and $v\in V$. We call $\beta_V$ the canonical B-linear mapping from V to $\mathscr{H}(\mathscr{T}(V))$. For every B-module $V'$ and every B-linear mapping $g: V\rightarrow V'$, we have a commutative diagram

V $^{\beta_V}$ /$/\mathscr{H}(\mathscr{T}(V))$

(II) $g\mathscr{H}_{(\mathscr{T}(g))}$

$V_'^{\beta_{V'}}$ /$/\mathscr{H}(\mathscr{T}(V_'))$.

Note that the adjunction morphism (5) coincides with the mapping that sends $u$ to $\mathscr{H}(u)\circ \beta_V$. Indeed, from relations (6) and (8), we deduce the equalities

$$
(\gamma (u)(v))(p) =u(p\otimes v) =u\circ (\beta_V(v))(p)
$$

for all $u\in$ Hom$_A(\mathscr{T}(V),M),v\in V$, and $p\in P$.

#### Remark 1 {#alg-viii-s4-n3-rem-1 .statement tag=004A}

Let V and $V'$ be B-modules. The adjunction isomorphism

$\gamma :$ Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))\longrightarrow$ Hom$_B(V,\mathscr{H}(\mathscr{T}(V')))$ satisfies the relation $\gamma (\mathscr{T}(f)) =\beta_{V'}\circ f$ for every $f\in$ Hom$_B(V,V')$ because

$$
(\gamma (\mathscr{T}(f))(v))(p) =\mathscr{T}(f)(p\otimes v) =p\otimes f(v) = (\beta_{V'}\circ f)(v)(p)
$$

Let M and $M'$ be A-modules; the inverse of the adjunction isomorphism

$\gamma^{-1}:$ Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))\longrightarrow$ Hom$_A(\mathscr{T}(\mathscr{H}(M)),M')$ satisfies the relation $\gamma^{-1}(\mathscr{H}(u)) =u\circ \alpha_M$ for every $u\in$ Hom$_B(M,M')$. Indeed, we have the relations

$$
\gamma^{-1}(\mathscr{H}(u))(p\otimes v) = (\mathscr{H}(u)(v))(p) =u(v(p)) =u\circ \alpha_M(p\otimes v)
$$

for all $u\in$ Hom$_B(M,M'),v\in \mathscr{H}$ (M), and $p\in P$.

#### Remark 2 {#alg-viii-s4-n3-rem-2 .statement tag=004B}

Let M be a left A-module. The B-linear mappings $\beta_{\mathscr{H}(M)}:\mathscr{H}(M)\rightarrow \mathscr{H}(\mathscr{T}(\mathscr{H}(M)))$ and $\mathscr{H}(\alpha_M) :\mathscr{H}(\mathscr{T}(\mathscr{H}(M)))\rightarrow \mathscr{H}(M)$ satisfy the relation $\mathscr{H}(\alpha_M)\circ \beta_{\mathscr{H}(M)}= 1_{\mathscr{H}(M)}$. They are not bijective in general.

Let V be a left B-module. The A-linear mappings $\mathscr{T}(\beta_V) :\mathscr{T}(V)\rightarrow \mathscr{T}(\mathscr{H}(\mathscr{T}(V)))$ and $\alpha_{\mathscr{T}(V)}:\mathscr{T}(\mathscr{H}(\mathscr{T}(V)))\rightarrow \mathscr{T}(V)$ satisfy the relation $\alpha_{\mathscr{T}(V)}\circ \mathscr{T}(\beta_V) = 1_{\mathscr{T}(V)}$. They are not bijective in general.

#### Remark 3 {#alg-viii-s4-n3-rem-3 .statement tag=004C}

Suppose that P is finitely generated as an A-module. Let M be the direct sum of a family $(M_i)_{i\in I}$ of A-modules. The A-modules $\mathscr{T}(\mathscr{H}(M))$ and $\bigoplus_i\mathscr{T}(\mathscr{H}(M_i))$ are canonically isomorphic. When we identify them, $\alpha_M$ is identified with $\bigoplus_i\alpha_{M_i}$. Likewise, let V be the direct sum of a family $(V_j)_{j\in J}$ of B-modules. The B-module $\mathscr{H}(\mathscr{T}(V))$ is identified with $\bigoplus_j\mathscr{H}(\mathscr{T}(V_j))$, and the linear mapping $\beta_V$ with $\bigoplus_j\beta_{V_j}$.

### 4. Isotypical Modules

Let A be a ring and S a simple left A-module. Let D be the opposite ring of the endomorphism ring of S; it is a field. Endowed with the actions of A and D, S is an $(A$, D)-bimodule.

#### Proposition 1 {#alg-viii-s4-prop-1 .statement tag=004D}

Let M be an A-module. The following properties are equivalent:

(i) There exists a set I such that M is isomorphic to $S^{(I)}$.

(ii) The module M is the direct sum of a family of submodules isomorphic to S.

(iii) The module M is the sum of a family of submodules isomorphic to S.

(iv) There exists a left vector space V over the field D such that the A-module M is isomorphic to $S\otimes_DV$.

The equivalence of (i) and (ii) is immediate, and that of (ii) and (iii) follows from Theorem 1 of VIII, p. 56, applied to the case N = 0. Every left vector space over D is isomorphic to a vector space of the form $D_s^{(I)}$, where I is a set (II, §7, No. 1, p. 292, Theorem 1). Since the tensor product commutes with direct sums, (i) is equivalent to (iv).

#### Definition 2 {#alg-viii-s4-def-2 .statement tag=004E}

An A-module M is isotypical of type S if it has the equivalent properties of Proposition 1. The module M is called isotypical if there exists a simple A-module T such that M is isotypical of type T.

Every isotypical module is semisimple.

#### Proposition 2 {#alg-viii-s4-prop-2 .statement tag=004F}

If a module is the sum of isotypical submodules of type S, then it is isotypical of type S. The submodules and the quotient modules of an isotypical module of type S are isotypical of type S.

The first assertion follows from the definitions, the second from Corollary 3 of VIII, p. 56.

#### Remark {#alg-viii-s4-n4-rem-1 .statement tag=004G}

Every nonzero isotypical module of type S has a quotient module and a submodule isomorphic to S; consequently, if M and $M'$ are nonzero isotypical A-modules of type S, then the group Hom$_A(M,M')$ is not reduced to 0.

#### Proposition 3 {#alg-viii-s4-prop-3 .statement tag=004H}

a) Let M be an isotypical A-module of type S. The A-linear mapping $\alpha_M: S\otimes_D$Hom$_A(S,M)\rightarrow M$ characterized by $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 59) is bijective.

b) Let V be a left vector space over the field D. The D-linear mapping $\beta_V: V\rightarrow$ Hom$_A(S,S\otimes_DV)$ defined by $\beta_V(v)(s) =s\otimes v$ (VIII, p. 59) is bijective.

Denote the left D-vector space Hom$_A(S,M)$ by $\mathscr{H}(M)$. The A-module M is, by assumption, the direct sum of a family of submodules isomorphic to S. The A-module S is monogenous; to prove that the mapping $\alpha_M$ is bijective, it therefore suffices to consider the case M = S (VIII, p. 60, Remark 3). Now, $\mathscr{H}(S)$ is simply the D-vector space $D_s$, and $\alpha_S$ is simply the isomorphism $\iota : S\otimes_DD_s\rightarrow S$ defined by $\iota (s\otimes d) =sd$.

Likewise, to prove b), it suffices to consider the case $V = D_s$. Since the mapping $\alpha_S$ is bijective, the mapping $\beta_{D_s}=\beta_{\mathscr{H}(S)}$ is too (VIII, p. 60, Remark 2).

### 5. Description of an Isotypical Module

As in the previous subsection, A denotes a ring, S a simple left A-module, and D the field End$_A(S)^o$. We view S as an $(A$, D)-bimodule.

#### Definition 3 {#alg-viii-s4-def-3 .statement tag=004I}

Let M be an isotypical A-module of type S. A description of M with respect to S is a pair $(V, \alpha )$, where V is a left vector space over the field D and $\alpha : S\otimes_DV\rightarrow M$ is an isomorphism of A-modules.

Every isotypical A-module M of type S has a canonical description: it is the pair (Hom$_A(S,M), \alpha_M)$, where $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$ is the isomorphism of A-modules characterized by $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 62, Proposition 3, a)).

#### Theorem 2 {#alg-viii-s4-thm-2 .statement tag=004J}

Let M be an isotypical A-module of type S and $(V, \alpha )$ a description of M. Denote by $\mathscr{D}_D(V)$ the set, ordered by inclusion, of D-linear subspaces of V, and by $\mathscr{D}_A(M)$ that of A-submodules of M. For every $W\in$ $\mathscr{D}_D(V)$, identify the A-module $S\otimes_DW$ with its canonical image in $S\otimes_DV$.

a) The mapping $W\mapsto \alpha (S\otimes_DW)$ is an isomorphism of ordered sets from $\mathscr{D}_D(V)$ to $\mathscr{D}_A(M)$.

b) The inverse isomorphism sends a submodule N of M to the linear subspace of V consisting of the elements $v$ such that $\alpha (s\otimes v)$ belongs to N for every $s\in S$.

For $W\in \mathscr{D}_D$(V), set $\varphi (W) =\alpha (S\otimes_DW)$. For $N\in \mathscr{D}_A$(M), denote by $\psi (N)$ the set of elements $v\in V$ such that $\alpha (s\otimes v)\in N$ for every $s\in S$. This defines two mappings $\varphi :\mathscr{D}_D(V)\rightarrow \mathscr{D}_A(M)$ and $\psi :\mathscr{D}_A(M)\rightarrow \mathscr{D}_D(V)$. They are clearly increasing.

Let N be a submodule of M. It is isotypical of type S (VIII, p. 61, Proposition 2). Set $W =\psi (N)$. By Proposition 3, b) of VIII, p. 62, the A-linear mappings $h: S\rightarrow M$ are simply the mappings $s\mapsto \alpha (s\otimes v)$, where $v$ runs through V. Those with image contained in N are the mappings $s\mapsto \alpha (s\otimes w)$ where $w$ runs through W; their images generate N because N is isotypical of type S. We therefore have $\alpha (S\otimes_DW) = N$, that is, $\varphi (\psi (N)) = N$. This proves that $\varphi \circ \psi$ is the identity mapping on $\mathscr{D}_A(M)$. In particular, $\varphi$ is surjective and $\psi$ is injective.

To finish the proof, it suffices to prove that the mapping $\varphi$ is injective. Let W and $W'$ be linear subspaces of V such that $\varphi (W) =\varphi (W')$. The vector spaces $S\otimes_DW$ and $S\otimes_DW'$ coincide when viewed as linear subspaces of $S\otimes_DV$. Choose a nonzero linear form $f$ on the D-vector space S, and let $g: S\otimes_DV\rightarrow V$ be the group homomorphism defined by $g(s\otimes v) =f(s)v$. We have $W =g(S\otimes_DW) =g(S\otimes_DW') = W'$, so $\varphi$ is injective.

#### Remark 1 {#alg-viii-s4-n5-rem-1 .statement tag=004K}

Let M be an isotypical A-module of type S and $(V, \alpha )$ a description of M. Then M has finite length if and only if V is finite-dimensional, and in this case, we have the relation

long$_A(M) =$ dim$_D(V)$.

#### Corollary 1 {#alg-viii-s4-thm-2-cor-1 .statement tag=004L}

Let M be an isotypical A-module of type S. For every A-submodule N of M, identify Hom$_A(S,N)$ with the linear subspace of Hom$_A(S,M)$ consisting of the mappings with image contained in N.

a) The mapping $N\mapsto$ Hom$_A(S,N)$ is an isomorphism of ordered sets from $\mathscr{D}_A(M)$ to $\mathscr{D}_D$(Hom$_A(S,M))$.

b) The inverse bijection sends a linear subspace W of Hom$_A(S,M)$ to the submodule $\sum_{h\in W}h(S)$ of M.

This is a reformulation of Theorem 2 when we take $(V, \alpha )$ to be the canonical description of M.

#### Corollary 2 {#alg-viii-s4-thm-2-cor-2 .statement tag=004M}

Let V be a left vector space over D and $\mathscr{F}$ a set of endomorphisms of V. An A-submodule of $S\otimes_DV$ is stable under all endomorphisms $1_S\otimes u$, where $u$ runs through $\mathscr{F}$, if and only if it is of the form $S\otimes_DW$, where W is a linear subspace of V that is stable under all endomorphisms belonging to $\mathscr{F}$.

Indeed, by Theorem 2, every A-submodule N of $S\otimes_DV$ is equal to $S\otimes_DW$, where W is the linear subspace of V consisting of the elements $v$ such that $s\otimes v$ belongs to N for every $s\in S$.

#### Theorem 3 {#alg-viii-s4-thm-3 .statement tag=004N}

Let M and $M'$ be isotypical A-modules of type S. Let $(V, \alpha )$ and $(V', \alpha ')$ be descriptions of M and $M'$, respectively. For any D-linear mapping $f: V\rightarrow V'$, denote by $\widetilde{f}: M\rightarrow M'$ the unique A-linear mapping that makes the following diagram commute:

$S\otimes_DV^{\alpha}$ // M

$$
1_{_S\otimes f}\widetilde{f} \tag{9}
$$

$S\otimes_DV_'^{\alpha'}$ // $M_'$.

The mapping $f\mapsto \widetilde{f}$ from Hom$_D(V,V')$ to Hom$_A(M,M')$ is a group isomorphism.

It suffices to prove that the $\mathbf{Z}$-linear mapping $u\mapsto 1_S\otimes u$ from Hom$_D(V,V')$ to Hom$_A(S\otimes_DV,S\otimes_DV')$ is bijective. In the notation of No.3 applied to the $(A$, D)-bimodule S, this corresponds to showing that the mapping

$\mathscr{T}:$ Hom$_D(V,V')\longrightarrow$ Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$

is bijective. But by Remark 1 of VIII, p. 60, since the adjunction isomorphism (VIII, p. 59) is bijective, this corresponds to showing that the mapping that sends $u$ to $\beta_{V'}\circ u$ is bijective, which follows from the fact that the D-linear mapping $\beta_{V'}$ is bijective (VIII, p. 62, Proposition 3, b)).

We keep the notation of Theorem 3. Let $M''$ be an isotypical A-module of type S, and let $(V'', \alpha '')$ be a description of $M''$. For every $f\in$ Hom$_D(V,V')$ and every $g\in$ Hom$_D(V',V'')$, we have $g]\circ f=\widetilde{g}\circ \widetilde{f}$. In particular, for $M = M'$, $V = V'$, and $\alpha =\alpha '$, the mapping $f\mapsto \widetilde{f}$ from End$_D(V)$ to End$_A(M)$ is a ring isomorphism.

#### Remark 2 {#alg-viii-s4-n5-rem-2 .statement tag=004O}

Let M be an isotypical A-module of type S, and let $(V, \alpha )$ be a description of M. Let B be a subring of the ring End$_A(M)^o$. The ring isomorphism from End$_D(V)^o$ to End$_A(M)^o$ endows V with the structure of a $(D$, B)-bimodule, so that $\alpha$ is an isomorphism of $(A$, B)-bimodules. There exists an isomorphism from the set of $(D$, B)-sub-bimodules of V, ordered by inclusion, to the set of $(A$, B)-sub-bimodules of M (VIII, p. 62, Theorem 2 and VIII, p. 63, Corollary 2).

#### Corollary {#alg-viii-s4-n5-cor-1 .statement tag=004P}

Let M and $M'$ be isotypical A-modules of type S. The mapping $u\mapsto$ Hom(1$_S, u)$ from Hom$_A(M,M')$ to Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,M'))$ is a group isomorphism. When M is equal to $M'$, it is a ring isomorphism from End$_A(M)$ to End$_D$(Hom$_A(S,M))$.

Because of the commutativity of diagram (I) of VIII, p. 59, this corollary follows from Theorem 3, applied to the canonical descriptions of M and $M'$.

### 6. Isotypical Components of a Module

#### Definition 4 {#alg-viii-s4-def-4 .statement tag=004Q}

Let A be a ring, M an A-module, and S a simple A-module. The isotypical component of type S of M, denoted by $M_S$, is the sum of the submodules of M isomorphic to S.

It is clear that $M_S$ is the greatest submodule of M that is isotypical of type S. Because every submodule of $M_S$ is isotypical of type S (VIII, p. 61, Proposition 2), we have $N_S= M_S\cap N$ for every submodule N of M.

If $S'$ is a simple A-module isomorphic to S, then we clearly have $M_S=$ $M_{S'}$, so $M_S$ depends only on the class of S (VIII, p. 51).

Let M be an A-module. There exists a greatest semisimple submodule of M, called the socle of M; it is the sum of the simple submodules of M and also the sum of the isotypical components of M. In particular, M is semisimple if and only if it is equal to its socle.

#### Proposition 4 {#alg-viii-s4-prop-4 .statement tag=004R}

Let A be a ring. Denote the set of classes of simple A-modules by $\mathscr{S}$. Let M be a semisimple A-module.

a) The module M is the direct sum of the family $(M_{\lambda})_{\lambda\in\mathscr{S}}$ of its isotypical components.

b) Suppose that M is the direct sum of a family $(N_i)_{i\in I}$ of simple submodules. For every $\lambda \in \mathscr{S}$, let $I(\lambda )$ be the set of indices $i\in I$ such that $N_i$ is of class $\lambda$. We have $M_{\lambda}=\bigoplus_{i\in I(\lambda)}N_i$.

c) If M is finitely generated, then the set of $\lambda \in \mathscr{S}$ such that $M_{\lambda}\not= 0$ is finite.

d) For every submodule N of M and every $\lambda \in \mathscr{S}$, we have $N_{\lambda}= N\cap M_{\lambda}$ and $(M/N)_{\lambda}= (M_{\lambda}+ N)/N$.

Since M is semisimple, it is the sum of the family $(M_{\lambda})_{\lambda\in\mathscr{S}}$; let us prove that this sum is direct. Let $\lambda \in \mathscr{S}$. Denote the sum of the family

$(M_\mu)_{\mu\in\mathscr{S}\{\lambda\}}$ by $M'_{\lambda}$. The module $M'_{\lambda}$ is the direct sum of a family of simple modules not isomorphic to $\lambda$ (VIII, p. 56, Theorem 1). By Corollary 3 of Theorem 1 of VIII, p. 56, $M'_{\lambda}$ does not contain any simple submodules of class $\lambda$. We consequently have $M_{\lambda}\cap M'_{\lambda}= 0$. Assertion a) is therefore proved. By construction, we have $M_{\lambda}\supset \bigoplus_{i\in I(\lambda)}N_i$, so assertion b) follows from Remark 1 of II, §1, No. 8, p. 208.

Assertion c) follows from a) and Proposition 23 of II, §1, No. 12, p. 221.

Let N be a submodule of M and $\lambda \in \mathscr{S}$. The isotypical component $N_{\lambda}$ of type $\lambda$ of N is contained in $M_{\lambda}$ and $M_{\lambda}\cap N\subset N_{\lambda}$. The intersection $N\cap M_{\lambda}$ is therefore the isotypical component of N of type $\lambda$.

For every $\lambda \in \mathscr{S}$, the module $M_{\lambda}+N/N$ is isomorphic to $M_{\lambda}/(M_{\lambda}\cap N)$. It is therefore isotypical of type $\lambda$ and contained in $(M/N)_{\lambda}$. The last assertion then follows from a) and II, §1, No. 8, p. 208, Remark 1.

#### Corollary {#alg-viii-s4-n6-cor-1 .statement tag=004S}

Let A be a ring and $\mathscr{S}$ the set of classes of simple A-modules. Let M be a semisimple A-module and N a submodule of M. Then we have $N =\bigoplus_{\lambda\in\mathscr{S}}N\cap M_{\lambda}$ and $M/N =\bigoplus_{\lambda\in\mathscr{S}}(M_{\lambda}+ N)/N$.

Since N and $M/N$ are semisimple (VIII, p. 56, Corollary 3), the corollary follows from Proposition 4, d).

The support of a semisimple A-module M is the set of classes $\lambda$ of simple A-modules such that the isotypical component of M of type $\lambda$ is nonzero. The support of a finitely generated semisimple A-module is finite.

#### Proposition 5 {#alg-viii-s4-prop-5 .statement tag=004T}

Let A be a ring, and let $\mathscr{S}$ be the set of classes of simple A-modules. Let M and N be A-modules.

a) Let $f: M\rightarrow N$ be a homomorphism. For every $\lambda \in \mathscr{S},f$ induces a homomorphism $f_{\lambda}$ from $M_{\lambda}$ to $N_{\lambda}$; if M is semisimple and $f$ surjective, then each of the homomorphisms $f_{\lambda}$ is surjective.

b) Suppose that M is semisimple. The mapping $f\mapsto (f_{\lambda})_{\lambda\in\mathscr{S}}$ is a group isomorphism from Hom$_A(M,N)$ to $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(M_{\lambda},N_{\lambda})$. When M is equal to N, the mapping is a ring isomorphism from End$_A(M)$ to $\prod_{\lambda\in\mathscr{S}}$ End$_A(M_{\lambda})$.

For every $\lambda \in \mathscr{S}$, the submodule $f(M_{\lambda})$ of N is isomorphic to a quotient of an isotypical module of type $\lambda$; it is therefore isotypical of type $\lambda$ and, consequently, contained in $N_{\lambda}$.

Suppose that M is semisimple and $f$ surjective. Then $f$ induces an isomorphism from $M/$ Ker($f)$ to N that sends $(M_{\lambda}$+Ker($f))/$ Ker($f)$ to $f(M_{\lambda})$. By Proposition 4 of VIII, p. 65, we have $N_{\lambda}=f(M_{\lambda})$, which completes the proof of a).

The mapping considered in b) is clearly a group homomorphism, and it is a ring homomorphism when M is equal to N. Let $(f_{\lambda})_{\lambda\in\mathscr{S}}$ be an element of $\prod_{\lambda\in\mathscr{S}}$ Hom(M$_{\lambda},N_{\lambda})$. The unique element of its inverse image under the mapping in b) is the homomorphism $f: M\rightarrow N$ defined by

$$
f(\sum_{\lambda\in\mathscr{S}}x_{\lambda}=_{\lambda}\sum_{\in\mathscr{S}}f_{\lambda}(x_{\lambda})
$$

for every $(x_{\lambda})_{\lambda\in\mathscr{S}}\in \bigoplus_{\lambda}M_{\lambda}$.

#### Remark {#alg-viii-s4-n6-rem-1 .statement tag=004U}

Let A and B be rings. Let M be an $(A$, B)-bimodule. It follows from Proposition 5 that the isotypical components of the A-module M are sub-bimodules of M. This holds, in particular, when M is an A-module and B is the opposite ring of End$_A(M)$.

#### Example {#alg-viii-s4-n6-exa-1 .statement tag=004V}

Let us consider the case when the ring A is commutative. The mapping that sends a maximal ideal $\mathfrak{m}$ onto cl(A$/\mathfrak{m})$ is a bijection from the set of maximal ideals of A to the set $\mathscr{S}$ of classes of simple A-modules (VIII, p. 51). The inverse bijection sends $\lambda$ to its annihilator $\mathfrak{m}_{\lambda}$.

Let M be an A-module. For every $\lambda \in \mathscr{S}$, the isotypical component $M_{\lambda}$ of type $\lambda$ of M consists of the elements annihilated by $\mathfrak{m}_{\lambda}$, and we can view $M_{\lambda}$ as a vector space over the field $A/\mathfrak{m}_{\lambda}$. If M is semisimple and N is another A-module, then we can deduce a group isomorphism from Hom$_A(M,N)$ to $\prod_{\lambda\in\mathscr{S}}$ Hom$_{A/\mathfrak{m}_{\lambda}}(M_{\lambda},N_{\lambda})$ from Proposition 5.

#### Corollary 1 {#alg-viii-s4-prop-5-cor-1 .statement tag=004W}

Let M be a semisimple A-module and N a submodule of M. The following properties are equivalent:

(i) There exists a unique submodule supplementary to N in M.

(ii) We have Hom$_A(M/N,N) = 0$.

(iii) There exists a subset Λ of $\mathscr{S}$ such that $N =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$.

Choose a submodule $N'$ supplementary to N in M (VIII, p. 56, Corollary 2). If we identify M with $N'\times N$, then the submodules of M supplementary to N are the graphs of the A-linear mappings from $N'$ to N. Since $N'$ is isomorphic to $M/N$, we have proved the equivalence of properties (i) and (ii). By Proposition 5, b), the group Hom$_A(N',N)$ is isomorphic to the group $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(N'_{\lambda},N_{\lambda})$. It is zero if and only if for every $\lambda \in \mathscr{S}$, we have $N_{\lambda}= 0$ or $N'_{\lambda}= 0$ (VIII, p. 61, Remark), that is, $N_{\lambda}= 0$ or $N_{\lambda}= M_{\lambda}$. This proves the equivalence of properties (ii) and (iii).

#### Corollary 2 {#alg-viii-s4-prop-5-cor-2 .statement tag=00R0}

Let M be an A-module. The following two conditions are equivalent:

(i) Every submodule of M admits a unique supplementary submodule.

(ii) The module M is the direct sum of a family $(S_i)_{i\in I}$ of simple, pairwise nonisomorphic modules. Suppose that M satisfies these conditions. Then, for every submodule N of M, there exists a unique subset J of I such that we have $N =\bigoplus_{j\in J}S_j$ and every simple submodule of M is equal to one of the $S_i$.

Conditions (i) and (ii) both imply that M is semisimple.

Suppose that condition (i) is satisfied. Let $\lambda \in \mathscr{S}$. By the equivalence of (i) and (iii) in Corollary 1, every submodule of $M_{\lambda}$ is zero or equal to $M_{\lambda}$. Consequently, $M_{\lambda}$ is zero or simple, and (ii) follows from the fact that M is the direct sum of the family $(M_{\lambda})_{\lambda\in\mathscr{S}}$.

Conversely, if condition (ii) is satisfied, then $M_{\lambda}$ is zero or simple for every $\lambda \in \mathscr{S}$. If N is a submodule of M, then $N\cap M_{\lambda}$ is equal to 0 or $M_{\lambda}$ for every $\lambda \in \mathscr{S}$. Since we have $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, Corollary), the submodule N has property (iii) of Corollary 1 and therefore admits a unique supplementary submodule in M. This proves that (ii) implies (i), as well as the last assertions of the corollary.

Let M be an A-module and S a simple A-module. Denote the opposite ring of the field End$_A(S)$ by D, and view S as an $(A$, D)-bimodule. Then Hom$_A(S,M)$ is a left vector space over D, and Hom$_A(M,S)$ is a right vector space over D. The dual of the left D-vector space Hom$_A(S,M)$ is a right vector space over D (II, §2, No. 3, p. 232, Definition 2). For every $u\in$ Hom$_A(M,S)$, the mapping $h(u) :v\mapsto u\circ v$ from Hom$_A(S,M)$ to Hom$_A(S,S) = D$ is a linear form on the left D-vector space Hom$_A(S,M)$.

#### Proposition 6 {#alg-viii-s4-prop-6 .statement tag=004X}

Keep the notation above, and suppose that the A-module M is semisimple. The mapping $u\mapsto h(u)$ from the right D-vector space Hom$_A(M,S)$ to the dual of the left D-vector space Hom$_A(S,M)$ is D-linear and bijective.

Let $u\in$ Hom$_A(M,S),v\in$ Hom$_A(S,M)$, and $d\in D$. We have

$$
h(ud)(v) =h(d\circ u)(v) =d\circ u\circ v=d\circ (h(u)(v)) =h(u)(v)d
$$

This proves that the mapping $h$ is D-linear. It is simply the mapping given by $u\mapsto$ Hom(1$_S, u)$ from Hom$_A(M,S)$ to Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,S))$. To prove that it is bijective, by Proposition 5, b) of VIII, p. 66, it suffices to treat the case when M is isotypical of type S; we can then apply the corollary of VIII, p. 65.

### 7. Description of a Semisimple Module

For the remainder of this section, A is a ring, and $\mathscr{S}$ is the set of classes of simple A-modules. For every $\lambda \in \mathscr{S}$, we choose a simple module $S_{\lambda}$ of class $\lambda$ (for example, $S_{\lambda}=\lambda )$; we denote the opposite ring of the field of endomorphisms of $S_{\lambda}$ by $D_{\lambda}$. We view $S_{\lambda}$ as an $(A,D_{\lambda}$)-bimodule.

Let M be an A-module. For every $\lambda \in \mathscr{S}$, Hom$_A(S_{\lambda},M)$ is a left vector space over the field $D_{\lambda}$. By VIII, p. 59, and II, §1, No. 6, p. 202, Proposition 6, there exists a unique A-linear mapping, called canonical,

$\alpha_M:_{\lambda}\bigoplus_{\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)\rightarrow M$

satisfying the relation

$$
\alpha_M(s\otimes f) =f(s) \tag{10}
$$

for $\lambda \in \mathscr{S},s\in S_{\lambda}$, and $f\in$ Hom$_A(S_{\lambda},M)$. If we endow $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))$ and M with their natural structures of End$_A$(M)-modules, then the mapping $\alpha_M$ is End$_A$(M)-linear.

#### Proposition 7 {#alg-viii-s4-prop-7 .statement tag=004Y}

Let M be an A-module. The canonical mapping $\alpha_M$ is injective. For every $\lambda \in \mathscr{S}$, the image under $\alpha_M$ of $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ is the isotypical component of M of type $\lambda$. The image of $\alpha_M$ is the socle of M. The A-module M is semisimple if and only if the mapping $\alpha_M$ is bijective.

Let $\lambda \in \mathscr{S}$. Denote the isotypical component of M of type $\lambda$ by $M_{\lambda}$. Every A-linear mapping from $S_{\lambda}$ to M takes its values in $M_{\lambda}$ (VIII, p. 66, Proposition 5). Consequently, by Proposition 3, a) of VIII, p. 62, the mapping $\alpha_M$ induces a bijection from $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ to $M_{\lambda}$. The proposition follows because the socle of M is the direct sum of the family $(M_{\lambda})_{\lambda\in\mathscr{S}}$ and the module M is semisimple if and only if it is equal to its socle.

#### Definition 5 {#alg-viii-s4-def-5 .statement tag=004Z}

Let M be a semisimple A-module. A description of M (with respect to the family $(S_{\lambda})_{\lambda\in\mathscr{S}})$ is a pair $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$, where $V_{\lambda}$ is a left vector space over the field $D_{\lambda}$ for each $\lambda \in \mathscr{S}$ and $\alpha :\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})\rightarrow M$ is an isomorphism of A-modules.

By Proposition 7, every semisimple A-module M has a canonical description: it is the pair ((Hom$_A(S_{\lambda},M))_{\lambda\in\mathscr{S}}, \alpha_M)$, where $\alpha_M$ is the A-linear mapping defined by formula (10).

#### Proposition 8 {#alg-viii-s4-prop-8 .statement tag=0050}

Let M be a semisimple A-module and $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ a description of M.

a) For every $\lambda \in \mathscr{S}$, the mapping $\alpha$ induces an isomorphism from the A-module $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ to the isotypical component of M of type $\lambda$.

b) For every $\lambda \in \mathscr{S}$, the mapping $\beta_{\lambda}: V_{\lambda}\rightarrow$ Hom$_A(S_{\lambda},M)$ defined by $\beta_{\lambda}(v)(s) =\alpha (s\otimes v)$ is $D_{\lambda}$-linear and bijective.

c) Let N be a submodule of M. There exists a unique family $(W_{\lambda})_{\lambda\in\mathscr{S}}$ with the following properties: $W_{\lambda}$ is a $D_{\lambda}$-linear subspace of $V_{\lambda}$ for every $\lambda \in \mathscr{S}$, and N is the image under $\alpha$ of the module $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ identified with its canonical image in the module $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$. For every $\lambda \in \mathscr{S},W_{\lambda}$ is the set of elements $v\in V_{\lambda}$ such that $\alpha (s\otimes v)$ belongs to N for every $s\in S_{\lambda}$.

The A-module $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ is isotypical of type $\lambda$ for every $\lambda \in \mathscr{S}$. Assertion a) then follows from the facts that $\alpha$ is an isomorphism and that M is the direct sum of the family $(M_{\lambda})_{\lambda\in\mathscr{S}}$ (VIII, p. 65, Proposition 4, a)).

Let $\lambda \in \mathscr{S}$. Denote the restriction of $\alpha$ to $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ by $\alpha_{\lambda}: S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}\rightarrow$ M. With the notation of No. 3 applied to the $(A,D_{\lambda}$)-bimodule $S_{\lambda}$, we have

$$
\beta_{\lambda}=\gamma (\alpha_{\lambda}) =\mathscr{H}(\alpha_{\lambda})\circ \beta_{V_{\lambda}}
$$

where the last equality follows from VIII, p. 60. Hence, $\beta_{\lambda}$ is the composition of the $D_{\lambda}$-linear homomorphism $\mathscr{H}(\alpha_{\lambda})$ and $\beta_{V_{\lambda}}$. Assertion b) then follows from Proposition 3, b) of VIII, p. 62.

Let N be a submodule of M. We have $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, Corollary), so c) follows from Theorem 2 of VIII, p. 62.

#### Corollary {#alg-viii-s4-n7-cor-1 .statement tag=0051}

Let M be a semisimple A-module. For every submodule N of M and every element $\lambda$ of $\mathscr{S}$, identify Hom$_A(S_{\lambda},N)$ with the $D_{\lambda}$-linear subspace of Hom$_A(S_{\lambda},M)$ consisting of the mappings with image contained in N.

a) The mapping $N\mapsto$ (Hom$_A(S_{\lambda},N))_{\lambda\in\mathscr{S}}$ is a bijection from the set of A-submodules of M to the set of families $(W_{\lambda})_{\lambda\in\mathscr{S}}$ such that for every $\lambda \in \mathscr{S}$, $W_{\lambda}$ is a $D_{\lambda}$-linear subspace of Hom$_A(S_{\lambda},M)$.

b) The inverse bijection sends a family $(W_{\lambda})_{\lambda\in\mathscr{S}}$ to the A-submodule $\sum_{\lambda\in\mathscr{S}}\sum_{w\in W_{\lambda}}w(S_{\lambda})$ of M.

This is a reformulation of Proposition 8, c) applied to the canonical description of M.

#### Proposition 9 {#alg-viii-s4-prop-9 .statement tag=0052}

Let M and $M'$ be semisimple A-modules, and consider descriptions $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ and $((V'_{\lambda})_{\lambda\in\mathscr{S}}, \alpha ')$ of M and $M'$, respectively. For every family $\boldsymbol{f}= (f_{\lambda})_{\lambda\in\mathscr{S}}$ in $\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V_{\lambda}')$, there exists a unique A-linear mapping $\varphi (\boldsymbol{f})\in$ Hom$_A(M,M')$ for which the following diagram commutes:

$\bigoplus(S_{\lambda}\otimes_DV_{\lambda})^{\alpha}$ // M

$$
\lambda \in \mathscr{S}\lambda
$$

$\bigoplus(1_S\otimes f_{\lambda})$

$$
_{\lambda}\varphi (\boldsymbol{f})
$$

$\lambda \in \mathscr{S}$

$\bigoplus(S_{\lambda}\otimes_DV'_{\lambda})^{\alpha'}$ // $M_'$.

$\lambda \in \mathscr{S}\lambda$

The mapping $\varphi :\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V'_{\lambda})\rightarrow$ Hom$_A(M,M')$ defined this way is a group isomorphism. When we have $M = M',V_{\lambda}= V'_{\lambda}$ for every $\lambda \in \mathscr{S}$,

and $\alpha =\alpha '$, the mapping $\varphi$ is a ring isomorphism from $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}(V_{\lambda})$ to End$_A(M)$.

In view of the description of the isotypical components of M and $M'$ given in Proposition 8, a), this follows from Theorem 3 of VIII, p. 64 and Proposition 5, b) of VIII, p. 66.

#### Corollary {#alg-viii-s4-n7-cor-2 .statement tag=0053}

Let M be a semisimple A-module and $M'$ an A-module. The mapping $u\mapsto$ (Hom(1$_{S_{\lambda}}, u))_{\lambda\in\mathscr{S}}$ from Hom$_A(M,M')$ to

$_{\lambda}\prod_{\in\mathscr{S}}$ Hom$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$, Hom$_A(S_{\lambda},M'))$

is a group isomorphism. When $M'$ is equal to M, it is an isomorphism from the ring End$_A(M)$ to the ring $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M))$.

This is a reformulation of Proposition 9 applied to the canonical descriptions of M and of the socle of $M'$.

### 8. Multiplicities and Lengths in Semisimple Modules

#### Proposition 10 {#alg-viii-s4-prop-10 .statement tag=0054}

Let M be a semisimple A-module. Let $(M_i)_{i\in I}$ be a family of simple submodules with direct sum M. The following properties are equivalent:

(i) M has finite length.

(ii) M is Artinian.

(iii) M is Noetherian.

(iv) M is finitely generated.

(v) I is finite. If M has these properties, then the length of M is equal to the cardinal of I.

If the set I is finite, then M has properties (i), (ii), (iii), and (iv). Suppose that the set I is infinite. By Example 2 of VIII, p. 2, the module M is neither Artinian nor Noetherian; because every module of finite length is Artinian and Noetherian (VIII, p. 2, Proposition 1), M also does not have finite length. Finally, every element of M belongs to the sum of a finite number of submodules $M_i$, so M is not finitely generated. This proves the equivalence of properties (i) through (v). If these hold, then we have long(M) $=\sum_{i\in I}$ long(M$_i) =$ Card(I) (II, §1, No. 10, p. 213, Corollary 5).

#### Proposition 11 {#alg-viii-s4-prop-11 .statement tag=0055}

Let M be a semisimple A-module that is the direct sum of a family $(M_i)_{i\in I}$ of simple submodules. For every $\lambda \in \mathscr{S}$, we denote by $I(\lambda )$ the set of indices $i\in I$ such that $M_i$ is of class $\lambda$. The cardinal of $I(\lambda )$ is equal to the dimension of the left $D_{\lambda}$-vector space Hom$_A(S_{\lambda},M)$.

The isotypical component of A of type $\lambda$ is isomorphic to $S_{\lambda}^{(I(\lambda))}$ (VIII, p. 65, Proposition 4, b)). The $D_{\lambda}$-vector space Hom$_A(S_{\lambda},M)$ may be identified with Hom$_A(S_{\lambda},M_{\lambda})$, so is isomorphic to $D_{\lambda}^{(I(\lambda))}$ (No. 2). This proves the proposition.

Every simple module is primordial (VIII, p. 45), so every semisimple module is semiprimordial. Let M be a semisimple A-module, and let $\lambda \in \mathscr{S}$. The multiplicity of $\lambda$ in M is the primordial multiplicity $[M :\lambda ]$ of $\lambda$ in M defined in VIII, p. 34. Proposition 11 translates to the equality

(11) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M))$.

More generally, if $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ is a description of M, then $[M :\lambda ]$ is equal to dim$_{D_{\lambda}}(V_{\lambda})$. By Proposition 6 of VIII, p. 68, we also have

(12) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(M,S_{\lambda}))$

when the multiplicity $[M :\lambda ]$ is finite. Semisimple A-modules M and $M'$ are isomorphic if and only if we have $[M :\lambda ] = [M':\lambda ]$ for every $\lambda \in \mathscr{S}$.

Let M be a semisimple A-module. There exists a cardinal $\mathbf{I}$ that has the following property: for every decomposition $M =\bigoplus_{i\in I}M_i$ of M into a direct sum of simple modules, the cardinal of I is equal to $\mathbf{I}$ (VIII, p. 34, Corollary 2). This cardinal is called the length of the semisimple A-module M and denoted by long$_A(M)$ or long(M). When M has finite length, this definition is compatible with that of II, §1, No. 10, p. 212, by Proposition 10.

The simple A-modules are the semisimple A-modules of length 1, and we have the formula

(13) long$_A\bigoplus_{j\in J}M_j=\sum_{j\in J}$ long$_A(M_j)$

for every family $(M_j)_{j\in J}$ of semisimple A-modules. By Proposition 11, we have

(14) long$_A(M) =_{\lambda}\sum_{\in\mathscr{S}}$ dim$_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$.

By applying this formula to $M_{\lambda}$, we obtain $[M :\lambda ] =$ long$_A(M_{\lambda})$ for every $\lambda \in \mathscr{S}$.

When A is a field, the simple A-modules are the vector spaces of dimension 1; every A-module is then semisimple (II, §7, No. 1, p. 292, Theorem 1), and its length is simply its dimension as a vector space over A (II, §7, No. 2, p. 293) .

### Exercises {#alg-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).

[^1]: By Corollary 2 of VIII, p. 56, this definition coincides with that given in VII, §2, No. 2, p. 9
