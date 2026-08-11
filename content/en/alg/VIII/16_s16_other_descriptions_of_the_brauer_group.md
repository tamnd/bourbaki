---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 16
section_title: Other Descriptions of the Brauer Group
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.285-A VIII.333
pdf_pages: 0302-0350
extraction: native
subsections:
    - "no": 1
      title: $\tau$-Extensions of Groups
      page: 285
      pdf_page: 302
    - "no": 2
      title: Inverse Image of a $\tau$-Extension
      page: 287
      pdf_page: 304
    - "no": 3
      title: Direct Image of a $\tau$-Extension
      page: 289
      pdf_page: 306
    - "no": 4
      title: Group Law on the Classes of $\tau$-Extensions
      page: 293
      pdf_page: 310
    - "no": 5
      title: Cohomological Description
      page: 295
      pdf_page: 312
    - "no": 6
      title: Restriction and Corestriction
      page: 299
      pdf_page: 316
    - "no": 7
      title: Galois Algebras
      page: 304
      pdf_page: 321
    - "no": 8
      title: Actions on Galois Algebras
      page: 312
      pdf_page: 329
    - "no": 9
      title: Cross Products
      page: 314
      pdf_page: 331
    - "no": 10
      title: Application to the Brauer Group
      page: 317
      pdf_page: 334
    - "no": 11
      title: Index and Exponent
      page: 322
      pdf_page: 339
statements: 59
exercises: 17
content_sha256: 97498f8fa6bfa8d5146ddd88a2f2c93625312d8ea5d3e5a93a45a6be85d617f9
---

## § 16. OTHER DESCRIPTIONS OF THE BRAUER GROUP

In this section, if F is an abelian group and $g$ an automorphism of F, then we write $g\cdot f$ for $g(f)$.

### 1. $\tau$-Extensions of Groups

In this subsection, we fix a group G, an abelian group F written multiplicatively, and a group homomorphism $\tau$ from G to the automorphism group Aut(F) of F. We denote the identity element of G by $e$ and the identity element of F by 1.

Recall (I, §6, No. 1, p. 65) that an extension $\mathscr{E}$ of G by F is a triple $(Γ, \iota , \pi )$, where Γ is a group, $\pi : Γ\rightarrow G$ is a surjective homomorphism, and $\iota$ is an injective homomorphism from F to Γ such that Im($\iota ) =$ Ker($\pi )$. Let $\mathscr{E}= (Γ, \iota , \pi )$ be such an extension. For every $\gamma \in Γ$, the mapping $\varphi_{\gamma}: F\rightarrow F$ defined by

$$
\iota (\varphi_{\gamma}(f)) =\gamma \iota (f)\gamma^{-1}
$$

for $f\in F$ is an automorphism of F. Since F is commutative, for every $f\in F$, the automorphism defined by $\iota (f)$ is the identity mapping on F. By passing to the quotient, we obtain a homomorphism Int$_{\mathscr{E}}$ from G to Aut(F) characterized by

$\gamma \iota (f)\gamma^{-1}=\iota$(Int$_{\mathscr{E}}(\pi (\gamma ))\cdot f)$ for $\gamma \in Γ$ and $f\in F$.

$A\tau$-extension of G by F is an extension $\mathscr{E}= (Γ, \iota , \pi )$ such that Int$_{\mathscr{E}}$ is equal to $\tau$, in other words, that satisfies the relation

$$
\gamma \iota (f)\gamma^{-1}=\iota (\tau (\pi (\gamma ))\cdot f) \tag{1}
$$

for $\gamma \in Γ$ and $f\in F$. If $\mathscr{E}= (Γ, \iota , \pi )$ and $\mathscr{E}'= (Γ', \iota ', \pi ')$ are $\tau$-extensions, then a morphism of $\tau$-extensions from $\mathscr{E}$ to $\mathscr{E}'$ is a morphism of extensions from $\mathscr{E}$ to $\mathscr{E}'$ (I, §6, No. 1, p. 65), that is, a group homomorphism $u: Γ\rightarrow Γ'$ such that $\pi '\circ u=\pi$ and $\iota '=u\circ \iota$. Note that the $\tau$-extensions form a species of structures for which every morphism is an isomorphism (Set Theory, IV, §1, No. 5, p. 264 and I, §6, No. 1, p. 66, Proposition 1). Denote by Iso$_{\tau}(\mathscr{E},\mathscr{F})$ the relation

“$\mathscr{E}$ and $\mathscr{F}$ are isomorphic $\tau$-extensions.” This is an equivalence relation; the class of the extension $\mathscr{E}$ is the class of objects equivalent to $\mathscr{E}$ for Iso$_{\tau}($Set Theory, II, §6, No. 6, p. 122).

#### Lemma 1 {#alg-viii-s16-lem-1 .statement}

The relation

“$\alpha$ is the class of a $\tau$-extension for Iso$_{\tau}$”

is collectivizing in $\alpha$.

Set $E_0= F\times G$, and consider the mappings $\iota_0: F\rightarrow E_0$ and $\pi_0: E_0\rightarrow G$ defined by $\iota_0(f) = (f, e)$ for $f\in F$ and $\pi_0(f, g) =g$ for $(f, g)\in F\times G$. Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension of G by F. The mapping $\pi$ is surjective, so has a section $\sigma : G\rightarrow Γ$ such that $\sigma (e) =e$. The mapping $u: (f, g)\mapsto \iota (f)\sigma (g)$ from $F\times G$ to Γ is bijective. We endow $F\times G$ with the group law obtained by transfer of structure. The triple $(E_0, \iota_0, \pi_0)$ is then a $\tau$-extension isomorphic to $\mathscr{E}$. Lemma 1 now follows from Set Theory, II, §6, No. 6, p. 122.

We denote by Ex$_{\tau}(G,F)$ the set of classes of $\tau$-extensions for the relation Iso$_{\tau}$.

#### Example 1 {#alg-viii-s16-n1-exa-1 .statement}

The external semidirect product $(F\times_{\tau}G, i, p)$ (I, §6, No. 1, p. 66, Proposition 3) is a $\tau$-extension; we denote it by $\mathscr{I}_{\tau}$. We say that a $\tau$-extension is semitrivial if it is isomorphic to the $\tau$-extension $\mathscr{I}_{\tau}$.

#### Example 2 {#alg-viii-s16-n1-exa-2 .statement}

For $i\in  \{1,2\}$, take a group $G_i$, an abelian group $F_i$, and a group homomorphism $\tau_i$ from $G_i$ to the automorphism group of $F_i$. We denote by $\tau_1\times \tau_2: G_1\times G_2\rightarrow$ Aut(F$_1\times F_2)$ the homomorphism defined by

$$
(\tau_1\times \tau_2)(g_1, g_2)\cdot (f_1, f_2) = (\tau_1(g_1)\cdot f_1, \tau_2(g_2)\cdot f_2)
$$

for $g_1\in G_1,g_2\in G_2,f_1\in F_1$, and $f_2\in F_2$. Let $\mathscr{E}_1= (Γ_1, \iota_1, \pi_1)$ be a $\tau_1$-extension of $G_1$ by $F_1$ and $\mathscr{E}_2= (Γ_2, \iota_2, \pi_2)$ a $\tau_2$-extension of $G_2$ by $F_2$. Then the triple $(Γ_1\times Γ_2, \iota_1\times \iota_2, \pi_1\times \pi_2)$ is a $\tau_1\times \tau_2$-extension of $G_1\times G_2$ by $F_1\times F_2$; it is called the exterior product of the extensions $\mathscr{E}_1$ and $\mathscr{E}_2$ and denoted by $\mathscr{E}_1\times \mathscr{E}_2$.

### 2. Inverse Image of a $\tau$-Extension

Let G and $G'$ be groups. Let F be an abelian group, and let $\tau : G\rightarrow$ Aut(F) and $u: G'\rightarrow G$ be group homomorphisms. Consider the group homomorphism $\tau '=\tau \circ u: G'\rightarrow$ Aut(F), and denote by $Γ'$ the fiber product $Γ\times_GG'$ with respect to $\pi$ and $u$ (I, §4, No. 8, p. 46). It is the subgroup of $Γ\times G'$ consisting of the pairs $(\gamma , g')$ such that $\pi (\gamma ) =u(g')$. Let $\iota ': F\rightarrow Γ'$ be the group homomorphism given by $\iota '(\alpha ) = (\iota (\alpha ), e)$ for $\alpha \in F$, and denote the second projection by $\pi ': Γ'\rightarrow G'$. Then the morphism $\iota '$ is injective, the morphism $\pi '$ is surjective because $\pi$ is, and the image of $\iota '$ coincides with the kernel of $\pi '$. Moreover, for every $\alpha \in F$ and $\gamma '= (\gamma , g)\in Γ'$, we have the relations

$$
\gamma '\iota '(\alpha )\gamma^{'-1}= (\gamma , g)(\iota (\alpha ), e)(\gamma , g)^{-1}= (\iota (\tau (\pi (\gamma )).\alpha ), e) =\iota '(\tau '(\pi '(\gamma ')).\alpha )
$$

Consequently, $(Γ', \iota ', \pi ')$ is a $\tau '$-extension of $G'$ by F; we call it the inverse image of $\mathscr{E}$ by $u$ and denote it by $u^*(\mathscr{E})$. The first projection is a group homomorphism $\varphi : Γ'\rightarrow Γ$ that we call canonical.

#### Proposition 1 {#alg-viii-s16-prop-1 .statement}

The following diagram commutes:

F $^{\iota'}$ // $Γ_'^{\pi'}$ // $G_'$ (2)

$\varphi u$

F $^{\iota}$ // Γ $^{\pi}$ // G. Moreover, if $\mathscr{E}_1'= (Γ'_1, \iota '_1, \pi '_1)$ is a $\tau '$-extension and $\varphi_1: Γ'_1\rightarrow Γ$ is a group homomorphism such that the diagram

F $^{\iota'_1}$ // $Γ_{'1}^{\pi'_1}$ // $G_'$

$\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

commutes, then there exists a unique morphism $\psi$ of $\tau '$-extensions from $\mathscr{E}_1'$ to $u^*(\mathscr{E})$ such that we have $\varphi_1=\varphi \circ \psi$.

The commutativity of the first diagram follows from the definition of $\varphi$. The existence and uniqueness of $\psi$ follow from Lemma 2 below.

#### Lemma 2 {#alg-viii-s16-lem-2 .statement}

Let $F'_1$ be an abelian group, and let $w: F'_1\rightarrow$ F and $\tau_1: G'\rightarrow$ Aut(F$'_1)$ be group homomorphisms such that

$$
w(\tau_1(g)(f)) =\tau (u(g))(w(f))
$$

for every $f\in F'_1$ and $g\in G'$. Let $\mathscr{E}_1'= (Γ'_1, \iota '_1, \pi '_1)$ be a $\tau_1$-extension of $G'$ by $F'_1$ and $\varphi_1: Γ'_1\rightarrow Γ$ a group homomorphism such that the following diagram commutes:

$F_{'1}^{\iota'_1}$ // $Γ_{'1}^{\pi'_1}$ // $G_'$

$w\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G. Then there exists a unique group homomorphism $\psi : Γ'_1\rightarrow Γ'$ such that the diagram

$F_{'1}^{\iota'_1}$ // $Γ_{'1}^{\pi_1'}$ // $G_'$

$w\psi$

F $^{\iota'}$ // $Γ_'^{\pi'}$ // $G_'$

commutes and $\varphi_1=\varphi \circ \psi$.

If the group homomorphism $\psi : Γ'_1\rightarrow Γ'$ has the desired properties, then it satisfies the relations

$$
\psi (\gamma ) = (\varphi \circ \psi (\gamma ), \pi '\circ \psi (\gamma )) = (\varphi_1(\gamma ), \pi '_1(\gamma ))
$$

for every $\gamma \in Γ'_1$. Conversely, the group homomorphism from $Γ'_1$ to $Γ\times G'$ defined by $\gamma \mapsto (\varphi_1(\gamma ), \pi_1'(\gamma ))$ has values in the fiber product $Γ\times_GG'$ because $\pi \circ \varphi_1(\gamma ) =u\circ \pi_1'(\gamma )$ for every $\gamma \in Γ'_1$.

#### Corollary 1 {#alg-viii-s16-lem-2-cor-1 .statement}

Let $\mathscr{E}_1$ and $\mathscr{E}_2$ be $\tau$-extensions of G by F, and let $\psi$ be a morphism of $\tau$-extensions from $\mathscr{E}_1$ to $\mathscr{E}_2$. Denote by $\varphi_1($resp. $\varphi_2)$ the canonical homomorphism for $u^*(\mathscr{E}_1) ($resp. $u^*(\mathscr{E}_2))$. Then there exists a unique morphism of $\tau '$-extensions from $u^*(\mathscr{E}_1)$ to $u^*(\mathscr{E}_2)$, denoted by $u^*(\psi )$, such that $\varphi_2\circ u^*(\psi ) =\psi \circ \varphi_1$.

It suffices to apply Proposition 1 to $\psi \circ \varphi_1$.

The class of the $\tau '$-extension $u^*(\mathscr{E})$ therefore depends only on the class of $\mathscr{E}$. We also denote by $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G',F)$ the mapping that sends the class of a $\tau$-extension $\mathscr{E}$ to the class of the $\tau '$-extension $u^*(\mathscr{E})$.

#### Corollary 2 {#alg-viii-s16-lem-2-cor-2 .statement}

Let $u': G''\rightarrow G'$ be a group homomorphism, and let $\mathscr{E}$ be a $\tau$-extension of G by F. Set $\tau ''=\tau '\circ u'$, and denote by $\varphi ($resp. $\varphi ',\varphi '')$ the canonical homomorphism associated with the $\tau '$-extension $u^*(\mathscr{E}) ($resp. the $\tau ''$-extension $u^{'*}(u^*(\mathscr{E}))$, the $\tau ''$-extension $(u\circ u')^*(\mathscr{E}))$. Then there exists a unique morphism $\psi$ from the $\tau ''$-extension $u^{'*}(u^*(\mathscr{E}))$ to the $\tau ''$-extension $(u\circ u')^*(\mathscr{E})$ such that $\varphi ''\circ \psi =\varphi \circ \varphi '$. **Example.** — Let H be a subgroup of G and $j: H\rightarrow G$ the canonical injection. Then for every $\tau$-extension $\mathscr{E}= (Γ, \iota , \pi )$, the $\tau \circ j$-extension $j^*(\mathscr{E})$ is isomorphic to $(^-\pi^1(H), \iota ', \pi ')$, where $\iota ': F\rightarrow^-\pi^1(H)$ (resp. $\pi ':^-\pi^1(H)\rightarrow H)$ is the group homomorphism $f\mapsto \iota (f)$ (resp. $\gamma \mapsto \pi (\gamma ))$. More generally, if the group homomorphism $u: G'\rightarrow G$ is injective, then the canonical homomorphism $\varphi$ is injective with image $^-\pi^1(u(G'))$.

### 3. Direct Image of a $\tau$-Extension

Let G be a group, let F and $F'$ be abelian groups, let $\tau$ (resp. $\tau ')$ be a group homomorphism from G to the automorphism group of F (resp. $F')$, and let $v: F\rightarrow F'$ be a group homomorphism such that

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{3}
$$

for every $g\in G$ and $f\in F$. Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension of G by F. Let $\widetilde{Γ}$ be the external semidirect product $F'\times_{\tau'\circ\pi}Γ$. We denote by $\widetilde{ı}: F'\rightarrow \widetilde{Γ}$ the homomorphism $f\mapsto (f, e)$ and by $\widetilde{p}:\widetilde{Γ}\rightarrow Γ$ the first projection. Let $j: F\rightarrow \widetilde{Γ}$ be the mapping defined by $f\mapsto (v(f), \iota (f)^{-1})$. Since the image of $\iota$ is contained in the kernel of $\tau '\circ \pi$, the mapping $j$ is a group homomorphism; it is injective because $\iota$ is injective. We have the relations

$$
(f', \gamma )j(f)(f', \gamma )^{-1}= (f', \gamma )(v(f), \iota (f)^{-1})(f', \gamma )^{-1}
$$

(4) $= (\tau '(\pi (\gamma ))\cdot v(f), \iota (\tau (\pi (\gamma ))\cdot f)^{-1})$

$$
=j(\tau (\pi (\gamma ))\cdot f)
$$

for $f\in F,\gamma \in Γ$, and $f'\in F'$. Consequently, the image of $j$ is a normal subgroup of $\widetilde{Γ}$. We denote by $Γ'$ the quotient of $\widetilde{Γ}$ by the image of $j$. We denote by $\iota '$ the composition of the canonical surjection from $\widetilde{Γ}$ to $Γ'$ and $\widetilde{ı}$. The kernel of the homomorphism $\pi \circ \widetilde{p}$ is the product $F'\times \iota$(F), which contains the image of $j$. We define $\pi ': Γ'\rightarrow G$ as the group homomorphism deduced from $\pi \circ \widetilde{p}$ by passing to the quotient. Since $\iota$ is injective, the intersection of $j(F)$ and $\widetilde{ı}(F')$ is reduced to the identity element of $\widetilde{Γ}$; it follows that $\iota '$ is injective. The mapping from $F'\times F$ to $F'\times \iota (F) =$ Ker($\pi \circ \widetilde{p})$ given by

$$
(f', f)\longmapsto (f'v(f), \iota (f)^{-1})
$$

is a group isomorphism. The image of $\iota '$ therefore coincides with the kernel of $\pi '$. Since $\pi$ and $\widetilde{p}$ are surjective, so is $\pi '$. This proves that $\mathscr{E}'= (Γ', \iota , \pi ')$ is a $\tau '$-extension of G by $F'$; we call it the direct image of $\mathscr{E}$ by $v$ and denote it by $v_*(\mathscr{E})$. The composition of the canonical surjection from $\widetilde{Γ}$ to $Γ'$ and the group homomorphism from Γ to $\widetilde{Γ}$ given by $\gamma \mapsto (1, \gamma )$ is a group homomorphism $\varphi : Γ\rightarrow Γ'$ that we call canonical.

#### Proposition 2 {#alg-viii-s16-prop-2 .statement}

In the notation above, the following diagram commutes:

F $^{\iota}$ // Γ $^{\pi}$ // G (5) $v\varphi$

$F_'^{\iota'}$ // $Γ_'^{\pi'}$ // G .

Let $\mathscr{E}_1'= (Γ'_1, \iota '_1, \pi_1')$ be a $\tau '$-extension of G by $F'$, and let $\varphi_1: Γ\rightarrow Γ'_1$ be a group homomorphism such that the following diagram commutes:

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1$

$F_'^{\iota'_1}$ // $Γ_{'1}^{\pi'_1}$ // G.

Then there exists a unique morphism $\psi$ of $\tau '$-extensions from $v_*(\mathscr{E})$ to $\mathscr{E}_1'$ such that we have $\varphi_1=\psi \circ \varphi$.

The commutativity of the first diagram follows by construction. The existence and uniqueness of $\psi$ follow from Lemma 3 below.

#### Lemma 3 {#alg-viii-s16-lem-3 .statement}

Let $G'_1$ be a group, and let $w: G\rightarrow G'_1$ and $\tau_1: G'_1\rightarrow$ Aut(F$')$ be group homomorphisms such that $\tau '=\tau_1\circ w$. Let $\mathscr{E}_1'= (Γ'_1, \iota '_1, \pi '_1)$ be a $\tau_1$-extension of $G'_1$ by $F'$, and let $\varphi_1: Γ\rightarrow Γ'_1$ be a group homomorphism such that the following diagram commutes:

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1w$

$F_'^{\iota'_1}$ // $Γ_{'1}^{\pi'_1}$ // $G_{'1}$.

Then there exists a unique group homomorphism $\psi : Γ'\rightarrow Γ'_1$ such that the diagram

$F_'^{\iota'}$ // $Γ_'^{\pi'}$ // G

$\psi w$

$F_'^{\iota'_1}$ // $Γ_{'1}^{\pi'_1}$ // $G_{'1}$ commutes and $\varphi_1=\psi \circ \varphi$.

For any $(f, \gamma )\in F'\times Γ$, denote the class of $(f, \gamma )$ in $Γ'$ by $(f, \gamma )$. If the group homomorphism $\psi : Γ'\rightarrow Γ'_1$ has the desired properties, then it satisfies the relations

$$
\psi (f', \gamma )=\psi (\iota '(f')\varphi (\gamma )) =\iota '_1(f')\varphi_1(\gamma )
$$

for every $f'\in F'$ and $\gamma \in Γ$. Conversely, the mapping $\widetilde{\psi}$ from $F'\times_{\tau'\circ\pi}Γ$ to $Γ'_1$ given by $(f, \gamma )\mapsto \iota '_1(f)\varphi_1(\gamma )$ is a group homomorphism. Indeed, we have the relations

$$
\iota '_1(f)\varphi_1(\gamma )\iota '_1(f')\varphi_1(\gamma ') =\iota '_1(f \tau_1(\pi '_1(\varphi_1(\gamma )))\cdot f')\varphi_1(\gamma \gamma ')
$$

$$
=\iota '_1(f \tau '(\pi (\gamma ))\cdot f')\varphi_1(\gamma \gamma ')
$$

for $f, f'\in F'$ and $\gamma , \gamma '\in Γ$. The kernel of $\widetilde{\psi}$ contains the image of $j$ because $\iota '_1(v(f)) =\varphi_1(\iota (f))$ for $f\in F$, and the morphism $\psi$ deduced from $\widetilde{\psi}$ by passing to the quotient has the desired properties.

#### Remark {#alg-viii-s16-n3-rem-1 .statement}

Denote by Σ the species of structures of $\tau '$-extensions, and define $\alpha$-mappings to be mappings from Γ to a group $Γ'$ underlying a $\tau '$-extension that are group homomorphisms and that make the following diagram commute:

F $^{\iota}$ // Γ $^{\pi}$ // G (6) $v\varphi$

$F_'^{\iota'}$ // $Γ_'^{\pi'}$ // G .

Proposition 2 expresses that $v_*(\mathscr{E})$ is a solution of the corresponding universal mapping problem (Set Theory, IV, §3, No. 1, p. 284).

#### Corollary 1 {#alg-viii-s16-lem-3-cor-1 .statement}

Let $\mathscr{E}_1$ and $\mathscr{E}_2$ be $\tau$-extensions of G by F, and let $\psi$ be a morphism of $\tau$-extensions from $\mathscr{E}_1$ to $\mathscr{E}_2$. Denote by $\varphi_1($resp. $\varphi_2)$ the canonical homomorphism for $v_*(\mathscr{E}_1) ($resp. $v_*(\mathscr{E}_2))$. Then there exists a unique morphism of $\tau '$-extensions from $v_*(\mathscr{E}_1)$ to $v_*(\mathscr{E}_2)$, denoted by $v_*(\psi )$, such that $\varphi_2\circ \psi =v_*(\psi )\circ \varphi_1$.

It suffices to apply Proposition 2 to $\varphi_2\circ \psi$.

The class of the $\tau '$-extension $v_*(\mathscr{E})$ therefore depends only on the class of $\mathscr{E}$. We also denote by $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ the mapping that sends the class of a $\tau$-extension $\mathscr{E}$ to the class of the $\tau '$-extension $v_*(\mathscr{E})$. **Corollary 2.** — We keep the notation of the proposition. Let $F''$ be an abelian group, and let $\tau '': G\rightarrow$ Aut(F$'')$ and $v': F'\rightarrow F''$ be group homomorphisms such that

$$
\tau ''(g)\cdot v'(f) =v'(\tau '(g)\cdot f)
$$

for $g\in G$ and $f\in F'$. Let $\mathscr{E}$ be a $\tau$-extension of G by F, and denote by $\varphi ($resp. $\varphi ',\varphi '')$ the canonical homomorphism associated with $v_*(\mathscr{E}) ($resp. $v_*'(v_*(\mathscr{E}))$, $(v'\circ v)_*(\mathscr{E}))$. Then there exists a unique morphism $\psi$ from the $\tau ''$-extension $v_*'(v_*(\mathscr{E}))$ of G by $F''$ to the $\tau ''$-extension $(v'\circ v)_*(\mathscr{E})$ such that $\varphi ''=\psi \circ \varphi '\circ \varphi$.

#### Example 1 {#alg-viii-s16-n3-exa-1 .statement}

Let $j:\{1\} \rightarrow F$ be the canonical injection. The semitrivial extension $\mathscr{I}_{\tau}$ is isomorphic to $j_*((G, i$, Id$_G))$, where $i:\{e\} \rightarrow G$ is the canonical injection. Let $c: F\rightarrow F$ be the constant homomorphism $f\mapsto 1$, and let $\mathscr{E}$ be a $\tau$-extension. The $\tau$-extension $c_*(\mathscr{E})$ is also isomorphic to $\mathscr{I}_{\tau}$.

#### Example 2 {#alg-viii-s16-n3-exa-2 .statement}

Let E be a subgroup of F stable under the action of G. Denote by $F'$ the quotient of F by E, by $v: F\rightarrow F'$ the canonical homomorphism, and by $\tau ': G\rightarrow$ Aut(F$')$ the action of G on $F'$ characterized by

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

