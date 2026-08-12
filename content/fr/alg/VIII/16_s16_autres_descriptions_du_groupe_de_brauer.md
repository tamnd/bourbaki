---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 16
section_title: Autres descriptions du groupe de Brauer
lang: fr
source: alg-viii-fr
book_pages: A VIII.281-A VIII.328
pdf_pages: 0284-0331
extraction: native
subsections:
    - "no": 1
      title: $\tau$-extensions de groupes
      page: 281
      pdf_page: 284
    - "no": 2
      title: Image inverse d’une $\tau$-extension
      page: 283
      pdf_page: 286
    - "no": 3
      title: Image directe d’une $\tau$-extension
      page: 285
      pdf_page: 288
    - "no": 4
      title: Loi de groupe sur les classes de $\tau$-extensions
      page: 289
      pdf_page: 292
    - "no": 5
      title: Description cohomologique
      page: 291
      pdf_page: 294
    - "no": 6
      title: Restriction et corestriction
      page: 294
      pdf_page: 297
    - "no": 7
      title: Algèbres galoisiennes
      page: 300
      pdf_page: 303
    - "no": 8
      title: Opérations sur les algèbres galoisiennes
      page: 307
      pdf_page: 310
    - "no": 9
      title: Produits croisés
      page: 309
      pdf_page: 312
    - "no": 10
      title: Application au groupe de Brauer
      page: 312
      pdf_page: 315
    - "no": 11
      title: Indice et exposant
      page: 317
      pdf_page: 320
statements: 63
exercises: 17
content_sha256: affcfeb2439479ad0f3e0d3588f3ce0f1244ca79339c32d92f9d3be594c8f876
---

## § 16. AUTRES DESCRIPTIONS DU GROUPE DE BRAUER

Dans ce paragraphe, si F est un groupe abélien et $g$ un automorphisme de F, on note $g.f$ pour $g(f)$.

### 1. $\tau$-extensions de groupes

Dans ce numéro, on fixe un groupe G, un groupe abélien F noté multiplicativement et un homomorphisme de groupes $\tau$ de G dans le groupe Aut(F) des automorphismes du groupe F. On note $e$ l’élément neutre de G et 1 l’élément neutre de F.

Rappelons (I, p. 62) qu’une extension $\mathscr{E}$ de G par F est un triplet $(\Gamma , \iota , \pi )$, où Γ est un groupe, $\pi : \Gamma \rightarrow G$ est un homomorphisme surjectif et $\iota$ un homomorphisme injectif de F dans Γ tel que Im($\iota$ ) $=$ Ker($\pi$ ). Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une telle extension. Pour tout $\gamma \in \Gamma$, l’application $\varphi_{\gamma}: F\rightarrow F$ définie par

$$
\iota (\varphi_{\gamma}(f)) =\gamma \iota (f)\gamma^{-1}
$$

pour tout $f\in F$ est un automorphisme de F. Comme F est commutatif, pour tout $f\in F$, l’automorphisme défini par $\iota (f)$ est l’application identique de F. Par passage au quotient, on obtient un homomorphisme Int$_{\mathscr{E}}$ de G dans Aut(F) caractérisé par

$\gamma \iota (f)\gamma^{-1}=\iota$(Int$_{\mathscr{E}}(\pi (\gamma )).f)$

pour $\gamma \in \Gamma$ et $f\in F$.

On appelle $\tau$-extension de G par F une extension $\mathscr{E}= (\Gamma , \iota , \pi )$ telle que Int$_{\mathscr{E}}$ soit égal à $\tau$, c’est-à-dire vérifiant la relation

$$
\gamma \iota (f)\gamma^{-1}=\iota (\tau (\pi (\gamma )).f) \tag{1}
$$

pour $\gamma \in \Gamma$ et $f\in F$. Si $\mathscr{E}= (\Gamma , \iota , \pi )$ et $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ sont des $\tau$-extensions, un morphisme de $\tau$-extensions de $\mathscr{E}$ dans $\mathscr{E}'$ est un morphisme d’extensions de $\mathscr{E}$ dans $\mathscr{E}'$ (I, p. 63), c’est-à-dire un homomorphisme de groupes $u: \Gamma \rightarrow \Gamma '$ tel que $\pi '\circ u=\pi$ et $\iota '=u\circ \iota$. Notons que les $\tau$-extensions forment une espèce de structure pour laquelle tout morphisme est un isomorphisme (E, IV, p. 6 et I, p. 63, prop. 1). Notons Iso$_{\tau}(\mathscr{E},\mathscr{F})$ la relation

« $\mathscr{E}$ et $\mathscr{F}$ sont des $\tau$-extensions isomorphes. »

C’est une relation d’équivalence ; on appelle classe de l’extension $\mathscr{E}$ la classe d’objets équivalents à $\mathscr{E}$ pour Iso$_{\tau}$ (E, II, p. 47).

#### Lemme 1 {#alg-viii-s16-lem-1 .statement tag=00I9}

La relation

« $\alpha$ est la classe d’une $\tau$-extension pour Iso$_{\tau}$ »

est collectivisante en $\alpha$.

Posons $E_0= F\times G$ et considérons les applications $\iota_0: F\rightarrow E_0$ et $\pi_0: E_0\rightarrow G$ définies par $\iota_0(f) = (f, e)$ pour $f\in F$ et $\pi_0(f, g) =g$ pour $(f, g)\in F\times G$. Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension de G par F. L’application $\pi$ est surjective, donc possède une section $\sigma : G\rightarrow \Gamma$ telle que $\sigma (e) =e$. L’application $u: (f, g)\rightarrow \iota (f)\sigma (g)$ de $F\times G$ dans Γ est bijective. Munissons $F\times G$ de la loi de groupe obtenue par transport de structure. Le triplet $(E_0, \iota_0, \pi_0)$ est alors une $\tau$-extension isomorphe à $\mathscr{E}$. Le lemme 1 résulte alors de E, II, p. 47.

On note Ex$_{\tau}(G,F)$ l’ensemble des classes de $\tau$-extensions pour la relation Iso$_{\tau}$.

#### Exemple 1 {#alg-viii-s16-n1-exa-1 .statement tag=00IA}

Le produit semi-direct externe $(F\times_{\tau}G, i, p)$ (I, p. 64, prop. 3) est une $\tau$-extension qu’on notera $\mathscr{I}_{\tau}$. On dira qu’une $\tau$-extension est semi-triviale si elle est isomorphe à la $\tau$-extension $\mathscr{I}_{\tau}$.

#### Exemple 2 {#alg-viii-s16-n1-exa-2 .statement tag=00IB}

Pour $i\in  \{1,2\}$, on se donne un groupe $G_i$, un groupe abélien $F_i$ et un homomorphisme de groupes $\tau_i$ de $G_i$ dans le groupe des automorphismes de $F_i$. On note $\tau_1\times \tau_2: G_1\times G_2\rightarrow$ Aut(F$_1\times F_2)$ l’homomorphisme défini par

$$
(\tau_1\times \tau_2)(g_1, g_2).(f_1, f_2) = (\tau_1(g_1).f_1, \tau_2(g_2).f_2)
$$

pour $g_1\in G_1,g_2\in G_2,f_1\in F_1$ et $f_2\in F_2$. Soient $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ une $\tau_1$-extension de $G_1$ par $F_1$ et $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ une $\tau_2$-extension de $G_2$ par $F_2$. Alors le triplet $(\Gamma_1\times \Gamma_2, \iota_1\times \iota_2, \pi_1\times \pi_2)$ est une $\tau_1\times \tau_2$-extension de $G_1\times G_2$ par $F_1\times F_2$ appelée le produit extérieur des extensions $\mathscr{E}_1$ et $\mathscr{E}_2$ et notée $\mathscr{E}_1\times \mathscr{E}_2$.

### 2. Image inverse d’une $\tau$-extension

Soient G et $G'$ des groupes. Soit F un groupe abélien, soit $\tau : G\rightarrow$ Aut(F) un homomorphisme de groupes et soit $u: G'\rightarrow G$ un homomorphisme de groupes. Considérons l’homomorphisme de groupes $\tau '=\tau \circ u: G'\rightarrow$ Aut(F) et notons $\Gamma '$ le produit fibré $\Gamma \times_GG'$ relativement à $\pi$ et $u$ (I, p. 44). C’est le sous-groupe de $\Gamma \times G'$ formé des couples $(\gamma , g')$ tels que $\pi (\gamma ) =u(g')$. Soit $\iota ': F\rightarrow \Gamma '$ l’homomorphisme de groupes donné par $\iota '(\alpha ) = (\iota (\alpha ), e)$ pour $\alpha \in F$ et notons $\pi ': \Gamma '\rightarrow G'$ la seconde projection. Alors le morphisme $\iota '$ est injectif, le morphisme $\pi '$ est surjectif puisque $\pi$ l’est et l’image de $\iota '$ coïncide avec le noyau de $\pi '$. En outre, pour tout $\alpha \in F$ et tout $\gamma '= (\gamma , g)\in \Gamma '$, on a les relations

$$
\gamma '\iota '(\alpha )\gamma^{'-1}= (\gamma , g)(\iota (\alpha ), e)(\gamma , g)^{-1}= (\iota (\tau (\pi (\gamma )).\alpha ), e) =\iota '(\tau '(\pi '(\gamma ')).\alpha )
$$

Par conséquent, $(\Gamma ', \iota ', \pi ')$ est une $\tau '$-extension de $G'$ par F qu’on appelle l’image inverse par $u$ de $\mathscr{E}$ et qu’on note $u^*(\mathscr{E})$. La première projection est un homomorphisme de groupes $\varphi : \Gamma '\rightarrow \Gamma$ qui sera dit canonique.

#### Proposition 1 {#alg-viii-s16-prop-1 .statement tag=00IC}

Le diagramme

F $^{\iota'}$ // $\Gamma '^{\pi'}$ // $G'$

$$
\varphi \tag{2}
$$

$u$

F $^{\iota}$ // Γ $^{\pi}$ // G

est commutatif. En outre, si $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$est une $\tau '$-extension et $\varphi_1: \Gamma '_1\rightarrow \Gamma$est un homomorphisme de groupes tel que le diagramme

F $^{\iota'_1}$ // $\Gamma '_1^{\pi'_1}$ // $G'$

$\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

soit commutatif, alors il existe un unique morphisme $\psi$ de $\tau '$-extensions de $\mathscr{E}_1'$ dans $u^*(\mathscr{E})$tel qu’on ait $\varphi_1=\varphi \circ \psi$.

La commutativité du premier diagramme découle de la définition de $\varphi$. L’existence et l’unicité de $\psi$ résultent du lemme qui suit.

#### Lemme 2 {#alg-viii-s16-lem-2 .statement tag=00ID}

Soit $F'_1$ un groupe abélien et soient $w: F'_1\rightarrow F$et $\tau_1: G'\rightarrow$ Aut(F$'_1)$ des homomorphismes de groupes tels que

$$
w(\tau_1(g)(f)) =\tau (u(g))(w(f))
$$

pour tout $f\in F'_1$ et tout $g\in G'$. Soit $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi_1')$une $\tau_1$-extension de $G'$ par $F'_1$ et $\varphi_1: \Gamma '_1\rightarrow \Gamma$un homomorphisme de groupes tel que le diagramme

$F'_1^{\iota'_1}$ // $\Gamma '_1^{\pi_1'}$ // $G'$

$w\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

soit commutatif. Alors il existe un unique homomorphisme de groupes $\psi : \Gamma '_1\rightarrow \Gamma '$ tel que le diagramme

$F'_1^{\iota'_1}$ // $\Gamma '_1^{\pi_1'}$ // $G'$

$w\psi$

F $^{\iota'}$ // $\Gamma '^{\pi'}$ // $G'$

soit commutatif et tel que $\varphi_1=\varphi \circ \psi$.

Si l’homomorphisme de groupes$\psi : \Gamma '_1\rightarrow \Gamma '$ convient, alors il vérifie les relations

$$
\psi (\gamma ) = (\varphi \circ \psi (\gamma ), \pi '\circ \psi (\gamma )) = (\varphi_1(\gamma ), \pi_1'(\gamma ))
$$

pour tout $\gamma \in \Gamma '_1$. Inversement, l’homomorphisme de groupes de $\Gamma '_1$ dans $\Gamma \times G'$ défini par $\gamma \rightarrow (\varphi_1(\gamma ), \pi '_1(\gamma ))$ est à valeurs dans le produit fibré $\Gamma \times_GG'$ puisque $\pi \circ \varphi_1(\gamma ) =u\circ \pi_1'(\gamma )$ pour tout $\gamma \in \Gamma '_1$.

#### Corollaire 1 {#alg-viii-s16-lem-2-cor-1 .statement tag=00IE}

Soient $\mathscr{E}_1$ et $\mathscr{E}_2$ des $\tau$-extensions de G par F et soit $\psi$ un morphisme de $\tau$-extensions de $\mathscr{E}_1$ dans $\mathscr{E}_2$. Notons $\varphi_1$ (resp. $\varphi_2)$l’homomorphisme canonique pour $u^*(\mathscr{E}_1)$ (resp. $u^*(\mathscr{E}_2))$. Alors il existe un unique morphisme de $\tau '$-extensions de $u^*(\mathscr{E}_1)$dans $u^*(\mathscr{E}_2)$, noté $u^*(\psi )$, tel que $\varphi_2\circ u^*(\psi ) =\psi \circ \varphi_1$.

Il suffit d’appliquer la prop. 1 à $\psi \circ \varphi_1$.

La classe de la $\tau '$-extension $u^*(\mathscr{E})$ ne dépend donc que de la classe de $\mathscr{E}$. On note également $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G',F)$ l’application qui envoie la classe d’une $\tau$-extension $\mathscr{E}$ sur la classe de la $\tau '$-extension $u^*(\mathscr{E})$.

#### Corollaire 2 {#alg-viii-s16-lem-2-cor-2 .statement tag=00IF}

Soit $u': G''\rightarrow G'$ un homomorphisme de groupes et soit $\mathscr{E}$ une $\tau$-extension de G par F. Posons $\tau ''=\tau '\circ u'$ et notons $\varphi$ (resp. $\varphi ',\varphi '')$l’homomorphisme canonique associé à la $\tau '$-extension $u^*(\mathscr{E})$ (resp. la $\tau ''$-extension $u^{'*}(u^*(\mathscr{E}))$, la $\tau ''$-extension $(u\circ u')^*(\mathscr{E}))$. Alors il existe un unique morphisme $\psi$ de la $\tau ''$-extension $u^{'*}(u^*(\mathscr{E}))$dans la $\tau ''$-extension $(u\circ u')^*(\mathscr{E})$telle que $\varphi ''\circ \psi =\varphi \circ \varphi '$.

#### Exemple {#alg-viii-s16-n2-exa-1 .statement tag=00RI}

Soit H un sous-groupe de G et $j: H\rightarrow G$ l’injection canonique. Alors pour toute $\tau$-extension $\mathscr{E}= (\Gamma , \iota , \pi )$, la $\tau \circ j$-extension $j^*(\mathscr{E})$ est isomorphe à $(^-\pi^1(H), \iota ', \pi ')$ où $\iota ': F\rightarrow^-\pi^1(H)$ (resp. $\pi ':^-\pi^1(H)\rightarrow H)$ est l’homomorphisme de groupes $f\rightarrow \iota (f)$ (resp. $\gamma \rightarrow \pi (\gamma ))$. Plus généralement, si l’homomorphisme de groupes $u: G'\rightarrow G$ est injectif, alors l’homomorphisme canonique $\varphi$ est injectif d’image $^-\pi^1(u(G'))$.

### 3. Image directe d’une $\tau$-extension

Soit G un groupe, soient F et $F'$ des groupes abéliens, soit $\tau$ (resp. $\tau ')$ un homomorphisme de groupes de G dans le groupe des automorphismes de F (resp. $F')$ et soit $v: F\rightarrow F'$ un homomorphisme de groupes tel que

$$
v(\tau (g).f) =\tau '(g).v(f) \tag{3}
$$

pour $g\in G$ et $f\in F$. Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension de G par F. Soit $\widetilde{\Gamma}$ le produit semi-direct externe $F'\times_{\tau'\circ\pi}\Gamma$. On note $\widetilde{\imath}: F'\rightarrow \widetilde{\Gamma}$ l’homomorphisme $f\rightarrow (f, e)$ et $\widetilde{p}:\widetilde{\Gamma}\rightarrow \Gamma$ la première projection. Soit $j: F\rightarrow \widetilde{\Gamma}$ l’application définie par $f\rightarrow (v(f), \iota (f)^{-1})$. Comme l’image de $\iota$ est contenue dans le noyau de $\tau '\circ \pi$, l’application $j$ est un homomorphisme de groupes ; il est injectif puisque $\iota$ est injectif. On a les relations

$$
(f', \gamma )j(f)(f', \gamma )^{-1}= (f', \gamma )(v(f), \iota (f)^{-1})(f', \gamma )^{-1}
$$

$$
= (\tau '(\pi (\gamma )).v(f), \iota (\tau (\pi (\gamma )).f)^{-1}) \tag{4}
$$

$$
=j(\tau (\pi (\gamma )).f)
$$

pour tout $f\in F$, tout $\gamma \in \Gamma$ et tout $f'\in F'$. Par conséquent, l’image de $j$ est un sous-groupe distingué dans $\widetilde{\Gamma}$. Notons $\Gamma '$ le quotient de $\widetilde{\Gamma}$ par l’image de $j$. On note $\iota '$ la composée de la surjection canonique de $\widetilde{\Gamma}$ dans $\Gamma '$ et de $\widetilde{\imath}$. Le noyau de l’homomorphisme $\pi \circ \widetilde{p}$ est le produit $F'\times \iota (F)$ qui contient l’image de $j$. On définit $\pi ': \Gamma '\rightarrow G$ comme l’homomorphisme de groupes déduit de $\pi \circ \widetilde{p}$ par passage au quotient. Comme $\iota$ est injective, l’intersection de $j(F)$ avec $\widetilde{\imath}(F')$ est réduite à l’élément neutre de $\widetilde{\Gamma}$; il en résulte que $\iota '$ est injective. L’application de $F'\times F$ dans $F'\times \iota (F) =$ Ker($\pi \circ \widetilde{p}$) donnée par

$$
(f', f)\longrightarrow (f'v(f), \iota (f)^{-1})
$$

est un isomorphisme de groupes. L’image de $\iota '$ coïncide donc avec le noyau de $\pi '$. Comme $\pi$ et $\widetilde{p}$ sont surjectifs, il en est de même de $\pi '$. Ceci démontre que $\mathscr{E}'=$ $(\Gamma ', \iota , \pi ')$ est une $\tau '$-extension de G par $F'$ qu’on appelle l’image directe de $\mathscr{E}$ par $v$ et qu’on note $v_*(\mathscr{E})$. La composée de la surjection canonique de $\widetilde{\Gamma}$ dans $\Gamma '$ et de l’homomorphisme de groupes de Γ dans $\widetilde{\Gamma}$, donné par $\gamma \rightarrow (1, \gamma )$ est un homomorphisme de groupes $\varphi : \Gamma \rightarrow \Gamma '$ qui est dit canonique.

#### Proposition 2 {#alg-viii-s16-prop-2 .statement tag=00IG}

Avec les notations qui précèdent, le diagramme

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{5}
$$

$F'^{\iota'}$ // $\Gamma '^{\pi'}$ // G

est commutatif. Soit $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$une $\tau '$-extension de G par $F'$ et soit $\varphi_1: \Gamma \rightarrow \Gamma '_1$ un homomorphisme de groupes tel que le diagramme

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1$

$F'^{\iota'_1}$ // $\Gamma '_1^{\pi'_1}$ // G

soit commutatif, alors il existe un unique morphisme $\psi$ de $\tau '$-extensions de $v_*(\mathscr{E})$ dans $\mathscr{E}_1'$ tel qu’on ait $\varphi_1=\psi \circ \varphi$.

La commutativité du premier diagramme résulte des constructions. L’existence et l’unicité de $\psi$ découlent du lemme qui suit.

#### Lemme 3 {#alg-viii-s16-lem-3 .statement tag=00IH}

Soit $G'_1$ un groupe et soient $w: G\rightarrow G'_1$ et $\tau_1: G'_1\rightarrow$ Aut(F$')$des homomorphismes de groupes tels que $\tau '=\tau_1\circ w$. Soit $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$une $\tau_1$-extension de $G'_1$ par $F'$ et soit $\varphi_1: \Gamma \rightarrow \Gamma '_1$ un homomorphisme de groupes tel que le diagramme

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1w$

$F'^{\iota'_1}$ // $\Gamma '_1^{\pi'_1}/$/ $G'_1$

soit commutatif. Alors il existe un unique homomorphisme de groupes $\psi : \Gamma '\rightarrow \Gamma '_1$ tel que le diagramme

$F'^{\iota'}$ // $\Gamma '^{\pi'}$ // G

