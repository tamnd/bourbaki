---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 21
section_title: Linear Representations of Finite Groups
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.397-A VIII.434
pdf_pages: 0414-0451
extraction: native
subsections:
    - "no": 1
      title: Linear Representations
      page: 397
      pdf_page: 414
    - "no": 2
      title: Maschke’s Theorem
      page: 401
      pdf_page: 418
    - "no": 3
      title: Induced and Coinduced Representations
      page: 402
      pdf_page: 419
    - "no": 4
      title: Representations and the Grothendieck Group
      page: 404
      pdf_page: 421
    - "no": 5
      title: Fourier Inversion Formula
      page: 406
      pdf_page: 423
    - "no": 6
      title: Schur Orthogonality Relations
      page: 409
      pdf_page: 426
    - "no": 7
      title: Orthogonality Relation for Characters
      page: 410
      pdf_page: 427
    - "no": 8
      title: Central Functions on a Finite Group
      page: 411
      pdf_page: 428
    - "no": 9
      title: The Case of Abelian Groups
      page: 414
      pdf_page: 431
    - "no": 10
      title: Characters and Grothendieck Groups
      page: 415
      pdf_page: 432
    - "no": 11
      title: Dimension of Simple Representations
      page: 415
      pdf_page: 432
    - "no": 12
      title: Change of Base Field
      page: 416
      pdf_page: 433
    - "no": 13
      title: Complex Linear Representations
      page: 421
      pdf_page: 438
statements: 34
exercises: 30
content_sha256: 9a1649fc8d1272ef983df643375471ca76019cb0c719210a9ce74942cd47c333
---

## § 21. LINEAR REPRESENTATIONS OF FINITE GROUPS

In this section, G is a group, and K is a commutative ring. If G is a finite group, then we denote by $|G|$ the element Card(G)$\cdot 1$ of K. From No. 5 on, we assume that the group G is finite, that the ring K is an algebraically closed field, and that $|G|$ is not zero.

### 1. Linear Representations

#### Definition 1 {#alg-viii-s21-def-1 .statement}

Let M be a K-module. A linear representation of G in M is a group homomorphism from G to the linear group $\mathbf{G}\mathbf{L}(M)$ (II, §1, No. 2, p. 195).

Let $\pi$ be a linear representation of G in a K-module M. We also say that the pair $(M, \pi )$ is a linear representation of G. When K is nonzero and M is a free K-module, the dimension of M is called the degree (or dimension) of the representation $\pi$.

Recall that the canonical mapping $g\mapsto e_g$ from G to the algebra K[G] of the group G is a basis of the K-module K[G]. By abuse of notation, we also denote the element $e_g$ of K[G] by $g$. Given a linear representation $\pi : G\rightarrow \mathbf{G}\mathbf{L}(M)$ of G, there exists a unique homomorphism of K-algebras from K[G] to End$_K(M)$ that extends $\pi$ (III, §2, No. 6, p. 447, Example); we also denote this extension by $\pi$. It is a representation of the algebra K[G] in M (VIII, p. 373, Definition 1), so that M is a K[G]-module. Conversely, every linear representation $\rho$ of the algebra K[G] in M defines a linear representation of G in M given by $g\mapsto \rho (g)$.

We will freely apply the terminology concerning the K[G]-module structure to linear representations of the group G. For example, we speak of a subrepresentation, a simple representation, a direct sum of representations, etc. Let $(M, \pi )$ and $(M', \pi ')$ be linear representations of G; we denote by Hom$_G(\pi , \pi ')$ the K-module Hom$_{K[G]}(M,M')$ of homomorphisms of K[G]-modules from M to $M'$.[^1]

A mapping $f$ from G to K is called a central function if we have $f(gg') =$ $f(g'g)$ for every pair $(g, g')$ of elements of G; equivalently, we have $f(ghg^{-1}) =$ $f(h)$ for every pair of elements $g, h$ of G. The central functions are therefore the functions on G whose restriction to each conjugacy class is constant. They form a submodule of the space of mappings from G to K, denoted by $\mathscr{Z}_K(G)$. When G is finite, the K-algebra $\mathscr{Z}_K(G)$ is a free K-module of dimension the number of conjugacy classes of G. The center Z(K[G]) of the algebra K[G] consists of the elements $a=\sum a_gg$ of K[G] such that $hah^{-1}=a$ for every $h\in G$. Now, we have

$$
hah^{-1}=_g\sum_{\in G}a_{h^{-1}gh}g
$$

consequently, when G is finite, the center Z(K[G]) of the algebra K[G] consists of the central functions.

Let $(M, \pi )$ be a linear representation of G. Suppose that M is a finite-dimensional free K-module. The trace of $\pi$ is the trace of the representation of K[G] associated with $\pi$, that is (VIII, p. 382), the linear form $a\mapsto$ Tr($\pi (a))$ on K[G]. This linear form is determined by the mapping $g\mapsto$ Tr($\pi (g))$ from G to K, which we call the character of the representation $\pi$ and denote by $\chi_{\pi}$. The character of a representation is a central function (II, §4, No. 3, p. 273, Proposition 3).

Let M and $M'$ be finite-dimensional free K-modules. Let $\pi$ and $\pi '$ be linear representations of G in M and $M'$, respectively. Then $M\oplus M'$ is a finite-dimensional free K-module, and, by Proposition 1 of III, §9, No. 2, p. 543, we have

$$
\chi_{\pi\oplus\pi'}=\chi_{\pi}+\chi_{\pi'}
$$

More generally, let

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

be an exact sequence of K[G] modules, and let $\pi ,\pi '$, and $\pi ''$ be the linear representations of G associated with $M, M'$, and $M''$, respectively. Suppose that the K-modules $M'$ and $M''$ are free and finite-dimensional. Then so is M (II, §1, No. 11, p. 218, Proposition 21), and we have

$$
\chi_{\pi}=\chi_{\pi'}+\chi_{\pi''} \tag{1}
$$

#### Proposition 1 {#alg-viii-s21-prop-1 .statement}

Suppose that K is a commutative field. Let $\pi$ and $\pi '$ be finite-dimensional semisimple K-linear representations of G.

a) If the characteristic polynomials of $\pi (g)$ and $\pi '(g)$ are the same for every $g\in G$, then the representations $\pi$ and $\pi '$ are isomorphic.

b) Suppose, moreover, that K has characteristic 0. If the characters $\chi_{\pi}$ and $\chi_{\pi'}$ are equal, then the representations $\pi$ and $\pi '$ are isomorphic.

Assertion a) follows from Corollary 1 of VIII, p. 386; assertion b) follows from part a) of the corollary of VIII, p. 384.

#### Example 1 {#alg-viii-s21-n1-exa-1 .statement}

The unit or trivial representation of G is the representation $(K, \varepsilon )$, where $\varepsilon (g) =$ Id$_K$ for every $g\in G$. Its character is the constant function with value 1.

#### Example 2 {#alg-viii-s21-n1-exa-2 .statement}

The (left) regular representation of G is the representation $\boldsymbol{\gamma }$ of G in K[G] defined by $\boldsymbol{\gamma }(g)(x) =gx$ for $g\in G$ and $x\in K[G]$. It corresponds to the left regular representation of the algebra K[G] (VIII, p. 375). Suppose that the group G is finite. The regular representation then has finite degree. For every element $g$ of G different from the identity, the matrix of left multiplication by $g$ in K[G] with respect to the canonical basis is the matrix of a permutation without fixed point. We therefore have

$|G|$ if $g$ is the identity element, (2) $\chi_{\boldsymbol{\gamma }}(g) =$

0 otherwise.

We define the right regular representation of G likewise. The biregular representation of G is the representation $\rho$ of $G\times G$ in K[G] defined by $\rho (g, g')(x) =gxg^{'-1}$ for $(g, g')\in G\times G$ and $x\in K[G]$.

#### Example 3 {#alg-viii-s21-n1-exa-3 .statement}

Given a linear representation $(M, \pi )$ of G, the contragredient or dual representation $\pi^{\vee}$ of $\pi$ is the representation of G in the K-module dual to M defined by the relation $\pi^{\vee}(g) =^t\pi (g^{-1})$ for every $g\in G$ (cf. II, §2, No. 5, p. 234). If M is a finite-dimensional free K-module, then so is its dual, and we have $\chi_{\pi^{\vee}}(g) =\chi_{\pi}(g^{-1})$ for every $g\in G$.

#### Example 4 {#alg-viii-s21-n1-exa-4 .statement}

Let $(M, \pi )$ and $(M', \pi ')$ be linear representations of G. In Example 1 of VIII, p. 198, we defined a K[G]-module structure on $M\otimes_KM'$. The corresponding linear representation is called the tensor product of $\pi$ and $\pi '$ and is denoted by $\pi \otimes \pi '$. For $g\in G,x\in M$, and $x'\in M'$, we have $(\pi \otimes \pi ')(g)(x\otimes x') =\pi (g)x\otimes \pi '(g)x'$.

If M and $M'$ are finite-dimensional free K-modules, then by Proposition 2 of III, §9, No. 2, p. 543, we have

$$
\chi_{\pi\otimes\pi'}=\chi_{\pi}\chi_{\pi'} \tag{3}
$$

#### Example 5 {#alg-viii-s21-n1-exa-5 .statement}

Suppose that G is the product $G'\times G''$ of two groups. The K-linear mapping from $K[G']\otimes_KK[G'']$ to K[G] that sends $g'\otimes g''$ to $(g', g'')$ for $g'\in G'$ and $g''\in G''$ is an algebra isomorphism. Let $(M', \pi ')$ be a linear representation of $G'$ and $(M'', \pi '')$ a linear representation of $G''$. The external tensor product of $\pi '$ and $\pi ''$, denoted by $\pi '\pi ''$, is the representation of $G'\times G''$ in the vector space $M'\otimes M''$ defined by $(\pi '\pi '')(g', g'') =\pi '(g')\otimes \pi ''(g'')$ for $(g', g'')\in G'\times G''$. If $M'$ and $M''$ are finite-dimensional free K-modules, then $M'\otimes_KM''$ is a finite-dimensional free K-module and the character of the representation $\pi '\pi ''$ is given by the formula

$$
\chi_{\pi'\pi''}(g', g'') =\chi_{\pi'}(g')\chi_{\pi''}(g'')
$$

for $g'\in G'$ and $g''\in G''$ (Proposition 2 of III, §9, No. 2, p. 542).

#### Example 6 {#alg-viii-s21-n1-exa-6 .statement}

Let $(V, \pi )$ be a linear representation of G such that V is a finite-dimensional free K-module. We define a representation $\rho$ of $G\times G$ in End$_K(V)$ by the formula

$$
\rho (g, g')(u) =\pi (g')\circ u\circ \pi (g^{-1})
$$

The K-module isomorphism $\theta_V: V^*\otimes_KV\rightarrow$ End$_K(V)$ of II, §4, No. 2, p. 271 is an isomorphism of representations from the external tensor product $\pi^{\vee}\pi$ to $\rho$. The mapping $g\mapsto \rho (1, g)$ (resp. $g\mapsto \rho (g,1))$ is a representation of G isomorphic to $\pi^{dim_KV}$ (resp. $(\pi^{\vee})^{dim_KV})$.

Let L be a commutative K-algebra, and let $(M, \pi )$ be a linear representation of the group G. The group homomorphism $\pi_{(L)}: G\rightarrow \mathbf{G}\mathbf{L}(M_{(L)})$ defined by $g\mapsto$ Id$_L\otimes \pi (g)$ is a linear representation of G in the L-module $M_{(L)}$, called the linear representation of G deduced from the representation $\pi$ by extension of the ring of scalars K to L.

Suppose that K is a field and that L is a nonzero commutative K algebra. Let $(M, \pi )$ and $(M', \pi ')$ be linear representations of G. The representations $\pi$ and $\pi '$ are isomorphic if and only if $\pi_{(L)}$ and $\pi '_{(L)}$ are (VIII, p. 37, Theorem 3).

Suppose, moreover, that the algebra L is an extension of K. Consider the rings $R_K(G)$ and $R_L(G)$ defined in Example 1 of VIII, p. 198. Extension of scalars defines a ring homomorphism

$$
u: R_K(G)\longrightarrow R_L(G)
$$

This homomorphism is injective, and an element $\xi \in R_K(G)$ is effective if and only if $u(\xi )$ is (VIII, p. 195, Theorem 1).

### 2. Maschke’s Theorem

#### Theorem 1 {#alg-viii-s21-thm-1 .statement}

Suppose that the group G is finite. Let M be a K[G]-module, and let N be a K[G]-submodule of M. Suppose that N is a direct factor of the K-module M and that $|G|$ is invertible in K. Then N is a direct factor of the K[G]-module M.

Let $p$ be a K-linear projector in M with image N. We define an endomorphism $q$ of the K-module M by setting

$$
q(x) =|G|^{-1}_g\sum_{\in G}g p(g^{-1}x)
$$

for every $x\in M$. Since N is stable under the action of G and $p$ induces the identity on N, we see that $q$ sends M into N and induces the identity on N.

The K-module M is therefore the direct sum of the image N of $q$ and the kernel of $q$. We have $g q(x) =q(gx)$ for every $x\in M$ and $g\in G$, so that the kernel of $q$ is a K[G]-submodule of M. This proves that N is a direct factor of the K[G]-module M.

Corollary 1 (Maschke). — Suppose that the group G is finite and that K is a commutative field. The algebra K[G] is semisimple if and only if the element $|G|$ of the field K is not zero.

Suppose $|G| \not= 0$. By Theorem 1, every K[G]-submodule of $K[G]_s$ is a direct factor. Hence K[G] is semisimple.

Conversely, suppose that $|G|$ is zero, and denote by $\varepsilon$ the element $\sum_{g\in G}g$ of the center of K[G]. We have $\varepsilon \not= 0$ but $\varepsilon^2=|G|\varepsilon = 0$, so K[G] is not semisimple (VIII, p. 153, Proposition 3, a) and VIII, p. 157, Remark 1).

#### Corollary 2 {#alg-viii-s21-thm-1-cor-2 .statement}

Suppose that the group G is finite and that $|G|$ is invertible in K. An exact sequence of K[G]-modules splits if and only if it splits as an exact sequence of K-modules.

Given an exact sequence of K[G]-modules

0 // $M_'^f$ // M // $M_{''}$ // $0$,

it suffices to apply Theorem 1 to the image of the morphism $f$.

#### Corollary 3 {#alg-viii-s21-thm-1-cor-3 .statement}

Suppose that the group G is finite and that $|G|$ is invertible in K. A K[G]-module is projective if and only if it is projective as a K-module.

Let P be a K[G]-module. If P is a direct factor of a free K[G]-module M, then it is a fortiori a direct factor of the free K-module M. The converse follows from Corollary 2, in view of II, §2, No. 2, p. 231, Proposition 4, d).

#### Corollary 4 {#alg-viii-s21-thm-1-cor-4 .statement}

a) Suppose that the group G is finite and that K is a commutative field of characteristic 0. Two finite-dimensional linear representations of G are isomorphic if and only if they have the same character.

b) Suppose that K is a perfect field of characteristic a prime number $p$ and that the group G is finite, of cardinal prime to $p$. The character of a finite-dimensional linear representation of G is zero if and only if this representation is isomorphic to the direct sum of $p$ pairwise isomorphic representations.

Under the assumptions of the corollary, every finite-dimensional linear representation of G is semisimple. The corollary then follows from the corollary of VIII, p. 384.

#### Corollary 5 {#alg-viii-s21-thm-1-cor-5 .statement}

Suppose that the group G is finite and that K is a commutative field in which $|G| \not= 0$. Let $\pi$ and $\pi '$ be finite-dimensional linear representations of G. Then $\pi$ and $\pi '$ are isomorphic if and only if for every $g$ in G, the endomorphisms $\pi (g)$ and $\pi '(g)$ have the same characteristic polynomial.

This follows from Corollary 1 of VIII, p. 386.

### 3. Induced and Coinduced Representations

Let H be a subgroup of the group G.