for $g\in G$ and $f\in F$. Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension of G by F. Then $\iota (E)$ is a normal subgroup of Γ, and the $\tau '$-extension $v_*(\mathscr{E})$ of G by $F'$ is isomorphic to the extension $(Γ/\iota (E), \iota , \pi )$, where $\iota$ and $\pi$ are the group homomorphisms deduced from $\iota$ and $\pi$ by passing to the quotients. By this isomorphism, the canonical homomorphism $\varphi$ associated with $v_*(\mathscr{E})$ corresponds to the canonical homomorphism from Γ to $Γ/\iota (E)$.

#### Proposition 3 {#alg-viii-s16-prop-3 .statement}

Let G and $G'$ be groups, and let F and $F'$ be abelian groups. Let $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'),u: G'\rightarrow G$, and $v: F\rightarrow F'$ be group homomorphisms such that

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

for $g\in G$ and $f\in F$. We write $\tau ''=\tau '\circ u$. Let $\mathscr{E}$ be a $\tau$-extension of G by F. We denote by $\varphi_u($resp. $\varphi_v,\varphi '_u,\varphi '_v)$ the canonical homomorphism corresponding to the $\tau \circ u$-extension $u^*(\mathscr{E}) ($resp. to the $\tau '$-extension $v_*(\mathscr{E})$, to the $\tau ''$-extensions $u^*(v_*(\mathscr{E}))$ and $v_*(u^*(\mathscr{E})))$. Then there exists a unique morphism $\psi$ of $\tau ''$-extensions from $v_*(u^*(\mathscr{E}))$ to $u^*(v_*(\mathscr{E}))$ such that $\varphi_v\circ \varphi_u=$ $\varphi '_u\circ \psi \circ \varphi '_v$.

We denote the $\tau \circ u$-extension $u^*(\mathscr{E})$ (resp. the $\tau ''$-extension $u^*(v_*(\mathscr{E})))$ by $(Γ_u, \iota_u, \pi_u)$ (resp. $(Γ'_u, \iota '_u, \pi_u'))$. Applying Lemma 2 of VIII, p. 287 to $\varphi_v\circ \varphi_u$, we find that there exists a group homomorphism $\psi_1: Γ_u\rightarrow Γ'_u$ such that the diagram

F $^{\iota_u}$ // $Γ_u^{\pi_u}$ // $G_'$

$v\psi_1$

$F_'^{\iota'_u}$ // $Γ_{'u}^{\pi'_u}$ // $G_'$

commutes and $\varphi '_u\circ \psi_1=\varphi_v\circ \varphi_u$. The existence of $\psi$ follows from Proposition 2 applied to $\psi_1$. Conversely, if $\psi '$ also has the desired properties, then we have $\psi '\circ \varphi '_v=\psi_1$ by Lemma 2, so $\psi '=\psi$ (Proposition 2).

### 4. Group Law on the Classes of $\tau$-Extensions

Let G be a group, F be an abelian group, and $\tau : G\rightarrow$ Aut(F) be a group homomorphism. We denote by $\delta : G\rightarrow G\times G$ the diagonal mapping $g\mapsto$ $(g, g)$ and by $m: F\times F\rightarrow F$ the multiplication homomorphism $(f_1, f_2)\mapsto$ $f_1f_2$. We denote by $s: F\rightarrow F$ the group homomorphism given by $f\mapsto f^{-1}$. Let $\mathscr{E}_1= (Γ_1, \iota_1, \pi_1)$ and $\mathscr{E}_2= (Γ_2, \iota_2, \pi_2)$ be $\tau$-extensions of G by F. Since we have the relation

$$
m(((\tau \times \tau )\circ \delta )(g)\cdot (f_1, f_2)) =\tau (g)\cdot m(f_1, f_2)
$$

for every $g\in G$ and all $f_1, f_2\in F$, the extension $m_*(\delta^*(\mathscr{E}_1\times \mathscr{E}_2))$ is a $\tau$-extension; we call it the product of the $\tau$-extensions $\mathscr{E}_1$ and $\mathscr{E}_2$ and denote it by $\mathscr{E}_1\mathscr{E}_2$. The class of this extension depends only on the classes of the extensions $\mathscr{E}_1$ and $\mathscr{E}_2$ (VIII, p. 288, Corollary 1 and VIII, p. 291, Corollary 1). So this gives a law of composition on Ex$_{\tau}(G,F)$.

#### Remark {#alg-viii-s16-n4-rem-1 .statement}

Let $\mathscr{E}_1= (Γ_1, \iota_1, \pi_1)$ and $\mathscr{E}_2= (Γ_2, \iota_2, \pi_2)$ be $\tau$-extensions of G by F. Let $\mathscr{E}_1\mathscr{E}_2= (Γ, \iota , \pi )$ be the product of these extensions. Following the example of VIII, p. 289, the construction gives a surjective group homomorphism from the fiber product $Γ_1\times_GΓ_2$ to Γ whose kernel is the image of the group homomorphism $f\mapsto (\iota_1(f), \iota_2(f)^{-1})$ from F to $Γ_1\times_GΓ_2$.

#### Proposition 4 {#alg-viii-s16-prop-4 .statement}

The product of $\tau$-extensions endows the set Ex$_{\tau}(G,F)$ with the structure of an abelian group. Its identity element is the class of the semitrivial extension $\mathscr{I}_{\tau}$. The inverse of the class of a $\tau$-extension $\mathscr{E}$ is the class of $s_*(\mathscr{E})$.

The associativity of the law follows from the commutativity of the diagrams

G $^{\delta}$ // $G\times GF\times F\times F^{m\times Id}/$/ $F\times F$

$_{\delta}$ Id$_{\times\delta}$ and Id$_{\times m}m$

$G\times G^{\delta\times Id}/$/ $G\times G\times GF\times F^m$ // F

and from Corollary 2 of VIII, p. 288; Corollary 2 of VIII, p. 291; and Proposition 3 of VIII, p. 292.

Let ∆$: F\rightarrow F\times F$ be the diagonal mapping $f\mapsto (f, f)$. Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension. Let $\widetilde{∆} : Γ\rightarrow Γ\times_GΓ$ be the group homomorphism given by $\gamma \mapsto (\gamma , \gamma )$. The following diagram commutes:

F $^{\iota}$ // Γ $^{\pi}$ // G

∆ $\widetilde{∆}$

$F\times F$ // $Γ\times_GΓ$ // G .

By Proposition 2 of VIII, p. 290, it follows that the $(\tau \times \tau )\circ \delta$-extension $\delta^*(\mathscr{E}\times \mathscr{E})$ is isomorphic to ∆$_*(\mathscr{E})$.

Denote by $c: F\rightarrow F$ the constant homomorphism $f\mapsto 1$. by Example 1 of VIII, p. 292, the fact that $\mathscr{I}_{\tau}$ is an identity element for this law of composition follows from the isomorphism from $\delta^*(\mathscr{E}\times \mathscr{E})$ to ∆$_*(\mathscr{E})$ and the commutative diagram

$F^{(Id_F\times c)\circ∆}/$/ $F\times F$

Id$_F$ $(c\times$Id$_F)\circ$∆ $m$

$_m$ &&//

$F\times F$ F . The last assertion follows from the commutative diagram

$F^{(Id_F\times s)\circ∆}/$/ $F\times F$

$$
c
$$

$(s\times$Id$_F)\circ$∆ $m$

$_m$ &&//

$F\times F$ F .

Let $\mathscr{E}_1= (Γ_1, \iota_1, \pi_1)$ and $\mathscr{E}_2= (Γ_2, \iota_2, \pi_2)$ be $\tau$-extensions. The group isomorphism $Γ_1\times Γ_2\rightarrow Γ_2\times Γ_1$ given by $(\gamma_1, \gamma_2)\mapsto (\gamma_2, \gamma_1)$ restricts to a group isomorphism $\sigma : Γ_1\times_GΓ_2\rightarrow Γ_2\times_GΓ_1$. Because of the relations

$$
\sigma (\iota_1(f), \iota_2(f)^{-1}) = (\iota_2(f^{-1}), \iota_1(f^{-1})^{-1})
$$

for $f\in F$, the group homomorphism $\sigma$ induces, by passing to the quotients, a morphism of $\tau$-extensions from $\mathscr{E}_1\mathscr{E}_2$ to $\mathscr{E}_2\mathscr{E}_1$. So the law of composition is commutative.

#### Proposition 5 {#alg-viii-s16-prop-5 .statement}

a) Let G and $G'$ be groups, and let F be an abelian group. Let $\tau : G\rightarrow$ Aut(F) and $u: G'\rightarrow G$ be group homomorphisms. The mapping $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau\circ u}(G',F)$ is a group homomorphism.

b) Let G be a group, and let F and $F'$ be abelian groups. Let $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$')$, and $v: F\rightarrow F'$ be group homomorphisms such that

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

for $g\in G$ and $f\in F$. The mapping $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ is a group homomorphism.

This follows from the commutativity of the diagrams

$G_'^{\delta}$ // $G_'\times G_'F\times F^m$ // F

$_uu_{\times u}$ and $v_{\times v}v$

G $^{\delta}$ // $G\times GF_'\times F_'^m$ // $F_'$.

### 5. Cohomological Description

Let G be a group, let F be an abelian group, and let $\tau : G\rightarrow$ Aut(F) be a group homomorphism. For any $g\in G$ and $f\in F$, we also write $^gf$ for $\tau (g)\cdot f$. A 2-cocycle of G with values in F is a mapping $c: G\times G\rightarrow F$ such that for every $(g_1, g_2, g_3)\in G\times G\times G$, we have

$$
g_{_1}c(g_2, g_3)c(g_1, g_2g_3) =c(g_1, g_2)c(g_1g_2, g_3) \tag{7}
$$

Since F is commutative, the set of 2-cocycles is a subgroup of the group of mappings from $G\times G$ to F; we denote it by $Z^2(G,F)$. We denote the group of mappings from G to F by $C^1(G,F)$. For every $h\in C^1(G,F)$ and $(g_1, g_2)\in G\times G$, set

$$
(\partial h)(g_1, g_2) =^{g_1}h(g_2)h(g_1g_2)^{-1}h(g_1) \tag{8}
$$

A simple calculation shows that the mapping $\partial h: G\times G\rightarrow F$ is a 2-cocycle. The mapping $\partial : C^1(G,F)\rightarrow Z^2(G,F)$ is a group homomorphism. For any $h\in C^1(G,F)$, the 2-cocycle $\partial h$ is called a 2-coboundary. The group $Z^2(G,F)/\partial (C^1(G,F))$ is denoted by $H^2(G,F)$ and is called the second cohomology group of G with coefficients in F.

$*$The notation above agrees with that of X, §6, n$_o8$, p. 112 concerning group cohomology.$*$

Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension. Let $\sigma$ be a section of the surjective mapping $\pi ($Set Theory, II, §3, No. 8, p. 86), that is, a mapping from G to Γ such that $\pi (\sigma (g)) =g$ for every $g$ in G. For every $g_1, g_2\in G$, $\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}$ belongs to Ker($\pi )$, so that there exists a unique mapping $c_{\sigma}: G\times G\rightarrow F$ such that

$$
\iota (c_{\sigma}(g_1, g_2)) =\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1} \tag{9}
$$

for all $g_1, g_2\in G$. The mapping $c_{\sigma}$ is constant with value 1 if and only if $\sigma$ is a group homomorphism.

#### Proposition 6 {#alg-viii-s16-prop-6 .statement}

The mapping $c_{\sigma}$ is an element of the group $Z^2(G,F)$, and its class in the cohomology group $H^2(G,F)$ depends only on the class of the $\tau$-extension $\mathscr{E}$.

We say that the mapping $c_{\sigma}$ is the 2-cocycle associated with $\sigma$ and that its cohomology class in $H^2(G,F)$ is the cohomology class of the $\tau$-extension $\mathscr{E}$.

Let us first verify that $c_{\sigma}$ satisfies the cocycle condition. Let $g_1,g_2$, and $g_3$ be elements of G. Using formula (1) of VIII, p. 285 and (9), we obtain the relations

