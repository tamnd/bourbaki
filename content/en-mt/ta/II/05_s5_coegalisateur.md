---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 5
section_title: Coégalisateur
lang: en
source: ta-i-iv-fr
book_pages: TA II.196-TA II.214, TA II.227-TA II.228
pdf_pages: 0212-0230, 0243-0244
extraction: native
subsections:
    - "no": 1
      title: Contraction des flèches d’une homotopie
      page: 196
      pdf_page: 212
    - "no": 2
      title: Définition du coégalisateur
      page: 199
      pdf_page: 215
    - "no": 3
      title: Comparaison des groupes d’isotropie du cohomotopeur et du coégalisateur
      page: 201
      pdf_page: 217
    - "no": 4
      title: Groupe d’isotropie d’un coégalisateur
      page: 206
      pdf_page: 222
    - "no": 5
      title: Quotient d’un groupoïde par l’action d’un groupe
      page: 210
      pdf_page: 226
statements: 22
exercises: 3
content_sha256: 711dd705966b5505898a3e12ce8803f21dfe784179862e01ca5ae334296e89f9
translated_from: content/fr/ta/II/05_s5_coegalisateur.md
source_lang: fr
translation_method: machine
source_content_sha256: c6621f3052830a86807effbd63135f54125cae6481244086852339122e66081a
translation_model: gpt-5.4
translation_run: translate-en-mt-16968d00
glossary_version: 34
glossary_terms_sha256: e8952ea4da11d71e10e9d693b755c7bf6647a27753198f75c9be6ca3416d35ca
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. COEQUALIZER

### 1. Contraction of the arrows of a homotopy

Let H be a quiver, let G be a groupoid, let $\varphi$ and $\psi$ be quiver morphisms of H into G, and let $h:$ Som(H) $\rightarrow$ Fl(G) be a homotopy connecting $\varphi$ to $\psi$. Let $G'$ be the groupoid deduced from G by contraction of the arrows of the image of $h($II, p. 175, No.$^o11$) and let $\beta : G\rightarrow G'$ be the canonical morphism.

Let us denote by Γ the quiver (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )). By definition of a homotopy, the pair (Id$_{Som(G)}, h$) is a quiver morphism of Γ into G; it extends to a unique groupoid morphism $\eta :$ Grp(Γ) $\rightarrow$ G. By construction, the set of vertices of $G'$ is the set of connected components of the quiver Γ.

In all that follows in this No.$^o$, we shall suppose that the groupoid G is transitive. According to remark 1 of II, p. 170, this amounts to supposing that the groupoid $G'$ is so. We also fix a vertex $a_0$ of G.

Let us denote by $\widetilde{\Gamma}$ the graph associated with the quiver Γ (cf. II, p. 156). The set of loops of length $\geqslant 1$ in $\widetilde{\Gamma}$ is identified with the set $\Omega (\widetilde{\Gamma})$ of finite sequences $(z_1, . . . , z_n)$, where $n$ is an integer such that $n\geqslant 1$ and $z_1, . . . , z_n$ are elements of Fl($\widetilde{\Gamma}$) such that $t(z_i) =o(z_{i+1})$ for every integer $i$ such that $1\leqslant i < n$ and $t(z_n) =o(z_1)$.