$\psi w$

$F'^{\iota'_1}$ // $\Gamma '_1^{\pi'_1}/$/ $G'_1$ soit commutatif et tel que $\varphi_1=\psi \circ \varphi$.

Pour tout $(f, \gamma )\in F'\times \Gamma$, notons $(f, \gamma )$ la classe de $(f, \gamma )$ dans $\Gamma '$. Si l’homomorphisme de groupes $\psi : \Gamma '\rightarrow \Gamma '_1$ convient, il vérifie les relations

$$
\psi ((f', \gamma ))=\psi (\iota '(f')\varphi (\gamma )) =\iota '_1(f')\varphi_1(\gamma )
$$

pour tout $f'\in F'$ et tout $\gamma \in \Gamma$. Inversement, l’application $\widetilde{\psi}$ de $F'\times_{\tau'\circ\pi}\Gamma$ dans $\Gamma '_1$ donnée par $(f, \gamma )\rightarrow \iota '_1(f)\varphi_1(\gamma )$ est un homomorphisme de groupes. En effet, on a les relations

$$
\iota '_1(f)\varphi_1(\gamma )\iota '_1(f')\varphi_1(\gamma ') =\iota '_1(f \tau_1(\pi_1'(\varphi_1(\gamma ))).f')\varphi_1(\gamma \gamma ') =\iota '_1(f \tau '(\pi (\gamma )).f')\varphi_1(\gamma \gamma ')
$$

pour $f, f'\in F'$ et $\gamma , \gamma '\in \Gamma$. Le noyau de $\widetilde{\psi}$ contient l’image de $j$ puisque $\iota '_1(v(f)) =$ $\varphi_1(\iota (f))$ pour $f\in F$ et le morphisme $\psi$ déduit de $\widetilde{\psi}$ par passage au quotient convient.

#### Remarque {#alg-viii-s16-n3-rem-1 .statement tag=00II}

Notons Σ l’espèce de structure de $\tau '$-extension et définissons les $\alpha$-applications comme les applications de Γ dans un groupe $\Gamma '$ sous-jacent à une $\tau '$-extension qui sont des homomorphismes de groupes et qui rendent le diagramme

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{6}
$$

$F'^{\iota'}$ // $\Gamma '^{\pi'}$ // G

commutatif. La prop. 2 exprime que $v_*(\mathscr{E})$ est une solution du problème d’application universelle correspondant (E, IV, p. 22).

#### Corollaire 1 {#alg-viii-s16-lem-3-cor-1 .statement tag=00IJ}

Soient $\mathscr{E}_1$ et $\mathscr{E}_2$ des $\tau$-extensions de G par F et soit $\psi$ un morphisme de $\tau$-extensions de $\mathscr{E}_1$ dans $\mathscr{E}_2$. Notons $\varphi_1$ (resp. $\varphi_2)$l’homomorphisme canonique pour $v_*(\mathscr{E}_1)$ (resp. $v_*(\mathscr{E}_2))$. Alors il existe un unique morphisme de $\tau '$-extensions de $v_*(\mathscr{E}_1)$dans $v_*(\mathscr{E}_2)$, noté $v_*(\psi )$, tel que $\varphi_2\circ \psi =v_*(\psi )\circ \varphi_1$.

Il suffit d’appliquer la prop. 2 à $\varphi_2\circ \psi$.

La classe de la $\tau '$-extension $v_*(\mathscr{E})$ ne dépend donc que de la classe de $\mathscr{E}$. On note également $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ l’application qui envoie la classe d’une $\tau$-extension $\mathscr{E}$ sur la classe de la $\tau '$-extension $v_*(\mathscr{E})$.

#### Corollaire 2 {#alg-viii-s16-lem-3-cor-2 .statement tag=00RJ}

On conserve les notations de la proposition. Soit $F''$ un groupe abélien et soient $\tau '': G\rightarrow$ Aut(F$'')$et $v': F'\rightarrow F''$ des homomorphismes de groupes tels que

$$
\tau ''(g).v'(f) =v'(\tau '(g).f)
$$

pour $g\in G$et $f\in F'$. Soit $\mathscr{E}$ une $\tau$-extension de G par F et notons $\varphi$ (resp. $\varphi ',\varphi '')$ l’homomorphisme canonique associé à $v_*(\mathscr{E})$ (resp. $v'_*(v_*(\mathscr{E}))$, $(v'\circ v)_*(\mathscr{E}))$. Alors il existe un unique morphisme $\psi$ de la $\tau ''$-extension $v_*'(v_*(\mathscr{E}))$de G par $F''$ dans la $\tau ''$-extension $(v'\circ v)_*(\mathscr{E})$tel que $\varphi ''=\psi \circ \varphi '\circ \varphi$.

#### Exemple 1 {#alg-viii-s16-n3-exa-1 .statement tag=00IK}

Soit $j:\{1\} \rightarrow F$ l’injection canonique. L’extension semi-triviale $\mathscr{I}_{\tau}$ est isomorphe à $j_*((G, i$,Id$_G))$ où $i:\{e\} \rightarrow G$ est l’injection canonique. Soit $c: F\rightarrow F$ l’homomorphisme constant $f\rightarrow 1$ et soit $\mathscr{E}$ une $\tau$-extension. La $\tau$-extension $c_*(\mathscr{E})$ est également isomorphe à $\mathscr{I}_{\tau}$.

#### Exemple 2 {#alg-viii-s16-n3-exa-2 .statement tag=00IL}

Soit E un sous-groupe de F stable pour l’action de G. Notons $F'$ le quotient de F par $E,v: F\rightarrow F'$ l’homomorphisme canonique et $\tau ': G\rightarrow$ Aut(F$')$ l’action de G sur $F'$ caractérisée par

$$
\tau '(g).v(f) =v(\tau (g).f)
$$

pour $g\in G$ et $f\in F$. Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension de G par F. Alors $\iota (E)$ est un sous-groupe distingué de Γ et la $\tau '$-extension $v_*(\mathscr{E})$ de G par $F'$ est isomorphe à l’extension $(\Gamma /\iota (E), \iota , \pi )$ où $\iota$ et $\pi$ sont les homomorphismes de groupes déduits de $\iota$ et $\pi$ par passages aux quotients. L’homomorphisme canonique $\varphi$ associé à $v_*(\mathscr{E})$ correspond par cet isomorphisme à l’homomorphisme canonique de Γ dans $\Gamma /\iota (E)$.

#### Proposition 3 {#alg-viii-s16-prop-3 .statement tag=00IM}

Soient G et $G'$ des groupes. Soient F et $F'$ des groupes abéliens. Soient $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'),u: G'\rightarrow G$et $v: F\rightarrow F'$ des homomorphismes de groupes tels que

$$
\tau '(g).v(f) =v(\tau (g).f)
$$

pour $g\in G$et $f\in F$. On note $\tau ''=\tau '\circ u$. Soit $\mathscr{E}$ une $\tau$-extension de G par F. On note $\varphi_u$ (resp. $\varphi_v,\varphi '_u,\varphi '_v)$l’homomorphisme canonique correspondant à la $\tau \circ u$-extension $u^*(\mathscr{E})$ (resp. à la $\tau '$-extension $v_*(\mathscr{E})$, aux $\tau ''$-extensions $u^*(v_*(\mathscr{E}))$et $v_*(u^*(\mathscr{E})))$. Alors il existe un unique morphisme $\psi$ de $\tau ''$-extensions de $v_*(u^*(\mathscr{E}))$dans $u^*(v_*(\mathscr{E}))$ tel que $\varphi_v\circ \varphi_u=\varphi '_u\circ \psi \circ \varphi '_v$.

