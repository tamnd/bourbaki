---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 2
section_title: Tores maximaux des groupes de Lie compacts
lang: fr
source: lie-ix-fr
book_pages: LIE IX.7-LIE IX.15, LIE IX.108-LIE IX.110
pdf_pages: 0010-0018, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Sous-algèbres de Cartan des algèbres compactes
      page: 7
      pdf_page: 10
    - "no": 2
      title: Tores maximaux
      page: 8
      pdf_page: 11
    - "no": 3
      title: Tores maximaux des sous-groupes et des groupes quotients
      page: 11
      pdf_page: 14
    - "no": 4
      title: Sous-groupes de rang maximum
      page: 12
      pdf_page: 15
    - "no": 5
      title: Le groupe de Weyl
      page: 13
      pdf_page: 16
    - "no": 6
      title: Tores maximaux et relèvement d’homomorphismes
      page: 15
      pdf_page: 18
statements: 33
exercises: 11
content_sha256: 31be9da97c8052633252671d3863584cd62d0e193e2f78b07f66cb5ff204ffd3
---

## § 2. TORES MAXIMAUX DES GROUPES DE LIE COMPACTS

### 1. Sous-algèbres de Cartan des algèbres compactes

#### Lemme 1 {#lie-ix-s2-lem-1 .statement tag=019Z}

Soient G un groupe de Lie, K un sous-groupe compact de G, et F une forme bilinéaire invariante sur L(G). Soient x, y ∈ L(G). Il existe un élément k de K tel que pour tout u ∈ L(K), on ait F(u, [(Ad k)(x), y]) = 0.

La fonction v ↦ F((Ad v)(x), y) de K dans R est continue, donc possède un minimum en un point k ∈ K. Soit u ∈ L(K) et posons

$$
h(t) = F((\mathrm{Ad}\exp(tu).k)(x), y), \quad t \in \mathbf{R}.
$$

On a h(t) ≥ h(0) pour tout t ; par ailleurs, d’après III, § 3, n° 12, prop. 44, on a

$$
\frac{dh}{dt}(0) = F([u, (\mathrm{Ad}\ k)(x)], y) = F(u, [(Ad\ k)(x), y]),
$$

d’où le lemme (FVR, I, p. 20, prop. 7).

#### Théorème 1 {#lie-ix-s2-thm-1 .statement tag=01A0}

Soit g une algèbre de Lie compacte. Les sous-algèbres de Cartan de g (VII, § 2, n° 1, déf. 1) sont ses sous-algèbres commutatives maximales ; en particulier, g est la réunion de ses sous-algèbres de Cartan. Le groupe Int(g) opère transitivement sur l’ensemble des sous-algèbres de Cartan de g.

Comme g est réductive, ses sous-algèbres de Cartan sont commutatives (VII, § 2, n° 4, cor. 3 au th. 2). Inversement, soit t une sous-algèbre commutative de g. D’après § 1, n° 3, prop. 1, ad x est semi-simple pour tout x ∈ t ; d’après VII, § 2, n° 3, prop. 10, il existe une sous-algèbre de Cartan de g contenant t. Cela démontre la première assertion du théorème.

Soient maintenant t et t’ deux sous-algèbres de Cartan de g. Prouvons qu’il existe u ∈ Int(g) tel que u(t) = t’. D’après la prop. 1 du § 1, n° 3, on peut supposer que g est de la forme L(G), où G est un groupe de Lie compact connexe, et choisir une forme bilinéaire symétrique invariante séparante F sur g. Soit x (resp. x’) un élément régulier de g tel que t = g^0(x) (resp. t’ = g^0(x’)) (VII, § 3, n° 3, th. 2). Appliquant le lemme 1 avec K = G, on voit qu’il existe k ∈ G tel que [(Ad k)(x), x’] soit orthogonal à g pour F, donc nul ; on a alors (Ad k)(x) ∈ g^0(x’) = t’, donc g^0((Ad k)(x)) = t’ puisque (Ad k)(x) est régulier. On en conclut que (Ad k)(t) = t’, d’où le théorème.

#### Corollaire {#lie-ix-s2-n1-cor-1 .statement tag=01A1}

