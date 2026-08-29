---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 5
section_title: Théorème de van Kampen
lang: en
source: ta-i-iv-fr
book_pages: TA IV.405-TA IV.436, TA IV.463-TA IV.477
pdf_pages: 0421-0452, 0479-0493
extraction: native
subsections:
    - "no": 1
      title: Coégalisateur des projections d’un carré fibré
      page: 405
      pdf_page: 421
    - "no": 2
      title: Recouvrements
      page: 409
      pdf_page: 425
    - "no": 3
      title: Cas particulier d’un recouvrement formé de deux parties
      page: 421
      pdf_page: 437
    - "no": 4
      title: Espaces quotients
      page: 424
      pdf_page: 440
    - "no": 5
      title: Cônes ; contraction d’un sous-espace
      page: 425
      pdf_page: 441
    - "no": 6
      title: Éclatement et recollement
      page: 429
      pdf_page: 445
statements: 31
exercises: 34
content_sha256: 84e9569f0eddb7fac79bf16826926ee8cb4b772f7dd4d387346d3742ab8abf2a
translated_from: content/fr/ta/IV/05_s5_theoreme_de_van_kampen.md
source_lang: fr
translation_method: machine
source_content_sha256: c9cb3c126ca51430bcfdf8f79aa2c3b874dfc666fe3ef32ccf2a87eeb6f4025f
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-en-mt-6c72ca22
glossary_version: 34
glossary_terms_sha256: cb277f4e684964334e365e17b870d4028125a3c69a7e591928174c2605138984
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. VAN KAMPEN THEOREM

### 1. Coequalizer of the projections of a fibre square

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Denote by Z the fibre square $X\times_YX$ and by $p_1,p_2$ the two projections of Z into X. Denote by W the fibre product $X\times_YX\times_YX$; for every pair $(s, t)$ of integers equal to 1, 2 or 3, denote by $q_{st}: W\rightarrow Z$ the mapping defined by $q_{st}(x_1, x_2, x_3) = (x_s, x_t)$.

Denote by Coeg($f$) the groupoid Coeg($\varpi (p_1), \varpi (p_2)$), coequalizer of the two morphisms $\varpi (p_1),\varpi (p_2)$ of the Poincaré groupoid $\varpi (Z)$ into the Poincaré groupoid $\varpi (X)$. Denote by $\gamma :\varpi (X)\rightarrow$ Coeg($f$) the canonical morphism of groupoids. Since $f\circ p_1$ = $f\circ p_2$, the morphisms of groupoids $\varpi (f)\circ \varpi (p_1)$ and $\varpi (f)\circ \varpi (p_2)$ of $\varpi (Z)$ into $\varpi (Y)$ are equal; there thus exists a unique morphism of groupoids $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ such that $\varpi '(f)\circ \gamma =\varpi (f)$.

#### Definition 1 {#ta-iv-s5-def-1 .statement tag=0230}

One says that the mapping $f$ satisfies the property (VK) if it is strict, surjective and if the morphism $\varpi '(f)$ is an isomorphism.

#### Example 1 {#ta-iv-s5-n1-exa-1 .statement tag=0231}

This property is satisfied under one of the following assumptions:

(i) The spaces X and Y are delacable, the space $X\times_YX$ is locally arcwise connected, the mapping $f$ is surjective, proper, separated, with locally connected fibres;

(ii) The spaces X and Y are delacable, the mapping $f$ is surjective, proper, separated, with finite fibres, the diagonal $\Delta_X$ of $X\times_YX$ is open and its complement is locally connected;

(iii) The spaces X and Y are delacable, the mapping $f$ is surjective, open and possesses the path lifting property;

(iv) Every point of Y possesses a neighbourhood above which there exists a continuous section of the mapping $f$.

Indeed, under each of these assumptions, the mapping $f$ is surjective; it is also strict by virtue of I, p. 18, example 2. Finally, the morphism $\varpi '(f)$ is an isomorphism, both under the assumptions (i), (ii) or (iii) according to IV, p. 398, th. 1, and under assumption (iv) ( IV, p. 400, th. 2).

The prop. 5 of II, p. 208 describes the isotropy groups of the groupoid Coeg($f$). The purpose of this no$^o$ is to make explicit, when $f$ satisfies the property (VK), the description of the Poincaré groups of Y which is deduced from it by composition with the isomorphism of groupoids $\varpi '(f)$. The following nos$^{os}$ will be devoted to important particular cases.

Suppose that the mapping $f$ satisfies the property (VK).

Put $\mathsf{I}=\pi_0(X),\mathsf{J}=\pi_0(Z),\mathsf{K}=\pi_0(W)$; for $j\in \mathsf{J}$ and $s\in  \{1,2\}$, put $i_s(j) =\pi_0(p_s)(j)$ ; for $k\in \mathsf{K}$ and $s,t\in  \{1,2,3\}$, put $j_{st}(k) =\pi_0(q_{st})(k)$. Denote by $\mathsf{\Gamma}$ the skeleton of the pair $(\varpi (p_1), \varpi (p_2))$ of morphisms of groupoids from $\varpi (Z)$ into $\varpi (X)$ (II, p. 185, def. 3). It is the quiver $(\mathsf{I},\mathsf{J}, \pi_0(p_1), \pi_0(p_2))$, since the orbits of the Poincaré groupoid of a topological space are the arcwise connected components of this space.

Suppose moreover that Y is arcwise connected and nonempty. According to II, p. 200, remark 2, $\pi_0(\mathsf{\Gamma})$ is then in bijection with the set of orbits of the groupoid Coeg($f$); since the mapping $f$ satisfies the property (VK), the groupoid Coeg($f$) is isomorphic to the groupoid $\varpi (Y)$. The graph $\mathsf{\Gamma}$ is thus connected and nonempty.

Call van Kampen data of $f$ the data of the following elements:

(i) for every $i\in \mathsf{I}$, a point $\mathsf{a}(i)$ of the path-connected component $i$ of X ;

(ii) for every $j\in \mathsf{J}$, a point $\mathsf{b}(j) = (\mathsf{b}_1(j),\mathsf{b}_2(j))$ of the path-connected component $j$ of Z ;

(iii) for every $k\in \mathsf{K}$, a point $\mathsf{c}(k) = (\mathsf{c}_1(k),\mathsf{c}_2(k),\mathsf{c}_3(k))$ of the path-connected component $k$ of W;

(iv) for every $j\in \mathsf{J}$, the class $\beta_1(j)$ of a path in X joining $\mathsf{b}_1(j)$ to $\mathsf{a}(i_1(j))$ and the class $\beta_2(j)$ of a path in X joining $\mathsf{b}_2(j)$ to $\mathsf{a}(i_2(j))$;

(v) for every $k\in \mathsf{K}$ and for every pair $(s, t)$ equal to $(1,2)$, $(2,3)$ or $(1,3)$, the class $\gamma_{st}(k)$ of a path in Z joining $(\mathsf{c}_s(k),\mathsf{c}_t(k))$ to $\mathsf{b}(j_{st}(k))$;

(vi) a subquiver $\mathsf{T}$ of $\mathsf{\Gamma}$ whose associated graph is a maximal tree of the graph $\widetilde{\mathsf{\Gamma }}$;

(vii) an element $i_0$ of $\mathsf{I}$.

Let us choose a van Kampen datum of $f$. Then, $(\mathsf{a},\mathsf{b}, \beta_1, \beta_2,\mathsf{T}, i_0)$ is a basic equipment of the pair $(\varpi (p_1), \varpi (p_2))$ of groupoid morphisms from $\varpi (Z)$ into $\varpi (X)$ (II, p. 192, déf. 4). Moreover, the triples

$$
\mathsf{z}= ((q_{12}(\mathsf{c}(k)),1),(q_{23}(\mathsf{c}(k)),1),(q_{13}(\mathsf{c}(k)),-1))
$$

and the classes of paths $(\gamma_{1,2}(k), \gamma_{2,3}(k), \gamma_{1,3}(k))$, where $k$ describes $\mathsf{K}$, define a complementary equipment of the pair $(\varpi (p_1), \varpi (p_2))$ (II, p. 208, déf. 3 ; II, p. 205, exemple ; II, p. 205, remarque). We shall say that the complete equipment of the coequalizer Coeg($f$) thus defined is deduced from the van Kampen datum of $f$ that we have chosen.

For every $j\in \mathsf{J}$, let $\varphi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_1(j)))$ and $\psi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_2(j)))$ denote the group homomorphisms defined by

$\varphi_j=$ Int($\beta_1(j)$)$^{-1}\circ (p_1)_*,v\mapsto \beta_1(j)^{-1}((p_1)_*(v))\beta_1(j)$

(1)

$\psi_j=$ Int($\beta_2(j)$)$^{-1}\circ (p_2)_*,v\mapsto \beta_2(j)^{-1}((p_2)_*(v))\beta_2(j)$,

for $v\in \pi_1(Z,\mathsf{b}(j))$. For every $k\in \mathsf{K}$ and every $s\in  \{1,2,3\}$, let $\lambda_s(k)$ denote the class of a loop at the point $\mathsf{a}(i_s(k))$ in X defined by

(2)

$$
\lambda_1(k) =\beta_1(j_{13}(k))^{-1}\cdot ((p_1)_*(\gamma_{13}(k)))^{-1}\cdot ((p_1)_*(\gamma_{12}(k)))\cdot \beta_1(j_{12}(k))
$$

$\lambda_2(k) =\beta_2(j_{12}(k))^{-1}\cdot ((p_2)_*(\gamma_{12}(k)))^{-1}\cdot ((p_1)_*(\gamma_{23}(k)))\cdot \beta_1(j_{23}(k))$,

$$
\lambda_3(k) =\beta_2(j_{23}(k))^{-1}\cdot ((p_2)_*(\gamma_{23}(k)))^{-1}\cdot ((p_2)_*(\gamma_{13}(k)))\cdot \beta_2(j_{13}(k))
$$

Let $\tau$ denote the unique groupoid morphism from Grp($\mathsf{\Gamma}$) into $\varpi (Y)$ such that the mapping Som($\tau$ ) maps $i\in \mathsf{I}$ onto $f(\mathsf{a}(i))$ and Fl($\tau$ ) maps $j\in \mathsf{J}$ onto the class of paths $f_*(\beta_1(j))^{-1}f_*(\beta_2(j))$ joining $f(\mathsf{a}(i_1(j)))$

$$
\mathsf{a}(i_1(k))
$$

$$
\lambda_1(k)
$$

$$
\mathsf{b}_1(j_{12}(k))\mathsf{b}_1(j_{13}(k))
$$

$$
\mathsf{b}_2(j_{12}(k))\mathsf{b}_2(j_{13}(k))
$$

$$
\mathsf{c}_1(k)
$$

$$
\mathsf{c}_2(k)\mathsf{c}_3(k)
$$

$$
\lambda_2(k)\lambda_3(k)
$$

$$
\mathsf{a}(i_2(k))\mathsf{b}_1(j_{23}(k))\mathsf{b}_2(j_{23}(k))\mathsf{a}(i_3(k))
$$

to $f(\mathsf{a}(i_2(j)))$ in Y. For $i\in \mathsf{I}$, let $d_i\in$ Grp($\mathsf{\Gamma}$) be the class of the unique path without backtracking joining $i_0$ to $i$ in the tree $\widetilde{\mathsf{T}}$ and put $\delta_i=$ $\tau (d_i)$.

If S is a set, recall that F(S) denotes the free group on S; the image in F(S) of an element $s\in S$ by the canonical mapping is denoted by $[s]$, or by $s$ if there is no possible confusion.

#### Theorem 1 {#ta-iv-s5-thm-1 .statement tag=0232}

Suppose that Y is path connected and that $f$ verifies the property (VK). With the preceding notations, there exists a unique group homomorphism

$$
\mathsf{L}:(_i*_{\in\mathsf{I}}\pi_1(X,\mathsf{a}(i)))*F(\mathsf{J})\rightarrow \pi_1(Y, f(\mathsf{a}(i_0)))
$$

such that

$\mathsf{L}(v) =\delta_if_*(v)\delta^{-1}_i$ for $i\in \mathsf{I}$ and $v\in \pi_1(X,\mathsf{a}(i))$,

$\mathsf{L}(j) =\delta_{i_1(j)}\tau (j)\delta^{-1}_{i_2(j)}$ for $j\in \mathsf{J}$.

Moreover, the homomorphism $\mathsf{L}$ is surjective and its kernel is the smallest normal subgroup containing the following elements:

($R_1$)$\mathsf{r}_1(j) =j$ for $j$ in Fl($\mathsf{T}$) ;

($R_2$)$\mathsf{r}_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$ for $j\in \mathsf{J}$ and $v\in \pi_1(Z,\mathsf{b}(j))$;

($R_3$)$\mathsf{r}_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$, for $k\in \mathsf{K}$.