Let $\mathbf{z}= ((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ be an element of $\Omega (\widetilde{\Gamma})$. The conjugacy class of the element

Int($g$)$(\eta (\mathbf{z})) =gh(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}g^{-1}$

in $G_{a_0}$ does not depend on the choice of the arrow $g$ of G joining the vertex $a_0$ to the origin of $(b_1, \varepsilon )$. We denote this conjugacy class by $c(\mathbf{z})$.

#### Proposition 1 {#ta-ii-s5-prop-1 .statement tag=01UI}

The group morphism $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$ is surjective, and its kernel is the smallest subgroup of $G_{a_0}$ containing the conjugacy classes $c(\mathbf{z})$ for $\mathbf{z}\in \Omega (\widetilde{\Gamma})$.

Let K be the smallest distinguished subgroupoid of G whose set of arrows contains the image of $h$. The morphism $G_{a_0}\rightarrow G'_{\beta(a_0)}$ is surjective and its kernel is equal to $K_{a_0}($II, p. 170, prop. 2). The proposition then follows from prop. 8 of II, p. 176.

#### Definition 1 {#ta-ii-s5-def-1 .statement tag=01UJ}

A subset Z of $\Omega (\widetilde{\Gamma})$ is said to be distinguished (relative to the pair $(\varphi , \psi )$) if it satisfies the following properties:

(i) For every arrow $z$ of $\widetilde{\Gamma}$, one has $(z, z)\in Z$ ;

(ii) For every $(z_1, . . . , z_n)\in$ Z, one has $(\overline{z}_n, . . . ,\overline{z}_2,\overline{z}_1)\in$ Z and $(z_n, z_1, . . . , z_{n-1})\in Z$ ;

(iii) Let $\mathbf{z}= (z_1, . . . , z_n)$ and $\mathbf{z}'= (z'_1, . . . , z'_m)$ be elements of Z such that $t(z_n) =o(z'_1)$. Put $\mathbf{z}\mathbf{z}'= (z_1, . . . , z_n, z'_1, . . . , z'_m)$. If two elements among $\mathbf{z},\mathbf{z}',\mathbf{z}\mathbf{z}'$ belong to Z, the same is true of the third;

(iv) For every arrow $f$ of H, put $\widetilde{\varphi}(f,1) =\widetilde{\psi}(f,-1) =$ $\varphi (f)$ and $\widetilde{\varphi}(f,-1) =\widetilde{\psi}(f,1) =\psi (f)$. Let $n$ be an integer $\geqslant$ 1 and $(f_1, \varepsilon_1), . . . ,(f_n, \varepsilon_n)$ a sequence of elements of Fl(H) $\times  \{-1,1\}$ such that $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ for $1\leqslant i < n$ and $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$; let $a_i$ denote the origin of $f_i$ and $b_i$ its term. In order that $((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ belong to Z, it is necessary and sufficient that $((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ belong to Z.

The intersection in $\Omega (\widetilde{\Gamma})$ of every family of distinguished subsets (relative to $(\varphi , \psi )$) is again distinguished. In particular, there exists a smallest distinguished subset containing a given subset Z of $\Omega (\widetilde{\Gamma})$.

#### Proposition 2 {#ta-ii-s5-prop-2 .statement tag=01UK}

If N is a distinguished subgroup of $G_a$, the set of elements $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ such that $c(\mathbf{z})$ is contained in N is a distinguished subset of $\Omega (\widetilde{\Gamma})$.

Let Z denote the set of elements $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ such that $c(\mathbf{z})\subset N$.

Let $z\in$ Fl($\widetilde{\Gamma}$). We have $c(z, z) =\{e_a\}$ by definition, whence $(z, z)\in Z$.

Let $(z_1, . . . , z_n)\in Z$. By definition of $c$, the conjugacy class $c(z_1, . . . , z_n)$ is equal to $c(z_n, z_1, . . . , z_{n-1})$ and is formed by the inverses of the elements of $c(\overline{z}_n, . . . ,\overline{z}_1)$. This shows that Z satisfies condition (ii).

With the notation of condition (iii), one can choose elements $u\in c(\mathbf{z}),v\in c(\mathbf{z}')$ and $w\in c(\mathbf{z}\mathbf{z}')$ such that $uv=w$. If two of the elements $u,v$ and $w$ belong to N, the same is true of the third, therefore N satisfies (iii).

The notation being that of (iv), we have, for every integer $i$ such that $1\leqslant i\leqslant n$, the relation

$$
\varphi (f_i)h(b_i) =h(a_i)\psi (f_i)
$$

for $h$ is a homotopy joining $\varphi$ to $\psi$. This equality can also be written

$$
\widetilde{\varphi}(f_i, \varepsilon_i)h(b_i)^{\varepsilon_i}=h(a_i)^{\varepsilon_i}\widetilde{\psi}(f_i, \varepsilon_i)
$$

Taking into account the relations $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ for $1\leqslant i < n$ and $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$, one deduces

$$
\widetilde{\varphi}(f_1, \varepsilon_1)h(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}=h(a_1)^{\varepsilon_1}. . . h(a_n)^{\varepsilon_n}\widetilde{\varphi}(f_1, \varepsilon_1)
$$

so that the conjugacy classes $c((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ and $c((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ are equal. This shows that Z satisfies condition (iv) and completes the proof of the proposition.

#### Corollary {#ta-ii-s5-n1-cor-1 .statement tag=01UL}

Let Z be a subset of $\Omega (\widetilde{\Gamma})$; in order that the conjugacy classes $c(\mathbf{z})$, for $\mathbf{z}\in$ Z, generate the kernel of the canonical homomorphism $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$, it is enough that the smallest distinguished subset of $\Omega (\widetilde{\Gamma})$ containing Z be equal to $\Omega (\widetilde{\Gamma})$.

Let N be the smallest subgroup of $G_{a_0}$ containing $c(\mathbf{z})$ for every $\mathbf{z}\in Z$; it is distinguished. Let $Z'$ be the set of elements $\mathbf{z}$ of $\Omega (\widetilde{\Gamma})$ such that $c(\mathbf{z})\in N$. By proposition 2, $Z'$ is a distinguished subset of $\Omega (\widetilde{\Gamma})$. It contains Z. By hypothesis, it is therefore equal to $\Omega (\widetilde{\Gamma})$. It then follows from prop. 1 (II, p. 197) that N is the kernel of the homomorphism $\beta_a$.

### 2. Definition of the coequalizer

Let H be a quiver, let G be a groupoid and let $\varphi ,\psi$ be morphisms of quivers from H into G. Let us denote by Coh($\varphi , \psi$ ) the cohomotopizer of the pair $(\varphi , \psi )$ (II, p. 185, def. 3)$,\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) the canonical groupoid morphism and $h$ the canonical homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$.

Let Coeg($\varphi , \psi$ ) be the groupoid obtained from Coh($\varphi , \psi$ ) by contraction of the arrows belonging to the image of $h$ (II, p. 196, n$^o$ 1), let us denote by $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) the canonical morphism and let us put $\gamma =\beta \circ \alpha$.

#### Definition 2 {#ta-ii-s5-def-2 .statement tag=01UM}

The groupoid Coeg($\varphi , \psi$ ) is called the coequalizer of the pair $(\varphi , \psi )$; the groupoid morphism $\gamma$ is called the canonical morphism from G into Coeg($\varphi , \psi$ ).

#### Proposition 3 {#ta-ii-s5-prop-3 .statement tag=01UN}

The pair (Coeg($\varphi , \psi$ )$, \gamma$ ) has the following universal property:

a) We have $\gamma \circ \varphi =\gamma \circ \psi$.

b) Let $G'$ be a groupoid and let $\theta : G\rightarrow G'$ be a groupoid morphism such that $\theta \circ \varphi =\theta \circ \psi$. There exists a unique groupoid morphism $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ such that $\overline{\theta}\circ \gamma =\theta$.

Let $a$ be a vertex of H. The arrow $h(a)$ of Coh($\varphi , \psi$ ) joins $\alpha (\varphi (a))$ to $\alpha (\psi (a))$. By definition of the groupoid Coeg($\varphi , \psi$ ), the origin and the end of the arrow $\beta (h(a))$ are equal; therefore we have $\gamma (\varphi (a)) =\gamma (\psi (a))$.

Let $f$ be an arrow of H; if $a$ denotes its origin and $b$ its end, we thus have

$$
\alpha (\varphi (f))\cdot h(b) =h(a)\cdot \alpha (\psi (b))
$$

Taking the image by $\beta$ of the two members of this equality, one obtains the relation $\gamma (\varphi (f)) =\gamma (\psi (f))$. This proves assertion a).

Let us prove b). The mapping $\eta :$ Som(H) $\rightarrow$ Fl(G$'$) which associates with every vertex $a$ of H the arrow $e_{\theta(\varphi(a))}$ of $G'$ is a homotopy joining $\theta \circ \varphi$ to $\theta \circ \psi$. By the universal property of cohomotopizers (II, p. 185, prop. 3), there exists a unique groupoid morphism $\theta_1:$ Coh($\varphi , \psi$ )$\rightarrow G'$ such that $\theta_1\circ \alpha =\theta$ and $\theta_1(h(a)) =e_{\theta(\varphi(a))}$ for every vertex $a$ of H. By prop. 7 of II, p. 176, this latter property implies the existence of a unique groupoid morphism $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ such that $\overline{\theta}\circ \beta =\theta_1$. One then has $\overline{\theta}\circ \gamma =\theta_1\circ \alpha =\theta$.

Conversely, if $\overline{\theta}':$ Coeg($\varphi , \psi$ )$\rightarrow G'$ is a groupoid morphism such that $\overline{\theta}'\circ \gamma =\theta$, one has $(\overline{\theta}'\circ \beta )\circ \alpha = (\overline{\theta}\circ \beta )\circ \alpha$, whence $\overline{\theta}'\circ \beta =\overline{\theta}\circ \beta$ by II, p. 185, prop. 3, whence $\overline{\theta}'=\overline{\theta}$ by prop. 7 of II, p. 176. This proves the uniqueness of $\overline{\theta}$, hence assertion b).

#### Corollary {#ta-ii-s5-n2-cor-1 .statement tag=01UO}

The groupoid Coeg($\varphi , \psi$ ) is generated by the image of the morphism $\gamma$.

Let C be the subgroupoid of Coeg($\varphi , \psi$ ) generated by the image of G; let $i$ denote the canonical morphism of C into Coeg($\varphi , \psi$ ) and $\theta : G\rightarrow C$ the morphism such that $i\circ \theta =\gamma$. By proposition 2, there exists a unique groupoid morphism $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow C$ such that $\overline{\theta}\circ \gamma =\theta$. Then $\gamma =i\circ \overline{\theta}\circ \gamma$, hence $i\circ \overline{\theta}$ is the identity morphism of Coeg($\varphi , \psi$ ) (loc. cit.). In particular, the mappings Som($i$) and Fl($i$) are surjective, therefore C = Coeg($\varphi , \psi$ ).

#### Remark 1 {#ta-ii-s5-n2-rem-1 .statement tag=01UP}

The set of vertices of Coeg($\varphi , \psi$ ) is the set of connected components of the quiver

Γ = (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ ))

(II, p. 197). In other words, it is the quotient set of Som(G) by the finest equivalence relation such that $\varphi (a)$ is equivalent to $\psi (a)$ for every $a\in$ Som(G).

#### Remark 2 {#ta-ii-s5-n2-rem-2 .statement tag=01UQ}

The mapping Orb($\gamma$ ), deduced from $\gamma$ by passing to orbits, defines by passage to the quotient a bijection of the set of connected components of the framework of the pair $(\varphi , \psi )$ onto the set of orbits of the coequalizer. This results from II, p. 185, prop. 4 and from the fact that the mapping deduced from $\beta$ by passing to orbits is bijective ( II, p. 170, remark 1).

Consequently, the mapping of Som(G) into Orb(Coeg($\varphi , \psi$ )) deduced from $\gamma$ identifies the set of orbits of Coeg($\varphi , \psi$ ) with the quotient set of Som(G) by the equivalence relation generated by the pairs $(\varphi (x), \psi (x))$ for $x\in$ Som(H) and the pairs $(o(f), t(f))$ for $f\in$ Fl(G).

#### Remark 3 {#ta-ii-s5-n2-rem-3 .statement tag=01UR}

The mapping Fl($\gamma$ ) of Fl(G) into Fl(Coeg($\varphi , \psi$ )) is not in general surjective.

### 3. Comparison of the isotropy groups of the cohomotopizer and the coequalizer

Let H be a quiver, let G be a groupoid, and let $\varphi$ and $\psi$ be morphisms of quivers from H into G. Let us denote by $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ), $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) and $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) the canonical morphisms of groupoids, and by $h$ the canonical homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$. These notations are summarized by the following diagram