Soient t et t’ deux sous-algèbres de Cartan de g, a une partie de t, et u un automorphisme de g qui applique a dans t’. Il existe un élément v de Int(g) tel que u ∘ v applique t sur t’, et coïncide avec u sur a.

Posons G = Int(g), et considérons le fixateur Z_G(a) de a dans G ; c’est un sous-groupe de Lie de G, dont l’algèbre de Lie z_g(a) est formée des éléments de g qui commutent à tous les éléments de a (III, § 9, n° 3, prop. 7). Alors t et u^{-1}(t’) sont deux sous-algèbres de Cartan de l’algèbre de Lie compacte z_g(a). D’après le th. 1, il existe un élément v de Z_G(a) tel que v(t) = u^{-1}(t’) ; un tel élément répond à la question.

### 2. Tores maximaux

Soit G un groupe de Lie. On appelle tore de G tout sous-groupe fermé qui est un tore (§ 1, n° 2), c’est-à-dire tout sous-groupe compact connexe commutatif. Les éléments maximaux de l’ensemble ordonné par inclusion des tores de G sont appelés les tores maximaux de G.

#### Théorème 2 {#lie-ix-s2-thm-2 .statement tag=01A2}

Soit G un groupe ae Lie compact connexe.
a) Les algèbres de Lie des tores maximaux de G sont les sous-algèbres de Cartan de L(G).
b) Soient T_1 et T_2 deux tores maximaux de G. Il existe g ∈ G tel que T_2 = gT_1g^{-1}.
c) G est la réunion de ses tores maximaux.

Soit t une sous-algèbre de Cartan de L(G) ; le sous-groupe intégral de G d’algèbre de Lie t est fermé (VII, § 2, n° 1, cor. 4 à la prop. 4) et commutatif (th. 1), donc est un tore de G. Si T est un tore maximal de G, son algèbre de Lie est commutative, donc contenue dans une sous-algèbre de Cartan de $L(G)$ (th. 1). Il en résulte que les tores maximaux de $G$ sont exactement les sous-groupes intégraux de $G$ associés aux sous-algèbres de Cartan de $G$, d'où $a$. L’assertion $b$ résulte alors du th. 1, puisque l’homomorphisme canonique $G \to \operatorname{Int}(L(G))$ est surjectif (III, § 6, no 4, cor. 4 à la prop. 10).

Notons $X$ la réunion des tores maximaux de $G$, et soit $T$ un tore maximal de $G$. L’application continue $(g, t) \mapsto gtg^{-1}$ de $G \times T$ dans $G$ a pour image $X$, qui est donc fermé dans $G$; pour démontrer $c$, il suffit donc de prouver que $X$ est ouvert dans $G$; comme $X$ est invariant par automorphismes intérieurs, il suffit de montrer que pour tout $a \in T$, $X$ est un voisinage de $a$. Raisonnons par récurrence sur la dimension de $G$ et distinguons deux cas :

1) $a$ n’est pas central dans $G$. Soit alors $H$ la composante neutre du centralisateur de $a$ dans $G$; c’est un sous-groupe compact connexe de $G$ distinct de $G$, qui contient $T$, donc $a$. Comme $\operatorname{Ad}\,a$ est semi-simple ($§ 1$, no 1 ), l’algèbre de Lie de $H$ est le nilspace de $\operatorname{Ad}\,a - 1$; il résulte alors de VII, § 4, no 2, prop. 4, que la réunion $Y$ des conjugués de $H$ est un voisinage de $a$. D’après l’hypothèse de récurrence, on a $H \subset X$, donc $Y \subset X$; ainsi $X$ est un voisinage de $a$.

2) $a$ est central dans $G$. Il suffit de prouver que $a \exp x$ appartient à $X$ pour tout $x$ dans $L(G)$. Or tout élément $x$ de $L(G)$ appartient à une sous-algèbre de Cartan de $G$ (th. 1); le sous-groupe intégral $T'$ correspondant contient $\exp x$; comme il est conjugué à $T$, il contient $a$ et donc $a \exp x$, d’où l’assertion cherchée.

#### Corollaire 1 {#lie-ix-s2-thm-2-cor-1 .statement tag=01A3}

a) *L’application exponentielle de $G$ est surjective*.