If $(V, \pi )$ is a linear representation of G, then the restriction of $\pi$ to H is a linear representation of H in V; we denote it by Res$^G_H(\pi )$. The K[H]module associated with Res$^G_H(\pi )$ is simply the module deduced from the K[G]-module V by restriction of scalars (II, §1, No. 13, p. 221). If V is a finite-dimensional free K-module, then the character of Res$^G_H(\pi )$ is the restriction of the character of $\pi$ to H.

Let $(M, \sigma )$ be a representation of H.

We view K[G] as a $(K[G]$, K[H])-bimodule and M as a K[H]-module. The K[G]-module $\mathscr{T}(M) = K[G]\otimes_{K[H]}M$ (VIII, p. 58) defines a linear representation of G, denoted by Ind$^G_H(\sigma )$ and called the representation of G induced by $\sigma$. If $(V, \pi )$ is a linear representation of G, then the K[H]-module $\mathscr{H}(V) =$ Hom$_{K[G]}(K[G],V)$ can be identified with the K[H]-module corresponding to the representation Res$^G_H(\pi )$. Consequently, the adjunction morphism (VIII, p. 59) gives a K-module isomorphism, called canonical, from Hom$_H(\sigma$, Res$^G_H(\pi ))$ to Hom$_G$(Ind$^G_H(\sigma ), \pi )$ (“Frobenius reciprocity”).

We view K[G] as a $(K[H]$, K[G])-bimodule. The K[G]-module $\mathscr{H}(M) =$ Hom$_{K[H]}(K[G],M)$ defines a representation of G, denoted by Coind$^G_H(\sigma )$ and called the representation of G coinduced by $\sigma$. If $(V, \pi )$ is a linear representation of G, then the K[H]-module $\mathscr{T}(V) = K[G]\otimes_{K[G]}V$ can be identified with the K[H]-module corresponding to the representation Res$^G_H(\pi )$. Consequently, the adjunction morphism (loc. cit.) gives a K-module isomorphism, called canonical, from Hom$_H$(Res$^G_H(\pi ), \sigma )$ to Hom$_G(\pi$, Coind$^G_H(\sigma ))$.

Let $\varepsilon : K[G]\rightarrow K[H]$ be the K-module homomorphism characterized by the relations $\varepsilon (h) =h$ if $h\in$ H and $\varepsilon (g) = 0$ if $g\in G$ H. The mapping $\varepsilon$ is a homomorphism of $(K[H]$, K[H])-bimodules. Let $(M, \sigma )$ be a linear representation of H. The mapping $v\mapsto v\circ \varepsilon$ from Hom$_{K[H]}(K[H],M)$ to Hom$_{K[H]}(K[G],M)$ is a homomorphism of K[H]-modules. By identifying M with Hom$_{K[H]}(K[H],M)$, we obtain a homomorphism of K[H]-modules from M to Res$^G_H$(Coind$^G_H(\sigma ))$. Frobenius reciprocity sends it to a homomorphism $\iota$ of K[G]-modules from Ind$^G_H(\sigma )$ to Coind$^G_H(\sigma )$ characterized by the relation

$$
\iota (g\otimes m)(g') =\varepsilon (g'g)m
$$

for $g, g'\in G$ and $m\in M$. This homomorphism is called canonical.

#### Proposition 2 {#alg-viii-s21-prop-2 .statement}

Let H be a subgroup of G, and let $(M, \sigma )$ be a linear representation of H. The canonical homomorphism $\iota :$ Ind$^G_H(\sigma )\rightarrow$ Coind$^G_H(\sigma )$ is injective. If the subgroup H has finite index in G, then $\iota$ is an isomorphism of K[G]-modules.

Let $S\subset G$ be a system of representatives of $G/H$. The family $(s)_{s\in S}$ is a basis of the right K[H]-module K[G]. It follows that the mapping $M^{(S)}\rightarrow$ Ind$^G_H(\sigma )$ defined by $(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ is an isomorphism of K-modules. For all $s, s'\in S$ and every $m\in M$, we have the relations

$_'-m$ if $s=s'$,

$$
\iota (s\otimes m)(s^1) =
$$

0 otherwise.

It follows that $\iota '$ is injective.

Suppose that H has finite index in G. The set S is then finite; let $\rho$ be the mapping from Coind$^G_H(\sigma )$ to Ind$^G_H(\sigma )$ given by $u\mapsto \sum_{s\in S}s\otimes u(s^{-1})$. It satisfies $(\iota \circ \rho (u))(s^{-1}) =u(s^{-1})$ for $u\in$ Coind$^G_H(\sigma )$ and $s\in S$. Since the family $(s^{-1})_{s\in S}$ is a basis of the left K[H]-module K[G], the mapping $\iota \circ \rho$ is the identity mapping. Consequently, $\iota$ is bijective with inverse bijection $\rho$.

Let H be a subgroup of G of finite index. Let $u$ be a central function on H; denote by $u^0$ the function on G that extends $u$ and that is zero at every point of G H. Let S be a system of representatives of $G/H$. For $g\in G$, set

(4) Ind$^G_H(u)(g) =\sum_{s\in S}u^0(s^{-1}gs)$.

Note that for all $x, g\in G$ and every $h\in H$, we have $u^0((xh)^{-1}gxh) =$ $u^0(x^{-1}gx)$. It follows that Ind$^G_H(u)$ is a central function on G that does not depend on the choice of S. We thus define a K-linear mapping Ind$^G_H$ from $\mathscr{Z}_K(H)$ to $\mathscr{Z}_K(G)$.

#### Proposition 3 {#alg-viii-s21-prop-3 .statement}

Let H be a subgroup of G of finite index. Let $(M, \sigma )$ be a linear representation of H. Suppose that M is a finite-dimensional free K-module. Denote by $(V, \pi )$ the representation of G induced by $\sigma$. Then the K-module V is free and finite-dimensional, and

(5) $\chi_{\pi}=$ Ind$^G_H(\chi_{\sigma})$.

Let S be a system of representatives of $G/H$. As we saw above, the linear mapping $M^S\rightarrow$ Ind$^G_H(M)$ given by $(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ is a K-module isomorphism. In particular, V is a finite-dimensional free K-module. For any $g\in G$, denote by $M_g$ the image of M by the mapping $m\mapsto g\otimes m$. For all $g, g'\in G$, we have $M_g= M_{g'}$ if and only if $gH =g'H$, and V is the direct sum of the submodules $M_s$ for $s\in S$. For all $g, g'\in G$, we also have $\pi (g)M_{g'}= M_{gg'}$. For any $g\in G$, denote by $S_g$ the set of elements $s$ of S such that $s^{-1}gs\in H$. For all $g, g'\in G$ such that $g^{'-1}gg'\in H$, the automorphism $\pi (g)$ of V induces an automorphism $\pi (g)_{g'}$ of $M_{g'}$, and we have

Tr($\pi (g)) =_s\sum_{\in S_g}$ Tr($\pi (g)_s) =_s\sum_{\in S_g}$ Tr($\sigma (s^{-1}gs))$.

The last assertion of the proposition follows.

### 4. Representations and the Grothendieck Group

In this subsection, we assume that K is a commutative field. Given a finite-dimensional linear representation $(M, \pi )$ of G, we denote by $[\pi ]$ the class of the K[G]-module M in the Grothendieck ring $R_K(G)$ (VIII, p. 198, Example 1).

By the definition of the laws of composition on the ring $R_K$(G), if $\pi$ and $\pi '$ are finite-dimensional linear representations of G, then we have

$$
[\pi \oplus \pi '] = [\pi ] + [\pi '],[\pi \otimes \pi '] = [\pi ] [\pi ']
$$

The unit element of the ring $R_K(G)$ is the class of the unit representation of G (VIII, p. 399, Example 1).

The ring $R_K(G)$ is a free $\mathbf{Z}$-module with basis the set of classes of simple K[G]-modules of finite dimension over K. When $|G|$ is invertible in K, two finite-dimensional representations are isomorphic if and only if they have the same class in $R_K(G)$ (VIII, p. 190, Corollary and p. 401, Corollary 1).

For every finite-dimensional linear representation $(M, \pi )$ of G, the contragredient $\pi^{\vee}$ is also finite-dimensional. The representations $\pi$ and $(\pi^{\vee})^{\vee}$ are isomorphic. If $\pi '$ is also a finite-dimensional linear representation of G, then the representations $(\pi \otimes \pi ')^{\vee}$ and $\pi^{\vee}\otimes \pi^{'\vee}$ are isomorphic. If

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

is an exact sequence of K[G]-modules of finite dimension over K, then the contragredient representations give an exact sequence of K[G]-modules

$$
0\longrightarrow M^{''\vee}\longrightarrow M^{\vee}\longrightarrow M^{'\vee}\longrightarrow 0
$$

(II, §7, No. 5, p. 299, Corollary of Theorem 5). By the universal property of Grothendieck groups (VIII, p. 186, Proposition 4), there exists an automorphism $c\mapsto c^{\vee}$ of the ring $R_K(G)$ characterized by $[\pi ]^{\vee}= [\pi^{\vee}]$ for every finite-dimensional linear representation $\pi$ of G; we have $(c^{\vee})^{\vee}=c$ for every element $c$ of $R_K(G)$.

Let H be a subgroup of G. Restriction preserves exact sequences. By the universal property of Grothendieck groups (loc. cit.), there consequently exists a group homomorphism, denoted by Res$^G_H$, from $R_K(G)$ to $R_K(H)$ characterized by the relation

(6) Res$^G_H[\pi ] =$ [Res$^G_H(\pi )]$

for every finite-dimensional linear representation $\pi$ of G; it is a ring homomorphism. If H has finite index in G, then by Proposition 14 of II, §7, No. 7, p. 306, we can define, analogously, a group homomorphism Ind$^G_H$ from $R_K(H)$ to $R_K(G)$ characterized by the relation

(7) Ind$^G_H[\sigma ] =$ [Ind$^G_H(\sigma )]$

for every finite-dimensional linear representation $\sigma$ of H.

By relations (1) of VIII, p. 399 and (3) of VIII, p. 400 and the universal property of Grothendieck groups mentioned above, there exists a ring homomorphism $Θ_G$ from $R_K(G)$ to the algebra $\mathscr{Z}_K(G)$ of central functions on G, characterized by $Θ_G([\pi ]) =\chi_{\pi}$ for every finite-dimensional representation $\pi$ of G.

If H is a subgroup of G, then the homomorphisms $Θ_G$ and $Θ_H$ associated with the groups G and H are compatible with the operations Res$^G_H$ and Ind$^G_H$ (VIII, p. 402 and VIII, p. 404, Proposition 3).

Suppose that G is the product $G'\times G''$ of two groups. By VIII, p. 213, Remark 2, there exists a $\mathbf{Z}$-linear mapping $\kappa$ from $R_K(G')\otimes_{\mathbf{Z}}R_K(G'')$ to the group $R_K(G'\times G'')$ characterized by the relation $\kappa ([\pi ']\otimes [\pi '']) = [\pi '\pi '']$ for $\pi '$ (resp. $\pi '')$ a finite-dimensional representation of $G'$ (resp. $G'')$ and $\pi '\pi ''$ the external tensor product (VIII, p. 400, Example 5). It is a ring homomorphism. If the field K is algebraically closed, then the mapping $\kappa$ is an isomorphism (VIII, p. 213, Remark 2).

Suppose that G is the product $G'\times G''$ of two groups. Denote by $\psi$ the homomorphism from $\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')$ to $\mathscr{Z}_K(G)$ that sends $f'\otimes f''$ to the function $(g', g'')\mapsto f'(g')f''(g'')$. The following diagram commutes:

$R_K(G_')\otimes_{\mathbf{Z}}R_K(G_{''})^{\kappa}$ // $R_K(G)$

$Θ_{G'}\otimes Θ_{G''}Θ_G$

$\mathscr{Z}_K(G_')\otimes_K\mathscr{Z}_K(G_{''})^{\psi}$ /$/\mathscr{Z}_K(G)$.

### 5. Fourier Inversion Formula

For the remainder of this section, we assume that the group G is finite and that K is an algebraically closed field whose characteristic does not divide the order of G, so that the element $|G|$ of K is not zero.

The algebra K[G] is semisimple (Maschke’s theorem) and finite-dimensional. Denote by $\widehat{G}$ the set of classes of simple K[G]-modules. For every $\lambda \in \widehat{G}$, choose a linear representation $(V_{\lambda}, \pi_{\lambda})$ of G such that the associated K[G]-module has class $\lambda$. The set $\widehat{G}$ is finite, and the vector spaces $V_{\lambda}$ are finite-dimensional (VIII, p. 141, Example). For any $\lambda \in \widehat{G}$, denote by $d_{\lambda}$ the degree of the representation $\pi_{\lambda}$, that is, the dimension of the K-vector space $V_{\lambda}$, and denote its character by $\chi_{\lambda}$.

Denote by $F(\widehat{G})$ the product algebra $\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ and by $\mathscr{F}$ the mapping from K[G] to $F(\widehat{G})$ defined by $\mathscr{F}(a) = (\pi_{\lambda}(a))_{\lambda\in\widehat{G}}$. Since the field K is algebraically closed, the mapping $\mathscr{F}$ is an algebra isomorphism (loc. cit.).

For every $\lambda \in \widehat{G}$, the dimension of the algebra End$_K(V_{\lambda})$ is $d^2_{\lambda}$; that of the algebra K[G] is Card(G). We therefore have the relation (8) Card(G) $=_{\lambda}\sum_{\in\widehat{G}}d^2_{\lambda}$.

Denote by $\tau$ the trace in the algebra K[G]; by definition, the trace $\tau (a)$ of an element $a$ of K[G] is the trace of the endomorphism $x\mapsto ax$ of K[G] (III, §7, No. 7, p. 515). Let $a=\sum_{g\in G}a_gg$ be an element of K[G]; by formula (2), we have $\tau (ag^{-1}) =|G|a_g$ for every $g\in G$, and therefore the relation (9) $a=|G|^{-1}_g\sum_{\in G}\tau (ag^{-1})g$.

Denote by $\widehat{\tau}$ the trace in the algebra $F(\widehat{G})$. Let $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ be an element of $F(\widehat{G})$; we have (cf. III, §9, No. 3, p. 545, Example 3) (10) $\widehat{\tau}(A) =\sum d_{\lambda}$ Tr(A$_{\lambda})$.

Since the mapping $\mathscr{F}$ is a K-algebra isomorphism, we have$^{\lambda\in\widehat{G}}\widehat{\tau}\circ \mathscr{F}=\tau$, and therefore

$\tau (a) =\widehat{\tau}(\mathscr{F}(a)) =\widehat{\tau}(\pi_{\lambda}(a))_{\lambda\in\widehat{G}}=\sum d_{\lambda}$ Tr($\pi_{\lambda}(a)) =\sum d_{\lambda}$ Tr$_{\lambda}(a)$

for every $a\in K[G]$, that is $\lambda^{\in\widehat{G}\lambda\in\widehat{G}}$ (11) $\tau =\sum d_{\lambda}$ Tr$_{\lambda}$.

Therefore, by (2) of VIII, p. 399$,^{\lambda}$for$^{\in\widehat{G}}g\in G$, we have

$\sum|G|$ if $g$ is the identity element, (12) $d_{\lambda}\chi_{\lambda}(g) =$

0 otherwise$$. For $a\in K[G]$, relation $(^{\lambda\in\widehat{G}}$ 9) takes on the following form: (13) $a=|G|^{-1}_g\sum_{\in G\lambda}\sum_{\in\widehat{G}}d_{\lambda}$ Tr($\pi_{\lambda}(a)\pi_{\lambda}(g^{-1}))g$;

it follows that for every element $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ of $F(\widehat{G})$, we have (14) $\mathscr{F}^{-1}(A) =|G|^{-1}_g\sum_{\in G\lambda}\sum_{\in\widehat{G}}d_{\lambda}$ Tr(A$_{\lambda}\pi_{\lambda}(g^{-1}))g$ (“Fourier inversion formula”).

For $µ\in \widehat{G}$, denote by $j_µ:$ End$_K(V_µ)\longrightarrow \prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ the mapping such that $j_µ(u) = (v_{\lambda})$, where $v_{\lambda}= 0$ if $\lambda \not=µ$ and $v_µ=u$. By formula (14), we have (15) $\mathscr{F}^{-1}(j_µ(u)) =|G|^{-1}d_{µg}\sum_{\in G}$ Tr($u\pi_µ(g^{-1}))g$.

The center of the algebra $F(\widehat{G}) =\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ consists of the families $(a_{\lambda}1_{V_{\lambda}})_{\lambda\in\widehat{G}}$, where $(a_{\lambda})$ is a family of elements of K. It is the image by $\mathscr{F}$ of the center of the algebra K[G]. That center therefore has a basis $(e_{\lambda})_{\lambda\in\widehat{G}}$ characterized by the relation (16) $\pi_{\lambda}(e_µ) =\delta_{\lambda µ}1_{V_{\lambda}}$

for $\lambda , µ\in \widehat{G}$, where $\delta_{\lambda µ}$ is the Kronecker delta function. By formula (15), we have, for every $µ\in \widehat{G}$, (17) $e_µ=|G|^{-1}d_{µg}\sum_{\in G}\chi_µ(g^{-1})g$.

These elements satisfy the relations (18) $\sum e_{\lambda}= 1,e^2_µ=e_µ$, and $e_µe_{\nu}= 0$

for all $µ, \nu \in \widehat{G}$ such that$^{\lambda\in\widehat{G}}µ\not=\nu$; they are the indecomposable idempotents of Z(K[G]) (VIII, p. 147, Proposition 15)

#### Remark {#alg-viii-s21-n5-rem-1 .statement}

Let $(V, \pi )$ be a linear representation of G. By Maschke’s theorem, the K[G]-module V is semisimple. For any $\lambda \in \widehat{G}$, denote by $V^{\lambda}$ the isotypical component of type $\lambda$ of the K[G]-module V; we have $V =\bigoplus_{\lambda\in\widehat{G}}V^{\lambda}$. By Proposition 15 of VIII, p. 147 and formula (17), the projector of V with image $V^{\lambda}$ associated with this decomposition of V is equal to (19) $\pi (e_{\lambda}) =|G|^{-1}d_{\lambda g}\sum_{\in G}\chi_{\lambda}(g^{-1})\pi (g)$.

Applying this formula to $\pi =\pi_{\lambda}$, we obtain that the element $d_{\lambda}\cdot 1$ of K is not zero. We will see further on (VIII, p. 420, Corollary 2) that $d_µ$ divides the cardinal of G.

Let $\lambda$ be an element of $\widehat{G}$. The mapping $\pi_{\lambda}$ from K[G] to End$_K(V_{\lambda})$ induces an isomorphism of $(K[G]$, K[G])-bimodules from $e_{\lambda}K[G]$ to End$_K(V_{\lambda})$. By Proposition 15 of VIII, p. 147, the K[G]-submodule $e_{\lambda}K[G]$ is the isotypical component of K[G] of type $\lambda$. It is also the isotypical component of type $\lambda^{\vee}$ for the right regular representation of G (VIII, p. 143, Proposition 11) as well as the isotypical component of type $\lambda \times \lambda^{\vee}$ for the biregular representation (VIII, p. 381, Proposition 4).

### 6. Schur Orthogonality Relations

We keep the notation of the previous subsection. Let $\lambda$ be an element of $\widehat{G}$, and let $u$ and $v$ be elements of End$_K(V_{\lambda})$; by formula (10), we have

$\tau$ˆ$(j_{\lambda}(u)j_{\lambda}(v)) =d_{\lambda}$ Tr($uv)$. Since $\tau =$ ˆ$\tau \circ \mathscr{F}$, we deduce from formulas (2) and (15) the relation

$d^2_{\lambda}|G|^{-1}_g\sum_{\in G}$ Tr($u\pi_{\lambda}(g))$ Tr($v\pi_{\lambda}(g^{-1})) =d_{\lambda}$ Tr($uv)$.

We observed previously that $d_{\lambda}.1\not= 0$ in the field K; it follows that (20) $|G|^{-1}_g\sum_{\in G}$ Tr($u\pi_{\lambda}(g))$ Tr($v\pi_{\lambda}(g^{-1})) =d^-_{\lambda}^1$ Tr($uv)$.

Let us apply this relation to the case when $u$ and $v$ have rank $\leqslant 1$; we obtain (21) $|G|^{-1}_g\sum_{\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\lambda}(g^{-1})y\rangle =d^-_{\lambda}^1\langle x^*, y\rangle \langle y^*, x\rangle$

for $x,y$ in $V_{\lambda}$ and $x^*, y^*$ in the dual $V^*_{\lambda}$ of $V_{\lambda}$.

For every $\lambda \in \widehat{G}$, let $(e_{\lambda ,j})_{1\leqslant j\leqslant d_{\lambda}}$ be a basis of $V_{\lambda}$; denote by $(\pi^{\lambda}_{ij}(g))$ the matrix of the endomorphism $\pi_{\lambda}(g)$ of $V_{\lambda}$ with respect to this basis. If we denote by $(e^*_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ the basis of $V^*_{\lambda}$ dual to $(e_{\lambda ,j})$, then we have $\pi^{\lambda}_{ij}(g) =\langle e^*_{\lambda ,i}, \pi_{\lambda}(g)e_{\lambda ,j}\rangle$, and therefore (22) $|G|^{-1}_g\sum_{\in G}\pi_{ij}^{\lambda}(g)\pi^{\lambda}_{k`}(g^{-1}) =d^-_{\lambda}^1\delta_{i`}\delta_{jk}$.

Now let $\lambda$ and $µ$ be two distinct elements of $\widehat{G}$, and let $u\in$ End$_K(V_{\lambda})$ and $v\in$ End$_K(V_µ)$. Again by relation (15), we have (23) $g\sum_{\in G}$ Tr($u\pi_{\lambda}(g))$ Tr($v\pi_µ(g^{-1})) = 0$.

As above, we deduce that (24) $g\sum_{\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_µ(g^{-1})y\rangle = 0$

for $x\in V_{\lambda},x^*\in V^*_{\lambda},y\in V_µ$, and $y^*\in V^*_µ$. We also have (25) $g\sum_{\in G}\pi^{\lambda}_{ij}(g)\pi^µ_{k`}(g^{-1}) = 0$ for $i, j$ in $[1, d_{\lambda}]$ and $k, `$ in $[1, d_µ]$.

Relations (20) through (25) are known as the Schur orthogonality relations.

#### Remark {#alg-viii-s21-n6-rem-1 .statement}

We identify the algebra End$_K(V_{\lambda})$ with the matrix algebra $\mathbf{M}_{d_{\lambda}}(K)$ via the basis $(e_{\lambda ,j})$ of $V_{\lambda}$. The mapping $\mathscr{F}^{-1}$ is an isomorphism from the algebra $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ to the algebra K[G]. For $µ\in \widehat{G}$, denote by $E^µ_{ij}$ the element of $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ whose component of index $µ$ is the matrix unit $E_{ij}$ of $\mathbf{M}_{d_µ}(K)$ (II, §10, No. 3, p. 341) and whose other components are zero; set $u^µ_{ij}=\mathscr{F}^{-1}(E^µ_{ij})$. The family of elements $u^{\lambda}_{ij}$, for $\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}$, $1\leqslant j\leqslant d_{\lambda}$, is a basis of the algebra K[G]; the multiplication table is

$$
u^{\lambda}_{ij}u^µ_{k`}=\delta_{\lambda µ}\delta_{jk}u^{\lambda}_{i`} \tag{26}
$$

Moreover, by formula (15), we have

$$
u^{\lambda}_{ij}=|G|^{-1}d_{\lambda g}\sum_{\in G}\pi^{\lambda}_{ji}(g^{-1})g \tag{27}
$$

### 7. Orthogonality Relation for Characters

We keep the notation of Subsections 5 and 6. Recall that Z(K[G]) consists of the central functions.

We define a symmetric bilinear mapping from $K[G]\times K[G]$ to K by the formula

$$
\langle f, f'\rangle_G=|G|^{-1}_g\sum_{\in G}f_gf_g'_{_{-1}} \tag{28}
$$

for every $f=\sum f_gg$ and $f'=\sum f_g'g$ belonging to K[G]. We have $\langle f, f'\rangle_G=$ $|G|^{-2}\tau (f f')$.

Proposition 4 (Orthogonality relation for characters)

For $\lambda$ and $µ$ in $\widehat{G}$, we have $\langle \chi_{\lambda}, \chi_µ\rangle_G=\delta_{\lambda µ}$.

This is the specific case of relations (20) and (23) when the endomorphisms $u$ and $v$ are taken to be the identity.

#### Corollary {#alg-viii-s21-n7-cor-1 .statement}

Let $\pi$ and $\pi '$ be finite-dimensional linear representations of G. In the field K, we have

(29) $\langle \chi_{\pi}, \chi_{\pi'}\rangle_G=$ (dim$_K$ Hom$_G(\pi , \pi '))\cdot 1$.

We first suppose that $\pi$ and $\pi '$ are simple representations. The vector space Hom$_G(\pi , \pi ')$ has dimension 1 or 0 according to whether or not $\pi$ and $\pi '$ are isomorphic (Schur’s lemma, VIII, p. 47, Proposition 2). In this case, formula (29) follows from Proposition 4.

In the general case, the representation $\pi$ (resp. $\pi ')$ is the direct sum of simple representations $\pi_1, . . . , \pi_m$ (resp. $\pi '_1, . . . , \pi_n')$. The space Hom$_G(\pi , \pi ')$ is isomorphic to the direct sum of the spaces Hom$_G(\pi_i, \pi '_j)$ for $1\leqslant i\leqslant m$, $1\leqslant j\leqslant n$, and we have

$$
\chi_{\pi}=\chi_{\pi_1}+\cdots +\chi_{\pi_m},\chi_{\pi'}=\chi_{\pi'_1}+\cdots +\chi_{\pi'_n}
$$

By linearity, the proof of formula (29) is reduced to the case of simple representations.

### 8. Central Functions on a Finite Group

#### Proposition 5 {#alg-viii-s21-prop-5 .statement}

The family $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ is a basis of the vector space of central functions. The number of classes of simple linear representations of G is equal to the number of conjugacy classes of G.

For $a=\sum_{g\in G}a_gg\in K[G]$, write $a^{\vee}=\sum_{g\in G}a_{g^{-1}}g$; the mapping $a\mapsto a^{\vee}$ is an involutive antiautomorphism of the algebra K[G]. By formula (17), we have $e_{\lambda}=|G|^{-1}d_{\lambda}\chi^{\vee}_{\lambda}$ for every $\lambda \in \widehat{G}$. The proposition then follows from the fact that the family $(e_{\lambda})_{\lambda\in\widehat{G}}$ is a basis of the center of K[G].

Denote by $\mathscr{C}$ the set of conjugacy classes of G. Let C be an element of $\mathscr{C}$; the image $C^{-1}$ of C by the mapping $g\mapsto g^{-1}$ is a conjugacy class. The commutants of the elements of C are mutually conjugate subgroups of G; their cardinal $d(C)$ satisfies

(30) Card(G) = Card(C) $d(C)$.

In particular, we have $d(C)\cdot 1\not= 0$ in the field K.

Let $f$ be a central function on G. For any conjugacy class C, denote by $f(C)$ the common value of the $f(x)$ for $x\in C$. With this notation, the orthogonality relation for characters (VIII, p. 410, Proposition 4) can be written as

$$
C\sum_{\in\mathscr{C}}\chi_{\lambda}(C^{-1})\chi_µ(C)d(C)^{-1}=\delta_{\lambda µ} \tag{31}
$$

for $\lambda$ and $µ$ in $\widehat{G}$.

Denote by A the matrix of type $\widehat{G}\times \mathscr{C}$ with entries $\chi_{\lambda}(C)$ and by B the matrix of type $\mathscr{C}\times \widehat{G}$ with entries $\chi_{\lambda}(C^{-1})d(C)^{-1}$. The sets $\widehat{G}$ and $\mathscr{C}$ have the same cardinal (Proposition 5); relation (31) expresses the fact that the matrix product AB is the matrix unit of type $\widehat{G}\times \widehat{G}$. By Proposition 11 of II, §10, No. 12, p. 360, the matrix product BA is the matrix unit of type $\mathscr{C}\times \mathscr{C}$; in other words, we have the relation

$$
\sum\chi_{\lambda}(C^{-1})\chi_{\lambda}(C') =d(C)\delta_{CC'} \tag{32}
$$

for C and $C'$ in $\mathscr{C}$ (sometimes called the “$^{\lambda\in\widehat{G}}$ second orthogonality relation for characters”).

Let H be a subgroup of G. Let us note that the integer Card(H) divides Card(G) and that $|G|$ is not zero in K; we therefore have $|H| \not= 0$ in K.

Denote by Res$^G_H$ the linear mapping from Z(K[G]) to Z(K[H]) that sends a central function on G to its restriction to H. We have seen that if $\chi_{\pi}$ is the character of a finite-dimensional representation $\pi$ of G, then Res$^G_H(\chi_{\pi})$ is the character of the representation Res$^G_H(\pi )$ of H.

#### Proposition 6 {#alg-viii-s21-prop-6 .statement}

Let $f$ be a central function on G and $u$ be a central function on H. We have

(33) $\langle$Ind$^G_H(u), f\rangle_G=\langle u$, Res$^G_H(f)\rangle_H$.

The characters of the simple representations of G form a basis of Z(K[G]) (VIII, p. 411, Proposition 5), and the same holds for H. It therefore suffices to establish (33) in the case when $f$ is the character $\chi_{\pi}$ of a simple representation $\pi$ of G and $u$ is the character $\chi_{\sigma}$ of a simple representation $\sigma$ of H. In this case, Ind$^G_H(u)$ is the character of the representation Ind$^G_H(\sigma )$ of G, and, by VIII, p. 410, Corollary, we have

$\langle$Ind$^G_H(u), f\rangle_G=$ (dim$_K$ Hom$_G$(Ind$^G_H(\sigma ), \pi ))\cdot 1$.

We show the relation

$\langle u$, Res$^G_H(f)\rangle_H=$ (dim$_K$ Hom$_H(\sigma$, Res$^G_H(\pi )))\cdot 1$

likewise, and equality (33) follows by Frobenius reciprocity.

#### Proposition 7 {#alg-viii-s21-prop-7 .statement}

Let $f$ be a mapping from G to K. The following assertions are equivalent:

(i) There are an element $\lambda$ of $\widehat{G}$ and an element $a$ of K such that $f=a\chi_{\lambda}$.

(ii) For every pair $(g, g')$ of elements of G, we have (34) $f(g)f(g') =|G|^{-1}f(1)_h\sum_{\in G}f(hgh^{-1}g')$.

Let $\lambda$ be an element of $\widehat{G}$; for every endomorphism $u$ of $V_{\lambda}$, set (35) $u^\=|G|^{-1}_h\sum_{\in G}\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})$.

The endomorphism $u^\$ of $V_{\lambda}$ is K[G]-linear. By Schur’s lemma (VIII, p. 47, Theorem 1$),u^\$ is a homothety. Since $u$ and $u^\$ have the same trace, we therefore have

$u^\=d^-_{\lambda}^1$ Tr($u) 1_{V_{\lambda}}$. Let $u$ and $v$ be endomorphisms of $V_{\lambda}$; it follows that (36) Tr($u)$ Tr($v) =d_{\lambda}$ Tr($u^\v) =d_{\lambda}|G|^{-1}_h\sum_{\in G}$ Tr($\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})v)$.

Take $u=\pi_{\lambda}(g)$ and $v=\pi_{\lambda}(g')$ in formula (36); relation (34) for $f=\chi_{\lambda}$ follows.

Conversely, suppose that assertion (ii) holds. If we have $f(1) = 0$, then it follows that $f(g)f(g') = 0$ for every pair $(g, g')$ of elements of G, and therefore $f= 0$. We can therefore assume $f(1)\not= 0$. Taking $g'= 1$ in (34), we obtain the relation

$$
f(g) =|G|^{-1}_h\sum_{\in G}f(hgh^{-1})
$$

for every $g\in G$, which implies that $f$ is a central function. By Proposition 5, there exists a family $(a_{\lambda})$ of elements of K such that $f=\sum_{\lambda\in\widehat{G}}a_{\lambda}\chi_{\lambda}$. Let us replace $f$ with this expression in formula (34); taking into account that each of the characters $\chi_{\lambda}$ also satisfies this relation, we find (37) $\sum a_{\lambda}a_µ\chi_{\lambda}(g)\chi_µ(g') =\sum a_{\lambda}d^-_{\lambda}^1f(1)\chi_{\lambda}(g)\chi_{\lambda}(g')$

for $g, g'\in^{\lambda ,µ}G$. This relation can also be written as$^{\in\widehat{G}\lambda\in\widehat{G}}$ (38) $\sum_{\lambda ,µ}(a_{\lambda}a_µ-\delta_{\lambda µ}a_{\lambda}d^-_{\lambda}^1f(1))\chi_{\lambda}(g)\chi_µ(g') = 0$

for $g, g'\in G$. Now, the functions $\chi_{\lambda}$, for $\lambda \in \widehat{G}$, are linearly independent (Proposition 5 of VIII, p. 411); it follows that

$$
a_{\lambda}a_µ=\delta_{\lambda µ}a_{\lambda}d^-_{\lambda}^1f(1)
$$

for $\lambda , µ\in \widehat{G}$. In particular, $a_{\lambda}a_µ= 0$ whenever $\lambda \not=µ$. Consequently, there exists at most one element $\lambda$ of $\widehat{G}$ such that $a_{\lambda}\not= 0$, and we have $f=a_{\lambda}\chi_{\lambda}$, and therefore (i).

### 9. The Case of Abelian Groups

In this subsection, we assume that the group G is abelian.

By Schur’s lemma (VIII, p. 48, Corollary 1), every simple representation of G has dimension 1. Let $(M, \pi )$ be such a representation and $\chi$ be its character; for every $g\in G$ and $x\in M$, we have $\pi (g)(x) =\chi (g)x$. Consequently, the character $\chi$ is a homomorphism from G to the multiplicative group $K^*$ of K. Conversely, every homomorphism from G to $K^*$ is the character of a representation of G of degree 1. So the set $\widehat{G}$ of classes of simple K[G]-modules can be identified with the set Hom(G$,K^*)$ of homomorphisms from G to $K^*$. We deduce from this an abelian group structure on $\widehat{G}$; the product in $\widehat{G}$ corresponds to the tensor product of representations. The groups G and $\widehat{G}$ have the same cardinal by Proposition 5 of VIII, p. 411. Every function on G is central, and $\widehat{G}$ is a basis of the vector space of mappings from G to K (loc. cit.). Because of the orthogonality relation for characters, such a mapping $f$ has the following unique decomposition with respect to the basis $\widehat{G}:$

$$
f=\sum\langle \chi , f\rangle_G\chi \tag{39}
$$

For mappings $f$ and $f'$ from G to K, we have the relation$^{\chi\in\widehat{G}}$

$$
\langle f, f'\rangle_G=_{\chi}\sum_{\in\widehat{G}}\langle \chi , f\rangle_G\langle \chi , f'\rangle_G \tag{40}
$$

Let $(V, \pi )$ be a linear representation of G. For any $\chi \in \widehat{G}$, denote by $V^{\chi}$ the subspace of V consisting of the vectors $v$ such that $\pi (g)(v) =\chi (g)v$ for every $g\in G$. The space $V^{\chi}$ is the isotypical component of type $\chi$ of the K[G]-module V. The space V is the direct sum of the family $(V^{\chi})_{\chi\in\widehat{G}}$, and the projector $p_{\chi}$ of V with image $V^{\chi}$ associated with this decomposition is given by

$$
p_{\chi}=|G|^{-1}_g\sum_{\in G}\chi (g^{-1})\pi (g) \tag{41}
$$

because of relation (19).

#### Remark {#alg-viii-s21-n9-rem-1 .statement}

Let $n$ be the cardinal of the group G, and let $µ_n(K)$ be the group of $n$-th roots of unity in K. For every $g\in G$, we have $g^n= 1$; consequently, $\widehat{G}$ can be identified with the group Hom(G$, µ_n(K))$. The group $µ_n(K)$ is cyclic of order $n$ (V, §11, No. 2, p. 78, Theorem 1). The group $\widehat{G}$ is therefore isomorphic to the group D(G) = Hom(G$,\mathbf{Q}/\mathbf{Z})$. By VII, §4, No. 9, p. 26, Proposition 10, the group $\widehat{G}$ is isomorphic to the group G, and the mapping that sends an element $g$ of G to the homomorphism $\chi \mapsto \chi (g)$ from $\widehat{G}$ to $K^*$ is an isomorphism from G to $\widehat{\widehat{G}}$.

### 10. Characters and Grothendieck Groups

Denote by $\theta_G$ the K-algebra homomorphism from $K\otimes_{\mathbf{Z}}R_K(G)$ to $\mathscr{Z}_K(G)$ that sends $1\otimes [\pi ]$ to $\chi_{\pi}$ for every finite-dimensional representation $\pi$.

#### Proposition 8 {#alg-viii-s21-prop-8 .statement}

a) The homomorphism $\theta_G$ is an isomorphism from $K\otimes_{\mathbf{Z}}R_K(G)$ to $\mathscr{Z}_K(G)$.