$\gamma$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )$^{\beta}$ Coeg($\varphi , \psi$ ) .

In the whole remainder of this n$^o$, we suppose that the framework of the pair $(\varphi , \psi )$ is a connected quiver and we fix a vertex $a_0$ of G. Consequently, the groupoids Coh($\varphi , \psi$ ) and Coeg($\varphi , \psi$ ) are transitive.

Let Γ denote the quiver (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )), $\widetilde{\Gamma}$ the graph associated with Γ, and let $\Omega (\widetilde{\Gamma})$ be the set of finite sequences $(z_1, . . . , z_n)$ of arrows of $\widetilde{\Gamma}$, with $n\geqslant 1$, such that the terminus of $z_i$ is the origin of $z_{i+1}$ if $1\leqslant i < n$ and that the terminus of $z_n$ is the origin of $z_1$. In No. 1 there was constructed a mapping $\mathbf{z}\mapsto c(\mathbf{z})$ of the set $\Omega (\widetilde{\Gamma})$ into the set of conjugacy classes of the group Coh($\varphi , \psi$ )$_{a_0}$.

Let $H\times_GH$ denote the equalizer in $H\times H$ of the quiver morphisms $\psi \circ$pr$_1$ and $\varphi \circ$pr$_2$. The set of its vertices is the set of pairs $(a, b)$ of vertices of H such that $\psi (a) =\varphi (b)$; the set of its arrows is the set of pairs $(f, g)$ of arrows of H such that $\psi (f) =\varphi (g)$; the origin of an arrow $(f, g)$ is the vertex $(o(f), o(g))$ and its term is the vertex $(t(f), t(g))$ (cf. II, p. 153).

Finally, let Ker($\varphi , \psi$ ) denote the equalizer of $\varphi$ and $\psi$; recall (II, p. 165, example 2) that this is the subquiver of H whose vertices $a$ are those such that $\varphi (a) =\psi (a)$ and whose arrows are the $f\in$ Fl(H) such that $\varphi (f) =\psi (f)$.

#### Proposition 4 {#ta-ii-s5-prop-4 .statement tag=01US}

Let $\mu: H\times_GH\rightarrow H$ be a quiver morphism such that $\varphi \circ \mu=\varphi \circ$ pr$_1$ and $\psi \circ \mu=\psi \circ$ pr$_2$. Suppose that, for every pair $(a, b)$ of vertices of H such that $\varphi (a) =\varphi (b)$, there exists a vertex $c$ of H such that $\varphi (c) =\psi (b)$ and $a=\mu(b, c)$.

Let $A_1$ be a set of vertices of Ker($\varphi , \psi$ ) meeting each of its connected components and let $Z_1$ be the set of elements of $\Omega (\widetilde{\Gamma})$ of the form $((a,1))$, where $a\in A_1$. Let also $A_2$ be a set of vertices of $H\times_GH$ meeting each connected component of $H\times_GH$ and let $Z_2$ be the set of triples of the form $((a,1),(b,1),(\mu(a, b),-1))$, as $(a, b)$ ranges over $A_2$.

Then $\Omega (\widetilde{\Gamma})$ is the smallest distinguished subset of $\Omega (\widetilde{\Gamma})$ containing $Z_1\cup Z_2$. In particular, the conjugacy classes $c(\mathbf{z})$ in Coh($\varphi , \psi$ )$_{a_0}$, where $\mathbf{z}$ ranges over $Z_1\cup Z_2$, generate the kernel of the canonical homomorphism $\beta_a$ of Coh($\varphi , \psi$ )$_{a_0}$ into Coeg($\varphi , \psi$ )$_{\beta(a_0)}$.

Let $Z'_1,Z'_2$ and $Z'$ denote the smallest distinguished subsets of $\Omega (\widetilde{\Gamma})$ containing respectively $Z_1,Z_2$ and $Z_1\cup Z_2($II, p. 197, definition 1). It is required to prove that $Z'$ is equal to $\Omega (\widetilde{\Gamma})$; by II, p. 199, Corollary 1 of Proposition 1 of II, p. 197, the last assertion of the proposition will follow.

#### Lemma 1 {#ta-ii-s5-lem-1 .statement tag=01UT}

a) For every vertex $a$ of Ker($\varphi , \psi$ ), $((a,1))$ belongs to $Z'_1$.

b) For every vertex $(a, b)$ of $H\times_GH$, $((a,1),(b,1),(\mu(a, b),-1))$ belongs to $Z'_2$.

a) Let $A'_1$ be the set of vertices $a$ of Ker($\varphi , \psi$ ) such that $((a,1))$ belongs to $Z'_1$. We have $A_1\subset A'_1$, by definition of $Z'_1$. Let $f$ be an arrow of Ker($\varphi , \psi$ ), let $a$ be its origin and $b$ its end. It follows from property (iv) in the definition of a distinguished subset (II, p. 197, definition 1) applied to the sequence $((f,1))$ that $a\in A'_1$ is equivalent to $b\in A'_1$. Since $A_1$ meets every connected component of Ker($\varphi , \psi$ ), we have $A'_1=$ Som(Ker($\varphi , \psi$ )), which was to be proved.

b) Let $A'_2$ be the set of vertices $(a, b)$ of $H\times_GH$ such that the triple $((a,1),(b,1),(\mu(a, b),-1))$ belongs to $Z'_2$. By hypothesis, we have $A_2\subset A'_2$. Since $A_2$ meets each connected component of $H\times_GH$, it is enough to establish that, if there exists an arrow $(f, f')$ joining a vertex $(a', b')$ to a vertex $(a, b)$, then $(a, b)$ belongs to $A'_2$ if and only if analogously for $(a', b')$.