$$
\iota (^{g_1}c_{\sigma}(g_2, g_3)c_{\sigma}(g_1, g_2g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_2g_3)^{-1}\sigma (g_1)^{-1}\sigma (g_1)\sigma (g_2g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

and

$$
\iota (c_{\sigma}(g_1, g_2)c_{\sigma}(g_1g_2, g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}\sigma (g_1g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

The mapping $c_{\sigma}$ is therefore an element of $Z^2(G,F)$.

Let us now prove that the image of $c_{\sigma}$ in $H^2(G,F)$ is independent of the chosen section $\sigma$. Let $\sigma$ and $\sigma '$ be such sections. For every element $g$ of G, there exists a unique element $a_g$ of F such that $\sigma '(g) =\iota (a_g)\sigma (g)$. Let $g_1$ and $g_2$ be elements of G. Using the definition (9), we obtain the equalities

$$
\iota (c_{\sigma'}(g_1, g_2)) =\sigma '(g_1)\sigma '(g_2)\sigma '(g_1g_2)^{-1}
$$

(10) $=\iota (a_{g_1})\sigma (g_1)\iota (a_{g_2})\sigma (g_2)\sigma (g_1g_2)^{-1}\iota (a_{g_1g_2})^{-1}$

$$
=\iota (a_{g_1})\iota (^{g_1}a_{g_2})\iota (c_{\sigma}(g_1, g_2))\iota (a_{g_1g_2})^{-1}
$$

Since the group F is commutative, we have the relations

$$
c_{\sigma'}(g_1, g_2)c_{\sigma}(g_1, g_2)^{-1}= (^{g_1}a_{g_2})a^-_{g_1}^1_{g_2}a_{g_1}= (\partial a)(g_1, g_2) \tag{11}
$$

as follows from (8). This proves that the classes of $c_{\sigma'}$ and $c_{\sigma}$ in $H^2(G,F)$ coincide.

Finally, let $\mathscr{E}= (Γ, \iota , \pi )$ and $\mathscr{E}'= (Γ', \iota ', \pi ')$ be isomorphic $\tau$-extensions, let $u:\mathscr{E}\rightarrow \mathscr{E}'$ be a morphism of $\tau$-extensions, and let $\sigma$ be a section of the mapping $\pi$. The mapping $u\circ \sigma$ is a section of the mapping $\pi '$, and we have $c_{\sigma}=c_{u\circ\sigma}$. The class of $c_{\sigma}$ in $H^2(G,F)$ therefore depends only on the class of $\mathscr{E}$ in Ex$_{\tau}(G,F)$.

We denote by $Θ_{\tau}$ : Ex$_{\tau}(G,F)\rightarrow H^2(G,F)$, or more simply Θ, the mapping that sends the class of a $\tau$-extension $(Γ, \iota , \pi )$ to the class of the 2-cocycle $c_{\sigma}$, where $\sigma$ is a section of the surjection $\pi$.

#### Theorem 1 {#alg-viii-s16-thm-1 .statement}

The mapping Θ is a group isomorphism from Ex$_{\tau}(G,F)$ to $H^2(G,F)$.

Let us first prove that Θ is a group homomorphism. Let $\mathscr{E}= (Γ, \iota , \pi )$ and $\mathscr{E}'= (Γ', \iota ', \pi ')$ be $\tau$-extensions, and let $\sigma$ (resp. $\sigma ')$ be a section of the mapping $\pi$ (resp. $\pi ')$. We denote by $\mathscr{E} \mathscr{E}'= (Γ'', \iota '', \pi '')$ the product of the $\tau$-extensions $\mathscr{E}$ and $\mathscr{E}'$. We denote by $[\gamma , \gamma ']$ the image in $Γ''$ of an element $(\gamma , \gamma ')$ of $Γ\times_GΓ'$ by the surjective homomorphism from the remark of VIII, p. 293. The mapping from G to $Γ''$ that sends an element $g$ to $[\sigma (g), \sigma '(g)]$ is a section $\sigma ''$ of the mapping $\pi ''$. Let $g_1$ and $g_2$ be elements of G. We have the relations

$$
\iota ''(c_{\sigma''}(g_1, g_2)) =\sigma ''(g_1)\sigma ''(g_2)\sigma ''(g_1g_2)^{-1}
$$

$$
= [\iota (c_{\sigma}(g_1, g_2)), \iota '(c_{\sigma'}(g_1, g_2)]
$$

$$
=\iota ''(c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2))
$$

We therefore have $c_{\sigma''}(g_1, g_2) =c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2)$.

Let us prove that the mapping Θ is injective. Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension, and let $\sigma$ be a section of the mapping $\pi$ such that the image of $c_{\sigma}$ in $H^2(G,F)$ is trivial. There exists a mapping $a: G\rightarrow F$ such that

$$
c_{\sigma}(g_1, g_2) = (^{g_1}a(g_2))a(g_1g_2)^{-1}a(g_1)
$$

for all $g_1, g_2\in G$. We then define $\sigma ': G\rightarrow Γ$ by

$$
\sigma '(g) =\iota (a(g)^{-1})\sigma (g)
$$

for $g\in G$. Using (11), we obtain that $c_{\sigma'}$ is constant with value 1; consequently, $\sigma '$ is a group homomorphism, which proves that the $\tau$-extension $\mathscr{E}$ is semitrivial (I, §6, No. 1, p. 67, Proposition 4).

Let us prove that the mapping Θ is surjective. Let $c$ be an element of $Z^2(G,F)$. We endow the set $Γ = F\times G$ with the following law of composition: (12) $(f_1, g_1)(f_2, g_2) =f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2$ for all $f_1, f_2\in F$ and $g_1, g_2\in G$. We have the relations

$$
(f_1, g_1) ((f_2, g_2)(f_3, g_3)) = (f_1, g_1)f_2(^{g_2}f_3)c(g_2, g_3), g_2g_3
$$

= $f_1(^{g_1}f_2)(^{g_1g_2}f_3)(^{g_1}c(g_2, g_3))c(g_1, g_2g_3), g_1g_2g_3$ and

$$
((f_1, g_1)(f_2, g_2)) (f_3, g_3) =f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2(f_3, g_3)
$$

= $f_1(^{g_1}f_2)(^{g_1g_2}f_3)c(g_1, g_2)c(g_1g_2, g_3), g_1g_2g_3$ for all $f_1, f_2, f_3\in F$ and $g_1,g_2, g_3\in G$. It follows that this law is associative because $c$ is a 2-cocycle. For every $(f, g)\in Γ$, we have

$$
(f, g)(c(e, e)^{-1}, e) = (f(^gc(e, e)^{-1})c(g, e), g)
$$

Now, it follows from the definition of a 2-cocycle that $c(g, e) =^gc(e, e)$, from which we deduce that $(f, g)(c(e, e)^{-1}, e) = (f, g)$. We prove likewise that

$$
(c(e, e)^{-1}, e)(f, g) = (f c(e, e)^{-1}c(e, g), g) = (f, g)
$$

The law of composition defined by (12) therefore has identity element $(c(e, e)^{-1}, e)$, and every element $(f, g)$ of Γ is invertible, with inverse

$$
(^{g^{-1}}(f^{-1}c(e, e)^{-1}c(g, g^{-1})^{-1}), g^{-1})
$$

So we have endowed Γ with a group structure. Let us denote by $\iota : F\rightarrow G$ the mapping that sends $f$ to $(c(e, e)^{-1}f, e)$, by $\pi : Γ\rightarrow G$ the second projection, and by $\sigma$ the mapping $g\mapsto (1, g)$. The mappings $\iota$ and $\pi$ are group homomorphisms, so the triple $\mathscr{E}= (Γ, \iota , \pi )$ is a $\tau$-extension, $\sigma$ is a section of the mapping $\pi$, and the associated cocycle $c_{\sigma}$ is equal to $c$ because $\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}= (1, g_1)(1, g_2)(1, g_1g_2)^{-1}= (c(g_1, g_2), g_1g_2)(1, g_1g_2)^{-1}$

$$
= (c(g_1, g_2)c(e, g_1g_2)^{-1}, e) = (c(e, e)^{-1}c(g_1, g_2), e)
$$

for $g_1, g_2\in G$. **Remark.** — Let G be a group, let F and $F'$ be abelian groups, let $\tau$ (resp. $\tau ')$ be a group homomorphism from G to the automorphism group of F (resp. $F')$, and let $v: F\rightarrow F'$ be a group morphism such that

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{13}
$$

for $g\in G$ and $f\in F$. Let $\alpha$ be an element of Ex$_{\tau}(G,F)$. If the cocycle $c$ represents $Θ(\alpha )$, then $v\circ c$ represents $Θ(v_*(\alpha ))\in H^2(G,F')$.

### 6. Restriction and Corestriction

Let G and $G'$ be groups, F be an abelian group, and $\tau$ be a homomorphism from G to the automorphism group of F. Let $u: G'\rightarrow G$ be a group homomorphism. We write $\tau '=\tau \circ u$.

If $\psi : G\times G\rightarrow F$ is a 2-cocycle of G with values in F, then the mapping $\psi \circ (u\times u)$ from $G'\times G'$ to F given by $(g_1, g_2)\mapsto \psi (u(g_1), u(g_2))$ is a 2-cocycle of $G'$ with values in F, and the mapping $\psi \mapsto \psi \circ (u\times u)$ from $Z^2(G,F)$ to $Z^2(G',F)$ induces a group homomorphism $u^*: H^2(G,F)\rightarrow H^2(G',F)$. For any $\lambda \in H^2(G,F)$, the element $u^*(\lambda )$ is called the inverse image of $\lambda$ by $u$. When $G'$ is a subgroup of G and $u: G'\rightarrow G$ is the canonical injection, the homomorphism $u^*$ is called the restriction homomorphism from G to $G'$; we denote it by Res$^G_{G'}$. When G is a quotient of $G'$ and $u: G'\rightarrow G$ is the canonical surjection, the homomorphism $u^*$ is called the inflation homomorphism from G to $G'$.

#### Proposition 7 {#alg-viii-s16-prop-7 .statement}

In the notation from above, the following diagram commutes:

Ex$_{\tau}(G,F)^{u^*}$ // Ex$_{\tau}(G_',F)$

$Θ_{\tau}Θ_{\tau'}$

$H_2(G,F)^{u^*}$ // $H_2(G_',F)$.

Let H be a subgroup of G of finite index. Let $s$ be a section of the canonical surjection from G to $H\backslash G$. We denote by $(g, x)\mapsto x\cdot g$ the right action of G on $H\backslash G$ induced by the right action of G on itself by multiplication. Note that for every $x\in H\backslash G$ and $g\in G$, the element $s(x)gs(x\cdot g)^{-1}$ belongs to H. For any mapping $c: H\times H\rightarrow F$, we can therefore define a mapping $\widetilde{c}_s: G\times G\rightarrow F$ by the relation

$$
\widetilde{c}_s(g_1, g_2) =_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}
$$

for $g_1,g_2\in G$. The mapping $c\mapsto \widetilde{c}_s$ is a group homomorphism from $F^{H\times H}$ to $F^{G\times G}$.

#### Lemma 4 {#alg-viii-s16-lem-4 .statement}

If $c: H\times H\rightarrow F$ is a 2-cocycle of H with values in F, then $\widetilde{c}_s$ is a 2-cocycle of G with values in F.

Let $g_1,g_2$, and $g_3$ be elements of G. For every $i\in  \{1,2,3\}$, we define a mapping $h_i: H\backslash G\rightarrow H$ by the relation

$$
h_i(x) =s(x\cdot g_1\cdots g_{i-1})g_is(x\cdot g_1\cdots g_i)^{-1}
$$

for $x\in H\backslash G$. Note that

$$
h_1(x)h_2(x) =s(x)g_1g_2s(x\cdot g_1g_2)^{-1}
$$

$$
h_2(x)h_3(x) =s(x\cdot g_1)g_2g_3s(x\cdot g_1g_2g_3)^{-1}
$$

for $x\in H\backslash G$. We then have the relations

$$
^{g_1}\widetilde{c}_s(g_2, g_3)\widetilde{c}_s(g_1g_2, g_3)^{-1}\widetilde{c}_s(g_1, g_2g_3)\widetilde{c}_s(g_1, g_2)^{-1}
$$

$$
=_{x\in}\prod_{H\backslash G}^{g_1s(x)^{-1}}c s(x)g_2s(x\cdot g_2)^{-1}, s(x\cdot g_2)g_3s(x\cdot g_2g_3)^{-1}
$$

$$
\times_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c(h_1(x)h_2(x), h_3(x))^{-1}
$$

$$
\times c(h_1(x), h_2(x)h_3(x))c(h_1(x), h_2(x))^{-1}
$$

$$
=_{x\in}\prod_{H\backslash G}^{s(x\cdot g_1^{-1})^{-1}h_1(x\cdot g^-_1^1)}c(h_2(x\cdot g_1^{-1}), h_3(x\cdot g_1^{-1}))
$$

$$
\times_{x\in}\prod_{H\backslash G}^{s(x)^{-1}h_1(x)}c(h_2(x), h_3(x))^{-1}
$$

$$
= 1
$$

where the second equality follows from the fact that $c$ is a 2-cocycle.

#### Lemma 5 {#alg-viii-s16-lem-5 .statement}

If $c$ is a 2-coboundary, then so is $\widetilde{c}_s$.

Let $t: H\rightarrow F$ be a mapping such that $c=\partial t$. Let $\widetilde{t}_s: G\rightarrow F$ be the mapping defined by

$$
\widetilde{t}_s(g) =_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}t(s(x)gs(x\cdot g)^{-1})
$$

for $g\in G$. It suffices to prove that $\widetilde{c}_s=\partial \widetilde{t}_s$, which follows from the relations $\widetilde{c}_s(g_1, g_2) =\prod^{s(x)^{-1}s(x)g_1s(x\cdot g_1)^{-1}}t(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

$$
\times^{x\in}_x^H_{\in}\prod^{\backslash}_H^G_{\backslash G}^{s(x)^{-1}}t(s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}t(s(x)g_1s(x\cdot g_1)^{-1})
$$

$$
=\partial \widetilde{t}_s(g_1, g_2)
$$

for $g_1, g_2\in G$.

#### Lemma 6 {#alg-viii-s16-lem-6 .statement}

Let $c$ be a 2-cocycle of H with values in F. The image of $\widetilde{c}_s$ in the group $H^2(G,F)$ does not depend on the choice of the section $s$.

Let $s'$ be a section of the canonical surjection from G to $H\backslash G$. Let $h: H\backslash G\rightarrow H$ be the mapping characterized by the relation

$$
s'(x) =h(x)s(x)
$$

for $x\in H\backslash G$. The 2-cocycle $\widetilde{c}_{s'}$ is then given by the relations

$$
\widetilde{c}_{s'}(g_1, g_2)
$$

= $\prod^{s(x)^{-1}h(x)^{-1}}c h(x)s(x)g_1s'(x\cdot g_1)^{-1}, s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$

$$
=^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_G^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}
$$

$\prod s(x)_{-1}-1''-1-1$

$\times c h(x), s(x)g_1g_2s(x\cdot g_1g_2)$

$x\in H\backslash G$

$$
\times c h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}
$$

$=_{x\in}\prod_{H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$

$$
\times_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}
$$

$\prod s(x)_{-1}-1-1-1$

$\times c s(x)g_1s(x\cdot g_1), h(x\cdot g_1)$ $\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_G^{s(x)^{-1}}c h(x)^{-1}, s'(x)g_1g_2s'(x\cdot g_1g_2)^{-1-1}$

$$
\times c h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}
$$

$=_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$

$\prod s(x)_{-1}-1-1-1$

$\times c s(x)g_1s(x\cdot g_1), h(x\cdot g_1)$ $\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_G^{g_1s(x)^{-1}}c h(x)^{-1}, h(x)s(x)g_2s'(x\cdot g_2)^{-1}$

$\prod s(x)^-_1-1''-1-1$

$\times c h(x), s(x)g_1g_2s(x\cdot g_1g_2)$

$x\in H\backslash G$

$$
\times c h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}
$$

for all $g_1, g_2\in G$. The first equality comes from the cocycle relation (VIII, p. 295, formula (7)) applied to the elements

$h(x)^{-1},h(x)s(x)g_1s'(x\cdot g_1)^{-1}$, and $s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$; the second is obtained by applying the cocycle relation to the elements $s(x)g_1s(x\cdot g_1)^{-1},h(x\cdot g_1)^{-1}$, and $h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$; and the last simply uses the fact that the mapping $x\mapsto x\cdot g_1$ is a permutation of $H\backslash G$.

The last two lines of the obtained expression correspond to a 2-coboundary. We find that $\widetilde{c}_{s'}$ has the same class in $H^2(G,F)$ as the cocycle whose value in $(g_1, g_2)\in G^2$ is given by the expression $_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}h(x\cdot g_1g_2)^{-1}$

$\prod s(x)_{-1}-1-1-1$

$\times c s(x)g_1s(x\cdot g_1), h(x\cdot g_1)$

$x\in H\backslash G$

$=_{x\in}\prod_{H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1-1}$

$$
\times \prod^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}
$$

$$
\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_G^{s(x)^{-1}}c s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1}
$$

$-1-1-1$

$\times c s(x)g_1s(x\cdot g_1), h(x\cdot g_1)$ $=_{x\in}\prod_{H\backslash G}^{s(x)^{-1}}c s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$

$\prod gs(x)_{-1}-1-1-1$

$\times$ 1 $c s(x)g_2s(x\cdot g_2), h(x\cdot g_2)$

$$
\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_G^{s(x)^{-1}}c s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1}
$$

$$
\times c s(x)g_1s(x\cdot g_1)^{-1}, h(x\cdot g_1)^{-1-1}
$$

where the first equality follows from the cocycle relation applied to the elements

$s(x)g_1s(x\cdot g_1)^{-1},s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$, and $h(x\cdot g_1g_2)^{-1}$. The last two lines of the obtained expression correspond to a 2-coboundary. We find that the class of $\widetilde{c}_{s'}$ coincides with that of $\widetilde{c}_s$.

We have constructed a homomorphism from the group $H^2(H,F)$ to the group $H^2(G,F)$, which we call the corestriction homomorphism from H to G and denote by Cor$^G_H$.

#### Proposition 8 {#alg-viii-s16-prop-8 .statement}

Let H be a subgroup of G of finite index. The endomorphism Cor$^G_H\circ$ Res$^G_H$ of the group $H^2(G,F)$ coincides with multiplication by the index (G : H).

Let $\alpha$ be an element of $H^2(G,F)$, and let $c$ be an element of $Z^2(G,F)$ representing $\alpha$. The element Cor$^G_H\circ$ Res$^G_H(\alpha )$ is the class of the cocycle whose value in $(g_1, g_2)\in G^2$ is given by the expression

$$
\prod^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
^x=^{\in H\backslash}\prod^Gc(g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times^{x\in H}\prod^{\backslash G}c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1})
$$

= $\prod^{x\in H\backslash gG_1}c(s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

$$
\times^{x\in H}\prod^{\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_Gc(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1})
$$

= $\prod c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}$

$$
\times^{x\in H}\prod^{\backslash Gg_1}c(s(x)^{-1}, s(x)g_2s(xg_2)^{-1})
$$

$$
\times^x_x^{\in}_{\in}\prod^H_H^{\backslash}_{\backslash}^G_Gc(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1})
$$

The first equality comes from the cocycle relation (VIII, p. 295, formula (7)) applied to the elements

$s(x)^{-1},s(x)g_1s(x\cdot g_1)^{-1}$, and $s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$; the second is obtained by applying the cocycle relation to the elements

$g_1,s(x\cdot g_1)^{-1}$, and $s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$.

By removing a coboundary, we obtain that Cor$^G_H\circ$ Res$^G_H(\alpha )$ is the class of the cocycle whose value in $(g_1, g_2)\in G^2$ is given by the expression