On note $(\Gamma_u, \iota_u, \pi_u)$ (resp. $(\Gamma '_u, \iota '_u, \pi_u'))$ la $\tau \circ u$-extension $u^*(\mathscr{E})$ (resp. la $\tau ''$-extension $u^*(v_*(\mathscr{E})))$. En appliquant le lemme 2 de VIII, p. 283 à $\varphi_v\circ \varphi_u$, on obtient qu’il existe un homomorphisme de groupes $\psi_1: \Gamma_u\rightarrow \Gamma '_u$ tel que le diagramme

F $^{\iota_u}$ // $\Gamma_u^{\pi_u}$ // $G'$

$v\psi_1$

$F'^{\iota'_u}$ // $\Gamma '_u^{\pi'_u}$ // $G'$

soit commutatif et tel que $\varphi '_u\circ \psi_1=\varphi_v\circ \varphi_u$. L’existence de $\psi$ s’en déduit à l’aide de la proposition 2 appliquée à $\psi_1$. Inversement, si $\psi '$ convient également, on a $\psi '\circ \varphi '_v=\psi_1$ par le lemme 2, donc $\psi '=\psi$ (prop. 2).

### 4. Loi de groupe sur les classes de $\tau$-extensions

Soit G un groupe, soit F un groupe abélien et soit $\tau : G\rightarrow$ Aut(F) un homomorphisme de groupes. On désigne par $\delta : G\rightarrow G\times G$ l’application diagonale $g\rightarrow (g, g)$ et par $m: F\times F\rightarrow F$ l’homomorphisme de multiplication $(f_1, f_2)\rightarrow f_1f_2$. On note $s: F\rightarrow F$ l’homomorphisme de groupes donné par $f\rightarrow f^{-1}$. Soient $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ et $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ des $\tau$-extensions de G par F. Comme on a la relation

$$
m(((\tau \times \tau )\circ \delta )(g).(f_1, f_2)) =\tau (g).m(f_1, f_2)
$$

pour tout $g\in G$ et tous $f_1, f_2\in F$, l’extension $m_*(\delta^*(\mathscr{E}_1\times \mathscr{E}_2))$ est une $\tau$-extension qu’on appelle le produit des $\tau$-extensions $\mathscr{E}_1$ et $\mathscr{E}_2$ et qu’on note $\mathscr{E}_1\mathscr{E}_2$. La classe de cette extension ne dépend que des classes des extensions $\mathscr{E}_1$ et $\mathscr{E}_2$ (VIII, p. 284, cor. 1 et VIII, p. 287, cor. 1). On en déduit donc une loi de composition sur Ex$_{\tau}(G,F)$.

#### Remarque {#alg-viii-s16-n4-rem-1 .statement tag=00IN}

Soient $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ et $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ des $\tau$-extensions de G par F. Soit $\mathscr{E}_1\mathscr{E}_2= (\Gamma , \iota , \pi )$ le produit de ces extensions. Compte tenu de l’exemple de VIII, p. 284, la construction fournit un homomorphisme de groupes surjectif du produit fibré $\Gamma_1\times_G\Gamma_2$ dans Γ dont le noyau est l’image de l’homomorphisme de groupes $f\rightarrow (\iota_1(f), \iota_2(f)^{-1})$ de F dans $\Gamma_1\times_G\Gamma_2$.

#### Proposition 4 {#alg-viii-s16-prop-4 .statement tag=00IO}

Le produit des $\tau$-extensions munit l’ensemble Ex$_{\tau}(G,F)$d’une structure de groupe abélien. Son élément neutre est la classe de l’extension semi-triviale $\mathscr{I}_{\tau}$. L’inverse de la classe d’une $\tau$-extension $\mathscr{E}$ est la classe de $s_*(\mathscr{E})$.

L’associativité de la loi résulte de la commutativité des diagrammes

G $^{\delta}$ // $G\times GF\times F\times F^{m\times Id}/$/ $F\times F$

$\delta$ Id$\times \delta$ et Id$\times mm$

$G\times G^{\delta\times Id}/$/ $G\times G\times GF\times F^m$ // $F$,

du cor. 2 de VIII, p. 284, du cor. 2 de VIII, p. 287 et de la prop. 3 de VIII, p. 288.

Soit $\Delta  : F\rightarrow F\times F$ l’application diagonale $f\rightarrow (f, f)$. Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension. Soit $\widetilde{\Delta} : \Gamma \rightarrow \Gamma \times_G\Gamma$ l’homomorphisme de groupes donné par $\gamma \rightarrow (\gamma , \gamma )$. Le diagramme

F $^{\iota}$ // Γ $^{\pi}$ // G

Δ $\widetilde{\Delta}$

$F\times F$ // $\Gamma \times_G\Gamma$ // G

est commutatif. D’après la prop. 2 de VIII, p. 286, il en résulte que la $(\tau \times \tau )\circ \delta$-extension $\delta^*(\mathscr{E}\times \mathscr{E})$ est isomorphe à $\Delta_*(\mathscr{E})$.

Notons $c$ : F $\rightarrow$ F l’homomorphisme constant $f\rightarrow$ 1. Compte tenu de l’exemple 1 de VIII, p. 288, le fait que $\mathscr{I}_{\tau}$ soit un élément neutre pour cette loi de composition résulte de l’isomorphisme de $\delta^*(\mathscr{E}\times \mathscr{E})$ sur $\Delta_*(\mathscr{E})$ et du diagramme commutatif

F $M^{(Id}M$M$M^{^F}M^{\times}M^{c)\circ\Delta}/$/ $F\times F$

$_{\times\circ}M^{Id}MM^{^F}$ $^{(cId_F)\Delta}$ MMM $^m$

$F\times F^m$ M//&& $F$.

La dernière assertion résulte du diagramme commutatif

F $M^{(Id}M$M$M^{^F}M^{\times}M^{s)\circ\Delta}/$/ $F\times F$

$_{(s\times Id)\circ\Delta}$ M$M^cM$

$^{^F}$ MMM $^m$

$F\times F^m$ M//&& $F$.

Soient $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ et $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ des $\tau$-extensions. L’isomorphisme de groupes $\Gamma_1\times \Gamma_2\rightarrow \Gamma_2\times \Gamma_1$ donné par $(\gamma_1, \gamma_2)\rightarrow (\gamma_2, \gamma_1)$ induit par passage aux sous-ensembles un isomorphisme de groupes $\sigma : \Gamma_1\times_G\Gamma_2\rightarrow \Gamma_2\times_G\Gamma_1$. Compte tenu des relations

$$
\sigma (\iota_1(f), \iota_2(f)^{-1}) = (\iota_2(f^{-1}), \iota_1(f^{-1})^{-1})
$$

pour $f\in F$, l’homomorphisme de groupes $\sigma$ induit par passage aux quotients un morphisme de $\tau$-extensions de $\mathscr{E}_1\mathscr{E}_2$ sur $\mathscr{E}_2\mathscr{E}_1$. Donc la loi de composition est commutative.

#### Proposition 5 {#alg-viii-s16-prop-5 .statement tag=00IP}

a) Soient G et $G'$ des groupes. Soit F un groupe abélien. Soient $\tau : G\rightarrow$ Aut(F) et $u: G'\rightarrow G$des homomorphismes de groupes. L’application $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau\circ u}(G',F)$est un homomorphisme de groupes.

b) Soit G un groupe. Soient F et $F'$ des groupes abéliens. Soient $\tau : G\rightarrow$ Aut(F), $\tau ': G\rightarrow$ Aut(F$')$et $v: F\rightarrow F'$ des homomorphismes de groupes tels que

$$
\tau '(g).v(f) =v(\tau (g).f)
$$

pour $g\in G$et $f\in F$. L’application $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$est un homomorphisme de groupes.

Cela résulte de la commutativité des diagrammes

$G'^{\delta}$ // $G'\times G'F\times F^m$ // F

$_uu_{\times u}$ et $v_{\times v}v$

G $^{\delta}$ // $G\times GF'\times F'^m$ // $F'$.

### 5. Description cohomologique

Soit G un groupe, soit F un groupe abélien et soit $\tau : G\rightarrow$ Aut(F) un homomorphisme de groupes. Pour tout $g\in G$ et tout $f\in F$ on note également $^gf$ pour $\tau (g).f$. Un 2-cocycle de G à valeurs dans F est une application $c: G\times G\rightarrow F$ telle que pour tout $(g_1, g_2, g_3)\in G\times G\times G$, on ait

$$
g_{_1}c(g_2, g_3)c(g_1, g_2g_3) =c(g_1, g_2)c(g_1g_2, g_3) \tag{7}
$$

Comme F est commutatif, l’ensemble des 2-cocycles est un sous-groupe du groupe des applications de $G\times G$ dans F, on le note $Z^2(G,F)$. Notons $C^1(G,F)$ le groupe des applications de G dans F. Pour tout $h\in C^1(G,F)$ et tout $(g_1, g_2)\in G\times G$, posons

$$
(\partial h)(g_1, g_2) =^{g_1}h(g_2)h(g_1g_2)^{-1}h(g_1) \tag{8}
$$

Un calcul simple démontre que l’application $\partial h: G\times G\rightarrow F$ est un 2-cocycle. L’application $\partial : C^1(G,F)\rightarrow Z^2(G,F)$ est un homomorphisme de groupes. Pour tout $h\in C^1(G,F)$, le 2-cocycle $\partial h$ est appelé un 2-cobord. Le groupe $Z^2(G,F)/\partial (C^1(G,F))$ est noté $H^2(G,F)$ et est appelé le deuxième groupe de cohomologie de G à coefficients dans F.

$*$Les notations qui précèdent sont conforme à celles de X, p. 112 concernant la cohomologie des groupes. $*$

Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension. Soit $\sigma$ une section de l’application surjective $\pi (E$ II, p. 18), c’est-à-dire une application de G dans Γ telle que $\pi (\sigma (g)) =g$ pour tout $g$ dans G. On appelle 2-cocycle associé à $\sigma$, l’application $c_{\sigma}: G\times G\rightarrow F$ définie par la formule

$$
\iota (c_{\sigma}(g_1, g_2)) =\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1} \tag{9}
$$

pour $g_1, g_2\in G$. L’application $c_{\sigma}$ est constante de valeur 1 si et seulement si $\sigma$ est un homomorphisme de groupes.

#### Proposition 6 {#alg-viii-s16-prop-6 .statement tag=00IQ}

L’application $c_{\sigma}$ est un élément du groupe $Z^2(G,F)$et sa classe dans le groupe de cohomologie $H^2(G,F)$ne dépend que de la classe de la $\tau$-extension $\mathscr{E}$. On l’appelle la classe de cohomologie de la $\tau$-extension $\mathscr{E}$.

Vérifions tout d’abord que $c_{\sigma}$ satisfait à la condition de cocycle. Soient $g_1,g_2$ et $g_3$ des éléments de G. En utilisant la relation (1) de VIII, p. 281 et (9), on obtient les relations