Put $f''=\mu(f, f')$; this is an arrow joining $\mu(a', b')$ to $\mu(a, b)$, and one has $\varphi (f'') =\varphi (f)$ and $\psi (f'') =\psi (f')$. By condition (iv) in the definition of a distinguished subset of $\Omega (\widetilde{\Gamma})$ (loc. cit.) applied to the sequence $((f,1),(f',1),(f'',-1))$, the two conditions

(i) the triple $((a,1),(b,1),(\mu(a, b),-1))$ belongs to $Z'$;

(ii) the triple $((a',1),(b',1),(\mu(a', b'),-1))$ belongs to $Z'$;

are equivalent. This shows that $(a, b)$ belongs to $A'_2$ if and only if $(a', b')$ belongs to $A'_2$ and completes the proof of the lemma.

Let us now prove by induction on the integer $n\geqslant 1$ that every element $((a_1, \varepsilon_1),(a_2, \varepsilon_2), . . . ,(a_n, \varepsilon_n))$ of $\Omega (\widetilde{\Gamma})$ belongs to $Z'$.

A) Case in which $n= 1$.

Let $((a, \varepsilon ))$ be an element of $\Omega (\widetilde{\Gamma})$ of length 1. We have $\varphi (a) =\psi (a)$, whence $((a,1))\in Z'$ by lemma 1. Condition (ii) in the definition of a distinguished subset then implies that $((a,-1))$ belongs to $Z'$.

B) Case in which $n\geqslant 2$.

By virtue of condition (ii) for a distinguished subset, it is enough to treat the case in which $\varepsilon_2= 1$. Suppose that $\varepsilon_1= 1$; then $(a_1, a_2)$ is a vertex of $H\times_GH$; put $a=\mu(a_1, a_2)$; by lemma 1, the triple $((a_1,1),(a_2,1),(a,-1))$ therefore belongs to $Z'$. In the case in which $\varepsilon_1=-1$, we have $\varphi (a_1) =\varphi (a_2)$; we can therefore choose a vertex $a$ of H such that $\mu(a_2, a) =a_1$ and the triple $((a_2,1),(a,1),(a_1,-1))$ belongs to $Z'$, hence the triple $((a_1,-1),(a_2,1),(a,1))$ also, by virtue of condition (ii) in the definition of a distinguished subset.

Then $((a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))$ belongs to $\Omega (\widetilde{\Gamma})$ and is of length $n-1$. By induction, it is an element of $Z'$. By virtue of conditions (i), (ii) and (iii) in the definition of a distinguished subset, we deduce successively that the elements

$$
((a_1, \varepsilon_1),(a_2,1),(a,-\varepsilon_1),(a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))
$$

$$
((a,-\varepsilon_1),(a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n),(a_1, \varepsilon_1),(a_2,1))
$$

$$
((a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n),(a_1, \varepsilon_1),(a_2,1))
$$

$$
((a_1, \varepsilon_1),(a_2,1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))
$$

belong to $Z'$. This completes the proof of the proposition.

#### Corollary {#ta-ii-s5-n3-cor-1 .statement tag=01UU}

a) With the notation of proposition 4, suppose moreover that the mapping (Som($\varphi$ ), Som($\psi$ )) of Som(H) into Som(G) $\times$ Som(G) is injective and that its image is the graph of an equivalence relation in Som(G). Then, for every vertex $(a, b)$ of $H\times_GH$, there exists a unique vertex $c_{a,b}$ of H such that $\varphi (c_{a,b}) =\varphi (a)$ and $\psi (c_{a,b}) =\psi (b)$.

b) Suppose further that for every arrow $(f, f')$ of $H\times_GH$, there exists an arrow $f''$ of H such that $\varphi (f'') =\varphi (f)$ and $\psi (f'') =\psi (f')$.

Let A be a set of vertices of $H\times_GH$ meeting each of its connected components. Then, the kernel of the morphism $\beta_{a_0}$ is the smallest distinguished subgroup of Coh($\varphi , \psi$ )$_{a_0}$ containing the conjugacy classes $c((a,1),(b,1),(c_{a,b},-1))$, for $(a, b)\in A$.

Let R be the equivalence relation in Som(G) whose graph is the image of the mapping (Som($\varphi$ ), Som($\psi$ )). Let $(a, b)$ be a vertex of $H\times_GH$. Then we have $R\{\varphi (a), \psi (a)\}$ and $R\{\varphi (b), \psi (b)\}$, whence $R\{\varphi (a), \psi (b)\}$ since $\psi (a) =\varphi (b)$. Consequently, there exists a unique vertex $c$ of H such that $\varphi (c) =\varphi (a)$ and $\psi (c) =\psi (b)$; we denote it by $\mu(a, b)$.

For every arrow $(f, f')$ of $H\times_GH$, choose an arrow $f''$ of H such that $\varphi (f'') =\varphi (f)$ and $\psi (f'') =\psi (f)$ and denote it by $\mu(f, f')$.

Thus a quiver morphism $\mu: H\times_GH\rightarrow H$ has been defined such that $\varphi \circ \mu=\varphi \circ$ pr$_1$ and $\psi \circ \mu=\psi \circ$ pr$_2$.

Let $(a, b)$ be a pair of vertices of H such that $\varphi (a) =\varphi (b)$. We have $R\{\varphi (a), \psi (a)\}$ and $R\{\varphi (b), \psi (b)\}$, hence $R\{\psi (b), \psi (a)\}$. Consequently there exists a unique vertex $c$ of H such that $\varphi (c) =\psi (b)$ and $\psi (c) =\psi (a)$. The vertex $\mu(b, c)$ satisfies $\varphi (\mu(b, c)) =\varphi (b) =\varphi (a)$ and $\psi (\mu(b, c)) =$ $\psi (c) =\psi (a)$. Hence $\mu(b, c) =a$ because the mapping (Som($\varphi$ ), Som($\psi$ )) of Som(H) into Som(G) $\times$ Som(G) is injective.

Let $A_1$ be the set of vertices of Ker($\varphi , \psi$ ) and let $Z_1$ be the set of elements of $\Omega (\widetilde{\Gamma})$ of the form $((a,1))$, for $a\in A_1$. Put $A_2= A$ and let $Z_2$ be the set of elements $((a,1),(b,1),(\mu(a, b),-1))$ of $\Omega (\widetilde{\Gamma})$, for $(a, b)\in A_2$. Let $\widetilde{Z}$ (resp. $\widetilde{Z}_1$, resp. $\widetilde{Z}_2$) denote the smallest distinguished subset of $\Omega (\widetilde{\Gamma})$ containing $Z_1\cup Z_2$ (resp. $Z_1$, resp. $Z_2$).

Let $a\in A_1$; one has $\varphi (a) =\psi (a)$ ; let us put $x=\varphi (a)$. The vertex $a$ is the unique vertex of H such that $\varphi (a) =\psi (a) =x$; in particular, one has $\mu(a, a) =a$. The triplet $((a,1),(a,1),(a,-1))$ therefore belong to $Z_2$. It then follows from conditions (i) and (iii) in the definition of a distinguished subset that $((a,1))$ belong to $\widetilde{Z}_2$. Consequently, one has $Z_1\subset \widetilde{Z}_2$, whence $\widetilde{Z} =\widetilde{Z}_2$.

By Proposition 4, $\Omega (\widetilde{\Gamma})$ is the smallest distinguished subset of $\Omega (\widetilde{\Gamma})$ containing $Z_2$ and the kernel of $\beta_{a_0}$ is the smallest distinguished subgroup of Coh($\varphi , \psi$ )$_{a_0}$ containing the conjugacy classes $c(\mathbf{z})$, for $\mathbf{z}\in Z_2$, whence the corollary.

#### Example {#ta-ii-s5-n3-exa-1 .statement tag=01UV}