$$
\prod c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
^x=^{\in H\backslash}\prod^{Gg_1}c(g_2, s(x\cdot g_1g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, g_2)
$$

$$
\times^{x\in H}\prod^{\backslash G}c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
=_{x\in}\prod^x_H^{\in}_{\backslash}^H_G^{\backslash gG_1}c(g_2, s(x\cdot g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times c(g_1, g_2)^{(G:H)}
$$

which proves the result.

### 7. Galois Algebras

Let K be a commutative field. If E is a K-algebra, then we denote its automorphism group by Aut$_K(E)$. If E is a Galois extension of the field K, then the group Aut$_K(E)$ is simply the Galois group Gal(E$/K)$ (V, §10, No. 2, p. 58).

Let G be a group. $A (K,G)$-algebra is a K-algebra E endowed with a group homomorphism $\lambda : G\rightarrow$ Aut$_K(E)$. The homomorphism $\lambda$ then endows E with the structure of a group with operators in G as well as the structure of a left K[G]-module with external law given by

$$
(\sum_{g\in G}µ_ggx=_g\sum_{\in G}µ_g\lambda (g).x \tag{14}
$$

for every $x\in L$ and every element $(µ_g)_{g\in G}$ of K[G]. A morphism of $(K,G)$-algebras is a morphism of algebras that is also a morphism of groups with operators.

For every family $(E_i)_{i\in I}$ of $(K$, G)-algebras, the product K-algebra $\prod_{i\in I}E_i$ endowed with its structure of a product group with operators is a $(K$, G)-algebra.

If E is a $(K$, G)-algebra, then the set $E^G$ of elements of E invariant under G is a subalgebra of E.

Let E be a $(K$, G)-algebra, where G acts by $\lambda : G\rightarrow$ Aut$_K(E)$. If $K'$ is an extension of K, then for any $g\in G$, let $\lambda '(g)$ be the automorphism Id$_{K'}\otimes \lambda (g)$ of the $K'$-algebra $L_{(K')}$. Then $\lambda ':g\mapsto \lambda '(g)$ endows $L_{(K')}$ with the structure of a $(K'$, G)-algebra.

Given a group H and H-sets X and Y, we denote by $\mathscr{F}_H(X,Y)$ the set of morphisms of H-sets from X to Y. It is the set of mappings $f: X\rightarrow Y$ such that $f(hx) =hf(x)$ for every $h\in H$ and $x\in X$.

Let G be a group with identity element $e$, let H be a subgroup of G, and let E be a $(K$, H)-algebra. The $(K,G)$-algebra deduced from E by coinduction from H to G, denoted by Coind$^G_H$(E), is the K-algebra $\mathscr{F}_H(G,E)$ endowed with the action of G given by the homomorphism $\lambda$ from G to Aut$_K$(Coind$^G_H(E))$ defined by

$$
(\lambda (g)\cdot f)(g') =f(g'g) \tag{15}
$$

for $f\in$ Coind$^G_H(E)$ and $g, g'\in G$.

#### Lemma 7 {#alg-viii-s16-lem-7 .statement}

a) Let S be a subset of G such that every element of G can be written uniquely as $hs$ with $h\in H$ and $s\in S$. Then the mapping that sends $f$ to $(f(s))_{s\in S}$ is an isomorphism from the K-algebra Coind$^G_H(E)$ to the K-algebra $\mathscr{F}(S,E)$ of mappings from S to E.

b) The algebra Coind$^G_H(E)$ has finite degree over K if and only if E has finite degree over K and the index of H in G is finite. In this case, we have the formula

[Coind$^G_H(E) : K] = (G : H)[E : K]$.

c) Let $E^H$ be the algebra of invariants of the group H in E and Coind$^G_H(E)^G$ that of the group G in Coind$^G_H(E)$. The mapping $f\mapsto f(e)$ from Coind$^G_H(E)$ to E restricts to an algebra isomorphism from Coind$^G_H(E)^G$ to $E^H$.

Assertion a) follows from the definitions and implies b). By (15), a mapping from G to E is an element of Coind$^G_H(E)$ invariant under G if and only if it is constant with value an element of E invariant under H.

#### Remark 1 {#alg-viii-s16-n7-rem-1 .statement}

Let G be a group, H a subgroup of G, and N a subgroup of H. Let E be a $(K$, N)-algebra. Let $\alpha$ be an element of $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$. We have the relation

$$
\alpha (g)(nh) =n(\alpha (g)(h)) \tag{16}
$$

for every $g\in G,h\in H$, and $n\in N$ and the relations

$$
\alpha (hg)(h') = (h\alpha (g))(h') =\alpha (g)(h'h) \tag{17}
$$

for all $h, h'\in H$ and every $g\in G$. Consequently, $\alpha (ng)(e) =\alpha (g)(n) =$ $n(\alpha (g)(e))$ for every $g\in G$ and $n\in N$. We can therefore consider the mapping

$$
\psi :\mathscr{F}_H(G,\mathscr{F}_N(H,E))\rightarrow \mathscr{F}_N(G,E)
$$

defined by the relation $\psi (\alpha )(g) =\alpha (g)(e)$ for $\alpha$ in $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$ and $g$ in G. The mapping $\psi$ is an algebra isomorphism from Coind$^G_H$(Coind$^H_N(E))$ to Coind$^G_N(E)$ whose inverse sends an element $\beta$ from $\mathscr{F}_N(G,E)$ to the mapping $\alpha$ defined by the relation $\alpha (g)(h) =\beta (hg)$ for $g\in G$ and $h\in H$.

We now suppose given a finite group G and a reduced (V, §6, No. 6, p. 32) commutative K-algebra L of finite degree endowed with an action of G given by a homomorphism $\lambda$ from G to Aut$_K(L)$. For $x\in L$ and $g\in G$, we denote by $g\cdot x$ the transform of $x$ under the automorphism $\lambda (g)$ of L. Let $\mathscr{S}$ be the set of maximal ideals of L; we denote by $g\cdot \mathfrak{m}$ the transform of an element $\mathfrak{m}$ of $\mathscr{S}$ under the automorphism $\lambda (g)$ of L. It is an element of $\mathscr{S}$. For every $\mathfrak{m}$ in $\mathscr{S}$, the field $L/\mathfrak{m}$ is a finite extension of K. We write $\pi_{\mathfrak{m}}: L\rightarrow L/\mathfrak{m}$ for the projection and denote by $G_{\mathfrak{m}}$ the stabilizer of $\mathfrak{m}$ in G, that is, the set of $g\in G$ such that $g\cdot \mathfrak{m}=\mathfrak{m}$. The K-algebra $L/\mathfrak{m}$ is endowed with an action of $G_{\mathfrak{m}}$ through the homomorphism $\lambda_{\mathfrak{m}}$ from $G_{\mathfrak{m}}$ to Aut$_K(L/\mathfrak{m})$ that sends an element $h$ of $G_{\mathfrak{m}}$ to the automorphism of $L/\mathfrak{m}$ deduced from $\lambda (h)$ when passing to the quotients.

Let $\mathscr{O}$ be the set of orbits of G in $\mathscr{S}$. Given an orbit $\sigma \in \mathscr{O}$, set $\mathfrak{a}_{\sigma}=\bigcap_{\mathfrak{m}\in\sigma}\mathfrak{m}$ and $L_{\sigma}= L/\mathfrak{a}_{\sigma}$. Since $\mathfrak{a}_{\sigma}$ is invariant under G, by passing to the quotients, the action of G on L defines a homomorphism $\lambda_{\sigma}$ from G to Aut$_K(L_{\sigma})$. Finally, denote by $\pi_{\sigma}$ the canonical mapping from L to $L_{\sigma}$. **Lemma 8.** — a) For every $g\in G,\sigma \in \mathscr{O}$, and $\mathfrak{m}\in \sigma$, we have

$[L_{\sigma}: K] =$ Card($\sigma )[L/\mathfrak{m}: K]$.

b) The mapping $\pi :x\mapsto (\pi_{\sigma}(x))_{\sigma\in\mathscr{O}}$ is an isomorphism of $(K,G)$-algebras from L to $\prod_{\sigma\in\mathscr{O}}L_{\sigma}$.

c) Denote by $L^G($resp. $L^G_{\sigma})$ the subalgebra of L (resp. $L_{\sigma})$ of elements invariant under the action of G. Then $\pi$ induces an isomorphism from $L^G$ to $\prod_{\sigma\in\mathscr{O}}L^G_{\sigma}$.

Since the algebra L is reduced and of finite degree, the intersection of the maximal ideals of L is reduced to 0 (VIII, p. 173, Corollary 2). Moreover, if $\mathfrak{m}$ and $\mathfrak{m}'$ are two distinct maximal ideals of L, then we have $\mathfrak{m}+\mathfrak{m}'= L$. By Proposition 10 of I, §8, No. 11, p. 110, the canonical mapping from L to $\prod_{\mathfrak{m}\in\mathscr{S}}L/\mathfrak{m}$ is an isomorphism, as is the canonical mapping from $L/\mathfrak{a}_{\sigma}$ to $\prod_{\mathfrak{m}\in\sigma}L/\mathfrak{m}$ for every $\sigma \in \mathscr{O}$. Assertion a) follows. Since $\mathscr{O}$ is a partition of $\mathscr{S}$, assertion b) follows; assertion c) is an immediate consequence of b).

Let us now fix an orbit $\sigma \in \mathscr{O}$ and an element $\mathfrak{m}$ of $\sigma$. Set $F_{\mathfrak{m}}$ = Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$, and denote by $\lambda_{F_{\mathfrak{m}}}$ the action of G on $F_{\mathfrak{m}}$. For any $x\in L$, denote by $x$ the mapping from G to $L/\mathfrak{m}$ that sends $g$ to $\pi_{\mathfrak{m}}(gx)$. By formula (15) of VIII, p. 305 and the definition of the action of $G_{\mathfrak{m}}$ on $L/\mathfrak{m}$, it is immediate that $x$ belongs to $F_{\mathfrak{m}}$, and the mapping $u:x\mapsto x$ from L to $F_{\mathfrak{m}}$ satisfies $\lambda_{F_{\mathfrak{m}}}(g)\circ u=u\circ \lambda (g)$ for $g\in G$. In other words, $u$ is a morphism of $(K$, G)-algebras.

#### Lemma 9 {#alg-viii-s16-lem-9 .statement}

The morphism $u$ is surjective with kernel $\mathfrak{a}_{\sigma}$. The mapping deduced from $u$ by passing to the quotient is an isomorphism of $(K,G)$-algebras from $L_{\sigma}$ to $F_{\mathfrak{m}}$.

Since the kernel of $\pi_{\mathfrak{m}}$ is equal to $\mathfrak{m}$, that of $u$ is equal to $\bigcap_{g\in G}g^{-1}.\mathfrak{m}=\mathfrak{a}_{\sigma}$. To prove that $u$ is surjective, it suffices to prove that the vector spaces $L_{\sigma}=$ $L/\mathfrak{a}_{\sigma}$ and $F_{\mathfrak{m}}$ have the same dimension over K. Now, all ideals $g\cdot \mathfrak{m}$ have the same codimension in L, and, by Lemma 8, a),

$[L_{\sigma}: K] =$ Card($\sigma ).[L/\mathfrak{m}: K]$.

Moreover, by Lemma 7, b), we have

$$
[F_{\mathfrak{m}}: K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]
$$

Since we have Card($\sigma ) = (G : G_{\mathfrak{m}})$, we have proved the equality $[L_{\sigma}: K] =$ $[F_{\mathfrak{m}}: K]$.

We now suppose, furthermore, that the homomorphism $\lambda$ from G to Aut$_K(L)$ is injective. We identify K with its image in L through the mapping $\xi \mapsto \xi \cdot 1$. Let Ω be an algebraically closed extension of K. The set $\mathscr{F}(G,Ω)$ of mappings from G to Ω coincides with the coinduced $(Ω$, G)-algebra Coind$^G_{\{e\}}(Ω)$. It is a free Ω[G]-module of rank 1. Let $\mathscr{H}$ be the set of K-algebra homomorphisms from L to Ω. We define a right action of G on $\mathscr{H}$ by $(g, \chi )\mapsto \chi \circ \lambda (g)$. The Ω-algebra $\mathscr{F}(\mathscr{H},Ω)$ is then endowed with the structure of an $(Ω$, G)-algebra deduced from the right action of G on $\mathscr{H}$.

#### Lemma 10 {#alg-viii-s16-lem-10 .statement}

Let L be a $(K,G)$-algebra that is étale over K. The mapping $\psi$ from $L_{(Ω)}$ to $\mathscr{F}(\mathscr{H},Ω)$ characterized by the relation

$$
\psi (\xi \otimes x) = (\xi \chi (x))_{\chi\in\mathscr{H}}
$$

is an isomorphism of $(K,G)$-algebras.

Since L is étale, the mapping $\psi$ is an isomorphism of Ω-algebras (V, §6, No. 3, p. 30, Proposition 2 and V, §6, No. 3, p. 29, Proposition 1, c)). We have the relations

$\psi$((Id $\otimes \lambda (g))(\xi \otimes x)) = (\xi (\chi \circ \lambda (g))(x))_{\chi\in\mathscr{H}}$

for $\xi \in Ω,x\in L$, and $g\in G$. So $\psi$ is a morphism of $(Ω$, G)-algebras.

#### Theorem 2 {#alg-viii-s16-thm-2 .statement}

Let G be a finite group, and let L be a commutative K-algebra of finite degree endowed with an action of G given by an injective homomorphism $\lambda$ from G to Aut$_K(L)$. The following properties are then equivalent:

(i) There exist a subgroup H of G, a Galois extension E of K of finite degree, an isomorphism from H to Gal(E$/K)$, and an isomorphism of $(K,G)$-algebras from L to Coind$^G_H(E)$.

(ii) The algebra L is étale, and $\mathscr{H}$ is a homogeneous principal G-set (I, §5, No. 6, p. 60, Definition 7).

(iii) There exists an isomorphism of $(Ω,G)$-algebras $\psi : L_{(Ω)}\rightarrow \mathscr{F}(G,Ω)$; in other words, for every $g\in G$, the automorphism $\psi \circ \lambda (g)_{(Ω)}\circ \psi^{-1}$ of $Ω^G$ is equal to the automorphism

$$
(x_h)_{h\in G}\longmapsto (x_{hg})_{h\in G}
$$

(iv) The algebra L is reduced, and L is a free K[G]-module of rank 1.

(v) The algebra L is reduced, we have Card(G) = [L : K], and K is the subring of L of elements invariant under the action of G.

(vi) The algebra L is reduced, the group G acts transitively on the set of maximal ideals of L, and, for every maximal ideal $\mathfrak{m}$ of L, the stabilizer $G_{\mathfrak{m}}$ of $\mathfrak{m}$ in G acts faithfully on $L/\mathfrak{m}$ and admits K as subfield of invariants.

(i)$\Rightarrow$(ii): Let E be a Galois extension of K of finite degree and $\tau$ an isomorphism from H to Aut$_K(E)$. Let S be a system of representatives of the right cosets of G modulo H. The K-algebra F = Coind$^G_H(E)$ is isomorphic to $\mathscr{F}(S,E)$ (Lemma 7, a)); it is therefore étale. We denote by $\lambda_F$ the action of G on F. Furthermore, let $\psi$ be a K-algebra homomorphism from E to Ω, and let $\chi_0$ be the homomorphism $f\mapsto \psi (f(e))$ from F to Ω. Let $g\in G$ be such that we have $\chi_0\circ \lambda_F(g) =\chi_0$; since $\psi$ is injective, we then have $f(g) =f(e)$ for every $f\in F$. In view of Lemma 7, a), we have $g\in H$, and by the formula

$$
f(h) =\tau (h)\cdot f(e) \tag{18}
$$

which holds for every $h\in H$, this can only happen if $g=e$. On the other hand, by Lemma 7, b) and Theorem 3 of V, §10, No. 6, p. 66, we have

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G)$$.

The set $\mathscr{K}$ of K-homomorphisms from F to Ω has cardinal [F : K] because F is étale (V, §6, No. 5, p. 32, Proposition 4), so Card($\mathscr{K}) =$ Card(G). Since the stabilizer of $\chi_0$ in G is equal to $\{e\}$ by the above, $\mathscr{K}$ is a homogenous principal G-set.

(ii)$\Rightarrow$(iii): Suppose that L is étale and that $\mathscr{H}$ is a homogenous principal G-set. By Lemma 10, the $(Ω$, G)-algebras $L_{(Ω)}$ and $\mathscr{F}(\mathscr{H},Ω)$ are isomorphic. Since $\mathscr{H}$ is a homogenous principal G-set, the $(Ω$, G)-algebras $\mathscr{F}(\mathscr{H},Ω)$ and $\mathscr{F}(G,Ω)$ are isomorphic.

(iii)$\Rightarrow$(iv): Suppose that property (iii) holds. Then $L_{(Ω)}$ is a free module of rank 1 over the algebra Ω[G]; the latter can be canonically identified with $K[G]_{(Ω)}$. We then apply Theorem 3 of VIII, p. 37.

The implication (iv)$\Rightarrow$(v) is immediate.

Let us prove the implication (v)$\Rightarrow$(vi). The algebra L is reduced. By Lemma 8, c), the group G acts transitively on the set $\mathscr{S}$ of maximal ideals of L. Let $\mathfrak{m}$ be an element of $\mathscr{S}$. By Lemma 9, since $\bigcap_{\mathfrak{n}\in\mathscr{S}}\mathfrak{n}=\{0\}$, the algebra L is isomorphic to the algebra Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$. The algebra of invariants of $G_{\mathfrak{m}}$ in $L/\mathfrak{m}$ therefore coincides with K by Lemma 7, c). Hence the homomorphism $\lambda_{\mathfrak{m}}$ from $G_{\mathfrak{m}}$ to Gal((L$/\mathfrak{m})/K)$ is surjective. By Lemma 7, we moreover have

Card(G) $= [L : K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]$. So Card(G$_{\mathfrak{m}}) = [L/\mathfrak{m}: K]$, and the homomorphism $\lambda_{\mathfrak{m}}$ is injective.

It remains to prove the implication (vi)$\Rightarrow$(i). Let $\mathfrak{m}$ be a maximal ideal of L. By Lemma 9, the algebra L is isomorphic to the algebra Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ as a $(K$, G)-algebra. Since $G_{\mathfrak{m}}$ acts faithfully in $L/\mathfrak{m}$ and admits K as subfield of invariants, the group homomorphism $\lambda_{\mathfrak{m}}$ defines an isomorphism from $G_{\mathfrak{m}}$ to Gal((L$/\mathfrak{m})/K)$.

#### Remark 2 {#alg-viii-s16-n7-rem-2 .statement}

In Theorem 2, we can replace the assumption that Ω is algebraically closed with the assumption that Ω is separably closed. Indeed, if L is étale, then the image of every K-algebra homomorphism from L to Ω is a separable extension of K.

#### Remark 3 {#alg-viii-s16-n7-rem-3 .statement}

The normal basis theorem (V, §10, No. 9, p. 73, Theorem 6) is a specific case of the implication (i)$\Rightarrow$(iv) in Theorem 2.

#### Definition 1 {#alg-viii-s16-def-1 .statement}

Let G be a finite group, and let L be a nonzero commutative algebra of finite degree over K endowed with the structure of a $(K,G)$-algebra, where the action of G is given by an injective homomorphism from G to the group Aut$_K(L)$. We say that L is a Galois algebra with group G if it has the equivalent properties (i) through (vi) of Theorem 2.

#### Remark 4 {#alg-viii-s16-n7-rem-4 .statement}

Suppose that L is an extension of K endowed with an action $\lambda$ of G. Then L is a Galois algebra over K if and only if L is a Galois extension of K and $\lambda$ is an isomorphism from G to the Galois group of L over K.

#### Remark 5 {#alg-viii-s16-n7-rem-5 .statement}

Suppose that the group G is abelian. If G acts faithfully and transitively on a set X, then the stabilizer of any point of X is reduced to the identity (because the stabilizers of the points of X are all equal and their intersection is reduced to the identity element of G). Consequently, properties (i) through (vi) of Theorem 2 are also equivalent to the following:

(vii) The algebra L is étale, and G acts faithfully and transitively on $\mathscr{H}$.

#### Remark 6 {#alg-viii-s16-n7-rem-6 .statement}

By V, §10, No. 1, p. 75, Lemma 5; V, §10, No. 1, p. 76, Proposition 12; and VIII, p. 137, Proposition 3, a Galois algebra is commutative and semisimple.

#### Example 1 {#alg-viii-s16-n7-exa-1 .statement}

Let $n$ be a strictly positive integer, prime to the characteristic exponent of K. Suppose that the group $µ_n$ of $n$-th roots of unity in K has order $n$. Then for every divisor $d$ of $n$, the group $µ_d$ of $d$-th roots of unity has order $d$. Let $a$ be a nonzero element of K, let L be the algebra $K[X]/(X^n-a)$, and let $x$ be the class of X in L. The sequence $(1, x, . . . , x^{n-1})$ is a basis of the vector space L over the field K, and we have $x^n=a$. Moreover, the polynomial $X^n-a$ is prime to its derivative $nX^{n-1}$, so the algebra L is étale (V, §7, No. 2, p. 37, Proposition 3). For every $\zeta$ in $µ_n$, the automorphism $P(X)\mapsto P(\zeta X)$ of the ring K[X] defines, by passing to the quotients, an endomorphism $\lambda (\zeta )$ of L because we have $(\zeta X)^n-a= X^n-a$; it is an automorphism. We have