$$
\iota (^{g_1}c_{\sigma}(g_2, g_3)c_{\sigma}(g_1, g_2g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_2g_3)^{-1}\sigma (g_1)^{-1}\sigma (g_1)\sigma (g_2g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

et

$$
\iota (c_{\sigma}(g_1, g_2)c_{\sigma}(g_1g_2, g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}\sigma (g_1g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

L’application $c_{\sigma}$ est donc un élément de $Z^2(G,F)$.

Démontrons maintenant que l’image de $c_{\sigma}$ dans $H^2(G,F)$ est indépendante de la section $\sigma$ choisie. Soient $\sigma$ et $\sigma '$ de telles sections. Pour tout élément $g$ de G, il existe un unique élément $a_g$ de F tel que $\sigma '(g) =\iota (a_g)\sigma (g)$. Soient $g_1$ et $g_2$ des éléments de G. En utilisant la définition (9) on obtient les égalités suivantes :

$$
\iota (c_{\sigma'}(g_1, g_2)) =\sigma '(g_1)\sigma '(g_2)\sigma '(g_1g_2)^{-1}
$$

$$
=\iota (a_{g_1})\sigma (g_1)\iota (a_{g_2})\sigma (g_2)\sigma (g_1g_2)^{-1}\iota (a_{g_1g_2})^{-1} \tag{10}
$$

$$
=\iota (a_{g_1})\iota (^{g_1}a_{g_2})\iota (c_{\sigma}(g_1, g_2))\iota (a_{g_1g_2})^{-1}
$$

Le groupe F étant commutatif, on a les relations

$$
c_{\sigma'}(g_1, g_2)c_{\sigma}(g_1, g_2)^{-1}= (^{g_1}a_{g_2})a^{-1}_{g_1g_2}a_{g_1} \tag{11}
$$

et les classes de $c_{\sigma'}$ et $c_{\sigma}$ dans $H^2(G,F)$ coïncident.

Enfin, soient $\mathscr{E}= (\Gamma , \iota , \pi )$ et $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ des $\tau$-extensions isomorphes, soit $u:\mathscr{E}\rightarrow \mathscr{E}'$ un morphisme de $\tau$-extensions et soit $\sigma$ une section de l’application $\pi$. L’application $u\circ \sigma$ est une section de l’application $\pi '$ et l’on a $c_{\sigma}=c_{u\circ\sigma}$. La classe de $c_{\sigma}$ dans $H^2(G,F)$ ne dépend donc que de la classe de $\mathscr{E}$ dans Ex$_{\tau}(G,F)$.

On note $\Theta_{\tau}:$ Ex$_{\tau}(G,F)\rightarrow H^2(G,F)$ ou, plus simplement, Θ l’application qui envoie la classe d’une $\tau$-extension $(\Gamma , \iota , \pi )$ sur la classe du 2-cocycle $c_{\sigma}$, où $\sigma$ est une section de la surjection $\pi$.

#### Théorème 1 {#alg-viii-s16-thm-1 .statement tag=00IR}

L’application Θ est un isomorphisme de groupes de Ex$_{\tau}(G,F)$sur $H^2(G,F)$.

Démontrons tout d’abord que Θ est un homomorphisme de groupes. Soient $\mathscr{E}= (\Gamma , \iota , \pi )$ et $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ des $\tau$-extensions et soit $\sigma$ (resp. $\sigma ')$ une section de l’application $\pi$ (resp. $\pi ')$. Notons $\mathscr{E} \mathscr{E}'= (\Gamma '', \iota '', \pi '')$ le produit des $\tau$-extensions $\mathscr{E}$ et $\mathscr{E}'$. On notera $[\gamma , \gamma ']$ l’image dans $\Gamma ''$ d’un élément $(\gamma , \gamma ')$ de $\Gamma \times_G\Gamma '$ par l’homomorphisme surjectif de la remarque de VIII, p. 289. L’application de G dans $\Gamma ''$ qui envoie un élément $g$ sur $[\sigma (g), \sigma '(g)]$ est une section $\sigma ''$ de l’application $\pi ''$. Soient $g_1$ et $g_2$ des éléments de G. On a les relations

$$
\iota ''(c_{\sigma''}(g_1, g_2)) =\sigma ''(g_1)\sigma ''(g_2)\sigma ''(g_1g_2)^{-1}
$$

$$
= [\iota (c_{\sigma}(g_1, g_2)), \iota '(c_{\sigma'}(g_1, g_2)]
$$

$$
=\iota ''(c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2))
$$

On a donc $c_{\sigma''}(g_1, g_2) =c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2)$.

Démontrons que l’application Θ est injective. Soit donc $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension et soit $\sigma$ une section de l’application $\pi$ telle que l’image de $c_{\sigma}$ dans $H^2(G,F)$ soit triviale. Il existe donc une application $a: G\rightarrow F$ telle que

$$
c_{\sigma}(g_1, g_2) = (^{g_1}a(g_2))a(g_1g_2)^{-1}a(g_1)
$$

pour tous $g_1, g_2\in G$. On définit alors $\sigma ': G\rightarrow \Gamma$ par

$$
\sigma '(g) =\iota (a(g)^{-1})\sigma (g)
$$

pour $g\in G$. En utilisant (11), on obtient que $c_{\sigma'}$ est constante de valeur 1 ; par conséquent, $\sigma '$ est un homomorphisme de groupes ce qui prouve que la $\tau$-extension $\mathscr{E}$ est semi-triviale (I, p. 64, prop. 4).

Démontrons que l’application Θ est surjective. Soit $c$ un élément de $Z^2(G,F)$. On munit l’ensemble $\Gamma  = F\times G$ de la loi de composition suivante :

$$
(f_1, g_1)(f_2, g_2) = (f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2) \tag{12}
$$

pour tous $f_1, f_2\in F$ et tous $g_1, g_2\in G$; on a les relations

$$
(f_1, g_1)((f_2, g_2)(f_3, g_3)) = (f_1, g_1)(f_2(^{g_2}f_3)c(g_2, g_3), g_2g_3)
$$

$$
= (f_1(^{g_1}f_2)(^{g_1g_2}f_3)(^{g_1}c(g_2, g_3))c(g_1, g_2g_3), g_1g_2g_3)
$$

et

$$
((f_1, g_1)(f_2, g_2))(f_3, g_3) = (f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)(f_3, g_3)
$$

$$
= (f_1(^{g_1}f_2)(^{g_1g_2}f_3)c(g_1, g_2)c(g_1g_2, g_3), g_1g_2g_3)
$$

pour tous $f_1, f_2, f_3\in F$ et tous $g_1,g_2, g_3\in G$. Il en résulte que cette loi est associative car $c_{\sigma}$ est un 2-cocycle. Pour tout $(f, g)\in \Gamma$, on a

$$
(f, g)(c(e, e)^{-1}, e) = (f(^gc(e, e)^{-1})c(g, e), g)
$$

or il résulte de la définition d’un 2-cocycle que $c(g, e) =^gc(e, e)$, d’où l’on déduit que $(f, g)(c(e, e)^{-1}, e) = (f, g)$. De manière analogue on démontre que

$$
(c(e, e)^{-1}, e)(f, g) = (f c(e, e)^{-1}c(e, g), g) = (f, g)
$$

La loi de composition définie par (12) admet donc $(c(e, e)^{-1}, e)$ comme élément neutre et tout élément $(f, g)$ de Γ est inversible, d’inverse

$$
(^{g^{-1}}(f^{-1}c(e, e)^{-1}c(g, g^{-1})^{-1}), g^{-1})
$$

On a donc muni Γ d’une structure de groupe. Notons alors $\iota : F\rightarrow G$ l’application envoyant $f$ sur $(c(e, e)^{-1}f, e),\pi : \Gamma \rightarrow G$ la deuxième projection et $\sigma$ l’application $g\rightarrow (1, g)$. Les applications $\iota$ et $\pi$ sont des homomorphismes de groupes, le triplet $\mathscr{E}= (\Gamma , \iota , \pi )$ est alors une $\tau$-extension, $\sigma$ une section de l’application $\pi$ et le cocycle associé $c_{\sigma}$ est égal à $c$, car

$$
\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}= (1, g_1)(1, g_2)(1, g_1g_2)^{-1}= (c(g_1, g_2), g_1g_2)(1, g_1g_2)^{-1}
$$

$$
= (c(g_1, g_2)c(e, g_1g_2)^{-1}, e) = (c(e, e)^{-1}c(g_1, g_2), e)
$$

pour $g_1, g_2\in G$.

#### Remarque {#alg-viii-s16-n5-rem-1 .statement tag=00RK}

Soit G un groupe, soient F et $F'$ des groupes abéliens, soit $\tau$ (resp. $\tau ')$ un homomorphisme de groupes de G dans le groupe des automorphismes de F (resp. $F')$ et soit $v: F\rightarrow F'$ un morphisme de groupes tel que

$$
v(\tau (g).f) =\tau '(g).v(f) \tag{13}
$$

pour $g\in G$ et $f\in F$. Soit $\alpha$ un élément de Ex$_{\tau}(G,F)$. Si le cocycle $c$ représente $\Theta (\alpha )$, alors $v\circ c$ représente $\Theta (v_*(\alpha ))\in H^2(G,F')$.

### 6. Restriction et corestriction

Soient G et $G'$ des groupes, soit F un groupe abélien et soit $\tau$ un homomorphisme de G dans le groupe des automorphismes du groupe F. Soit $u: G'\rightarrow G$ un homomorphisme de groupes. On note $\tau '=\tau \circ u$.

Si $\psi : G\times G\rightarrow F$ est un 2-cocycle de G à valeurs dans F, alors l’application $\psi \circ (u\times u)$ de $G'\times G'$ dans F donnée par $(g_1, g_2)\rightarrow \psi (u(g_1), u(g_2))$ est un 2cocycle de $G'$ à valeurs dans F et l’application $\psi \rightarrow \psi \circ (u\times u)$ de $Z^2(G,F)$ dans $Z^2(G',F)$ induit un homomorphisme de groupes $u^*: H^2(G,F)\rightarrow H^2(G',F)$. Pour tout $\lambda \in H^2(G,F)$, l’élément $u^*(\lambda )$ est appelé l’image inverse de $\lambda$ par $u$. Lorsque $G'$ est un sous-groupe de G et $u: G'\rightarrow G$ est l’injection canonique, l’homomorphisme $u^*$ est appelée l’homomorphisme de restriction de G à $G'$ et on le note Res$^G_{G'}$. Lorsque G est un quotient de $G'$ et $u: G'\rightarrow G$ est la surjection canonique, l’homomorphisme $u^*$ est appelée l’homomorphisme d’inflation de G à $G'$.

#### Proposition 7 {#alg-viii-s16-prop-7 .statement tag=00IS}

Avec les notations qui précèdent, le diagramme

Ex$_{\tau}(G,F)^{u^*}/$/ Ex$_{\tau}(G',F)$

$\Theta_{\tau}\Theta_{\tau'}$

$H^2(G,F)^{u^*}$ // $H^2(G',F)$

est commutatif.

Soit H un sous-groupe d’indice fini de G. Soit $s$ une section de la surjection canonique de G dans $H\backslash G$. On note $(g, x)\rightarrow x.g$ l’action à droite de G sur $H\backslash G$ induite par l’action à droite de G sur lui-même par multiplication. Notons que pour tout $x\in H\backslash G$ et tout $g\in G$, l’élément $s(x)gs(x.g)^{-1}$ appartient à H. Pour toute application $c: H\times H\rightarrow F$, on définit donc une application $\widetilde{c}_s: G\times G\rightarrow F$ par la relation

$$
\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

pour $g_1,g_2\in G$. L’application $c\rightarrow \widetilde{c}_s$ est un homomorphisme de groupes de $F^{H\times H}$ dans $F^{G\times G}$.

#### Lemme 4 {#alg-viii-s16-lem-4 .statement tag=00IT}

Si $c: H\times H\rightarrow F$est un 2-cocycle de H à valeurs dans F, alors $\widetilde{c}_s$ est un 2-cocycle de G à valeurs dans F.

Soient $g_1,g_2$ et $g_3$ des éléments de G. Pour tout $i\in  \{1,2,3\}$ on définit une application $h_i: H\backslash G\rightarrow H$ par la relation

$$
h_i(x) =s(x.g_1. . . g_{i-1})g_is(x.g_1. . . g_i)^{-1}
$$

pour $x\in H\backslash G$. Notons que

$h_1(x)h_2(x) =s(x)g_1g_2s(x.g_1g_2)^{-1}$ et $h_2(x)h_3(x) =s(x.g_1)g_2g_3s(x.g_1g_2g_3)^{-1}$ pour $x\in H\backslash G$. On a alors les relations

$$
^{g_1}\widetilde{c}_s(g_2, g_3)\widetilde{c}_s(g_1g_2, g_3)^{-1}\widetilde{c}_s(g_1, g_2g_3)\widetilde{c}_s(g_1, g_2)^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(s(x)g_2s(x.g_2)^{-1}, s(x.g_2)g_3s(x.g_2g_3)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h_1(x)h_2(x), h_3(x))^{-1}c(h_1(x), h_2(x)h_3(x))c(h_1(x), h_2(x))^{-1})
$$

$$
=\prod_{x\in H\backslash G}^{s(x.g_1^{-1})^{-1}h_1(x.g^-_1^1)}c(h_2(x.g_1^{-1}), h_3(x.g_1^{-1}))
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}h_1(x)}c(h_2(x), h_3(x))^{-1}
$$

$$
= 1
$$

où la deuxième égalité résulte du fait que $c$ est un 2-cocycle.

#### Lemme 5 {#alg-viii-s16-lem-5 .statement tag=00IU}

Si $c$ est un 2-cobord, alors il en est de même de $\widetilde{c}_s$.

Soit $t: H\rightarrow F$ une application telle que $c=\partial t$. Soient $\widetilde{t}_s: G\rightarrow F$ l’application définie par

$$
\widetilde{t}_s(g) =\prod_{x\in H\backslash G}^{s(x)^{-1}}t(s(x)gs(x.g)^{-1})
$$

pour $g\in G$. Il suffit de démontrer que $\widetilde{c}_s=\partial \widetilde{t}_s$, ce qui découle des relations

$$
\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}s(x)g_1s(x.g_1)^{-1}}t(s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(t(s(x)g_1g_2s(x.g_1g_2)^{-1})^{-1}t(s(x)g_1s(x.g_1)^{-1}))
$$

$$
=\partial \widetilde{t}_s(g_1, g_2)
$$

pour $g_1, g_2\in G$.

#### Lemme 6 {#alg-viii-s16-lem-6 .statement tag=00IV}

Soit $c$ un 2-cocycle de H à valeurs dans F. L’image de $\widetilde{c}_s$ dans le groupe $H^2(G,F)$ne dépend pas du choix de la section $s$.

Soit $s'$ une section de la surjection canonique de G dans $H\backslash G$. Soit $h: H\backslash G\rightarrow H$ l’application caractérisée par les relations

$$
s'(x) =h(x)s(x)
$$

pour $x\in H\backslash G$. Le 2-cocycle $\widetilde{c}_{s'}$ est alors donné par les relations

$$
\widetilde{c}_{s'}(g_1, g_2)
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}h(x)^{-1}}c(h(x)s(x)g_1s'(x.g_1)^{-1}, s'(x.g_1)g_2s'(x.g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}h(x.g_1)^{-1}, h(x.g_1)s(x.g_1)g_2s'(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h(x)^{-1}, s'(x)g_1g_2s'(x.g_1g_2)^{-1})^{-1}c(h(x)^{-1}, s'(x)g_1s'(x.g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}^{g_1s(x.g_1)^{-1}}c(h(x.g_1)^{-1}, h(x.g_1)s(x.g_1)g_2s'(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s'(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, h(x.g_1)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h(x)^{-1}, s'(x)g_1g_2s'(x.g_1g_2)^{-1})^{-1}c(h(x)^{-1}, s'(x)g_1s'(x.g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s'(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, h(x.g_1)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(h(x)^{-1}, h(x)s(x)g_2s'(x.g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h(x)^{-1}, s'(x)g_1g_2s'(x.g_1g_2)^{-1})^{-1}c(h(x)^{-1}, s'(x)g_1s'(x.g_1)^{-1}))
$$

pour tous $g_1, g_2\in G$; la première égalité provient de la relation de cocycle (VIII, p. 291, relation (7)) appliquée aux éléments

$h(x)^{-1},h(x)s(x)g_1s'(x.g_1)^{-1}$ et $s'(x.g_1)g_2s'(x.g_1g_2)^{-1}$,

la seconde est obtenue en appliquant la relation de cocycle aux éléments

$s(x)g_1s(x.g_1)^{-1},h(x.g_1)^{-1}$ et $h(x.g_1)s(x.g_1)g_2s'(x.g_1g_2)^{-1}$,

la dernière utilise simplement le fait que l’application $x\rightarrow x.g_1$ est une permutation de $H\backslash G$.

Les deux dernières lignes de l’expression obtenue correspondent à un 2-cobord. On obtient que $\widetilde{c}_{s'}$ a la même classe dans $H^2(G,F)$ que le cocycle dont la valeur en $(g_1, g_2)\in G^2$ est donnée par l’expression

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1}h(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, h(x.g_1)^{-1})^{-1}
$$

$=\prod_{x\in H\backslash G}^{g_1s(x.g_1)^{-1}}c(s(x.g_1)g_2s(x.g_1g_2)^{-1}, h(x.g_1g_2)^{-1})^{-1}$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x.g_1g_2)^{-1}, h(x.g_1g_2)^{-1})c(s(x)g_1s(x.g_1)^{-1}, h(x.g_1)^{-1})^{-1})
$$

$=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})$

$$
\times \prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(s(x)g_2s(x.g_2)^{-1}, h(x.g_2)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x.g_1g_2)^{-1}, h(x.g_1g_2)^{-1})c(s(x)g_1s(x.g_1)^{-1}, h(x.g_1)^{-1})^{-1})
$$

où la première égalité résulte de la relation de cocycle appliquée aux éléments

$s(x)g_1s(x.g_1)^{-1},s(x.g_1)g_2s(x.g_1g_2)^{-1}$ et $h(x.g_1g_2)^{-1}$

Les deux dernières lignes de l’expression obtenue correspondent à un 2-cobord. On obtient que la classe de $\widetilde{c}_{s'}$ coïncide avec celle de $\widetilde{c}_s$.

Nous avons construit un homomorphisme du groupe $H^2(H,F)$ dans le groupe $H^2(G,F)$, qu’on appelle l’homomorphisme de corestriction de H à G et qu’on note Cor$^G_H$.

#### Proposition 8 {#alg-viii-s16-prop-8 .statement tag=00IW}

Soit H un sous-groupe d’indice fini de G. L’endomorphisme Cor$^G_H\circ$ Res$^G_H$ du groupe $H^2(G,F)$coïncide avec la multiplication par l’indice (G : H).

Soit $\alpha$ un élément de $H^2(G,F)$. Soit $c$ un élément de $Z^2(G,F)$ représentant $\alpha$. L’élément Cor$^G_H\circ$ Res$^G_H(\alpha )$ est la classe du cocycle dont la valeur en $(g_1, g_2)\in G^2$ est donnée par l’expression

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}c(g_1s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x.g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x.g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(s(x.g_1)^{-1}, s(x.g_1)g_2s(x.g_1g_2)^{-1})
$$

$$
\times \prod c(g_1, g_2s(x.g_1g_2)^{-1})c(g_1, s(x.g_1)^{-1})^{-1}
$$

$$
\times \prod^x_x^{\in}_{\in}^H_H^{\backslash}_{\backslash}^G_G(c(s(x)^{-1}, s(x)g_1g_2s(x.g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x.g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}c(g_1, g_2s(x.g_1g_2)^{-1})c(g_1, s(x.g_1)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}^{g_1}c(s(x)^{-1}, s(x)g_2s(xg_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x.g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x.g_1)^{-1}))
$$

la première égalité provient de la relation de cocycle (VIII, p. 291, relation (7)) appliquée aux éléments

$s(x)^{-1},s(x)g_1s(x.g_1)^{-1}$ et $s(x.g_1)g_2s(x.g_1g_2)^{-1}$,

la seconde est obtenue en appliquant la relation de cocycle aux éléments

$g_1,s(x.g_1)^{-1}$ et $s(x.g_1)g_2s(x.g_1g_2)^{-1}$.

En ôtant un cobord, on obtient que Cor$^G_H\circ$ Res$^G_H(\alpha )$ est la classe du cocycle dont la valeur en $(g_1, g_2)\in G^2$ est donnée par l’expression

$$
\prod_{x\in H\backslash G}c(g_1, g_2s(x.g_1g_2)^{-1})c(g_1, s(x.g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x.g_1g_2)^{-1})^{-1}c(g_1g_2, s(x.g_1g_2)^{-1})c(g_1, g_2)
$$

$$
\times \prod_{x\in H\backslash G}c(g_1, s(x.g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x.g_2)^{-1})^{-1}c(g_1g_2, s(x.g_1g_2)^{-1})c(g_1, s(x.g_1)^{-1})^{-1}
$$

$$
\times c(g_1, g_2)^{(G:H)}
$$

ce qui démontre le résultat.

### 7. Algèbres galoisiennes

Soit K un corps commutatif. Si E est une K-algèbre, on note Aut$_K(E)$ le groupe de ses automorphismes ; si E est une extension galoisienne du corps K, le groupe Aut$_K(E)$ n’est autre que le groupe de Galois Gal(E$/K)$ (V, p. 56).

Soit G un groupe. On appelle $(K,G)$-algèbre une K-algèbre E munie d’un homomorphisme de groupes $\lambda : G\rightarrow$ Aut$_K(E)$. L’homomorphisme $\lambda$ munit alors E d’une structure de groupe à opérateurs dans G ainsi que d’une structure de K[G]-module à gauche dont la loi d’action est donnée par

$$
(\sum_{g\in G}\mu_gg)x=\sum_{g\in G}\mu_g\lambda (g).x \tag{14}
$$

pour tout $x\in L$ et tout élément $(\mu_g)_{g\in G}$ de K[G]. Un morphisme de $(K$, G)-algèbres est un morphisme d’algèbres qui est également un morphisme de groupes à opérateurs.

Pour toute famille $(E_i)_{i\in I}$ de $(K$, G)-algèbres, la K-algèbre produit$\prod_{i\in I}E_i$ munie de sa structure de groupe à opérateurs produit est une $(K$, G)-algèbre.

Si E est une $(K$, G)-algèbre, l’ensemble $E^G$ des éléments de E invariants sous G est une sous-algèbre de E.

Soit E une $(K$, G)-algèbre, où G opère par $\lambda : G\rightarrow$ Aut$_K(E)$. Si $K'$ est une extension de K, pour tout $g\in G$, soit $\lambda '(g)$ l’automorphisme Id$_{K'}\otimes \lambda (g)$ de la $K'$-algèbre $L_{(K')}$. Alors $\lambda ':g\rightarrow \lambda '(g)$ munit $L_{(K')}$ d’une structure de $(K'$, G)-algèbre.

Étant donné un groupe H et des H-ensembles X et Y, on note $\mathscr{F}_H(X,Y)$ l’ensemble des morphismes de H-ensembles de X dans Y. C’est donc l’ensemble des applications $f: X\rightarrow Y$ telles que $f(hx) =hf(x)$ pour tout $h\in H$ et tout $x\in X$.

Soit G un groupe d’élément neutre $e$, soit H un sous-groupe de G et soit E une $(K$, H)-algèbre. On note Coïnd$^G_H(E)$ et on appelle $(K,G)$-algèbre déduite de E par coïnduction de H à G la K-algèbre $\mathscr{F}_H(G,E)$ munie de l’action de G donnée par l’homomorphisme $\lambda$ de G dans Aut$_K$(Coïnd$^G_H(E))$ défini par

$$
(\lambda (g).f)(g') =f(g'g) \tag{15}
$$

pour $f\in$ Coïnd$^G_H(E)$ et $g, g'\in G$.

#### Lemme 7 {#alg-viii-s16-lem-7 .statement tag=00IX}

a) Soit S une partie de G telle que tout élément de G s’écrive de manière unique sous la forme $hs$ avec $h\in H$et $s\in S$. Alors l’application envoyant $f$ sur $(f(s))_{s\in S}$ est un isomorphisme de la K-algèbre Coïnd$^G_H(E)$sur la K-algèbre $\mathscr{F}(S,E)$des applications de S dans E.

b) L’algèbre Coïnd$^G_H(E)$est de degré fini sur K si et seulement si E est de degré fini sur K et l’indice de H par rapport à G est fini. Dans ce cas, on a la formule

[Coïnd$^G_H(E) : K] = (G : H)[E : K]$.

c) Soient $E^H$ l’algèbre des invariants du groupe H dans E et Coïnd$^G_H(E)^G$ celle du groupe G dans Coïnd$^G_H(E)$. L’application $f\rightarrow f(e)$de Coïnd$^G_H(E)$dans E induit par passage aux sous-ensembles un isomorphisme d’algèbres de Coïnd$^G_H(E)^G$ sur $E^H$.

L’assertion a) résulte des définitions et b) en découle. Par (15), une application de G dans E est un élément de Coïnd$^G_H(E)$ invariant sous G si et seulement si elle est constante de valeur un élément de E invariant sous H.