Let X and R be topological spaces, let $o$ and $t$ be continuous mappings of R into X, let C be the set of pairs $(f, g)\in R^2$ such that $t(f) =o(g)$ in R, and let $m$ be a continuous mapping of C into R making the quiver $(X,R, o, t)$ into a groupoid; suppose moreover that the mapping $f\mapsto f^{-1}$ of R into R is continuous. Then the hypotheses of the proposition are satisfied if one puts $H =\varpi (R)$, $G =\varpi (X),\varphi =\varpi (o),\psi =\varpi (t)$ and $\mu=\varpi (m)$.

Suppose further that R is the graph of an equivalence relation in X, the mappings $o$ and $t$ being deduced from the projections of $X\times X$ into X by passing to the subspaces. Then the hypotheses of the corollary are satisfied.

#### Remark {#ta-ii-s5-n3-rem-1 .statement tag=01UW}

*More generally, the hypotheses of the proposition are satisfied when $(G,H, \varphi , \psi , \mu)$ is a "groupoid of groupoids." This means that G and H are groupoids, $\varphi$ and $\psi$ are groupoid morphisms of H into G, making the quadruplet $(G,H, \varphi , \psi )$ into a "quiver in groupoids"; finally, $\mu$ is a law of composition in this "quiver" given by a groupoid morphism $H\times_GH\rightarrow H$, satisfying a certain number of properties expressing the associativity of the law and the fact that every "arrow" is invertible. The reader will moreover remark that the mappings to the fundamental groupoid studied in this work all fall under this case.*

### 4. Isotropy Group of a Coequalizer

Let G and H be groupoids; let $\varphi$ and $\psi$ be groupoid morphisms of H into G. The purpose of this No. is to summarize the calculus of the isotropy groups of the cohomotopizer (II, p. 193, prop. 6) and the comparison of the isotropy groups of the cohomotopizer and of the coequalizer made in the preceding No. in order to deduce from it the calculus of the isotropy groups of the coequalizer Coeg($\varphi , \psi$ ).

Let us denote by $\alpha : G\rightarrow$ Coh($\varphi , \psi$ )$,\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) and $\gamma =\beta \circ$ $\alpha : G\rightarrow$ Coeg($\varphi , \psi$ ) the canonical groupoid morphisms. Let us denote by $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) the canonical homotopy; let us recall that the set of vertices of Coh($\varphi , \psi$ ) is equal to Som(G).

Let $\Gamma$ denote the quiver (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )); let then $\varphi_0$ and $\psi_0$ denote the mappings deduced from $\varphi$ and $\psi$ by passing to orbits and $\Gamma_0$ the framework (Orb(G), Orb(H)$, \varphi_0, \psi_0$) of the pair $(\varphi , \psi )$. We shall assume that the quiver $\Gamma_0$ is connected and that the set of its vertices is not empty, which amounts to assuming that the groupoids Coh($\varphi , \psi$ ) and Coeg($\varphi , \psi$ ) are transitive.

Recall (cf. II, p. 192, definition 4) that a basic equipment consists in the data of a family $(a, b, c_1, c_2,T, i_0)$ where: for every $i\in$ Orb(G)$,a(i)$ is a vertex in the orbit $i$ of G; for every $j\in$ Orb(H)$,b(j)$ is a vertex in the orbit $j$ of H$,c_1(j)$ and $c_2(j)$ are arrows of G joining respectively $\varphi (b(j))$ to $a(\varphi_0(j))$ and $\psi (b(j))$ to $a(\psi_0(j))$; T is a subquiver of $\Gamma_0$ whose associated tree is a maximal tree of the graph $\widetilde{\Gamma}_0$; finally, $i_0$ is an orbit of G and one sets $a_0=a(i_0)$.

One then defines a morphism of quivers $\tau_0$ from $\Gamma_0$ into Coh($\varphi , \psi$ ) such that $\tau_0(i) =\beta (a(i))$ and $\tau_0(j) =\alpha (c_1(j))^{-1}h(b(j))\alpha (c_2(j))$ for $i\in$ Orb(G) and $j\in$ Orb(H). If $i$ belongs to Orb(G), let $d_i$ be the unique class of paths in the graph $\widetilde{T}$ joining $i_0$ to $i$, and let $\delta_i$ denote its image in Coh($\varphi , \psi$ ) under the morphism of groupoids $\tau_0$.

From these data, Prop. 6 (II, p. 193) yields a surjective homomorphism

$\Lambda :(_{i\in\pi}*_{_0(G)}G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

and describes generators of its kernel, thus providing a presentation of the group Coh($\varphi , \psi$ )$_{a_0}$.

The set of loops of length $\geqslant 1$ in the graph $\widetilde{\Gamma}$ associated to Γ is identified with the set $\Omega (\widetilde{\Gamma})$ of sequences $(z_1, . . . , z_n)$ of arrows of $\widetilde{\Gamma}$, indexed by $\mathbf{Z}/n\mathbf{Z}$, where $n$ runs through the set of integers $\geqslant 1$, such that for every $k\in \mathbf{Z}/n\mathbf{Z}$, the terminus of $z_k$ is the origin of $z_{k+1}$. Let Z be a subset of $\Omega (\widetilde{\Gamma})$ such that the conjugacy classes $c(z)$, for $z\in Z$, generate the kernel of the surjective homomorphism $\beta_{a_0}$. The homomorphism $\beta_{a_0}\circ \Lambda$ is surjective; to deduce its kernel, that is to say a presentation of the group Coeg($\varphi , \psi$ )$_{\beta(a_0)}$, it remains to choose, for every $z\in Z$, an element $C(z)$ in the group $(*G_{a(i)})*F(\pi_0(H))$

$i\in$Orb(G)

such that $\Lambda (C(z))$ belongs to the conjugacy class $c(z)$.

Let therefore $z= (z_1, . . . , z_n)$ be an element of $\Omega (\widetilde{\Gamma})$; put $z_k= (y_k, \varepsilon_k)$, where $y_k\in$ Fl(Γ) = Som(H) and $\varepsilon_k\in  \{\pm 1\}$. By definition, $c(z)$ is the conjugacy class of the element

$$
gh(y_1)^{\varepsilon_1}. . . h(y_n)^{\varepsilon_n}g^{-1}
$$

of the groupoid Coh($\varphi , \psi$ )$_{a_0}$, where $g$ is an arbitrary arrow in Coh($\varphi , \psi$ ) joining $a_0$ to the origin of $z_1$. For $k\in \mathbf{Z}/n\mathbf{Z}$, let $j_k$ be the orbit of $y_k$ in H and choose an arrow $f_k$ of H joining $y_k$ to the vertex $b(j_k)$. By definition of a homotopy, one then has the relation

$$
h(y_k)(\alpha \circ \psi )(f_k) = (\alpha \circ \varphi )(f_k)h(b(j_k))
$$

in the groupoid Coh($\varphi , \psi$ ). Consequently, using the definition of the quiver morphism $\tau_0$, one has

$$
h(y_k) = (\alpha \circ \varphi )(f_k)\cdot h(b(j_k))\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \tau_0(j_k)\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \delta_{\varphi_0(j_k)}^{-1}\cdot
$$

$$
\cdot \delta_{\varphi_0(j_k)}\cdot \tau_0(j_k)\cdot \delta_{\psi_0(j_k)}^{-1}\cdot
$$

$$
\cdot \delta_{\psi_0(j_k)}\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
=u_k\Lambda (j_k)v_k
$$

where we have put

$u_k=\alpha (\varphi (f_k)c_1(j_k))\cdot \delta_{\varphi_0(j_k)}^{-1}$ and $v_k=\delta_{\psi_0(j_k)}\cdot \alpha (\psi (f_k)c_2(j_k))^{-1}$. For every element $k\in \mathbf{Z}/n\mathbf{Z}$, define arrows $\widetilde{u}_k,\widetilde{v}_k$ in G by

$$
h(y_k)^{\varepsilon_k}=\widetilde{u}_k\Lambda (j_k)^{\varepsilon_k}\widetilde{v}_k
$$

so that

$(u_k, v_k)$ if $\varepsilon_k= 1$ ;

$$
(\widetilde{u}_k,\widetilde{v}_k) =_{--}
$$

$(v_k^1, u_k^1)$ if $\varepsilon_k=-1$.

Let $x_k$ denote the origin of the arrow $h(y_k)^{\varepsilon_k}$; its end is then $x_{k+1}$; let $i_k$ be the orbit of $x_k$. We then define a loop $\lambda_k(z)$ at $a(i_k)$ in the groupoid G by the formula

(1)

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ if $(\varepsilon_{k-1}, \varepsilon_k) = (1,1)$;

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ if $(\varepsilon_{k-1}, \varepsilon_k) = (1,-1)$; $\lambda_k(z) =$

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ if $(\varepsilon_{k-1}, \varepsilon_k) = (-1,1)$;

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ if $(\varepsilon_{k-1}, \varepsilon_k) = (-1,-1)$. By construction, one has

$$
\Lambda (\lambda_k(z)) =\widetilde{v}_{k-1}\widetilde{u}_k
$$

so that the image under the homomorphism Λ of the element

$$
C(z) =\lambda_1(z)(j_1)^{\varepsilon_1}\lambda_2(z)(j_2)^{\varepsilon_2}. . . \lambda_n(z)(j_n)^{\varepsilon_n} \tag{2}
$$

belongs to the conjugacy class $c(z)$.

#### Definition 3 {#ta-ii-s5-def-3 .statement tag=01UX}

Let G and H be groupoids; let $\varphi$ and $\psi$ be morphisms of groupoids from H into G. Suppose that the groupoid Coeg($\varphi , \psi$ ) is transitive. Let $(a, b, c_1, c_2,T, i_0)$ be a basic equipment of the pair $(\varphi , \psi )$.

A complementary equipment is the data of a subset Z of $\Omega (\widetilde{\Gamma})$ such that the conjugacy classes $c(\mathbf{z})$ for $\mathbf{z}\in$ Z generate the kernel of the homomorphism $\beta_{a(i_0)}$ and, for every element $\mathbf{z}= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))$ of Z, of a sequence $f(\mathbf{z}) = (f_1, . . . , f_n)$ of arrows in H such that $f_k$ joins $y_k$ to the vertex $b(j_k)$, $j_k$ denoting the orbit of $y_k$ in H.