$$
\lambda (\zeta )x^i=\zeta^ix^i \tag{19}
$$

for $0\leqslant i < n$. The mapping $\lambda :\zeta \mapsto \lambda (\zeta )$ is an injective homomorphism from $µ_n$ to Aut$_K$(L), and the ring of invariants of the group $\lambda (µ_n)$ in L is equal to $K\cdot 1$. Since the cardinal of $µ_n$ is equal to $n= [L : K]$, the algebra L endowed with the action of $\lambda$ is a Galois algebra (VIII, p. 308, Theorem 2, (v)).

Let $r$ be the least strictly positive integer such that $a^r$ belongs to $K^{*n}$; it divides $n$, and there exists an element $b$ of $K^*$ such that $a=b^{n/r}$. Then (V, §11, No. 8, p. 91, Remark) the polynomial $X^r-b$ is irreducible, and we have $X^n-a=\prod_{\zeta\inµ_{n/r}}(X^r-\zeta b)$. Let E be the field $K[Y]/(Y^r-b)$, and let $y$ be the class of Y in E. There exists an isomorphism $\theta$ from $µ_{n/r}$ to Gal(E$/K)$, characterized by the relation $\theta (\xi )(y) =\xi y$ (V, §11, No. 8, p. 91, Example 3). We then verify that the Galois algebra L is isomorphic to the $(K, µ_n$)-algebra Coind$^µ_{µ^n_{n/r}}(E)$.

#### Example 2 {#alg-viii-s16-n7-exa-2 .statement}

Now suppose that the field K has characteristic $p\not= 0$. Let $c$ be an element of K. The polynomial $f= X^p-X-c$ is prime to its derivative $f'=-1$, so the algebra $L = K[X]/(f)$ is étale (V, §7, No. 2, p. 37, Proposition 3). We denote the image of X in L by $x$; we have the relation $x^p=x+c$. The sequence $(1, x, . . . , x^{p-1})$ is a basis of L viewed as a vector space over K.

Let P be the additive group of the prime subfield of K; it is a cyclic group of order $p$, generated by the unit element 1 of K. For every $j$ in P, we have $j^p=j$ (V, §1, No. 3, p. 4, formula (4)) and therefore $f(X +j) =f(X)$. Hence there exists an automorphism $\gamma (j)$ of the algebra L characterized by the relation $\gamma (j)(x) =x+j$; moreover, the resulting mapping $\gamma$ is an injective homomorphism from P to Aut$_K(L)$.

Let Ω be an algebraically closed extension of K, and let $\xi$ be a root of the polynomial $f$ in Ω. We have $\xi^p=\xi +c$, hence

$$
X^p-X-c= (X^p-\xi^p)-(X-\xi ) = (X-\xi )^p-(X-\xi ) =_j\prod_{\in P}(X-\xi -j)
$$

by V, §12, No. 1, p. 94, formula (1). For every $j$ in P, there exists a unique algebra homomorphism $\chi_j: L\rightarrow Ω$ that sends $x$ to $\xi +j$; moreover, every homomorphism from L to Ω is one of the $\chi_j$, and we have the relation $\chi_j=\chi_0\circ \gamma (j)$. The algebra L endowed with $\gamma$ has property (ii) of Theorem 2 of VIII, p. 308 and is therefore a Galois algebra over K.

To describe the structure of L, we must distinguish between two cases:

a) We have $\xi \notin K$. Then the polynomial $f(X)$ is irreducible in K[X] (V, §11, No. 9, p. 93, Example 3). In this case, L is a cyclic extension of K of degree $p$, and $\gamma$ is an isomorphism from P to Gal(L$/K)$.

b) We have $\xi \in K$. Then the mapping $\psi :y\mapsto (\chi_j(y))_{j\in P}$ is an isomorphism from the algebra L to the product algebra $K^P$; moreover, $\psi \circ \gamma (k)\circ \psi^{-1}$ is the automorphism $(x_j)_{j\in P}\mapsto (x_{j+k})_{j\in P}$ of $K^P$ for every $k\in P$.

### 8. Actions on Galois Algebras

#### Proposition 9 {#alg-viii-s16-prop-9 .statement}

Let G be a finite group, H be a subgroup of G, and E be a Galois algebra over the field K with group H. Then the $(K,G)$-algebra Coind$^G_H(E)$ deduced from E by coinduction from H to G is a Galois algebra over the field K with group G.

Since E is a Galois algebra over K, by property (v) of Theorem 2 of VIII, p. 308, it is reduced, we have Card(H) = [E : K], and K is the ring of invariants of H in E. But by Lemma 7 of VIII, p. 305, the algebra F = Coind$^G_H(E)$ is reduced, and we have

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G)$$,

and K is the ring of invariants of G in F. So F is a Galois algebra by the criterion given in Theorem 2, (v).

#### Proposition 10 {#alg-viii-s16-prop-10 .statement}

Let G be a finite group. Let L be a Galois algebra over the field K with group G, and let $K'$ be an extension of K. Then the $(K',G)$-algebra $L_{(K')}$ is a Galois algebra over $K'$.

We use property (v) in Theorem 2 by observing that if the K-algebra L is étale, then the $K'$-algebra $L_{(K')}$ is too (V, §6, No. 5, p. 32, Corollary 2), that we have the equality $[L_{(K')}: K'] = [L : K]$, and that the ring of invariants of G in $L_{(K')}$ is $(L^G)_{(K')}$, where $L^G$ is the ring of invariants of G in L.

#### Proposition 11 {#alg-viii-s16-prop-11 .statement}

Let $G_1$ and $G_2$ be groups. Let $L_1$ and $L_2$ be Galois algebras over K with respective actions $\lambda_1: G_1\rightarrow$ Aut$_K(L_1)$ and $\lambda_2: G_2\rightarrow$ Aut$_K(L_2)$. Set $L = L_1\otimes_KL_2,G = G_1\times G_2$, and $\lambda (g_1, g_2) =\lambda_1(g_1)\otimes \lambda_2(g_2)$ for $(g_1, g_2)\in G$. Then the K-algebra L endowed with the action $\lambda$ is a Galois algebra over K.

We reason as before, taking the following into account: If $L_1$ and $L_2$ are étale, then so is the algebra $L = L_1\otimes_KL_2$ (V, §6, No. 5, p. 32, Corollary 1), and we have the equalities

$[L : K] = [L_1: K][L_2: K]$ and Card(G) = Card(G$_1)$ Card(G$_2)$.

Moreover, if $L^G_{i^i}$ denotes the ring of invariants of $G_i$ in $L_i$, then it follows from Lemma 11 below that $L^G_{1^1}\otimes_KL^G_{2^2}$ is the ring of invariants of $G_1\times G_2$ in $L_1\otimes_KL_2$.

#### Lemma 11 {#alg-viii-s16-lem-11 .statement}

Let $G_1$ and $G_2$ be groups, and let $W_1$ and $W_2$ be K-vector spaces. We endow $W_1($resp. $W_2)$ with an action of $G_1($resp. $G_2)$ given by a group homomorphism $\rho_1: G_1\rightarrow$ Aut$_K(W_1) ($resp. $\rho_2: G_2\rightarrow$ Aut$_K(W_2))$. We consider the group homomorphism

$\rho_1\otimes \rho_2: G_1\times G_2\longrightarrow$ Aut$_K(W_1\otimes_KW_2)$

defined by the relation $(\rho_1\otimes \rho_2)(g_1, g_2)(w_1\otimes w_2) =\rho_1(g_1)(w_1)\otimes \rho_2(g_2)(w_2)$ for $g_1\in G_1,g_2\in G_2,w_1\in W_1$, and $w_2\in W_2$. Then the linear mapping from $W^G_{1^1}\otimes_KW^G_{2^2}$ to $W_1\otimes_KW_2$ given by the tensor product of the canonical injections induces an isomorphism of K-vector spaces from $W_1^{G_1}\otimes_KW^G_{2^2}$ to $(W_1\otimes_KW_2)^{G_1\times G_2}$.

This follows from Lemma 1 of VIII, p. 213 applied to the K[G]-modules $M_1= M_2= K$ endowed with the trivial action of $G, N_1= W_1$, and $N_2= W_2$.

#### Remark {#alg-viii-s16-n8-rem-1 .statement}

Let L be a Galois extension of the field K of finite degree, and let G be its Galois group; we denote the identity mapping on G by $\lambda$. Then L endowed with $\lambda$ is a Galois algebra over K with group G. Let $K'$ be an extension of K. By Proposition 10, the algebra $L_{(K')}$ is Galois over $K'$, but it is not in general an extension of $K'$. Analogously, by Proposition 11, the tensor product of Galois extensions E and F of K of finite degree can be viewed as a Galois algebra; in general, it is not a Galois extension of K. It is one, however, if E and F are moreover linearly disjoint subextensions of an extension of K (V, §2, No. 5, p. 13 and V, §10, No. 1, p. 57, Proposition 1).

### 9. Cross Products

Let K be a field, and let G be a group whose identity element we denote by $e$. Let L be a commutative K-algebra, and let $\lambda$ be a homomorphism from G to the automorphism group of the K-algebra L. For any $g$ in G, let $\tau (g)$ be the automorphism of the multiplicative group $L^*$ of L induced by $\lambda (g)$.

Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension of the group G by $L^*$. Define a right action of the group $L^*$ on the set $L\times Γ$ by

$$
(\beta , \gamma ).\alpha = (\beta \alpha , \iota (\alpha )^{-1}\gamma ) \tag{20}
$$

for $\alpha \in L^*,\beta \in L$, and $\gamma \in Γ$. We denote by E the set of orbits of $L^*$ in $L\times Γ$ and by $[\beta ;\gamma ]$ the orbit of the pair $(\beta , \gamma )$. We therefore have, by construction, the relation

$$
[\beta \alpha ;\gamma ] = [\beta ;\iota (\alpha )\gamma ] \tag{21}
$$

for $\alpha \in L^*,\beta \in L$, and $\gamma \in Γ$.

Given $\beta$ in L and $\gamma$ in Γ, we denote by $^{\gamma}\beta$ the transform of $\beta$ under the automorphism $\lambda \circ \pi (\gamma )$ of L; we have the relations

(22) $^{\gamma}(^{\gamma'}\beta ) =^{\gamma \gamma'}\beta  ,^{\gamma}(\beta +\beta ') =^{\gamma}\beta +^{\gamma}\beta '$, and $^{\gamma}(\beta \beta ') =^{\gamma}\beta^{\gamma}\beta '$

for $\gamma , \gamma '$ in Γ and $\beta , \beta '$ in L. There exists a law of composition on E characterized by the relation

$$
[\beta ;\gamma ][\beta ';\gamma '] = [\beta^{\gamma}\beta ';\gamma \gamma '] \tag{23}
$$

Indeed, it suffices to verify that the right-hand side does not change if we replace, respectively, $\beta ,\gamma ,\beta '$, and $\gamma '$ with $\beta \alpha ,\iota (\alpha )^{-1}\gamma ,\beta '\alpha '$, and $\iota (\alpha ')^{-1}\gamma '$ for all $\alpha ,\alpha '$ in $L^*$. This follows immediately by applying to $\mathscr{E}$ formula (1) of VIII, p. 285, which can also be written as $\gamma \iota (\alpha ) =\iota (^{\gamma}\alpha )\gamma$ for $\gamma \in Γ$ and $\alpha \in L^*$. By the formulas in (22), the set E endowed with this law is a monoid with identity element $[1;e]$.

Since $\pi \circ \iota$ is constant with value $e$, there exists a mapping $\widetilde{\pi}$ from E to G such that we have

$$
\widetilde{\pi}([\beta ;\gamma ]) =\pi (\gamma ) \tag{24}
$$

for $\beta \in L$ and $\gamma \in Γ$.

Let $g$ be an element of G, and let $E_g=\widetilde{\pi}^{-1}(g)$. If $\gamma_0$ is a fixed element of $\pi^{-1}(g)$, then the mapping $\beta \mapsto [\beta ;\gamma_0]$ is a bijection from L to $E_g$, thanks to which we will transfer to $E_g$ the K-vector space structure on L. Since $\pi^{-1}(g)$ is composed of elements of the form $\iota (\alpha )\gamma_0$, where $\alpha$ runs through $L^*$, and we have

$$
[\beta ;\iota (\alpha )\gamma_0] = [\beta \alpha ;\gamma_0]
$$

the vector space structure on $E_g$ does not depend on the choice of $\gamma_0$.

Let $g$ and $g'$ be elements of G; by formulas (22) and (23), the law of composition on E induces by restriction a K-bilinear mapping from $E_g\times E_{g'}$ to $E_{gg'}$. Consequently, the vector space $P =\bigoplus_{g\in G}E_g$ is endowed with the structure of an associative and unital algebra, whose multiplication induces the previous bilinear mapping from $E_g\times E_{g'}$ to $E_{gg'}$ for all $g$ and $g'$ in G. The algebra P is called the cross product of L and $\mathscr{E}$ and is denoted by $\mathbf{A}[\mathscr{E}; L]$; its unit element is the element $[1;e]$ of $E_e$.

Set

$$
u(\beta ) = [\beta ;e] \tag{25}
$$

for $\beta$ in L. Then $u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ is an injective homomorphism of K-algebras. By (23), for every $\gamma \in Γ$, the element $[1;\gamma ]$ is invertible in $\mathbf{A}[\mathscr{E},L]$, and the mapping $v: Γ\rightarrow \mathbf{A}[\mathscr{E},L]^*$ that sends $\gamma$ to $[1;\gamma ]$ is an injective group homomorphism. The homomorphisms $u$ and $v$ are called canonical. We have the relations

$$
u(\alpha ) =v(\iota (\alpha )) \tag{26}
$$

(27) $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$, (28) $[\beta ;\gamma ] =u(\beta )v(\gamma )$

for $\alpha \in L^*,\beta \in L$, and $\gamma \in Γ$.

Conversely, we have the following universal property of the algebra $\mathbf{A}[\mathscr{E}; L]$.

#### Proposition 12 {#alg-viii-s16-prop-12 .statement}

Let B be a K-algebra, $u': L\rightarrow B$ a K-algebra homomorphism, and $v': Γ\rightarrow B^*$ a group homomorphism. We assume satisfied the relations

$$
u'(\alpha ) =v'(\iota (\alpha )) \tag{29}
$$

(30) $u'(^{\gamma}\beta ) =v'(\gamma )u'(\beta )v'(\gamma )^{-1}$

for $\alpha \in L^*,\beta \in L$, and $\gamma \in Γ$. Then there exists a unique algebra homomorphism $f$ from $\mathbf{A}[\mathscr{E}; L]$ to B such that we have $u'=f\circ u$ and $v'=f\circ v$.

To prove the uniqueness of $f$, observe that the vector space $\mathbf{A}[\mathscr{E}; L]$ over the field K is generated by the set of elements of the form $[\beta ;\gamma ] =u(\beta )v(\gamma )$. If the homomorphism $f':\mathbf{A}[\mathscr{E}; L]\rightarrow B$ satisfies $f'\circ u=u'$ and $f'\circ v=v'$, then it sends $[\beta ;\gamma ]$ to $u'(\beta )v'(\gamma )$ and therefore coincides with $f$.

By formula (29), we have

$$
u'(\beta \alpha )v'(\iota (\alpha )^{-1}\gamma ) =u'(\beta )v'(\gamma ) \tag{31}
$$

for $\alpha$ in $L^*,\beta$ in L, and $\gamma$ in Γ. By the definition of E, there consequently exists a mapping $f_0: E\rightarrow B$ such that $f_0([\beta ;\gamma ]) =u'(\beta )v'(\gamma )$. By formulas (23) and (30), we have $f_0(xx') =f_0(x)f_0(x')$ for $x$ and $x'$ in E. The restriction of $f_0$ to $E_g$ is K-linear for every element $g$ of G; consequently, there exists a unique K-linear mapping $f$ from $\mathbf{A}[\mathscr{E}; L]$ to B that coincides with $f_0$ on E. The mapping $f$ is an algebra morphism that satisfies $u'=f\circ u$ and $v'=f\circ v$.

#### Remark {#alg-viii-s16-n9-rem-1 .statement}

Let $\sigma : G\rightarrow Γ$ be a section of the mapping $\pi$. Set $\varepsilon_g=v(\sigma (g))$ for every $g$ in G, and denote by $c_{\sigma}$ the 2-cocycle associated with $\sigma$ (VIII, p. 296). In particular, we have

$$
\varepsilon_g\varepsilon_{g'}=u(c_{\sigma}(g, g'))\varepsilon_{gg'} \tag{32}
$$

for all $g, g'\in G$. Let us, moreover, identify L with a subalgebra of $\mathbf{A}[\mathscr{E}; L]$ via the homomorphism $u$. Then every element of $\mathbf{A}[\mathscr{E}; L]$ can be written uniquely as $\sum_{g\in G}a_g\varepsilon_g$, where $(a_g)$ is a family of elements of L with finite support. The multiplication in $\mathbf{A}[\mathscr{E}; L]$ can be expressed by the formula

$$
\sum_ga_g\varepsilon_g\sum_gb_g\varepsilon_g=\sum_gd_g\varepsilon_g \tag{33}
$$

with

$$
d_g=_{hh}\sum^'_{=g}a_h(\lambda (h)\cdot b_{h'})c_{\sigma}(h, h') \tag{34}
$$

If the extension $\mathscr{E}$ is semitrivial, then we can choose a section $\sigma$ of $\pi$ that is a group morphism from G to Γ; the cocycle $c_{\sigma}$ is therefore constant with value 1, and formula (34) simplifies to

$$
d_g=_{hh}\sum^'_{=g}a_h\lambda (h)\cdot b_{h'} \tag{35}
$$

Let $K'$ be an extension of the field K. Denote by $L'$ the $K'$-algebra $L_{(K')}$, and for any $g$ in G, denote by $\lambda '(g)$ the automorphism $\lambda (g)_{(K')}$ induced by $\lambda (g)$ on $L_{(K')}$. Moreover, let us denote by $\tau '(g)$ the automorphism of $L^{'*}$ induced by $\lambda '(g)$. Finally, let $h$ be the homomorphism from $L^*$ to $L^{'*}$ that sends $x$ to $x\otimes 1$. Let $\mathscr{E}'= (Γ', \iota ', \pi ')$ be the direct image of the extension of $\mathscr{E}$ by $h$ (VIII, p. 289). Let $\mathbf{A}[\mathscr{E}',L']$ be the cross product $K'$-algebra of $\mathscr{E}'$ and $L'$, and let $u': L'\rightarrow \mathbf{A}[\mathscr{E}',L']$ and $v': Γ'\rightarrow \mathbf{A}[\mathscr{E}',L']^*$ be the canonical homomorphisms.

#### Proposition 13 {#alg-viii-s16-prop-13 .statement}

There exists a unique isomorphism of $K'$-algebras $\varphi$ from $\mathbf{A}[\mathscr{E}; L]_{(K')}$ to $\mathbf{A}[\mathscr{E}'; L']$ that satisfies the relations

$$
u'(h(\beta )) =\varphi (1\otimes u(\beta )) \tag{36}
$$

for $\beta \in L$ and (37) $v'(h(\gamma )) =\varphi (1\otimes v(\gamma ))$

for $\gamma \in Γ$.

The proof follows immediately from the constructions.

The isomorphism $\varphi$ is called canonical.

### 10. Application to the Brauer Group

In this subsection, K is a field, and L is a Galois algebra over K with action $\lambda : G\rightarrow$ Aut$_K(L)$. We denote the degree of L over K by $n$. We have $n=$ Card(G).

#### Theorem 3 {#alg-viii-s16-thm-3 .statement}

Let $\mathscr{E}= (Γ, \iota , \pi )$ be a $\tau$-extension of G by $L^*$. The algebra $\mathbf{A}[\mathscr{E}; L]$ is central simple and of degree $n^2$ over K. Moreover, the canonical homomorphism $u$ from L to $\mathbf{A}[\mathscr{E}; L]$ is an isomorphism from L to a maximal commutative subalgebra of $\mathbf{A}[\mathscr{E}; L]$.

#### Lemma 12 {#alg-viii-s16-lem-12 .statement}

a) There does not exist any ideal of L, other than $\{0\}$ and L that is invariant under G.

b) Let $g$ be an element of G distinct from the identity element, and let $\mathfrak{a}_g$ be the ideal of L generated by the elements of the form $x-\lambda (g)x$, where $x$ runs through L. We have $\mathfrak{a}_g= L$.

Let $\mathscr{S}$ be the set of maximal ideals of L; for any subset S of $\mathscr{S}$, set $\mathfrak{a}(S) =\bigcap_{\mathfrak{m}\in S}\mathfrak{m}$. Since the ring L is commutative and semisimple (VIII, p. 310, Remark 6), the map $W\mapsto \mathfrak{a}(W)$ is a bijection from the set of subsets of $\mathscr{S}$ to the set of ideals of L (VIII, p. 142, Proposition 9). The ideal $\mathfrak{a}(S)$ is invariant under G if and only if S is. Since G acts transitively on $\mathscr{S}$ (VIII, p. 308, Theorem 2, vi)), the only subsets of $\mathscr{S}$ invariant under G are $\emptyset$ and $\mathscr{S}$. Since $\mathfrak{a}(\emptyset ) = L$ and $\mathfrak{a}(\mathscr{S}) =\{0\}$, we have proved assertion a).