#### Remarque 1 {#alg-viii-s16-n7-rem-1 .statement tag=00IY}

Soient G un groupe, H un sous-groupe de G et N un sous-groupe de H. Soit E une $(K$, N)-algèbre. Soit $\alpha$ un élément de $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$. On a la relation

$$
\alpha (g)(nh) =n(\alpha (g)(h)) \tag{16}
$$

pour tout $g\in G$, tout $h\in H$ et tout $n\in N$ et les relations

$$
\alpha (hg)(h') = (h\alpha (g))(h') =\alpha (g)(h'h) \tag{17}
$$

pour tous $h, h'\in H$ et tout $g\in G$. Par conséquent, $\alpha (ng)(e) =\alpha (g)(n) =n(\alpha (g)(e))$ pour tout $g\in G$ et tout $n\in N$. On peut donc considérer l’application

$$
\psi :\mathscr{F}_H(G,\mathscr{F}_N(H,E))\rightarrow \mathscr{F}_N(G,E)
$$

définie par la relation $\psi (\alpha )(g) =\alpha (g)(e)$ pour tout élément $\alpha$ de $\mathscr{F}_H(G,\mathscr{F}_N(H,E))$ et tout élément $g$ de G. L’application $\psi$ est un isomorphisme d’algèbres de l’algèbre Coïnd$^G_H$(Coïnd$^H_N(E))$ sur Coïnd$^G_N(E)$ dont la réciproque envoie un élément $\beta$ de $\mathscr{F}_N(G,E)$ sur l’application $\alpha$ définie par la relation $\alpha (g)(h) =\beta (hg)$ pour $g\in G$ et $h\in H$.

On suppose maintenant donnés un groupe fini G, une K-algèbre L commutative, de degré fini et réduite (V, p. 33), munie en outre d’une action de G donnée par un homomorphisme $\lambda$ de G dans Aut$_K(L)$. Pour $x\in L$ et $g\in G$, on note $g.x$ le transformé de $x$ par l’automorphisme$\lambda (g)$ de L. Soit $\mathscr{S}$ l’ensemble des idéaux maximaux de L ; on note $g.\mathfrak{m}$ le transformé d’un élément $\mathfrak{m}$ de $\mathscr{S}$ par l’automorphisme $\lambda (g)$ de L. C’est un élément de $\mathscr{S}$. Pour tout $\mathfrak{m}$ de $\mathscr{S}$, le corps $L/\mathfrak{m}$ est une extension finie de K. On note $\pi_{\mathfrak{m}}: L\rightarrow L/\mathfrak{m}$ et $G_{\mathfrak{m}}$ le stabilisateur de $\mathfrak{m}$ dans G, c’est-à-dire l’ensemble des $g\in G$ tels que $g\mathfrak{m}=\mathfrak{m}$; la K-algèbre $L/\mathfrak{m}$ est munie d’une action de $G_{\mathfrak{m}}$ via l’homomorphisme $\lambda_{\mathfrak{m}}$ de $G_{\mathfrak{m}}$ dans Aut$_K(L/\mathfrak{m})$ qui, à un élément $h$ de $G_{\mathfrak{m}}$, associe l’automorphisme de $L/\mathfrak{m}$ déduit de $\lambda (h)$ par passage aux quotients.

Soit $\mathscr{O}$ l’ensemble des orbites de G dans $\mathscr{S}$. Étant donnée une orbite $\sigma \in \mathscr{O}$, posons $\mathfrak{a}_{\sigma}=\bigcap_{\mathfrak{m}\in\sigma}\mathfrak{m}$ et $L_{\sigma}= L/\mathfrak{a}_{\sigma}$. Comme $\mathfrak{a}_{\sigma}$ est invariant par G, l’action de G sur L définit par passage aux quotients un homomorphisme $\lambda_{\sigma}$ de G dans Aut$_K(L_{\sigma})$. Enfin, notons $\pi_{\sigma}$ l’application canonique de L sur $L_{\sigma}$.

#### Lemme 8 {#alg-viii-s16-lem-8 .statement tag=00RL}

a) Pour tout $g\in G$, tout $\sigma \in \mathscr{O}$ et tout $\mathfrak{m}\in \sigma$,

$[L_{\sigma}: K] =$ Card($\sigma$ )$[L/\mathfrak{m}: K]$.

b) L’application $\pi :x\rightarrow (\pi_{\sigma}(x))_{\sigma\in\mathscr{O}}$ est un isomorphisme de $(K,G)$-algèbres de L sur $\prod_{\sigma\in\mathscr{O}}L_{\sigma}$.

c) Notons $L^G$ (resp. $L^G_{\sigma})$la sous-algèbre de L (resp. $L_{\sigma})$des éléments invariants sous l’action de G dans L (resp. $L_{\sigma})$. Alors $\pi$ induit un isomorphisme de $L^G$ sur $\prod_{\sigma\in\mathscr{O}}L^G_{\sigma}$.

Comme l’algèbre L est réduite et de degré fini, l’intersection des idéaux maximaux de L est réduite à 0 (VIII, p. 169, cor. 2). De plus si $\mathfrak{m}$ et $\mathfrak{m}'$ sont deux idéaux maximaux de L distincts, on a $\mathfrak{m}+\mathfrak{m}'= L$. D’après la prop. 10 de I, p. 105, l’application canonique de L dans $\prod_{\mathfrak{m}\in\mathscr{S}}L/\mathfrak{m}$ est un isomorphisme de même que l’application canonique de $L/\mathfrak{a}_{\sigma}$ dans $\prod_{\mathfrak{m}\in\sigma}L/\mathfrak{m}$, pour tout $\sigma \in \mathscr{O}$. L’assertion a) en résulte. Comme $\mathscr{O}$ est une partition de $\mathscr{S}$, l’assertion b) en découle et c) est une conséquence immédiate de b).

Fixons maintenant une orbite $\sigma \in \mathscr{O}$ et un élément $\mathfrak{m}$ de $\sigma$. Posons $F_{\mathfrak{m}}=$ Coïnd$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ et notons $\lambda_{F_{\mathfrak{m}}}$ l’action de G sur $F_{\mathfrak{m}}$. Pour tout $x\in L$, notons $x$ l’application de G dans $L/\mathfrak{m}$ qui envoie $g$ sur $\pi_{\mathfrak{m}}(gx)$. Compte tenu de la formule (15) de VIII, p. 300 et de la définition de l’action de $G_{\mathfrak{m}}$ sur $L/\mathfrak{m}$, il est immédiat que $x$ appartient à $F_{\mathfrak{m}}$ et l’application $u:x\rightarrow x$ de L dans $F_{\mathfrak{m}}$ vérifie $\lambda_{F_{\mathfrak{m}}}(g)\circ u=u\circ \lambda (g)$ pour $g\in G$. Autrement dit, $u$ est un morphisme de $(K$, G)-algèbres.

#### Lemme 9 {#alg-viii-s16-lem-9 .statement tag=00IZ}

Le morphime $u$ est surjectif de noyau $\mathfrak{a}_{\sigma}$. L’application déduite de $u$ par passage au quotient est un isomorphisme de $(K,G)$-algèbres de $L_{\sigma}$ sur $F_{\mathfrak{m}}$.

Comme le noyau de $\pi_{\mathfrak{m}}$ est égal à $\mathfrak{m}$, celui de $u$ est égal à $\bigcap_{g\in G}g^{-1}.\mathfrak{m}=\mathfrak{a}_{\sigma}$. Pour prouver que $u$ est surjectif, il suffit de démontrer que les espaces vectoriels $L_{\sigma}= L/\mathfrak{a}_{\sigma}$ et $F_{\mathfrak{m}}$ ont même dimension sur K. Or tous les idéaux $g.\mathfrak{m}$ ont la même codimension dans L et, par le lemme 8 a),

$[L_{\sigma}: K] =$ Card($\sigma$ )$.[L/\mathfrak{m}: K]$.

Par ailleurs, d’après le lemme 7, b) de VIII, p. 300, on a

$$
[F_{\mathfrak{m}}: K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]
$$

comme on a Card($\sigma$ ) $= (G : G_{\mathfrak{m}})$, on a prouvé l’égalité $[L_{\sigma}: K] = [F_{\mathfrak{m}}: K]$.

On suppose maintenant en outre que l’homomorphisme$\lambda$ de G dans Aut$_K(L)$ est injectif. On identifie K à son image dans L par l’application $\xi \rightarrow \xi .1$. Par ailleurs, soit Ω une extension algébriquement close de K. L’ensemble $\mathscr{F}(G,\Omega )$ des applications de G dans Ω coïncide avec la $(\Omega$, G)-algèbre coïnduite Coïnd$^G_{\{e\}}(\Omega )$. C’est un Ω[G]module libre de rang 1. Soit $\mathscr{H}$ l’ensemble des homomorphismes de K-algèbres de L dans Ω. On fait opérer G à droite sur $\mathscr{H}$ par la loi d’action $(g, \chi )\rightarrow \chi \circ \lambda (g)$. La Ω-algèbre $\mathscr{F}(\mathscr{H},\Omega )$ est alors munie d’une structure de $(\Omega$, G)-algèbre déduite de l’action à droite de G sur $\mathscr{H}$.

#### Lemme 10 {#alg-viii-s16-lem-10 .statement tag=00J0}

Soit L une $(K,G)$-algèbre qui est étale sur K. L’application $\psi$ de $L_{(\Omega )}$ dans $\mathscr{F}(\mathscr{H},\Omega )$caractérisée par la relation

$$
\psi (\xi \otimes x) = (\xi \chi (x))_{\chi\in\mathscr{H}}
$$

est un isomorphisme de $(K,G)$-algèbres.

Comme L est étale, l’application $\psi$ est un isomorphisme de Ω-algèbres (V, p. 29, prop. 2 et V, p. 28, prop. 1, c)). On a les relations

$\psi$((Id $\otimes \lambda (g))(\xi \otimes x)) = (\xi (\chi \circ \lambda (g))(x))_{\chi\in\mathscr{H}}$

pour $\xi \in \Omega ,x\in L$ et $g\in G$. Donc $\psi$ est un morphisme de $(\Omega$, G)-algèbres.

#### Théorème 2 {#alg-viii-s16-thm-2 .statement tag=00J1}

Soit G un groupe fini et soit L une K-algèbre commutative, de degré fini et réduite munie d’une action de G donnée par un homomorphisme injectif $\lambda$ de G dans Aut$_K(L)$. Alors, les conditions suivantes sont équivalentes :

(i) Il existe un sous-groupe H de G, une extension galoisienne E de degré fini de K, un isomorphisme de H sur Gal(E$/K)$et un isomorphisme de $(K,G)$-algèbres de L sur Coïnd$^G_H(E)$;

(ii) L’algèbre L est étale et $\mathscr{H}$ est un G-ensemble principal homogène (I, p. 58, déf. 7) ;

(iii) Il existe un isomorphisme de $(\Omega ,G)$-algèbres $\psi : L_{(\Omega )}\rightarrow \mathscr{F}(G,\Omega )$autrement dit, pour tout $g\in G$, l’automorphisme $\psi \circ \lambda (g)_{(\Omega )}\circ \psi^{-1}$ est égal à l’automorphisme

$$
(x_h)_{h\in G}\longrightarrow (x_{hg})_{h\in G}
$$

de $\Omega^G$;

(iv) L’algèbre L est réduite et L est un K[G]-module libre de rang 1 ;

(v) L’algèbre L est réduite, on a Card(G) = [L : K] et K est le sous-anneau de L des éléments invariants sous l’action de G ;

(vi) L’algèbre L est réduite, le groupe G opère transitivement sur l’ensemble des idéaux maximaux de L et, pour tout idéal maximal $\mathfrak{m}$ de L, le stabilisateur $G_{\mathfrak{m}}$ de $\mathfrak{m}$ dans G agit fidèlement dans $L/\mathfrak{m}$ et admet K comme sous-corps des invariants.

(i)$\Rightarrow$(ii) : Soient E une extension galoisienne de degré fini de K et $\tau$ un isomorphisme de H sur Aut$_K(E)$. Soit S un système de représentants des classes à droite suivant H dans G. La K-algèbre F = Coïnd$^G_H(E)$ est isomorphe à $\mathscr{F}(S,E)$ (VIII, p. 300, lemme 7 a)), elle est donc étale. Notons $\lambda_F$ l’action de G sur F. Par ailleurs, soit $\psi$ un homomorphisme de K-algèbres de E dans Ω et soit $\chi_0$ l’homomorphisme $f\rightarrow \psi (f(e))$ de F dans Ω. Soit $g\in G$ tel que l’on ait $\chi_0\circ \lambda_F(g) =\chi_0$; Comme $\psi$ est injective, on a alors $f(g) =f(e)$ pour tout $f\in F$. Compte tenu du lemme 7, a) de VIII, p. 300$,g\in H$ et par la formule

$$
f(h) =\tau (h).f(e) \tag{18}
$$

valide pour tout $h\in H$, ceci ne peut avoir lieu que pour $g=e$. D’autre part, d’après le lemme 7, b) de VIII, p. 300 et le th. 3 de V, p. 64, on a

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G).

L’ensemble $\mathscr{K}$ des K-homomorphismes de F dans Ω est de cardinal [F : K] puisque F est étale (V, p. 31, prop. 4), d’où Card($\mathscr{K}$) $=$ Card(G). Comme le stabilisateur de $\chi_0$ dans G est égal à $\{e\}$ par ce qui précède, le G-ensemble $\mathscr{K}$ est principal homogène.

(ii)$\Rightarrow$(iii) : Supposons que L soit étale et que $\mathscr{H}$ soit un G-ensemble principal homogène. Par le lemme 10, les $(\Omega$, G)-algèbres $L_{(\Omega )}$ et $\mathscr{F}(\mathscr{H},\Omega )$ sont isomorphes. Comme $\mathscr{H}$ est un G-ensemble principal homogène, les $(\Omega$, G)-algèbres $\mathscr{F}(\mathscr{H},\Omega )$ et $\mathscr{F}(G,\Omega )$ sont isomorphes.

(iii)$\Rightarrow$(iv) : Supposons la propriété (iii) satisfaite ; alors $L_{(\Omega )}$ est un module libre de rang 1 sur l’algèbre Ω[G] et cette dernière s’identifie canoniquement à $K[G]_{(\Omega )}$. On applique alors le théorème 3 de VIII, p. 34.

L’implication (iv)$\Rightarrow$(v) est immédiate.

Démontrons l’implication (v)$\Rightarrow$(vi). L’algèbre L est réduite. Par le lemme 8, c), G opère transitivement sur l’ensemble $\mathscr{S}$ des idéaux maximaux de L. Soit $\mathfrak{m}$ un élément de $\mathscr{S}$. Par le lemme 9, comme $\bigcap_{\mathfrak{n}\in\mathscr{S}}\mathfrak{n}=\{0\}$, l’algèbre L est isomorphe à l’algèbre Coïnd$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$. L’algèbre des invariants de $G_{\mathfrak{m}}$ dans $L/\mathfrak{m}$ coïncide donc avec K par le lemme 7, c). Donc l’homomorphisme $\lambda_{\mathfrak{m}}$ de $G_{\mathfrak{m}}$ sur Gal((L$/\mathfrak{m})/K)$ est surjectif. Par la lemme 7, on a en outre

Card(G) $= [L : K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]$ Donc Card(G$_{\mathfrak{m}}) = [L/\mathfrak{m}: K]$ et l’homomorphisme $\lambda_{\mathfrak{m}}$ est injectif.