A complete equipment of the pair $(\varphi , \psi )$ is the data of a basic equipment and of a complementary equipment.

#### Proposition 5 {#ta-ii-s5-prop-5 .statement tag=01UY}

Let G and H be groupoids; let $\varphi$ and $\psi$ be morphisms of groupoids from H into G. Suppose that the groupoid Coeg($\varphi , \psi$ ) is transitive. Let $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) denote the canonical morphism of groupoids.

Let us endow the pair $(\varphi , \psi )$ with a complete equipment

$$
(a, b, c_1, c_2,T, i_0,Z,(f(\mathbf{z}))_{\mathbf{z}\in Z})
$$

For $j\in$ Orb(H), let $\varphi_j: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$ and $\psi_j: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$ be the group homomorphisms Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}$ and Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}$ respectively, where $\varphi_0$ and $\psi_0$ denote the canonical mappings deduced from $\varphi$ and $\psi$ by passing to orbits. Let $\tau$ be the morphism of the framework $\Gamma_0$ of the pair $(\varphi , \psi )$ into Coeg($\varphi , \psi$ ) defined by Som($\tau$ )$(i) =\gamma (a(i))$ if $i\in$ Orb(G) and such that Fl($\tau$ )$(j)$ is the path $\gamma (c_1(j))^{-1}\gamma (c_2(j))$ in Coeg($\varphi , \psi$ ). If $i$ is an orbit of G, let $c_i$ be the unique class of paths in $\widetilde{T}$ joining $i_0$ to $i$ and put $\delta_i=\widetilde{\tau}(c_i)$, where $\widetilde{\tau}:$ Grp(G) $\rightarrow$ Coeg($\varphi , \psi$ ) is the canonical groupoid morphism deduced from $\tau$.

There then exists a unique group homomorphism

$\lambda :(*G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coeg($\varphi , \psi$ )$_{\gamma(a(i_0))}$

$i\in$Orb(G)

such that

$\lambda (f) =\delta_i\gamma_{a(i)}(f)\delta_i^{-1}$ for $i\in$ Orb(G) and $f\in G_{a(i)}$,

$\lambda (j) =\delta_{\varphi_0(j)}\tau (j)\delta_{\psi_0(j)}^{-1}$ for $j\in$ Orb(H).

The homomorphism $\lambda$ is surjective; its kernel is the smallest normal subgroup containing the following elements:

($R_1$)$r_1(j) =j$ for $j$ in Fl(T) ;

($R_2$)$r_2(j, f) =\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$

for $j\in$ Orb(H) and $f\in H_{b(j)}$;

($R_3$)$r_3(z) =\lambda_1(z)j_1^{\varepsilon_1}\lambda_2(z)j_2^{\varepsilon_2}. . . \lambda_n(z)j_n^{\varepsilon_n}$

for $z= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))\in Z$,

where the loops $\lambda_i(z)$ are defined by formula (1), p. 208.

The existence and uniqueness of such a morphism result from the universal property of the free product of a family of groups (A, I, p. 85, prop. 8). Let us denote by $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) and $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) the canonical morphisms, so that $\gamma$ = $\beta \circ \alpha$. Let also $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) be the canonical homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$. Since $\beta$ is the groupoid morphism obtained by contraction of the arrows in the image of $h$, we have

Fl($\tau$ )$(j) =\gamma (c_1(j))^{-1}\gamma (c_2(j)) =\gamma (c_1(j)^{-1})\beta (h(j))\gamma (c_2(j)) =\beta (\tau_0(j))$ in Coeg($\varphi , \psi$ ), where $\tau_0: \Gamma_0\rightarrow$ Coh($\varphi , \psi$ ) denotes the quiver morphism deduced from the basic equipment $(a, b, c_1, c_2,T, i_0)$. Consequently, the homomorphism $\lambda$ is the composite of the homomorphism Λ defined in prop. 6 (II, p. 193) and the surjective homomorphism $\beta_{a(i_0)}$. In particular it is surjective.

Let $z\in Z$; by construction, $\Lambda (r_3(z))$ belongs to the conjugacy class $c(z)$. By definition of a complementary equipment, the kernel of the homomorphism $\beta_{a(i_0)}$ is therefore the smallest invariant subgroup of Coh($\varphi , \psi$ )$_{a(i_0)}$ containing the elements $\Lambda (r_3(z))$ for $z\in Z$. Since the homomorphism Λ is surjective, the kernel of the homomorphism $\lambda =\beta_{a(i_0)}\circ \Lambda$ is therefore the smallest invariant subgroup of the group $(*G_{a(i)})*F(\pi_0(H))$ containing the generators of the kernel