The existence and uniqueness of the homomorphism $\mathsf{L}$ follow from the universal property of free products and free groups. Moreover, this homomorphism is the composite of the homomorphism $\varpi '(f)_{\gamma(\mathsf{a}(i_0))}$ deduced from $\varpi '(f)$ by passing to isotropy groups and of the group homomorphism $\lambda$ defined by Prop. 5 of II, p. 208, taking into account the fact that the chosen van Kampen datum determines a complete equipment of the pair $(\varpi (p_1), \varpi (p_2))$ of groupoid morphisms from $\varpi (Z)$ into $\varpi (X)$. By that proposition, the image of the homomorphism $\lambda$ is the group Coeg($f$)$_{\gamma(\mathsf{a}(i_0))}$ and its kernel is the smallest normal subgroup containing the elements defined by relations ($R_1$)$, (R_2)$ and ($R_3$). On the other hand, the groupoid morphism $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ is an isomorphism, by definition of property (VK). The theorem is therefore proved.

### 2. Coverings

Let Y be a nonempty arcwise connected topological space, and let $(A_i)_{i\in I}$ be a covering of Y by nonempty arcwise connected subsets, indexed by a totally ordered set I. Let $X =\bigsqcup_{i\in I}A_i$ be the sum space of the family $(A_i)$ and let $f: X\rightarrow Y$ be the mapping deduced from the family of canonical injections of each $A_i$ into Y. Suppose that the mapping $f$ satisfies property (VK). This occurs in particular in the following two cases:

(i) the interiors of the sets $A_i$, for $i\in I$, cover Y (cf. IV, p. 402, Example 2);

(ii) the space Y is contractible, as are the spaces $A_i$, for $i\in I$, the family $(A_i)_{i\in I}$ is locally finite, the $A_i$ are closed in Y and their pairwise intersections are locally arcwise connected (cf. IV, p. 399, Example 1).

Let $J'$ be the set of triples $(i, i',V)$, where $i$ and $i'$ are elements of I and where V is an arcwise connected component of $A_i\cap A_{i'}$. If $j= (i, i',V)\in J'$, we set $i_1(j) =i,i_2(j) =i'$ and $\overline{j}= (i', i,V)$. Let J be the subset of $J'$ formed by the triples such that $i < i'$. The *framework* of the covering is the quiver Γ whose set of vertices is I, whose set of arrows is J, and whose origin and end mappings are respectively the mappings $j\mapsto i_1(j)$ and $j\mapsto i_2(j)$. We identify the graph associated with Γ with the graph $\widetilde{\Gamma}$ whose set of vertices is I, whose set of arrows is $J\cup \overline{J}$, whose origin and end mappings are the mappings $j\mapsto i_1(j)$ and $j\mapsto i_2(j)$, and whose involution is the mapping $j\mapsto \overline{j}$.

Let $p_1$ and $p_2$ denote the projections of the fibre square $X\times_YX$ onto X; let $\mathsf{\Gamma}$ be the framework of the pair $(\varpi (p_1), \varpi (p_2))$ of groupoid morphisms from $\varpi (X\times_YX)$ into $\varpi (X)$.

#### Lemma 1 {#ta-iv-s5-lem-1 .statement tag=0233}

The quiver Γ identifies with a subquiver of $\mathsf{\Gamma}$; the quivers Γ and $\mathsf{\Gamma}$ are connected.

The arcwise connected components of X are the $A_i$, for $i\in I$. The arcwise connected components of $X\times_YX$ are the $(V\times  \{i\})\times_Y$ $(V\times  \{i'\})$, for $(i, i',V)\in J'$. Consequently, the frame $\mathsf{\Gamma}$ of the pair $(\varpi (p_1), \varpi (p_2))$ is isomorphic to the quiver whose set of vertices is I, whose set of arrows is $J'$, the origin and term mappings being respectively the mappings $j\mapsto i_1(j)$ and $j\mapsto i_2(j)$. The quiver $\mathsf{\Gamma}$ is connected (IV, p. 406). Moreover, this description identifies Γ with a subquiver of $\mathsf{\Gamma}$. Let us also observe that for every arrow $j$ of $\mathsf{\Gamma}$, either $j\in$ Fl($\widetilde{\Gamma}$), or there exists $i\in I$ such that $j= (i, i,A_i)$. It follows that the mapping $\pi_0(\Gamma )\rightarrow \pi_0(\mathsf{\Gamma})$ deduced from the injection of Γ into $\mathsf{\Gamma}$ is bijective, so that Γ is connected.

For every element $i$ of I, choose a point $a(i)$ of $A_i$.

For every element $j= (i, i',V)$ of J, choose a point $b(j)$ in V, a path $B_1(j)$ joining $b(j)$ to $a(i)$ in $A_i$ and a path $B_2(j)$

joining$\overline{j}= (i', i,b(jV)$) tobelongs to$a(i')$ in A$J^{i'}$. Letand let us put$j= (i, ib(',\overline{j}V)$) =an element of$b(j)$, $B_1(j) = B\overline{J}_2$; then$(\overline{j})$ and $B_2(j) = B_1(\overline{j})$. For $j\in J'\cup \overline{J'}$, the paths $\overline{B_1(j)}$ and $B_2(j)$ in Y are composable. Put

$$
B(j) = B_1(j)*B_2(j) \tag{3}
$$

It is a path joining $a(i_1(j))$ to $a(i_2(j))$ in Y; one has the relation $B(\overline{j}) = B(j)$.