Il reste à démontrer l’implication (vi)$\Rightarrow$(i). Soit $\mathfrak{m}$ un idéal maximal de L. Par le lemme 9, l’algèbre L est isomorphe à l’algèbre Coïnd$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ en tant que $(K$, G)-algèbre. Comme $G_{\mathfrak{m}}$ agit fidèlement dans $L/\mathfrak{m}$ et admet K comme sous-corps des invariants, l’homomorphisme de groupes $\lambda_{\mathfrak{m}}$ définit un isomorphisme de $G_{\mathfrak{m}}$ sur Gal((L$/\mathfrak{m})/K)$.

#### Remarque 2 {#alg-viii-s16-n7-rem-2 .statement tag=00J2}

Dans le théorème 2, on peut remplacer l’hypothèse que Ω est algébriquement clos par l’hypothèse que Ω est séparablement clos. En effet, si L est étale, l’image de tout homomorphisme de K-algèbres de L dans Ω est une extension séparable de K.

#### Remarque 3 {#alg-viii-s16-n7-rem-3 .statement tag=00J3}

Le théorème de la base normale (V, p. 70, th. 6) est un cas particulier de l’implication (i)$\Rightarrow$(iv) dans le théorème 2.

#### Définition 1 {#alg-viii-s16-def-1 .statement tag=00J4}

Soit G un groupe fini et soit L une algèbre commutative, non nulle, et de degré fini sur K, munie d’une structure de $(K,G)$-algèbre, l’action de G étant donnée par un homomorphisme injectif de G dans le groupe Aut$_K(L)$. On dit que L est une algèbre galoisienne de groupe G si elle satisfait aux propriétés équivalentes (i) à (vi) du théorème 2.

#### Remarque 4 {#alg-viii-s16-n7-rem-4 .statement tag=00J5}

Supposons que L soit une extension de K munie d’une action $\lambda$ de G. Alors L est une algèbre galoisienne sur K si et seulement si L est une extension galoisienne de K et $\lambda$ un isomorphisme de G sur le groupe de Galois de L sur K.

#### Remarque 5 {#alg-viii-s16-n7-rem-5 .statement tag=00J6}

Supposons que le groupe G soit commutatif. Si G opère fidèlement et transitivement sur un ensemble X, le stabilisateur de tout point de X est réduit à l’identité (car les stabilisateurs des points de X sont tous égaux et leur intersection est réduite à l’élément neutre de G). Par suite, les propriétés (i) à (vi) énoncées dans le théorème 2 sont encore équivalentes à la suivante :

(vii) L’algèbre L est étale et G opère fidèlement et transitivement sur $\mathscr{H}$.

#### Remarque 6 {#alg-viii-s16-n7-rem-6 .statement tag=00J7}

D’après V, p. 72, lemme 5, V, p. 73, prop. 12 et VIII, p. 133, prop. 3, une algèbre galoisienne est commutative et semi-simple.

#### Exemple 1 {#alg-viii-s16-n7-exa-1 .statement tag=00J8}

Soit $n$ un entier strictement positif, étranger à l’exposant caractéristique de K. On suppose que le groupe $\mu_n$ des racines $n$-èmes de l’unité dans K est d’ordre $n$. Pour tout diviseur $d$ de $n$, le groupe $\mu_d$ des racines $d$-èmes de l’unité est alors d’ordre $d$. Soit $a$ un élément non nul de K, soit L l’algèbre $K[X]/(X^n-a)$ et soit $x$ la classe de X dans L. La suite $(1, x, . . . , x^{n-1})$ est une base de l’espace vectoriel L sur le corps K et l’on a $x^n=a$. De plus, le polynôme $X^n-a$ est étranger à sa dérivée $nX^{n-1}$, donc l’algèbre L est étale (V, p. 36, prop. 3). Pour tout $\zeta$ dans $\mu_n$, l’automorphisme $P(X)\rightarrow P(\zeta X)$ de l’anneau K[X] définit par passage aux quotients un endomorphisme $\lambda (\zeta )$ de L, puisqu’on a $(\zeta X)^n-a= X^n-a$; c’est un automorphisme. On a

$$
\lambda (\zeta )x^i=\zeta^ix^i \tag{19}
$$

pour $0\leqslant i < n$. L’application $\lambda :\zeta \rightarrow \lambda (\zeta )$ est un homomorphisme injectif de $\mu_n$ dans Aut$_K(L)$ et l’anneau des invariants du groupe $\lambda (\mu_n)$ dans L est égal à $K.1$. Comme le cardinal de $\mu_n$ est égal à $n= [L : K]$, l’algèbre L munie de l’action $\lambda$ est une algèbre galoisienne (VIII, p. 303, th. 2, (v)).

Soit $r$ le plus petit entier strictement positif tel que $a^r$ appartienne à $K^{*n}$; c’est un diviseur de $n$ et il existe un élément $b$ de $K^*$ tel que $a=b^{n/r}$. Alors (V, p. 87, remarque), le polynôme $X^r-b$ est irréductible et l’on a $X^n-a=\prod_{\zeta\in\mu_{n/r}}(X^r-\zeta b)$. Soit E le corps $K[Y]/(Y^r-b)$ et soit $y$ la classe de Y dans E. Il existe un isomorphisme $\theta$ de $\mu_{n/r}$ sur Gal(E$/K)$, caractérisé par la relation $\theta (\xi )(y) =\xi y$ (V, p. 86, exemple 3). On vérifie alors que l’algèbre galoisienne L est isomorphe à la $(K, \mu_n$)-algèbre Coïnd$^{\mu}_{\mu^n_{n/r}}(E)$.

#### Exemple 2 {#alg-viii-s16-n7-exa-2 .statement tag=00J9}

Supposons maintenant que le corps K soit de caractéristique $p\not= 0$. Soit $c$ un élément de K. Le polynôme $f= X^p-X-c$ est étranger à sa dérivée $f'=-1$, l’algèbre $L = K[X]/(f)$ est donc étale (V, p. 36, prop. 3). On note $x$ l’image de X dans L, et on a la relation $x^p=x+c$; la suite $(1, x, . . . , x^{p-1})$ est une base de L considéré comme espace vectoriel sur K.

Soit P le groupe additif du sous-corps premier de K ; c’est un groupe cyclique d’ordre $p$, engendré par l’élément unité 1 de K. Pour tout $j$ dans P, on a $j^p=j$ (V, p. 4, (4)), d’où $f(X +j) =f(X)$. Il existe donc un automorphisme $\gamma (j)$ de l’algèbre L caractérisé par la relation $\gamma (j)(x) =x+j$; de plus, l’application $\gamma$ ainsi définie est un homomorphisme injectif de P dans Aut$_K(L)$.

Soit Ω une extension algébriquement close de K et soit $\xi$ une racine du polynôme $f$ dans Ω. On a $\xi^p=\xi +c$, d’où

$$
X^p-X-c= (X^p-\xi^p)-(X-\xi ) = (X-\xi )^p-(X-\xi ) =\prod_{j\in P}(X-\xi -j)
$$

d’après V, p. 89, formule (1). Pour tout $j$ dans P, il existe un unique homomorphisme d’algèbres $\chi_j: L\rightarrow \Omega$ qui applique $x$ sur $\xi +j$; de plus, tout homomorphisme de L dans Ω est l’un des $\chi_j$ et l’on a la relation $\chi_j=\chi_0\circ \gamma (j)$. D’après la condition (ii) du th. 2 de VIII, p. 303, l’algèbre L munie de $\gamma$ est une algèbre galoisienne sur K.

Pour décrire la structure de L on doit distinguer deux cas :

a) On a $\xi \notin K :$ alors le polynôme $f(X)$ est irréductible dans K[X] (V, p. 89, exemple 3). Dans ce cas L est une extension cyclique de degré $p$ de K et $\gamma$ est un isomorphisme de P sur Gal(L$/K)$.

b) On a $\xi \in K :$ alors l’application $\psi :y\rightarrow (\chi_j(y))_{j\in P}$ est un isomorphisme de l’algèbre L sur l’algèbre produit $K^P$; de plus, $\psi \circ \gamma (k)\circ \psi^{-1}$ est l’automorphisme $(x_j)_{j\in P}\rightarrow (x_{j+k})_{j\in P}$ de $K^P$ pour tout $k\in P$.

### 8. Opérations sur les algèbres galoisiennes

#### Proposition 9 {#alg-viii-s16-prop-9 .statement tag=00JA}

Soit G un groupe fini, soit H un sous-groupe de G et soit E une algèbre galoisienne de groupe H sur le corps K. Alors la $(K,G)$-algèbre Coïnd$^G_H(E)$ déduite de E par coïnduction de H à G est une algèbre galoisienne de groupe G sur le corps K.

Comme E est une algèbre galoisienne sur K, l’algèbre E est réduite, on a Card(H) = [E : K] et K est l’anneau des invariants de H dans E (propriété (v) du th. 2 de VIII, p. 303). Mais d’après le lemme 7 de VIII, p. 300, l’algèbre F = Coïnd$^G_H(E)$ est réduite, et on a

[F : K] = (G : H)[E : K] = (G : H) Card(H) = Card(G),

et K est l’anneau des invariants de G dans F. Donc F est une algèbre galoisienne d’après le critère donné par le th. 2, (v).

#### Proposition 10 {#alg-viii-s16-prop-10 .statement tag=00JB}

Soit G un groupe fini. Soit L une algèbre galoisienne de groupe G sur le corps K et soit $K'$ une extension de K. Alors la $(K',G)$-algèbre $L_{(K')}$ est une algèbre galoisienne sur $K'$.

On utilise le th. 2, (v) en remarquant que si la K-algèbre L est étale, la $K'$-algèbre $L_{(K')}$ l’est aussi (V, p. 32, cor. 2), que l’on a l’égalité $[L_{(K')}: K'] = [L : K]$, et que l’anneau des invariants de G dans $L_{(K')}$ est $(L^G)_{(K')}$, où $L^G$ est l’anneau des invariants de G dans L.

#### Proposition 11 {#alg-viii-s16-prop-11 .statement tag=00JC}

Soient $G_1$ et $G_2$ des groupes. Soient $L_1$ et $L_2$ des algèbres galoisiennes sur K d’actions respectives $\lambda_1: G_1\rightarrow$ Aut$_K(L_1)$et $\lambda_2: G_2\rightarrow$ Aut$_K(L_2)$. Posons $L = L_1\otimes_KL_2, G = G_1\times G_2$ et $\lambda (g_1, g_2) =\lambda_1(g_1)\otimes \lambda_2(g_2)$pour $(g_1, g_2)\in G$. Alors la K-algèbre L munie de l’action $\lambda$ est une algèbre galoisienne sur K.

On raisonne comme précédemment au moyen des remarques suivantes : si $L_1$ et $L_2$ sont étales, il en est de même de l’algèbre $L = L_1\otimes_KL_2$ (V, p. 31, cor. 1) et l’on a les égalités

$[L : K] = [L_1: K][L_2: K]$ et Card(G) = Card(G$_1)$ Card(G$_2)$.

De plus si $L^G_{i^i}$ désigne l’anneau des invariants de $G_i$ dans $L_i$ alors il résulte du lemme suivant que $L^G_{1^1}\otimes_KL^G_{2^2}$ est l’anneau des invariants de $G_1\times G_2$ dans $L_1\otimes_KL_2$.

#### Lemme 11 {#alg-viii-s16-lem-11 .statement tag=00JD}

Soient $G_1$ et $G_2$ des groupes et soient $W_1$ et $W_2$ des K-espaces vectoriels. On munit $W_1$ (resp. $W_2)$d’une action de $G_1$ (resp. $G_2)$donnée par un homomorphisme de groupes $\rho_1: G_1\rightarrow$ Aut$_K(W_1)$ (resp. $\rho_2: G_2\rightarrow$ Aut$_K(W_2))$. On considère l’homomorphisme de groupes

$\rho_1\otimes \rho_2: G_1\times G_2\longrightarrow$ Aut$_K(W_1\otimes_KW_2)$

défini par la relation $(\rho_1\otimes \rho_2)(g_1, g_2)(w_1\otimes w_2) =\rho_1(g_1)(w_1)\otimes \rho_2(g_2)(w_2)$, pour tout $g_1\in G_1$ tout $g_2\in G_2$, tout $w_1\in W_1$ et tout $w_2\in W_2$. Alors l’application linéaire de $W^G_{1^1}\otimes_KW^G_{2^2}$ dans $W_1\otimes_KW_2$ donnée par le produit tensoriel des injections canoniques induit un isomorphisme de K-espaces vectoriels de $W^G_{1^1}\otimes_KW_2^{G_2}$ sur $(W_1\otimes_KW_2)^{G_1\times G_2}$.

Cela résulte du lemme 1 de VIII, p. 209, appliqué aux K[G]-modules $M_1=$ $M_2= K$ munis de l’action triviale de $G, N_1= W_1$ et $N_2= W_2$.

#### Remarque {#alg-viii-s16-n8-rem-1 .statement tag=00JE}

☡ Soit L une extension galoisienne de degré fini du corps K et soit G son groupe de Galois ; notons $\lambda$ l’application identique de G. Alors L muni de $\lambda$ est une algèbre galoisienne de groupe G sur K. Soit $K'$ une extension de K. D’après la proposition 10, $L_{(K')}$ est une algèbre galoisienne sur $K'$, mais ce n’est pas en général une extension de $K'$. De manière analogue, d’après la prop. 11, le produit tensoriel d’extensions galoisiennes E et F de degré fini de K peut être considéré comme une algèbre galoisienne ; en général, ce n’est pas une extension galoisienne de K. C’est néanmoins le cas si E et F sont en outre des sous-extensions linéairement disjointes d’une extension de K (V, p. 13 et p. 55, prop. 1).

### 9. Produits croisés

Soit K un corps et soit G un groupe dont on note $e$ l’élément neutre, soit L une K-algèbre commutative et soit $\lambda$ un homomorphisme de G dans le groupe des automorphismes de la K-algèbre L. Pour tout $g$ de G, soit $\tau (g)$ l’automorphisme du groupe multiplicatif $L^*$ de L qui est induit par $\lambda (g)$.

Soit $\mathscr{E}= (\Gamma , \iota , \pi )$ une $\tau$-extension du groupe G par $L^*$. Faisons opérer le groupe $L^*$ à droite sur l’ensemble $L\times \Gamma$ par la loi d’opération :

$$
(\beta , \gamma ).\alpha = (\beta \alpha , \iota (\alpha )^{-1}\gamma ) \tag{20}
$$

pour $\alpha \in L^*,\beta \in L$ et $\gamma \in \Gamma$. Notons E l’ensemble des orbites de $L^*$ dans $L\times \Gamma$ et $[\beta ;\gamma ]$ l’orbite du couple $(\beta , \gamma )$. On a donc par construction la relation

$$
[\beta \alpha ;\gamma ] = [\beta ;\iota (\alpha )\gamma ] \tag{21}
$$

pour $\alpha \in L^*,\beta \in L$ et $\gamma \in \Gamma$.

Étant donnés $\beta$ dans L et $\gamma$ dans Γ, on note $^{\gamma}\beta$ le transformé de $\beta$ par l’automorphisme $\lambda \circ \pi (\gamma )$ de L ; on a les relations