Let us prove b) by contradiction; suppose that we have $\mathfrak{a}_g\not= L$. Let $\mathfrak{m}$ be a maximal ideal of L containing $\mathfrak{a}_g$. We then have $\lambda (g)x\equiv x$ mod $\mathfrak{m}$ for every $x$ in L. In particular, $\mathfrak{m}$ is invariant under $g$, and $\lambda (g)$ is induced by the identity on the field $L/\mathfrak{m}$. By property (vi) in Theorem 2 of VIII, p. 308, the element $g$ of $G_{\mathfrak{m}}$ is trivial, which contradicts the assumption of b).

Let us now prove Theorem 3. The vector space $\mathbf{A}[\mathscr{E}; L]$ has finite dimension Card(G)[L$: K] =n^2$ over K, by VIII, p. 316 and the assumed equality Card(G) $= [L : K] =n$.

Let $\mathfrak{a}$ be a nonzero two-sided ideal of the algebra $\mathbf{A}[\mathscr{E}; L]$. We use the notation of VIII, p. 316. Every element $a$ of $\mathbf{A}[\mathscr{E}; L]$ can be written uniquely as $a=\sum_{g\in G}a_g\varepsilon_g$ with $a_g\in L$ for every $g\in G$; we denote by $Φ(a)$ the set of elements $g$ of G such that $a_g\not= 0$. By formula (32) of VIII, p. 316, we have the relation

$$
\varepsilon_g\varepsilon_{g'}=c_{\sigma}(g, g')\varepsilon_{gg'} \tag{38}
$$

for all $g, g'\in G$ and consequently

$$
Φ(a\varepsilon_g) = Φ(a).g \tag{39}
$$

for every $g\in G$ and $a\in \mathbf{A}[\mathscr{E}; L]$.

Let $a$ be a nonzero element of $\mathfrak{a}$ for which $Φ(a)$ is minimal for the inclusion; by formula (39), if necessary replacing $a$ with an element of the form $a\varepsilon_{g^{-1}}$ with $g\in Φ(a)$, we may assume that we have $e\in Φ(a)$. Let $s$ be an element of $Φ(a)$ distinct from $e$. By Lemma 12, b), there exists an element $x$ of L such that $a_s(x-\lambda (s)\cdot x)\not= 0$. But we have the relation

$$
xa-ax=\sum_ga_g(x-\lambda (g)\cdot x)\varepsilon_g \tag{40}
$$

where the sum is taken over the elements $g$ of $Φ(a)$ distinct from $e$. Because of the minimality of $Φ(a)$, we then have $xa-ax= 0$, but this contradicts the assumption on $x$. We have, therefore, proved by contradiction that $Φ(a)$ contains only the identity element $e$ of G, so we have $a\in L$.

Hence $L\cap \mathfrak{a}$ is an ideal of L not reduced to $\{0\}$. Moreover, for every $x$ in L, we have $\varepsilon_gx\varepsilon^-_g^1=\lambda (g)\cdot x$, so $L\cap \mathfrak{a}$ is invariant under G. By Lemma 12, we therefore have $L\cap \mathfrak{a}= L$, that is, $L\subset \mathfrak{a}$. Since L contains the identity element of $\mathbf{A}[\mathscr{E}; L]$, we have $\mathfrak{a}=\mathbf{A}[\mathscr{E}; L]$.

Since the algebra $\mathbf{A}[\mathscr{E}; L]$ has nonzero finite dimension over K and its only two-sided ideals are $\{0\}$ and $\mathbf{A}[\mathscr{E}; L]$, it is simple.

Let us prove that every element $a$ of $\mathbf{A}[\mathscr{E}; L]$ that commutes with L belongs to L. We write $a$ as $\sum_{g\in G}a_g\varepsilon_g$ with coefficients $a_g$ in L. For every $x$ in L, we have $xa-ax= 0$, and relation (40) shows that we have

$$
a_g(x-\lambda (g)\cdot x) = 0 \tag{41}
$$

for every $g\in G$ and $x\in L$. By Lemma 12, we therefore have $a_g= 0$ for $g\not=e$; consequently, $a\in L$.

Let us, finally, determine the center of $\mathbf{A}[\mathscr{E}; L]$. If $z$ belongs to the center, then it commutes with L, so belongs to L. But we then have

$$
0 =\varepsilon_gz-z\varepsilon_g= (\lambda (g)\cdot z-z)\varepsilon_g
$$

for every $g$ of G. Hence $z$ is invariant under the automorphism group $\lambda (G)$ of L. We therefore have $z\in K$ by assumption.

#### Theorem 4 {#alg-viii-s16-thm-4 .statement}

Let A be a central simple algebra of finite degree over K, and let L be a maximal commutative subalgebra of A. Then there exists a $\tau$-extension $\mathscr{E}$ of G by $L^*$ such that A is isomorphic to $\mathbf{A}[\mathscr{E}; L]$.

Without loss of generality, we may assume that L is a maximal commutative subalgebra of A. Let Γ be the multiplicative group consisting of the invertible elements $\gamma$ of A such that there exists a $g$ in G with

$$
\gamma x\gamma^{-1}=\lambda (g).x \tag{42}
$$

for every element $x$ of L. If $\gamma \in Γ$ is given, then the element $g$ satisfying this relation is unique; we denote it by $\pi (\gamma )$. It is immediate that $\pi$ is a homomorphism from Γ to G and that its kernel is equal to $L^*$. The surjectivity of $\pi$ follows from the Skolem–Noether theorem (VIII, p. 263, Corollary).

If we denote the canonical injection of $L^*$ into Γ by $\iota$, then it follows from the constructions that $\mathscr{E}= (Γ, \iota , \pi )$ is a $\tau$-extension of G by $L^*$. Let

$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ and $v: Γ\rightarrow \mathbf{A}[\mathscr{E}; L]$

be the canonical homomorphisms. By the universal property of $\mathbf{A}[\mathscr{E}; L]$ (VIII, p. 315, Proposition 12), there exists a unique algebra homomorphism $f:\mathbf{A}[\mathscr{E}; L]\rightarrow A$ such that $f\circ u(x) =x$ and $f\circ v(\gamma ) =\gamma$ for $x\in L$ and $\gamma \in Γ$. Since the algebra $\mathbf{A}[\mathscr{E}; L]$ is simple, the homomorphism $f$ is injective. Now, the algebra $\mathbf{A}[\mathscr{E}; L]$ has degree $n^2$ over K and so does A because L is a maximal commutative semisimple subalgebra of A and we have $n= [L : K]$ (VIII, p. 262, Proposition 3, (ii)). Hence $f$ is bijective.

#### Definition 2 {#alg-viii-s16-def-2 .statement}

Let $\mathscr{S}$ be the set of maximal ideals of L. We define

Br(L$/K) =_{\mathfrak{m}}\bigcap_{\in\mathscr{S}}$ Ker($r_{(L/\mathfrak{m})/K})$, where $r_{(L/\mathfrak{m})/K}:$ Br(K) $\rightarrow$ Br(L$/\mathfrak{m})$ is the extension of scalars homomorphism (VIII, p. 281).

#### Theorem 5 {#alg-viii-s16-thm-5 .statement}

There exists a group isomorphism

Ψ : Ex$_{\tau}(G,L^*)\longrightarrow$ Br(L$/K)$

that sends the class of a $\tau$-extension $\mathscr{E}$ of G by $L^*$ to the class in Br(L$/K)$ of the algebra $\mathbf{A}[\mathscr{E}; L]$.

To define Ψ and verify that it is a bijection, we must establish the following points:

a) If $\mathscr{E}$ and $\mathscr{E}'$ are isomorphic $\tau$-extensions of G by $L^*$, then the algebras $\mathbf{A}[\mathscr{E}; L]$ and $\mathbf{A}[\mathscr{E}'; L]$ are isomorphic.

b) Conversely, if the algebras $\mathbf{A}[\mathscr{E}; L]$ and $\mathbf{A}[\mathscr{E}'; L]$ are isomorphic, then the $\tau$-extensions $\mathscr{E}$ and $\mathscr{E}'$ of G by $L^*$ are isomorphic.

c) In every class in Br(L$/K)$, there is an algebra E containing L as a maximal commutative subalgebra.

d) If E is a central simple algebra of finite degree over K containing L as a maximal commutative subalgebra, then there exists a $\tau$-extension $\mathscr{E}$ of G by $L^*$ such that E is isomorphic to $\mathbf{A}[\mathscr{E}; L]$. Assertion a) follows from the construction of the cross product; b) follows from VIII, p. 263, Corollary. Assertion c) follows from Proposition 5 of VIII, p. 281, and d) is simply Theorem 4 above.

It remains to verify that Ψ is a group homomorphism; for this, it suffices to prove that if $\mathscr{E}_1= (Γ_1, \iota_1, \pi_1)$ and $\mathscr{E}_2= (Γ_2, \iota_2, \pi_2)$ are $\tau$-extensions, then the algebra $\mathbf{A}[\mathscr{E}_1\mathscr{E}_2; L]$ is equivalent to the algebra $\mathbf{A}[\mathscr{E}_1; L]\otimes \mathbf{A}[\mathscr{E}_2; L]$. We denote the product extension $\mathscr{E}_1\mathscr{E}_2$ by $\mathscr{E}= (Γ, \iota , \pi )$. The group Γ is isomorphic to the cokernel of the homomorphism $\rho$ from $L^*$ to the fiber product $Γ_1\times_GΓ_2$ that sends $µ$ to $(\iota_1(µ), \iota_2(µ)^{-1})$. For $i\in  \{1,2\}$, write $A_i=\mathbf{A}[\mathscr{E}_i; L]$. Let $u_i: L\rightarrow A_i$ and $v_i: Γ_i\rightarrow A^*_i$ be the canonical homomorphisms. We identify L with its images by the homomorphisms $u_i$, which make L into maximal commutative subalgebras of the $A_i$. We denote by $V_i$ the L-vector space defined by left multiplication in $A_i$. The ring $L\otimes_KA^o_i$ acts on $V_i$. Since it is simple and has dimension $n^2$ over L, we obtain an isomorphism from $L\otimes_KA^o_i$ to End$_L(V_i)$. Hence the ring $L\otimes_KA^o_1\otimes_KA^o_2$, which we can identify with $(L\otimes_KA^o_1)\otimes_L(L\otimes_KA^o_2)$, is isomorphic to End$_L(V_1\otimes_LV_2)$. Set C = End$_{A^o_1\otimes_KA^o_2}(V_1\otimes_LV_2)$. By Lemma 3 of VIII, p. 282, the ring C is similar to $A_1\otimes_KA_2$, and $L\otimes 1\otimes 1$ is a maximal commutative subalgebra of C. For every pair $(\gamma_1, \gamma_2)\in Γ_1\times Γ_2$ satisfying $\pi_1(\gamma_1) =\pi_2(\gamma_2)$, we denote by $w(\gamma_1, \gamma_2)$ the unique $\lambda (\pi_1(\gamma_1$))-semilinear (II, §1, No. 13, p. 223) endomorphism such that

$$
w(\gamma_1, \gamma_2)(x_1\otimes x_2) =v_1(\gamma_1)x_1\otimes v_2(\gamma_2)x_2
$$

for $x_1\in V_1$ and $x_2\in V_2$. We have $w(\gamma_1, \gamma_2)\in C^*$, and $w$ is a group homomorphism from the fiber product $Γ_1\times_GΓ_2$ to $C^*$. This homomorphism is trivial on the image of $\rho$ and induces a homomorphism $v$ from Γ to $C^*$. Denote by $u: L\rightarrow C$ the morphism given by $u:`\mapsto `\otimes 1\otimes 1$. We can verify the relations

$u(\alpha ) =v(\iota (\alpha ))$ and $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$

for $\alpha \in L^*,\beta \in L$, and $\gamma \in Γ$. Proposition 12 of VIII, p. 315 gives a homomorphism $f$ from the algebra $\mathbf{A}[\mathscr{E}; L]$ to C. Since the algebra $\mathbf{A}[\mathscr{E}; L]$ is simple, the homomorphism $f$ is injective. The algebras C and $\mathbf{A}[\mathscr{E}; L]$ have the same dimension over K, so $f$ is an isomorphism.

#### Remark 1 {#alg-viii-s16-n10-rem-1 .statement}

If L is an étale algebra over K and G is the automorphism group of L, then it is not always true that the algebra $\mathbf{A}[\mathscr{E}; L]$ is central simple (for example, we can take $L = K^n$ and $G =\mathfrak{S}_n)$.

#### Remark 2 {#alg-viii-s16-n10-rem-2 .statement}

We can calculate a 2-cocycle $c$ associated with an algebra A split by a finite Galois extension L with group G as follows. First, there exists a K-homomorphism $\varphi : A\rightarrow \mathbf{M}_m$(L), where $[A : K] =m^2$. For $g\in G$, let $\varphi^g$ be the homomorphism from A to $\mathbf{M}_m(L)$ given by $a\mapsto \varphi (g^{-1}ag)$. By the Skolem–Noether theorem (VIII, p. 256, Theorem 3), for every $g\in G$, there exists an element $u_g$ of $\mathbf{G}\mathbf{L}_m(L)$ such that

$$
\varphi^g(a) =u_g\varphi (a)u^-_g^1
$$

for $a\in A$. We then set

$$
c(g, g') =u_gu_{g'}u^-_{gg}^{1_'}
$$

We can also define an extension of G by $L^*$ using $\varphi :$ we consider the group $Γ\subset \mathbf{G}\mathbf{L}_m(L)$ consisting of the $\gamma$ for which there exists a $g\in G$ with

$$
\varphi^g(a) =\gamma \varphi (a)\gamma^{-1}
$$

for every $a\in A$. The class of this extension is the inverse image by Ψ of the class of A in Br(L$/K)$.

#### Corollary {#alg-viii-s16-n10-cor-1 .statement}

The mapping $Φ_{L/K}= Θ\circ Ψ^{-1}$ defines a group isomorphism from Br(L$/K)$ to $H^2(G,L^*)$.

Let $K'$ be an extension of K and $\varphi : K'\rightarrow L$ a morphism of K-algebras. The set H of elements $h$ of G such that $\lambda (h)\circ \varphi =\varphi$ is a subgroup of G, and the $K'$-algebra L endowed with the restriction of $\lambda$ to H is a Galois algebra over $K'$.

#### Proposition 14 {#alg-viii-s16-prop-14 .statement}

The following diagram commutes:

Br(L$/K)^{\Phi_{L/K}}/$/ $H_2(G,L_*)$

$r_{K'/K}$ Res$_G$

H

Br(L$/K_')^{\Phi_{L/K'}}/$/ $H_2(H,L_*)$ .

This follows from Propositions 7 of VIII, p. 299 and 13 of VIII, p. 317.

### 11. Index and Exponent

#### Theorem 6 {#alg-viii-s16-thm-6 .statement}

Let K be a commutative field, and let A be a central simple A-algebra of finite degree over K. Let L be a separable extension of K of finite degree that is a splitting field for the algebra A. Then [L : K][A] is zero in Br(K).

There exists an extension M of L that is a Galois extension of K of finite degree (V, §10, No. 1, p. 57, Proposition 2). The class [A] of A in the Brauer group of K belongs to the subgroup Br(M$/K)$. Let G be the Galois group of M over K, and let $\alpha$ be the image of [A] in $H^2(G,M^*)$ (VIII, p. 321, Corollary). Let H be the Galois group of M over L. Then H is a subgroup of index [L : K] in G (V, §10, No. 7, p. 68, Corollary 5). Since Res$^G_H(\alpha ) = Φ_{M/L}(A_{(L)})$ (Proposition 14), we have Res$^G_H(\alpha ) = 0$. By Proposition 8 of VIII, p. 303, it follows that $[L : K]\alpha = 0$, and consequently [L : K][A] = 0.

Let K be a commutative field, and let A be a central simple algebra of finite degree over K. Then A is isomorphic to an algebra of the form $\mathbf{M}_n$(D), where D is a field with center K, and [A] = [D] in Br(K). The reduced degree of D depends only on A. We call this reduced degree the index of A. The index of A divides the reduced degree of A. The exponent of A is the order of the class of A in the Brauer group of K.

#### Corollary 1 {#alg-viii-s16-thm-6-cor-1 .statement}

The exponent of a central simple algebra of finite degree over a commutative field divides its index.

It suffices to prove this for a field D of finite degree over its center K. Let L be a maximal commutative subfield of D that is a separable extension of K; we have $[D : K] = [L : K]^2$ (VIII, p. 265, Corollary 2, b) and c)). Then the extension L of K is a splitting field for the algebra D (VIII, p. 281, Proposition 5), and [L : K] coincides with the reduced degree of D. We then apply Theorem 6.

#### Corollary 2 {#alg-viii-s16-thm-6-cor-2 .statement}

Let K be a commutative field, and let A be a central simple algebra of finite degree over K. Let $p$ be a prime number. If $p$ divides the index of A, then it divides the exponent of A.

Let us suppose that the prime number $p$ does not divide the exponent of A and prove that it does not divide its index. It suffices to prove this result in the case when A is a field. Let L be a Galois extension of K of finite degree that splits A. Let G be the Galois group of L over K, and let H be a Sylow $p$-subgroup of G (I, §6, No. 6, p. 78). We denote by $L'= L^H$ the subfield of L of invariants of H. The exponent of $A_{(L')}$ divides that of A and is therefore prime to $p$. By Theorem 6, we have $[L : L'][A_{(L')}] = 0$ in the Brauer group of $L'$. It follows that $[A_{(L')}] = 0$ and that the field $L'$ splits A. We then apply Corollary 2 of VIII, p. 283; it follows that the index of A divides $[L': K]$ and is therefore not divisible by $p$.

#### Corollary 3 {#alg-viii-s16-thm-6-cor-3 .statement}