b) Suppose that K has characteristic 0. Then $\theta_G$ defines an isomorphism from $R_K(G)$ to the subring of $\mathscr{Z}_K(G)$ consisting of the linear combinations of the characters $\chi_{\lambda}$ for $\lambda$ in $\widehat{G}$ with integer coefficients.

The family $([\lambda ])_{\lambda\in\widehat{G}}$ is a basis of the $\mathbf{Z}$-module $R_K$(G), and the family $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ is a basis of the K-vector space $\mathscr{Z}_K(G)$. Assertions a) and b) follow (VIII, p. 411, Proposition 5).

### 11. Dimension of Simple Representations

Denote the cardinal of the group G by $n$. Let $\pi$ be a linear representation of G in a finite-dimensional K-vector space M. For every $g\in G$, we have $\pi (g)^n= 1_M$, so the minimal polynomial of $\pi (g)$ divides $T^n-1$. Since $n\cdot 1\not= 0$ in K, this minimal polynomial is separable (V, §11, No. 2, p. 78), and since the field K is algebraically closed, the endomorphism $\pi (g)$ of M is diagonalizable (VII, §5, No. 7, p. 40, Proposition 12). The eigenvalues of $\pi (g)$ are $n$-th roots of unity, and for every $\alpha \in K$, the geometric multiplicity of $\alpha$ as an eigenvalue of $\pi (g)$ (VII, §5, No. 2, p. 30, Definition 1) is equal to the multiplicity of $\alpha$ as a root of the characteristic polynomial of $\pi (g)$. Denote by $\mathscr{O}_n$ the subgroup of K generated by the set $µ_n(K)$ of $n$-th roots of unity; it is a finitely generated $\mathbf{Z}$-module and a subring of K. The character of $\pi$ takes its values in $\mathscr{O}_n$.

#### Proposition 9 {#alg-viii-s21-prop-9 .statement}

Suppose that the field K has characteristic zero. Then the degree of every simple representation of G divides the cardinal of G.

Let $(V, \pi )$ be a simple representation of G and $\chi$ be its character. For every element $a$ of Z(K[G]), the endomorphism $\pi (a)$ of V is a homothety (VIII, p. 47, Theorem 1); denote by $\varphi (a)$ the scalar such that $\pi (a) =\varphi (a)_V$. The resulting mapping $\varphi$ from Z(K[G]) to K is an algebra homomorphism. Let us take $a=\sum_{g\in G}\chi (g^{-1})g$; by the remark of VIII, p. 408, we have $\varphi (a) =$ (dim $V)^{-1}|G|$. On the other hand, $a$ belongs to the subring $\mathscr{O}_n[G]\cap Z(K[G])$ of K[G], which is a finitely generated $\mathbf{Z}$-module (VII, §3, p. 15, Corollary). So the element $\varphi (a) =$ (dim $V)^{-1}|G|$ of K belongs to a subring of K that is a finitely generated $\mathbf{Z}$-module. We conclude using the following lemma.

#### Lemma {#alg-viii-s21-n11-lem-1 .statement}

Let L be an extension of $\mathbf{Q}$. Let A be a subring of L. Suppose that A is a finitely generated $\mathbf{Z}$-module. We have $A\cap \mathbf{Q}=\mathbf{Z}$.

Since the $\mathbf{Z}$-module $A\cap \mathbf{Q}$ is finitely generated, there exists a strictly positive integer N such that $A\cap \mathbf{Q}$ is contained in $_N^1\mathbf{Z}$. Let $x$ be an element of $\mathbf{Q}\mathbf{Z}$; we write it as $x=^p_q$, where $p$ and $q$ are mutually prime integers and $q\geqslant 2$. We have $q^N\geqslant 2^N>N ($Set Theory, III, §3, No. 6, p. 165, Theorem 2), the integers $p^N$ and $q^N$ are mutually prime, and consequently $x^N\in /_N^1\mathbf{Z}$. It follows that $x$ does not belong to A. This concludes the proof of the lemma.

In the next subsection, we extend Proposition 9 to the case when we only assume that the characteristic of K does not divide the order of G.

### 12. Change of Base Field

We keep the notation of the previous subsection. Let $K'$ be an algebraically closed field such that the element $n\cdot 1$ of $K'$ is not zero. The groups $µ_n(K)$ and $µ_n(K')$ are cyclic of order $n$ (V, §11, No. 2, p. 78, Theorem 1). Choose an isomorphism $\varphi$ from $µ_n(K)$ to $µ_n(K')$. Let $\pi$ be a linear representation of G in a finite-dimensional K-vector space, and let $\pi '$ be a linear representation of G in a finite-dimensional $K'$-vector space. We say that $\pi$ and $\pi '$ are related (through $\varphi )$ if for every $g\in G$ and $\omega \in µ_n$(K), the multiplicity of $\omega$ as an eigenvalue of $\pi (g)$ is equal to the multiplicity of $\varphi (\omega )$ as an eigenvalue of $\pi '(g)$. When this is the case, $\pi$ and $\pi '$ have the same dimension, as can be seen by taking $g= 1$.

Let $\pi_1$ and $\pi_2$ (resp. $\pi_1'$ and $\pi_2')$ be linear representations of G in finite-dimensional vector spaces over K (resp. $K')$. We have the following properties:

a) If $\pi_1$ is related to $\pi '_1$ and $\pi_2'$, then $\pi '_1$ and $\pi_2'$ are isomorphic.

b) If $\pi_1$ is related to $\pi '_1$ and $\pi_2$ to $\pi_2'$, then $\pi_1\oplus \pi_2$ is related to $\pi '_1\oplus \pi_2'$ and $\pi_1\otimes \pi_2$ is related to $\pi '_1\otimes \pi_2'$.

Assertion a) follows from Corollary 5 of VIII, p. 402, and assertion b) is clear.

Here, we denote by $\mathscr{S}_K(G)$ the set of classes of simple K[G]-modules, previously denoted by $\widehat{G}$, and we define $\mathscr{S}_{K'}(G)$ likewise. The sets $\mathscr{S}_K(G)$ and $\mathscr{S}_{K'}(G)$ are both finite, with cardinal the number of conjugacy classes (VIII, p. 411, Proposition 5).

#### Proposition 10 {#alg-viii-s21-prop-10 .statement}

There exists a unique mapping $\varphi_G$ from $\mathscr{S}_K(G)$ to $\mathscr{S}_{K'}(G)$ such that $\lambda$ and $\varphi_G(\lambda )$ are related through $\varphi$ for every $\lambda$ in $\mathscr{S}_K(G)$. Moreover, $\varphi_G$ is bijective.

The uniqueness of $\varphi_G$ follows from property a) above.

A) Suppose that the field K has characteristic 0.

The group $µ_n(K)$ is cyclic (V, §11, No. 2, p. 78, Theorem 1); choose a generator $\zeta$ of this group. Consider the ring homomorphism $\rho :\mathbf{Z}[X]\rightarrow \mathscr{O}_n$ that sends X to $\zeta$. It is surjective. The cyclotomic polynomial $Φ_n(X)$ is irreducible in $\mathbf{Q}[X]$ (V, §11, No. 5, p. 84, Theorem 2); it is therefore the minimal polynomial of $\zeta$ over $\mathbf{Q}$. The polynomial $Φ_n$ is monic with integer coefficients (V, §11, No. 4, p. 81). Let $P\in \mathbf{Z}[X]$ be a polynomial such that $P(\zeta ) = 0$; by Euclidean division of polynomials (IV, §1, No. 6, p. 10), there exist two polynomial Q and R in $\mathbf{Z}[X]$ such that P = QΦ$_n+ R$ and deg(R) $<$ deg(Φ$_n)$. We have $R(\zeta ) = 0$, and therefore R = 0 because $Φ_n$ is the minimal polynomial of $\zeta$. Consequently, the kernel of $\rho$ is the ideal $Φ_n\mathbf{Z}[X]$ of $\mathbf{Z}[X]$, and $\rho$ induces a ring isomorphism from $\mathbf{Z}[X]/Φ_n\mathbf{Z}[X]$ to $\mathscr{O}_n$.

Set $\zeta '=\varphi (\zeta )$; it is a primitive $n$-th root of unity in $K'$, and we therefore have $Φ_n(\zeta ') = 0$ (V, §11, No. 5, p. 83, Lemma 3). Consequently, there exists a homomorphism $\varphi_0$ from the ring $\mathscr{O}_n$ to the field $K'$ that transforms $\zeta$ into $\zeta '$; it extends the mapping $\varphi$ from $µ_n(K)$ to $µ_n(K')$. Let $\mathscr{O}$ be the subring of K consisting of the elements $_n^{a_r}$ with $a\in \mathscr{O}_n$ and $r\in \mathbf{N}$. Since $n\cdot 1$ is invertible in $K'$, the homomorphism $\varphi_0$ extends to a homomorphism $\varphi_1$ from $\mathscr{O}$ to $K'$.

We identify the algebra $\mathscr{O}[G]$ of the group G over $\mathscr{O}$ with a subring of the algebra K[G] and define a ring homomorphism Φ from $\mathscr{O}[G]$ to $K'[G]$ by the formula

(42) Φ $_g\sum_{\in G}a_gg=_g\sum_{\in G}\varphi_1(a_g)g$.

Denote by $\mathscr{C}$ the set of conjugacy classes of G. For C in $\mathscr{C}$, denote by $u_C$ the element $\sum_{g\in C}g$ of $\mathscr{O}[G]$; the family $(u_C)_{C\in\mathscr{C}}$ is a basis over $\mathscr{O}$ of the center $Z(\mathscr{O}[G])$ of the algebra $\mathscr{O}[G]$ (VIII, p. 398). For any element $\lambda$ of $\mathscr{S}_K$(G), denote by $\chi_{\lambda}$ its character, by $d_{\lambda}$ its dimension, and by $e_{\lambda}$ the element of K[G] defined by

$$
e_{\lambda}=|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})g \tag{43}
$$

The family $(e_{\lambda})$ is a basis over K of the center Z(K[G]) of the ring K[G] (VIII, p. 408). We have

$$
e_{\lambda}=_C\sum_{\in\mathscr{C}}\alpha_{\lambda ,C}u_C \tag{44}
$$

with

$$
\alpha_{\lambda ,C}=|G|^{-1}d_{\lambda}\chi_{\lambda}(C^{-1}) \tag{45}
$$