b) *Pour tout $n \geqslant 1$, l’application $g \mapsto g^n$ de $G$ dans lui-même est surjective*.

En effet, $\exp(L(G))$ contient tous les tores maximaux de $G$, d’où $a$. L’assertion $b$ résulte alors de la formule $(\exp x)^n = \exp nx$ pour $x$ dans $L(G)$.

#### Remarque 1 {#lie-ix-s2-n2-rem-1 .statement tag=01A4}

Il existe une partie *compacte* $K$ de $L(G)$ telle que $\exp_G(K) = G$. En effet, si $T$ est un tore maximal de $G$, il existe un compact $C \subset L(T)$ tel que $\exp_T(C) = T$; il suffit de prendre $K = \bigcup_{g \in G} (\operatorname{Ad}\,g)(C)$.

#### Corollaire 2 {#lie-ix-s2-thm-2-cor-2 .statement tag=01A5}

*L’intersection des tores maximaux de $G$ est le centre de $G$*.

Soit $x$ un élément du centre de $G$; d’après le th. 2, $c$), il existe un tore maximal $T$ de $G$ contenant $x$; alors $x$ appartient à tous les conjugués de $T$, donc à tous les tores maximaux de $G$. Inversement, si $x$ appartient à tous les tores maximaux de $G$, il commute à tout élément de $G$ d’après le th. 2, $c$).

#### Corollaire 3 {#lie-ix-s2-thm-2-cor-3 .statement tag=01A6}

*Soit $g \in G$, et soit $C$ son centralisateur. Alors $g$ appartient à $C_0$; le groupe $C_0$ est la réunion des tores maximaux de $G$ contenant $g$*.

Il existe un tore maximal $T$ de $G$ contenant $g$ (th. 2, $c$), et donc contenu dans $C_0$. Par ailleurs, le groupe $C_0$ est un groupe de Lie compact connexe, donc réunion de ses tores maximaux (th. 2, $c$); ceux-ci contiennent tous $g$ (cor. 2), donc sont exactement les tores maximaux de $G$ contenant $g$.

#### Corollaire 4 {#lie-ix-s2-thm-2-cor-4 .statement tag=01A7}

Soit $g \in G$. Si $g$ est régulier (VII, § 4, n° 2, déf. 2), il appartient à un seul tore maximal, qui est la composante neutre de son centralisateur. Sinon, il appartient à une infinité de tores maximaux.

Comme $\mathrm{Ad}\,g$ est semi-simple, la dimension du nilspace de $\mathrm{Ad}\,g - 1$ est aussi celle du centralisateur $C$ de $g$. D’après loc. cit., prop. 8, et le th. 1, $g$ est régulier si et seulement si $C_0$ est un tore maximal de $G$. On conclut alors par le cor. 3.

#### Corollaire 5 {#lie-ix-s2-thm-2-cor-5 .statement tag=01A8}

a) Soit $S$ un tore de $G$. Le centralisateur de $S$ est connexe ; c’est la réunion des tores maximaux de $G$ contenant $S$.

b) Soit $s$ une sous-algèbre commutative de $L(G)$. Le fixateur de $s$ dans $G$ est connexe ; c’est la réunion des tores maximaux de $G$ dont l’algèbre de Lie contient $s$.

Pour démontrer a), il suffit de prouver que si un élément $g$ de $G$ centralise $S$, il existe un tore maximal de $G$ contenant $S$ et $g$. Or, si $C$ est le centralisateur de $g$, on a $g \in C_0$ (cor. 3) et $S \subset C_0$; si $T$ est un tore maximal du groupe de Lie compact connexe $C_0$ contenant $S$, on a $g \in T$ (cor. 2), d’où a). L’assertion b) résulte de a) appliqué à l’adhérence du sous-groupe intégral d’algèbre de Lie $s$, compte tenu de III, § 9, n° 3, prop. 9.

#### Remarque 2 {#lie-ix-s2-n2-rem-2 .statement tag=01A9}