(22) $^{\gamma}(^{\gamma'}\beta ) =^{\gamma \gamma'}\beta ,^{\gamma}(\beta +\beta ') =^{\gamma}\beta +^{\gamma}\beta '$ et $^{\gamma}(\beta \beta ') =^{\gamma}\beta^{\gamma}\beta '$

pour $\gamma , \gamma '$ dans Γ et $\beta , \beta '$ dans L. Il existe une loi de composition sur E caractérisée par la relation

$$
[\beta ;\gamma ][\beta ';\gamma '] = [\beta^{\gamma}\beta ';\gamma \gamma '] \tag{23}
$$

en effet, il suffit de vérifier que le membre de droite ne change pas si l’on remplace respectivement $\beta ,\gamma ,\beta ',\gamma '$ par $\beta \alpha ,\iota (\alpha )^{-1}\gamma ,\beta '\alpha ',\iota (\alpha ')^{-1}\gamma '$ avec $\alpha ,\alpha '$ dans $L^*$ et cela résulte aussitôt de la formule (1) de VIII, p. 281 appliquée à $\mathscr{E}$ qui s’écrit également $\gamma \iota (\alpha ) =\iota (^{\gamma}\alpha )\gamma$ pour $\gamma \in \Gamma$ et $\alpha \in L^*$. D’après les formules (22), l’ensemble E muni de cette loi est un monoïde d’élément neutre $[1;e]$.

Comme $\pi \circ \iota$ est constante de valeur $e$, il existe une application $\widetilde{\pi}$ de E dans G telle que l’on ait

$$
\widetilde{\pi}([\beta ;\gamma ]) =\pi (\gamma ) \tag{24}
$$

pour $\beta \in L$ et $\gamma \in \Gamma$.

Soit $g$ un élément de G et soit $E_g=\widetilde{\pi}^{-1}(g)$. Si $\gamma_0$ est un élément fixé de $\pi^{-1}(g)$, l’application $\beta \rightarrow [\beta ;\gamma_0]$ est une bijection de L sur $E_g$, grâce à laquelle nous transporterons à $E_g$ la structure de K-espace vectoriel de L. Comme $\pi^{-1}(g)$ se compose des éléments de la forme $\iota (\alpha )\gamma_0$ où $\alpha$ parcourt $L^*$ et que l’on a

$$
[\beta ;\iota (\alpha )\gamma_0] = [\beta \alpha ;\gamma_0]
$$

la structure d’espace vectoriel de $E_g$ ne dépend pas du choix de $\gamma_0$.

Soient $g$ et $g'$ des éléments de G ; d’après les formules (22) et (23), la loi de composition de E induit par restriction une application K-bilinéaire de $E_g\times E_{g'}$ dans $E_{gg'}$. Par suite, l’espace vectoriel $P =\bigoplus_{g\in G}E_g$ est muni d’une structure d’algèbre associative et unifère, dont la multiplication induit l’application bilinéaire précédente de $E_g\times E_{g'}$ dans $E_{gg'}$, quels que soient $g$ et $g'$ dans G. L’algèbre P s’appelle le produit croisé de L par $\mathscr{E}$ et se note $\mathbf{A}[\mathscr{E}; L]$; son élément unité est l’élément $[1;e]$ de $E_e$.

Posons

$$
u(\beta ) = [\beta ;e] \tag{25}
$$

pour $\beta$ dans L. Alors $u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ est un homorphisme injectif de K-algèbres. Par (23), pour tout $\gamma \in \Gamma$, l’élément $[1;\gamma ]$ est inversible dans $\mathbf{A}[\mathscr{E},L]$ et l’application $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E},L]^*$ qui envoie $\gamma$ sur $[1;\gamma ]$ est un homomorphisme injectif de groupes. Les homomorphismes $u$ et $v$ sont dits canoniques. On a les relations

$$
u(\alpha ) =v(\iota (\alpha )) \tag{26}
$$

$$
u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1} \tag{27}
$$

$$
[\beta ;\gamma ] =u(\beta )v(\gamma ) \tag{28}
$$

pour $\alpha \in L^*,\beta \in L$ et $\gamma \in \Gamma$.

Réciproquement, on a la propriété universelle suivante de l’algèbre $\mathbf{A}[\mathscr{E}; L] :$

#### Proposition 12 {#alg-viii-s16-prop-12 .statement tag=00JF}

Soient B une K-algèbre, $u': L\rightarrow B$un homomorphisme de K-algèbres et $v': \Gamma \rightarrow B^*$ un homomorphisme de groupes. On suppose vérifiées les relations

$$
u'(\alpha ) =v'(\iota (\alpha )) \tag{29}
$$

$$
u'(^{\gamma}\beta ) =v'(\gamma )u'(\beta )v'(\gamma )^{-1} \tag{30}
$$

pour $\alpha$ dans $L^*,\beta$ dans L et $\gamma$ dans Γ. Il existe alors un homomorphisme d’algèbres $f$ de $\mathbf{A}[\mathscr{E}; L]$dans B, et un seul, tel que l’on ait $u'=f\circ u$ et $v'=f\circ v$.

Pour démontrer l’unicité de $f$, remarquons que l’espace vectoriel $\mathbf{A}[\mathscr{E}; L]$ sur le corps K est engendré par l’ensemble des éléments de la forme $[\beta ;\gamma ] =u(\beta )v(\gamma )$; si l’homomorphisme $f': \mathbf{A}[\mathscr{E}; L]\rightarrow B$ satisfait à $f'\circ u=u'$ et $f'\circ v=v'$ il envoie $[\beta ;\gamma ]$ sur $u'(\beta )v'(\gamma )$, donc coïncide avec $f$.

D’après la formule (29), on a

$$
u'(\beta \alpha )v'(\iota (\alpha )^{-1}\gamma ) =u'(\beta )v'(\gamma ) \tag{31}
$$

pour $\alpha$ dans $L^*,\beta$ dans L et $\gamma$ dans Γ. Vu la définition de E, il existe donc une application $f_0: E\rightarrow B$ telle que $f_0([\beta ;\gamma ]) =u'(\beta )v'(\gamma )$. D’après les formules (23) et (30), on a $f_0(xx') =f_0(x)f_0(x')$ pour $x$ et $x'$ dans E. La restriction de $f_0$ à $E_g$ est K-linéaire pour tout élément $g$ de G ; par suite, il existe une application K-linéaire $f$ de $\mathbf{A}[\mathscr{E}; L]$ dans B et une seule, qui coïncide avec $f_0$ sur E. L’application $f$ est un morphisme d’algèbres qui vérifie $u'=f\circ u$ et $v'=f\circ v$.

#### Remarque {#alg-viii-s16-n9-rem-1 .statement tag=00JG}

Soit $\sigma : G\rightarrow \Gamma$ une section de l’application $\pi$. Posons $\varepsilon_g=v(\sigma (g))$ pour tout $g$ de G et notons $c_{\sigma}$ le 2-cocycle associé à $\sigma$ (VIII, p. 291). En particulier

$$
\varepsilon_g\varepsilon_{g'}=u(c_{\sigma}(g, g'))\varepsilon_{gg'} \tag{32}
$$

pour tous $g, g'\in G$. Identifions par ailleurs L à une sous-algèbre de $\mathbf{A}[\mathscr{E}; L]$ par l’homomorphisme $u$. Alors tout élément de $\mathbf{A}[\mathscr{E}; L]$ s’écrit de manière unique sous la forme $\sum_{g\in G}a_g\varepsilon_g$, où $(a_g)$ est une famille à support fini d’éléments de L. La multiplication dans $\mathbf{A}[\mathscr{E}; L]$ s’exprime par la formule

$$
(\sum_ga_g\varepsilon_g)((\sum_gb_g\varepsilon_g)=\sum_gd_g\varepsilon_g \tag{33}
$$

avec

$$
d_g=\sum_{hh'=g}a_h(\lambda (h).b_{h'})c_{\sigma}(h, h') \tag{34}
$$

Si l’extension $\mathscr{E}$ est semi-triviale, on peut choisir une section $\sigma$ de $\pi$ qui est un morphisme de groupes de G dans Γ ; le cocycle $c_{\sigma}$ est donc constant de valeur 1 et la formule (34) se simplifie alors en

$$
d_g=\sum_{hh'=g}a_h\lambda (h).b_{h'} \tag{35}
$$

Soit $K'$ une extension du corps K. Notons $L'$ la $K'$-algèbre $L_{(K')}$ et pour tout $g$ de G, notons $\lambda '(g)$ l’automorphisme$\lambda (g)_{(K')}$ induit par $\lambda (g)$ sur $L_{(K')}$. Notons également $\tau '(g)$ l’automorphisme de $L^{'*}$ induit par $\lambda '(g)$. Enfin, soit $h$ l’homomorphisme de $L^*$ dans $L^{'*}$ qui envoie $x$ sur $x\otimes 1$. Soit alors $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ l’image directe de l’extension $\mathscr{E}$ par $h$ (VIII, p. 285). Soit $\mathbf{A}[\mathscr{E}',L']$ la $K'$-algèbre produit croisé de $\mathscr{E}'$ par $L'$ et soient $u': L'\rightarrow \mathbf{A}[\mathscr{E}',L']$ et $v': \Gamma '\rightarrow \mathbf{A}[\mathscr{E}',L']^*$ les homomorphismes canoniques.

#### Proposition 13 {#alg-viii-s16-prop-13 .statement tag=00JH}

Il existe un isomorphisme de $K'$-algèbres $\varphi$ de $\mathbf{A}[\mathscr{E}; L]_{(K')}$ dans $\mathbf{A}[\mathscr{E}'; L']$, et un seul, qui satisfasse aux relations

$$
u'(h(\beta )) =\varphi (1\otimes u(\beta )) \tag{36}
$$

pour $\beta \in L$et (37) $v'(h(\gamma )) =\varphi (1\otimes v(\gamma ))$.

pour $\gamma \in \Gamma$.

La démonstration résulte aussitôt des constructions.

L’isomorphisme $\varphi$ sera dit canonique.

### 10. Application au groupe de Brauer

Dans ce numéro, on note K un corps, L une algèbre galoisienne sur K d’action $\lambda : G\rightarrow$ Aut$_K(L)$. On note $n$ le degré de L sur K. On a $n=$ Card(G).

#### Théorème 3 {#alg-viii-s16-thm-3 .statement tag=00JI}

Soit $\mathscr{E}= (\Gamma , \iota , \pi )$une $\tau$-extension de G par $L^*$. L’algèbre $\mathbf{A}[\mathscr{E}; L]$ est simple, centrale et de rang $n^2$ sur K. De plus, l’homomorphisme canonique $u$ de L dans $\mathbf{A}[\mathscr{E}; L]$est un isomorphisme de L sur une sous-algèbre commutative maximale de $\mathbf{A}[\mathscr{E}; L]$.

#### Lemme 12 {#alg-viii-s16-lem-12 .statement tag=00JJ}

a) Il n’existe aucun idéal de L, autre que $\{0\}$ et L, qui soit invariant par G.

b) Soit $g$ un élément de G distinct de l’élément neutre et soit $\mathfrak{a}_g$ l’idéal de L engendré par les éléments de la forme $x-\lambda (g)x$ où $x$ parcourt L. On a $\mathfrak{a}_g= L$.

Soit $\mathscr{S}$ l’ensemble des idéaux maximaux de L ; pour toute partie S de $\mathscr{S}$, posons $\mathfrak{a}(S) =\bigcap_{\mathfrak{m}\in S}\mathfrak{m}$. Comme l’anneau L est commutatif et semi-simple (VIII, p. 305, remarque 6), l’application $S\rightarrow \mathfrak{a}(S)$ est une bijection de l’ensemble des parties de $\mathscr{S}$ sur l’ensemble des idéaux de L (VIII, p. 137, prop. 9). L’idéal $\mathfrak{a}(S)$ est invariant sous G si et seulement si S l’est. Comme G agit de manière transitive sur $\mathscr{S}$ (VIII, p. 303, th. 2 vi)), les seules parties de $\mathscr{S}$ invariantes par G sont $\emptyset$ et $\mathscr{S}$. Comme $\mathfrak{a}(\emptyset ) = L$ et $\mathfrak{a}(\mathscr{S}) =\{0\}$, on a démontré l’assertion a).

Pour démontrer b), raisonnons par l’absurde en supposant qu’on ait $\mathfrak{a}_g\not= L$. Soit $\mathfrak{m}$ un idéal maximal de L contenant $\mathfrak{a}_g$. On a donc $\lambda (g)x\equiv x$ mod. $\mathfrak{m}$ pour tout $x$ de L. En particulier, $\mathfrak{m}$ est invariant par $g$ et $\lambda (g)$ induit l’identité sur le corps $L/\mathfrak{m}$. Par le th. 2, (vi) de VIII, p. 303, l’élément $g$ de $G_{\mathfrak{m}}$ est trivial ce qui contredit l’hypothèse de b).

Démontrons maintenant le théorème 3. L’espace vectoriel $\mathbf{A}[\mathscr{E}; L]$ est de dimension finie Card(G)[L$: K] =n^2$ sur K, d’après VIII, p. 311 et l’égalité Card(G) = $[L : K] =n$ faite en hypothèse.

Soit $\mathfrak{a}$ un idéal bilatère non nul de l’algèbre $\mathbf{A}[\mathscr{E}; L]$. Reprenons les notations de VIII, p. 311. Tout élément $a$ de $\mathbf{A}[\mathscr{E}; L]$ s’écrit de manière unique sous la forme $a=\sum_{g\in G}a_g\varepsilon_g$ avec $a_g\in L$ pour tout $g\in G$; on note $\Phi (a)$ l’ensemble des éléments $g$ de G tels que $a_g\not= 0$. D’après la formule (32) de VIII, p. 311, on a la relation

$$
\varepsilon_g\varepsilon_{g'}=c_{\sigma}(g, g')\varepsilon_{gg'} \tag{38}
$$

pour tous $g, g'\in G$ et par suite

$$
\Phi (a\varepsilon_g) = \Phi (a).g \tag{39}
$$

pour tout $g\in G$ et tout $a\in \mathbf{A}[\mathscr{E}; L]$.

Soit $a$ un élément non nul de $\mathfrak{a}$, pour lequel $\Phi (a)$ soit minimal pour l’inclusion ; d’après la formule (39), on peut supposer, quitte à remplacer $a$ par un élément de la forme $a\varepsilon_{g^{-1}}$, où $g\in \Phi (a)$, qu’on a $e\in \Phi (a)$. Soit $s$ un élément de $\Phi (a)$ distinct de $e$. D’après le lemme 12, b), il existe un élément $x$ de L tel que $a_s(x-\lambda (s).x)\not= 0$. Mais on a la relation

$$
xa-ax=\sum_ga_g(x-\lambda (g).x)\varepsilon_g \tag{40}
$$

la somme s’étendant sur les éléments $g$ de $\Phi (a)$ distincts de $e$. Vu le caractère minimal de $\Phi (a)$, on a donc $xa-ax= 0$, mais ceci contredit l’hypothèse faite sur $x$. On a donc prouvé par l’absurde que $\Phi (a)$ contient seulement l’unité $e$ de G, d’où $a\in L$.

Donc $L\cap \mathfrak{a}$ est un idéal de L non réduit à $\{0\}$. De plus, pour tout $x$ de L, on a $\varepsilon_gx\varepsilon^{-1}_g=\lambda (g).x$, donc $L\cap \mathfrak{a}$ est invariant par G. D’après le lemme 12, on a donc $L\cap \mathfrak{a}= L$, c’est-à-dire $L\subset \mathfrak{a}$. Comme L contient l’élément unité de $\mathbf{A}[\mathscr{E}; L]$, on a $\mathfrak{a}= \mathbf{A}[\mathscr{E}; L]$.

Comme l’algèbre $\mathbf{A}[\mathscr{E}; L]$ est de dimension finie non nulle sur K et qu’elle n’a d’autre idéal bilatère que $\{0\}$ et $\mathbf{A}[\mathscr{E}; L]$, elle est simple.

Démontrons que tout élément $a$ de $\mathbf{A}[\mathscr{E}; L]$ qui commute à L appartient à L. Écrivons $a$ sous la forme $\sum_{g\in G}a_g\varepsilon_g$ avec des coefficients $a_g$ dans L. Pour tout $x$ de L, on a $xa-ax= 0$ et la relation (40) montre qu’on a

$$
a_g(x-\lambda (g).x) = 0 \tag{41}
$$

quels que soient $g\in G$ et $x\in L$. D’après le lemme 12, on a donc $a_g= 0$ pour $g\not=e$; d’où $a\in L$.

Déterminons enfin le centre de $\mathbf{A}[\mathscr{E}; L]$. Si $z$ appartient au centre, il commute à L, donc appartient à L. Mais on a alors

$$
0 =\varepsilon_gz-z\varepsilon_g= (\lambda (g).z-z)\varepsilon_g
$$

pour tout $g$ de G. Donc $z$ est invariant par le groupe $\lambda (G)$ d’automorphismes de L. On a donc $z\in K$ par hypothèse.