For $C\in \mathscr{C}$ and $\lambda \in \mathscr{S}_K$(G), set $\beta_{C,\lambda}=|G|d^-_{\lambda}^1d(C)^{-1}\chi_{\lambda}(C)$. The entries of the matrix $(\alpha_{\lambda ,C})$ are in $\mathscr{O}$, and it follows from formula (31) of VIII, p. 411 that its inverse matrix is the matrix $(\beta_{C,\lambda})$, whose entries are also in $\mathscr{O}$ by Proposition 9 of VIII, p. 415. Consequently, the family $(e_{\lambda})$ is a basis of the $\mathscr{O}$-module $Z(\mathscr{O}[G])$.

The elements $Φ(u_C) =\sum_{g\in C}g$ of $K'[G]$ form a basis over $K'$ of the center $Z(K'[G])$ of the ring $K'[G]$. We have

$$
Φ(e_{\lambda}) =_C\sum_{\in\mathscr{C}}\varphi_1(\alpha_{\lambda ,C}) Φ(u_C) \tag{46}
$$

and the matrix with entries $\varphi_1(\alpha_{\lambda ,C})$ is invertible. The family of the $Φ(e_{\lambda})$ is therefore a basis of $Z(K'[G])$. The family $(e_{\lambda})$ is a partition of the idempotent 1 in Z(K[G]) (VIII, p. 146 and p. 408); in other words, we have

$\sum_{\lambda}e_{\lambda}= 1,e^2_{\lambda}=e_{\lambda},e_{\lambda}e_µ= 0$ if $\lambda \not=µ$.

It follows that the family of the $Φ(e_{\lambda})$ is a partition of the idempotent 1 in $Z(K'[G])$; since this family is a basis of $Z(K'[G])$ over $K'$, its elements are the indecomposable idempotents in $Z(K'[G])$ (VIII, p. 148, Remark 4).

For $\lambda '$ in $\mathscr{S}_{K'}$(G), define $\chi_{\lambda'},d_{\lambda'}$, and $e_{\lambda'}$ as above. By VIII, p. 408, the elements $e_{\lambda'}$ are the indecomposable idempotents in $Z(K'[G])$. Hence there exists a bijection $\varphi_G$ from $\mathscr{S}_K(G)$ to $\mathscr{S}_{K'}(G)$ such that $Φ(e_{\lambda}) =e_{\varphi_G(\lambda)}$ for every $\lambda$ in $\mathscr{S}_K(G)$.

Let $\lambda$ in $\mathscr{S}_K(G)$; set $\lambda '=\varphi_G(\lambda )$. Let $(V_{\lambda}, \pi_{\lambda})$ (resp. $(V_{\lambda'}, \pi_{\lambda'}))$ be a linear representation of G whose associated K[G]-module (resp. $K'$[G]-module) has class $\lambda$ (resp. $\lambda ')$. Let us prove that $\lambda$ and $\lambda '$ are related. Let $g$ be an element of G. Let $\delta (T)$ be the determinant of the endomorphism $1 + T\pi_{\lambda}(g)$ of the K[T]-module $K[T]\otimes_KV_{\lambda}$. Let $\omega_1, . . . , \omega_{d_{\lambda}}$ be the eigenvalues of $\pi_{\lambda}(g)$; we have

$$
\delta (T) = (1 + T\omega_1)\cdots (1 + T\omega_{d_{\lambda}})
$$

We define $\delta '(T)$ likewise, and we denote the eigenvalues of $\pi_{\lambda'}(g)$ by $\omega '_1, . . . , \omega '_{d_{\lambda'}}$. The $\mathscr{O}$-module $\mathscr{O}[G]$ is free with basis G, and the K-vector space K[G] has basis G. Denote by ∆(T) the determinant of multiplication by $1 +e_{\lambda}gT$ in the $\mathscr{O}$[T]-module $\mathscr{O}[T]\otimes_{\mathscr{O}}\mathscr{O}[G]$. It is also the determinant of multiplication by $1 +e_{\lambda}gT$ in the K[T]-module $K[T]\otimes_KK[G]$. Let $\varphi_1$ be the homomorphism from $\mathscr{O}[T]$ to $K'[T]$ that extends $\varphi_1$ and sends T to T. Since G is a basis of the $K'$-vector space $K'[G]$, the polynomial $\varphi_1$(∆(T)) is equal to the determinant ∆$'(T)$ of multiplication by $1 +e_{\lambda'}gT$ in the $K'$-vector space $K'[G]$.

The algebra K[G] is the direct sum of its simple components $e_µK[G]$ for $µ$ running through $\mathscr{S}_K(G)$. For $µ$ different from $\lambda$, the element $e_{\lambda}g$ annihilates $e_µK[G]$. Moreover, multiplication by $e_{\lambda}g$ coincides with multiplication by $g$ in $e_{\lambda}K[G]$. In view of VIII, p. 409 and Example 6 of VIII, p. 400, the representation of G in $e_{\lambda}K[G]$ is the direct sum of $d_{\lambda}$ representations of class $\lambda$. We consequently have ∆(T) $=\delta (T)^{d_{\lambda}}$.

Analogously, we have ∆$'(T) =\delta '(T)^{d_{\lambda'}}$.

From the relation ∆$'(T) =\varphi_1$(∆(T)), we deduce first that $d^2_{\lambda}=d^2_{\lambda'}$, and therefore $d_{\lambda}=d_{\lambda'}$, and then that the sequence $\varphi (\omega_1), . . . , \varphi (\omega_{d_{\lambda}})$ can be deduced from the sequence $(\omega '_1, . . . , \omega '_{d'_{\lambda'}})$ by a permutation of the set of indices.

Since this is true for every element $g$ of G, the representations $\lambda$ and $\lambda '$ are related. We have therefore proved Proposition 10 when the field K has characteristic 0.

B) General case.

Let L be an algebraically closed field of characteristic 0 (for example, an algebraic closure of $\mathbf{Q})$. Denote by $\mathscr{S}_L(G)$ the set of classes of simple L[G]-modules. Choose an isomorphism $\eta$ from the group $µ_n(L)$ to the group $µ_n$(K), and set $\eta '=\varphi \circ \eta$. By part A) of the proof, there exist bijections

$$
\eta_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_K(G),\eta_G':\mathscr{S}_L(G)\rightarrow \mathscr{S}_{K'}(G)
$$

with the following property: for every $\lambda$ in $\mathscr{S}_L$(G), the representations $\lambda$ and $\eta_G(\lambda )$ are related through $\eta$, and the representations $\lambda$ and $\eta '_G(\lambda )$ are related through $\eta '$. The bijection $\varphi_G=\eta '_G\circ \eta_G^{-1}$ has the desired properties.

The bijection $\varphi_G$ from $\mathscr{S}_K(G)$ to $\mathscr{S}_{K'}(G)$ extends to an isomorphism, also denoted by $\varphi_G$, from the Grothendieck group $R_K(G)$ to the group $R_{K'}(G)$.

#### Remark 1 {#alg-viii-s21-n12-rem-1 .statement}

Suppose that $K'$ is an extension of K and that the isomorphism $\varphi$ is the mapping $\xi \mapsto \xi \cdot 1$; then the mapping $\varphi_G$ is given by extension of scalars from K to $K'$.

#### Corollary 1 {#alg-viii-s21-prop-10-cor-1 .statement}

The mapping $\varphi_G$ is a ring isomorphism from $R_K(G)$ to $R_{K'}(G)$. For every finite-dimensional representation $\pi$ of G in a K-vector space, we have $\varphi_G([\pi ]) = [\pi ']$, where $\pi '$ is a representation related to $\pi$ through $\varphi$.

This follows from the semisimplicity of the representations of G and property b) of VIII, p. 416.

#### Corollary 2 {#alg-viii-s21-prop-10-cor-2 .statement}

The dimension of each simple representation of G divides the order of G.

This follows from Proposition 10 and Proposition 9 of VIII, p. 415.

#### Remark 2 {#alg-viii-s21-n12-rem-2 .statement}

Suppose that the group G is abelian. We saw in the remark of VIII, p. 414 that $\mathscr{S}_K(G)$ can be identified with the set Hom(G$, µ_n(K))$. Likewise, $\mathscr{S}_{K'}(G)$ can be identified with Hom(G$, µ_n(K'))$. With these identifications, the bijection $\varphi_G$ is simply the mapping $\chi \mapsto \varphi \circ \chi$.

#### Remark 3 {#alg-viii-s21-n12-rem-3 .statement}

Let $\pi_1$ and $\pi_2$ be linear representations of G in finite-dimensional vector spaces over K. For $i= 1,2$, let $\pi_i'$ be a representation related to $\pi_i$ through $\varphi$. We have

(47) dim$_K$ Hom$_K(\pi_1, \pi_2) =$ dim$_{K'}$ Hom$_{K'}(\pi '_1, \pi_2')$.

The proof follows that of Corollary VIII, p. 410, by reducing to the case when the $\pi_i$ (and therefore the $\pi_i')$ are simple.

#### Remark 4 {#alg-viii-s21-n12-rem-4 .statement}

Let H be a subgroup of G of cardinal $m$. The isomorphism $\varphi$ restricts to an isomorphism from $µ_m(K)$ to $µ_m(K')$ and, consequently, a ring isomorphism $\varphi_H$ from $R_K(H)$ to $R_{K'}(H)$. The following diagrams commute:

$R_K(G)^{Res^G_H}$ // $R_K(H)R_K(H)^{Ind^G_H}$ // $R_K(G)$

$\varphi_G\varphi_H\varphi_H\varphi_G$

$R_{K'}(G)^{Res^G_H}/$/ $R_{K'}(H),R_{K'}(H)^{Ind^G_H}/$/ $R_{K'}(G)$. The commutativity of the first diagram is obvious, and that of the second follows from it using Frobenius reciprocity and formula (47).

#### Remark 5 {#alg-viii-s21-n12-rem-5 .statement}

Suppose that G is the product $G'\times G''$ of two finite groups. We define isomorphisms $\varphi_{G'}$ and $\varphi_{G''}$ as in the previous example.

We have a commutative diagram

$R_K(G_')\otimes_{\mathbf{Z}}R_K(G_{''})^{\kappa}$ // $R_K(G)$

$\varphi_{G'}\otimes \varphi_{G''}\varphi_G$

$R_{K'}(G_')\otimes_{\mathbf{Z}}R_{K'}(G_{''})^{\kappa'}$ // $R_{K'}(G)$,

where the isomorphisms $\kappa$ and $\kappa '$ are those defined in VIII, p. 406.

### \*13. Complex Linear Representations

In this subsection, we assume that K is the field $\mathbf{C}$ of complex numbers.

Let $(M, \pi )$ be a linear representation of G. We say that a Hermitian form Φ on M is invariant under G if we have

$$
Φ(\pi (g)x, \pi (g)x') = Φ(x, x') \tag{48}
$$

for all $x, x'\in M$ and every $g\in G$. This also means that for every $g\in G$, the automorphism $\pi (g)$ of M is unitary with respect to Φ.

#### Proposition 11 {#alg-viii-s21-prop-11 .statement}

Let $(M, \pi )$ be a finite-dimensional linear representation of G.

a) There exists on M a Hermitian form that is positive, separating, and invariant under G.

b) Suppose that the representation $\pi$ is simple. If Φ and Ψ are nonzero Hermitian forms on M that are invariant under G, then there exists a real number $a$ such that $Ψ =aΦ$.

Choose a separating positive Hermitian form on the vector space M, and denote it by $Φ_0$. We define a separating positive Hermitian form Φ that is invariant under G by setting

$$
Φ(x, x') =_g\sum_{\in G}Φ_0(\pi (g)x, \pi (g)x') \tag{49}
$$

for $x, x'\in M$.

Let Ψ be a Hermitian form on M; there exists a unique endomorphism A of M such that $Ψ(x, x') = Φ(x,Ax')$ for $x, x'$ in M. If, moreover, Ψ is invariant under G, then the endomorphism A commutes with the automorphism $\pi (g)$ for $g\in G$. If the representation $\pi$ is simple, then by Schur’s lemma (VIII, p. 47, Theorem 1), A is a homothety and there consequently exists a complex number $a$ such that $Ψ =aΦ$. Since Φ and Ψ are Hermitian and Φ is nonzero, $a$ is a real number. The proposition follows.

We endow the vector space $\mathbf{C}[G]$ of complex functions on G with the Hilbert space structure whose inner product is given by

$$
\langle f|f'\rangle_G=|G|^{-1}_g\sum_{\in G}f(g)f'(g) \tag{50}
$$

For any function $f\in \mathbf{C}[G]$, we denote by $f^*$ the function defined by

$$
f^*(g) =f(g^{-1}) \tag{51}
$$

for $g\in G$; the mapping $f\mapsto f^*$ is a semilinear involution of $\mathbf{C}[G]$. We also have

$$
\langle f|f'\rangle_G=\langle f^*, f'\rangle_G \tag{52}
$$

for $f, f'\in \mathbf{C}[G]$, with the notation of formula (28) of VIII, p. 410. We therefore have

$$
\langle f|f'\rangle_G=|G|^{-2}\tau (f^*f') \tag{53}
$$

Let $(M, \pi )$ be a finite-dimensional linear representation of G. We endow the vector space M with the structure of a Hilbert space for which the endomorphisms $\pi (g)$ are unitary (Proposition 11). If we denote by $A^*$ the adjoint of a endomorphism A of M for this structure, then we have Tr(A$^*) =$ Tr(A). For every $g\in G$, we have $\pi (g^{-1}) =\pi (g)^*$, and therefore $\chi_{\pi}(g^{-1}) =\chi_{\pi}(g)$; in other words, we have $\chi_{\pi}=\chi^*_{\pi}$. The orthogonality relation for characters (VIII, p. 410, Proposition 4) then has the form

$$
\langle \chi_{\lambda}|\chi_µ\rangle_G=\delta_{\lambda µ} \tag{54}
$$

for $\lambda , µ\in \widehat{G}$. It expresses the fact that the family of the characters $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ of the simple representations of G is an orthonormal basis of the Hilbert space $Z(\mathbf{C}[G])$ of central functions.

Let $\pi$ and $\pi '$ be finite-dimensional linear representations of G. We have the relation $\langle \chi_{\pi}|\chi_{\pi'}\rangle_G=$ dim$_{\mathbf{C}}$ Hom$_G(\pi , \pi ')$ (VIII, p. 410, Corollary). The representation $\pi$ is irreducible if and only if $\langle \chi_{\pi}|\chi_{\pi}\rangle_G= 1$.

For every element $\lambda$ of $\widehat{G}$, we endow the vector space $V_{\lambda}$ with the structure of a Hilbert space for which the automorphisms $\pi_{\lambda}(g)$ are unitary. We denote by $\langle v|v'\rangle_{\lambda}$ the inner product of two elements $v, v'$ of $V_{\lambda}$ and by $u^*$ the adjoint of an endomorphism $u$ of $V_{\lambda}$. Let $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ and $A'= (A'_{\lambda})_{\lambda\in\widehat{G}}$ be elements of $F(\widehat{G})$. We write $A^*= (A^*_{\lambda})_{\lambda\in\widehat{G}}$. We have $\mathscr{F}(a^*) = (\mathscr{F}(a))^*$ for every element $a$ of $\mathbf{C}[G]$. Set (55) $\langle A|A'\rangle_{\widehat{G}}=|G|^{-2}\widehat{\tau}(A^*A')$. By formula (10) of VIII, p. 407, we have

$_'$ 1 $\sum_{*'}$ (56) $\langle A|A\rangle$ = $d_{\lambda}$ Tr(A$_{\lambda}A_{\lambda})$.

$$
^{\widehat{G}}|G|^2
$$

Since ˆ$\tau \circ \mathscr{F}=\tau$, formulas (53) and $^{\lambda\in}(55^{\widehat{G}})$ imply that the mapping $\mathscr{F}$ is an isomorphism of Hilbert spaces from $\mathbf{C}[G]$ to $F(\widehat{G})$.