Il résulte du cor. 5 qu’un tore maximal de $G$ en est un sous-groupe commutatif maximal. La réciproque n’est pas vraie : par exemple, dans le groupe $SO(3, \mathbf{R})$, les tores maximaux sont de dimension 1, et ne peuvent donc contenir le sous-groupe des matrices diagonales, qui est isomorphe à $(\mathbf{Z}/2\mathbf{Z})^2$. Par ailleurs, si $g \in SO(3, \mathbf{R})$ est une matrice diagonale non scalaire, $g$ est un élément régulier de $SO(3, \mathbf{R})$ dont le centralisateur n’est pas connexe (cf. cor. 4).

#### Corollaire 6 {#lie-ix-s2-thm-2-cor-6 .statement tag=01AA}

Les tores maximaux de $G$ sont leurs propres centralisateurs, et sont les fixateurs de leurs algèbres de Lie.

Soient $T$ un tore maximal de $G$ et $C$ son centralisateur ; comme $L(T)$ est une sous-algèbre de Cartan de $L(G)$, on a $L(T) = L(C)$, donc $C = T$ puisque $C$ est connexe (cor. 5).

#### Corollaire 7 {#lie-ix-s2-thm-2-cor-7 .statement tag=01AB}

Soient $T$ et $T'$ deux tores maximaux de $G$, $A$ une partie de $T$ et $s$ un automorphisme de $G$ qui applique $A$ dans $T'$. Il existe $g \in G$ tel que $s \circ (\mathrm{Int}\,g)$ applique $T$ sur $T'$ et coïncide avec $s$ sur $A$.

Soit $C$ le centralisateur de $A$. Alors $T$ et $s^{-1}(T')$ sont deux tores maximaux de $C_0$; tout élément $g$ de $C_0$ tel que $(\mathrm{Int}\,g)(T) = s^{-1}(T')$ répond à la question.

#### Corollaire 8 {#lie-ix-s2-thm-2-cor-8 .statement tag=01AC}

Soient $H$ un groupe de Lie compact, $T$ un tore maximal de $H$. On a alors $H = N_H(T).H_0$, et l’injection de $N_H(T)$ dans $H$ induit un isomorphisme de $N_H(T)/N_{H_0}(T)$ sur $H/H_0$.

Soit $h \in H$. Alors $h^{-1}Th$ est un tore maximal de $H_0$, donc (th. 2) il existe $g \in H_0$ tel que $hg \in N_H(T)$; ainsi $h$ appartient à $N_H(T).H_0$, d’où la première assertion. La seconde en résulte immédiatement.

#### Remarque 3 {#lie-ix-s2-n2-rem-3 .statement tag=01AD}

Soit G un groupe de Lie connexe d’algèbre de Lie compacte. Appelons sous-groupes de Cartan de G les sous-groupes intégraux dont les algèbres de Lie sont les sous-algèbres de Cartan de L(G) (les sous-groupes de Cartan d’un groupe compact connexe sont donc ses tores maximaux). Le théorème 2 et ses corollaires sont encore valides pour G, en y remplaçant partout l’expression « tore maximal » par « sous-groupe de Cartan ». Cela résulte aussitôt du fait qu’en vertu de la prop. 5 du § 1, n° 4, G est le produit direct d’un groupe vectoriel V par un groupe compact connexe K et que les sous-groupes de Cartan de G sont les produits de V par les tores maximaux de K. Notons d’ailleurs qu’il résulte alors du cor. 6 ci-dessus qu’on peut aussi définir les sous-groupes de Cartan de G comme les fixateurs des sous-algèbres de Cartan de L(G).

#### Remarque 4 {#lie-ix-s2-n2-rem-4 .statement}

On peut aussi démontrer la partie c) du théorème 2 de la façon suivante. Munissons G d’une métrique riemannienne invariante (§ 1, n° 3, prop. 3). Alors, pour tout élément g de G, il existe une géodésique maximale passant par g et l’élément neutre de G (théorème de Hopf-Rinow), et on vérifie que l’adhérence d’une telle géodésique est un sous-tore de G. \*

### 3. Tores maximaux des sous-groupes et des groupes quotients

#### Proposition 1 {#lie-ix-s2-prop-1 .statement tag=01AE}

Soient G et G’ deux groupes de Lie compacts connexes.

a) Soit f : G → G’ un morphisme surjectif de groupes de Lie. Les tores maximaux de G’ sont les images par f des tores maximaux de G. Si le noyau de f est central dans G (par exemple discret), les tores maximaux de G sont les images réciproques par f des tores maximaux de G’.