$i\in$Orb(G)

of Λ given by formulae ($R_1$)$, (R_2)$, together with the elements defined by formulae ($R_3$). The proposition is thus proved.

### 5. Quotient of a groupoid by the action of a group

Let G be a transitive groupoid, let K be a group, and let $\theta : K\rightarrow$ Aut(G)$^{\circ}$ be a group homomorphism of K into the opposite group of the automorphism group of the groupoid G. We shall say that the group K acts on the right on G. If $k\in K$, we shall sometimes denote by $k^*x$ (resp. $k^*f$) the image of a vertex $x$ (resp. of an arrow $f$) of G under the groupoid automorphism $\theta (k)$.

Let $|K|$ be the groupoid whose set of vertices is K and whose set of arrows joining two vertices is empty if these vertices are distinct, and is reduced to one element otherwise. Let H be the product groupoid $G\times  |K|$; a vertex of H is a pair $(a, k)$, where $a$ is a vertex of G and $k$ is an element of K; if $f$ is an arrow of G joining a vertex $a$ to a vertex $b$, we shall denote by $(f, k)$ the unique arrow of H joining $(a, k)$ to $(b, k)$. Let $\varphi : H\rightarrow G$ be the groupoid morphism given by the first projection and let $\psi : H\rightarrow G$ be the groupoid morphism such that Som($\psi$ )$((a, k)) =k^*a$ and Fl($\psi$ )$((f, k)) =k^*f$ if $k\in K,a\in$ Som(G) and $f\in$ Fl(G).

Let us denote by $G/K$ the coequalizer Coeg($\varphi , \psi$ ) and let $\gamma : G\rightarrow G/K$ be the canonical groupoid morphism.

Let $o$ be a vertex of G. For $k\in K$, choose an arrow $c_k$ joining $k^*o$ to $o$ in G; there exists one since G is transitive. For $k\in K$, let us denote by Fix($k$) the subgroupoid of G whose vertices (resp. arrows) are the elements of Som(G) (resp. of Fl(G)) fixed by $k$; choose a set $A_k$ of vertices of Fix($k$) meeting all the orbits of this groupoid. For $k\in K$ and $a\in A_k$, choose also an arrow $f_{(a,k)}$ in G joining the vertex $a$ to the vertex $o$.

#### Proposition 6 {#ta-ii-s5-prop-6 .statement tag=01UZ}

The unique group homomorphism

$$
\lambda : G_o*F(K)\rightarrow (G/K)_{\gamma(o)}
$$

such that $\lambda (f) =\gamma_o(f)$ for $f\in G_o$ and $\lambda ([k]) =\gamma (c_k)$ for $k\in K$ is surjective. Its kernel is the smallest normal subgroup of $G_o*F(K)$ containing the following elements:

($R_2$)$r_2(k, f) = [k]^{-1}f[k](c^{-1}_kk^*(f)^{-1}c_k)$

for $k\in K$ and $f\in G_o$;

($R'_3$)$r'_3(k, a) = [k](c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)}))$

for $k\in K-\{e\}$ and $a\in A_k$

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})$

for $k$ and $h\in K$.

Since G is transitive, the mapping which to an element $k\in K$ associates the orbit of $(o, k)$ is a bijection of K onto the set of orbits of H. Thus Orb(G) is identified with $\{o\}$ and Orb(H) with K. The framework $\Gamma_0$ of the pair $(\varphi , \psi )$ is then identified with the quiver having a unique vertex $o$ and whose set of arrows is K. Let T be the subquiver of $\Gamma_0$ with set of vertices $\{o\}$ and whose set of arrows is empty; the associated graph is the unique maximal tree of the graph $\widetilde{\Gamma}_0$.

The family $(o,(o, k)_{k\in K},(e_o)_{k\in K},(c_k)_{k\in K},T, o)$ is a basic equipment of the pair $(\varphi , \psi )$.

The mapping $f\mapsto (f, k)$ defines an isomorphism of the isotropy group $G_o$ onto the isotropy group $H_{(o,k)}$; by means of this isomorphism, the homomorphisms $\varphi_k$ and $\psi_k$ of $H_{(o,k)}$ into $G_o$ defined by Prop. 5 of II, p. 208 are given by

(3) $\varphi_k(f, k) =f$ et $\psi_k(f, k) =c^{-1}_kk^*(f)c_k$,

for $k\in K$ and $f\in G_o$.

The quiver $H\times_GH$ is the equalizer in $H\times H$ of the quiver morphisms $\psi \circ$ pr$_1$ and $\varphi \circ$ pr$_2$. Its vertices are the pairs $((a, k),(b, h))$ where $a$ and $b$ are vertices of G and $k$ and $h$ elements of K such that $b=k^*a$, and its arrows are the pairs $((f, k),(g, h))$ where $f$ and $g$ are arrows of G, and $k$ and $h$ elements of K such that $g=k^*f$; the origin of the arrow $((f, k),(g, h))$ is equal to $((o(f), k),(o(g), h))$; its end is equal to $((t(f), k),(t(g), h))$.

One then defines a quiver morphism $\mu$ from $H\times_GH$ into H by putting $\mu((a, k),(b, h)) = (a, kh)$ and $\mu((f, k),(g, h)) = (f, kh)$. We have $\varphi \circ \mu=\varphi \circ$ pr$_1$ and $\psi \circ \mu=\psi \circ$ pr$_2$.

Let $x$ and $y$ be vertices of H such that $\varphi (x) =\varphi (y)$. Then there exist a vertex $a$ of G and elements $k$ and $h$ of K such that $x= (a, k)$ and $y= (a, h)$. Put $z= (h^*a, h^{-1}k)$; then $\mu(y, z) =x$. This shows that the pair $(\varphi , \psi )$ satisfies the hypotheses of Prop. 4 (II, p. 202).

A vertex $(a, k)$ of H belong to the groupoid Ker($\varphi , \psi$ ), equalizer of $\varphi$ and $\psi$, if and only if $k^*a=a$, that is to say, if $k$ belong to the stabilizer of the vertex $a$ in the group K. Let $A_1$ be the set of pairs $(a, k)$, for $k\in K$ and $a\in A_k$; it meets all the orbits of the subgroupoid Ker($\varphi , \psi$ ) of H. Let $Z_1$ be the subset of $\Omega (\widetilde{\Gamma})$ formed by the sequences of the form $(((a, k),1))$, for $(a, k)\in A_1$. For $\mathbf{z}= ((a, k),1)\in Z_1,(f_{(a,k)}, k)$ is an arrow of H joining $(a, k)$ to $(o, k)$. Put $f(\mathbf{z}) = ((f_{(a,k)}, k))$.

The set $A_2$ of vertices of $H\times_GH$ of the form $((o, k),(k^*o, h))$, for $(k, h)\in K^2$, meets all the orbits of $H\times_GH$. Observe also that one has $\mu((o, k),(k^*o, h)) = (o, kh)$. The arrows $(e_o, k)$, $(c_k, h)$, $(e_o, kh)$ in H join respectively $(o, k)$, $(k^*o, h)$, $(o, kh)$ to $(o, k)$, $(o, h)$ and $(o, kh)$. Let $Z_2$ denote the set of sequences of the form $(((o, k),1),((k^*o, h),1),((o, kh),-1))$ in $\Omega (\widetilde{\Gamma})$; for such an element $\mathbf{z}$ of $Z_2$, put $f(\mathbf{z}) = ((e_o, k),(c_k, h),(e_o, kh))$.