The Schur orthogonality relations (VIII, p. 410) can be reformulated using Hilbertian inner products. Relations (21) and (24) then give the following assertions. For $\lambda \in \widehat{G}$ and $x, x', y, y'$ in $V_{\lambda}$, we have (57) $|G|^{-1}_g\sum_{\in G}\langle x|\pi_{\lambda}(g)x'\rangle_{\lambda}\langle y|\pi_{\lambda}(g)y'\rangle_{\lambda}=d^-_{\lambda}^1\langle x|y\rangle_{\lambda}\langle x'|y'\rangle_{\lambda}$.

If $\lambda$ and $µ$ are two distinct elements of $\widehat{G}$, then for $x, x'$ in $V_{\lambda}$ and $y, y'$ in $V_µ$, we have (58) $\sum\langle x|\pi_{\lambda}(g)x'\rangle_{\lambda}\langle y|\pi_µ(g)y'\rangle_µ= 0$.

For every $\lambda \in \widehat{G}$, we choose an orthonormal basis $(^{g\in G}e_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ of $V_{\lambda}$. For any $g\in G$, we denote by $(\pi^{\lambda}_{ij}(g))$ the matrix of the endomorphism $\pi_{\lambda}(g)$ of $V_{\lambda}$ with respect to this basis; we have (59) $\pi^{\lambda}_{ij}(g) =\langle e_{\lambda ,i}|\pi_{\lambda}(g)e_{\lambda ,j}\rangle_{\lambda}$.

Since the endomorphism $\pi_{\lambda}(g)$ is unitary, its inverse is equal to $\pi_{\lambda}(g)^*$, so that (60) $\pi^{\lambda}_{ij}(g) =\pi_{ji}^{\lambda}(g^{-1})$. It then follows from formulas (22) of VIII, p. 409 and (25), p. 409 that the functions $(d_{\lambda})^{1/2}\pi_{ij}^{\lambda}$, for $\lambda \in \widehat{G},1\leqslant i\leqslant d_{\lambda},1\leqslant j\leqslant d_{\lambda}$, form an orthonormal basis of the Hilbert space $\mathbf{C}[G].*$

### Exercises {#alg-viii-s21-exercises}

1) Let A be a commutative ring, G a group, and H a subgroup of G of finite index. Suppose that the element $(G : H)1_A$ of A is invertible. Let M be an A[G]-module and N an A[G]-submodule of M. Prove that if N admits a supplementary A[H]submodule in M, then it admits a supplementary A[G]-submodule in M (adapt the proof of Theorem 1 of VIII, p. 401). Deduce that an A[G]-module that is projective as an A[H]-module is projective.

2) Let A be a commutative ring and G a group. a) Suppose that the algebra A[G] of the group G is an absolutely flat ring (VIII, p. 171, Exercise 27). Prove that the ring A is absolutely flat. Let H be a subgroup of G that admits a finite generating subset; prove that the left ideal $I_H$ of A[G] (VIII, p. 22, Exercise 25) admits a supplementary in A[G], and deduce that H is finite (observe that in the opposite case, the annihilator of $I_H$ would be reduced to (0)). b) Keep the assumption of a). Let $g$ be an element of G of finite order $n$. Prove that $n1_A$ is invertible in A (let $x$ be an element of A such that $(1-e_g)x(1-e_g) = (1-e_g)$; construct an element $y$ of A such that $1-(1-e_g)x=y(1 +e_g+\cdots +e_{g^{n-1}}))$. Deduce that the order of every finite subgroup of G is invertible in A. c) Suppose that A is an absolutely flat ring and that every finite subset of G generates a finite subgroup with cardinal invertible in A. Prove that the ring A[G] is absolutely flat (reduce to the case when G is finite, and use Exercise 1).

3) Let A be a commutative ring and G a group. a) Suppose that the algebra A[G] of the group G is semisimple. Prove that A is semisimple, that G is finite, and that its order is invertible in A (use Exercise 2 and Exercise 25 of VIII, p. 22). b) Suppose that the algebra A[G] is isomorphic to the product of a finite family of fields. Prove that every subgroup of G is normal (use a), and observe that every idempotent in A[G] is central).

In Exercises 4 through 26 below, G is a finite group, and K is an algebraically closed field; we assume that the order of G is invertible in K.

4) Let $(M, \pi )$ be a faithful[^2] finite-dimensional representation of G and $(N, \rho )$ an irreducible representation; suppose that the character $\chi_{\pi}$ has exactly $s$ distinct values. Prove that there exists an integer $n < s$ such that the K[G]-module N is isomorphic to a submodule of $M^{\otimes n}$ (calculate $\langle \chi_{\rho}, \chi^n_{\pi}\rangle$, observing that the equality $\chi_{\pi}(g) =$ dim M is equivalent to $g= 1)$.

5) Let $(M, \pi )$ be a representation of G. a) Let H be a subgroup of G, S a system of representatives in G of the left cosets (mod H), and N a linear subspace of M stable under H. The representation of G in M is isomorphic to the representation induced by that of H in N if and only if we have $M =\bigoplus_{s\in S}sN$. b) Suppose that M is the direct sum of a family $(M_i)_{i\in I}$ of subspaces and that there exists a transitive action of G on I such that $\pi (g)(M_i)\subset M_{gi}$ for $g\in G,i\in I$. Let $o\in I$, and let $G_o$ be its stabilizer in G. Prove that $\pi$ is isomorphic to the representation induced by the representation of $G_o$ in $M_o$. If $\pi$ is irreducible, then the condition that the action of G on I is transitive is automatically satisfied.

6) Let X be a finite set on which G acts. We consider the representation $\pi$ of G in $K^X$ such that $\pi (g)e_x=e_{gx}$ for $g\in G,x\in X$ (“permutation representation” associated with X). a) For $g\in G$, prove that $\chi_{\pi}(g)$ is equal to the number of points of X fixed by $g$. b) Prove that the multiplicity of the unit representation in $\pi$ is equal to the number of orbits of G in X. c) Assume from now on that the action of G is transitive; fix a point $x$ of X, and denote its stabilizer by H. Prove that $\pi$ is isomorphic to the representation induced by the unit representation of H and that $\langle \chi_{\pi}, \chi_{\pi}\rangle$ is equal to the number of orbits of H in X. d) Let V be the subspace of $K^X$ consisting of the vectors for which the sum of the coordinates is zero; it is stable under G, and we denote by $\pi_X$ the representation of G in V deduced from $\pi$. Prove that $\pi_X$ is irreducible if and only if the action of G is doubly transitive (I, §5, p. 143, Exercise 14).

7) For any representation V of G of finite dimension, we denote by $\varphi (V)$ the dimension of the subspace of V fixed by G; we extend $\varphi$ by linearity to a $\mathbf{Z}$-linear form on $R_K(G)$. Let $(V_{\lambda})_{\lambda\in\widehat{G}}$ be the family of irreducible representations of G, and let $\omega$ be the element $\sum_{\lambda\in Gˆ}[V_{\lambda}] [V_{\lambda}^*]$ of $R_K(G)$. Prove the formula $\varphi (\omega^n) =\sum_Cd(C)^{n-1}$ for every integer $n\geqslant 0$ (apply Proposition 8 of VIII, p. 415 and the second orthogonality relation for characters).

8) Let H and F be subgroups of G, and let S be a subset of G such that G is the disjoint union of the double classes $FsH$. Let $(N, \sigma )$ be a representation of H. For $s\in G$, set $H_s= F\cap sHs^{-1}$, and denote by $\sigma_s$ the representation of $H_s$ in N defined by $\sigma_s(x) =\sigma (s^{-1}xs)$. a) Prove that the representation Res$^G_F$(Ind$^G_H(\sigma ))$ is isomorphic to the direct sum of the representations Ind$^F_{H_s}(\sigma_s)$ for $s\in S$. (Denote the representation Ind$^G_H(\sigma )$ by $(M, \pi )$. The space M can be identified with the direct sum of the $\pi (x)N$ for $x\in G/H$. For $s\in S$, let $M(s)$ be the subspace of M generated by the $\pi (x)N$ with $x\in FsH$. Observe that $M(s)$ is the direct sum of the subspaces $\pi (xs)N$ for $x\in F/H_s$, and deduce from Exercise 5, b) that as a K[F]-module, $M(s)$ is isomorphic to Ind$^F_{H_s}(\sigma_s).)$ b) Take F = H (so that we have $H_s= H\cap sHs^{-1})$. Prove that the representation Ind$^G_H(\sigma )$ is irreducible if and only if $\sigma$ is irreducible and for every $s\in G$ H, the supports (VIII, p. 66) of the representations $\sigma_s$ and Res$^H_{H_s}(\sigma )$ are disjoint (“Mackey’s criterion”: apply a) and Frobenius reciprocity). c) Assume that H is normal; then Ind$^G_H(\sigma )$ is irreducible if and only if $\sigma$ is irreducible and is not isomorphic to any of its conjugates $\sigma \circ$ int($g)$ for $g\in G$ H.

9) Let $(M, \pi )$ be an irreducible representation of G and H a normal subgroup of G. a) Let $M =\bigoplus_{i\in I}M_i$ be the decomposition of the K[H]-module M as a direct sum of isotypical submodules. Prove that the action of G on M permutes the submodules $M_i$ transitively. Deduce that $(M, \pi )$ is isomorphic to the representation induced by a subgroup of G containing H (apply Exercise 5, b)). b) Let $\mathscr{S}$ be the support of the K[H]-module M; there exists an integer $e$ such that M is K[H]-isomorphic to $\sum_{\lambda\in\mathscr{S}}\lambda^e$.

10) Let $(M, \pi )$ be an irreducible representation of G and H a normal subgroup of G. a) Suppose that H is equal to the center of G. Prove that the degree of $\pi$ divides the index of H in G. (For $m\geqslant 1$, let $H_m$ be the subgroup of $H^m$ consisting of the elements $(h_1, . . . , h_m)$ such that $h_1. . . h_m= 1$. Observe that the representation $\pi^{\times m}: G^m\rightarrow$ End$_K(M^{\otimes m})$ defines an irreducible representation of $G^m/H_m$, and apply Corollary 2 of Proposition 10 (VIII, p. 420) to it.) b) Suppose that H is commutative. Prove that the degree of $\pi$ divides (G : H). (Using Exercise 9, a), and reasoning by induction on the cardinal of G, reduce to the case when the restriction of $\pi$ to H is isotypical. Prove that $\pi (H)$ is central in $\pi$(G), and apply a).)

11) Let A and H be subgroups of G. Suppose that A is commutative and normal and that G is the semidirect product of H and A. The group H acts on $\widehat{A} =$ Hom(A$,K^*)$; choose a system of representatives $(\alpha_i)_{i\in\widehat{A}/H}$ of the orbits of H in $\widehat{A}$. For $i\in \widehat{A}/H$, let $H_i$ be the stabilizer of $\alpha_i$ in H, and let $G_i=$ AH$_i$. For every irreducible representation $\sigma$ of $H_i$, define a representation $\rho_{i,\sigma}$ of $G_i$ by setting $\rho_{i,\sigma}(ah) =$ $\alpha_i(a)\sigma (h)$ for $a\in A$ and $h\in H$. Prove that the representations Ind$^G_{G_i}(\rho_{i,\sigma})$, for $i\in \widehat{A}/H$ and $\sigma \in \widehat{H}_i$, are irreducible and pairwise nonisomorphic, and that we obtain all irreducible representations of G this way (apply Exercise 9).

$\P 12)$ Let H be a subgroup of G; suppose that for every $g\in G$ H, we have the equality $H\cap gHg^{-1}=\{1\}$. a) Let $u$ be a central function on H. Prove that the function Ind$^G_H(u)$ coincides with $u$ on H $\{1\}$. If $v$ is another central function on H such that $v(1) = 0$, then we have $\langle$Ind$^G_H(u)$, Ind$^G_H(v)\rangle_G=\langle u, v\rangle_H$. b) Let $\lambda \in \widehat{H}$; we denote by $\chi '_{\lambda}$ the function $\chi_{\lambda}-d_{\lambda}$ on H and by $\theta_{\lambda}$ the function $d_{\lambda}+$ Ind$^G_H(\chi '_{\lambda})$ on G. Prove that $\theta_{\lambda}$ is the character of an irreducible representation of G of degree $d_{\lambda}$ whose restriction to H is isomorphic to $\lambda$ (use a) to calculate $\langle \theta_{\lambda}, \theta_{\lambda}\rangle ,\langle \theta_{\lambda},1\rangle$, and $\langle$Res$^G_H(\theta_{\lambda}), \chi_{\lambda}\rangle )$. c) Set $\theta =\sum_{\lambda}d_{\lambda}\theta_{\lambda}$. Prove that we have $\theta (h) = 0$ if $h\in H\{1\}$ and $\theta (g) =$ $\theta (1) =$ Card(H) if $g$ does not belong to any conjugates of H. d) Let $L'$ be the set of elements of G that do not belong to any conjugates of H, and set $L = L'\cup  \{1\}$. Prove that L is a normal subgroup of G (deduce from c) that L is the kernel of a representation with character $\theta )$. e) Prove that G is the semidirect product of H and L (calculate the order of L). f ) Let $h\in H\{1\}$. Prove that the automorphism int($h)$ restricted to L has no fixed point other than 1. Deduce that the order of H divides Card(L) $-1$. g) Prove that if the subgroup H has even order, then L is commutative (apply Exercise 23, d) of I, §6, p. 145).

13) Let $\mathscr{H}$ be a set of subgroups of G. a) Prove that the following properties are equivalent:

(i) The union of the conjugates of the subgroups belonging to $\mathscr{H}$ is equal to G.

(ii) Every character of G is a linear combination with rational coefficients of characters induced by the characters of subgroups belonging to $\mathscr{H}$. (Deduce from Proposition 6 of VIII, p. 412 that property (ii) is equivalent to the injectivity of the restriction homomorphism $\mathscr{Z}_K(G)\rightarrow \bigoplus_{H\in\mathscr{H}}\mathscr{Z}_K(H).)$ b) Let $\mathscr{C}$ be the set of cyclic subgroups of G; it obviously has property (i). For every cyclic subgroup C of G, we denote by $\varphi_C$ the function on C with value Card(C) on the generators of C and 0 on the other elements. Prove the equality Card(G) $=\sum_{C\in\mathscr{C}}$ Ind$^G_C(\varphi_C)$. c) Let $C\in \mathscr{C}$. Prove that the function $\varphi_C$ belongs to the subgroup $R_K(G)$ of $\mathscr{Z}_K(G)$ generated by the characters (reason by induction on the order of C, using b)). d) Let $\chi$ be the character of an irreducible representation G. Prove the equality $\chi =$ Card(G)$^{-1}\sum_{C\in\mathscr{C}}$ Ind$^G_C(\varphi_C$ Res$^G_C(\chi ))$, which gives an explicit formula for property (ii) of a).

14) A representation of G is called monomial if it is the direct sum of representations induced by degree 1 representations of subgroups of G. a) Suppose that the representations of the proper subgroups of G are monomial and that G contains a noncentral commutative normal subgroup H. Prove that every faithful irreducible representation of G is monomial (observe that the restriction to H of such a representation is not isotypical, and apply Exercise 9, a)). b) Deduce that all representations of supersolvable groups (I, §6, p. 146, Exercise 26), and in particular of nilpotent groups, are monomial. c) Take G to be the group $\mathbf{S}\mathbf{L}(2,\mathbf{F}_3)$. Its center Z has order 2, and the group $G/Z$ is isomorphic to the alternating group $\mathfrak{A}_4$ (II, §10, p. 422, Exercise 14, g)); in particular, G is solvable. Prove that its derived group has index 3 (cf. I, §5, p. 142, Exercise 10). Using formula (8) of VIII, p. 407, deduce that G admits an irreducible representation of degree 2, and prove that this representation is not monomial.

$\P 15)$ Suppose that all representations of G are monomial; let us prove that G is solvable. Reasoning by induction on the order of G, we may assume that every quotient group of G different from G is solvable. a) If G contains two distinct minimal nontrivial normal subgroups $H_1$ and $H_2$, then it is solvable (consider the canonical homomorphism from G to $G/H_1\times G/H_2)$.