b) Soit H un sous-groupe fermé connexe de G. Tout tore maximal de H est l’intersection avec H d’un tore maximal de G.

c) Soit H un sous-groupe fermé connexe distingué de G. Les tores maximaux de H sont les intersections avec H des tores maximaux de G.

a) Soit T un tore maximal de G ; alors L(T) est une sous-algèbre de Cartan de L(G) (n° 2, th. 2, a)), donc L(f(T)) une sous-algèbre de Cartan de L(G’) (VII, § 2, n° 1, cor. 2 à la prop. 4) ; il en résulte que f(T) est un tore maximal de G’ (n° 2, th. 2, a)). Si Ker f est central dans G, il est contenu dans T (cor. 2 au th. 2), donc T = f^{-1}(f(T)).

Inversement, soit T’ un tore maximal de G’ ; montrons qu’il existe un tore maximal T de G tel que f(T) = T’. Soit T_1 un tore maximal de G ; alors f(T_1) est un tore maximal de G’ et il existe g’ ∈ G’ tel que T’ = g’f(T_1) g’^{-1} (th. 2, b)) ; si g ∈ G est tel que f(g) = g’, on a T’ = f(T), avec T = gT_1g^{-1}.

b) Soit S un tore maximal de H ; c’est un tore de G et il existe donc un tore maximal T de G contenant S. Alors T ∩ H est un sous-groupe commutatif de H contenant S, donc égal à S (n° 2, remarque 2).

c) D’après § 1, n° 3, prop. 2, c), L(G) est produit direct de L(H) par un idéal ; les sous-algèbres de Cartan de L(H) sont donc les intersections avec L(H) des sous-algèbres de Cartan de L(G). Pour tout tore maximal T de G, T ∩ H contient donc un tore maximal S de H et on a S = T ∩ H (n° 2, remarque 2).

#### Remarque 1 {#lie-ix-s2-n3-rem-1 .statement tag=01AF}

La proposition 1 se généralise aussitôt aux groupes connexes à algèbre de Lie compacte. En particulier, si G est un groupe de Lie connexe dont l’algèbre de Lie est compacte, les sous-groupes de Cartan de G (cf. remarque 3, n° 2) ne sont autres que les images réciproques des tores maximaux du groupe de Lie compact connexe Ad(G) (par l’homomorphisme canonique de G sur Ad(G)).

#### Remarque 2 {#lie-ix-s2-n3-rem-2 .statement tag=01AG}

Soient G un groupe de Lie compact connexe, $\tilde{D}(G)$ le revêtement universel du groupe $D(G)$ et $f : \tilde{D}(G) \to G$ le morphisme composé des morphismes canoniques de $\tilde{D}(G)$ sur $D(G)$ et de $D(G)$ dans G. Alors l’application $T \mapsto f^{-1}(T)$ est une bijection de l’ensemble des tores maximaux de G sur l’ensemble des tores maximaux de $\tilde{D}(G)$; la bijection réciproque associe au tore maximal $\tilde{T}$ de $\tilde{D}(G)$ le tore maximal $C(G)_0 . f(\tilde{T})$ de G.

### 4. Sous-groupes de rang maximum

Nous appellerons rang d’un groupe de Lie connexe G et noterons rg G, le rang de son algèbre de Lie. D’après le th. 2, a), le rang d’un groupe de Lie compact connexe est la dimension commune de ses tores maximaux.

Soient G un groupe de Lie compact connexe et H un sous-groupe fermé de G. Si H est connexe, on a $\mathrm{rg}\ H \leq \mathrm{rg}\ G$ (puisque les tores maximaux de H sont des tores de G). D’après le th. 2, c), dire que H est connexe et de rang maximum (c’est-à-dire de rang $\mathrm{rg}\ G$) signifie que H est réunion de tores maximaux de G. On déduit alors aussitôt de la proposition 1 :

#### Proposition 2 {#lie-ix-s2-prop-2 .statement tag=01AH}