Let $p$ be a prime number and let K be a perfect field of characteristic $p$. Let A be a central simple algebra of finite degree over K. Then $p$ does not divide the index of A.

Let us prove that the Brauer group of K does not contain any element of order $p$. Every Galois extension M of K of finite degree is a perfect field (V, §7, No. 1, p. 36, Proposition 2). Hence taking the $p$-th power is an automorphism of the group $M^*$. It follows that multiplication by $p$ is an automorphism of the group $H^2$(Gal(M$/K),M^*)$ that is isomorphic to Br(M$/K)$.

Consequently, the order of [A] is prime to $p$ and, by Corollary 2, its index is not divisible by $p$.

#### Remark {#alg-viii-s16-n11-rem-1 .statement}

By considering tensor products of quaternion algebras, it is possible to construct fields with center K, exponent 2, and arbitrarily large index (cf. VIII, p. 371, Exercises 7 and 8).

$*$Conversely, if K is a finite Galois extension of a $p$-adic field or a field of formal power series over a finite field, then the exponent of a central simple algebra of finite degree over K is equal to its index (VIII, p. 332, Exercise 17, e)).$*$

### Exercises {#alg-viii-s16-exercises}

1) Let G be a group and $\mathbf{Z}[G]$ the algebra of G over $\mathbf{Z}$; we identify G with the canonical basis of $\mathbf{Z}[G]$. Let M be a $\mathbf{Z}$[G]-module, that is, an abelian group endowed with an action of G respecting its group structure. For any integer $n\geqslant 0$, denote by $C^n(G,M)$ the group of mappings from $G^n$ to M; set $C^n(G,M) = 0$ for $n <0$. Define a homomorphism $d^n: C^n(G,M)\rightarrow C^{n+1}(G,M)$ by the formula

$$
(d^nc)(g_0, . . . , g_n) =g_0c(g_1, . . . , g_n) +^n\sum_{i=0}^{-1}(-1)^{i+1}c(g_0, . . . , g_ig_{i+1}, . . . , g_n)
$$

$$
+ (-1)^{n+1}c(g_0, . . . , g_{n-1})
$$

For any integer $n$, set $Z^n(G,M) =$ Ker $d^n$ and $B^n(G,M) =$ Im $d^n$. a) Prove that $B^n(G,M)$ is contained in $Z^n(G,M)$.

Set $H^n(G,M) = Z^n(G,M)/B^n(G,M)$. The group $H^0(G,M)$ is the set of elements of M fixed by the action of G. The group $Z^1(G,M)$ is the group of mappings $f: G\rightarrow M$ satisfying $f(gg') =f(g) +g f(g')$, and $B^1(G,M)$ is the subgroup of mappings $f$ for which there exists an $m\in M$ such that $f(g) =gm-m$ (cf. I, §6, p. 148, Exercise 7). b) Let N be a $\mathbf{Z}$[G]-module and $u: M\rightarrow N$ a $\mathbf{Z}$[G]-linear mapping. For every integer $n$, the mapping $c\mapsto u\circ c$ is a homomorphism from $C^n(G,M)$ to $C^n(G,N)$ that sends $Z^n(G,M)$ into $Z^n(G,N)$ and $B^n(G,M)$ into $B^n(G,N)$ and therefore induces a homomorphism from $H^n(G,M)$ to $H^n(G,N)$ that we denote by $H^n(G, u)$ or simply $H^n(u)$. If $v: N\rightarrow P$ is a homomorphism of $\mathbf{Z}$[G]-modules, then we have $H^n(v\circ u) = H^n(v)\circ H^n(u)$. c) Let $0\rightarrow M'\rightarrow^{\iota}M\rightarrow^{\pi}M''\rightarrow 0$ be an exact sequence of $\mathbf{Z}$[G]-modules. Let $n$ be an integer and $x''$ an element of $H^n(G,M'')$, the class of an element $c''\in$ $Z^n(G,M'')$. Let $c\in C^n(G,M)$ be such that $\pi \circ c=c''$. Prove that there exists an element $c'\in Z^{n+1}(G,M')$ such that $\iota \circ c'=d^n(c)$ and that the class of $c'$ in $H^{n+1}(G,M')$ depends only on $x''$; we denote that class by $\partial^n(x'')$. The mapping $\partial^n: H^n(G,M'')\rightarrow H^{n+1}(G,M')$ is a homomorphism (“linking homomorphism”). Prove that the sequence

$n'H^n(\iota )nH^n(\pi )n''\partial^nn+1'$

$\cdots  \longrightarrow H(G,M)\longrightarrow H(G,M)\longrightarrow$ H $(G,M)\longrightarrow H(G,M)\longrightarrow  \cdots$

is exact.

2) Let $\varphi : H\rightarrow G$ be a group homomorphism, M a $\mathbf{Z}$[G]-module, N a $\mathbf{Z}$[H]-module, and $u: M\rightarrow N$ a homomorphism of abelian groups. We say that $\varphi$ and $u$ are compatible if we have $u(\varphi (h)x) =hu(x)$ for every $h\in H$ and $x\in M$. a) For $n\geqslant 0$, let $\varphi^n: H^n\rightarrow G^n$ be the mapping deduced from $\varphi$; if $\varphi$ and $u$ are compatible, then the homomorphism $c\mapsto u\circ c\circ \varphi^n$ from $C^n(G,M)$ to $C^n(H,N)$ sends $Z^n(G,M)$ into $Z^n(H,N)$ and $B^n(G,M)$ into $B^n(H,N)$ and therefore induces a homomorphism $H^n(\varphi , u)$ from $H^n(G,M)$ to $H^n(H,N)$. b) Let $\psi : K\rightarrow H$ be another group homomorphism, P a$\mathbf{Z}$[K]-module, and $v: N\rightarrow P$ a homomorphism of abelian groups. If $\varphi$ and $u$ are compatible, and $\psi$ and $v$ also are, then we have $H^n(\varphi \circ \psi , v\circ u) = H^n(\psi , v)\circ H^n(\varphi , u)$. c) Consider a commutative diagram

0 // $M_'$ // M // $M_{''}$ // 0

$u'uu''$

0 // $N_'$ // N // $N_{''}$ // 0 ,

where the first (resp. second) line is an exact sequence of $\mathbf{Z}$[G]-modules (resp. of $\mathbf{Z}$[H]-modules) and where $u', u, u''$ are compatible with $\varphi$. Prove that the diagram

$\cdots$ // $H_n(G,M_')$ // $H_n(G,M)$ // $H_n(G,M_{''})$ // $H_{n+1}(G,M_')$ /$/\cdots$

$H^n(\varphi ,u')H^n(\varphi ,u)H^n(\varphi ,u'')H^{n+1}(\varphi ,u)$

$\cdots$ // $H_n(H,N_')$ // $H_n(H,N)$ // $H_n(H,N_{''})$ // $H_{n+1}(H,N_')$ /$/\cdots$

(whose horizontal lines are the long exact sequences defined in Exercise 1, c)) is commutative. d) Examples: If H = G, then the mapping $u$ is compatible with Id$_G$ if and and only if it is $\mathbf{Z}$[G]-linear, and we have $H^n$(Id$_G, u) = H^n(G, u)$. If N is equal to M endowed with the $\mathbf{Z}$[G]-module structure deduced from $\varphi$, then the homomorphisms $\varphi$ and $1_M$ are compatible; we denote by Res$^q: H^q(G,M)\rightarrow H^q(H,M)$ the homomorphism $H^q(\varphi ,1_M)$ (“restriction homomorphism”). e) Let H be a normal subgroup of G, and let $M^H$ be the subgroup of M consisting of the elements invariant under H, endowed with the action of $G/H$ deduced from that of G by passing to the quotient. The canonical surjection $p: G\rightarrow$ $G/H$ and the canonical injection $j: M^H\rightarrow M$ are compatible; we denote by Inf$^q: H^q(G/H,M^H)\rightarrow H^q(G,M)$ the homomorphism $H^q(p, j)$ (“inflation homomorphism”). Prove that the sequence

$$
0\rightarrow H^1(G/H,M^H)\longrightarrow^{Inf^1}H^1(G,M)\longrightarrow^{Res^1}H^1(H,M)
$$

is exact. If, moreover, $H^1(H,M)$ is zero, then the sequence

$$
0\rightarrow H^2(G/H,M^H)\longrightarrow^{Inf^2}H^2(G,M)\longrightarrow^{Res^2}H^2(H,M)
$$

is exact.

$\P 3)$ Let G be a group and M a $\mathbf{Z}$[G]-module. Let G act on $C^1(G,M)$ by sending $(g, f)\in G\times C^1(G,M)$ to the function $h\mapsto gf(g^{-1}h)$ on G. Recall (I, §6, p. 149, Exercise 8) that a G-mean on M is a $\mathbf{Z}$[G]-linear mapping $µ: C^1(G,M)\rightarrow M$ satisfying $µ(c_x) =x$, where $c_x$ denotes the constant function with value $x\in M$. a) Prove that if M admits a G-mean, then $H^n(G,M)$ is zero for $n\geqslant 1$. (For $q\geqslant 1$, let $h^q: C^q(G,M)\rightarrow C^{q-1}(G,M)$ be the following homomorphism: for $g_1, . . . , g_{q-1}$ in G and $c\in C^q(G,M)$, define $h^q(c)(g_1, . . . , g_{q-1})$ as the image by $µ$ of the function $g\mapsto c(g_1, . . . , g_{q-1},(g_1\cdots g_{q-1})^{-1}g)$. Prove the equality $h^{q+1}\circ d^q+d^{q-1}\circ h^q=$ $1_{C^q(G,M)}.)$ b) Let A be an abelian group; denote by $\mathscr{F}(G,A)$ the group of mappings from G to A, endowed with the action of G defined by $^gf(h) =f(hg)$ for $g, h$ in G and $f$ in $\mathscr{F}(G,A)$. For any mapping $c$ from G to $\mathscr{F}(G,A)$, denote by $µ(c)$ the mapping $g\mapsto c(g^{-1})(g)$ from G to A. Show that $µ$ is a G-mean on $\mathscr{F}(G,A)$; we therefore have $H^q(G,\mathscr{F}(G,A)) = 0$ for $q\geqslant 1$. c) Let $j: M\rightarrow \mathscr{F}(G,M)$ be the mapping that sends an element $m$ of M to the function $g\mapsto gm$, and let $M'$ be its cokernel. Prove that $j$ is injective and $\mathbf{Z}[G]$-linear. Deduce that the homomorphism $\partial^q: H^q(G,M')\rightarrow H^{q+1}(G,M)$ is bijective for $q\geqslant 1$. d) Let L be a finite Galois extension of the commutative field K and G be its Galois group. Deduce from b) and the normal basis theorem (V, §10, No. 9, p. 73) that the groups $H^n(G,L)$ are zero for $n\geqslant 1$.

$\P 4)$ Let G be a group and H a subgroup of G. For any $\mathbf{Z}$[H]-module N, denote by $\widetilde{N}$ the group Hom$_{\mathbf{Z}[H]}(\mathbf{Z}[G],N)$ endowed with a $\mathbf{Z}$[G]-module structure deduced from the right $\mathbf{Z}$[G]-module structure on $\mathbf{Z}[G]$. a) Prove that $\widetilde{N}$ can be identified with the $\mathbf{Z}$[G]-submodule of $\mathscr{F}(G,N)$ (Exercise 3) consisting of the mappings $f$ such that $f(hg) =hf(g)$ for every $h\in H$ and $g\in G$. If A is an abelian group, then the $\mathbf{Z}$[G]-module $\mathscr{F}^(H,A)$ is canonically isomorphic to $\mathscr{F}(G,A)$. b) Let $0\rightarrow N'\rightarrow^iN\rightarrow^pN''\rightarrow 0$ be an exact sequence of $\mathbf{Z}$[H]-modules; the sequence

$'$ Hom(1$,i)$ Hom(1$,p)''$

$$
0\longrightarrow \widetilde{N}---\longrightarrow \widetilde{N}---\longrightarrow \widetilde{N}\longrightarrow 0
$$

is exact (observe that the $\mathbf{Z}$[H]-module $\mathbf{Z}[G]$ is free). c) Let $u_N:\widetilde{N}\rightarrow N$ be the mapping $f\mapsto f(1)$; it is compatible with the canonical injection $i: H\rightarrow G$ (Exercise 2). Prove that the homomorphism

$$
H^q(i, u_N) : H^q(G,\widetilde{N})\rightarrow H^q(H,N)
$$

is bijective for every $q\geqslant 0$ (first treat the case $q= 0$ and then reason by induction on $q$ using the above; Exercise 3, c); and Exercise 2, c)). d) Suppose that H has finite index $n$ in G. Let M be a $\mathbf{Z}$[G]-module, which we view as a $\mathbf{Z}$[H]-module by restriction of scalars. Let $f\in \widetilde{M}$; the element $g^{-1}f(g)$ depends only on the right class $Hg$ of $g$. Set $\pi (f) =\sum_{Hg\in H\backslash G}g^{-1}f(g)$. Prove that $\pi$ is a $\mathbf{Z}$[G]-linear homomorphism from $\widetilde{M}$ to M. For any integer $q\geqslant 0$, denote by Cor$^q: H^q(H,M)\rightarrow H^q(G,M)$ the homomorphism $H^q(\pi )\circ H^q(i, u_M)^{-1}$ (“corestriction homomorphism”). e) Prove that the endomorphism Cor$^q\circ$ Res$^q$ of $H^q(G,M)$ is multiplication by $n$ (first treat the case $q= 0$ and then treat the general case as in the proof of c)). f ) Suppose that G is finite; prove that for every $\mathbf{Z}$[G]-module M and every integer $q\geqslant 1$, the group $H^q(G,M)$ is annihilated by the order of G.

5) Let G be a group and M a not necessarily abelian group endowed with a homomorphism $\varphi : G\rightarrow$ Aut(M); for $g\in G$ and $m\in M$, set $^gm=\varphi (g)(m)$. Denote by $H^0(G,M)$ the subgroup of M consisting of the elements fixed by the action of G; its identity element is called the marked or distinguished element of $H^0(G,M)$. Let $Z^1(G,M)$ be the set of mappings $c: G\rightarrow M$ satisfying $c(gh) =c(g)^gc(h)$ for $g, h$ in G. For $c\in Z^1(G,M)$ and $m\in M$, the mapping $g\mapsto m c(g) (^gm)^{-1}$ belongs to $Z^1(G,M)$; this defines an action of the group M on $Z^1(G,M)$. The quotient set is denoted by $H^1(G,M)$; it is endowed with a marked element, namely the class of the constant mapping with value 1. If M is abelian, then the set $H^1(G,M)$ coincides with that defined in Exercise 1. a) Let N be a second group endowed with an action of G and $u: M\rightarrow N$ a group homomorphism compatible with the actions of G. For $i= 0,1$, define homomorphisms $H^i(u) : H^i(G,M)\rightarrow H^i(G,N)$ that send the marked element of $H^i(G,M)$ to that of $H^i(G,N)$. b) Let $0\rightarrow M'\rightarrow^{\iota}M\rightarrow^{\pi}M''\rightarrow 0$ be an exact sequence of groups with operators in G. Let $x''\in H^0(G,M'')$, and let $x$ be an element of M such that $\pi (x) =x''$. Prove that there exists an element $c'\in Z^1(G,M')$ such that $\iota \circ c'(g) =g^{-1}c(g)$ for every $g\in G$ and that the class of $c'$ in $H^1(G,M')$ depends only on $x''$; we denote that class by $\partial (x'')$. Prove that the sequence

$$
0\rightarrow H^0(G,M')\longrightarrow^{H^0(\iota)}H^0(G,M)-\longrightarrow^{H^0(\pi)}H^0(G,M'')-\rightarrow^{\partial}
$$

$$
H^1(G,M')\longrightarrow^{H^1(\iota)}H^1(G,M)-\longrightarrow^{H^1(\pi)}H^1(G,M'')
$$

is exact (a sequence of mappings $G\rightarrow^iF\rightarrow^pE$, where the set E is endowed with a marked element $e$, is called exact in F if Im($i) =p^{-1}(e))$. c) Suppose, moreover, that $M'$ is contained in the center of M. Construct a mapping $\partial^1: H^1(G,M'')\rightarrow H^2(G,M')$ such that the inverse image of the identity element by $\partial^1$ is the image of $H^1(\pi )$. Also define an action of the group $H^1(G,M')$ on the set $H^1(G,M)$ such that two elements are conjugate for this action if and only if they have the same image by $H^1(\pi )$. d) Let K be a commutative field, L a finite Galois extension of K with Galois group G, and $n$ an integer. Let G act on the group $\mathbf{G}\mathbf{L}_n(L)$ by setting $^{\sigma}A= (\sigma (a_{ij}))$ for $\sigma \in G$ and A $= (a_{ij})\in \mathbf{G}\mathbf{L}_n(L)$. Deduce from V, §10, No. 5, p. 64, Proposition 9 that the set $H^1(G,\mathbf{G}\mathbf{L}_n(L))$ is reduced to one element (“Hilbert’s 90 theorem”).

$\P 6)$ Let L be a finite Galois extension of the commutative field K, with Galois group G. Let V and $V'$ be K-vector spaces and $w$ (resp. $w')$ a tensor of type $(p, q)$ on V (resp. $V')$. An L-isomorphism from $(V, w)$ to $(V', w')$ is an L-linear isomorphism $u: V_{(L)}\rightarrow V'_{(L)}$ such that $u^{\otimes p}\otimes (^tu^{-1})^{\otimes q}$ sends the image of $w$ to that of $w'$. We denote by Aut$_L(V, w)$ the group of L-automorphisms of $(V, w)$, on which G acts by $^{\sigma}\varphi = (1_V\otimes \sigma )\circ \varphi \circ (1_V\otimes \sigma )^{-1}$. a) Let $u$ be an L-isomorphism from $(V, w)$ to $(V', w')$ and $\sigma$ an element of G; the mapping $^{\sigma}u= (1_{V'}\otimes \sigma )\circ u\circ (1_V\otimes \sigma )^{-1}$ is an L-isomorphism from $(V, w)$ to $(V', w')$, so that $c(\sigma ) =u^{-1}\circ^{\sigma}u$ is an element of Aut$_L(V, w)$. Prove that the mapping $c: G\rightarrow$ Aut$_L(V, w)$ belongs to $Z^1(G$, Aut$_L(V, w))$ and that its class $\theta (V', w')$ in $H^1(G$, Aut$_L(V, w))$ does not depend on the choice of $u$. b) Prove that the mapping $(V', t')\mapsto \theta (V', t')$ defines a bijection from the set of K-isomorphism classes of pairs $(V', w')$ L-isomorphic to $(V, w)$ to the set $H^1(G$, Aut$_L(V, w))$. (Given an element $c$ of $Z^1(G$, Aut$_L(V, w))$, deduce from Exercise 5, d) an L-automorphism $f$ of $V_{(L)}$ such that $c(\sigma ) =f^{-1}\circ^{\sigma}f$. Prove that the image $w'$ of $w$ by the automorphism deduced from $f$ is rational over K, and consider the pair $(V, w').)$ $*$c) Examples: The set $H_1(G,\mathbf{S}\mathbf{p}$ (L)) is reduced to one element. If Q is a quadratic

$2n$

form on K, then the set $H^1(G,\mathbf{O}(Q_{(L)}))$ can be identified with the set of equivalence classes of quadratic forms on K equivalent to Q over $L.*$ d) Let A be a K-algebra and M the automorphism group of the L-algebra $A_{(L)}$, endowed with the action of G defined above. The construction in b) defines a bijection from the set of isomorphism classes of pairs $(B, u)$, where B is a K-algebra and $u$ is an isomorphism from $B_{(L)}$ to $A_{(L)}$, to the set $Z^1(G,M)$. The inverse bijection sends an element $c$ of $Z^1(G,M)$ to the K-subalgebra of $A_{(L)}$ consisting of the elements $a$ satisfying $c(\sigma )(\sigma (a)) =a$ for every $\sigma \in G$.