Assume from now on that G admits a unique minimal nontrivial normal subgroup H. b) Prove that a representation of G is faithful if its restriction to H is nontrivial. c) Let $\pi$ be a faithful representation of minimal degree; there exist subgroups $H_i$ of G and representations $\sigma_i$ of $H_i$ of degree 1 such that $\pi$ is isomorphic to $\bigoplus$ Ind$^G_{H_i}(\sigma_i)$. Let $\pi_0=\bigoplus$ Ind$^G_{H_i}(\varepsilon_{H_i})$, where $\varepsilon_{H_i}$ denotes the unit representation. Prove that the kernel of $\pi_0$ is commutative and nontrivial (observe that $\pi_0$ is irreducible); deduce that G is solvable.

16) Suppose that the characteristic of K is zero. We say that an element $x$ of K is integral over $\mathbf{Z}$ if it belongs to a subring of K that is a finitely generated $\mathbf{Z}$-module or, equivalently, if the subring $\mathbf{Z}[x]$ of K is a finitely generated $\mathbf{Z}$-module $*$(cf.

Comm. Alg., V, §1, No. 1, p. $303)*$. a) Prove that the set of elements of K integral over $\mathbf{Z}$ is a subring of K (for $x, y$ integral over $\mathbf{Z}$, consider the subring $\mathbf{Z}[x, y])$. b) An element $x$ of K is integral over$\mathbf{Z}$ if and only if it is a root of a monic polynomial in $\mathbf{Z}[X]$ (when $x$ is integral, adapt the proof of Lemma 1 of VIII, p. 81 to show that it satisfies an equation of the form det($xI_m-A$) = 0 with $A\in \mathbf{M}_m(\mathbf{Z}))$. c) If $x$ is integral over $\mathbf{Z}$, then the same holds for its conjugates $x_1, . . . , x_m$ over $\mathbf{Q}$; the element $x_1\cdots x_m$ belongs to $\mathbf{Z}$ (use the lemma of VIII, p. 416).

17) Let C be a conjugacy class of G and $\pi$ an irreducible representation of G of degree $d$. a) Prove that the element $d^{-1}$ Card(C) $\chi (C)$ of K is integral over $\mathbf{Z}$ (reason as in the proof of Proposition 9 of VIII, p. 415). b) Suppose that $d$ and Card(C) are mutually prime integers. Prove that the element $d^{-1}\chi (C)$ is integral over $\mathbf{Z}$. $*$c) Suppose, moreover, $K =\mathbf{C}$. Prove that all conjugates of $d_{-1}\chi (C)$ over $\mathbf{Q}$ have absolute value $\leqslant 1$. Deduce from Exercise 16, c) that $|\chi (C)|$ is zero or equal to $d$. Conclude that if $\chi (C)$ is not zero, then $\pi (x)$ is a homothety for every $x\in C$. In particular, if $\pi$ is faithful and C is not reduced to one element, then we have $\chi (C) = 0.*$

18) Suppose that the group G is simple but not cyclic. a) Prove that there is no conjugacy class different from $\{1\}$ whose cardinal is a power of a prime number. (Let C be a class of cardinal $p^r$ with $r\geqslant 1$. Deduce from Exercise 17, b) that $p^{-1}\chi_{\lambda}(1)\chi_{\lambda}(C)$ is integral over $\mathbf{Z}$ when $\lambda$ is different from the unit representation, and deduce a contradiction using the second orthogonality relation for characters). b) Prove that the order of G is divisible by at least three distinct prime numbers (apply a) to the conjugacy class of a central element $x\not= 1$ in a Sylow subgroup of G). c) Prove that a finite group whose order is divisible by at most two distinct prime numbers is solvable (“Burnside’s theorem”: reason by induction on the cardinal of the group, using b)).

$*19)$ Let $\pi$ be an irreducible complex representation of G of degree $>1$. Prove that there exists an element $x$ of G such that $\chi_{\pi}(x) = 0$. (Let $\{\lambda_1, . . . , \lambda_s\}$ be the orbit of $\pi$ in $\widehat{G}$ for the action of the group Gal($\mathbf{C}/\mathbf{Q})$, and let $\chi_1, . . . , \chi_s$ be the corresponding characters. Let $g\in G$; if $\chi (g)\not= 0$, then prove as in Exercise 17, c) that we have $|\chi_1(g). . . \chi_s(g)|\geqslant 1$, and therefore $\sum_i|\chi_i(g)|^2\geqslant s($FRV, III, §1, No. 1, p. 93, Proposition 2). If this holds for every $g\in G$, then deduce from the orthogonality relation for characters that we have equality, which leads to a contradiction by taking $g= 1.)*$

20) Let G be a finite group, H a subgroup of $G,\sigma$ a finite-dimensional representation of H, and $\rho$ the representation of G induced by $\sigma$. Let C be a conjugacy class of G; the set $C\cap H$ is the disjoint union of a finite family $(D_i)_{i\in I}$ of conjugacy classes of H. a) Prove the formula $\chi_{\rho}(C) =_{Card(C)}^{(G:H)}\sum_{i\in I}$ Card(D$_i)\chi_{\sigma}(D_i)$. b) If $\sigma$ is the trivial representation, then $\chi_{\rho}(C)=(G : H)$ Card(C)$^{-1}$Card(C $\cap H)$ holds.

$\P 21)$ Let $n\in \mathbf{N}$. Denote by $\mathscr{D}_n$ the subset of $\mathbf{N}^n$ consisting of the elements $(p_1, . . . , p_n)$ such that $p_1\geqslant \cdots \geqslant p_n$; endow it with the lexicographical order. For $\mathbf{p}\in \mathscr{D}_n$, denote by $\mathbf{p}'$ the element of $\mathscr{D}_n$ defined by $p'_i=p_i+n-i$. Let $\mathbf{X}= (X_1, . . . ,X_n)$ be a sequence of variables; set ∆($\mathbf{X}) =\prod_{i<j}(X_i-X_j)$. a) Let $P\in \mathbf{Z}[\mathbf{X}]$ be an antisymmetric polynomial, that is, a polynomial satisfying the relation $P(X_{\sigma}$[^1]$, . . . ,X_{\sigma(n)}) =\varepsilon (\sigma )P(X_1, . . . ,X_n)$ for every element $\sigma \in \mathfrak{S}_n$. Prove that there exists a symmetric polynomial $Q\in \mathbf{Z}[\mathbf{X}]$ such that P = ∆Q. b) For every $\mathbf{p}\in \mathscr{D}_n$, set $S_{\mathbf{p}}(\mathbf{X}) =$ ∆($\mathbf{X})^{-1}$ det(X$^p_{j'^i})_{1\leqslant i,j\leqslant n}$. Prove that $S_{\mathbf{p}}$ is a homogeneous symmetric polynomial of degree $\sum p_i$ with integer coefficients. c) If $\mathbf{q}= (q_i)_{1\leqslant i\leqslant n}$ is an element of $\mathscr{D}_n$ and P is an element of $\mathbf{Q}[\mathbf{X}]$, then we denote by $[P]_{\mathbf{q}}$ the coefficient of $\mathbf{x}^{\mathbf{q}}$ in P. Set $K_{\mathbf{p}\mathbf{q}}= [S_{\mathbf{p}}]_{\mathbf{q}}$. Prove that we have $K_{\mathbf{p}\mathbf{p}}= 1$ and $K_{\mathbf{p}\mathbf{q}}= 0$ for $\mathbf{q}>\mathbf{p}$ (expand the equality det(X$_j^{p'_i}) = S_{\mathbf{p}}(\mathbf{X})$ ∆($\mathbf{X})$ in the lexicographical order). Deduce that the polynomials $S_{\mathbf{p}}$ for $\mathbf{p}\in \mathscr{D}_n$ form a basis of the $\mathbf{Z}$-submodule of $\mathbf{Z}[\mathbf{X}]$ consisting of the symmetric polynomials. d) Let $\mathbf{Y}= (Y_1, . . . ,Y_n)$ be a sequence of variables. Prove the equality of formal power series

$$
_{1\leqslant}\prod_{i,j\leqslant n}(1-X_iY_j)^{-1}=_{\mathbf{p}}\sum_{\in\mathscr{D}_n}S_{\mathbf{p}}(\mathbf{X}) S_{\mathbf{p}}(\mathbf{Y})
$$

(use the equality det $(1-X_iY_j)^{-1}_{1\leqslant i,j\leqslant n}=$ ∆($\mathbf{X})$ ∆($\mathbf{Y})\prod_{1\leqslant i,j\leqslant n}(1-X_iY_j)^{-1}$ (cf. III, §8, p. 639, Exercise 5) by calculating the left-hand side using the expansion of $(1-T)^{-1}$ as a formal power series). e) Let $P\in \mathbf{Q}[\mathbf{X}]$ be a symmetric polynomial. For every $\mathbf{p}\in \mathscr{D}_n$, set $\omega_{\mathbf{p}}(P) =$ [P∆]$_{\mathbf{p}'}$. Prove the equality $\omega_{\mathbf{p}}(S_{\mathbf{q}}) =\delta_{\mathbf{p}\mathbf{q}}$. Deduce that for every $\mathbf{q}\in \mathscr{D}_n$, we have $[P]_{\mathbf{q}}=\sum_{\mathbf{p}\in\mathscr{D}_n}K_{\mathbf{p}\mathbf{q}}\omega_{\mathbf{p}}(P)$. f ) For $\boldsymbol{\alpha }\in \mathbf{N}^n$, set $f^{\boldsymbol{\alpha }}(\mathbf{X}) =\prod^n_{j=1}(\sum_iX^j_i)^{\alpha_j}$ and $c_{\boldsymbol{\alpha }}=\prod^n_{j=1j^{\alpha j}}^1_{\alpha_j!}$. Prove that we have $\sum_{\boldsymbol{\alpha }\in\mathbf{N}^n}c_{\boldsymbol{\alpha }}\omega_{\mathbf{p}}(f^{\boldsymbol{\alpha }})\omega_{\mathbf{q}}(f^{\boldsymbol{\alpha }}) =\delta_{\mathbf{p}\mathbf{q}}$ for $\mathbf{p},\mathbf{q}$ in $\mathscr{D}_n$ (observe that we have

$$
\prod_{-1}\prod^{\infty}1\sum_k\sum_k\sum_{\boldsymbol{\alpha }\boldsymbol{\alpha }}
$$

$(1-X_iY_j)$ = exp ( $X_i)(Y_j)$ = $c_{\boldsymbol{\alpha }}f(\mathbf{X})f(\mathbf{Y})$.

$$
kn
$$

$1\leqslant i,j\leqslant nk=0ij\boldsymbol{\alpha }\in \mathbf{N}$

$\P 22)$ Let $n$ be a natural number. Denote by $\mathscr{S}_n$ the set of decreasing finite sequences of strictly positive integers with sum $n$. Let $\mathbf{p}= (p_i)_{1\leqslant i\leqslant d}$ be an element of $\mathscr{S}_n$. For $1\leqslant i\leqslant d$, denote by $P_i$ the set of integers $r$ such that $p_1+\cdots +p_{i-1}< r\leqslant p_1+\cdots +p_i$, and for $1\leqslant j\leqslant p_1$, denote by $P'_j$ the set of integers of the form $p_1+\cdots +p_{i-1}+j$ with $1\leqslant i\leqslant d$ and $p_i\geqslant j$. The subsets $P_i$, on the one hand, and the subsets $P'_j$, on the other, form a partition of the interval $[1, n]$ in $\mathbf{N}$.

(We often represent this situation by a diagram, called a Young diagram: in the example below, we have $n= 9$ and $\mathbf{p}= (4,2,2,1)$. The set $P_i$ consists of the elements of the $i$-th row, and $P'_j$ of those of the $j$-th column.)

1 2 3 4

5 6

7 8

9

Let $\mathscr{P}$ (resp. $\mathscr{P}')$ be the subgroup of $\mathfrak{S}_n$ consisting of the permutations $\sigma$ such that $\sigma (P_i)\subset P_i$ for every $i$ (resp. $\sigma (P'_j)\subset P'_j$ for every $j)$. a) Prove that we have $\mathscr{P}\cap \mathscr{P}'=\{1\}$. b) Let $\sigma \in \mathfrak{S}_n$. Show that if Card(P$_i\cap \sigma (P'_j))\leqslant 1$ for every $i$ and $j$, then $\sigma$ belongs to $\mathscr{P}\mathscr{P}'$. Deduce that if $\sigma  /\in \mathscr{P}\mathscr{P}'$, then the subgroup $\mathscr{P}\cap \sigma \mathscr{P}'\sigma^{-1}$ contains a transposition. c) In the group algebra $\mathbf{Z}[\mathfrak{S}_n]$, set

$$
a_{\mathbf{p}}=_{\sigma}\sum_{\in\mathscr{P}}e_{\sigma},b_{\mathbf{p}}=_{\tau}\sum_{\in\mathscr{P}'}\varepsilon (\tau )e_{\tau},c_{\mathbf{p}}=a_{\mathbf{p}}b_{\mathbf{p}}
$$

Prove that $c_{\mathbf{p}}$ satisfies $e_{\sigma}c_{\mathbf{p}}e_{\sigma'}=\varepsilon (\sigma ')c_{\mathbf{p}}$ for every $\sigma \in \mathscr{P}$ and $\sigma '\in \mathscr{P}'$ and that every element that has this property belongs to $\mathbf{Z}c_{\mathbf{p}}$ (write such a element as $\sum n_{\sigma}e_{\sigma}$, and deduce from b) that $n_{\sigma}$ is zero for $\sigma  /\in \mathscr{P}\mathscr{P}')$. Deduce that for every element $x$ of $\mathbf{Z}[\mathfrak{S}_n]$, the element $c_{\mathbf{p}}xc_{\mathbf{p}}$ belongs to $\mathbf{Z}c_{\mathbf{p}}$. d) Denote by A the $\mathbf{Q}$-algebra $\mathbf{Q}[\mathfrak{S}_n]$. Prove that the ideal $V_{\mathbf{p}}= Ac_{\mathbf{p}}$ of A is an absolutely simple A-module. (Observe that we have $c_{\mathbf{p}}V_{\mathbf{p}}\subset \mathbf{Q}c_{\mathbf{p}}$ by c). Prove that if $\mathfrak{a}$ is a left ideal strictly contained in $V_{\mathbf{p}}$, then we have $c_{\mathbf{p}}\mathfrak{a}= 0$, and therefore $\mathfrak{a}^2= 0$ and finally $\mathfrak{a}= 0.)$ e) Prove that we have $c^2_{\mathbf{p}}= (n$!$/[V_{\mathbf{p}}:\mathbf{Q}])c_{\mathbf{p}}$ (calculate the trace of the endomorphism $x\mapsto xc_{\mathbf{p}}$ of A).

$\P 23)$ Keep the notation of the previous exercise. Let $\mathbf{p}= (p_i)$ and $\mathbf{q}= (q_j)$ be two elements of $\mathscr{S}_n$. a) Suppose that we have $\mathbf{p}>\mathbf{q}$ for the lexicographical order. Prove that we have $a_{\mathbf{p}}xb_{\mathbf{q}}= 0$ for every $x\in A$. (Reduce to the case $x= 1$. Observe that if $(P_i),(P'_j)$ denote the partitions associated with $\mathbf{p}$ and $(Q_k),(Q'_l)$ those associated with $\mathbf{q}$, then, denoting by $s$ the smallest integer $n$ such that $p_n\not=q_n$, we have Card(P$_s\cap Q'_1)\geqslant 2$, and construct a transposition $\tau$ such that $a_{\mathbf{p}}\tau =a_{\mathbf{p}}$ and $\tau  b_{\mathbf{q}}=-b_{\mathbf{q}}.)$ b) Deduce that if $\mathbf{p}\not=\mathbf{q}$, then the A-modules $V_{\mathbf{p}}$ and $V_{\mathbf{q}}$ are not isomorphic (apply a), using the antiautomorphism of A that sends $e_{\sigma}$ to $e_{\sigma^{-1}})$. c) Prove that the mapping that sends a sequence $\mathbf{p}$ to the representation $(V_{\mathbf{p}})_{(K)}$ defines a bijection from $\mathscr{S}_n$ to the set $\mathscr{S}_K(\mathfrak{S}_n)$ of classes of simple $K[\mathfrak{S}_n$]-modules. d) For $\mathbf{p}\in \mathscr{S}_n$, denote by $\mathbf{p}$ the sequence defined by $p_j=$ Card(P$'_j)$ (Exercise 22). Prove that the mapping $\mathbf{p}\mapsto \mathbf{p}$ is a involution of $\mathscr{S}_n$; the A-module $V_{\mathbf{p}}$ is isomorphic to $V_{\mathbf{p}}\otimes_{\mathbf{Q}}\mathbf{Q}_{\varepsilon}$, where $\mathbf{Q}_{\varepsilon}$ denotes the 1-dimensional representation over $\mathbf{Q}$ associated with the signature. e) Describe the representations corresponding to the sequences $(1, . . . ,1)$ and $(n)$, as well as to the sequence $(n-1,1)$.