Soit $f : G \to G'$ un morphisme surjectif de groupes de Lie compacts connexes dont le noyau est central. Les applications $H \mapsto f(H)$ et $H' \mapsto f^{-1}(H')$ sont des bijections réciproques l’une de l’autre entre l’ensemble des sous-groupes fermés connexes de rang maximum de G et l’ensemble analogue pour $G'$.

#### Proposition 3 {#lie-ix-s2-prop-3 .statement tag=01AI}

Soient G un groupe de Lie compact connexe, et H un sous-groupe fermé connexe de rang maximum.

a) La variété compacte $G/H$ est simplement connexe.

b) L’homomorphisme $\pi_1(H) \to \pi_1(G)$, déduit de l’injection canonique de H dans G, est surjectif.

Comme H est connexe, on a une suite exacte (TG, XI, à paraître)

$$
\pi_1(H) \to \pi_1(G) \to \pi_1(G/H, \overline{e}) \to 0
$$

où $\overline{e}$ est l’image dans $G/H$ de l’élément neutre de G. Comme $G/H$ est connexe, cela entraîne aussitôt l’équivalence des assertions a) et b). Par ailleurs, si $f : G' \to G$ est un morphisme surjectif de groupes de Lie compacts connexes dont le noyau est central, il revient au même de démontrer la proposition (sous la forme a)) pour G ou pour $G'$ (prop. 2). On peut donc d’abord remplacer G par $\mathrm{Ad}(G)$, donc supposer G semi-simple, puis remplacer G par un revêtement universel (§ 1, n° 4, cor. 2), donc supposer G simplement connexe. Mais alors l’assertion b) est triviale.

#### Proposition 4 {#lie-ix-s2-prop-4 .statement tag=01AJ}

Soient G un groupe de Lie compact, H un sous-groupe fermé connexe de G de rang maximum et N le normalisateur de H dans G. Alors H est d’indice fini dans N et est la composante neutre de N.

En effet, l’algèbre de Lie de H contient une sous-algèbre de Cartan de L(G). D’après VII, § 2, n° 1, cor. 4 à la prop. 4, H est donc la composante neutre de N. Puisque N est compact, H est d’indice fini dans N.

#### Remarque 1 {#lie-ix-s2-n4-rem-1 .statement tag=01AK}

Tout sous-groupe intégral H de G tel que rg H = rg G est fermé : en effet, la démonstration précédente montre que H est la composante neutre de son normalisateur, qui est un sous-groupe fermé de G.

#### Remarque 2 {#lie-ix-s2-n4-rem-2 .statement tag=01AL}

Avec les notations de la prop. 4, tout sous-groupe fermé H′ de G contenant H et tel que (H′ : H) soit fini normalise H, donc est contenu dans N ; de même le normalisateur de H′ est contenu dans N. En particulier, N est son propre normalisateur.

### 5. Le groupe de Weyl

Soient G un groupe de Lie compact connexe et T un tore maximal de G. Notons N_G(T) le normalisateur de T dans G ; d’après la prop. 4 (n° 4), le groupe quotient N_G(T)/T est fini. On le note W_G(T) ou W(T) et on l’appelle le groupe de Weyl du tore maximal T de G, ou le groupe de Weyl de G relativement à T. Puisque T est commutatif, l’opération de N_G(T) sur T déduite des automorphismes intérieurs de G induit par passage au quotient une opération, dite canonique, du groupe W_G(T) sur le groupe de Lie T. D’après le cor. 6 au th. 2 du n° 2, cette opération est fidèle : l’homomorphisme W_G(T) → Aut T qui lui est associé est injectif.

Si T′ est un autre tore maximal de G et si g ∈ G est tel que Int g applique T sur T′ (n° 2, th. 2, b)), on déduit de Int g un isomorphisme a_g de W_G(T) sur W_G(T′) et on a a_g(s)(gtg^{-1}) = gs(t)g^{-1} pour tout s ∈ W_G(T) et tout t ∈ T.

#### Proposition 5 {#lie-ix-s2-prop-5 .statement tag=01J9}

a) Toute classe de conjugaison dans G rencontre T.

b) Les traces sur T des classes de conjugaison de G sont les orbites du groupe de Weyl.