7) Let L be an extension of K. For any integer $n\geqslant 1$, denote by $\mathscr{A}_n(L/K)$ the set of isomorphism classes of central simple K-algebras of degree $n^2$ split by L. a) Prove that the kernel Br(L$/K)$ of the canonical homomorphism Br(K) $\rightarrow$ Br(L) is isomorphic to the direct limit of the sets $\mathscr{A}_n(L/K)$; specify a system of mappings. b) Assume from now on that L is a finite Galois extension of K, with Galois group G. Deduce a bijection $\theta_n:\mathscr{A}_n(L/K)\rightarrow H^1(G,\mathbf{P}\mathbf{G}\mathbf{L}_n(L))$ from Exercise 6. c) Denote by $\partial_n: H^1(G,\mathbf{P}\mathbf{G}\mathbf{L}_n(L))\rightarrow H^2(G,L^*)$ the mapping deduced from the exact sequence $1\rightarrow L^*\rightarrow \mathbf{G}\mathbf{L}_n(L)\rightarrow \mathbf{P}\mathbf{G}\mathbf{L}_n(L)\rightarrow 1$ (Exercise 5, c)) and by $\delta_n:\mathscr{A}_n(L/K)\rightarrow H^2(G,L^*)$ the mapping $\partial_n\circ \theta_n$. If $A\in \mathscr{A}_n(L/K)$, then we have $\delta_n(A) = 0$ if and only if A is a matrix algebra over K; if $A\in \mathscr{A}_p(L/K)$ and $B\in \mathscr{A}_q(L/K)$, then we have $\delta_{pq}(A\otimes_KB) =\delta_p(A) +\delta_q(B)$. Deduce an injective group homomorphism $\delta_{L/K}:$ Br(L$/K)\rightarrow H^2(G,L^*)$ by passing to the direct limit. d) Prove that $\partial_n$ is surjective for $n=$ Card(G). (Let $c: G\times G\rightarrow L^*$ be an element of $Z^2(G,L^*)$. For every $\sigma \in G$, consider the endomorphism $u(\sigma )$ of $L^G$ that sends $e_{\tau}$ to $c(\sigma , \tau )e_{\sigma \tau}$ for every $\tau \in G$, and determine $u(\sigma )^{\sigma}u(\tau )u(\sigma \tau )^{-1}.)$ e) Compare $\delta_{L/K}$ and $Φ_{L/K}$. f ) Prove that the group Br(K) can be identified with the limit of the direct system of groups $H^2$(Gal $(L/K),L^*)$ with respect to the set (ordered by inclusion) of finite Galois extensions of K contained in a fixed algebraic closure of K, where the homomorphisms between these groups are the (injective) inflation homomorphisms. g) Let F be an extension of K contained in L and Γ the subgroup of G that leaves F invariant. Prove that the following diagram commutes:

Br(L$/K)^{r_{F/K}}$ // Br(F$/L)$

$\delta_{L/K}\delta_{F/L}$

$H_2(G,L_*)^{Res^2}/$/ $H_2(Γ,L_*)$.

Deduce a canonical isomorphism from Br(F$/K)$ to the kernel of the homomorphism Res$^2: H^2(G,L^*)\rightarrow H^2(Γ,L^*)$.

8) Let L be an extension of K. Suppose that K has characteristic $p >0$ and $L = K^{1/p}$. Prove that the group Br(L$/K)$ is equal to the kernel of multiplication by $p$ in Br(K) (observe that if N is a finite Galois extension of K, then $N^{1/p}$ is a Galois extension of L with the same Galois group).

9) Let G be a finite group and M a $\mathbf{Z}$[G]-module. Denote by $N_G$ the homomorphism $m\mapsto \sum_ggm$ from M to M; its image is contained in the submodule $M^G$ of M consisting of the invariant elements. Let $T_G(M)$ be the quotient group $M^G/N_G(M)$. a) Let $c\in Z^2(G,M)$. Prove that the element $\sum_hc(h, g)$ belongs to $M^G$; we denote its class in $T_G(M)$ by $\theta_c(g)$. Prove that $\theta_c$ is a homomorphism from G to $T_G(M)$ that is zero when $c\in B^2(G,M)$. Deduce a homomorphism $\theta_M: H^2(G,M)\rightarrow$ Hom(G$,T_G(M))$ from it. b) Let $u: M\rightarrow N$ be a homomorphism of $\mathbf{Z}$[G]-modules and $\widetilde{u}: T_G(M)\rightarrow T_G(N)$ the homomorphism induced by $u$. Prove that we have $\theta_N\circ H^2(u) =$ Hom(1$_G,\widetilde{u})\circ \theta_M$. c) Assume from now on that G is cyclic; let $\sigma$ be a generator of G, and denote its order by $n$. Let $\chi \in$ Hom(G$,\mathbf{Z}/n\mathbf{Z})$ be the homomorphism that sends $\sigma$ to the class of 1, and let $\lambda \in H^2(G,\mathbf{Z})$ be its image by the connecting homomorphism associated with the exact sequence $0\rightarrow \mathbf{Z}\rightarrow \mathbf{Z}\rightarrow \mathbf{Z}/n\mathbf{Z}\rightarrow 0$. Prove that $\lambda$ is the class of the element $\varepsilon \in Z^2(G,\mathbf{Z})$ such that for $0\leqslant p < n$ and $0\leqslant q < n$, the image $\varepsilon (\sigma^p, \sigma^q)$ is equal to 0 if $p+q < n$ and to 1 if $p+q\geqslant n$. For $m\in M^G$, denote by $h_m$ the $\mathbf{Z}$[G]-linear mapping from $\mathbf{Z}$ to M such that $h_m(1) =m$. Prove that the image of $H^2(h_m)(\lambda )$ by $\theta_M$ is equal to the class of $m$, so that $\theta_M$ is surjective. d) Prove that $\theta_M$ is an isomorphism. (Let $c\in Z^2(G,M)$. Prove that we may assume $c(g,1) =c(1, g) = 1$ for every $g\in G$, and determine the images by $d^1$ of the elements $b$ and $a_m(m\in M)$ of $C^1(G,M)$ defined by $b(\sigma^p) =\sum^p_{i=0}^{-1}c(\sigma^i, \sigma )$ and $a_m(\sigma^p) =\sum^p_{i=0}^{-1}\sigma^im.)$

10) a) Let L be a cyclic extension of K. Deduce from Exercises 9 and 7 that the groups Br(L$/K)$ and $K^*/N_{L/K}(L^*)$ are isomorphic. b) Suppose that every extension L of K of finite degree is cyclic and that the norm mapping $N_{L/K}: L^*\rightarrow K^*$ is surjective. Prove that every field extension of K of finite degree with center K is equal to K. c) Apply the previous question to finite fields.

11) Let L be a cyclic extension of K with Galois group G, and let $\sigma$ be a generator of G. Exercise 10 gives a canonical isomorphism Br(L$/K)\rightarrow K^*/N_{L/K}(L^*)$, whose inverse we will now construct explicitly.

Let $\theta \in K^*$, and let $c_{\theta}\in Z^2(G,L^*)$ be the element defined by $c_{\theta}(\sigma^p, \sigma^q) =\theta^{\varepsilon(p,q)}$ (Exercise 9, c)). Prove that the cross product $A[\mathscr{E},L]$ of L and the extension $\mathscr{E}$ associated with $c_{\theta}$ is isomorphic to the quotient of the K-algebra $L[X]_{\sigma}$ (VIII, p. 11) by the (two-sided) ideal generated by the central element $X^n-\theta$. The class of $A_{\theta}$ in Br(L$/K)$ corresponds to the class of $\theta$ (mod $N_{L/K}(L^*))$ by the isomorphism defined above.

12) Let A be a commutative ring. Endow the set of isomorphism classes of Azumaya A-algebras (VIII, p. 270, Exercise 8) with the structure of a monoid by setting cl(S) cl(T) = cl(S $\otimes_AT)$. a) Prove that the quotient monoid for Morita equivalence is an abelian group; we denote it by Br(A) and call it the Brauer group of A (when A is a field, this definition coincides with that given in VIII, p. 279). Denote by [S] the class of an Azumaya A-algebra S in Br(A). The identity element of Br(A) is the class of A, and the inverse of an element [S] is $[S^o]$. b) Let S be an Azumaya A-algebra. We have [S] = [A] if and only if there exists a finitely generated, projective, faithful A-module P such that S is isomorphic to End$_A(P)$. c) Let B be a commutative A-algebra. Define a group homomorphism $r_{B/A}:$ Br(A) $\rightarrow$ Br(B) such that $r_{B/A}([S]) = [S_{(B)}]$ for every Azumaya A-algebra S. We denote the kernel of this homomorphism by Br(B$/A)$.

$\P 13)$ Let A be a commutative ring, B a commutative A-algebra, and G a finite group of automorphisms of the A-algebra B. Suppose that B is a finitely generated, projective, faithful A-module and that the A-linear homomorphism $\psi : B\otimes_AB\rightarrow B^G$ defined by $\psi (b\otimes b') = (\sigma (b)b')_{\sigma\in G}$ is bijective. a) Let N be a B-module, endowed with a homomorphism $\sigma \mapsto u_{\sigma}$ from G to Aut$_A(N)$ satisfying $u_{\sigma}(bx) =\sigma (b)u_{\sigma}(x)$ for $\sigma \in G,b\in B,x\in N$. Let M be the A-submodule of N consisting of the elements $x$ such that $u_{\sigma}(x) =x$ for every $\sigma \in G$. Prove that the canonical B-homomorphism $B\otimes_AM\rightarrow N$ is bijective (use Exercise 7, d) of VIII, p. 270 to reduce to the case when B is the product algebra $A^G$ on which G acts by permuting the factors). b) Let S be an A-algebra and M the automorphism group of the B-algebra $S_{(B)}$, on which G acts by $^{\sigma}\varphi =$ (Id$_S\otimes \sigma )\circ \varphi \circ$ (Id$_S\otimes \sigma )^{-1}$. Extend the construction of Exercise 6 to define a bijection from the set of isomorphism classes of pairs $(T, u)$, where T is an A-algebra and $u$ an isomorphism from $T_{(B)}$ to $S_{(B)}$, to the set $Z^1(G,M)$, as well as a bijection from the set of isomorphism classes of A-algebras T such that the B-algebras $T_{(B)}$ and $S_{(B)}$ are isomorphic to $H^1(G,M)$. c) Assume from now on that every projective B-module is free. Adapt the reasoning of Exercise 8 to construct an isomorphism $\theta :$ Br(B$/A)\rightarrow H^2(G,B^*)$.

$\P 14)$ Let A be a Noetherian commutative local ring, $\mathfrak{m}$ its maximal ideal, $\kappa$ the field $A/\mathfrak{m}$, and S an Azumaya algebra over A. a) Let $e$ be an idempotent in S whose image in $S/\mathfrak{m}S$ is an indecomposable idempotent. Deduce from Nakayama’s lemma (cf. VIII, p. 168, Exercise 16) that the canonical homomorphism $S\rightarrow$ End$_A(Se)$ is bijective. b) Suppose that $\mathfrak{m}$ is nilpotent $*$(or, more generally, that A is complete for the $\mathfrak{m}$-adic topology)$*$. Prove that the homomorphism $r_{\kappa /A}:$ Br(A) $\rightarrow$ Br($\kappa )$ is injective. $*$c) Assume from now on that A is complete. Let L be a separable extension of $\kappa$ of

finite degree that is a splitting field for the $\kappa$-algebra $S/\mathfrak{m}S$. Let $x$ be a primitive element of $L,f$ its minimal polynomial, F a monic polynomial in A[X] whose image in $\kappa [X]$ is $f$, and $B = A[X]/(F)$. Prove that B is a local A-algebra, free and finitely generated as an A-module, with maximal ideal $\mathfrak{m}B$ and residue field isomorphic to L; the B-algebra $S_{(B)}$ is isomorphic to a matrix algebra. d) Suppose, moreover, that L is a Galois extension of $\kappa$, with Galois group G. Prove that the action of G on L lifts to an action on the A-algebra B (let $G'$ be the automorphism group of this algebra; deduce from Hensel’s lemma (Comm. Alg., III, §4, No. 3, p. 215, Theorem 1) that the natural homomorphism $G'\rightarrow G$ is bijective). Deduce from Nakayama’s lemma that the homomorphism $\psi : B\otimes_AB\rightarrow B^G$ defined in Exercise 13 is bijective. e) Prove that the homomorphism $H^q(\pi ) : H^q(G,B^*)\rightarrow H^q(G,L^*)$ is bijective for every $q\geqslant 1$. (For $i\geqslant 1$, let $U^i$ be the subgroup of elements $b$ of $B^*$ such that $b\equiv 1$ (mod $\mathfrak{m}^iB)$. Observe that the $\mathbf{Z}$[G]-module $U^i/U^{i+1}$ is isomorphic to $\mathfrak{m}^iB/\mathfrak{m}^{i+1}B$, hence to a power of L, and deduce from Exercise 5, d) that $H^q(G,U^i/U^{i+1})$ is zero for $q\geqslant 1$. Let $c\in Z^q(G,U^1)$. Construct, by induction, a sequence $(b_n)$ with $b_n\in Z^{q-1}(G,U^n)$ such that $c-d^{q-1}(\sum^n_{i=1}b_i)$ belongs to $Z^q(G,U^{n+1})$. Conclude that $H^q(G,U^1)$ is zero for $q\geqslant 1.)$ f ) Conclude that the canonical homomorphisms Br(B$/A)\rightarrow$ Br(L$/\kappa )$ and Br(A) $\rightarrow$ Br($\kappa )$ are bijective.$*$ $15)*$a) Let A be a regular integral domain (AC, X, §4, n$_o2$, p. 55) and K its field of fractions. The homomorphism $r_{K/A}:$ Br(A) $\rightarrow$ Br(K) is injective (VIII, p. 271, Exercise 11$).*$ b) Prove that the ring $A =\mathbf{Q}[X,Y]/(X^2+ Y^2)$ is an integral domain; let K be its field of fractions. Let H be the quaternion algebra of type $(-1,0,-1)$ over $\mathbf{Q}$, which is a field (cf. III, §2, No. 5, p. 445). Prove that the class of the Azumaya A-algebra $H_{(A)}$ in Br(A) is not zero but that $H_{(K)}$ is isomorphic to $\mathbf{M}_2$(K), so that the homomorphism $r_{K/A}$ is not injective (observe that K contains an element of square $-1)$.

16) a) Prove that the homomorphism $r_{K[X]/K}:$ Br(K) $\rightarrow$ Br(K[X]) induces an isomorphism from Br(K) to a direct factor of Br(K[X]). $*$b) Suppose that the field K is perfect. Prove that $r_{K[X]/K}$ is an isomorphism (deduce from Tsen’s theorem (VIII, p. 360, Exercise 7) that Br(K[X]) is the union of the groups Br(L[X]$/K[X])$, where L runs through the Galois extensions of K of finite degree, and then apply Exercise 13). c) Let A be a regular $\mathbf{Q}$-algebra that is an integral domain. Prove that the homomorphism $r_{A[X]/A}:$ Br(A) $\rightarrow$ Br(A[X]) is bijective (use b) and Exercise 15 to prove that the homomorphism Br(A[X]) $\rightarrow$ Br(A) deduced from the surjection $P\mapsto P(0)$ is injective).$*$ d) Suppose that K has characteristic $p >0$ and is not perfect; let $\theta \in KK^p$. View B = K[U] as a K[X]-algebra via the homomorphism $\rho : K[X]\rightarrow B$ determined by $\rho (X) = U^p-U$. Let $\sigma$ be the automorphism of this K[X]-algebra such that $\sigma (U) = U + 1$, and let S be the quotient K[X]-algebra of $B[V]_{\sigma}$ (VIII, p. 11) by the two-sided ideal $B(V^p-\theta )$. Let L be a K[X]-algebra that is a commutative field. Prove that if the equation $y^p-y= X$ has a solution in L, then $S_{(L)}$ is a matrix algebra over L (let $L'= L[t]/(t^p-\theta )$; consider the homomorphism $S\rightarrow$ End$_L(L')$ that sends V to the multiplication $m_t$ by $t$ and U to $m_y-D$, where D is the L-derivation of $L'$ such that $D(t) =t)$. In the opposite case, $S_{(L)}$ is a central simple L-algebra; it is a matrix algebra if and only if $\theta$ is the norm of an element of the extension $L[Y]/(Y^p-Y-X)$ of L (apply Exercise 11).

Deduce that S is an Azumaya K[X]-algebra and that its class in Br(K[X]) does not come from Br(K) (take L = K(X)).

$*17)$ Suppose that the field K is complete for a discrete valuation $v$, assumed normed (cf. Exercise 12 of VIII, p. 272); denote the ring of $v$ by A and its residue field by $\kappa$. The homomorphism $r_{\kappa /A}:$ Br(A) $\rightarrow$ Br($\kappa )$ is bijective (Exercise 14); denote by $\iota :$ Br($\kappa )\rightarrow$ Br(K) the homomorphism $r_{A/K}\circ r_{\kappa /}^{-1}_A$. a) Let L be an unramified Galois extension of K of finite degree, with Galois group G. Let B be the valuation ring of $v_L$ extending $v$ and $\kappa_L$ be its residue field. The homomorphism $\iota$ induces a homomorphism $\iota_L:$ Br($\kappa_L/\kappa )\rightarrow$ Br(L$/K)$. Construct a split exact sequence

$0\rightarrow$ Br($\kappa_L/\kappa )\longrightarrow^{\iota_L}$ Br(L$/K)\rightarrow H^2(G,\mathbf{Z})\rightarrow 0$,

where $\mathbf{Z}$ is endowed with the trivial action of G (observe that the exact sequence of $\mathbf{Z}$[G]-modules $0\rightarrow B^*\rightarrow L^*\longrightarrow^{v_L}\mathbf{Z}$ splits, and use Exercise 14). b) Let G be a group. Using the exact sequence $0\rightarrow \mathbf{Z}\rightarrow \mathbf{Q}\rightarrow \mathbf{Q}/\mathbf{Z}\rightarrow 0$, prove that the linking homomorphism of Exercise 1 induces an isomorphism from Hom(G$,\mathbf{Q}/\mathbf{Z})$ to $H^2(G,\mathbf{Z})$. c) Conclude that we have a split exact sequence

$0\rightarrow$ Br($\kappa )\rightarrow^{\iota}$ Br(K) $\rightarrow Ξ(\mathfrak{g},\mathbf{Q}/\mathbf{Z})\rightarrow 0$,

where $\mathfrak{g}$ is the Galois group of a separable closure of $\kappa$ over $\kappa$ and $Ξ(\mathfrak{g})$ is the group of continuous homomorphisms from $\mathfrak{g}$ to $\mathbf{Q}/\mathbf{Z}$, endowed with the discrete topology (pass to the direct limit using Exercise 12 of VIII, p. 272 and the fact that every finite Galois extension of $\kappa$ is the residue field extension of an unramified finite Galois extension of K, unique up to isomorphism). d) Deduce that Br(K) $=\{0\}$ if $\kappa$ is algebraically closed. e) Suppose that the field $\kappa$ is finite, in other words, that K is a finite extension of a $p$-adic field or a field of formal power series over a finite field. Construct an isomorphism from Br(K) to $\mathbf{Q}/\mathbf{Z}.*$
