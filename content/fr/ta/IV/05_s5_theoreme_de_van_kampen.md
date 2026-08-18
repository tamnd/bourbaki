---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 5
section_title: Théorème de van Kampen
lang: fr
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
content_sha256: 33d8e3d3f896507e9f4ad56afa068d2ab5c5b0ad62de16239fee73cca722508f
---

## § 5. THÉORÈME DE VAN KAMPEN

### 1. Coégalisateur des projections d’un carré fibré

Soient X et Y des espaces topologiques et soit $f$ une application continue de X dans Y. On note Z le carré fibré $X\times_YX$ et $p_1,p_2$ les deux projections de Z dans X. On note W le produit fibré $X\times_YX\times_YX$ ; pour tout couple $(s, t)$ d’entiers égaux à 1, 2 ou 3, on note $q_{st}: W\rightarrow Z$ l’application définie par $q_{st}(x_1, x_2, x_3) = (x_s, x_t)$.

Notons Coeg($f$) le groupoïde Coeg($\varpi (p_1), \varpi (p_2)$), coégalisateur des deux morphismes $\varpi (p_1),\varpi (p_2)$ du groupoïde de Poincaré $\varpi (Z)$ dans le groupoïde de Poincaré $\varpi (X)$. Notons $\gamma :\varpi (X)\rightarrow$ Coeg($f$) le morphisme de groupoïdes canonique. Comme $f\circ p_1$ = $f\circ p_2$, les morphismes de groupoïdes $\varpi (f)\circ \varpi (p_1)$ et $\varpi (f)\circ \varpi (p_2)$ de $\varpi (Z)$ dans $\varpi (Y)$ sont égaux ; il existe ainsi un unique morphisme de groupoïdes $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ tel que $\varpi '(f)\circ \gamma =\varpi (f)$.

#### Définition 1 {#ta-iv-s5-def-1 .statement tag=0230}

On dit que l’application $f$ vérifie la propriété (VK) si elle est stricte, surjective et si le morphisme $\varpi '(f)$ est un isomorphisme.

#### Exemple 1 {#ta-iv-s5-n1-exa-1 .statement tag=0231}

Cette propriété est vérifiée sous l’une des hypothèses suivantes :

(i) Les espaces X et Y sont délaçables, l’espace $X\times_YX$ est localement connexe par arcs, l’application $f$ est surjective, propre, séparée, à fibres localement connexes ;

(ii) Les espaces X et Y sont délaçables, l’application $f$ est surjective, propre, séparée, à fibres finies, la diagonale $\Delta_X$ de $X\times_YX$ est ouverte et son complémentaire est localement connexe ;

(iii) Les espaces X et Y sont délaçables, l’application $f$ est surjective, ouverte et possède la propriété de relèvement des chemins ;

(iv) Tout point de Y possède un voisinage au-dessus duquel il existe une section continue de l’application $f$.

En effet, sous chacune de ces hypothèses, l’application $f$ est surjective ; elle est aussi stricte en vertu de I, p. 18, exemple 2. Enfin, le morphisme $\varpi '(f)$ est un isomorphisme, tant sous les hypothèses (i), (ii) ou (iii) d’après IV, p. 398, th. 1, que sous l’hypothèse (iv) ( IV, p. 400, th. 2).

La prop. 5 de II, p. 208 décrit les groupes d’isotropie du groupoïde Coeg($f$). Le but de ce n$^o$ est d’expliciter, lorsque $f$ vérifie la propriété (VK), la description des groupes de Poincaré de Y qui s’en déduit par composition avec l’isomorphisme de groupoïdes $\varpi '(f)$. Les n$^{os}$ suivants seront consacrés à des cas particuliers importants.

Supposons que l’application $f$ satisfasse la propriété (VK).

Posons $\mathsf{I}=\pi_0(X),\mathsf{J}=\pi_0(Z),\mathsf{K}=\pi_0(W)$; pour $j\in \mathsf{J}$ et $s\in  \{1,2\}$, on pose $i_s(j) =\pi_0(p_s)(j)$ ; pour $k\in \mathsf{K}$ et $s,t\in  \{1,2,3\}$, on pose $j_{st}(k) =\pi_0(q_{st})(k)$. Notons $\mathsf{\Gamma}$ l’armature du couple $(\varpi (p_1), \varpi (p_2))$ de morphismes de groupoïdes de $\varpi (Z)$ dans $\varpi (X)$ (II, p. 185, déf. 3). C’est le carquois $(\mathsf{I},\mathsf{J}, \pi_0(p_1), \pi_0(p_2))$, car les orbites du groupoïde de Poincaré d’un espace topologique sont les composantes connexes par arcs de cet espace.

Supposons de plus que Y soit connexe par arcs et non vide. D’après II, p. 200, remarque 2, $\pi_0(\mathsf{\Gamma})$ est alors en bijection avec l’ensemble des orbites du groupoïde Coeg($f$) ; puisque l’application $f$ satisfait à la propriété (VK), le groupoïde Coeg($f$) est isomorphe au groupoïde $\varpi (Y)$. Le graphe $\mathsf{\Gamma}$ est ainsi connexe et non vide.

Appelons donnée de van Kampen de $f$ la donnée des éléments suivants :

(i) pour tout $i\in \mathsf{I}$, un point $\mathsf{a}(i)$ de la composante connexe par arcs $i$ de X ;

(ii) pour tout $j\in \mathsf{J}$, un point $\mathsf{b}(j) = (\mathsf{b}_1(j),\mathsf{b}_2(j))$ de la composante connexe par arcs $j$ de Z ;

(iii) pour tout $k\in \mathsf{K}$, un point $\mathsf{c}(k) = (\mathsf{c}_1(k),\mathsf{c}_2(k),\mathsf{c}_3(k))$ de la composante connexe par arcs $k$ de W;

(iv) pour tout $j\in \mathsf{J}$, la classe $\beta_1(j)$ d’un chemin dans X reliant $\mathsf{b}_1(j)$ à $\mathsf{a}(i_1(j))$ et la classe $\beta_2(j)$ d’un chemin dans X reliant $\mathsf{b}_2(j)$ à $\mathsf{a}(i_2(j))$;

(v) pour tout $k\in \mathsf{K}$ et pour tout couple $(s, t)$ égal à $(1,2)$, $(2,3)$ ou $(1,3)$, la classe $\gamma_{st}(k)$ d’un chemin dans Z reliant $(\mathsf{c}_s(k),\mathsf{c}_t(k))$ à $\mathsf{b}(j_{st}(k))$;

(vi) un sous-carquois $\mathsf{T}$ de $\mathsf{\Gamma}$ dont le graphe associé est un arbre maximal du graphe $\widetilde{\mathsf{\Gamma }}$;

(vii) un élément $i_0$ de $\mathsf{I}$.

Choisissons une donnée de van Kampen de $f$. Alors, $(\mathsf{a},\mathsf{b}, \beta_1, \beta_2,\mathsf{T}, i_0)$ est un équipement de base du couple $(\varpi (p_1), \varpi (p_2))$ de morphismes de groupoïdes de $\varpi (Z)$ dans $\varpi (X)$ (II, p. 192, déf. 4). Par ailleurs, les triplets

$$
\mathsf{z}= ((q_{12}(\mathsf{c}(k)),1),(q_{23}(\mathsf{c}(k)),1),(q_{13}(\mathsf{c}(k)),-1))
$$

et les classes de chemins $(\gamma_{1,2}(k), \gamma_{2,3}(k), \gamma_{1,3}(k))$, où $k$ décrit $\mathsf{K}$, définissent un équipement complémentaire du couple $(\varpi (p_1), \varpi (p_2))$ (II, p. 208, déf. 3 ; II, p. 205, exemple ; II, p. 205, remarque). Nous dirons que l’équipement complet du coégalisateur Coeg($f$) ainsi défini est déduit de la donnée de van Kampen de $f$ que nous avons choisie.

Pour tout $j\in \mathsf{J}$, notons $\varphi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_1(j)))$ et $\psi_j:\pi_1(Z,\mathsf{b}(j))\rightarrow \pi_1(X,\mathsf{a}(i_2(j)))$ les homomorphismes de groupes définis par

$\varphi_j=$ Int($\beta_1(j)$)$^{-1}\circ (p_1)_*,v\mapsto \beta_1(j)^{-1}((p_1)_*(v))\beta_1(j)$

(1)

$\psi_j=$ Int($\beta_2(j)$)$^{-1}\circ (p_2)_*,v\mapsto \beta_2(j)^{-1}((p_2)_*(v))\beta_2(j)$,

pour $v\in \pi_1(Z,\mathsf{b}(j))$. Pour tout $k\in \mathsf{K}$ et tout $s\in  \{1,2,3\}$, notons $\lambda_s(k)$ la classe de lacet au point $\mathsf{a}(i_s(k))$ dans X définie par

(2)

$$
\lambda_1(k) =\beta_1(j_{13}(k))^{-1}\cdot ((p_1)_*(\gamma_{13}(k)))^{-1}\cdot ((p_1)_*(\gamma_{12}(k)))\cdot \beta_1(j_{12}(k))
$$

$\lambda_2(k) =\beta_2(j_{12}(k))^{-1}\cdot ((p_2)_*(\gamma_{12}(k)))^{-1}\cdot ((p_1)_*(\gamma_{23}(k)))\cdot \beta_1(j_{23}(k))$,

$$
\lambda_3(k) =\beta_2(j_{23}(k))^{-1}\cdot ((p_2)_*(\gamma_{23}(k)))^{-1}\cdot ((p_2)_*(\gamma_{13}(k)))\cdot \beta_2(j_{13}(k))
$$

Notons $\tau$ l’unique morphisme de groupoïdes de Grp($\mathsf{\Gamma}$) dans $\varpi (Y)$ tel que l’application Som($\tau$ ) applique $i\in \mathsf{I}$ sur $f(\mathsf{a}(i))$ et Fl($\tau$ ) applique $j\in \mathsf{J}$ sur la classe de chemins $f_*(\beta_1(j))^{-1}f_*(\beta_2(j))$ reliant $f(\mathsf{a}(i_1(j)))$

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

à $f(\mathsf{a}(i_2(j)))$ dans Y. Pour $i\in \mathsf{I}$, soit $d_i\in$ Grp($\mathsf{\Gamma}$) la classe de l’unique chemin sans aller-retour reliant $i_0$ à $i$ dans l’arbre $\widetilde{\mathsf{T}}$ et posons $\delta_i=$ $\tau (d_i)$.

Si S est un ensemble, rappelons que F(S) désigne le groupe libre sur S ; l’image dans F(S) d’un élément $s\in S$ par l’application canonique est notée $[s]$, voire $s$ s’il n’y a pas de confusion possible.

#### Théorème 1 {#ta-iv-s5-thm-1 .statement tag=0232}

Supposons que Y soit connexe par arcs et que $f$ vérifie la propriété (VK). Avec les notations précédentes, il existe un unique homomorphisme de groupes

$$
\mathsf{L}:(_i*_{\in\mathsf{I}}\pi_1(X,\mathsf{a}(i)))*F(\mathsf{J})\rightarrow \pi_1(Y, f(\mathsf{a}(i_0)))
$$

tel que

$\mathsf{L}(v) =\delta_if_*(v)\delta^{-1}_i$ pour $i\in \mathsf{I}$ et $v\in \pi_1(X,\mathsf{a}(i))$,

$\mathsf{L}(j) =\delta_{i_1(j)}\tau (j)\delta^{-1}_{i_2(j)}$ pour $j\in \mathsf{J}$.

De plus, l’homomorphisme $\mathsf{L}$ est surjectif et son noyau est le plus petit sous-groupe distingué contenant les éléments suivants :

($R_1$)$\mathsf{r}_1(j) =j$ pour $j$ dans Fl($\mathsf{T}$) ;

($R_2$)$\mathsf{r}_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$ pour $j\in \mathsf{J}$ et $v\in \pi_1(Z,\mathsf{b}(j))$;

($R_3$)$\mathsf{r}_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$, pour $k\in \mathsf{K}$.

L’existence et l’unicité de l’homomorphisme $\mathsf{L}$ résultent de la propriété universelle des produits libres et des groupes libres. Du reste, cet homomorphisme est le composé de l’homomorphisme $\varpi '(f)_{\gamma(\mathsf{a}(i_0))}$ déduit de $\varpi '(f)$ par passage aux groupes d’isotropie et de l’homomorphisme de groupes $\lambda$ défini par la prop. 5 de II, p. 208, compte tenu de ce que la donnée de van Kampen choisie détermine un équipement complet du couple $(\varpi (p_1), \varpi (p_2))$ de morphismes de groupoïdes de $\varpi (Z)$ dans $\varpi (X)$. D’après cette proposition, l’homomorphisme $\lambda$ a pour image le groupe Coeg($f$)$_{\gamma(\mathsf{a}(i_0))}$ et son noyau est le plus petit sous-groupe distingué contenant les éléments définis par les relations ($R_1$)$, (R_2)$ et ($R_3$). D’autre part, le morphisme de groupoïdes $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ est un isomorphisme, par définition de la propriété (VK). Le théorème est donc démontré.

### 2. Recouvrements

Soit Y un espace topologique connexe par arcs, non vide, et soit $(A_i)_{i\in I}$ un recouvrement de Y par des parties connexes par arcs non vides, indexé par un ensemble totalement ordonné I. Soit $X =\bigsqcup_{i\in I}A_i$ l’espace somme de la famille $(A_i)$ et soit $f: X\rightarrow Y$ l’application déduite de la famille des injections canoniques de chaque $A_i$ dans Y. Supposons que l’application $f$ satisfait à la propriété (VK). Cela a lieu notamment dans les deux cas suivants :

(i) les intérieurs des ensembles $A_i$, pour $i\in I$, recouvrent Y (cf. IV, p. 402, exemple 2) ;

(ii) l’espace Y est délaçable, ainsi que les espaces $A_i$, pour $i\in I$, la famille $(A_i)_{i\in I}$ est localement finie, les $A_i$ sont fermés dans Y et leurs intersections deux à deux sont localement connexes par arcs (cf. IV, p. 399, exemple 1).