Soit g ∈ G ; d’après le th. 2 du n° 2, il existe h ∈ G tel que g ∈ hTh^{-1}, d’où a). Par définition du groupe de Weyl, deux éléments d’une même orbite de W_G(T) dans T sont conjugués dans G ; inversement, soient a, b deux éléments de T conjugués dans G. Il existe h ∈ G tel que b = hah^{-1} ; appliquant le cor. 7 au th. 2 (n° 2) avec A = {a}, s = Int h, T′ = T, on voit qu’il existe g ∈ G tel que Int hg applique T dans T et a sur b. La classe de hg dans W_G(T) applique alors a sur b, d’où la proposition.

#### Corollaire 1 {#lie-ix-s2-prop-5-cor-1 .statement tag=01JA}

L’injection canonique de T dans G définit par passage au quotient un homéomorphisme de T/W_G(T) sur l’espace G/Int(G) des classes de conjugaison de G.

En effet, c’est une application continue et bijective entre deux espaces compacts (cf. TG, III, p. 29, cor. 1).

#### Corollaire 2 {#lie-ix-s2-prop-5-cor-2 .statement tag=01JB}

Soit E une partie de G stable par les automorphismes intérieurs. Pour que E soit ouverte (resp. fermée, resp. dense) dans G, il faut et il suffit que E ∩ T soit ouverte (resp. fermée, resp. dense) dans T.
Cela résulte du cor. 1 et de ce que les applications canoniques T → T/W_G(T) et G → G/Int(G) sont ouvertes (TG, III, p. 10, lemme 2).

Notons g l’algèbre de Lie de G, et t celle de T. On déduit de l’opération de W_G(T) dans T une représentation, dite canonique, du groupe W_G(T) dans le R-espace vectoriel t.

#### Proposition 6 {#lie-ix-s2-prop-6 .statement tag=01JC}

a) Toute orbite de G dans g (pour la représentation adjointe) rencontre t.
    b) Les traces sur t des orbites de G sont les orbites de W_G(T) dans t.
L’assertion a) résulte du th. 1 (n° 1). Soient x, y deux éléments de t conjugués sous Ad(G), et soit h ∈ G tel que (Ad h)(x) = y. Appliquant le corollaire au th. 1 (n° 1) avec a = {x}, u = Ad h, t' = t, on voit qu’il existe g ∈ G tel que Ad hg applique t sur t et x sur y. On a alors hg ∈ N_G(T) (III, § 9, n° 4, prop. 11), et la classe de hg dans W_G(T) applique x sur y, d’où la proposition.

#### Corollaire {#lie-ix-s2-n5-cor-1 .statement tag=01JD}

L’injection canonique de t dans g définit par passage au quotient un homéomorphisme de t/W_G(T) sur g/Ad(G).
Notons j cette application ; elle est bijective et continue (prop. 6). On a un diagramme commutatif

$$
\begin{array}{ccc}
t & \xrightarrow{i} & g \\
|_p & & |_q \\
t/W_G(T) & \xrightarrow{j} & g/Ad(G)
\end{array}
$$

où p et q sont les applications de passage au quotient, et i l’injection canonique. Comme i et q sont propres (TG, I, p. 72, prop. 2 et TG, III, p. 28, prop. 2, c)) et que p est surjective, on en déduit que j est propre (TG, I, p. 73, prop. 5), donc est un homéomorphisme.

#### Proposition 7 {#lie-ix-s2-prop-7 .statement tag=01JE}

Soit H un sous-groupe fermé de G contenant T.
a) Notons W_H(T) le sous-groupe N_H(T)/T de W_G(T); le groupe H/H_0 est isomorphe au groupe quotient W_H(T)/W_{H_0}(T).
b) Pour que H soit connexe, il faut et il suffit que tout élément de W_G(T) qui a un représentant dans H appartienne à W_{H_0}(T).
L’assertion a) résulte du cor. 8 au th. 2 (n° 2), et l’assertion b) est un cas particulier de a).

### 6. Tores maximaux et relèvement d’homomorphismes

Soient G un groupe de Lie compact connexe, T un tore maximal de G. Considérons le groupe dérivé D(G) de G et son revêtement universel $\tilde{D}(G)$; soit $p : \tilde{D}(G) \to G$ le morphisme composé des morphismes canoniques $\tilde{D}(G) \to D(G)$ et $D(G) \to G$. Alors $\tilde{D}(G)$ est un groupe de Lie compact connexe ($§ 1$, no 4, cor. 2 à la prop. 4); de plus, l’image réciproque $\tilde{T}$ de T par $p$ est un tore maximal de $\tilde{D}(G)$ (no 3, prop. 1).

