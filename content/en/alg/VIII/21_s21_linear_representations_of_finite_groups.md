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
content_sha256: 0e5deb34291587d4a1d8a7a45209a10bf955b05cd9dffa7094c05b7d274161a4
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

See the [exercises for § 21](exercises/s21/).

[^1]: The elements of Hom$_G(\pi , \pi ')$ are sometimes called intertwining operators of $\pi$ and $\pi '$.