#### Théorème 4 {#alg-viii-s16-thm-4 .statement tag=00JK}

Soit A une algèbre simple et centrale, de rang fini sur K et soit L une sous-algèbre commutative maximale de A. Alors il existe une $\tau$-extension $\mathscr{E}$ de G par $L^*$ telle que A soit isomorphe à $\mathbf{A}[\mathscr{E}; L]$.

On ne restreint pas la généralité en supposant que L est une sous-algèbre commutative maximale de A. Soit Γ le groupe multiplicatif formé des éléments inversibles $\gamma$ de A tels qu’il existe $g$ appartenant à G avec

$$
\gamma x\gamma^{-1}=\lambda (g).x \tag{42}
$$

pour tout élément $x$ de L. Si $\gamma \in \Gamma$ est donné, l’élément $g$ satisfaisant à cette relation est unique, on le note $\pi (\gamma )$; il est immédiat que $\pi$ est un homomorphisme de Γ dans G et que son noyau est égal à $L^*$. Que $\pi$ soit surjectif résulte du théorème de Skolem-Noether (VIII, p. 259, cor.).

Si l’on note $\iota$ l’injection canonique de $L^*$ dans Γ, il résulte des constructions que $\mathscr{E}= (\Gamma , \iota , \pi )$ est une $\tau$-extension de G par $L^*$. Soient

$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ et $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E}; L]$

les homomorphismes canoniques. D’après la propriété universelle de $\mathbf{A}[\mathscr{E}; L]$ (VIII, p. 310, prop. 12), il existe un unique homomorphisme d’algèbres $f: \mathbf{A}[\mathscr{E}; L]\rightarrow A$ tel que $f\circ u(x) =x$ et $f\circ v(\gamma ) =\gamma$ pour $x\in L$ et $\gamma \in \Gamma$. Comme l’algèbre $\mathbf{A}[\mathscr{E}; L]$ est simple, l’homomorphisme $f$ est injectif. Or l’algèbre $\mathbf{A}[\mathscr{E}; L]$ est de rang $n^2$ sur K et il en est de même de A, puisque L est une sous-algèbre semi-simple commutative maximale de A et qu’on a $n= [L : K]$ (VIII, p. 258, prop. 3, (ii)). Donc $f$ est bijectif.

#### Définition 2 {#alg-viii-s16-def-2 .statement tag=00JL}

Soit $\mathscr{S}$ l’ensemble des idéaux maximaux de L. On définit

Br(L$/K) =\bigcap_{\mathfrak{m}\in\mathscr{S}}$ Ker($r_{(L/\mathfrak{m})/K}$),

où $r_{(L/\mathfrak{m})/K}:$ Br(K) $\rightarrow$ Br(L$/\mathfrak{m})$est l’homomorphisme d’extension des scalaires (VIII, p. 277).

#### Théorème 5 {#alg-viii-s16-thm-5 .statement tag=00JM}

Il existe un isomorphisme de groupes

Ψ : Ex$_{\tau}(G,L^*)\longrightarrow$ Br(L$/K)$

qui à la classe de toute $\tau$-extension $\mathscr{E}$ de G par $L^*$ associe la classe dans Br(L$/K)$ de l’algèbre $\mathbf{A}[\mathscr{E}; L]$.

Pour définir Ψ et vérifier que c’est une bijection, il s’agit d’établir les points suivants :

a) Si $\mathscr{E}$ et $\mathscr{E}'$ sont des $\tau$-extensions isomorphes de G par $L^*$, les algèbres $\mathbf{A}[\mathscr{E}; L]$ et $\mathbf{A}[\mathscr{E}'; L]$ sont isomorphes ;

b) Réciproquement, si les algèbres $\mathbf{A}[\mathscr{E}; L]$ et $\mathbf{A}[\mathscr{E}'; L]$ sont isomorphes, les $\tau$-extensions $\mathscr{E}$ et $\mathscr{E}'$ de G par $L^*$ sont isomorphes ;

c) Dans toute classe appartenant à Br(L$/K)$, il y a une algèbre E contenant L comme sous-algèbre commutative maximale ;

d) Si E est une algèbre simple et centrale de rang fini sur K et contenant L comme sous-algèbre commutative maximale, alors il existe une $\tau$-extension $\mathscr{E}$ de G par $L^*$ telle que E soit isomorphe à $\mathbf{A}[\mathscr{E}; L]$.

La vérification de a) résulte de la construction du produit croisé ; celle de b) résulte de VIII, p. 259, cor. L’assertion c) résulte de la prop. 5 de VIII, p. 277 et l’assertion d) n’est autre que le th. 4 ci-dessus.

Il reste à vérifier que Ψ est un homomorphisme de groupes ; pour cela il suffit de démontrer que si $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ et $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ sont des $\tau$-extensions alors l’algèbre $\mathbf{A}[\mathscr{E}_1\mathscr{E}_2; L]$ est équivalente à l’algèbre $\mathbf{A}[\mathscr{E}_1; L]\otimes \mathbf{A}[\mathscr{E}_2; L]$. Notons $\mathscr{E}= (\Gamma , \iota , \pi )$ l’extension produit $\mathscr{E}_1\mathscr{E}_2$. Le groupe Γ est donc isomorphe au conoyau de l’homomorphisme $\rho$ de $L^*$ dans le produit fibré $\Gamma_1\times_G\Gamma_2$ qui envoie $\mu$ sur $(\iota_1(\mu ), \iota_2(\mu )^{-1})$. Pour $i\in  \{1,2\}$, notons $A_i= \mathbf{A}[\mathscr{E}_i; L]$. Soient $u_i: L\rightarrow A_i$ et $v_i: \Gamma_i\rightarrow A^*_i$ les homomorphismes canoniques et identifions L avec ses images par les homomorphismes $u_i$, ce qui fait de L une sous-algèbre commutative maximale de $A_i$. Notons $V_i$ le L-espace vectoriel défini par la multiplication à gauche dans $A_i$. L’anneau $L\otimes_KA^o_i$ opère sur $V_i$. Comme il est simple et de dimension $n^2$ sur L, on obtient un isomorphisme de $L\otimes_KA^o_i$ sur End$_L(V_i)$. Donc l’anneau $L\otimes_KA^o_1\otimes_KA^o_2$, qu’on peut identifier à $(L\otimes_KA^o_1)\otimes_L(L\otimes_KA^o_2)$ est isomorphe à End$_L(V_1\otimes_LV_2)$. Posons C = End$_{A^o_1\otimes_KA^o_2}(V_1\otimes_LV_2)$. Par le lemme 3 de VIII, p. 277, C est semblable à $A_1\otimes_KA_2$ et $L\otimes 1\otimes 1$ est une sous-algèbre commutative maximale de C. Pour tout couple $(\gamma_1, \gamma_2)\in \Gamma_1\times \Gamma_2$ vérifiant $\pi_1(\gamma_1) =\pi_2(\gamma_2)$, notons $w(\gamma_1, \gamma_2)$ l’unique endomorphisme $\lambda (\pi_1(\gamma_1$))-semi-linéaire (II, p. 32) tel que

$$
w(\gamma_1, \gamma_2)(x_1\otimes x_2) =v_1(\gamma_1)x_1\otimes v_2(\gamma_2)x_2
$$

pour $x_1\in V_1$ et $x_2\in V_2$. On a $w(\gamma_1, \gamma_2)\in C^*$ et $w$ est un homomorphisme de groupes du produit fibré $\Gamma_1\times_G\Gamma_2$ dans $C^*$. Cet homomorphisme est trivial sur l’image de $\rho$ et induit un homomorphisme $v$ de Γ dans $C^*$. Notons $u: L\rightarrow C$ le morphisme donné par $u:l\rightarrow l\otimes 1\otimes 1$. On vérifie alors les relations

$u(\alpha ) =v(\iota (\alpha ))$ et $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$

pour $\alpha \in L^*,\beta \in L$ et $\gamma \in \Gamma$. La proposition 12 de VIII, p. 310 fournit un homomorphisme $f$ de l’algèbre $\mathbf{A}[\mathscr{E}; L]$ dans C. Comme l’algèbre $\mathbf{A}[\mathscr{E}; L]$ est simple, l’homomorphisme $f$ est injectif. Les algèbres C et $\mathbf{A}[\mathscr{E}; L]$ ayant la même dimension sur $K,f$ est un isomorphisme.

#### Remarque 1 {#alg-viii-s16-n10-rem-1 .statement tag=00JN}

Si L est une algèbre étale sur K et G le groupe des automorphismes de L, il n’est pas toujours vrai que l’algèbre $\mathbf{A}[\mathscr{E}; L]$ soit simple et centrale (par exemple, on peut prendre $L = K^n$ et $G =\mathfrak{S}_n)$.

#### Remarque 2 {#alg-viii-s16-n10-rem-2 .statement tag=00JO}

On peut calculer comme suit un 2-cocycle $c$ associé à une algèbre A déployée par une extension galoisienne finie L de groupe G. Tout d’abord, il existe un K-homomorphisme $\varphi : A\rightarrow \mathbf{M}_m$(L), où $[A : K] =m^2$. Pour $g\in G$, soit $\varphi^g$ l’homomorphisme de A dans $\mathbf{M}_m(L)$ donné par $a\rightarrow \varphi (g^{-1}ag)$. D’après le théorème de Skolem-Noether, il existe, pour tout $g\in G$, un élément $u_g$ de $\mathbf{G}\mathbf{L}_m(L)$ tels que

$$
\varphi^g(a) =u_g\varphi (a)u^{-1}_g
$$

pour $a\in A$. On pose ensuite

$$
c(g, g') =u_gu_{g'}u^{-1}_{gg'}
$$

On peut également définir une extension de G par $L^*$ au moyen de $\varphi :$ on considère le groupe $\Gamma \subset \mathbf{G}\mathbf{L}_m(L)$ formé des $\gamma$ pour lesquels il existe $g\in G$ avec

$$
\varphi^g(a) =\gamma \varphi (a)\gamma^{-1}
$$

pour tout $a\in A$. La classe de cette extension est l’image inverse par Ψ de la classe de A dans Br(L$/K)$.

#### Corollaire {#alg-viii-s16-n10-cor-1 .statement tag=00JP}

L’application $\Phi_{L/K}= \Theta \circ \Psi^{-1}$ définit un isomorphisme de groupes de Br(L$/K)$sur $H^2(G,L^*)$.

Soient $K'$ une extension de K et $\varphi : K'\rightarrow L$ un morphisme de K-algèbres. L’ensemble H des éléments $h$ de G tels que $\lambda (h)\circ \varphi =\varphi$ est un sous-groupe de G et la $K'$-algèbre-L munie de la restriction de $\lambda$ à H est une algèbre galoisienne sur $K'$.

#### Proposition 14 {#alg-viii-s16-prop-14 .statement tag=00JQ}

Le diagramme

Br(L$/K)^{\Phi_{L/K}}/$/ $H^2(G,L^*)$

$r_{K'/K}$ Res$^G_H$

Br(L$/K')^{\Phi_{L/K'}}/$/ $H^2(H,L^*)$

est commutatif

Cela resulte de la prop. 7 de VIII, p. 295 et de la prop. 13 de VIII, p. 311.

### 11. Indice et exposant

#### Théorème 6 {#alg-viii-s16-thm-6 .statement tag=00JR}

Soit K un corps commutatif et soit A une algèbre centrale, simple et de degré fini sur K. Soit L une extension séparable de degré fini de K qui déploie l’algèbre A. Alors [L : K][A] est nul dans Br(K).

Il existe une extension M de L qui est une extension galoisienne de degré fini de K (V, p. 55, prop. 2). La classe [A] de A dans le groupe de Brauer de K appartient au sous-groupe Br(M$/K)$. Soit G le groupe de Galois de M sur K et soit $\alpha$ l’image de [A] dans $H^2(G,M^*)$ (VIII, p. 316, cor.). Soit H le groupe de Galois de M sur L. Alors H est un sous-groupe d’indice [L : K] dans G (V, p. 66, cor. 5). Comme Res$^G_H(\alpha ) = \Phi_{M/L}(A_{(L)})$ (prop. 14), on a Res$^G_H(\alpha ) = 0$. Par la prop. 8 de VIII, p. 298, on en déduit que $[L : K]\alpha = 0$, puis [L : K][A] = 0.

Soit K un corps commutatif et soit A une algèbre centrale, simple et de degré fini sur K. Alors A est isomorphe à une algèbre de la forme $\mathbf{M}_n$(D), où D est un corps de centre K et [A] = [D] dans Br(K). Le degré réduit de D ne dépend que de A. On appelle indice de A ce degré réduit. L’indice de A divise donc le degré réduit de A. On appelle exposant de A l’ordre de la classe de A dans le groupe de Brauer de K.

#### Corollaire 1 {#alg-viii-s16-thm-6-cor-1 .statement tag=00JS}

L’exposant d’une algèbre centrale simple et de degré fini sur un corps commutatif divise son indice.

Il suffit de le démontrer pour un corps D de degré fini sur son centre K. Soit L un sous-corps commutatif maximal de D qui est une extension séparable de K ; on a $[D : K] = [L : K]^2$ (VIII, p. 261, cor. 2, b) et c)). Alors l’extension L de K déploie l’algèbre D (VIII, p. 277, prop. 5) et [L : K] coïncide avec le degré réduit de D. On applique alors le théorème 6.

#### Corollaire 2 {#alg-viii-s16-thm-6-cor-2 .statement tag=00JT}

Soit K un corps commutatif et soit A une algèbre centrale, simple et de degré fini sur K. Soit $p$ un nombre premier. Si $p$ divise l’indice de A, alors il divise l’exposant de A.

Supposons que le nombre premier $p$ ne divise pas l’exposant de A et démontrons qu’il ne divise pas son indice. Il suffit de démontrer ce résultat dans le cas où A est un corps. Soit L une extension galoisienne de degré fini de K qui déploie A. Soit G le groupe de Galois de L sur K et soit H un $p$-sous-groupe de Sylow de G (I, p. 74). On note $L'= L^H$ le sous-corps de L des invariants de H. L’exposant de $A_{(L')}$ divise celui de A donc est premier à $p$. Par le théorème 6, on a que $[L : L'][A_{(L')}] = 0$ dans le groupe de Brauer de $L'$. Il en résulte que $[A_{(L')}] = 0$ et que le corps $L'$ déploie A. On applique alors le cor. 2 de VIII, p. 278 ; il en résulte que l’indice de A divise $[L': K]$ et n’est donc pas divisible par $p$.

#### Corollaire 3 {#alg-viii-s16-thm-6-cor-3 .statement tag=00JU}

Soit K un corps parfait de caractéristique $p$ et soit A une algèbre centrale et simple de degré fini sur K, alors $p$ ne divise pas l’indice de A.

Il suffit de traiter le cas où $p$ est strictement positif.

Démontrons dans ce cas que le groupe de Brauer de K ne contient pas d’élément d’ordre $p$. Pour toute extension M galoisienne de degré fini sur K, le corps M est parfait (V, p. 35, prop. 2). Donc l’élévation à la puissance $p$ est un automorphisme du groupe $M^*$. Il en résulte que la multiplication par $p$ est un automorphisme du groupe $H^2$(Gal(M$/K),M^*)$ qui est isomorphe à Br(M$/K)$.

Par conséquent, l’ordre de [A] est premier à $p$ et, par le corollaire 2, son indice n’est pas divisible par $p$.

#### Remarque {#alg-viii-s16-n11-rem-1 .statement tag=00JV}

En considérant des produits tensoriels d’algèbres de quaternions, il est possible de construire des corps de centre K d’exposant 2 et d’indice arbitrairement grand (cf. VIII, p. 363, exercices 7 et 8).

$*$Par contre, si K est une extension finie d’un corps $p$-adique ou un corps de

série formelle sur un corps fini, alors l’exposant d’une algèbre centrale simple et de degré fini sur K est égal à son indice (VIII, p. 327, exerc. 17, e)).$*$

## EXERCICES {#alg-viii-s16-exercises}

See the [exercises for § 16](exercises/s16/).