#### Lemme 2 {#lie-ix-s2-lem-2 .statement tag=01AO}

Soient H un groupe de Lie, $f_T : T \to H$ et $\tilde{f} : \tilde{D}(G) \to H$ des morphismes de groupes de Lie tels que, pour tout $t \in \tilde{T}$, on ait $f_T(p(t)) = \tilde{f}(t)$. Il existe un unique morphisme de groupes de Lie $f : G \to H$ tel que $f \circ p = \tilde{f}$ et que la restriction de $f$ à T soit $f_T$.

Posons $Z = C(G)_0$; d’après $§ 1$, no 4, cor. 1 à la prop. 4, le morphisme de groupes de Lie $g : Z \times \tilde{D}(G) \to G$ tel que $g(z, x) = z^{-1}p(x)$ est un revêtement; son noyau est formé des couples $(z, x)$ tels que $p(x) = z$, pour lesquels on a donc $x \in p^{-1}(Z) \subset \tilde{T}$. Puisque le morphisme $(z, x) \mapsto f_T(z^{-1})\tilde{f}(x)$ de $Z \times \tilde{D}(G)$ dans H applique Ker $g$ dans $\{e\}$, il existe un morphisme $f$ de G dans H tel que $f \circ p = \tilde{f}$ et $f(z) = f_T(z)$ pour $z \in Z$. Mais on a aussi $f(t) = f_T(t)$ pour $t \in p(\tilde{T})$; comme $T = Z.p(\tilde{T})$, la restriction de $f$ à T est bien $f_T$.

#### Proposition 8 {#lie-ix-s2-prop-8 .statement tag=01AP}

Soient G un groupe de Lie compact connexe, T un tore maximal de G, H un groupe de Lie et $\varphi : L(G) \to L(H)$ un homomorphisme d’algèbres de Lie. Pour qu’il existe un morphisme de groupes de Lie $f : G \to H$ tel que $L(f) = \varphi$, il faut et il suffit qu’il existe un morphisme de groupes de Lie $f_T : T \to H$ tel que $L(f_T) = \varphi|L(T)$; on a alors $f_T = f|T$.

Si $f : G \to H$ est un morphisme de groupes de Lie tel que $L(f) = \varphi$, alors la restriction $f_T$ de $f$ à T est l’unique morphisme de T dans H tel que $L(f_T) = \varphi|L(T)$. Inversement, soit $f_T : T \to H$ un morphisme de groupes de Lie tel que $L(f_T) = \varphi|L(T)$. Soient $\tilde{D}(G)$ et $p$ comme ci-dessus; l’application $L(p)$ induit un isomorphisme de $L(\tilde{D}(G))$ sur l’algèbre dérivée b de $L(G)$. Il existe un morphisme de groupes de Lie $\tilde{f} : \tilde{D}(G) \to H$ tel que $L(\tilde{f}) = (\varphi|b) \circ L(p)$ (III, $§ 6$, no 1, th. 1). Les morphismes $t \mapsto \tilde{f}(t)$ et $t \mapsto f_T(p(t))$ de $\tilde{T}$ dans H induisent le même homomorphisme des algèbres de Lie, donc coïncident. Appliquant le lemme 2, on en déduit l’existence d’un morphisme $f : G \to H$ tel que $L(f)$ et $\varphi$ coïncident sur $L(T)$ et b. Comme $L(G) = b + L(T)$, on a bien $L(f) = \varphi$.

#### Proposition 9 {#lie-ix-s2-prop-9 .statement tag=01AQ}

Soient G un groupe de Lie compact connexe, T un tore maximal de G, H un groupe de Lie, $f : G \to H$ un morphisme. Alors f est injectif si et seulement si sa restriction à T est injective.

En effet d’après le th. 2 (no 2), le sous-groupe distingué Ker $f$ de G est réduit à l’élément neutre si et seulement si son intersection avec T est réduite à l’élément neutre.

## EXERCICES {#lie-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