Soit $J'$ l’ensemble des triplets $(i, i',V)$, où $i$ et $i'$ sont des éléments de I et où V est une composante connexe par arcs de $A_i\cap A_{i'}$. Si $j= (i, i',V)\in J'$, on pose $i_1(j) =i,i_2(j) =i'$ et $\overline{j}= (i', i,V)$. Soit J le sous-ensemble de $J'$ formé des triplets tels que $i < i'$. On appelle armature du recouvrement le carquois Γ dont l’ensemble des sommets est I, dont l’ensemble des flèches est J et les applications origine et terme sont respectivement les applications $j\mapsto i_1(j)$ et $j\mapsto i_2(j)$. Nous identifierons le graphe associé à Γ au graphe $\widetilde{\Gamma}$ dont l’ensemble des sommets est I, l’ensemble des flèches est $J\cup \overline{J}$, les applications origine et terme sont les applications $j\mapsto i_1(j)$ et $j\mapsto i_2(j)$ et l’involution est l’application $j\mapsto \overline{j}$.

Notons $p_1$ et $p_2$ les projections du carré fibré $X\times_YX$ vers X ; soit $\mathsf{\Gamma}$ l’armature du couple $(\varpi (p_1), \varpi (p_2))$ de morphismes de groupoïdes de $\varpi (X\times_YX)$ dans $\varpi (X)$.

#### Lemme 1 {#ta-iv-s5-lem-1 .statement tag=0233}

Le carquois Γ s’identifie à un sous-carquois de $\mathsf{\Gamma}$; les carquois Γ et $\mathsf{\Gamma}$ sont connexes.

Les composantes connexes par arcs de X sont les $A_i$, pour $i\in I$. Les composantes connexes par arcs de $X\times_YX$ sont les $(V\times  \{i\})\times_Y$ $(V\times  \{i'\})$, pour $(i, i',V)\in J'$. Par suite, l’armature $\mathsf{\Gamma}$ du couple $(\varpi (p_1), \varpi (p_2))$ est isomorphe au carquois dont l’ensemble des sommets est I, l’ensemble des flèches est $J'$, les applications origine et terme étant respectivement les applications $j\mapsto i_1(j)$ et $j\mapsto i_2(j)$. Le carquois $\mathsf{\Gamma}$ est connexe (IV, p. 406). En outre, cette description identifie Γ à un sous-carquois de $\mathsf{\Gamma}$. Observons aussi que pour tout flèche $j$ de $\mathsf{\Gamma}$, ou bien $j\in$ Fl($\widetilde{\Gamma}$), ou bien il existe $i\in I$ tel que $j= (i, i,A_i)$. Il s’ensuit que l’application $\pi_0(\Gamma )\rightarrow \pi_0(\mathsf{\Gamma})$ déduite de l’injection de Γ dans $\mathsf{\Gamma}$ est bijective, si bien que Γ est connexe.

Pour tout élément $i$ de I, choisissons un point $a(i)$ de $A_i$.

Pour tout élément $j= (i, i',V)$ de J, choisissons un point $b(j)$ dans V, un chemin $B_1(j)$ reliant $b(j)$ à $a(i)$ dans $A_i$ et un chemin $B_2(j)$

reliant$\overline{j}= (i', i,b(jV)$) àappartient à$a(i')$ dans A$J^{i'}$. Soitet l’on pose$j= (i, ib(',\overline{j}V)$) =un élément de$b(j)$, $B_1(j) = B\overline{J}_2$; alors$(\overline{j})$ et $B_2(j) = B_1(\overline{j})$. Pour $j\in J'\cup \overline{J'}$, les chemins $\overline{B_1(j)}$ et $B_2(j)$ dans Y sont juxtaposables. Posons

$$
B(j) = B_1(j)*B_2(j) \tag{3}
$$

C’est un chemin qui relie $a(i_1(j))$ à $a(i_2(j))$ dans Y ; on a la relation $B(\overline{j}) = B(j)$.