For every $j= (i, i',V)\in J'$, denote by $p_{j,1}: V\rightarrow A_i$ and $p_{j,2}: V\rightarrow A_{i'}$ the canonical injections; also denote by $\varphi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_i, a(i))$ and $\psi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_{i'}, a(i'))$ the group homomorphisms defined by

$$
\varphi_j(v) = [B_1(j)]^{-1}(p_{j,1})_*(v)[B_1(j)]
$$

and

$$
\psi_j(v) = [B_2(j)]^{-1}(p_{j,2})_*(v)[B_2(j)]
$$

for $v\in \pi_1(V, b(j))$ (cf. IV, p. 407).

Fix an element $i_0$ of I, as well as a subquiver T in the quiver Γ whose associated graph $\widetilde{T}$ is a maximal tree of the graph $\widetilde{\Gamma}$.

For $i\in I$, let $(i_0, j_1, i_1, . . . , j_n, i)$ be the unique path without backtracking joining $i_0$ to $i$ in the tree $\widetilde{T}$, and put

$$
\delta (i) = [B(j_1)][B(j_2)]. . .[B(j_n)]
$$

this is the class of a path joining $a(i_0)$ to $a(i)$ in Y. Let $\alpha_i$ denote the homomorphism of $\pi_1(A_i, a(i))$ into $\pi_1(Y, a(i))$ deduced from the canonical injection, and let $\mu_i:\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ be the group homomorphism defined by

$$
\mu_i(v) =\delta (i)\alpha_i(v)\delta (i)^{-1}
$$

Finally, let $\mu: F(J)\rightarrow \pi_1(Y, a(i_0))$ be the unique group homomorphism such that one has

$$
\mu(j) =\delta (i_1(j))[B(j)]\delta (i_2(j))^{-1}
$$

for every $j\in J$. There exists a unique group homomorphism

$$
\mathsf{M}:(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow \pi_1(Y, a(i_0))
$$

which coincides with $\mu_i$ on $\pi_1(A_i, a(i))$, for every $i\in$ I, and with $\mu$ on F(J).

Let $K'$ be the set of quadruples $(i_1, i_2, i_3,U)$, where $i_1, i_2, i_3$ are elements of I and where U is a pathwise connected component of $A_{i_1}\cap A_{i_2}\cap A_{i_3}$. For every element $k= (i_1, i_2, i_3,U)$ of $K'$ and every pair $(s, t)$ of elements of $\{1,2,3\}$, put $j_{st}(k) = (i_s, i_t,V)$, where V is the pathwise connected component of $A_{i_s}\cap A_{i_t}$ which contains U; this is an element of $J'$.

Let K be the subset of $K'$ formed by the quadruples $(i_1, i_2, i_3,U)$ such that $i_1< i_2< i_3$. For every element $k= (i_1, i_2, i_3,U)$ of K, choose a point $c(k)$ of U, together with paths $C_{12}(k)$, $C_{23}(k)$ and $C_{13}(k)$, such that $C_{st}(k)$ joins $c(k)$ to $b(j_{st}(k))$ in $A_{i_s}\cap A_{i_t}$ for $s, t\in  \{1,2,3\}$ with $s < t$.

Put then, for $k\in K$,

$$
L_1(k) = B_1(j_{13}(k))*\overline{C_{13}(k)}*C_{12}(k)*B_1(j_{12}(k))
$$

(4) L$L^2_3((kk) = B) = B^2_2((jj^{12}_{23}((kk))))**\overline{CC^{1223}((kk))}**CC^{23}_{13}((kk))**BB^1_2((jj^{23}_{13}((kk))))$,.

For $s\in  \{1,2,3\}$, let $\lambda_s(k)$ denote the class in $\pi_1(A_{i_s}, a(i_s))$ of the loop $L_s(k)$.

#### Proposition 1 {#ta-iv-s5-prop-1 .statement tag=0234}

Let Y be a pathwise connected topological space and let $(A_i)_{i\in I}$ be a covering of Y by non-empty, pathwise connected subsets, indexed by a totally ordered set I. Suppose that the canonical mapping of the sum space of the family $(A_i)_{i\in I}$ into Y satisfies property (VK). Then the homomorphism $\mathsf{M}$ introduced above is surjective, and its kernel is the smallest normal subgroup containing the following elements:

($R_1$)$r_1(j) =j$ for $j$ in Fl(T);

($R_2$)$r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$

for $j= (i, i',V)\in J$ and $v\in \pi_1(V, b(j))$;

($R_3$)$r_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$

for $k\in K$.

Let X be the topological sum of the family $(A_i)_{i\in I}$ and let $f: X\rightarrow Y$ be the mapping induced by the family of canonical injections of each $A_i$ into Y. The mapping $f$ satisfies property (VK) by hypothesis; we shall therefore apply Theorem 1 of No$^o1$ to it. We therefore take up again the notation of this No$^o$ and begin by defining a van Kampen datum for the mapping $f$.

The arcwise connected components of X are the sets $X_i=$ $A_i\times  \{i\}$ for $i\in I$. Thus $\pi_0(X)$ is identified with the set I. For each $i\in I$, let $\mathsf{a}(i)$ denote the point $(a(i), i)$ of $X_i$.

Put $Z = X\times_YX$. The arcwise connected components of Z are the sets $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$, where $j= (i, i',V)$ runs through $J'$. Thus $\pi_0(Z)$ is identified with the set $J'$. Let $J_0$ be the set of elements of J of the form $(i, i,A_i)$, so that the family $(J_0,J,J)$ is a partition of $J'$. For $i\in I$ and $j= (i, i,A_i)\in J_0$, put $\mathsf{b}(j) = (\mathsf{a}(i),\mathsf{a}(i))$ and take for $\beta_1(j)$ and $\beta_2(j)$ the class of the constant path at $\mathsf{a}(i)$. For $j= (i, i',V)\in J\cup \overline{J}$, let $\mathsf{b}(j)$ denote the point $((b(j), i),(b(j), i'))$ of $Z_j$ and let $\beta_1(j)$ and $\beta_2(j)$ denote the classes of the paths $t\mapsto (B_1(j)(t), i)$ and $t\mapsto (B_2(j)(t), i')$ in X.

Put $W = X\times_YX\times_YX$. The arcwise connected components of W are the sets $W_k= (U\times  \{i_1\})\times_Y(U\times  \{i_2\})\times_Y(U\times  \{i_3\})$, where $k= (i_1, i_2, i_3,U)$ runs through $K'$. Thus $\pi_0(W)$ is identified with the set $K'$.

Let $K_0$ denote the set of elements of $K'$ of the form $k= (i, i, i,A_i)$, for $i\in I$. For such an element $k\in K_0$, put $\mathsf{c}(k) = (\mathsf{a}(i),\mathsf{a}(i),\mathsf{a}(i))$ and choose for $\gamma_{st}(k)$ the class of the constant path at $(\mathsf{a}(i),\mathsf{a}(i))$.

Let $K_1$ denote the set of elements of $K'$ of the form $k$ = $(i_1, i_2, i_3,V)$ for which the set $\{i_1, i_2, i_3\}$ has two elements. Let $k$ be an element of $K'$ of the form $(i, i, i',V)$, so that $j= (i, i',V)$ belongs to $J\cup \overline{J}$. We then put

$$
\mathsf{c}(k) = ((b(j), i),(b(j), i),(b(j), i')),\gamma_{12}(k) = (\beta_1(j), \beta_1(j))
$$

and we take for $\gamma_{13}(k)$ and $\gamma_{23}(k)$ the class of the constant path at $\mathsf{b}(j)$. One defines analogously $c(k),\gamma_{12}(k),\gamma_{13}(k),\gamma_{23}(k)$ for every element $k$ of $K'$.

For every element $k= (i_1, i_2, i_3,U)$ of K, put

$$
\mathsf{c}(k) = ((c(k), i_1),(c(k), i_2),(c(k), i_3))
$$

for every pair $(s, t)$ of distinct elements of $\{1,2,3\}$, take for $\gamma_{st}(k)$ the image under the mapping $x\mapsto ((x, s),(x, t))$ of the class of the path $C_{st}(k)$ in $A_{i_s(k)}\cap A_{i_t(k)}$.

For every point $x= (x_1, x_2, x_3)$ of $X\times_YX\times_YX$ and every permutation $\sigma \in \mathfrak{S}_3$, put $\sigma (x) = (x_{\sigma^{-1}(1)}, x_{\sigma^{-1}(2)}, x_{\sigma^{-1}(3)})$. Thus an operation of the group $\mathfrak{S}_3$ on W is defined. For every $k= (i_1, i_2, i_3,U)\in K'$ and every permutation $\sigma \in \mathfrak{S}_3$, put analogously $\sigma (k) = (i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$; one has

$$
\sigma (W_k) = (U\times  \{i_{\sigma^{-1}(1)}\})\times_Y(U\times  \{i_{\sigma^{-1}(2)}\})\times_Y(U\times  \{i_{\sigma^{-1}(3)}\}) = W_{\sigma(k)}
$$

Let $k= (i_1, i_2, i_3,U)$ be an element of $K'$ such that $i_1, i_2, i_3$ are pairwise distinct. There exists a unique permutation $\sigma \in$ $\mathfrak{S}_3$ such that $i_{\sigma^{-1}(1)}< i_{\sigma^{-1}(2)}< i_{\sigma^{-1}(3)}$, so that $\sigma (k) =$ $(i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$ belongs to K. For $s\in  \{1,2,3\}$, one then puts $c_s(k) =c_{\sigma(s)}(\sigma (k))$ and $c(k) = (c_1(k), c_2(k), c_3(k))$, so that $c(k) =\sigma^{-1}(c(\sigma (k)))$. For $(s, t)\in  \{(1,2),(1,3),(2,3)\}$, one defines $C_{st}(k) = C_{\sigma^{-1}(s)\sigma^{-1}(t)}(\sigma (k))$; it is a path joining $c(k)$ to $b(j_{\sigma(s)\sigma(t)}(\sigma (k))) =b(j_{st}(k))$.

Let $g$ denote the morphism of quivers from Γ into $\mathsf{\Gamma}$ which associates with a vertex $i\in I$ of Γ the vertex $X_i= A_i\times  \{i\}$ of $\mathsf{\Gamma}$ and with an arrow $j= (i, i',V)\in J'$ of Γ the arrow $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$ of $\mathsf{\Gamma}$. The mapping Som($g$) is bijective; the mapping Fl($g$) is injective and the graph Γ is connected (IV, p. 410, lemma 1), and the image under $g$ of the subquiver T is a subquiver $\mathsf{T}$ of $\mathsf{\Gamma}$ whose associated graph is a maximal tree of the graph $\widetilde{\mathsf{\Gamma }}$.

The points $\mathsf{a}(i)$, for $i\in I$, the points $\mathsf{b}(j)$, for $j\in J'$, the points $\mathsf{c}(k)$, for $k\in K'$, the classes of paths $\beta_1(j)$ and $\beta_2(j)$, for $j\in J'$, the classes of paths $\gamma_{st}(k)$, for $k\in K'$, the subquiver $g(T)$ of $\mathsf{\Gamma}$ and the element $i_0$ of I define a van Kampen datum for $f$.

Let $\rho$ denote the unique group homomorphism

$$
\rho :(_i*_{\in I}\pi_1(X,\mathsf{a}(i)))*F(J')\rightarrow (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)
$$

which induces the isomorphism of $\pi_1(X,\mathsf{a}(i))$ onto $\pi_1(A_i, a(i))$ deduced from the identification of $A_i\times  \{i\}$ and $A_i$, for all $i\in I$, and such that one has

$\rho (j) = 1$ for $j\in J_0$

$\rho (j) =j,\rho (\overline{j}) =j^{-1}$ for $j\in J$.

Let $\mathsf{L}$ be the group homomorphism defined in Theorem 1 of IV, p. 408. For $j= (i, i,A_i)\in J_0$, one has $\mathsf{L}(j) = 1 =\mathsf{M}\circ \rho (j)$. Let $j= (i, i',V)$ be an element of J; one has $\mathsf{L}(j) = (\mathsf{M}\circ \rho )(j)$ by definition. Finally, if $j=$ $(i, i',V)$ is an element of $\overline{J},\overline{j}\in J$ and one verifies that

$$
\mathsf{L}(j) =\mathsf{L}(\overline{j})^{-1}=\mathsf{M}(\rho (\overline{j}))^{-1}=\mathsf{M}(\rho (j))
$$

Consequently, one has $\mathsf{M}\circ \rho =\mathsf{L}$.

The homomorphism $\mathsf{L}$ is surjective (loc. cit.), hence the homomorphism $\mathsf{M}$ is also. Since the homomorphism $\rho$ is surjective, the kernel of $\mathsf{M}$ is the smallest normal subgroup of $(_i*_{\in I}\pi_1(A_i, a(i)))*F(J_1)$ which contains the images under $\rho$ of the elements defined by relations ($R_1$), ($R_2$)$, (R_3)$ of theorem 1 (IV, p. 408). The proof will be complete once we have verified that these images are, besides the elements defined by relations ($R_1$)$, (R_2), (R_3)$ of Prop. 1, elements conjugate to them, or conjugate to their inverses, together with the identity element.

Elements $R_1$. — An arrow of the oriented tree $\mathsf{T}$ is of the form $Z_j$, with $j= (i, i',V)\in J$; its image is the element $j$ of F(J).

Elements $R_2$. — Let $j= (i, i',V)\in J'$. If $i=i'$, we have $\rho (\mathsf{r}_2(j, v)) = 1$ for every $v\in \pi_1(A_i,\mathsf{a}(i))$. If $j\in J$, the image of $\mathsf{r}_2(j, v)$ is the element $r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$, for every $v\in \pi_1(Z,\mathsf{b}(j))$. In the remaining case, we have $\overline{j}\in J$ and the equality

$$
\rho (\mathsf{r}_2(j, v)) =\rho (\varphi_j(v)j\psi_j(v)^{-1}j^{-1})
$$

$$
= [B_1(j)]^{-1}v[B_1(j)]\rho (j)[B_2(j)]^{-1}v^{-1}[B_2(j)]\rho (j)^{-1}
$$

$$
= [B_2(\overline{j})]^{-1}v[B_2(\overline{j})]\overline{j}^{-1}[B_1(\overline{j})]^{-1}v^{-1}[B_1(\overline{j})]\overline{j}
$$

implies that $\rho (\mathsf{r}_2(j, v))$ is conjugate to $\rho (\mathsf{r}_2(j, v^{-1}))$.

Elements $R_3$. — Let $k= (i_1, i_2, i_3,U)$ be an element of $K'$.

If $k\in K_0,i_1$ = $i_2$ = $i_3,\lambda_s(k)$ is the class of the trivial path for every $s\in  \{1,2,3\},j_{st}(k)\in J_0$ for every pair $(s, t)\in$ $\{(1,2),(1,3),(2,3)\}$. Then $\rho (\mathsf{r}_3(k))$ is the identity element.

Suppose $k\in K_1$. If $i_1=i_2$, then $j= (i_1, i_3,U)\in J\cup \overline{J}$ and we have

$$
\mathsf{r}_3(k) =\beta_1(j)^{-1}j_{12}\beta_1(j)j_{23}\beta_2(j)^{-1}\beta_2(j)j_{13}^{-1}
$$

whose image under $\rho$ is the identity element. The other cases are dealt with analogously.

Suppose that $i_1, i_2, i_3$ are pairwise distinct. If $i_1< i_2< i_3$, $k\in K$ and the image of $\rho (\mathsf{r}_3(k))$ is the element $r_3(k)$.

Let $\sigma \in \mathfrak{S}_3$ be the permutation carrying 1 to 2 and 2 to 3. We have

$$
\lambda_1(\sigma (k)) =\beta_1(j_{13}(\sigma (k)))^{-1}\cdot p_{1,*}(\gamma_{13}(\sigma (k)))^{-1}\cdot
$$

$$
\cdot p_{1,*}(\gamma_{12}(\sigma (k)))\cdot \beta_1(j_{12}(\sigma (k)))
$$

$$
=\beta_1(j_{32}(k))^{-1}\cdot p_{1,*}(\gamma_{32}(k))^{-1}\cdot p_{1,*}(\gamma_{31}(k))\cdot \beta_1(j_{31}(k))
$$

$$
=\beta_2(j_{23}(k))^{-1}\cdot p_{2,*}(\gamma_{2,3}(k))^{-1}\cdot p_{2,*}(\gamma_{13}(k))\cdot \beta_2(j_{13}(k))
$$

$$
=\lambda_3(k)
$$

One verifies analogously that $\lambda_2(\sigma (k)) =\lambda_1(k)$ and $\lambda_3(\sigma (k)) =\lambda_2(k)$. Hence,

$$
\rho (\mathsf{r}_3(\sigma (k))) =\lambda_1(\sigma (k))\rho (j_{12}(\sigma (k)))\lambda_2(\sigma (k))\cdot
$$

$$
\cdot \rho (j_{23}(\sigma (k)))\lambda_3(\sigma (k))\rho (j_{13}(\sigma (k)))^{-1}
$$

$$
=\lambda_3(k)\rho (j_{31}(k))\lambda_1(k)\rho (j_{12}(k))\lambda_2(k)\rho (j_{32}(k))^{-1}
$$

$$
=\lambda_3(k)j_{13}(k)^{-1}\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)
$$

which proves that $\rho (\mathsf{r}_3(\sigma (k)))$ is conjugate to

$$
\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}=\rho (\mathsf{r}_3(k))
$$

Let $\tau \in \mathfrak{S}_3$ be the transposition with support $\{1,2\}$. We have

$\lambda_1(\tau (k)) =\lambda_2(k)^{-1},\lambda_2(\tau (k)) =\lambda_1(k)^{-1}$ and $\lambda_3(\tau (k)) =\lambda_3(k)^{-1}$. The equalities

$$
\rho (\mathsf{r}_3(\tau (k))) =\lambda_2(k)^{-1}\rho (j_{21}(k))\lambda_1(k)^{-1}\rho (j_{13}(k))\lambda_3(k)^{-1}\rho (j_{23}(k))^{-1}
$$

$$
=(\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}\lambda_1(k)\rho (j_{12}(k))\lambda_2(k))^{-1}
$$

show that $\rho (\mathsf{r}_3(\tau (k)))$ is conjugate to the inverse of

$$
\lambda_1(k)\rho (j_{12}(k))^{-1}\lambda_2(k)\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}=\rho (\mathsf{r}_3(k))
$$

Since the group $\mathfrak{S}_3$ is generated by the permutations $\tau$ and $\sigma$, it follows that, for every $k\in K$ and every $\sigma \in \mathfrak{S}_3,\rho (\mathsf{r}_3(\sigma (k)))$ is conjugate to $\rho (\mathsf{r}_3(k))$ or to its inverse.

Thus Proposition 1 is proved.

#### Corollary 1 {#ta-iv-s5-prop-1-cor-1 .statement tag=0235}

Under the assumptions of proposition 1, suppose moreover that, for every $i\in$ I, the image of the homomorphism from $\pi_1(A_i, a(i))$ into $\pi_1(Y, a(i))$, induced by the canonical injection of $A_i$ into Y, is trivial. The homomorphism $\mathsf{M}': F(J)\rightarrow \pi_1(Y, a(i_0))$ induced by $\mathsf{M}$ by restriction is then surjective, and its kernel is the smallest distinguished subgroup containing the elements $j\in$ Fl(T) and the elements $j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$ for $k\in K$.

Let $\pi : (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow F(J)$ be the unique homomorphism which induces the trivial homomorphism on each $\pi_1(A_i, a(i))$ and the identity on F(J); it is surjective. Let $i\in I$. The definition of $\mathsf{M}$ and the assumption that the image of the homomorphism from $\pi_1(A_i, a(i))$ into $\pi_1(Y, a(i))$ induced by the canonical injection is trivial imply that, for every $v\in \pi_1(A_i, a(i)),\mathsf{M}(v)$ is the identity element of $\pi_1(Y, a(i_0))$. Hence $\mathsf{M}=\mathsf{M}'\circ \pi$. It follows that the homomorphism $\mathsf{M}'$ is surjective, and its kernel is the smallest distinguished subgroup containing the images under $\pi$ of the elements $r_1(j),r_2(j, v)$ and $r_3(k)$ defined in Prop. 1. For $j\in$ Fl(T), we have $\pi (r_1(j)) =j$. For every $j\in$ J and every $v\in \pi_1(V, b(j))$, we have $\pi (r_2(j, v)) =e$. Finally, for every $k= (i_1, i_2, i_3,U)\in K$ and every $s\in$ $\{1,2,3\},\lambda_s(k)$ is the class of a loop in $A_{i_s}$; hence $\pi (\lambda_s(k)) =e$, so that $\pi (r_3(k)) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. The corollary follows.

#### Corollary 2 {#ta-iv-s5-prop-1-cor-2 .statement tag=0236}

Under the assumptions of proposition 1, suppose moreover that for every $i\in I$, the group $\pi_1(A_i, a(i))$ is reduced to the identity element and that, for every triple $(i_1, i_2, i_3)$ of pairwise distinct elements of I, the set $A_{i_1}\cap A_{i_2}\cap A_{i_3}$ is empty. The homomorphism $\mathsf{M}'':$ F(J-Fl(T)) $\rightarrow \pi_1(Y, a(i_0))$ induced by $\mathsf{M}$ by restriction is then an isomorphism.

Let $\pi ': F(J)\rightarrow$ F(J - Fl(T)) be the homomorphism which maps $[j]$ to $[j]$ if $j\in$ J-Fl(T) and which maps $[j]$ to the identity element if $j\in$ Fl(T); it is surjective and one has $\mathsf{M}''\circ \pi '=\mathsf{M}'$, where $\mathsf{M}'$ is the surjective homomorphism defined in corollary 1. It follows that $\mathsf{M}''$ is surjective and that its kernel is the smallest distinguished subgroup of F(J-Fl(T)) which contains the images under $\pi '$ of the elements described in loc. cit. But, by construction, $\pi '(j) =e$ if $j\in$ Fl(T) and the set K is empty, by hypothesis. The homomorphism $\mathsf{M}''$ is therefore an isomorphism.

#### Example 1 {#ta-iv-s5-n2-exa-1 .statement tag=0237}

For the case of a covering formed of two sets, see No. 3.

#### Example 2 {#ta-iv-s5-n2-exa-2 .statement tag=0238}

Let G be a graph (II, p. 155, definition 1); let S denote the set of vertices of G, A the set of its oriented edges, $o$ and $t$ the origin and term mappings of A into S; for every oriented edge $a\in A$, let $\overline{a}$ denote the opposite oriented edge. Endow the sets S and A with the discrete topology; let X be the sum space of the space S and of the space $\mathbf{I}\times A$, and let $\sim$ be the finest equivalence relation in X for which $(u, a)\sim (1-u, a)$, $(0, a)\sim o(a)$ and $(1, a)\sim t(a)$ for every $u\in \mathbf{I}$ and every oriented edge $a\in A$. The quotient space $|G|= X/\sim$ is called the geometric realization of the graph G. Let $p$ denote the canonical projection of X onto $|G|$.

Let us prove that $|G|$ is locally contractible. Let $s\in S$. Let $X_s$ denote the union of $\{s\}$ and of the sets $[0,1[\times  \{a\}$ for $a\in \overset{-1}{o}(s)$ and of the

sets $]0,1]\times \{a\}$ for $a\in \overset{-1}{t}(s)$. Let $U_s$ be the image of $X_s$ in $|G|$; it is an open neighbourhood of $p(s)$ in $|G|$ because $X_s$ is an open saturated neighbourhood of $s$ in X. Let $f$ be the mapping of $X_s\times \mathbf{I}$ into $X_s$ defined, for $u, v\in \mathbf{I}$ and $a\in A$, by the relations

$$
f(s, v) =s
$$

$((1-v)u, a)$ if $0\leqslant u <1$ and $o(a) =s$,

$$
f((u, a), v) =
$$

$(1-(1-v)(1-u), a)$ if $0< u\leqslant 1$ and $t(a) =s$.

It is continuous and compatible with the equivalence relation $\sim$. It therefore defines by passing to the quotient a mapping $\varphi_s: U_s\times \mathbf{I}\rightarrow U_s$ which is continuous, since $\mathbf{I}$ is locally compact (I, p. 19, Prop. 10). It is a strong contraction of $U_s$ onto $p(s)$ (III, p. 237, Def. 6).

Let moreover $x= (\tau , a)\in ]0,1[\times A$. Let us denote by $X_x= ]0,1[\times  \{a, a\}$ and let $U_x$ be its image in $|G|$ by $p$; it is a neighbourhood of $p(x)$ in $|G|$, homeomorphic to $]0,1[$. The mapping of $X_x\times \mathbf{I}$ into $X_x$ given by $((u, a), v)\mapsto ((1-v)u+v\tau , a)$ and $((u, a), t)\mapsto ((1-v)u+v(1-\tau ), a)$ is continuous. It defines by passing to the quotient a mapping $\varphi_x: U_x\times$ $\mathbf{I}\rightarrow U_x$ which is continuous (loc. cit.) and is a strong contraction at $x$.

Every point of $|G|$ is the image of a point $s\in S$ or of a point of $\mathbf{I}\times A$ of the form $(\tau , a)$ where $0< \tau  <1$. It follows that every point of $|G|$ has a neighbourhood contractible at that point. In other words, $|G|$ is locally contractible and, in particular, unravelable (IV, p. 346, Prop. 5).

Let us choose a total order on S and consider the open covering $(U_s)_{s\in S}$ of $|G|$. Let $s$ and $s'$ be distinct elements of S. The intersection $U_s\cap U_{s'}$ is the union of the $p(]0,1[, a)$ where $a$ runs through the set of oriented edges of G whose extremities are $s$ and $s'$. Consequently, the framework of the covering $(U_s)_{s\in S}$ is identified with the quiver G. Moreover, for every $s\in S$, $U_s$ is contractible at $s$, hence $\pi_1(U_s, p(s))$ is reduced to the identity element. It then follows from Cor. 2 of IV, p. 416 that for every $s\in S,\pi_1(|G|, p(s))$ is a free group (Nielsen-Schreier theorem).

#### Corollary 3 {#ta-iv-s5-prop-1-cor-3 .statement tag=0239}

Under the hypotheses of Prop. 1, suppose in addition that the framework of the covering $(A_i)_{i\in I}$ is an oriented tree. The homomorphism $\mathsf{N}:_i*_{\in I}\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ deduced from $\mathsf{M}$ by restriction is then surjective; its kernel is the smallest normal subgroup of $_i*_{\in I}\pi_1(A_i, a(i))$ which contains the elements $\varphi_j(v)\psi_j(v)^{-1}$, for

every $j= (i_1, i_2,V)\in J$ and every $v\in \pi_1(V, b(j))$.

If the arcwise connected components of the intersections $A_i\cap A_{i'}$, for $i=\not i'$ are moreover simply connected, the homomorphism $\mathsf{N}$ is then an isomorphism.

Under the hypotheses of the corollary, the graph associated with the quiver Γ is a tree, whence T = Γ. It follows that the image of the group F(J) by the homomorphism $\mathsf{M}$ is reduced to the identity element.

Let

$$
\rho :(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow_i*_{\in I}\pi_1(A_i, a(i))
$$

be the unique group homomorphism which induces the identity homomorphism on $\pi_1(A_i, a(i))$ and whose kernel contains F(J). We have $\mathsf{M}=\mathsf{N}\circ \rho$. Consequently, the homomorphism $\mathsf{N}$ is surjective and its kernel is the smallest normal subgroup of $_i*_{\in I}\pi_1(A_i, a(i))$ which

contains the images under $\rho$ of the elements defined by relations ($R_1$), ($R_2$) and ($R_3$) of Prop. 1. We have $\rho (j) = 1$ for every $j\in$ Fl(Γ). Since the framework of the covering $(A_i)_{i\in I}$ is a tree, one has $A_{i_1}\cap A_{i_2}\cap A_{i_3}=\emptyset$ for every triple $(i_1, i_2, i_3)$ of distinct elements of I. It follows that the kernel of $\mathsf{N}$ is the smallest normal subgroup containing the elements $\varphi_j(v)\psi_j(v)^{-1}$ for every $j= (i_1, i_2,V)\in J$ and every $v\in \pi_1(V, b(j))$.

#### Example 3 (Plane deprived of $n$ points) {#ta-iv-s5-n2-exa-3 .statement tag=023A}

The fundamental group of $\mathbf{R}^2$ $\{0\}$ is isomorphic to $\mathbf{Z}$, and the class of the path $t\mapsto e^{2\pi it}$ is a generator of it (IV, p. 347, corollary). More generally, let $n$ be a natural number and let $A =\{z_1, . . . , z_n\}$ be a set of $n$ points of $\mathbf{R}^2$. Let Y be the space $\mathbf{R}^2-$ A; we shall prove that the fundamental group of Y is isomorphic to the free group $F_n$ on $n$ generators. For every $i$, put $z_i= (u_i, v_i)$. Replacing $z_i$ if necessary by $f(z_i)$, where $f:\mathbf{R}^2\rightarrow \mathbf{R}^2$ is a homeomorphism of the form $(u, v)\mapsto (u+\alpha v, v)$, one may suppose that the abscissae of the $z_i$ are pairwise distinct. There is likewise no loss in supposing that one has $u_1<\cdots < u_n$.

Put $V_1= ]-\infty , u_2[\times \mathbf{R},V_i= ]u_{i-1}, u_{i+1}[\times \mathbf{R}$ for $2\leqslant i\leqslant n-1$, $V_n= ]u_{n-1},+\infty [\times \mathbf{R}$. For $1\leqslant i\leqslant n$, the set $U_i= V_i-\{z_i\}$ is open in the plane and homeomorphic to $\mathbf{R}^2-\{0\}$. The family $(U_i)_{1\leqslant i\leqslant n}$ is an open covering of the space $Y =\mathbf{R}^2-$ A. The intersection $U_i\cap U_j$ is empty for $|i-j|\geqslant 2$, homeomorphic to $\mathbf{R}^2$ for $|i-j|= 1$. By Corollary 3, the fundamental group of Y is isomorphic to the free group $F_n$.

Let $a$ be a point of Y. For every integer $i\in  \{1, . . . , n\}$, let $r_i$ be a real number strictly positive and strictly less than the distances from $z_i$ to the points $z_j$, for $j=\not i$. Let us denote by $v_i$ the class of the loop $t\mapsto$ $z_i+r_ie^{2\pi it}$ at the point $z_i+r_i$ of Y. Let $\theta_i$ be the class of a path $\gamma_i$ joining the point $a$ to the point $z_i+r_i$ in Y. If the paths $\gamma_i$ are injective and if their images meet only at $a$, one can prove that the unique homomorphism of the free group $F(t_1, . . . , t_n)$ into $\pi_1(Y, a)$ such that $\varphi (t_i) =\theta_iv_i\theta^{-1}_i$ for every $i\in  \{1, . . . , n\}$ is a group isomorphism.

An analogous reasoning makes it possible to prove that for every discrete closed subset A of the plane, the fundamental group of $\mathbf{R}^2-$ A is isomorphic to F(A) (IV, p. 463, Exercise 1).

#### Corollary 4 {#ta-iv-s5-prop-1-cor-4 .statement tag=023B}

Under the hypotheses of Proposition 1, suppose that there exists a subset A of Y, connected by arcs and nonempty, such that the intersection $A_i\cap A_{i'}$ is equal to A for every pair $(i, i')$ of distinct elements of I. Let $a$ be a point of A. There exists a unique homomorphism $\varphi$ of the sum of the family of groups $(\pi_1(A_i, a))_{i\in I}$ amalgamated by $\pi_1(A, a)$ into $\pi_1(Y, a)$ which coincides with the homomorphism induced by the canonical injection of $A_i$ into Y, for every $i\in I$. The homomorphism $\varphi$ is an isomorphism.

In particular, if the group $\pi_1(A, a)$ is reduced to the identity element, the canonical homomorphism of the free product of the family of groups $(\pi_1(A_i, a))_{i\in I}$ into $\pi_1(Y, a)$ is an isomorphism.

For $i\in$ I, let us denote by $g_i:\pi_1(A, a)\rightarrow \pi_1(A_i, a)$ and $f_i:\pi_1(A_i, a)\rightarrow$ $\pi_1(Y, a)$ the canonical homomorphisms induced by the inclusions of A into $A_i$ and of $A_i$ into Y. Let us denote by $*\pi_1(A_i, a)$ the sum of the groups $\pi_1(A_i, a)$ amalgamated by $\pi_1(A, a)$. Let also$^Ap$ be the unique homomorphism of $_i*_{\in I}\pi_1(A_i, a)$ into $*_A\pi_1(A_i, a)$ which induces the identity on $\pi_1(A_i, a)$ (A, I, p. 80, prop. 4). The homomorphism $p$ is surjective and it follows from the definition of the monoid $*\pi_1(A_i, a)$ that its kernel is the smallest distinguished subgroup of$^A_i*_{\in I}\pi_1(A_i, a)$ which contains the

elements $g_i(v)g_{i'}(v)^{-1}$, for $i, i'\in I$ and $v\in \pi_1(A, a)$.

The homomorphisms $f_i\circ g_i:\pi_1(A, a)\rightarrow \pi_1(Y, a)$, for $i\in I$, are equal. It therefore follows from the universal property of amalgamated sums of monoids (A, I, p. 80, Prop. 4) that there exists a unique group homomorphism $\varphi$ (resp. $f$) from $*_A\pi_1(A_i, a)$ (resp. from $_i*_{\in I}\pi_1(A_i, a)$) into $\pi_1(Y, a)$ which induces the homomorphism $f_i$ on $\pi_1(A_i, a)$. We have $f=$ $\varphi \circ p$.

For $i\in$ I, let $u_i$ be the canonical injection of A into $A_i$ and $v_i$ the canonical injection of $A_i$ into Y. Let also $w$ be the canonical injection of A into Y. For every $i\in$ I, one has $v_i\circ u_i$ = $w$, hence $\pi_1(v_i, a)\circ \pi_1(u_i, a) =\pi_1(w, a)$. It then follows from the universal property of amalgamated sums of monoids (A, I, p. 80, Prop. 4) that there exists a unique group homomorphism $\varphi$ from $*_i\pi_1(A_i, a)$ into $\pi_1(Y, a)$ which induces the homomorphism $\pi_1(v_i, a)$ on $\pi_1(A_i, a)$. It remains to prove that $\varphi$ is an isomorphism.

The set J is identified with the set of pairs $(i, i')$ of elements of I such that $i < i'$. The set K is identified with the set of triples $(i_1, i_2, i_3)$ of elements of I such that $i_1< i_2< i_3$. Let us choose all the base points $a(i),b(j)$ and $c(k)$ equal to $a$ and all the paths $B(j)$, $C_{st}(k)$ equal to the constant path with image $a$. Let us also fix a point $i_0\in I$.

For every pair $(i, i')$ of distinct points of I, the framework Γ of the covering $(A_i)$ has exactly one arrow with endpoints $i$ and $i'$. The arrows of Γ one of whose endpoints is equal to $i_0$ are the arrows of an oriented maximal tree T.

For every element $k\in K$, one has $r_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$; let R be the normal subgroup of F(J) generated by the elements $j\in$ Fl(T) and the elements $r_3(k),k\in$ K. Let us prove that R = F(J). It is enough to show that every element $j= (i_1, i_2)$ of J belongs to R. This is true, by hypothesis, if $i_1=i_0$ or $i_2=i_0$. Suppose $i_0< i_1$ and put $k= (i_0, i_1, i_2)$. This is an element of K such that $j=j_{23}(k) =j$. Moreover, $j_{12}(k)$ and $j_{13}(k)$ belong to Fl(T). It follows that $j$ belongs to R. The cases where $i_1< i_0< i_2$ or $i_2< i_0$ are treated in an analogous manner.

It then follows from Prop. 1 (IV, p. 412) that the homomorphism $f$ is surjective and that its kernel is the smallest distinguished subgroup containing the relators $r_2(j, v) =g_i(v)g_{i'}(v)^{-1}$, for $j= (i, i',A)\in J$ and $v\in \pi_1(A, a)$. In other words, Ker($f$) $=$ Ker($p$). It follows that $\varphi$ is an isomorphism, as was to be proved.

If $\pi_1(A, a)$ is reduced to the identity element, $p$ is an isomorphism, whence the second assertion.

#### Example 4 {#ta-iv-s5-n2-exa-4 .statement tag=023C}

Let $((X_i, x_i))_{i\in I}$ be a family of pointed topological spaces. The bouquet of the family $((X_i, x_i))_{i\in I}$ is by definition, and is denoted by $\bigvee_{i\in I}(X_i, x_i)$, the quotient topological space of the sum space of the family $(X_i)_{i\in I}$ by the equivalence relation which identifies all the points $(x_i, i)$ with one another, for $i\in I$. Let X denote this topological space and $x$ the common image of the $x_i$. Suppose that, for every $i\in$ I, the point $x_i$ is closed in $X_i$ and that the spaces $X_i$ are simply connected. If I is finite, Corollary 4 implies that the canonical homomorphism $_i*_{\in I}\pi_1(X_i, x_i)\rightarrow \pi_1(X, x)$ is an isomorphism.

Remark 1 of IV, p. 429 and Exercise 3, IV, p. 463 give less restrictive conditions under which this homomorphism is an isomorphism. See nevertheless Exercise 4, IV, p. 464.

### 3. Particular case of a covering formed of two parts

Let X be an arcwise connected topological space, and let B and C be non-empty arcwise connected subsets of X. Assume further one of the two following hypotheses:

(i) The interiors of the sets B and C cover X;

(ii) The sets B and C are closed in X, their union is equal to X, the spaces X, B, C are simply connected, and the space $B\cap C$ is locally arcwise connected.

Under these hypotheses, the canonical mapping of the sum space of the family $(B,C)$ onto the space X satisfies property (VK) (cf. IV, p. 409).

Put $A = B\cap C$. Since the space X is connected, the set A is not empty. Let $a$ be a point of A; let $j_0$ denote the arcwise connected component of $a$ in A. For every arcwise connected component $j$ of A distinct from $j_0$, choose a point $a_j$ of $j$, the class $\beta_j$ of a path in B and the class $\gamma_j$ of a path in C, both joining $a_j$ to $a$; let $\varphi_j:\pi_1(A, a_j)\rightarrow \pi_1(B, a)$ and $\psi_j:\pi_1(A, a_j)\rightarrow \pi_1(C, a)$ denote the group homomorphisms defined by

$\varphi_j(v) =\beta_j^{-1}v\beta_j$ and $\psi_j(v) =\gamma_j^{-1}v\gamma_j$

for $v\in \pi_1(A, a_j)$. Let $\varphi_0$ and $\psi_0$ also denote the homomorphisms of $\pi_1(A, a)$ into $\pi_1(B, a)$ and $\pi_1(C, a)$ respectively induced by the canonical injections. Let $\iota_B$ and $\iota_C$ denote the homomorphisms of $\pi_1(B, a)$ and $\pi_1(C, a)$ respectively into $\pi_1(X, a)$ induced by the canonical injections. Finally, let $\mu$ be the unique homomorphism of the free group $F(\pi_0(A)-\{j_0\})$ into $\pi_1(X, a)$ such that $\mu(j) =\beta_j^{-1}\gamma_j$ for every $j\in \pi_0(A)-\{j_0\}$.

#### Proposition 2 {#ta-iv-s5-prop-2 .statement tag=023D}

There exists a unique group homomorphism

$$
\mathsf{M}:\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)-\{j_0\})\rightarrow \pi_1(X, a)
$$

which coincides with $\iota_B$ in $\pi_1(B, a)$, $\iota_C$ in $\pi_1(C, a)$ and $\mu$ in $F(\pi_0(A)$ $\{j_0\})$. This homomorphism is surjective and its kernel is the smallest normal subgroup containing the elements

$$
\varphi_j(v)j\psi_j(v)^{-1}j^{-1}
$$

for $j\in \pi_0(A)-\{j_0\}$ and $v\in \pi_1(A, a_j)$, and the elements

$$
\varphi_0(v)\psi_0(v)^{-1}
$$

for $v\in \pi_1(A, a)$.

The framework Γ of the covering of X defined by the family $(B,C)$ has two vertices $b$ and $c$ corresponding to the two sets B and C. The set of its arrows is equal to $\pi_0(A)$; they join the point $b$ to the point $c$. The graph associated with the subquiver of Γ whose only arrow is $j_0$ is a maximal tree of $\widetilde{\Gamma}$. The proposition then results from IV, p. 412, prop. 1.

#### Example {#ta-iv-s5-n3-exa-1 .statement tag=023E}

For $n\geqslant 1$, the sphere $\mathbf{S}_n$ is the union of two closed hemispheres, homeomorphic to the closed ball $\mathbf{B}_{n-1}$ (TG, VI, p. 12), and whose intersection is identified with the sphere $\mathbf{S}_{n-1}$. For $n\geqslant 2$, the sphere $\mathbf{S}_{n-1}$ is arcwise connected; it follows that the Poincaré group of $\mathbf{S}_n$ is trivial (cf. I, p. 127, example 3).

The sphere $\mathbf{S}_0$ has two arcwise connected components; thus one recovers that the Poincaré group of the circle $\mathbf{S}_1$ is isomorphic to a free group on one generator. More precisely, let B and C be the intersections of $\mathbf{S}_1$ with the half-planes of equations $y\geqslant 0$ and $y\leqslant 0$ in the plane $\mathbf{R}^2$. Put $a= (1,0),a'= (-1,0)$; one has $B\cap C =\{a, a'\}$; its connected components are $j_0=\{a\}$ and $j=\{a'\}$. Let $\beta$ be the class of the path $t\mapsto e^{\pi it}$ in $\mathbf{C}$; if one identifies $\mathbf{C}$ with $\mathbf{R}^2$, it joins $a$ to $a'$ in B. Analogously, let $\gamma$ be the class of the path $t\mapsto e^{-\pi it}$ joining $a$ to $a'$ in C. The path $\beta \gamma^{-1}$ is a loop at $a$, given by $t\mapsto e^{2\pi it}$. By proposition 2, its class generates the group $\pi_1(\mathbf{S}_1, a)$.

#### Corollary 1 {#ta-iv-s5-prop-2-cor-1 .statement tag=023F}

The homomorphism $\mu$ is injective. More precisely, there exists a retraction associated with $\mu$ which is a group homomorphism.

Let $\rho$ be the unique homomorphism of $\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)$ $\{j_0\})$ into $F(\pi_0(A)$ - $\{j_0\})$ which induces the trivial homomorphism on $\pi_1(B, a)$ and $\pi_1(C, a)$ and the identity on $F(\pi_0(A)-\{j_0\})$. Let N be the kernel of the homomorphism $\mathsf{M}$. By proposition $2,\rho (N)$ is reduced to the identity element. There therefore exists a unique homomorphism $\mathsf{r}$ of $\pi_1(X, a)$ into $F(\pi_0(A)-\{j_0\})$ such that $\rho =\mathsf{r}\circ \mathsf{M}$. For every $v\in F(\pi_0(A)-\{j_0\})$, one has $\mathsf{M}(v) =\mu(v)$, hence $\mathsf{r}\circ \mu$ is the identity homomorphism. The corollary follows.

#### Corollary 2 {#ta-iv-s5-prop-2-cor-2 .statement tag=023G}

If the group $\pi_1(X, a)$ is trivial, the set A = $B\cap C$ is arcwise connected; if it is commutative, the set A has at most two arcwise connected components.

In fact, if S is a set, the free group F(S) is trivial only if S is empty and is commutative only if Card $S\leqslant 1$.

#### Corollary 3 {#ta-iv-s5-prop-2-cor-3 .statement tag=023H}

If the groups $\pi_1(X, a)$ and $\pi_1(A, a)$ are trivial, the same is true of the groups $\pi_1(B, a)$ and $\pi_1(C, a)$.

By corollary 2, the set A is arcwise connected. The group $\pi_1(X, a)$ is therefore isomorphic to the free product of the groups $\pi_1(B, a)$ and $\pi_1(C, a)$. In particular it contains subgroups isomorphic to the groups $\pi_1(B, a)$ and $\pi_1(C, a)$ (A, I, p. 83). These two groups are therefore trivial if $\pi_1(X, a)$ is.

### 4. Quotient Spaces

Let X be an arcwise connected topological space endowed with a proper (right) operation of a discrete group G. Put $Y = X/G$ and denote by $f: X\rightarrow Y$ the canonical mapping. If $g\in G$ and $c:\mathbf{I}\rightarrow X$ is a path in X, let $g^*c$ denote the path $t\mapsto c(t)\cdot g$ and $g^*[c]$ its strict homotopy class.

Let $o$ be a point of X. For each $g\in G$, let $\beta_g$ be the class of a path joining $o\cdot g$ to $o$ in X. For each $g\in G$, let $X^g$ be the set of points $x\in X$ such that $x\cdot g=x$; for each arcwise connected component $j$ of $X^g$, let $a_j$ be a point of $j$ and let $\gamma_j$ be the class of a path in X joining $a_j$ to $o$. Let $\nu : F(G)\rightarrow \pi_1(Y, f(o))$ be the unique group homomorphism such that $\nu (g) =f_*(\beta_g)$ for $g\in G$. Let $\mathsf{N}:\pi_1(X, o)*F(G)\rightarrow \pi_1(Y, f(o))$ be the unique group homomorphism which coincides with $\pi_1(f, o)$ on $\pi_1(X, o)$ and with $\nu$ on F(G).

#### Proposition 3 {#ta-iv-s5-prop-3 .statement tag=023I}

Suppose that X is unlaceable. The homomorphism $\mathsf{N}$ is then surjective, and its kernel is the smallest distinguished subgroup of $\pi_1(X, o)*F(G)$ containing the elements

($R_2$)$r_2(k, v) = [k]^{-1}v[k](\beta_k^{-1}k^*(v)^{-1}\beta_k)$

for $k\in G$ and $v\in \pi_1(X, o)$;

($R'_3$)$r'_3(k, j) = [k](\beta_k^{-1}k^*(\gamma_j)^{-1}\gamma_j)$

for $k\in G$ and $j\in \pi_0(X^k)$;

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](\beta_h^{-1}h^*(\beta_k^{-1})\beta_{kh})$

for $k$ and $h\in G$.

The groupoid morphism $\varpi (f)$ induces a morphism

$$
\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)
$$

which is an isomorphism by Theorem 3 (IV, p. 403), since the space X is supposed unlaceable. The proposition then results from II, p. 211, prop. 6.

The three corollaries below follow from the immediately corresponding corollaries of prop. 6 of II, p. 211.

#### Corollary 1 {#ta-iv-s5-prop-3-cor-1 .statement tag=023J}

Suppose that X is unlaceable and that the group G is generated by the stabilizers of the points of X. The canonical morphism $\pi_1(f, o):\pi_1(X, o)\rightarrow \pi_1(Y, f(o))$ is then surjective. In particular, if X is simply connected by arcs, the same is true of Y.

#### Remark {#ta-iv-s5-n4-rem-1 .statement tag=023K}

If X is unlaceable, so is Y (IV, p. 349, prop. 8). Since a connected unlaceable space is simply connected by arcs if and only if it is simply connected (IV, p. 344, corollary 1 of Theorem 1), one thus recovers prop. 11 of I, p. 137.

#### Example 1 {#ta-iv-s5-n4-exa-1 .statement tag=023L}

Let X be an arcwise connected, unlaceable, separated topological space, and let $a$ be a point of X. Let $n$ be an integer $\geqslant 2$ and let Y be the quotient of the space $X^n$ by the action of the group $\mathfrak{S}_n$ operating by permutation of the factors; let $f: X^n\rightarrow Y$ denote the canonical mapping; let $g: X\rightarrow Y$ denote the mapping $x\mapsto f(x, a, . . . , a)$. It follows from the proposition that, for every $i$, the homomorphism $\pi_1(g, a)$ of $\pi_1(X, a)$ into $\pi_1(Y, g(a))$ is surjective and that its kernel is the derived group of $\pi_1(X, a)$. In particular, the group $\pi_1(Y, g(a))$ is abelian.

#### Corollary 2 {#ta-iv-s5-prop-3-cor-2 .statement tag=023M}

Suppose that X is unlaceable and that the group G operates freely in X. There exists a unique group homomorphism $p:\pi_1(Y, f(o))\rightarrow G$ whose kernel contains the image of $\pi_1(X, o)$ and such that $p(\mathsf{N}(g)) =g$ for every $g\in G$. Moreover, $\pi_1(X, o)\rightarrow \pi_1(Y, f(o))-\overset{p}{\rightarrow}G$ is an extension of G by $\pi_1(X, o)$.

#### Corollary 3 {#ta-iv-s5-prop-3-cor-3 .statement tag=023N}

Suppose that X is simply connected by arcs. The mapping of G into $\pi_1(Y, f(o))$ which, to $g\in$ G, associates the path class $f_*(\beta_g)$ is a surjective group homomorphism; its kernel is the subgroup of G generated by the stabilizers of the points of X.

### 5. Cones; contraction of a subspace

Let X and Y be non-empty topological spaces, and let $f: X\rightarrow Y$ be a continuous mapping. Let Cone$(f)$ be the cone of the mapping $f$, and let $s$ be its vertex. Let $\alpha '_f: X\times \mathbf{I}\rightarrow$ Cone$(f)$ and $\beta '_f: Y\rightarrow$ Cone$(f)$ denote the canonical mappings. The restriction of $\alpha '_f$ to the subspace $X\times  \{0\}$ of $X\times \mathbf{I}$ is the constant mapping with image $\{s\}$. The mapping $\beta '_f$ induces a homeomorphism of Y onto the base of the cone Cone$(f)$, by which we shall identify these two spaces. Also denote by

$\sigma '_f: ($Cone$(f)-\{s\})\times \mathbf{I}\rightarrow$ Cone$(f)-\{s\}$

the canonical contraction, and by $\rho '_f:$ Cone$(f)-\{s\} \rightarrow Y$ the canonical retraction of the cone deprived of its vertex onto its base.

Let $J =\pi_0(X)$; for each element $j$ of J, let $X_j$ denote the component $j$ of X, let $b_j$ be a point of $X_j$, and let $\gamma_j$ denote the class of the path $t\mapsto \alpha '_f(b_j, t)$ in Côn$(f)$ joining $s$ to $f(b_j)$.

Let I be the image of the mapping $\pi_0(f)$; this is the set of arcwise connected components of Y which meet $f(X)$; let $\varphi : J\rightarrow I$ denote the mapping deduced from $f$ by passing to arcwise connected components. For each element $i\in I$, let $Y_i$ denote the component $i$ of Y and choose a point $a_i$ in $Y_i$.

For each element $j$ of J, choose a path $B_j$ joining the point $f(b_j)$ to the point $a_{\varphi(j)}$ in $Y_{\varphi(j)}$, and let $\beta_j$ denote its class. Let $\psi_j$ denote the homomorphism from $\pi_1(X, b_j)$ into $\pi_1(Y, a_{\varphi(j)})$ defined by

$$
\psi_j(v) =\beta_j^{-1}f_*(v)\beta_j
$$

for $v\in \pi_1(X, a_j)$.

Let $\sigma : I\rightarrow J$ be a section of the mapping $\varphi$. Put $T =\sigma (I)$ and $\tau =\sigma \circ \varphi$; observe that $\varphi \circ \tau =\varphi$.

#### Proposition 4 {#ta-iv-s5-prop-4 .statement tag=023O}

Suppose that the arcwise connected components of Y are open. For each $i\in$ I, let $G_i$ be the quotient of the group $\pi_1(Y_i, b_i)$ by the smallest normal subgroup containing the image of the homomorphisms $\psi_j$, for $j\in \overset{-1}{\varphi}(i)$ ; let $p_i$ denote the canonical surjection of $\pi_1(Y_i, b_i)$ onto $G_i$.

There exists a unique group homomorphism

$\mathsf{P}:_i*_{\in I}G_i*F(J-T)\rightarrow \pi_1($Côn$(f), s)$

such that

$\mathsf{P}(p_i(v)) =$ Int($\gamma_{\sigma(i)}\beta_{\sigma(i)}$)$(v)$ for $i\in I$ and $v\in \pi_1(Y_i, b_i)$,

$\mathsf{P}(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}$ for $j\in J-T$.

The homomorphism $\mathsf{P}$ is an isomorphism.

Let $Y'$ denote the union of the arcwise connected components of Y which meet $f(X)$, and let $f': X\rightarrow Y'$ be the mapping given by $x\mapsto f(x)$. The set $Y'$ is an open subset of Y; its arcwise connected components are open. The cone Cone$(f')$ is identified with the arcwise connected component of $s$ in Cone$(f)$. This makes it possible to suppose that $Y = Y'$, in other words that the mapping $\pi_0(f)$ is surjective and $I =\pi_0(Y)$.

For each $j\in J$, let us put $V_j=\alpha '_f(X_j\times ]0,1[)$. On passing to subspaces, the mapping $\alpha '_f$ induces a homeomorphism of $X\times ]0,1[$ onto the complement of $Y\cup  \{s\}$ in Cone$(f)$. Hence the sets $V_j$ are the arcwise connected components of Cone$(f)-(Y\cup  \{s\})$.

For each $i\in I$, let us put $U_i= (\rho '_f)^{-1}(Y_i)$; this is an open subset of Cone$(f)$, since $Y_i$ is open in Y by hypothesis. For each $j\in \overset{-1}{\varphi}(i)$, one has $f(X_j)\subset Y_i$ and

$$
V_j\cup Y_i=\alpha '_f(X_j\times ]0,1])\cup Y_i
$$

so that $V_j\cup Y_i$ is an arcwise connected subset of Cone$(f)$ containing $Y_i$. Since $U_i$ is the union of $Y_i$ and of the sets $V_j$, for $j\in \overset{-1}{\varphi}(i)$, it follows that $U_i$ is arcwise connected.

Finally, the set $C'(X) =$ Cone$(f)$ - Y is an open subset of Cone$(f)$; it is contractible to $s$, hence arcwise connected.

The set $C'(X)$ and the sets $U_i$, for $i\in I$, constitute an open arcwise connected covering of Cone$(f)$, to which we shall apply prop. 1 of IV, p. 412. Let $I'$ be the set obtained by adjoining $s$ to I; let it be provided with a total ordering for which $s$ is its smallest element.

For distinct elements $i, i'$ of I, one has $U_i\cap U_{i'}=\emptyset$. For $i\in I$, $C'(X)\cap U_i$ is the union of the sets $V_j$, for $j\in \overset{-1}{\varphi}(i)$; they are connected and pairwise disjoint. The intersection of any three distinct sets of this covering is empty.

The framework Γ of the covering considered has the set $I'$ for its vertices. Its edges are the triplets $(s, i,V_j)$, for $j\in J$ and $i=\varphi (j)$; thus the set of edges of Γ will be identified with the set J.

For $i\in I$, one chooses as base point $\mathsf{a}(i) =a_i\in U_i$; one also puts $\mathsf{a}(s) =s\in C'(X)$.

For $j\in$ J, put $\mathsf{b}(j) =\alpha '_f(b_j,\frac{1}{2})$. Let $B_1(j)$ be the path in $C'(X)$ with origin $\mathsf{b}(j)$ and endpoint $\mathsf{a}(s)$ given by $t\mapsto \alpha '_f(b_j,(1-t)/2)$. Let $B_2(j)$ be the path in $U_{\varphi(j)}$ with origin $\mathsf{b}(j)$ and endpoint $\mathsf{a}(\varphi (j)) =a_{\varphi(j)}$, obtained by juxtaposing the path $t\mapsto \alpha '_f(b_j,(1 +t)/2)$ and the path $B_j$. Then the class of the path $B(j) =\overline{B}_1(j)*B_2(j)$ is equal to $\gamma_j\beta_j$.

We choose $i_0=s$.

We take for maximal oriented tree T the unique oriented tree of Γ whose set of arrows is $\sigma (I)$. We have $\delta (s) =e$, whereas for $i\in I,\delta (i) = [B(\sigma (i))] =\gamma_{\sigma(i)}\beta_{\sigma(i)}$.

Let $j\in J$ and let $i=\varphi (j)$.

The homomorphism $\varphi_j$ of $\pi_1(V_j,\mathsf{b}(j))$ into $\pi_1(C'(X), s)$ is the trivial homomorphism, since $C'(X)$ is contractible to $s$.

The mapping $\alpha '_f$ induces a homeomorphism of $X_j\times ]0,1[$ onto $V_j$; this homeomorphism induces an isomorphism of the group $\pi_1(V_j,\mathsf{b}(j))$ onto the group $\pi_1(X_j, b_j) =\pi_1(X, b_j)$. By passing to subspaces, the mapping $\sigma '_f$ induces a strong contraction of $U_i$ onto $Y_i$, which induces an isomorphism of the group $\pi_1(U_i,\mathsf{a}(i))$ onto the group $\pi_1(Y, a_i)$. By means of these isomorphisms, the homomorphism

$$
\psi_j:\pi_1(V_j,\mathsf{b}(j))\rightarrow \pi_1(U_{\varphi(j)},\mathsf{a}(\varphi (j)))
$$

is identified with the homomorphism Int($\beta_{\varphi(j)}^{-1}$)$\circ f_*$ of $\pi_1(X, b_j)$ into $\pi_1(Y, a_i)$.

Since $C'(X)$ is contractible to $s$, the homomorphism $\mu_s$ is the trivial homomorphism.

Let $i\in I$. The homomorphism $\mu_i$ of $\pi_1(U_i,\mathsf{a}(i))$ into $\pi_1($Côn$(f), s)$ is identified with the homomorphism of $\pi_1(Y, a_i)$ into $\pi_1($Côn$(f), s)$ obtained by composing the homomorphism Int($\delta (i)$) and the homomorphism of $\pi_1(U_i, s)$ into $\pi_1($Côn$(f), s)$ deduced from the canonical injection of $U_i$ into Côn$(f)$.

Finally, the homomorphism $\mu: F(J)\rightarrow \pi_1($Côn$(f), s)$ is given by

$$
\mu(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}
$$

Let $\mathsf{P}'$ be the unique group homomorphism

$\mathsf{P}':_i*_{\in I}\pi_1(Y_i, a_i)*F(J)\rightarrow \pi_1($Cone$(f), s)$

which coincides with the homomorphism Int($\delta (i)^{-1}$) on $\pi_1(Y_i, a_i)$ and with the homomorphism $\mu$ on F(J). By Prop. 1 of IV, p. 412, the homomorphism $\mathsf{P}'$ is surjective and its kernel is the smallest normal subgroup of $*_i\pi_1(Y_i, a_i)*F(J)$ which contains the elements $\mathsf{r}_1(j)$, for $j\in T$, and the elements $\mathsf{r}_2(j, v)$, for $j\in J$ and $v\in \pi_1(V_j,\mathsf{b}(j))$. (There are no elements $\mathsf{r}_3(k)$, since the set K is empty.)

For $j\in T$, one has $r_1(j) =j$. Let $j\in J$ and let $v\in \pi_1(V_j,\mathsf{b}(j))$. In view of the identification of $\pi_1(V_j,\mathsf{b}(j))$ with $\pi_1(X, b_j)$, one has $\mathsf{r}_2(j, v) =j\psi_j(v)j^{-1}$. Let $p$ denote the canonical surjective homomorphism of $*\pi_1(Y_i, a_i)*F(J)$ onto $*G_i*F(J$ - T). For $j\in T$, one has $p(\mathsf{r}_1(j)) =^ie$; for $j\in J$ and $v\in \pi_1(X^i, b_j)$, one has $p(\psi_j(v)) =e$. Hence there exists a unique group homomorphism $\mathsf{P}$ of $*G_i*F(J-T)$ into $\pi_1($Cone$(f), s)$ such that $\mathsf{P}'\circ p=\mathsf{P}$; it is an isomorphism.$^i$

#### Corollary 1 {#ta-iv-s5-prop-4-cor-1 .statement tag=023P}

Suppose moreover that the spaces X and Y are arcwise connected and let $a$ be a point of X. The canonical mapping of $\pi_1(Y, f(a))$ into $\pi_1($Cone$(f), f(a))$ is surjective, and its kernel is the smallest normal subgroup which contains the image of the homomorphism $\pi_1(f, a)$.

#### Corollary 2 {#ta-iv-s5-prop-4-cor-2 .statement tag=023Q}

Suppose moreover that the arcwise connected components of Y are simply arcwise connected. The homomorphism $\mu: F(J-T)\rightarrow \pi_1($Cone$(f), s)$ is then an isomorphism.

#### Remark 1 {#ta-iv-s5-n5-rem-1 .statement tag=023R}

Let X be a topological space whose arcwise connected components are open. Let A be a closed subspace of X; let $\iota : A\rightarrow$ X denote the canonical injection, let $X/A$ denote the space deduced from X by contracting A to a point $o$, and let $p: X\rightarrow X/A$ denote the canonical mapping. Suppose further that the pair $(X,A)$ has the homotopy extension property. The canonical mapping $\overline{\rho}:$ Cone$(\iota )\rightarrow X/A$ is then a homotopy equivalence (III, p. 255, Remark 1), and one deduces from Prop. 4 the calculation of the Poincaré group of $X/A$ at its base point $o$. In particular, if the arcwise connected components of X are simply arcwise connected, the group $\pi_1(X/A, o)$ is a free group.

### 6. Blowing up and gluing back together

Let C be a topological space and let $(B_{\ell})_{\ell\in L}$ be a finite family of closed subsets of C, pairwise disjoint. Let B be a topological space and, for each $\ell \in L$, let $h_{\ell}$ be a homeomorphism of B onto $B_{\ell}$. We denote by $B_L$ the union of the family $(B_{\ell})_{\ell\in L}$. We shall suppose that B and L are non-empty. Let R be the equivalence relation on C defined as follows. The class of an element $x$ of $C-B_L$ is the set $\{x\}$; if $x$ is an element of $B_{\ell}$, where $\ell \in L$, the class of $x$ is

the set of elements $h_k(\overset{-1}{h_{\ell}}(x))$, where $k$ runs through L. Let A be the quotient topological space $C/R$ and $f: C\rightarrow A$ the canonical surjection. One says that the space A is obtained from the space C by identification of the sets $B_{\ell}$ by means of the homeomorphisms $h_{\ell}$.

The mapping $f\circ h_{\ell}$ of B into A is independent of the element $\ell$ of L; it is closed and injective; it therefore induces a homeomorphism of B onto a closed subset of A. Thus we identify B with $f\circ h_{\ell}(B)$ by means of the homeomorphism $f\circ h_{\ell}$; the mapping $f$ induces a homeomorphism of $C-B_L$ onto A-B.

Suppose moreover that there exists a family $(N_{\ell})_{\ell\in L}$ of open subsets of C, pairwise disjoint, such that $N_{\ell}$ contains $B_{\ell}$ for each $\ell \in L$. The union U of the family $(f(N_{\ell}))_{\ell\in L}$ is open in A and contains B. The set U-B is the union of the pairwise disjoint open sets $f(N_{\ell}-B_{\ell})$, for $\ell \in L$.

#### Lemma 2 {#ta-iv-s5-lem-2 .statement tag=023S}

The mapping $f: C\rightarrow A$ is proper and separated; its fibres are finite.

Let us prove that $f$ is closed. Let X be a closed subset of C. Let us prove that its image is closed in A. For each $\ell \in L$, $X\cap B_{\ell}$ is closed in $B_{\ell}$, hence the space $Y =\bigcup_{\ell\in L}h^{-1}_{\ell}(X\cap B_{\ell})$ is closed in B since L is finite. The saturation $X^*$ of X for the equivalence relation R is then equal to $X\cup \bigcup_{\ell\in L}h_k(Y)$, hence is closed in C. Consequently, $f(X) =f(X^*)$ is closed in A, which was to be proved.

The fibres of $f$ are the equivalence classes of the relation R; they are finite. Consequently, the mapping $f$ is proper (TG, I, p. 75, Theorem 1).

Lastly, let us show that $f$ is separated. Let $x$ and $y$ be distinct points of C which have the same image under $f$. There therefore exists a point $b\in B$ and distinct elements $\ell$ and $m\in L$ such that $x=h_{\ell}(b)$ and $y=h_m(b)$. Consequently, $N_{\ell}$ and $N_m$ are disjoint neighbourhoods of $x$ and $y$ in C, whence the required assertion by virtue of Prop. 1 of I, p. 25.

Assume in addition the following hypotheses:

– the space A is simply connected and connected;

– the space C is simply connected;

– the space B is connected and locally arcwise connected.

Let us put $I =\pi_0(C)$; if $i$ is an element of I, let $C_i$ denote the connected component $i$ of C. Let $\eta : L\rightarrow I$ denote the mapping which associates to an element $\ell \in L$ the connected component of C containing $B_{\ell}$. The mapping $\eta$ is surjective. For, arguing by contradiction, consider a connected component X of C which meets no set $B_{\ell}$. It is an open and closed subset of C, saturated with respect to the equivalence relation R. Hence its image $f(X)$ is an open and closed subset of A, disjoint from B. Since A is assumed connected and B nonempty, $f(X)$ is empty, whence a contradiction.

Let $\sigma : I\rightarrow L$ be a section of the mapping $\eta$; put $\tau =\sigma \circ \eta$ and $T =\sigma (I)$.

Choose a point $b$ of B. For every $\ell \in L$, put $b_{\ell}=h_{\ell}(b)$ and choose the class $\beta_{\ell}$ of a path joining $b_{\ell}$ to $b_{\tau(\ell)}$ in C; if $\ell =\tau (\ell )$, choose for $\beta_{\ell}$ the class of the constant path whose image is $b_{\ell}$. For every $\ell \in L$, let $\vartheta_{\ell}$ denote the homomorphism from $\pi_1(B, b)$ into $\pi_1(C, b_{\tau(\ell)})$ defined by

$\vartheta_{\ell}(v) =$ Int($\beta_{\ell}$)$^{-1}((h_{\ell})_*(v)) =\beta_{\ell}^{-1}(h_{\ell})_*(v)\beta_{\ell}$,

for every $v\in \pi_1(B, b)$. Finally, fix an element $\ell_0$ of L such that $\ell_0=$ $\tau (\ell_0)$.

Let $\mathsf{Q}$ be the unique group homomorphism

$$
\mathsf{Q}:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)\rightarrow \pi_1(A, b)
$$

such that $\mathsf{Q}(\ell ) =f_*(\beta_{\ell})$ for every $\ell \in$ L - T and which coincides with $\pi_1(f, b_{\sigma(i)})$ on $\pi_1(C_i, b_{\sigma(i)})$ for every $i\in I$.

#### Proposition 5 (Van Kampen) {#ta-iv-s5-prop-5 .statement tag=023T}

The homomorphism $\mathsf{Q}$ is surjective; its kernel is the smallest normal subgroup containing the elements

$\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$ for $v\in \pi_1(B, b)$ and $\ell \in T$,

$\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$ for $v\in \pi_1(B, b)$ and $\ell \in L-T$.

The mapping $f: C\rightarrow$ A is proper, separated, with finite fibres (IV, p. 430, lemma 2); the spaces A and C are unlaceable. Moreover, $C\times_AC$ is the union of the diagonal $\Delta_C$ and of the disjoint subsets $B_{\ell}\times_AB_k=$ $(h_{\ell}, h_k)(B)$, for $(\ell , k)\in L^2$ with $\ell =\not k$. For such a pair $(\ell , k)$, we have $B_{\ell}\times_AB_k= N_{\ell}\times_AN_k$; hence this subset is open and closed in $C\times_AC$. Thus the diagonal $\Delta_C$ is open, and its complement in $C\times_AC$, a finite union of disjoint subsets homeomorphic to B, is locally connected. This proves that the mapping $f$ satisfies property (VK) (case (ii) of IV, p. 405). With a view to applying theorem 1 of IV, p. 408, we are going to define van Kampen data for $f$.

For each $i\in I$, let us choose as base point in $C_i$ the point $\mathsf{a}(i) =$ $b_{\sigma(i)}$.

Let J be the set of path-connected components of $C\times_AC$. The sets $\Delta_{C_i}$, for $i\in I$, are the connected components of the diagonal $\Delta_C$, which is open and closed in $C\times_AC$, therefore these sets belong to J. Analogously, the sets $[\ell_1, \ell_2] = B_{\ell_1}\times_A$ $B_{\ell_2}$ for $\ell_1$ and $\ell_2$ in L with $\ell_1=\not\ell_2$, belong to J. Since these sets form a partition of $C\times_AC$, they describe the set J.

Let $j$ be an element of J of the form $\Delta_{C_i}$, for $i\in I$. Let us choose as base point $\mathsf{b}(j)$ the point $(\mathsf{a}(i),\mathsf{a}(i)) = (b_{\sigma(i)}, b_{\sigma(i)})$ and let us take for path classes $\beta_1(j)$ and $\beta_2(j)$ the class of the constant path at $b_{\sigma(i)}$. Let $j$ be an element of J of the form $[\ell_1, \ell_2]$, where $\ell_1$ and $\ell_2$ are distinct elements of L. Let us then put $\mathsf{b}([\ell_1, \ell_2]) = (b_{\ell_1}, b_{\ell_2}),\beta_1([\ell_1, \ell_2]) =\beta_{\ell_1}$ and $\beta_2([\ell_1, \ell_2]) =\beta_{\ell_2}$.

Let $K =\pi_0(C\times_AC\times_AC)$.

Let $\Delta '_C$ denote the diagonal of the space $C\times_AC\times_AC$; this is a closed subset of $C\times_AC\times_AC$, because $f$ is separated, and it is homeomorphic to C. For every $i\in$ I, let $\Delta '_{C_i}$ also denote the image of $C_i$ under the diagonal mapping of C into $C\times_AC\times_AC$; these are open and closed subsets of $\Delta '_C$. For every triplet $(\ell_1, \ell_2, \ell_3)$ of elements of L, put also $[\ell_1, \ell_2, \ell_3] = B_{\ell_1}\times_AB_{\ell_2}\times_AB_{\ell_3}$; these are closed subsets of $C\times_A$ $C\times_AC$, homeomorphic to B. If the set $\{\ell_1, \ell_2, \ell_3\}$ has at least two elements, one has $[\ell_1, \ell_2, \ell_3] = N_{\ell_1}\times_AN_{\ell_2}\times_AN_{\ell_3}$, which implies that $[\ell_1, \ell_2, \ell_3]$ is also open in $C\times_AC\times_AC$. Moreover, $C\times_AC\times_AC$ is the union of the pairwise disjoint subsets $\Delta '_C$ and $[\ell_1, \ell_2, \ell_3]$, where $(\ell_1, \ell_2, \ell_3)$ runs through the set of triplets of elements of L which are not all equal to one and the same element. Thus, $\Delta_{C'}$, then the $\Delta '_{C_i}$, for $i\in I$, are open and closed in $C\times_AC\times_AC$. This implies that the set K of connected components of this space is the union of the following disjoint sets $K_0$ and $K_1$.

The set $K_0$ is the set of components of the form $\Delta '_{C_i}$. Let $i\in I$ and let $k= \Delta '_{C_i}$. Put $\mathsf{c}(k) = (b_{\sigma(i)}, b_{\sigma(i)}, b_{\sigma(i)})$. For $(s, t)\in  \{(1,2),(2,3),(1,3)\}$, choose for $\gamma_{st}(k)$ the class of the constant path at $(b_{\sigma(i)}, b_{\sigma(i)})$.

The set $K_1$ consists of the components of the form $k$ = $[\ell_1, \ell_2, \ell_3]$, where $\ell_1, \ell_2, \ell_3$ are three elements of B such that the set $\{\ell_1, \ell_2, \ell_3\}$ is of cardinal $\geqslant 2$. Put $\mathsf{c}(k) = (b_{\ell_1}, b_{\ell_2}, b_{\ell_3})$. Let $(s, t)\in  \{(1,2),(1,3),(2,3)\}$. If $\ell_s=\ell_t$, take for $\gamma_{st}(k)$ the class $(\beta_{\ell_s}, \beta_{\ell_t})$; if $\ell_s=\not\ell_t$, take for $\gamma_{st}(k)$ the class of the constant path at $(b_{\ell_s}, b_{\ell_t})$.

It is then verified that, for every $k\in K$ and for every $s\in  \{1,2,3\}$, the class of loops $\lambda_s(k)$ defined by relation (2) of IV, p. 407, is trivial.

The framework $\mathsf{\Gamma}$ of the pair of groupoid morphisms $(\varpi (p_1), \varpi (p_2))$ from $\varpi (C\times_AC)$ into $\varpi (C)$ has as vertices the set I and as oriented edges the set J. If $i\in I$, the arrow $j= \Delta_{C_i}$ has origin and end $i$; if $(\ell_1, \ell_2)$ is a pair of distinct elements of L, the arrow $j= [\ell_1, \ell_2]$ has origin $\eta (\ell_1)$ and end $\eta (\ell_2)$.

Let $\mathsf{T}$ be the subquiver of $\mathsf{\Gamma}$ whose set of vertices is I and whose arrows are those of the form $[\ell_0, \ell ]$, for $\ell \in T-\{\ell_0\}$. The associated graph of $\mathsf{T}$ is a maximal tree of $\widetilde{\mathsf{\Gamma }}$.

Put $i_0=\eta (\ell_0)$.

If $i\in I-\{i_0\}$, the unique path in $\mathsf{T}$ joining $i_0$ to $i$ is $(i_0,[\ell_0, \sigma (i)], i)$. The groupoid morphism from Grp($\mathsf{\Gamma}$) into $\varpi (Y)$ defined on p. 407 (and denoted by $\tau$ loc. cit.) maps $j$ to the identity element if $j= \Delta_{C_i}$, for $i\in I$, and maps $j= [\ell_1, \ell_2]$ to $f_*(\beta_{\ell_1})^{-1}f_*(\beta_{\ell_2})$, if $\ell_1$ and $\ell_2$ are distinct elements of L. For every $i\in I$, the path class $\delta_i$ defined loc. cit. and joining $b=f(b_{\sigma(i_0)})$ to $b=f(b_{\sigma(i)})$ is given by

$$
\delta_i=f_*(\beta_{\ell_0})^{-1}f_*(\beta_{\sigma(i)}) =e
$$

because $\beta_{\ell}=e$ if $\ell \in T$.

Thus a van Kampen datum of the mapping $f$ has been defined. Consider then the unique group homomorphism

$$
\mathsf{Q}':(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow \pi_1(A, b)
$$

which coincides with $\pi_1(f, b_{\sigma(i)})$ on $\pi_1(C, b_{\sigma(i)})$ and such that

$$
\mathsf{Q}'(j) =f_*(\beta_1(j))^{-1}f_*(\beta_2(j))
$$

for $j\in J$. By IV, p. 408, Theorem 1, this homomorphism is surjective and its kernel is the smallest normal subgroup containing the relators $\mathsf{r}_1(j)$ (for $j\in$ Fl($\mathsf{T}$)), $\mathsf{r}_2(j, v)$ (for $j\in$ J and $v\in$ $\pi_1(C\times_AC,\mathsf{b}(j))$) and $\mathsf{r}_3(k)$ (for $k\in K$) defined, loc. cit., by equations ($R_1$)$, (R_2)$ and ($R_3$).

Let $q'$ be the unique homomorphism of F(L) into F(L - T) such that $q'(\ell ) =\ell$ if $\ell \in L-T$ and $q'(\ell ) =e$ otherwise. Let

$$
q:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow (_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)
$$

be the unique group homomorphism which coincides with the identity on $\pi_1(C_i, b_{\sigma(i)})$, for $i\in$ I and such that one has $q(j) =e$ if $j= \Delta_{C_i}$, $q([\ell , \ell ']) =q'(\ell )^{-1}q'(\ell ')$ if $\ell$ and $\ell '$ are distinct elements of L. The homomorphism $q$ is surjective.

If $i\in I$ and $j= \Delta_{C_i}$, one has $\mathsf{Q}'(j) =e_b=\mathsf{Q}'(q(j))$. If $j= [\ell , \ell ']$, for $\ell$ and $\ell '$ in L, distinct, one has

$$
\mathsf{Q}'(j) =f_*(\beta_{\ell})^{-1}f_*(\beta_{\ell'}) =\mathsf{Q}(q'(\ell ))^{-1}\mathsf{Q}(q'(\ell '))
$$

$$
=\mathsf{Q}(q'(\ell )^{-1}q'(\ell ')) =\mathsf{Q}\circ q([\ell , \ell '])
$$

Therefore, $\mathsf{Q}'$ = $\mathsf{Q}\circ q$. It follows that the homomorphism $\mathsf{Q}$ is surjective and that its kernel is the smallest normal subgroup of $(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)$ containing the images under $q$ of the relators $\mathsf{r}_1(j)$ (for $j\in$ Fl($\mathsf{T}$))$,\mathsf{r}_2(j, v)$ (for $j\in J$ and $v\in \pi_1(C\times_AC,\mathsf{b}(j))$) and $\mathsf{r}_3(k)$ (for $k\in K$).

If $\ell \in T-\{\ell_0\}$ and $j= [\ell_0, \ell ]$, one has $\mathsf{r}_1(j) =j$ and $q(\mathsf{r}_1(j)) =e$.

Let $k\in K$. One has $\mathsf{r}_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. If $k= \Delta '_{C_i}$, for $i\in I$, let us put $j= \Delta_{C_i}$; then one has

$$
q(\mathsf{r}_3(k)) =q(jjj^{-1}) =q(j) =e
$$

Let $\ell$ and $\ell '$ be distinct elements of L. If $k= [\ell , \ell , \ell ']$, one has therefore

$$
q(\mathsf{r}_3(k)) =q(\Delta_{C_{\eta(\ell)}}[\ell , \ell '][\ell , \ell ']^{-1}) =q(\Delta_{C_{\eta(\ell)}}) =e
$$

If $k= [\ell , \ell ', \ell ]$, one gets

$$
q(\mathsf{r}_3(k)) =q([\ell , \ell '][\ell ', \ell ]\Delta^{-1_{(\ell)}}_{C_{\eta}})
$$

$$
=q'(\ell )^{-1}q'(\ell ')q'(\ell ')^{-1}q'(\ell )q(\Delta_{C_{\eta}(\ell)})^{-1}=e
$$

Moreover, if $k= [\ell ', \ell , \ell ]$, one has

$$
q(\mathsf{r}_3(k)) =q([\ell ', \ell ]\Delta_{C_{\eta(\ell)}}[\ell ', \ell ]^{-1})
$$

$$
=q(\ell ')^{-1}q(\ell )q(\Delta_{C_{\eta(\ell)}})q(\ell )^{-1}q(\ell ') =e
$$

Finally, if $k= [\ell_1, \ell_2, \ell_3]$, where $\ell_1, \ell_2, \ell_3$ are elements of L, pairwise distinct, one has

$$
q(\mathsf{r}_3(k)) =q([\ell_1, \ell_2])q([\ell_2, \ell_3])q([\ell_1, \ell_3])^{-1}=e
$$

Let $i\in I$ and put $j= \Delta_{C_i}$. The group homomorphisms $\varphi_j$ and $\psi_j$, from $\pi_1(C\times_AC,\mathsf{b}(j)) =\pi_1(C_i,\mathsf{a}(i))$ into $\pi_1(C,\mathsf{a}(i))$ defined by relations (1) of IV, p. 407, are equal respectively to $(p_1)_*$ and to $(p_2)_*$. We have then, for $v\in \pi_1(C_i,\mathsf{a}(i)),\mathsf{r}_2(j, v) =vjv^{-1}j^{-1}$, whence $q(\mathsf{r}_2(j, v)) =e$.

Finally, let $j= [\ell , \ell ']$, where $\ell$ and $\ell '$ are distinct elements of L. The group homomorphism $\varphi_j:\pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))\rightarrow \pi_1(C_{\eta(\ell)}, b_{\tau(\ell)})$ defined loc. cit. is the homomorphism $\vartheta_{\ell}$, and the homomorphism $\psi_j$ is the homomorphism $\vartheta_{\ell'}$. We have then, for $v\in \pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))$

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)q'(\ell )^{-1}q'(\ell ')\vartheta_{\ell'}(v)^{-1}q'(\ell ')^{-1}q'(\ell )
$$

Let us distinguish four cases. If $\ell$ and $\ell '$ both belong to T, we have

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})
$$

When $\ell '=\ell_0$, we obtain the inverse of the element $\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$. If $\ell \in T$ but $\ell '\notin T$, we have

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

$$
=(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

Analogously, if $\ell \notin T$ and $\ell '\in T$, we have

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell'}(v)^{-1}\ell
$$

$$
=\ell^{-1}(\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})\ell
$$

Taking $\ell '=\ell_0$, we obtain an element conjugate to the inverse of $\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$. Finally, if neither $\ell$ nor $\ell '$ belongs to T, we have

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell_0}(v)^{-1}\ell )\ell^{-1}(\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1})\ell
$$

These relations prove, on the one hand, that the elements announced in the proposition belong to the kernel of the homomorphism $\mathsf{Q}$, and, on the other hand, that these elements $q(\mathsf{r}_2(j, v))$ all belong to the smallest normal subgroup containing the elements announced in the statement. The proposition follows.

#### Remark {#ta-iv-s5-n6-rem-1 .statement tag=023U}

Let A be a topological space, let B be a closed subset of A, and let U be an open neighbourhood of B in A. Suppose that the set U-B is the union of a finite family $(M_{\ell})_{\ell\in L}$ of pairwise disjoint open sets. For each $\ell \in L$, put $N'_{\ell}= M_{\ell}\cup B$. Let $C'$ denote the topological sum of the spaces A-B and $N'_{\ell}$, for $\ell \in L$; let also $\varphi : A-B\rightarrow C'$ and $\varphi_{\ell}: N'_{\ell}\rightarrow C'$, for $\ell \in L$, denote the canonical injections. Let C be the quotient topological space of $C'$ by the finest equivalence relation S for which the points $\varphi (x)$ and $\varphi_{\ell}(x)$ are equivalent, for each $\ell \in L$ and each $x\in M_{\ell}$; let $\rho : C'\rightarrow C$ be the canonical mapping.

Let us prove that the space A is recovered from the space C by identification of the sets $B_{\ell}$ by means of the homeomorphisms $\rho \circ$ $(\varphi_{\ell}|B): B\rightarrow B_{\ell}$.

For every $\ell \in L$, the set $M_{\ell}$ is open in A-B and in $N'_{\ell}$. The mappings $\rho \circ \varphi$ and $\rho \circ \varphi_{\ell}$ are homeomorphisms of the spaces A-B and $N'_{\ell}$, for $\ell \in L$, onto open subsets of C (TG, I, p. 17, Prop. 9). For every $\ell \in L$, the set $\varphi_{\ell}(B)$ is closed in $C'$ and saturated for the equivalence relation S. Hence the set $B_{\ell}=\rho (\varphi_{\ell}(B))$ is closed in C and the mapping $\rho \circ \varphi_{\ell}$ induces a homeomorphism of B onto $B_{\ell}($loc. cit.). Analogously, for every $\ell \in L$, the set $N_{\ell}=\rho (\varphi_{\ell}(N'_{\ell}))$ is an open neighbourhood of $B_{\ell}$; the sets $N_{\ell}$ are mutually disjoint.

By passing to the quotient, the mapping $f': C'\rightarrow A$ deduced from the canonical injections into A of the spaces A-B and $N_{\ell}$, for $\ell \in L$, induces a

continuous mapping $f: C\rightarrow A$. If $x$ is a point of B, the fibre $\overset{-1}{f}(x)$ is the set of points $\rho (\varphi_{\ell}(x))$, for $\ell \in L$. The equivalence relation on C associated with the mapping $f$ is the relation R defined at the beginning of the number. Let $B_L$ denote the union of the family $(B_{\ell})_{\ell\in L}$. By construction, the mapping $f$ induces a homeomorphism of $C-B_L$ onto A-B and, for $\ell \in L$, a homeomorphism of $N'_{\ell}$ onto $N_{\ell}$. We shall prove that the mapping $f$ is closed; the topology of A will therefore be the quotient topology of C by the equivalence relation R (I, p. 18, Example 2). For this, let us prove that if F is a subset of A such that $F\cap (A-B)$ is closed in A-B and such that $F\cap N'_{\ell}$ is closed in $N'_{\ell}$, for $\ell \in L$, the set F is closed in A. The set U, union of the family $(N'_{\ell})_{\ell\in L}$, is open in A and the sets $N'_{\ell}$, for $\ell \in L$, constitute a finite closed covering of it. Hence the set $F\cap U$ is closed in U (TG, I, p. 18, Prop. 3). The sets U and A-B form an open covering of A, therefore the set F is closed in A (loc. cit.).

## EXERCISES {#ta-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