$\P 24)$ Keep the notation of Exercises 21 through 23. Let $\mathbf{p}= (p_i)_{1\leqslant i\leqslant d}\in \mathscr{S}_n$; denote by $\mathbf{p}$ the element $(p_1, . . . , p_d,0, . . . ,0)$ of $\mathscr{D}_n$. If $\boldsymbol{\alpha }= (\alpha_1, . . . , \alpha_n)$ is an element of $\mathbf{N}^n$ such that $\sum_ii\alpha_i=n$, then we denote by $C_{\boldsymbol{\alpha }}$ the conjugacy class of $\mathfrak{S}_n$ consisting of the elements that are the product of a family of cycles with disjoint support consisting of $\alpha_2$ cycles of order $2,\alpha_3$ cycles of order 3, etc. a) Prove that the representation $\rho_{\mathbf{p}}$ of $\mathfrak{S}_n$ in the A-module $Aa_{\mathbf{p}}$ is the representation induced by the trivial representation of $\mathscr{P}$. Use Exercise 20 to deduce the formula $\chi_{\rho_{\mathbf{p}}}(C_{\boldsymbol{\alpha }}) = [f^{\boldsymbol{\alpha }}]_{\mathbf{p}}$. b) For any $\mathbf{q}\in \mathscr{S}_n$, denote by $\lambda_{\mathbf{q}}$ the representation of $\mathfrak{S}_n$ in the A-module $V_{\mathbf{q}}$. Prove that there exist positive integers $n_{\mathbf{p}\mathbf{q}}$ such that we have $\chi_{\rho_{\mathbf{p}}}=\sum_{\mathbf{q}\in\mathscr{S}_n}n_{\mathbf{p}\mathbf{q}}\chi_{\lambda_{\mathbf{q}}}$ with $n_{\mathbf{p}\mathbf{p}}>0$. c) Let $\eta_{\mathbf{p}}$ be the central function on $\mathfrak{S}_n$ with value $\omega_{\mathbf{p}}(f^{\boldsymbol{\alpha }})$ on the elements of the class $C_{\boldsymbol{\alpha }}$. Prove that $\eta_{\mathbf{p}}$ is a linear combination of the characters $\chi_{\lambda_{\mathbf{q}}}$ for $\mathbf{q}\in \mathscr{S}_n$ with integer coefficients (use Exercise 21, c) and e)). Deduce that $\eta_{\mathbf{p}}$ is equal, up to a sign, to one of the characters $\chi_{\lambda_{\mathbf{q}}}$. (Calculate $\langle \eta_{\mathbf{p}}, \eta_{\mathbf{p}}\rangle$ using Exercise 21, f).) d) Deduce the equality $\chi_{\lambda_{\mathbf{p}}}(C_{\boldsymbol{\alpha }}) =$ [∆$f^{\boldsymbol{\alpha }}]_{\mathbf{p}'}$ (“Frobenius formula”). e) Prove that the multiplicity of the irreducible representation $\lambda_{\mathbf{p}}$ in the representation $\rho_{\mathbf{q}}$ is equal to $K_{\mathbf{p}\mathbf{q}}$. f ) Prove that the degree of $\lambda_{\mathbf{p}}$ is $_{\mathbf{p}}^{n_'!}_!$∆($\mathbf{p}')$ (expand the polynomial ∆($\mathbf{X})(\sum X_i)^n)$.

$\P 25)$ Consider the representation $\pi_{\mathbf{n}}$ of $\mathfrak{S}_n$ associated with the action of $\mathfrak{S}_n$ on the set $\mathbf{n}=[1, n]$ (Exercise 6). Let $k$ be a positive integer and $\chi_k$ the character of the representation $\wedge^k\pi_{\mathbf{n}}$. a) Let $\sigma \in \mathfrak{S}_n$. Prove the formula $\chi_k(\sigma ) =\sum\varepsilon (\sigma |S)$, where the sum is taken over the set of subsets S of $\mathbf{n}$ with $k$ elements such that $\sigma (S) = S$. b) Prove that $\wedge^k\pi_{\mathbf{n}}$ is the irreducible representation of $\mathfrak{S}_n$ associated with the element $(n-k,1, . . . ,1)$ of $\mathscr{S}_n$ (calculate the character of this representation using the Frobenius formula, observing that the only terms of the sum

∆($\mathbf{X})f^{\boldsymbol{\alpha }}(\mathbf{X}) =_{\sigma}\sum_{\in\mathfrak{S}_n}\varepsilon (\sigma )X^{\sigma}_1^{(n)-1}. . .X^{\sigma}_n$[^1]$^{-1}f^{\boldsymbol{\alpha }}(\mathbf{X})$

for which the coefficient of $\mathbf{X}^{\mathbf{p}'}$ is nonzero correspond to the permutations $\sigma$ that satisfy $\sigma (i)\leqslant i+ 1$ for every $i$ and $\sigma (i) =i$ for $1\leqslant i < n-k.)$

$\P 26)$ Let $q$ be a power of a prime number and F a finite field with $q$ elements; take G to be the group $\mathbf{G}\mathbf{L}(2,F)$. a) Describe the conjugacy classes of G (distinguish four types of classes, containing, respectively, $1,q^2-1,q^2+q$, and $q^2-q$ elements). b) The group G acts on the projective line P over F; consider the representation $\pi_P$ of G (Exercise 6). For any group homomorphism $\lambda : F^*\rightarrow K^*$, denote by $\delta_{\lambda}$ the representation of degree 1 associated with the homomorphism $\lambda \circ$ det from G to $K^*$, and set $\pi_{\lambda}=\pi_P\otimes \delta_{\lambda}$. Prove that $\pi_{\lambda}$ is irreducible, and calculate its character. c) Let B be the subgroup of G consisting of the upper triangular matrices. For $\lambda , µ$ in Hom(F$^*,K^*)$, denote by $\beta_{\lambda ,µ}$ the representation of B of degree 1 defined by $\beta_{\lambda ,µ}((a_{ij})) =\lambda (a_{11})µ(a_{22})$, and set $\pi_{\lambda ,µ}=$ Ind$^G_B(\beta_{\lambda ,µ})$. Prove that $\pi_{\lambda ,µ}$ is irreducible for $\lambda \not=µ$, while $\pi_{\lambda ,\lambda}$ is isomorphic to $\pi_P\oplus \delta_{\lambda}$ (apply Exercise 8). The representations $\pi_{\lambda ,µ}$ and $\pi_{\lambda',µ'}$ are isomorphic if and only if the subsets $\{\lambda , µ\}$ and $\{\lambda ', µ'\}$ of Hom(F$^*,K^*)$ are equal. d) Let $F'$ be an extension of F of degree 2; choosing a basis of $F'$ over F allows one to identify $F^{'*}$ with a subgroup of G = Aut$_F(F')$. Let $\varphi \in$ Hom(F$^{'*},K^*)$; calculate Ind$^G_{F^{'*}}(\varphi )$, and prove that it is equal to Ind$^G_{F^{'*}}(\varphi^q)$. Denote by $\lambda$ the restriction of $\varphi$ to $F^*$, and set $\chi_{\varphi}=\chi_{\pi_P\otimes\pi_{\lambda ,1}}-\chi_{\pi_{\lambda ,1}}-$ Ind$^G_{F^{'*}}(\varphi )$. Prove that if $\varphi \not=\varphi^q$, then we have $\langle \chi_{\varphi}, \chi_{\varphi}\rangle = 1$ and $\chi_{\varphi}(1) =q-1$, so that $\chi_{\varphi}$ is the character of an irreducible representation $\pi_{\varphi}$ of dimension $q-1$. Prove that we thus obtain $^1_2q(q-1)$ nonisomorphic irreducible representations. e) Prove that the irreducible representations $\pi_{\lambda}$ for $\lambda \in$ Hom(F$^*,K^*),\pi_{\lambda ,µ}$ for a subset $\{\lambda , µ\}$ of Hom(F$^*,K^*)$ with two elements, and $\pi_{\varphi}$ for $\varphi \in$ Hom(F$^{'*},K^*)$ with $\varphi \not=\varphi^q$ are pairwise nonisomorphic and that every irreducible representation of G is isomorphic to one of them.

27) Let F be an algebraically closed field of characteristic $p >0$ and G be a finite group. a) Let $x\in G$. Prove that there exists a unique decomposition $x=x_ux_s$, where the order of $x_u$ is a power of $p$, that of $x_s$ is prime to $p$, and $x_u$ and $x_s$ commute. The elements $x_u$ and $x_s$ are powers of $x$. b) Let $\pi$ be a linear representation of G over F of finite degree. Prove that we have $\chi_{\pi}(x) =\chi_{\pi}(x_s)$ for every $x\in G$. c) We say that an element $x$ of G is $p$-regular if its order is prime to $p$; we denote by $G^{reg}$ the set of $p$-regular elements of G and by $\mathscr{Z}_F(G^{reg})$ the space of central functions from $G^{reg}$ to F. From the homomorphism $R_F(G)\rightarrow \mathscr{Z}_F(G^{reg})$ that sends the class of a representation $\pi$ to the restriction of $\chi_{\pi}$ to $G^{reg}$, we deduce a ring homomorphism $\psi : F\otimes_{\mathbf{Z}}R_F(G)\rightarrow \mathscr{Z}_F(G^{reg})$. Prove that $\psi$ is injective (use b) and the corollary of VIII, p. 384). d) Let $x$ be a $p$-regular element of $G, Z(x)$ its commutant, P a Sylow $p$-subgroup of $Z(x)$, and $H_x$ the subgroup of G generated by P and $x$. Prove that $H_x$ is the direct product of P and the subgroup of G generated by $x$ and that its conjugacy class is well determined by the conjugacy class of $x$. e) Construct representations $\sigma_1, . . . , \sigma_m$ of $H_x$ of degree 1 and elements $a_1, . . . , a_m$ of F such that the function $\sum a_i\chi_{\sigma_i}$ takes value 1 at $x$ and 0 at the other powers of $x$ (first construct representations of the subgroup generated by $x)$. Let $\rho_i=$ Ind$^G_{H_x}\pi_i$ for $i= 1, . . . , m$, and let $f=\sum_ia_i\chi_{\rho_i}$. Prove that $f(x)$ is equal to $(Z(x) : H_x) 1_F$, which is nonzero in F, and that $f(y)$ is zero for every $p$-regular element of G that is not conjugate to $x$. f ) Deduce from e) that the homomorphism $\psi : F\otimes_{\mathbf{Z}}R_F(G)\rightarrow \mathscr{Z}_F(G^{reg})$ is bijective. In particular, the number of isomorphism classes of simple F[G]-modules is equal to the number of conjugacy classes of $p$-regular elements of G.

28) Keep the assumptions of Exercise 27. Let $m$ be the l.c.m. of the orders of the $p$-regular elements of G. Let $F_0$ be the subfield of F generated by the $m$-th roots of unity; it is a finite field. a) Prove that the character of any representation of G over F of finite degree takes all its values in $F_0$. b) Prove that the quotient ring of $F_0[G]$ by its radical is a product of matrix algebras over $F_0$ (use a) and Wedderburn’s theorem). Deduce that the canonical homomorphism $R_{F_0}(G)\rightarrow R_F(G)$ is bijective.

29) Keep the assumptions and notation of Exercises 27 and 28. Choose a primitive $m$-th root of unity $\zeta$. Let $\mathscr{O}_m$ be the ring $\mathbf{Z}[X]/(Φ_m)$ (VIII, p. 415); we denote the class of X in $\mathscr{O}_m$ by $x$. Let $\varphi :\mathscr{O}_m\rightarrow F$ be the homomorphism that sends $x$ to $\zeta$. It induces an isomorphism from the subgroup of $\mathscr{O}_m$ generated by $x$ to the group $µ_m(F)$; we denote the inverse isomorphism by $\tau$. a) Let $\pi$ be a linear representation of G over F, of finite dimension $d$. For $g\in G$, let $P_g(X) =\prod^d_{i=1}(X-\lambda_i)$ be the characteristic polynomial of $\pi (g)$; denote by $\beta_{\pi}(g)$ the element $\sum_i\tau (\lambda_i)$ of $\mathscr{O}_m$. The resulting function $\beta_{\pi}: G\rightarrow \mathscr{O}_m$ is called the Brauer character of $\pi$; we have $\varphi \circ \beta_{\pi}=\chi_{\pi}$ and $\beta_{\pi}(x) =\beta_{\pi}(x_s)$ for every $x$, so that $\beta_{\pi}$ is determined by its restriction to $G^{reg}$. b) Let $\widehat{G}$ be the set of isomorphism classes of simple F[G]-modules. Prove that the functions $(\beta_{\lambda})_{\lambda\in\widehat{G}}$ are linearly independent over $\mathbf{Z}$. (If there exists a nontrivial relation $\sum n_{\lambda}\beta_{\lambda}= 0$, then we may assume that one of the $n_{\lambda}$ is prime to $p$ and apply $\varphi$ to arrive at a contradiction using Exercise 27, f).) c) Let $\mathscr{B}$ be the set of functions from $G^{reg}$ to $\mathscr{O}_m$; the homomorphism $R_F(G)\rightarrow \mathscr{B}$ that sends the class of $\pi$ to $\beta_{\pi}$ is injective. Deduce that two semisimple F[G]-modules are isomorphic if and only if their Brauer characters are equal.

30) Let F be an algebraically closed field of characteristic $p >0$, let $\mathbf{F}_p$ be the prime subfield of F, and let $G =\mathbf{S}\mathbf{L}_2(\mathbf{F}_p)$. Denote by V the F-vector space $F\otimes_{\mathbf{F}_p}\mathbf{F}^2_p$ endowed with the action of G deduced from the action on $\mathbf{F}^2_p$. a) Prove that the F[G]-module $\mathsf{S}^d(V)$ is simple for $0\leqslant d < p$. (Let W be a nonzero F[G]-submodule of $\mathsf{S}^d$(V), and let $(e, f)$ be a basis of V. Prove that $e^d$ belongs to W using the matrix $(^{1 1}_{0 1})$, and then that W is equal to $\mathsf{S}^d(V)$ using the matrix $(^{1 0}_{1 1}).)$ b) Prove that the F[G]-module $\mathsf{S}^p(V)$ is not simple (consider the image of V by the mapping $v\mapsto v^p)$. c) For $p\geqslant 7$, prove that the dimension of $\mathsf{S}^{p-3}(V)$ does not divide the order of G. d) Prove that every simple F[G]-module is isomorphic to one of the modules $\mathsf{S}^d(V)$ for $0\leqslant d < p$ (use Exercise 27, f)).

[^1]: The elements of Hom$_G(\pi , \pi ')$ are sometimes called intertwining operators of $\pi$ and $\pi '$.
[^2]: This means that the homomorphism $\pi : G\rightarrow$ Aut$_K(M)$ is injective.