Pour tout $j= (i, i',V)\in J'$, notons $p_{j,1}: V\rightarrow A_i$ et $p_{j,2}: V\rightarrow A_{i'}$ les injections canoniques ; notons aussi $\varphi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_i, a(i))$ et $\psi_j:\pi_1(V, b(j))\rightarrow \pi_1(A_{i'}, a(i'))$ les homomorphismes de groupes définis par

$$
\varphi_j(v) = [B_1(j)]^{-1}(p_{j,1})_*(v)[B_1(j)]
$$

et

$$
\psi_j(v) = [B_2(j)]^{-1}(p_{j,2})_*(v)[B_2(j)]
$$

pour $v\in \pi_1(V, b(j))$ (cf. IV, p. 407).

Fixons un élément $i_0$ de I, ainsi qu’un sous-carquois T dans le carquois Γ dont le graphe associé $\widetilde{T}$ est un arbre maximal du graphe $\widetilde{\Gamma}$.

Pour $i\in I$, soit $(i_0, j_1, i_1, . . . , j_n, i)$ l’unique chemin sans aller-retour reliant $i_0$ à $i$ dans l’arbre $\widetilde{T}$ et posons

$$
\delta (i) = [B(j_1)][B(j_2)]. . .[B(j_n)]
$$

c’est la classe d’un chemin reliant $a(i_0)$ à $a(i)$ dans Y. Notons $\alpha_i$ l’homomorphisme de $\pi_1(A_i, a(i))$ dans $\pi_1(Y, a(i))$ déduit de l’injection canonique et soit $\mu_i:\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ l’homomorphisme de groupes défini par

$$
\mu_i(v) =\delta (i)\alpha_i(v)\delta (i)^{-1}
$$

Soit enfin $\mu: F(J)\rightarrow \pi_1(Y, a(i_0))$ l’unique homomorphisme de groupes tel que l’on ait

$$
\mu(j) =\delta (i_1(j))[B(j)]\delta (i_2(j))^{-1}
$$

pour tout $j\in J$. Il existe un unique homomorphisme de groupes

$$
\mathsf{M}:(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow \pi_1(Y, a(i_0))
$$

qui coïncide avec $\mu_i$ dans $\pi_1(A_i, a(i))$, pour tout $i\in$ I, et avec $\mu$ dans F(J).

Notons $K'$ l’ensemble des quadruplets $(i_1, i_2, i_3,U)$, où $i_1, i_2, i_3$ sont des éléments de I et où U est une composante connexe par arcs de $A_{i_1}\cap A_{i_2}\cap A_{i_3}$. Pour tout élément $k= (i_1, i_2, i_3,U)$ de $K'$ et tout couple $(s, t)$ d’éléments de $\{1,2,3\}$, on pose $j_{st}(k) = (i_s, i_t,V)$, où V est la composante connexe par arcs de $A_{i_s}\cap A_{i_t}$ qui contient U ; c’est un élément de $J'$.

Notons K le sous-ensemble de $K'$ formé des quadruplets $(i_1, i_2, i_3,U)$ tels que $i_1< i_2< i_3$. Pour tout élément $k= (i_1, i_2, i_3,U)$ de K, choisissons un point $c(k)$ de U, ainsi que des chemins $C_{12}(k)$, $C_{23}(k)$ et $C_{13}(k)$, tels que $C_{st}(k)$ relie $c(k)$ à $b(j_{st}(k))$ dans $A_{i_s}\cap A_{i_t}$ pour $s, t\in  \{1,2,3\}$ avec $s < t$.

Posons alors, pour $k\in K$,

$$
L_1(k) = B_1(j_{13}(k))*\overline{C_{13}(k)}*C_{12}(k)*B_1(j_{12}(k))
$$

(4) L$L_{23}((kk) = B) = B_{22}((jj_{1223}((kk))))**\overline{CC^{1223}((kk))}**CC_{2313}((kk))**BB_{12}((jj_{2313}((kk))))$,.

Pour $s\in  \{1,2,3\}$, on note $\lambda_s(k)$ la classe dans $\pi_1(A_{i_s}, a(i_s))$ du lacet $L_s(k)$.

#### Proposition 1 {#ta-iv-s5-prop-1 .statement tag=0234}

Soit Y un espace topologique connexe par arcs et soit $(A_i)_{i\in I}$ un recouvrement de Y par des parties non vides, connexes par arcs, indexé par un ensemble totalement ordonné I. Supposons que l’application canonique de l’espace somme de la famille $(A_i)_{i\in I}$ vers Y satisfait à la propriété (VK). Alors, l’homomorphisme $\mathsf{M}$ introduit ci-dessus est surjectif et son noyau est le plus petit sous-groupe distingué contenant les éléments suivants :

($R_1$)$r_1(j) =j$ pour $j$ dans Fl(T);

($R_2$)$r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$

pour $j= (i, i',V)\in J$ et $v\in \pi_1(V, b(j))$ ;

($R_3$)$r_3(k) =\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}$

pour $k\in K$.

Soit X l’espace topologique somme de la famille $(A_i)_{i\in I}$ et soit $f: X\rightarrow Y$ l’application déduite de la famille des injections canoniques de chaque $A_i$ dans Y. L’application $f$ satisfait à la propriété (VK) par hypothèse ; nous allons ainsi lui appliquer le th. 1 du n$^o1$. Nous reprenons donc les notations de ce n$^o$ et commençons par définir une donnée de van Kampen de l’application $f$.

Les composantes connexes par arcs de X sont les ensembles $X_i=$ $A_i\times  \{i\}$ pour $i\in I$. On identifie ainsi $\pi_0(X)$ à l’ensemble I. Pour tout $i\in I$, notons $\mathsf{a}(i)$ le point $(a(i), i)$ de $X_i$.

Posons $Z = X\times_YX$. Les composantes connexes par arcs de Z sont les ensembles $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$, où $j= (i, i',V)$ parcourt $J'$. On identifie ainsi $\pi_0(Z)$ à l’ensemble $J'$. Soit $J_0$ l’ensemble des éléments de J de la forme $(i, i,A_i)$, de sorte que la famille $(J_0,J,J)$ est une partition de $J'$. Pour $i\in I$ et $j= (i, i,A_i)\in J_0$, posons $\mathsf{b}(j) = (\mathsf{a}(i),\mathsf{a}(i))$ et prenons pour $\beta_1(j)$ et $\beta_2(j)$ la classe du chemin constant en $\mathsf{a}(i)$. Pour $j= (i, i',V)\in J\cup \overline{J}$, notons $\mathsf{b}(j)$ le point $((b(j), i),(b(j), i'))$ de $Z_j$ et notons $\beta_1(j)$ et $\beta_2(j)$ les classes des chemins $t\mapsto (B_1(j)(t), i)$ et $t\mapsto (B_2(j)(t), i')$ dans X.

Posons $W = X\times_YX\times_YX$. Les composantes connexes par arcs de W sont les ensembles $W_k= (U\times  \{i_1\})\times_Y(U\times  \{i_2\})\times_Y(U\times  \{i_3\})$, où $k= (i_1, i_2, i_3,U)$ parcourt $K'$. On identifie ainsi $\pi_0(W)$ à l’ensemble $K'$.

Notons $K_0$ l’ensemble des éléments de $K'$ de la forme $k= (i, i, i,A_i)$, pour $i\in I$. Pour un tel élément $k\in K_0$, on pose $\mathsf{c}(k) = (\mathsf{a}(i),\mathsf{a}(i),\mathsf{a}(i))$ et on choisit pour $\gamma_{st}(k)$ la classe du chemin constant en $(\mathsf{a}(i),\mathsf{a}(i))$.

Notons $K_1$ l’ensemble des éléments de $K'$ de la forme $k$ = $(i_1, i_2, i_3,V)$ pour lesquels l’ensemble $\{i_1, i_2, i_3\}$ a deux éléments. Soit $k$ un élément de $K'$ de la forme $(i, i, i',V)$, de sorte que $j= (i, i',V)$ appartient à $J\cup \overline{J}$. On pose alors

$$
\mathsf{c}(k) = ((b(j), i),(b(j), i),(b(j), i')),\gamma_{12}(k) = (\beta_1(j), \beta_1(j))
$$

et l’on prend pour $\gamma_{13}(k)$ et $\gamma_{23}(k)$ la classe du chemin constant en $\mathsf{b}(j)$. On définit de façon analogue $c(k),\gamma_{12}(k),\gamma_{13}(k),\gamma_{23}(k)$ pour tout élément $k$ de $K'$.

Pour tout élément $k= (i_1, i_2, i_3,U)$ de K, posons

$$
\mathsf{c}(k) = ((c(k), i_1),(c(k), i_2),(c(k), i_3))
$$

pour tout couple $(s, t)$ d’éléments distincts de $\{1,2,3\}$, prenons pour $\gamma_{st}(k)$ l’image par l’application $x\mapsto ((x, s),(x, t))$ de la classe du chemin $C_{st}(k)$ dans $A_{i_s(k)}\cap A_{i_t(k)}$.

Pour tout point $x= (x_1, x_2, x_3)$ de $X\times_YX\times_YX$ et toute permutation $\sigma \in \mathfrak{S}_3$, posons $\sigma (x) = (x_{\sigma^{-1}(1)}, x_{\sigma^{-1}(2)}, x_{\sigma^{-1}(3)})$. On définit ainsi une opération du groupe $\mathfrak{S}_3$ sur W. Pour tout $k= (i_1, i_2, i_3,U)\in K'$ et toute permutation $\sigma \in \mathfrak{S}_3$, posons de même $\sigma (k) = (i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$ ; on a

$$
\sigma (W_k) = (U\times  \{i_{\sigma^{-1}(1)}\})\times_Y(U\times  \{i_{\sigma^{-1}(2)}\})\times_Y(U\times  \{i_{\sigma^{-1}(3)}\}) = W_{\sigma(k)}
$$

Soit $k= (i_1, i_2, i_3,U)$ un élément de $K'$ tel que $i_1, i_2, i_3$ soient deux à deux distincts. Il existe une unique permutation $\sigma \in$ $\mathfrak{S}_3$ telle que $i_{\sigma^{-1}(1)}< i_{\sigma^{-1}(2)}< i_{\sigma^{-1}(3)}$, de sorte que $\sigma (k) =$ $(i_{\sigma^{-1}(1)}, i_{\sigma^{-1}(2)}, i_{\sigma^{-1}(3)},U)$ appartient à K. Pour $s\in  \{1,2,3\}$, on pose alors $c_s(k) =c_{\sigma(s)}(\sigma (k))$ et $c(k) = (c_1(k), c_2(k), c_3(k))$, de sorte que $c(k) =\sigma^{-1}(c(\sigma (k)))$. Pour $(s, t)\in  \{(1,2),(1,3),(2,3)\}$, on définit $C_{st}(k) = C_{\sigma^{-1}(s)\sigma^{-1}(t)}(\sigma (k))$; c’est un chemin qui relie $c(k)$ à $b(j_{\sigma(s)\sigma(t)}(\sigma (k))) =b(j_{st}(k))$.

Notons $g$ le morphisme de carquois de Γ dans $\mathsf{\Gamma}$ qui, à un sommet $i\in I$ de Γ, associe le sommet $X_i= A_i\times  \{i\}$ de $\mathsf{\Gamma}$ et, à une flèche $j= (i, i',V)\in J'$ de Γ, associe la flèche $Z_j= (V\times \{i\})\times_Y(V\times \{i'\})$ de $\mathsf{\Gamma}$. L’application Som($g$) est bijective ; l’application Fl($g$) est injective et le graphe Γ est connexe (IV, p. 410, lemme 1) et l’image par $g$ du sous-carquois T est un sous-carquois $\mathsf{T}$ de $\mathsf{\Gamma}$ dont le graphe associé est un arbre maximal du graphe $\widetilde{\mathsf{\Gamma }}$.

Les points $\mathsf{a}(i)$, pour $i\in I$, les point $\mathsf{b}(j)$, pour $j\in J'$, les points $\mathsf{c}(k)$, pour $k\in K'$, les classes de chemins $\beta_1(j)$ et $\beta_2(j)$, pour $j\in J'$, les classes de chemins $\gamma_{st}(k)$, pour $k\in K'$, le sous-carquois $g(T)$ de $\mathsf{\Gamma}$ et l’élément $i_0$ de I définissent une donnée de van Kampen de $f$.

Notons $\rho$ l’unique homomorphisme de groupes

$$
\rho :(_i*_{\in I}\pi_1(X,\mathsf{a}(i)))*F(J')\rightarrow (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)
$$

qui induit l’isomorphisme de $\pi_1(X,\mathsf{a}(i))$ sur $\pi_1(A_i, a(i))$ déduit de l’identification de $A_i\times  \{i\}$ et $A_i$, pour tout $i\in I$, et tel que l’on ait

$\rho (j) = 1$ pour $j\in J_0$

$\rho (j) =j,\rho (\overline{j}) =j^{-1}$ pour $j\in J$.

Soit $\mathsf{L}$ l’homomorphisme de groupes défini dans le th. 1 de IV, p. 408. Pour $j= (i, i,A_i)\in J_0$, on a $\mathsf{L}(j) = 1 =\mathsf{M}\circ \rho (j)$. Soit $j= (i, i',V)$ un élément de J ; on a $\mathsf{L}(j) = (\mathsf{M}\circ \rho )(j)$ par définition. Enfin, si $j=$ $(i, i',V)$ est un élément de $\overline{J},\overline{j}\in J$ et l’on vérifie que

$$
\mathsf{L}(j) =\mathsf{L}(\overline{j})^{-1}=\mathsf{M}(\rho (\overline{j}))^{-1}=\mathsf{M}(\rho (j))
$$

Par conséquent, on a $\mathsf{M}\circ \rho =\mathsf{L}$.

L’homomorphisme $\mathsf{L}$ est surjectif (loc. cit.), donc l’homomorphisme $\mathsf{M}$ l’est aussi. Comme l’homomorphisme $\rho$ est surjectif, le noyau de $\mathsf{M}$ est le plus petit sous-groupe distingué de $(_i*_{\in I}\pi_1(A_i, a(i)))*F(J_1)$ qui contient les images par $\rho$ des éléments définis par les relations ($R_1$), ($R_2$)$, (R_3)$ du théorème 1 (IV, p. 408). La démonstration sera terminée une fois que nous aurons vérifié que ces images sont, outre les éléments définis par les relations ($R_1$)$, (R_2), (R_3)$ de la prop. 1, des éléments qui leur sont conjugués, ou qui sont conjugués à leurs inverses, ainsi que l’élément neutre.

Éléments $R_1$. — Une flèche de l’arbre orienté $\mathsf{T}$ est de la forme $Z_j$, avec $j= (i, i',V)\in J$ ; son image est l’élément $j$ de F(J).

Éléments $R_2$. — Soit $j= (i, i',V)\in J'$. Si $i=i'$, on a $\rho (\mathsf{r}_2(j, v)) = 1$ pour tout $v\in \pi_1(A_i,\mathsf{a}(i))$. Si $j\in J$, l’image de $\mathsf{r}_2(j, v)$ est l’élément $r_2(j, v) =\varphi_j(v)j\psi_j(v)^{-1}j^{-1}$, pour tout $v\in \pi_1(Z,\mathsf{b}(j))$. Dans le cas restant, on a $\overline{j}\in J$ et l’égalité

$$
\rho (\mathsf{r}_2(j, v)) =\rho (\varphi_j(v)j\psi_j(v)^{-1}j^{-1})
$$

= [B$= [B_{12}((\frac{j}{j})])]^-_-^1_1vv[B[B_{12}((\frac{j}{j})])]\rho \overline{j}_-(j_1)[B[B_{12}(\frac{(}{j}j)])]_-^-_1^1vv_-^-_1^1[B[B_{12}(\frac{(}{j}j)])]\overline{j}\rho (j)^{-1}$

entraîne que $\rho (\mathsf{r}_2(j, v))$ est conjugué à $\rho (\mathsf{r}_2(j, v^{-1}))$.

Éléments $R_3$. — Soit $k= (i_1, i_2, i_3,U)$ un élément de $K'$.

Si $k\in K_0,i_1$ = $i_2$ = $i_3,\lambda_s(k)$ est la classe du chemin trivial pour tout $s\in  \{1,2,3\},j_{st}(k)\in J_0$ pour tout couple $(s, t)\in$ $\{(1,2),(1,3),(2,3)\}$. Alors, $\rho (\mathsf{r}_3(k))$ est l’élément neutre.

Supposons $k\in K_1$. Si $i_1=i_2$, alors $j= (i_1, i_3,U)\in J\cup \overline{J}$ et l’on a

$$
\mathsf{r}_3(k) =\beta_1(j)^{-1}j_{12}\beta_1(j)j_{23}\beta_2(j)^{-1}\beta_2(j)j_{13}^{-1}
$$

dont l’image par $\rho$ est l’élément neutre. Les autres cas se traitent de même.

Supposons que $i_1, i_2, i_3$ soient deux à deux distincts. Si $i_1< i_2< i_3$, $k\in K$ et l’image de $\rho (\mathsf{r}_3(k))$ est l’élément $r_3(k)$.

Soit $\sigma \in \mathfrak{S}_3$ la permutation qui applique 1 sur 2 et 2 sur 3. On a

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

On vérifie de même que l’on a $\lambda_2(\sigma (k)) =\lambda_1(k)$ et $\lambda_3(\sigma (k)) =\lambda_2(k)$. Par suite,

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

ce qui prouve que $\rho (\mathsf{r}_3(\sigma (k)))$ est conjugué à

$$
\lambda_1(k)j_{12}(k)\lambda_2(k)j_{23}(k)\lambda_3(k)j_{13}(k)^{-1}=\rho (\mathsf{r}_3(k))
$$

Soit $\tau \in \mathfrak{S}_3$ la transposition de support $\{1,2\}$. On a

$\lambda_1(\tau (k)) =\lambda_2(k)^{-1},\lambda_2(\tau (k)) =\lambda_1(k)^{-1}$ et $\lambda_3(\tau (k)) =\lambda_3(k)^{-1}$. Les égalités

$$
\rho (\mathsf{r}_3(\tau (k))) =\lambda_2(k)^{-1}\rho (j_{21}(k))\lambda_1(k)^{-1}\rho (j_{13}(k))\lambda_3(k)^{-1}\rho (j_{23}(k))^{-1}
$$

$$
=(\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}\lambda_1(k)\rho (j_{12}(k))\lambda_2(k))^{-1}
$$

montrent que $\rho (\mathsf{r}_3(\tau (k)))$ est conjugué à l’inverse de

$$
\lambda_1(k)\rho (j_{12}(k))^{-1}\lambda_2(k)\rho (j_{23}(k))\lambda_3(k)\rho (j_{13}(k))^{-1}=\rho (\mathsf{r}_3(k))
$$

Comme le groupe $\mathfrak{S}_3$ est engendré par les permutations $\tau$ et $\sigma$, il s’ensuit que, pour tout $k\in K$ et tout $\sigma \in \mathfrak{S}_3,\rho (\mathsf{r}_3(\sigma (k)))$ est conjugué à $\rho (\mathsf{r}_3(k))$ ou à son inverse.

La proposition 1 est ainsi démontrée.

#### Corollaire 1 {#ta-iv-s5-prop-1-cor-1 .statement tag=0235}

Sous les hypothèses de la proposition 1, supposons de plus que, pour tout $i\in$ I, l’image de l’homomorphisme de $\pi_1(A_i, a(i))$ dans $\pi_1(Y, a(i))$, déduit de l’injection canonique de $A_i$ dans Y, soit triviale. L’homomorphisme $\mathsf{M}': F(J)\rightarrow \pi_1(Y, a(i_0))$ déduit de $\mathsf{M}$ par restriction est alors surjectif et son noyau est le plus petit sous-groupe distingué qui contient les éléments $j\in$ Fl(T) et les éléments $j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$ pour $k\in K$.

Soit $\pi : (_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow F(J)$ l’unique homomorphisme qui induit l’homomorphisme trivial sur chaque $\pi_1(A_i, a(i))$ et l’identité sur F(J); il est surjectif. Soit $i\in I$. La définition de $\mathsf{M}$ et l’hypothèse que l’image de l’homomorphisme de $\pi_1(A_i, a(i))$ dans $\pi_1(Y, a(i))$ déduit de l’injection canonique soit triviale entraînent que, pour tout $v\in \pi_1(A_i, a(i)),\mathsf{M}(v)$ est l’élément neutre de $\pi_1(Y, a(i_0))$. On a donc $\mathsf{M}=\mathsf{M}'\circ \pi$. Par suite, l’homomorphisme $\mathsf{M}'$ est surjectif et son noyau est le plus petit sous-groupe distingué contenant les images par $\pi$ des éléments $r_1(j),r_2(j, v)$ et $r_3(k)$ définis dans la prop. 1. Pour $j\in$ Fl(T), on a $\pi (r_1(j)) =j$. Pour tout $j\in$ J et tout $v\in \pi_1(V, b(j))$, on a $\pi (r_2(j, v)) =e$. Enfin, pour tout $k= (i_1, i_2, i_3,U)\in K$ et tout $s\in$ $\{1,2,3\},\lambda_s(k)$ est la classe d’un lacet dans $A_{i_s}$; on a donc $\pi (\lambda_s(k)) =e$, si bien que $\pi (r_3(k)) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. Le corollaire en résulte.

#### Corollaire 2 {#ta-iv-s5-prop-1-cor-2 .statement tag=0236}

Sous les hypothèses de la proposition 1, supposons de plus que pour tout $i\in I$, le groupe $\pi_1(A_i, a(i))$ soit réduit à l’élément neutre et que, pour tout triplet $(i_1, i_2, i_3)$ d’éléments de I deux à deux distincts, l’ensemble $A_{i_1}\cap A_{i_2}\cap A_{i_3}$ soit vide. L’homomorphisme $\mathsf{M}'':$ F(J-Fl(T)) $\rightarrow \pi_1(Y, a(i_0))$ déduit de $\mathsf{M}$ par restriction est alors un isomorphisme.

Soit $\pi ': F(J)\rightarrow$ F(J - Fl(T)) l’homomorphisme qui applique $[j]$ sur $[j]$ si $j\in$ J-Fl(T) et qui applique $[j]$ sur l’élément neutre si $j\in$ Fl(T) ; il est surjectif et l’on a $\mathsf{M}''\circ \pi '=\mathsf{M}'$, où $\mathsf{M}'$ est l’homomorphisme surjectif défini dans le corollaire 1. Il en résulte que $\mathsf{M}''$ est surjectif et que son noyau est le plus petit sous-groupe distingué de F(J-Fl(T)) qui contient les images par $\pi '$ des éléments décrits dans loc. cit. Or, par construction, $\pi '(j) =e$ si $j\in$ Fl(T) et l’ensemble K est vide, par hypothèse. L’homomorphisme $\mathsf{M}''$ est donc un isomorphisme.

#### Exemple 1 {#ta-iv-s5-n2-exa-1 .statement tag=0237}

Pour le cas d’un recouvrement formé de deux ensembles, voir le n$^o3$.

#### Exemple 2 {#ta-iv-s5-n2-exa-2 .statement tag=0238}

Soit G un graphe (II, p. 155, définition 1) ; notons S l’ensemble des sommets de G, A l’ensemble de ses arêtes orientées, $o$ et $t$ les applications origine et terme de A dans S ; pour toute arête orientée $a\in A$, on note $\overline{a}$ l’arête orientée opposée. Munissons les ensembles S et A de la topologie discrète ; soit X l’espace somme de l’espace S et de l’espace $\mathbf{I}\times A$ et soit $\sim$ la relation d’équivalence la plus fine dans X pour laquelle $(u, a)\sim (1-u, a)$, $(0, a)\sim o(a)$ et $(1, a)\sim t(a)$ pour tout $u\in \mathbf{I}$ et toute arête orientée $a\in A$. L’espace quotient $|G|= X/\sim$ est appelé la réalisation géométrique du graphe G. On note $p$ la projection canonique de X sur $|G|$.

Démontrons que $|G|$ est localement contractile. Soit $s\in S$. Notons $X_s$ la réunion de $\{s\}$ et des parties $[0,1[\times  \{a\}$ pour $a\in \overset{-1}{o}(s)$ et des

parties $]0,1]\times \{a\}$ pour $a\in \overset{-1}{t}(s)$. Soit $U_s$ l’image de $X_s$ dans $|G|$; c’est un voisinage ouvert de $p(s)$ dans $|G|$ car $X_s$ est un voisinage ouvert saturé de $s$ dans X. Soit $f$ l’application de $X_s\times \mathbf{I}$ dans $X_s$ définie, pour $u, v\in \mathbf{I}$ et $a\in A$, par les relations

$$
f(s, v) =s
$$

$((1-v)u, a)$ si $0\leqslant u <1$ et $o(a) =s$,

$$
f((u, a), v) =
$$

$(1-(1-v)(1-u), a)$ si $0< u\leqslant 1$ et $t(a) =s$.

Elle est continue et compatible à la relation d’équivalence $\sim$. Elle définit donc par passage au quotient une application $\varphi_s: U_s\times \mathbf{I}\rightarrow U_s$ qui est continue, car $\mathbf{I}$ est localement compact (I, p. 19, prop. 10). C’est une contraction forte de $U_s$ sur $p(s)$ (III, p. 237, déf. 6).

Soit par ailleurs $x= (\tau , a)\in ]0,1[\times A$. Notons $X_x= ]0,1[\times  \{a, a\}$ et soit $U_x$ son image dans $|G|$ par $p$; c’est un voisinage de $p(x)$ dans $|G|$, homéomorphe à $]0,1[$. L’application de $X_x\times \mathbf{I}$ dans $X_x$ donnée par $((u, a), v)\mapsto ((1-v)u+v\tau , a)$ et $((u, a), t)\mapsto ((1-v)u+v(1-\tau ), a)$ est continue. Elle définit par passage au quotient une application $\varphi_x: U_x\times$ $\mathbf{I}\rightarrow U_x$ qui est continue (loc. cit.) et est une contraction forte en $x$.

Tout point de $|G|$ est l’image d’un point $s\in S$ ou d’un point de $\mathbf{I}\times A$ de la forme $(\tau , a)$ où $0< \tau  <1$. Il en résulte que tout point de $|G|$ possède un voisinage contractile en ce point. Autrement dit, $|G|$ est localement contractile et, en particulier, délaçable (IV, p. 346, prop. 5).

Choisissons un ordre total sur S et considérons le recouvrement ouvert $(U_s)_{s\in S}$ de $|G|$. Soient $s$ et $s'$ des éléments distincts de S. L’intersection $U_s\cap U_{s'}$ est la réunion des $p(]0,1[, a)$ où $a$ parcourt l’ensemble des arêtes orientées de G dont les extrémités sont $s$ et $s'$. Par suite, l’armature du recouvrement $(U_s)_{s\in S}$ s’identifie au carquois G. En outre, pour tout $s\in S$, $U_s$ est contractile en $s$, donc $\pi_1(U_s, p(s))$ est réduit à l’élément neutre. Il résulte alors du cor. 2 de IV, p. 416 que pour tout $s\in S,\pi_1(|G|, p(s))$ est un groupe libre (théorème de Nielsen-Schreier).

#### Corollaire 3 {#ta-iv-s5-prop-1-cor-3 .statement tag=0239}

Sous les hypothèses de la prop. 1, supposons de plus que l’armature du recouvrement $(A_i)_{i\in I}$ soit un arbre orienté. L’homomorphisme $\mathsf{N}:_i*_{\in I}\pi_1(A_i, a(i))\rightarrow \pi_1(Y, a(i_0))$ déduit de $\mathsf{M}$ par restriction est alors surjectif ; son noyau est le plus petit sous-groupe distingué de $_i*_{\in I}\pi_1(A_i, a(i))$ qui contient les éléments $\varphi_j(v)\psi_j(v)^{-1}$, pour

tout $j= (i_1, i_2,V)\in J$ et tout $v\in \pi_1(V, b(j))$.

Si les composantes connexes par arcs des intersections $A_i\cap A_{i'}$, pour $i=\not i'$ sont en outre simplement connexes par arcs, l’homomorphisme $\mathsf{N}$ est alors un isomorphisme.

Sous les hypothèses du corollaire, le graphe associé au carquois Γ est un arbre, d’où T = Γ. Il en résulte que l’image du groupe F(J) par l’homomorphisme $\mathsf{M}$ est réduite à l’élément neutre.

Soit

$$
\rho :(_i*_{\in I}\pi_1(A_i, a(i)))*F(J)\rightarrow_i*_{\in I}\pi_1(A_i, a(i))
$$

l’unique homomorphisme de groupes qui induit l’homomorphisme identique sur $\pi_1(A_i, a(i))$ et dont le noyau contient F(J). On a $\mathsf{M}=\mathsf{N}\circ \rho$. Par conséquent, l’homomorphisme $\mathsf{N}$ est surjectif et son noyau est le plus petit sous-groupe distingué de $_i*_{\in I}\pi_1(A_i, a(i))$ qui

contient les images par $\rho$ des éléments définis par les relations ($R_1$), ($R_2$) et ($R_3$) de la prop. 1. On a $\rho (j) = 1$ pour tout $j\in$ Fl(Γ). Comme l’armature du recouvrement $(A_i)_{i\in I}$ est un arbre, on a $A_{i_1}\cap A_{i_2}\cap A_{i_3}=\emptyset$ pour tout triplet $(i_1, i_2, i_3)$ d’éléments distincts de I. Il en résulte que le noyau de $\mathsf{N}$ est le plus petit sous-groupe distingué qui contient les éléments $\varphi_j(v)\psi_j(v)^{-1}$ pour tout $j= (i_1, i_2,V)\in J$ et tout $v\in \pi_1(V, b(j))$.

#### Exemple 3 (Plan privé de $n$ points) {#ta-iv-s5-n2-exa-3 .statement tag=023A}

Le groupe fondamental de $\mathbf{R}^2$ $\{0\}$ est isomorphe à $\mathbf{Z}$ et la classe du chemin $t\mapsto e^{2\pi it}$ en est un générateur (IV, p. 347, corollaire). Plus généralement, soit $n$ un entier naturel et soit $A =\{z_1, . . . , z_n\}$ un ensemble de $n$ points de $\mathbf{R}^2$. Soit Y l’espace $\mathbf{R}^2-$ A ; nous allons prouver que le groupe fondamental de Y est isomorphe au groupe libre $F_n$ à $n$ générateurs. Pour tout $i$, posons $z_i= (u_i, v_i)$. Quitte à remplacer $z_i$ par $f(z_i)$, où $f:\mathbf{R}^2\rightarrow \mathbf{R}^2$ est un homéomorphisme de la forme $(u, v)\mapsto (u+\alpha v, v)$, on peut supposer que les abscisses des $z_i$ sont deux à deux distinctes. Il n’est pas non plus restrictif de supposer que l’on a $u_1<\cdots < u_n$.

Posons $V_1= ]-\infty , u_2[\times \mathbf{R},V_i= ]u_{i-1}, u_{i+1}[\times \mathbf{R}$ pour $2\leqslant i\leqslant n-1$, $V_n= ]u_{n-1},+\infty [\times \mathbf{R}$. Pour $1\leqslant i\leqslant n$, l’ensemble $U_i= V_i-\{z_i\}$ est ouvert dans le plan et homéomorphe à $\mathbf{R}^2-\{0\}$. La famille $(U_i)_{1\leqslant i\leqslant n}$ est un recouvrement ouvert de l’espace $Y =\mathbf{R}^2-$ A. L’intersection $U_i\cap U_j$ est vide pour $|i-j|\geqslant 2$, homéomorphe à $\mathbf{R}^2$ pour $|i-j|= 1$. D’après le corollaire 3, le groupe fondamental de Y est isomorphe au groupe libre $F_n$.

Soit $a$ un point de Y. Pour tout entier $i\in  \{1, . . . , n\}$, soir $r_i$ un nombre réel strictement positif et strictement inférieur aux distances de $z_i$ aux points $z_j$, pour $j=\not i$. Notons $v_i$ la classe du lacet $t\mapsto$ $z_i+r_ie^{2\pi it}$ au point $z_i+r_i$ de Y. Soit $\theta_i$ la classe d’un chemin $\gamma_i$ reliant le point $a$ au point $z_i+r_i$ dans Y. Si les chemins $\gamma_i$ sont injectifs et que leurs images ne se rencontrent qu’en $a$, on peut démontrer que l’unique homomorphisme du groupe libre $F(t_1, . . . , t_n)$ dans $\pi_1(Y, a)$ tel que $\varphi (t_i) =\theta_iv_i\theta^{-1}_i$ pour tout $i\in  \{1, . . . , n\}$ est un isomorphisme de groupes.

Un raisonnement analogue permet de démontrer que pour toute partie fermée discrète A du plan, le groupe fondamental de $\mathbf{R}^2-$ A est isomorphe à F(A) (IV, p. 463, exerc. 1).

#### Corollaire 4 {#ta-iv-s5-prop-1-cor-4 .statement tag=023B}

Sous les hypothèses de la proposition 1, supposons qu’il existe une partie A de Y, connexe par arcs et non vide, telle que l’intersection $A_i\cap A_{i'}$ soit égale à A pour tout couple $(i, i')$ d’éléments distincts de I. Soit $a$ un point de A. Il existe un unique homomorphisme $\varphi$ de la somme de la famille de groupes $(\pi_1(A_i, a))_{i\in I}$ amalgamée par $\pi_1(A, a)$ dans $\pi_1(Y, a)$ qui coïncide avec l’homomorphisme déduit de l’injection canonique de $A_i$ dans Y, pour tout $i\in I$. L’homomorphisme $\varphi$ est un isomorphisme.

En particulier, si le groupe $\pi_1(A, a)$ est réduit à l’élément neutre, l’homomorphisme canonique du produit libre de la famille de groupes $(\pi_1(A_i, a))_{i\in I}$ dans $\pi_1(Y, a)$ est un isomorphisme.

Pour $i\in$ I, notons $g_i:\pi_1(A, a)\rightarrow \pi_1(A_i, a)$ et $f_i:\pi_1(A_i, a)\rightarrow$ $\pi_1(Y, a)$ les homomorphismes canoniques déduits des inclusions de A dans $A_i$ et de $A_i$ dans Y. Notons $*\pi_1(A_i, a)$ la somme des groupes $\pi_1(A_i, a)$ amalgamée par $\pi_1(A, a)$. Soit aussi$^Ap$ l’unique homomorphisme de $_i*_{\in I}\pi_1(A_i, a)$ dans $*_A\pi_1(A_i, a)$ qui induit l’identité sur $\pi_1(A_i, a)$ (A, I, p. 80, prop. 4). L’homomorphisme $p$ est surjectif et il découle de la définition du monoïde $*\pi_1(A_i, a)$ que son noyau est le plus petit sous-groupe distingué de$^A_i*_{\in I}\pi_1(A_i, a)$ qui contient les

éléments $g_i(v)g_{i'}(v)^{-1}$, pour $i, i'\in I$ et $v\in \pi_1(A, a)$.

Les homomorphismes $f_i\circ g_i:\pi_1(A, a)\rightarrow \pi_1(Y, a)$, pour $i\in I$, sont égaux. Il découle donc de la propriété universelle des sommes amalgamées de monoïdes (A, I, p. 80, prop. 4) qu’il existe un unique homomorphisme de groupes $\varphi$ (resp. $f)$ de $*_A\pi_1(A_i, a)$ (resp. de $_i*_{\in I}\pi_1(A_i, a)$) dans $\pi_1(Y, a)$ qui induit l’homomorphisme $f_i$ sur $\pi_1(A_i, a)$. On a $f=$ $\varphi \circ p$.

Pour $i\in$ I, notons $u_i$ l’injection canonique de A dans $A_i$ et $v_i$ l’injection canonique de $A_i$ dans Y. Notons aussi $w$ l’injection canonique de A dans Y. Pour tout $i\in$ I, on a $v_i\circ u_i$ = $w$, donc $\pi_1(v_i, a)\circ \pi_1(u_i, a) =\pi_1(w, a)$. Il découle alors de la propriété universelle des sommes amalgamées de monoïdes (A, I, p. 80, prop. 4) qu’il existe un unique homomorphisme de groupes $\varphi$ de $*_i\pi_1(A_i, a)$ dans $\pi_1(Y, a)$ qui induit l’homomorphisme $\pi_1(v_i, a)$ sur $\pi_1(A_i, a)$. Il s’agit de démontrer que $\varphi$ est un isomorphisme.

L’ensemble J s’identifie à l’ensemble des couples $(i, i')$ d’éléments de I tels que $i < i'$. L’ensemble K s’identifie à l’ensemble des triplets $(i_1, i_2, i_3)$ d’éléments de I tels que $i_1< i_2< i_3$. Choisissons tous les points-base $a(i),b(j)$ et $c(k)$ égaux à $a$ et tous les chemins $B(j)$, $C_{st}(k)$ égaux au chemin constant d’image $a$. Fixons aussi un point $i_0\in I$.

Pour tout couple $(i, i')$ de points distincts de I, l’armature Γ du recouvrement $(A_i)$ possède exactement une flèche d’extrémités $i$ et $i'$. Les flèches de Γ dont une des extrémités est égale à $i_0$ sont les flèches d’un sous-arbre orienté maximal T.

Pour tout élément $k\in K$, on a $r_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$; soit R le sous-groupe distingué de F(J) engendré par les éléments $j\in$ Fl(T) et les éléments $r_3(k),k\in$ K. Prouvons que R = F(J). Il suffit de montrer que tout élément $j= (i_1, i_2)$ de J appartient à R. C’est vrai, par hypothèse, si $i_1=i_0$ ou $i_2=i_0$. Supposons $i_0< i_1$ et posons $k= (i_0, i_1, i_2)$. C’est un élément de K tel que $j=j_{23}(k) =j$. De plus, $j_{12}(k)$ et $j_{13}(k)$ appartiennent à Fl(T). Il en résulte que $j$ appartient à R. Les cas où $i_1< i_0< i_2$ ou $i_2< i_0$ se traitent de manière analogue.

Il résulte alors de la prop. 1 (IV, p. 412) que l’homomorphisme $f$ est surjectif et que son noyau est le plus petit sous-groupe distingué qui contient les relateurs $r_2(j, v) =g_i(v)g_{i'}(v)^{-1}$, pour $j= (i, i',A)\in J$ et $v\in \pi_1(A, a)$. Autrement dit, Ker($f$) $=$ Ker($p$). Cela entraîne que $\varphi$ est un isomorphisme, ainsi qu’il fallait démontrer.

Si $\pi_1(A, a)$ est réduit à l’élément neutre, $p$ est un isomorphisme, d’où la seconde assertion.

#### Exemple 4 {#ta-iv-s5-n2-exa-4 .statement tag=023C}

Soit $((X_i, x_i))_{i\in I}$ une famille d’espaces topologiques pointés. On appelle bouquet de la famille $((X_i, x_i))_{i\in I}$, et on note $\bigvee_{i\in I}(X_i, x_i)$ l’espace topologique quotient de l’espace somme de la famille $(X_i)_{i\in I}$ par la relation d’équivalence qui identifie entre eux tous les points $(x_i, i)$, pour $i\in I$. Notons X cet espace topologique et $x$ l’image commune des $x_i$. Supposons que, pour tout $i\in$ I, le point $x_i$ soit fermé dans $X_i$ et que les espaces $X_i$ soient délaçables. Si I est fini, le corollaire 4 entraîne que l’homomorphisme canonique $_i*_{\in I}\pi_1(X_i, x_i)\rightarrow \pi_1(X, x)$ est un isomorphisme.

La remarque 1 de IV, p. 429 et l’exercice 3, IV, p. 463 donnent des conditions moins restrictives sous lesquelles cet homomorphisme est un isomorphisme. Voir néanmoins l’exercice 4, IV, p. 464.

### 3. Cas particulier d’un recouvrement formé de deux parties

Soit X un espace topologique connexe par arcs, soient B et C des parties non vides et connexes par arcs de X. On fait en outre l’une des deux hypothèses suivantes :

(i) Les intérieurs des ensembles B et C recouvrent X ;

(ii) Les ensembles B et C sont fermés dans X, leur réunion est égale à X, les espaces X, B, C sont délaçables et l’espace $B\cap C$ est localement connexe par arcs.

Sous ces hypothèses, l’application canonique de l’espace somme de la famille $(B,C)$ sur l’espace X vérifie la propriété (VK) (cf. IV, p. 409).

Posons $A = B\cap C$. Comme l’espace X est connexe, l’ensemble A n’est pas vide. Soit $a$ un point de A ; notons $j_0$ la composante connexe par arcs de $a$ dans A. Pour toute composante connexe par arcs $j$ de A distincte de $j_0$, choisissons un point $a_j$ de $j$, la classe $\beta_j$ d’un chemin dans B et la classe $\gamma_j$ d’un chemin dans C, reliant tous deux $a_j$ à $a$; notons $\varphi_j:\pi_1(A, a_j)\rightarrow \pi_1(B, a)$ et $\psi_j:\pi_1(A, a_j)\rightarrow \pi_1(C, a)$ les homomorphismes de groupes définis par

$\varphi_j(v) =\beta_j^{-1}v\beta_j$ et $\psi_j(v) =\gamma_j^{-1}v\gamma_j$

pour $v\in \pi_1(A, a_j)$. Notons aussi $\varphi_0$ et $\psi_0$ les homomorphismes de $\pi_1(A, a)$ dans $\pi_1(B, a)$ et $\pi_1(C, a)$ respectivement déduits des injections canoniques. Notons $\iota_B$ et $\iota_C$ les homomorphismes de $\pi_1(B, a)$ et $\pi_1(C, a)$ respectivement dans $\pi_1(X, a)$ déduits des injections canoniques. Soit enfin $\mu$ l’unique homomorphisme du groupe libre $F(\pi_0(A)-\{j_0\})$ dans $\pi_1(X, a)$ tel que $\mu(j) =\beta_j^{-1}\gamma_j$ pour tout $j\in \pi_0(A)-\{j_0\}$.

#### Proposition 2 {#ta-iv-s5-prop-2 .statement tag=023D}

Il existe un unique homomorphisme de groupes

$$
\mathsf{M}:\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)-\{j_0\})\rightarrow \pi_1(X, a)
$$

qui coïncide avec $\iota_B$ dans $\pi_1(B, a),\iota_C$ dans $\pi_1(C, a)$ et $\mu$ dans $F(\pi_0(A)$ $\{j_0\})$. Cet homomorphisme est surjectif et son noyau est le plus petit sous-groupe distingué contenant les éléments

$$
\varphi_j(v)j\psi_j(v)^{-1}j^{-1}
$$

pour $j\in \pi_0(A)-\{j_0\}$ et $v\in \pi_1(A, a_j)$, et les éléments

$$
\varphi_0(v)\psi_0(v)^{-1}
$$

pour $v\in \pi_1(A, a)$.

L’armature Γ du recouvrement de X défini par la famille $(B,C)$ a deux sommets $b$ et $c$ correspondant aux deux ensembles B et C. L’ensemble de ses flèches est égal à $\pi_0(A)$; elles relient le point $b$ au point $c$. Le graphe associé au sous-carquois de Γ dont l’unique flèche est $j_0$ est un arbre maximal de $\widetilde{\Gamma}$. La proposition résulte alors de IV, p. 412, prop. 1.

#### Exemple {#ta-iv-s5-n3-exa-1 .statement tag=023E}

Pour $n\geqslant 1$, la sphère $\mathbf{S}_n$ est réunion de deux hémisphères fermés, homéomorphes à la boule fermée $\mathbf{B}_{n-1}$ (TG, VI, p. 12), et dont l’intersection s’identifie à la sphère $\mathbf{S}_{n-1}$. Pour $n\geqslant 2$, la sphère $\mathbf{S}_{n-1}$ est connexe par arcs ; on en déduit que le groupe de Poincaré de $\mathbf{S}_n$ est trivial (cf. I, p. 127, exemple 3).

La sphère $\mathbf{S}_0$ a deux composantes connexes par arcs ; on retrouve ainsi que le groupe de Poincaré du cercle $\mathbf{S}_1$ est isomorphe à un groupe libre à un générateur. Plus précisément, soient B et C les intersections de $\mathbf{S}_1$ avec les demi-plans d’équations $y\geqslant 0$ et $y\leqslant 0$ dans le plan $\mathbf{R}^2$. Posons $a= (1,0),a'= (-1,0)$; on a $B\cap C =\{a, a'\}$; ses composantes connexes sont $j_0=\{a\}$ et $j=\{a'\}$. Soit $\beta$ la classe du chemin $t\mapsto e^{\pi it}$ dans $\mathbf{C}$; si l’on identifie $\mathbf{C}$ à $\mathbf{R}^2$, il relie $a$ à $a'$ dans B. De même, soit $\gamma$ la classe du chemin $t\mapsto e^{-\pi it}$ reliant $a$ à $a'$ dans C. Le chemin $\beta \gamma^{-1}$ est un lacet en $a$, donné par $t\mapsto e^{2\pi it}$. D’après la proposition 2, sa classe engendre le groupe $\pi_1(\mathbf{S}_1, a)$.

#### Corollaire 1 {#ta-iv-s5-prop-2-cor-1 .statement tag=023F}

L’homomorphisme $\mu$ est injectif. Plus précisément, il existe une rétraction associée à $\mu$ qui est un homomorphisme de groupes.

Soit $\rho$ l’unique homomorphisme de $\pi_1(B, a)*\pi_1(C, a)*F(\pi_0(A)$ $\{j_0\})$ dans $F(\pi_0(A)$ - $\{j_0\})$ qui induit l’homomorphisme trivial dans $\pi_1(B, a)$ et $\pi_1(C, a)$ et l’identité dans $F(\pi_0(A)-\{j_0\})$. Soit N le noyau de l’homomorphisme $\mathsf{M}$. D’après la proposition $2,\rho (N)$ est réduit à l’élément neutre. il existe donc un unique homomorphisme $\mathsf{r}$ de $\pi_1(X, a)$ dans $F(\pi_0(A)-\{j_0\})$ tel que $\rho =\mathsf{r}\circ \mathsf{M}$. Pour tout $v\in F(\pi_0(A)-\{j_0\})$, on a $\mathsf{M}(v) =\mu(v)$, donc $\mathsf{r}\circ \mu$ est l’homomorphisme identique. Le corollaire en résulte.

#### Corollaire 2 {#ta-iv-s5-prop-2-cor-2 .statement tag=023G}

Si le groupe $\pi_1(X, a)$ est trivial, l’ensemble A = $B\cap C$ est connexe par arcs ; s’il est commutatif, l’ensemble A possède au plus deux composantes connexes par arcs.

En effet, si S est un ensemble, le groupe libre F(S) n’est trivial que si S est vide et n’est commutatif que si Card $S\leqslant 1$.

#### Corollaire 3 {#ta-iv-s5-prop-2-cor-3 .statement tag=023H}

Si les groupes $\pi_1(X, a)$ et $\pi_1(A, a)$ sont triviaux, il en est de même des groupes $\pi_1(B, a)$ et $\pi_1(C, a)$.

D’après le corollaire 2, l’ensemble A est connexe par arcs. Le groupe $\pi_1(X, a)$ est donc isomorphe au produit libre des groupes $\pi_1(B, a)$ et $\pi_1(C, a)$. Il contient en particulier des sous-groupes isomorphes aux groupes $\pi_1(B, a)$ et $\pi_1(C, a)$ (A, I, p. 83). Ces deux groupes sont donc triviaux si $\pi_1(X, a)$ l’est.

### 4. Espaces quotients

Soit X un espace topologique connexe par arcs muni d’une opération (à droite) propre d’un groupe discret G. Posons $Y = X/G$ et notons $f: X\rightarrow Y$ l’application canonique. Si $g\in G$ et $c:\mathbf{I}\rightarrow X$ est un chemin dans X, on note $g^*c$ le chemin $t\mapsto c(t)\cdot g$ et $g^*[c]$ sa classe d’homotopie stricte.

Soit $o$ un point de X. Pour tout $g\in G$, soit $\beta_g$ la classe d’un chemin reliant $o\cdot g$ à $o$ dans X. Pour tout $g\in G$, soit $X^g$ l’ensemble des points $x\in X$ tels que $x\cdot g=x$; pour toute composante connexe par arcs $j$ de $X^g$, soit $a_j$ un point de $j$ et soit $\gamma_j$ la classe d’un chemin dans X reliant $a_j$ à $o$. Soit $\nu : F(G)\rightarrow \pi_1(Y, f(o))$ l’unique homomorphisme de groupes tel que $\nu (g) =f_*(\beta_g)$ pour $g\in G$. Soit $\mathsf{N}:\pi_1(X, o)*F(G)\rightarrow \pi_1(Y, f(o))$ l’unique homomorphisme de groupes qui coïncide avec $\pi_1(f, o)$ dans $\pi_1(X, o)$ et avec $\nu$ dans F(G).

#### Proposition 3 {#ta-iv-s5-prop-3 .statement tag=023I}

Supposons que X soit délaçable. L’homomorphisme $\mathsf{N}$ est alors surjectif et son noyau est le plus petit sous-groupe distingué de $\pi_1(X, o)*F(G)$ contenant les éléments

($R_2$)$r_2(k, v) = [k]^{-1}v[k](\beta_k^{-1}k^*(v)^{-1}\beta_k)$

pour $k\in G$ et $v\in \pi_1(X, o)$ ;

($R'_3$)$r'_3(k, j) = [k](\beta_k^{-1}k^*(\gamma_j)^{-1}\gamma_j)$

pour $k\in G$ et $j\in \pi_0(X^k)$ ;

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](\beta_h^{-1}h^*(\beta_k^{-1})\beta_{kh})$

pour $k$ et $h\in G$.

Le morphisme de groupoïdes $\varpi (f)$ induit un morphisme

$$
\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)
$$

qui est un isomorphisme d’après le théorème 3 (IV, p. 403), car l’espace X est supposé délaçable. La proposition résulte alors de II, p. 211, prop. 6.

Les trois corollaires ci-dessous découlent des corollaires aussitôt correspondants de la prop. 6 de II, p. 211.

#### Corollaire 1 {#ta-iv-s5-prop-3-cor-1 .statement tag=023J}

Supposons que X soit délaçable et que le groupe G soit engendré par les fixateurs des points de X. Le morphisme canonique $\pi_1(f, o):\pi_1(X, o)\rightarrow \pi_1(Y, f(o))$ est alors surjectif. En particulier, si X est simplement connexe par arcs, il en est de même de Y.

#### Remarque {#ta-iv-s5-n4-rem-1 .statement tag=023K}

Si X est délaçable, Y l’est aussi (IV, p. 349, prop. 8). Comme un espace délaçable connexe est simplement connexe par arcs si et seulement si il est simplement connexe (IV, p. 344, corollaire 1 du théorème 1), on retrouve ainsi la prop. 11 de I, p. 137.

#### Exemple 1 {#ta-iv-s5-n4-exa-1 .statement tag=023L}

Soit X un espace topologique connexe par arcs, délaçable et séparé, et soit $a$ un point de X. Soit $n$ un entier $\geqslant 2$ et soit Y le quotient de l’espace $X^n$ par l’action du groupe $\mathfrak{S}_n$ opérant par permutation des facteurs ; notons $f: X^n\rightarrow Y$ l’application canonique ; notons $g: X\rightarrow Y$ l’application $x\mapsto f(x, a, . . . , a)$. Il découle de la proposition que, pour tout $i$, l’homomorphisme $\pi_1(g, a)$ de $\pi_1(X, a)$ dans $\pi_1(Y, g(a))$ est surjectif et que son noyau est le sous-groupe dérivé de $\pi_1(X, a)$. En particulier, le groupe $\pi_1(Y, g(a))$ est abélien.

#### Corollaire 2 {#ta-iv-s5-prop-3-cor-2 .statement tag=023M}

Supposons que X soit délaçable et que le groupe G opère librement dans X. Il existe un unique homomorphisme de groupes $p:\pi_1(Y, f(o))\rightarrow G$ dont le noyau contient l’image de $\pi_1(X, o)$ et tel que $p(\mathsf{N}(g)) =g$ pour tout $g\in G$. De plus, $\pi_1(X, o)\rightarrow \pi_1(Y, f(o))-\overset{p}{\rightarrow}G$ est une extension de G par $\pi_1(X, o)$.

#### Corollaire 3 {#ta-iv-s5-prop-3-cor-3 .statement tag=023N}

Supposons que X soit simplement connexe par arcs. L’application de G dans $\pi_1(Y, f(o))$ qui, à $g\in$ G, associe la classe de chemins $f_*(\beta_g)$ est un homomorphisme de groupes surjectif ; son noyau est le sous-groupe de G engendré par les fixateurs des points de X.

### 5. Cônes ; contraction d’un sous-espace

Soient X et Y des espaces topologiques non vides et soit $f: X\rightarrow Y$ une application continue. Soit Côn$(f)$ le cône de l’application $f$ et soit $s$ son sommet. Notons $\alpha '_f: X\times \mathbf{I}\rightarrow$ Côn$(f)$ et $\beta '_f: Y\rightarrow$ Côn$(f)$ les applications canoniques. La restriction de $\alpha '_f$ au sous-espace $X\times  \{0\}$ de $X\times \mathbf{I}$ est l’application constante d’image $\{s\}$. L’application $\beta '_f$ induit un homéomorphisme de Y sur la base du cône Côn$(f)$ par lequel nous identifierons ces deux espaces. Notons aussi

$\sigma '_f: ($Côn$(f)-\{s\})\times \mathbf{I}\rightarrow$ Côn$(f)-\{s\}$

la contraction canonique et $\rho '_f:$ Côn$(f)-\{s\} \rightarrow Y$ la rétraction canonique du cône privé de son sommet sur sa base.

Posons $J =\pi_0(X)$; pour tout élément $j$ de J, notons $X_j$ la composante $j$ de X, soit $b_j$ un point de $X_j$ et notons $\gamma_j$ la classe du chemin $t\mapsto \alpha '_f(b_j, t)$ dans Côn$(f)$ qui relie $s$ à $f(b_j)$.

Soit I l’image de l’application $\pi_0(f)$ : c’est l’ensemble des composantes connexes par arcs de Y qui rencontrent $f(X)$; notons $\varphi : J\rightarrow I$ l’application déduite de $f$ par passage aux composantes connexes par arcs. Pour tout élément $i\in I$, notons $Y_i$ la composante $i$ de Y et choisissons un point $a_i$ dans $Y_i$.

Pour tout élément $j$ de J, choisissons un chemin $B_j$ reliant le point $f(b_j)$ au point $a_{\varphi(j)}$ dans $Y_{\varphi(j)}$ et notons $\beta_j$ sa classe. Désignons par $\psi_j$ l’homomorphisme de $\pi_1(X, b_j)$ dans $\pi_1(Y, a_{\varphi(j)})$ défini par

$$
\psi_j(v) =\beta_j^{-1}f_*(v)\beta_j
$$

pour $v\in \pi_1(X, a_j)$.

Soit $\sigma : I\rightarrow J$ une section de l’application $\varphi$. Posons $T =\sigma (I)$ et $\tau =\sigma \circ \varphi$; observons que $\varphi \circ \tau =\varphi$.

#### Proposition 4 {#ta-iv-s5-prop-4 .statement tag=023O}

Supposons que les composantes connexes par arcs de Y soient ouvertes. Pour tout $i\in$ I, soit $G_i$ le quotient du groupe $\pi_1(Y_i, b_i)$ par le plus petit sous-groupe distingué contenant l’image des homomorphismes $\psi_j$, pour $j\in \overset{-1}{\varphi}(i)$ ; notons $p_i$ la surjection canonique de $\pi_1(Y_i, b_i)$ sur $G_i$.

Il existe un unique homomorphisme de groupes

$\mathsf{P}:_i*_{\in I}G_i*F(J-T)\rightarrow \pi_1($Côn$(f), s)$

tel que

$\mathsf{P}(p_i(v)) =$ Int($\gamma_{\sigma(i)}\beta_{\sigma(i)}$)$(v)$ pour $i\in I$ et $v\in \pi_1(Y_i, b_i)$,

$\mathsf{P}(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}$ pour $j\in J-T$.

L’homomorphisme $\mathsf{P}$ est un isomorphisme.

Notons $Y'$ la réunion des composantes connexes par arcs de Y qui rencontrent $f(X)$ et soit $f': X\rightarrow Y'$ l’application donnée par $x\mapsto f(x)$. L’ensemble $Y'$ est une partie ouverte de Y ; ses composantes connexes par arcs sont ouvertes. Le cône Côn$(f')$ s’identifie à la composante connexe par arcs de $s$ dans Côn$(f)$. Cela permet de supposer que $Y = Y'$, autrement dit que l’application $\pi_0(f)$ est surjective et $I =\pi_0(Y)$.

Pour tout $j\in J$, posons $V_j=\alpha '_f(X_j\times ]0,1[)$. Par passage aux sous-espaces, l’application $\alpha '_f$ induit un homéomorphisme de $X\times ]0,1[$ sur le complémentaire de $Y\cup  \{s\}$ dans Côn$(f)$. Par suite, les ensembles $V_j$ sont les composantes connexes par arcs de Côn$(f)-(Y\cup  \{s\})$.

Pour tout $i\in I$, posons $U_i= (\rho '_f)^{-1}(Y_i)$ ; c’est une partie ouverte de Côn$(f)$, car $Y_i$ est ouvert dans Y par hypothèse. Pour tout $j\in \overset{-1}{\varphi}(i)$, on a $f(X_j)\subset Y_i$ et

$$
V_j\cup Y_i=\alpha '_f(X_j\times ]0,1])\cup Y_i
$$

si bien que $V_j\cup Y_i$ est une partie connexe par arcs de Côn$(f)$ contenant $Y_i$. Comme $U_i$ est la réunion de $Y_i$ et des ensembles $V_j$, pour $j\in \overset{-1}{\varphi}(i)$, il en résulte que $U_i$ est connexe par arcs.

Enfin, l’ensemble $C'(X) =$ Côn$(f)$ - Y est une partie ouverte de Côn$(f)$ ; elle est contractile en $s$, donc connexe par arcs.

L’ensemble $C'(X)$ et les ensembles $U_i$, pour $i\in I$, constituent un recouvrement de Côn$(f)$ par des parties ouvertes et connexes par arcs, recouvrement auquel nous allons appliquer la prop. 1 de IV, p. 412. Soit $I'$ l’ensemble obtenu par adjonction de $s$ à I ; on le munit d’un ordre total pour lequel $s$ est son plus petit élément.

Pour des éléments $i, i'$ de I distincts, on a $U_i\cap U_{i'}=\emptyset$. Pour $i\in I$, $C'(X)\cap U_i$ est la réunion des ensembles $V_j$, pour $j\in \overset{-1}{\varphi}(i)$ ; ils sont connexes et deux à deux disjoints. L’intersection de trois ensembles distincts quelconques de ce recouvrement est vide.

L’armature Γ du recouvrement considéré a pour sommets l’ensemble $I'$. Ses flèches sont les triplets $(s, i,V_j)$, pour $j\in J$ et $i=\varphi (j)$ ; on identifiera ainsi l’ensemble des flèches de Γ à l’ensemble J.

Pour $i\in I$, on choisit comme point-base $\mathsf{a}(i) =a_i\in U_i$; on pose aussi $\mathsf{a}(s) =s\in C'(X)$.

Pour $j\in$ J, on pose $\mathsf{b}(j) =\alpha '_f(b_j,\frac{1}{2})$. On note $B_1(j)$ le chemin dans $C'(X)$ d’origine $\mathsf{b}(j)$ et de terme $\mathsf{a}(s)$ donné par $t\mapsto \alpha '_f(b_j,(1-t)/2)$. On note $B_2(j)$ le chemin dans $U_{\varphi(j)}$ d’origine $\mathsf{b}(j)$ et de terme $\mathsf{a}(\varphi (j)) =a_{\varphi(j)}$, juxtaposition du chemin $t\mapsto \alpha '_f(b_j,(1 +t)/2)$ et du chemin $B_j$. Alors, la classe du chemin $B(j) = B_1(j)*B_2(j)$ est égale à $\gamma_j\beta_j$.

On choisit $i_0=s$.

On prend pour arbre orienté maximal T l’unique arbre orienté de Γ dont l’ensemble des flèches est $\sigma (I)$. On a $\delta (s) =e$, tandis que pour $i\in I,\delta (i) = [B(\sigma (i))] =\gamma_{\sigma(i)}\beta_{\sigma(i)}$.

Soit $j\in J$ et soit $i=\varphi (j)$.

L’homomorphisme $\varphi_j$ de $\pi_1(V_j,\mathsf{b}(j))$ dans $\pi_1(C'(X), s)$ est l’homomorphisme trivial car $C'(X)$ est contractile en $s$.

L’application $\alpha '_f$ induit un homéomorphisme de $X_j\times ]0,1[$ sur $V_j$; cet homéomorphisme induit un isomorphisme du groupe $\pi_1(V_j,\mathsf{b}(j))$ sur le groupe $\pi_1(X_j, b_j) =\pi_1(X, b_j)$. Par passage aux sous-espaces, l’application $\sigma '_f$ induit une contraction forte de $U_i$ sur $Y_i$, laquelle induit un isomorphisme du groupe $\pi_1(U_i,\mathsf{a}(i))$ sur le groupe $\pi_1(Y, a_i)$. Par ces isomorphismes, l’homomorphisme

$$
\psi_j:\pi_1(V_j,\mathsf{b}(j))\rightarrow \pi_1(U_{\varphi(j)},\mathsf{a}(\varphi (j)))
$$

s’identifie à l’homomorphisme Int($\beta_{\varphi(j)}^{-1}$)$\circ f_*$ de $\pi_1(X, b_j)$ dans $\pi_1(Y, a_i)$.

Comme $C'(X)$ est contractile en $s$, l’homomorphisme $\mu_s$ est l’homomorphisme trivial.

Soit $i\in I$. L’homomorphisme $\mu_i$ de $\pi_1(U_i,\mathsf{a}(i))$ dans $\pi_1($Côn$(f), s)$ s’identifie à l’homomorphisme de $\pi_1(Y, a_i)$ dans $\pi_1($Côn$(f), s)$ composé de l’homomorphisme Int($\delta (i)$) et de l’homomorphisme de $\pi_1(U_i, s)$ dans $\pi_1($Côn$(f), s)$ déduit de l’injection canonique de $U_i$ dans Côn$(f)$.

Enfin, l’homomorphisme $\mu: F(J)\rightarrow \pi_1($Côn$(f), s)$ est donné par

$$
\mu(j) =\gamma_j\beta_j\beta_{\tau(j)}^{-1}\gamma_{\tau(j)}^{-1}
$$

Soit $\mathsf{P}'$ l’unique homomorphisme de groupes

$\mathsf{P}':_i*_{\in I}\pi_1(Y_i, a_i)*F(J)\rightarrow \pi_1($Côn$(f), s)$

qui coïncide avec l’homomorphisme Int($\delta (i)^{-1}$) dans $\pi_1(Y_i, a_i)$ et avec l’homomorphisme $\mu$ dans F(J). D’après la prop. 1 de IV, p. 412, l’homomorphisme $\mathsf{P}'$ est surjectif et son noyau est le plus petit sous-groupe distingué de $*_i\pi_1(Y_i, a_i)*F(J)$ qui contient les éléments $\mathsf{r}_1(j)$, pour $j\in T$, et les éléments $\mathsf{r}_2(j, v)$, pour $j\in J$ et $v\in \pi_1(V_j,\mathsf{b}(j))$. (Il n’y a pas d’éléments $\mathsf{r}_3(k)$, car l’ensemble K est vide.)

Pour $j\in T$, on a $r_1(j) =j$. Soit $j\in J$ et soit $v\in \pi_1(V_j,\mathsf{b}(j))$. Compte tenu de l’identification de $\pi_1(V_j,\mathsf{b}(j))$ avec $\pi_1(X, b_j)$, on a $\mathsf{r}_2(j, v) =j\psi_j(v)j^{-1}$. Notons $p$ l’homomorphisme surjectif canonique de $*\pi_1(Y_i, a_i)*F(J)$ sur $*G_i*F(J$ - T). Pour $j\in T$, on a $p(\mathsf{r}_1(j)) =^ie$; pour $j\in J$ et $v\in \pi_1(X^i, b_j)$, on a $p(\psi_j(v)) =e$. Par suite, il existe un unique homomorphisme de groupes $\mathsf{P}$ de $*G_i*F(J-T)$ dans $\pi_1($Côn$(f), s)$ tel que $\mathsf{P}'\circ p=\mathsf{P}$; c’est un isomorphisme.$^i$

#### Corollaire 1 {#ta-iv-s5-prop-4-cor-1 .statement tag=023P}

Supposons de plus que les espaces X et Y soient connexes par arcs et soit $a$ un point de X. L’application canonique de $\pi_1(Y, f(a))$ dans $\pi_1($Côn$(f), f(a))$ est surjective, son noyau est le plus petit sous-groupe distingué qui contient l’image de l’homomorphisme $\pi_1(f, a)$.

#### Corollaire 2 {#ta-iv-s5-prop-4-cor-2 .statement tag=023Q}

Supposons de plus que les composantes connexes par arcs de Y soient simplement connexes par arcs. L’homomorphisme $\mu: F(J-T)\rightarrow \pi_1($Côn$(f), s)$ est alors un isomorphisme.

#### Remarque 1 {#ta-iv-s5-n5-rem-1 .statement tag=023R}

Soit X un espace topologique dont les composantes connexes par arcs sont ouvertes. Soit A un sous-espace fermé de X ; notons $\iota : A\rightarrow$ X l’injection canonique, $X/A$ l’espace déduit de X par contraction de A sur un point $o$ et $p: X\rightarrow X/A$ l’application canonique. Supposons en outre que le couple $(X,A)$ possède la propriété d’extension des homotopies. L’application canonique $\overline{\rho}:$ Côn$(\iota )\rightarrow X/A$ est alors une homéotopie (III, p. 255, remarque 1) et l’on déduit de la prop. 4 le calcul du groupe de Poincaré de $X/A$ en son point-base $o$. En particulier, si les composantes connexes par arcs de X sont simplement connexes par arcs, le groupe $\pi_1(X/A, o)$ est un groupe libre.

### 6. Éclatement et recollement

Soit C un espace topologique et soit $(B_{\ell})_{\ell\in L}$ une famille finie de parties fermées de C, deux à deux disjointes. Soit B un espace topologique et, pour tout $\ell \in L$, soit $h_{\ell}$ un homéomorphisme de B sur $B_{\ell}$. On note $B_L$ la réunion de la famille $(B_{\ell})_{\ell\in L}$. Nous supposerons que B et L ne sont pas vides. Soit R la relation d’équivalence sur C définie de la manière suivante. La classe d’un élément $x$ de $C-B_L$ est l’ensemble $\{x\}$; si $x$ est un élément de $B_{\ell}$, où $\ell \in L$, la classe de $x$ est

l’ensemble des éléments $h_k(\overset{-1}{h_{\ell}}(x))$, où $k$ parcourt L. Notons A l’espace topologique quotient $C/R$ et $f: C\rightarrow A$ la surjection canonique. On dit que l’espace A est obtenu à partir de l’espace C par identification des ensembles $B_{\ell}$ au moyen des homéomorphismes $h_{\ell}$.

L’application $f\circ h_{\ell}$ de B dans A est indépendante de l’élément $\ell$ de L ; elle est fermée et injective ; elle induit donc un homéomorphisme de B sur une partie fermée de A. Nous identifierons ainsi B à $f\circ h_{\ell}(B)$ par l’homéomorphisme $f\circ h_{\ell}$; l’application $f$ induit un homéomorphisme de $C-B_L$ sur A-B.

Supposons de plus qu’il existe une famille $(N_{\ell})_{\ell\in L}$ de parties ouvertes de C, deux à deux disjointes, telles que $N_{\ell}$ contienne $B_{\ell}$ pour tout $\ell \in L$. La réunion U de la famille $(f(N_{\ell}))_{\ell\in L}$ est ouverte dans A et contient B. L’ensemble U-B est la réunion des ensembles ouverts deux à deux disjoints $f(N_{\ell}-B_{\ell})$, pour $\ell \in L$.

#### Lemme 2 {#ta-iv-s5-lem-2 .statement tag=023S}

L’application $f: C\rightarrow A$ est propre et séparée ; ses fibres sont finies.

Démontrons que $f$ est fermée. Soit X une partie fermée de C. Prouvons que son image est fermée dans A. Pour tout $\ell \in L$, $X\cap B_{\ell}$ est fermé dans $B_{\ell}$ donc l’espace $Y =\bigcup_{\ell\in L}h^{-1}_{\ell}(X\cap B_{\ell})$ est fermé dans B puisque L est fini. Le saturé $X^*$ de X pour la relation d’équivalence R est alors égal à $X\cup \bigcup_{\ell\in L}h_k(Y)$, donc est fermé dans C. Par suite, $f(X) =f(X^*)$ est fermé dans A, ce qu’il fallait démontrer.

Les fibres de $f$ sont les classes d’équivalences de la relation R ; elles sont finies. Par suite, l’application $f$ est propre (TG, I, p. 75, théo-rème 1).

Montrons enfin que $f$ est séparée. Soient $x$ et $y$ des points distincts de C qui ont même image par $f$. Il existe donc un point $b\in B$ et des éléments distincts $\ell$ et $m\in L$ tels que $x=h_{\ell}(b)$ et $y=h_m(b)$. Par conséquent, $N_{\ell}$ et $N_m$ sont des voisinages disjoints de $x$ et $y$ dans C, d’où l’assertion voulue en vertu de la prop. 1 de I, p. 25.

Faisons en outre les hypothèses suivantes :

– l’espace A est délaçable et connexe ;

– l’espace C est délaçable ;

– l’espace B est connexe et localement connexe par arcs.

Posons $I =\pi_0(C)$; si $i$ est un élément de I, désignons par $C_i$ la composante connexe $i$ de C. Notons $\eta : L\rightarrow I$ l’application qui, à un élément $\ell \in L$, associe la composante connexe de C qui contient $B_{\ell}$. L’application $\eta$ est surjective. En effet, raisonnons par l’absurde et considérons une composante connexe X de C qui ne rencontre aucun ensemble $B_{\ell}$. C’est une partie ouverte et fermée de C, saturée pour la relation d’équivalence R. Par suite, son image $f(X)$ est une partie ouverte et fermée de A, disjointe de B. Puisque A est supposé connexe et B non vide, $f(X)$ est vide, d’où une contradiction.

Soit $\sigma : I\rightarrow L$ une section de l’application $\eta$; on pose $\tau =\sigma \circ \eta$ et $T =\sigma (I)$.

Choisissons un point $b$ de B. Pour tout $\ell \in L$, posons $b_{\ell}=h_{\ell}(b)$ et choisissons la classe $\beta_{\ell}$ d’un chemin reliant $b_{\ell}$ à $b_{\tau(\ell)}$ dans C ; si $\ell =\tau (\ell )$, on choisit pour $\beta_{\ell}$ la classe du chemin constant d’image $b_{\ell}$. Pour tout $\ell \in L$, on note $\vartheta_{\ell}$ l’homomorphisme de $\pi_1(B, b)$ dans $\pi_1(C, b_{\tau(\ell)})$ défini par

$\vartheta_{\ell}(v) =$ Int($\beta_{\ell}$)$^{-1}((h_{\ell})_*(v)) =\beta_{\ell}^{-1}(h_{\ell})_*(v)\beta_{\ell}$,

pour tout $v\in \pi_1(B, b)$. Fixons enfin un élément $\ell_0$ de L tel que $\ell_0=$ $\tau (\ell_0)$.

Soit $\mathsf{Q}$ l’unique homomorphisme de groupes

$$
\mathsf{Q}:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)\rightarrow \pi_1(A, b)
$$

tel que $\mathsf{Q}(\ell ) =f_*(\beta_{\ell})$ pour tout $\ell \in$ L - T et qui coïncide avec $\pi_1(f, b_{\sigma(i)})$ dans $\pi_1(C_i, b_{\sigma(i)})$ pour tout $i\in I$.

#### Proposition 5 (Van Kampen) {#ta-iv-s5-prop-5 .statement tag=023T}

L’homomorphisme $\mathsf{Q}$ est surjectif ; son noyau est le plus petit sous-groupe distingué contenant les éléments

$\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$ pour $v\in \pi_1(B, b)$ et $\ell \in T$,

$\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$ pour $v\in \pi_1(B, b)$ et $\ell \in L-T$.

L’application $f: C\rightarrow$ A est propre, séparée, à fibres finies (IV, p. 430, lemme 2) ; les espaces A et C sont délaçables. En outre, $C\times_AC$ est la réunion de la diagonale $\Delta_C$ et des parties disjointes $B_{\ell}\times_AB_k=$ $(h_{\ell}, h_k)(B)$, pour $(\ell , k)\in L^2$ avec $\ell =\not k$. Pour un tel couple $(\ell , k)$, on a $B_{\ell}\times_AB_k= N_{\ell}\times_AN_k$; par suite, cette partie est ouverte et fermée dans $C\times_AC$. La diagonale $\Delta_C$ est ainsi ouverte et son complémentaire dans $C\times_AC$, réunion finie de parties disjointes homéomorphes à B, est localement connexe. Cela prouve que l’application $f$ vérifie la propriété (VK) (cas (ii) de IV, p. 405). En vue d’appliquer le th. 1 de IV, p. 408, nous allons définir une donnée de van Kampen pour $f$.

Pour tout $i\in I$, choisissons pour point-base dans $C_i$ le point $\mathsf{a}(i) =$ $b_{\sigma(i)}$.

Soit J l’ensemble des composantes connexes par arcs de $C\times_AC$. Les ensembles $\Delta_{C_i}$, pour $i\in I$, sont les composantes connexes de la diagonale $\Delta_C$, laquelle est ouverte et fermée dans $C\times_AC$, donc ces ensembles appartiennent à J. De même, les ensembles $[\ell_1, \ell_2] = B_{\ell_1}\times_A$ $B_{\ell_2}$ pour $\ell_1$ et $\ell_2$ dans L avec $\ell_1=\not\ell_2$, appartiennent à J. Comme ces ensembles forment une partition de $C\times_AC$, ils décrivent l’ensemble J.

Soit $j$ un élément de J de la forme $\Delta_{C_i}$, pour $i\in I$. Choisissons pour point-base $\mathsf{b}(j)$ le point $(\mathsf{a}(i),\mathsf{a}(i)) = (b_{\sigma(i)}, b_{\sigma(i)})$ et prenons pour classes de chemins $\beta_1(j)$ et $\beta_2(j)$ la classe du chemin constant en $b_{\sigma(i)}$. Soit $j$ un élément de J de la forme $[\ell_1, \ell_2]$, où $\ell_1$ et $\ell_2$ sont des éléments de L, distincts. Posons alors $\mathsf{b}([\ell_1, \ell_2]) = (b_{\ell_1}, b_{\ell_2}),\beta_1([\ell_1, \ell_2]) =\beta_{\ell_1}$ et $\beta_2([\ell_1, \ell_2]) =\beta_{\ell_2}$.

Soit $K =\pi_0(C\times_AC\times_AC)$.

Notons $\Delta '_C$ la diagonale de l’espace $C\times_AC\times_AC$ ; c’est une partie fermée de $C\times_AC\times_AC$, car $f$ est séparée, elle est homéomorphe à C. Pour tout $i\in$ I, notons aussi $\Delta '_{C_i}$ l’image de $C_i$ par l’application diagonale de C dans $C\times_AC\times_AC$ ; ce sont des parties ouvertes et fermées dans $\Delta '_C$. Pour tout triplet $(\ell_1, \ell_2, \ell_3)$ d’éléments de L, posons aussi $[\ell_1, \ell_2, \ell_3] = B_{\ell_1}\times_AB_{\ell_2}\times_AB_{\ell_3}$; ce sont des parties fermées de $C\times_A$ $C\times_AC$, homéomorphes à B. Si l’ensemble $\{\ell_1, \ell_2, \ell_3\}$ a au moins deux éléments, on a $[\ell_1, \ell_2, \ell_3] = N_{\ell_1}\times_AN_{\ell_2}\times_AN_{\ell_3}$, ce qui entraîne que $[\ell_1, \ell_2, \ell_3]$ est aussi ouvert dans $C\times_AC\times_AC$. En outre, $C\times_AC\times_AC$ est la réunion des parties deux à deux disjointes $\Delta '_C$ et $[\ell_1, \ell_2, \ell_3]$, où $(\ell_1, \ell_2, \ell_3)$ parcourt l’ensemble des triplets d’éléments de L qui ne sont pas tous égaux à un même élément. Ainsi, $\Delta_{C'}$, puis les $\Delta '_{C_i}$, pour $i\in I$, sont ouvertes et fermées dans $C\times_AC\times_AC$. Cela entraîne que l’ensemble K des composantes connexes de cet espace est la réunion des ensembles disjoints $K_0$ et $K_1$ suivants.

L’ensemble $K_0$ est l’ensemble des composantes de la forme $\Delta '_{C_i}$. Soit $i\in I$ et soit $k= \Delta '_{C_i}$. On pose $\mathsf{c}(k) = (b_{\sigma(i)}, b_{\sigma(i)}, b_{\sigma(i)})$. Pour $(s, t)\in  \{(1,2),(2,3),(1,3)\}$, on choisit pour $\gamma_{st}(k)$ la classe du chemin constant en $(b_{\sigma(i)}, b_{\sigma(i)})$.

L’ensemble $K_1$ est constitué des composantes de la forme $k$ = $[\ell_1, \ell_2, \ell_3]$, où $\ell_1, \ell_2, \ell_3$ sont trois éléments de B tels que l’ensemble $\{\ell_1, \ell_2, \ell_3\}$ soit de cardinal $\geqslant 2$. On pose $\mathsf{c}(k) = (b_{\ell_1}, b_{\ell_2}, b_{\ell_3})$. Soit $(s, t)\in  \{(1,2),(1,3),(2,3)\}$. Si $\ell_s=\ell_t$, on prend pour $\gamma_{st}(k)$ la classe $(\beta_{\ell_s}, \beta_{\ell_t})$ ; si $\ell_s=\not\ell_t$, on prend pour $\gamma_{st}(k)$ la classe du chemin constant en $(b_{\ell_s}, b_{\ell_t})$.

On vérifie alors que, pour tout $k\in K$ et pour tout $s\in  \{1,2,3\}$, la classe de lacets $\lambda_s(k)$ définie par la relation (2) de IV, p. 407, est triviale.

L’armature $\mathsf{\Gamma}$ du couple de morphismes de groupoïdes $(\varpi (p_1), \varpi (p_2))$ de $\varpi (C\times_AC)$ dans $\varpi (C)$ a pour sommets l’ensemble I et pour arêtes orientées l’ensemble J. Si $i\in I$, la flèche $j= \Delta_{C_i}$ a pour origine et terme $i$; si $(\ell_1, \ell_2)$ est un couple d’éléments de L distincts, la flèche $j= [\ell_1, \ell_2]$ a pour origine $\eta (\ell_1)$ et pour terme $\eta (\ell_2)$.

Soit $\mathsf{T}$ le sous-carquois de $\mathsf{\Gamma}$ dont l’ensemble de sommets est I et dont les flèches sont celles de la forme $[\ell_0, \ell ]$, pour $\ell \in T-\{\ell_0\}$. Le graphe associé à $\mathsf{T}$ est un arbre maximal de $\widetilde{\mathsf{\Gamma }}$.

Posons $i_0=\eta (\ell_0)$.

Si $i\in I-\{i_0\}$, l’unique chemin de $\mathsf{T}$ reliant $i_0$ à $i$ est $(i_0,[\ell_0, \sigma (i)], i)$. Le morphisme de groupoïdes de Grp($\mathsf{\Gamma}$) dans $\varpi (Y)$ défini p. 407 (et noté $\tau$ en loc. cit.) applique $j$ sur l’élément neutre si $j= \Delta_{C_i}$, pour $i\in I$, et applique $j= [\ell_1, \ell_2]$ sur $f_*(\beta_{\ell_1})^{-1}f_*(\beta_{\ell_2})$, si $\ell_1$ et $\ell_2$ sont des éléments de L distincts. Pour tout $i\in I$, la classe de chemins $\delta_i$ définie loc. cit. et reliant $b=f(b_{\sigma(i_0)})$ à $b=f(b_{\sigma(i)})$ est donnée par

$$
\delta_i=f_*(\beta_{\ell_0})^{-1}f_*(\beta_{\sigma(i)}) =e
$$

car $\beta_{\ell}=e$ si $\ell \in T$.

On a ainsi défini une donnée de van Kampen de l’application $f$. Considérons alors l’unique homomorphisme de groupes

$$
\mathsf{Q}':(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow \pi_1(A, b)
$$

qui coïncide avec $\pi_1(f, b_{\sigma(i)})$ dans $\pi_1(C, b_{\sigma(i)})$ et tel que

$$
\mathsf{Q}'(j) =f_*(\beta_1(j))^{-1}f_*(\beta_2(j))
$$

pour $j\in J$. D’après IV, p. 408, th. 1, cet homomorphisme est surjectif et son noyau est le plus petit sous-groupe distingué contenant les relateurs $\mathsf{r}_1(j)$ (pour $j\in$ Fl($\mathsf{T}$)), $\mathsf{r}_2(j, v)$ (pour $j\in$ J et $v\in$ $\pi_1(C\times_AC,\mathsf{b}(j))$) et $\mathsf{r}_3(k)$ (pour $k\in K$) définis, loc. cit., par les équations ($R_1$)$, (R_2)$ et ($R_3$).

Soit $q'$ l’unique homomorphisme de F(L) dans F(L - T) tel que $q'(\ell ) =\ell$ si $\ell \in L-T$ et $q'(\ell ) =e$ sinon. Soit

$$
q:(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(J)\rightarrow (_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)
$$

l’unique homomorphisme de groupes qui coïncide avec l’identité sur $\pi_1(C_i, b_{\sigma(i)})$, pour $i\in$ I et tel que l’on ait $q(j) =e$ si $j= \Delta_{C_i}$, $q([\ell , \ell ']) =q'(\ell )^{-1}q'(\ell ')$ si $\ell$ et $\ell '$ sont des éléments de L, distincts. L’homomorphisme $q$ est surjectif.

Si $i\in I$ et $j= \Delta_{C_i}$, on a $\mathsf{Q}'(j) =e_b=\mathsf{Q}'(q(j))$. Si $j= [\ell , \ell ']$, pour $\ell$ et $\ell '$ dans L, distincts, on a

$$
\mathsf{Q}'(j) =f_*(\beta_{\ell})^{-1}f_*(\beta_{\ell'}) =\mathsf{Q}(q'(\ell ))^{-1}\mathsf{Q}(q'(\ell '))
$$

$$
=\mathsf{Q}(q'(\ell )^{-1}q'(\ell ')) =\mathsf{Q}\circ q([\ell , \ell '])
$$

Par suite, $\mathsf{Q}'$ = $\mathsf{Q}\circ q$. Il en résulte que l’homomorphisme $\mathsf{Q}$ est surjectif et que son noyau est le plus petit sous-groupe distingué de $(_i*_{\in I}\pi_1(C_i, b_{\sigma(i)}))*F(L-T)$ contenant les images par $q$ des relateurs $\mathsf{r}_1(j)$ (pour $j\in$ Fl($\mathsf{T}$))$,\mathsf{r}_2(j, v)$ (pour $j\in J$ et $v\in \pi_1(C\times_AC,\mathsf{b}(j))$) et $\mathsf{r}_3(k)$ (pour $k\in K$).

Si $\ell \in T-\{\ell_0\}$ et $j= [\ell_0, \ell ]$, on a $\mathsf{r}_1(j) =j$ et $q(\mathsf{r}_1(j)) =e$.

Soit $k\in K$. On a $\mathsf{r}_3(k) =j_{12}(k)j_{23}(k)j_{13}(k)^{-1}$. Si $k= \Delta '_{C_i}$, pour $i\in I$, posons $j= \Delta_{C_i}$; alors, on a

$$
q(\mathsf{r}_3(k)) =q(jjj^{-1}) =q(j) =e
$$

Soient $\ell$ et $\ell '$ des éléments de L, distincts. Si $k= [\ell , \ell , \ell ']$, on a donc

$$
q(\mathsf{r}_3(k)) =q(\Delta_{C_{\eta(\ell)}}[\ell , \ell '][\ell , \ell ']^{-1}) =q(\Delta_{C_{\eta(\ell)}}) =e
$$

Si $k= [\ell , \ell ', \ell ]$, il vient

$$
q(\mathsf{r}_3(k)) =q([\ell , \ell '][\ell ', \ell ]\Delta^{-1_{(\ell)}}_{C_{\eta}})
$$

$$
=q'(\ell )^{-1}q'(\ell ')q'(\ell ')^{-1}q'(\ell )q(\Delta_{C_{\eta}(\ell)})^{-1}=e
$$

En outre, si $k= [\ell ', \ell , \ell ]$, on a

$$
q(\mathsf{r}_3(k)) =q([\ell ', \ell ]\Delta_{C_{\eta(\ell)}}[\ell ', \ell ]^{-1})
$$

$$
=q(\ell ')^{-1}q(\ell )q(\Delta_{C_{\eta(\ell)}})q(\ell )^{-1}q(\ell ') =e
$$

Enfin, si $k= [\ell_1, \ell_2, \ell_3]$, où $\ell_1, \ell_2, \ell_3$ sont des éléments de L, deux à deux distincts, on a

$$
q(\mathsf{r}_3(k)) =q([\ell_1, \ell_2])q([\ell_2, \ell_3])q([\ell_1, \ell_3])^{-1}=e
$$

Soit $i\in I$ et posons $j= \Delta_{C_i}$. Les homomorphismes de groupes $\varphi_j$ et $\psi_j$, de $\pi_1(C\times_AC,\mathsf{b}(j)) =\pi_1(C_i,\mathsf{a}(i))$ dans $\pi_1(C,\mathsf{a}(i))$ définis par les relations (1) de IV, p. 407, sont égaux respectivement à $(p_1)_*$ et à $(p_2)_*$. On a alors, pour $v\in \pi_1(C_i,\mathsf{a}(i)),\mathsf{r}_2(j, v) =vjv^{-1}j^{-1}$, d’où $q(\mathsf{r}_2(j, v)) =e$.

Soit enfin $j= [\ell , \ell ']$, où $\ell$ et $\ell '$ sont des éléments de L, distincts. L’homomorphisme de groupes $\varphi_j:\pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))\rightarrow \pi_1(C_{\eta(\ell)}, b_{\tau(\ell)})$ défini loc. cit. est l’homomorphisme $\vartheta_{\ell}$, et l’homomorphisme $\psi_j$ est l’homomorphisme $\vartheta_{\ell'}$. On a alors, pour $v\in \pi_1(B_{\ell}\times_AB_{\ell'},\mathsf{b}(j))$

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)q'(\ell )^{-1}q'(\ell ')\vartheta_{\ell'}(v)^{-1}q'(\ell ')^{-1}q'(\ell )
$$

Distinguons quatre cas. Si $\ell$ et $\ell '$ appartiennent tous deux à T, on a

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})
$$

Lorsque $\ell '=\ell_0$, on obtient l’inverse de l’élément $\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1}$. Si $\ell \in T$ mais $\ell '\notin T$, on a

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

$$
=(\vartheta_{\ell_0}(v)\vartheta_{\ell}(v)^{-1})^{-1}\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1}
$$

De même, si $\ell \notin T$ et $\ell '\in T$, on a

$$
q(\mathsf{r}_2(j, v)) =\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell'}(v)^{-1}\ell
$$

$$
=\ell^{-1}(\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1})^{-1}(\vartheta_{\ell_0}(v)\vartheta_{\ell'}(v)^{-1})\ell
$$

En prenant $\ell '=\ell_0$, on obtient un élément conjugué à l’inverse de $\vartheta_{\ell_0}(v)\ell \vartheta_{\ell}(v)^{-1}\ell^{-1}$. Enfin, si ni $\ell$ ni $\ell '$ n’appartiennent à T, on a

$$
q(\mathsf{r}_2(j, v)) =(\vartheta_{\ell}(v)\ell^{-1}\vartheta_{\ell_0}(v)^{-1}\ell )\ell^{-1}(\vartheta_{\ell_0}(v)\ell '\vartheta_{\ell'}(v)^{-1}(\ell ')^{-1})\ell
$$

Ces relations démontrent, d’une part, que les éléments annoncés dans la proposition appartiennent au noyau de l’homomorphisme $\mathsf{Q}$, et, d’autre part, que ces éléments $q(\mathsf{r}_2(j, v))$ appartiennent tous au plus petit sous-groupe distingué contenant les éléments annoncés par l’énoncé. La proposition en résulte.

#### Remarque {#ta-iv-s5-n6-rem-1 .statement tag=023U}

Soit A un espace topologique, soit B une partie fermée de A et soit U un voisinage ouvert de B dans A. On suppose que l’ensemble U-B est la réunion d’une famille finie $(M_{\ell})_{\ell\in L}$ d’ensembles ouverts deux à deux disjoints. Pour tout $\ell \in L$, on pose $N'_{\ell}= M_{\ell}\cup B$. Notons $C'$ l’espace topologique somme des espaces A-B et $N'_{\ell}$, pour $\ell \in L$ ; on note aussi $\varphi : A-B\rightarrow C'$ et $\varphi_{\ell}: N'_{\ell}\rightarrow C'$, pour $\ell \in L$, les injections canoniques. Soit C l’espace topologique quotient de $C'$ par la relation d’équivalence S la plus fine pour laquelle les points $\varphi (x)$ et $\varphi_{\ell}(x)$ sont équivalents, pour tout $\ell \in L$ et tout $x\in M_{\ell}$; soit $\rho : C'\rightarrow C$ l’application canonique.

Démontrons que l’on retrouve l’espace A à partir de l’espace C par identification des ensembles $B_{\ell}$ au moyen des homéomorphismes $\rho \circ$ $(\varphi_{\ell}|B): B\rightarrow B_{\ell}$.

Pour tout $\ell \in L$, l’ensemble $M_{\ell}$ est ouvert dans A-B et dans $N'_{\ell}$. Les applications $\rho \circ \varphi$ et $\rho \circ \varphi_{\ell}$ sont des des homéomorphismes des espaces A-B et $N'_{\ell}$, pour $\ell \in L$, sur des parties ouvertes de C (TG, I, p. 17, prop. 9). Pour tout $\ell \in L$, l’ensemble $\varphi_{\ell}(B)$ est fermé dans $C'$ et saturé pour la relation d’équivalence S. Par suite, l’ensemble $B_{\ell}=\rho (\varphi_{\ell}(B))$ est fermé dans C et l’application $\rho \circ \varphi_{\ell}$ induit un homéomorphisme de B sur $B_{\ell}($loc. cit.). De même, pour tout $\ell \in L$, l’ensemble $N_{\ell}=\rho (\varphi_{\ell}(N'_{\ell}))$ est un voisinage ouvert de $B_{\ell}$; les ensembles $N_{\ell}$ sont mutuellement disjoints.

Par passage au quotient, l’application $f': C'\rightarrow A$ déduite des injections canoniques dans A des espaces A-B et $N_{\ell}$, pour $\ell \in L$, induit une

application continue $f: C\rightarrow A$. Si $x$ est un point de B, la fibre $\overset{-1}{f}(x)$ est l’ensemble des points $\rho (\varphi_{\ell}(x))$, pour $\ell \in L$. La relation d’équivalence sur C associée à l’application $f$ est la relation R définie au début du numéro. Notons $B_L$ la réunion de la famille $(B_{\ell})_{\ell\in L}$. Par construction, l’application $f$ induit un homéomorphisme de $C-B_L$ sur A-B et, pour $\ell \in L$, un homéomorphisme de $N'_{\ell}$ sur $N_{\ell}$. Nous allons démontrer que l’application $f$ est fermée ; la topologie de A sera donc la topologie quotient de C par la relation d’équivalence R (I, p. 18, exemple 2). Pour cela, démontrons que si F est une partie de A telle que $F\cap (A-B)$ soit fermé dans A-B et telle que $F\cap N'_{\ell}$ soit fermé dans $N'_{\ell}$, pour $\ell \in L$, l’ensemble F est fermé dans A. L’ensemble U, réunion de la famille $(N'_{\ell})_{\ell\in L}$ est ouvert dans A et les ensembles $N'_{\ell}$, pour $\ell \in L$, en constituent un recouvrement fermé fini. Par suite, l’ensemble $F\cap U$ est fermé dans U (TG, I, p. 18, prop. 3). Les ensembles U et A-B forment un recouvrement ouvert de A, l’ensemble F est donc fermé dans A (loc. cit.).

## EXERCICES {#ta-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