By Prop. 4 of II, p. 202, the set $Z = Z_1\cup Z_2$ and the family $(f(\mathbf{z}))_{z\in Z}$ is a complementary equipment.

Let $k\in K$ and let $a\in A_k$. The element $C((a, k),1)$ of the group $G_o*F(K)$ defined by formula (2) of II, p. 208 is equal to

$$
c^{-1}_k\psi ((f_{(a,k)}, k))^{-1}\varphi (f_{(a,k)})e_o[k] =(c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)})[k] \tag{4}
$$

Let $k$ and $h\in K$ be given. One verifies that the element

$$
C(((o, k),1),((k^*o, h),1),((o, kh),-1))
$$

of the group $G_o*F(K)$ defined by formula (2) of II, p. 208 is equal to

$$
[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})[kh]^{-1} \tag{5}
$$

The elements $r'_3(e, a)$ given by the relations ($R'_3$) for $k=e$ are all equal to $[e]c^{-1}_e$, an element of the group $G_o*F(K)$ which one obtains by applying the relation ($R''_3$) to $k=h=e$. Taking account of relations (3), (4), and (5), the proposition therefore follows from II, p. 208, Prop. 5.

#### Corollary 1 {#ta-ii-s5-prop-6-cor-1 .statement tag=01V0}

Suppose that the group K is generated by the stabilisers of the vertices of G. Then the group homomorphism $\gamma_o: G_o\rightarrow (G/K)_{\gamma(o)}$ is surjective. Moreover, if the groupoid G is simply transitive, the same is true of the groupoid $G/K$.

The relation ($R''_3$) implies $\lambda ([e]) =\lambda (c_e) =\gamma_o(c_e)$. The relations ($R''_3$) then imply that the set of $k\in K$ such that $\lambda ([k])$ belong to the image of $\gamma_o$ is a subgroup of K. Finally, the relations ($R'_3$) show that, for every element $k\in K$ whose stabiliser is not empty, $\lambda ([k])$ belong to the image of $\gamma_o$. The corollary follows.

#### Remark 1 {#ta-ii-s5-n5-rem-1 .statement tag=01V1}

One can give another description, sometimes more convenient, of the group $(G/K)_{\gamma(o)}$. For this, let $M = K\times G_o$ and define a law of composition in M by the formula

$$
(k, a)\cdot (h, b) = (kh, c^{-1}_{kh}h^*(c_ka)c_hb)
$$

for $k,h\in K$ and $a,b\in G_o$. One verifies that this law of composition is associative, that $(e, c^{-1}_e)$ is an identity element, and that the element $(k^{-1}, c^{-1_1}_{k^-}(k^{-1})^*(c_ka)^{-1}c_e)$ is the inverse of $(k, a)$. It therefore endows M with a group structure. Moreover, the mapping $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ defined by $(k, a)\mapsto \lambda ([k]a)$ is a group homomorphism. Let $\alpha '$ be the unique group morphism of $G_o*F(K)$ into M such that $\alpha '(f) =$ $(e, f)$ if $f\in G_o$ and $\alpha '([k]) = (k, e_o)$ if $k\in K$; one has $\lambda '\circ \alpha '=\lambda$.

The relations ($R_2$) and ($R''_3$) show that every element of $(G/K)_{\gamma(o)}$ is the image under the homomorphism $\lambda$ of an element of $G_o*F(K)$ of the form $[k]f$, with $f\in G_o$ and $k\in K$. Hence the homomorphism $\lambda '$ is surjective. One verifies moreover that the image under $\alpha '$ of an element of $G_o*$ F(K) of the form $(R_2)$ or $(R''_3)$ is equal to the identity element. Consequently, the kernel of the homomorphism $\lambda '$ is the smallest normal subgroup of M containing the images under $\alpha '$ of the elements of $G_o*F(K)$ of the form ($R'_3$).

#### Corollary 2 {#ta-ii-s5-prop-6-cor-2 .statement tag=01V2}

Suppose that the group K operates freely on Som(G). There then exists a unique group homomorphism $\pi : (G/K)_{\gamma(o)}\rightarrow$ K whose kernel contains the image of $\gamma_o$ and such that $\pi (\lambda ([k])) =k$ for every $k\in K$. Moreover, $G_o\longrightarrow^{\gamma_o}(G/K)_{\gamma(o)}-\rightarrow^{\pi}$ K is an extension of K by $G_o$.

If such a group homomorphism $\pi$ exists, the group homomorphism $\pi \circ \lambda$ is necessarily equal to the unique group homomorphism $p$ from $G_o*F(K)$ into K such that $p(f) =e$ for $f\in G_o$ and $p([k]) =k$. It is immediate to verify that the elements of $G_o*F(K)$ defined by formulas ($R_2$) and ($R''_3$) belong to the kernel of $p$. By assumption, there is no element of type ($R'_3$). Thus, the kernel of the morphism $\lambda$ contains that of $p$. Consequently, there exists a unique group homomorphism $\pi : (G/K)_{\gamma(o)}\rightarrow K$ such that $\pi \circ \lambda =p$.

It is evident that the homomorphism $\pi$ is surjective. To prove that the homomorphism $\gamma_o$ is injective and that its image is exactly the kernel of $\pi$, let us remark that the homomorphism $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ (II, p. 213, remark 1) is an isomorphism, since it has been assumed that K operates freely on Som(G). The composite homomorphism $(\lambda ')^{-1}\circ \gamma_o$ from $G_o$ into M is given by $f\mapsto (e, f)$, whereas the homomorphism $\pi \circ \lambda ': M\rightarrow K$ maps $(k, f)$ to $k$. The corollary follows.

#### Corollary 3 {#ta-ii-s5-prop-6-cor-3 .statement tag=01V3}

Suppose that the groupoid G is simply transitive. Let $K_0$ be the subgroup of K generated by the stabilizers of the vertices of G. The mapping from K into $(G/K)_{\gamma(o)}$ which to $k\in K$ associates $\gamma (c_k)$ is a surjective group homomorphism, with kernel $K_0$.

If an element $k\in K$ fixes a vertex $a$ of G, the element $g^{-1}kg$ fixes the vertex $g^*a$; this implies that $K_0$ is a normal subgroup of K.

By proposition 5, the unique homomorphism $\lambda : F(K)\rightarrow$ $(G/K)_{\gamma(o)}$ such that $\lambda ([k]) =\gamma (c_k)$ is surjective, and its kernel is the smallest normal subgroup of F(K) containing the elements $[k]$, where $k$ is an element of K which fixes a vertex of G, and the elements $[kh]^{-1}[k][h]$, where $(k, h)\in K^2$. In particular, the mapping $\lambda ': K\rightarrow (G/K)_{\gamma(o)}$, defined by $\lambda '(k) =\gamma (c_k) =\lambda ([k])$ for $k\in K$, is a group homomorphism. One has $\lambda =\lambda '\circ p$, where $p: F(K)\rightarrow K$ denotes the canonical surjective group homomorphism. Consequently, the homomorphism $\lambda '$ is surjective and its kernel is the smallest normal subgroup of K which contains the elements $k$, for $k$ fixing a vertex of G, that is to say $K_0$. This proves the proposition.

## EXERCISES {#ta-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
