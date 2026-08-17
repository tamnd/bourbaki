---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 5
section_title: Coégalisateur
lang: fr
source: ta-i-iv-fr
book_pages: A II.196-A II.214, A II.227-A II.228
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
content_sha256: 4c7139c74bd316bb578998218cff570e16b782d3a06c0a047cef2419d39beb3c
---

## § 5. COÉGALISATEUR

### 1. Contraction des flèches d’une homotopie

Soit H un carquois, soit G un groupoïde, soient $\varphi$ et $\psi$ des morphismes de carquois de H dans G, et soit $h:$ Som(H) $\rightarrow$ Fl(G) une homotopie reliant $\varphi$ à $\psi$. Soit $G'$ le groupoïde déduit de G par contraction des flèches de l’image de $h($II, p. 175, n$^o11$) et soit $\beta : G\rightarrow G'$ le morphisme canonique.

Notons Γ le carquois (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )). Par définition d’une homotopie, le couple (Id$_{Som(G)}, h)$ est un morphisme de carquois de Γ dans G ; il se prolonge en un unique morphisme de groupoïdes $\eta :$ Grp(Γ) $\rightarrow$ G. Par construction, l’ensemble des sommets de $G'$ est l’ensemble des composantes connexes du carquois Γ.

Dans toute la suite de ce n$^o$, nous supposerons que le groupoïde G est transitif. D’après la remarque 1 de II, p. 170, cela revient à supposer que le groupoïde $G'$ l’est. On fixe aussi un sommet $a_0$ de G.

Notons $\widetilde{\Gamma}$ le graphe associé au carquois Γ (cf. II, p. 156). L’ensemble des lacets de longueur $\geqslant 1$ dans $\widetilde{\Gamma}$ s’identifie à l’ensemble $\Omega (\widetilde{\Gamma})$ des suites finies $(z_1, . . . , z_n)$, où $n$ est un entier tel que $n\geqslant 1$ et $z_1, . . . , z_n$ sont des éléments de Fl($\widetilde{\Gamma}$) tels que $t(z_i) =o(z_{i+1})$ pour tout entier $i$ tel que $1\leqslant i < n$ et $t(z_n) =o(z_1)$.

Soit $\mathbf{z}= ((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ un élément de $\Omega (\widetilde{\Gamma})$. La classe de conjugaison de l’élément

Int($g$)$(\eta (\mathbf{z})) =gh(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}g^{-1}$

dans $G_{a_0}$ ne dépend pas du choix de la flèche $g$ de G reliant le sommet $a_0$ à l’origine de $(b_1, \varepsilon )$. On note $c(\mathbf{z})$ cette classe de conjugaison.

#### Proposition 1 {#ta-ii-s5-prop-1 .statement tag=01UI}

Le morphisme de groupes $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$ est surjectif, son noyau est le plus petit sous-groupe de $G_{a_0}$ contenant les classes de conjugaison $c(\mathbf{z})$ pour $\mathbf{z}\in \Omega (\widetilde{\Gamma})$.

Soit K le plus petit sous-groupoïde distingué de G dont l’ensemble des flèches contient l’image de $h$. Le morphisme $G_{a_0}\rightarrow G'_{\beta(a_0)}$ est surjectif et son noyau est égal à $K_{a_0}($II, p. 170, prop. 2). La proposition résulte alors de la prop. 8 de II, p. 176.

#### Définition 1 {#ta-ii-s5-def-1 .statement tag=01UJ}

On dit qu’une partie Z de $\Omega (\widetilde{\Gamma})$ est distinguée (relativement au couple $(\varphi , \psi )$) si elle vérifie les propriétés suivantes :

(i) Pour toute flèche $z$ de $\widetilde{\Gamma}$, on a $(z, z)\in Z$ ;

(ii) Pour tout $(z_1, . . . , z_n)\in$ Z, on a $(\overline{z}_n, . . . , z_2, z_1)\in$ Z et $(z_n, z_1, . . . , z_{n-1})\in Z$ ;

(iii) Soient $\mathbf{z}= (z_1, . . . , z_n)$ et $\mathbf{z}'= (z'_1, . . . , z'_m)$ des éléments de Z tels que $t(z_n) =o(z'_1)$. Posons $\mathbf{z}\mathbf{z}'= (z_1, . . . , z_n, z'_1, . . . , z'_m)$. Si deux éléments parmi $\mathbf{z},\mathbf{z}',\mathbf{z}\mathbf{z}'$ appartiennent à Z, il en est de même du troisième ;

(iv) Pour toute flèche $f$ de H, posons $\widetilde{\varphi}(f,1) =\widetilde{\psi}(f,-1) =$ $\varphi (f)$ et $\widetilde{\varphi}(f,-1) =\widetilde{\psi}(f,1) =\psi (f)$. Soient $n$ un entier $\geqslant$ 1 et $(f_1, \varepsilon_1), . . . ,(f_n, \varepsilon_n)$ une suite d’éléments de Fl(H) $\times  \{-1,1\}$ telle que $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ pour $1\leqslant i < n$ et $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$ ; notons $a_i$ l’origine de $f_i$ et $b_i$ son terme. Pour que $((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ appartienne à Z, il faut et il suffit que $((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ appartienne à Z.

L’intersection dans $\Omega (\widetilde{\Gamma})$ de toute famille de parties distinguées (relativement à $(\varphi , \psi )$) l’est encore. En particulier, il existe une plus petite partie distinguée contenant une partie Z donnée de $\Omega (\widetilde{\Gamma})$.

#### Proposition 2 {#ta-ii-s5-prop-2 .statement tag=01UK}

Si N est un sous-groupe distingué de $G_a$, l’ensemble des éléments $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ tels que $c(\mathbf{z})$ soit contenu dans N est une partie distinguée de $\Omega (\widetilde{\Gamma})$.

Notons Z l’ensemble des éléments $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ tels que $c(\mathbf{z})\subset N$.

Soit $z\in$ Fl($\widetilde{\Gamma}$). On a $c(z, z) =\{e_a\}$ par définition, d’où $(z, z)\in Z$.

Soit $(z_1, . . . , z_n)\in Z$. Par définition de $c$, la classe de conjugaison $c(z_1, . . . , z_n)$ est égale à $c(z_n, z_1, . . . , z_{n-1})$ et est formée des inverses des éléments de $c(\overline{z}_n, . . . , z_1)$. Cela montre que Z vérifie la condition (ii).

Avec les notations de la condition (iii), on peut choisir des éléments $u\in c(\mathbf{z}),v\in c(\mathbf{z}')$ et $w\in c(\mathbf{z}\mathbf{z}')$ tels que $uv=w$. Si deux des éléments $u,v$ et $w$ appartiennent à N, il en est de même du troisième, donc N satisfait à (iii).

Les notations étant celles de (iv), on a, pour tout entier $i$ tel que $1\leqslant i\leqslant n$, la relation

$$
\varphi (f_i)h(b_i) =h(a_i)\psi (f_i)
$$

car $h$ est une homotopie reliant $\varphi$ à $\psi$. Cette égalité s’écrit aussi

$$
\widetilde{\varphi}(f_i, \varepsilon_i)h(b_i)^{\varepsilon_i}=h(a_i)^{\varepsilon_i}\widetilde{\psi}(f_i, \varepsilon_i)
$$

Compte tenu des relations $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ pour $1\leqslant i < n$ et $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$, on en déduit

$$
\widetilde{\varphi}(f_1, \varepsilon_1)h(b_1)^{\varepsilon_1}. . . h(b_n)^{\varepsilon_n}=h(a_1)^{\varepsilon_1}. . . h(a_n)^{\varepsilon_n}\widetilde{\varphi}(f_1, \varepsilon_1)
$$

si bien que les classes de conjugaison $c((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ et $c((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ sont égales. Cela montre que Z satisfait à la condition (iv) et termine la démonstration de la proposition.

#### Corollaire {#ta-ii-s5-n1-cor-1 .statement tag=01UL}

Soit Z une partie de $\Omega (\widetilde{\Gamma})$; pour que les classes de conjugaison $c(\mathbf{z})$, pour $\mathbf{z}\in$ Z, engendrent le noyau de l’homomorphisme canonique $\beta_{a_0}: G_{a_0}\rightarrow G'_{\beta(a_0)}$, il suffit que la plus petite partie distinguée de $\Omega (\widetilde{\Gamma})$ contenant Z soit égale à $\Omega (\widetilde{\Gamma})$.

Soit N le plus petit sous-groupe de $G_{a_0}$ contenant $c(\mathbf{z})$ pour tout $\mathbf{z}\in Z$ ; il est distingué. Soit $Z'$ l’ensemble des éléments $\mathbf{z}$ de $\Omega (\widetilde{\Gamma})$ tels que $c(\mathbf{z})\in N$. D’après la proposition 2, $Z'$ est une partie distinguée de $\Omega (\widetilde{\Gamma})$. Elle contient Z. Par hypothèse, elle est donc égale à $\Omega (\widetilde{\Gamma})$. Il résulte alors de la prop. 1 (II, p. 197) que N est le noyau de l’homomorphisme $\beta_a$.

### 2. Définition du coégalisateur

Soit H un carquois, soit G un groupoïde et soient $\varphi ,\psi$ des morphismes de carquois de H dans G. Notons Coh($\varphi , \psi$ ) le cohomotopeur du couple $(\varphi , \psi )$ (II, p. 185, déf. 3$),\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) le morphisme de groupoïdes canonique et $h$ l’homotopie canonique reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$.

Soit Coeg($\varphi , \psi$ ) le groupoïde déduit de Coh($\varphi , \psi$ ) par contraction des flèches appartenant à l’image de $h$ (II, p. 196, n$^o$ 1), notons $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) le morphisme canonique et posons $\gamma =\beta \circ \alpha$.

#### Définition 2 {#ta-ii-s5-def-2 .statement tag=01UM}

On dit que le groupoïde Coeg($\varphi , \psi$ ) est le coégalisateur du couple $(\varphi , \psi )$ ; le morphisme de groupoïdes $\gamma$ s’appelle le morphisme canonique de G dans Coeg($\varphi , \psi$ ).

#### Proposition 3 {#ta-ii-s5-prop-3 .statement tag=01UN}

Le couple (Coeg($\varphi , \psi$ )$, \gamma )$ possède la propriété universelle suivante :

a) On a $\gamma \circ \varphi =\gamma \circ \psi$.

b) Soient $G'$ un groupoïde et $\theta : G\rightarrow G'$ un morphisme de groupoïdes tel que $\theta \circ \varphi =\theta \circ \psi$. Il existe un unique morphisme de groupoïdes $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ tel que $\overline{\theta}\circ \gamma =\theta$.

Soit $a$ un sommet de H. La flèche $h(a)$ de Coh($\varphi , \psi$ ) relie $\alpha (\varphi (a))$ à $\alpha (\psi (a))$. Par définition du groupoïde Coeg($\varphi , \psi$ ), l’origine et le terme de la flèche $\beta (h(a))$ sont égaux ; on a donc $\gamma (\varphi (a)) =\gamma (\psi (a))$.

Soit $f$ une flèche de H ; si $a$ désigne son origine et $b$ son terme, on a ainsi

$$
\alpha (\varphi (f))\cdot h(b) =h(a)\cdot \alpha (\psi (b))
$$

En prenant l’image par $\beta$ des deux membres de cette égalité, on obtient la relation $\gamma (\varphi (f)) =\gamma (\psi (f))$. Cela démontre l’assertion a).

Démontrons b). L’application $\eta :$ Som(H) $\rightarrow$ Fl(G$')$ qui à tout sommet $a$ de H associe la flèche $e_{\theta(\varphi(a))}$ de $G'$ est une homotopie reliant $\theta \circ \varphi$ à $\theta \circ \psi$. D’après la propriété universelle des cohomotopeurs (II, p. 185, prop. 3), il existe un unique morphisme de groupoïdes $\theta_1:$ Coh($\varphi , \psi$ )$\rightarrow G'$ tel que $\theta_1\circ \alpha =\theta$ et $\theta_1(h(a)) =e_{\theta(\varphi(a))}$ pour tout sommet $a$ de H. D’après la prop. 7 de II, p. 176, cette dernière propriété implique l’existence d’un unique morphisme de groupoïdes $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow G'$ tel que $\overline{\theta}\circ \beta =\theta_1$. On a alors $\overline{\theta}\circ \gamma =\theta_1\circ \alpha =\theta$.

Inversement, si $\overline{\theta}':$ Coeg($\varphi , \psi$ )$\rightarrow G'$ est un morphisme de groupoïdes tel que $\overline{\theta}'\circ \gamma =\theta$, on a $(\overline{\theta}'\circ \beta )\circ \alpha = (\overline{\theta}\circ \beta )\circ \alpha$, d’où $\overline{\theta}'\circ \beta =\overline{\theta}\circ \beta$ d’après II, p. 185, prop. 3, d’où $\overline{\theta}'=\overline{\theta}$ d’après la prop. 7 de II, p. 176. Cela démontre l’unicité de $\overline{\theta}$, d’où l’assertion b).

#### Corollaire {#ta-ii-s5-n2-cor-1 .statement tag=01UO}

Le groupoïde Coeg($\varphi , \psi$ ) est engendré par l’image du morphisme $\gamma$.

Soit C le sous-groupoïde de Coeg($\varphi , \psi$ ) engendré par l’image de G ; notons $i$ le morphisme canonique de C dans Coeg($\varphi , \psi$ ) et $\theta : G\rightarrow C$ le morphisme tel que $i\circ \theta =\gamma$. D’après la proposition 2, il existe un unique morphisme de groupoïdes $\overline{\theta}:$ Coeg($\varphi , \psi$ )$\rightarrow C$ tel que $\overline{\theta}\circ \gamma =\theta$. Alors, $\gamma =i\circ \overline{\theta}\circ \gamma$, donc $i\circ \overline{\theta}$ est le morphisme identique de Coeg($\varphi , \psi$ ) (loc. cit.). En particulier, les applications Som($i$) et Fl($i$) sont surjectives, donc C = Coeg($\varphi , \psi$ ).

#### Remarque 1 {#ta-ii-s5-n2-rem-1 .statement tag=01UP}

L’ensemble des sommets de Coeg($\varphi , \psi$ ) est l’ensemble des composantes connexes du carquois

Γ = (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ ))

(II, p. 197). Autrement dit, c’est l’ensemble quotient de Som(G) par la relation d’équivalence la plus fine telle que $\varphi (a)$ soit équivalent à $\psi (a)$ pour tout $a\in$ Som(G).

#### Remarque 2 {#ta-ii-s5-n2-rem-2 .statement tag=01UQ}

L’application Orb($\gamma$ ), déduite de $\gamma$ par passage aux orbites, définit par passage au quotient une bijection de l’ensemble des composantes connexes de l’armature du couple $(\varphi , \psi )$ sur l’ensemble des orbites du coégalisateur. Cela résulte de II, p. 185, prop. 4 et de ce que l’application déduite de $\beta$ par passage aux orbites est bijective ( II, p. 170, remarque 1).

Par suite, l’application de Som(G) dans Orb(Coeg($\varphi , \psi$ )) déduite de $\gamma$ identifie l’ensemble des orbites de Coeg($\varphi , \psi$ ) à l’ensemble quotient de Som(G) par la relation d’équivalence engendrée par les couples $(\varphi (x), \psi (x))$ pour $x\in$ Som(H) et les couples $(o(f), t(f))$ pour $f\in$ Fl(G).

#### Remarque 3 {#ta-ii-s5-n2-rem-3 .statement tag=01UR}

L’application Fl($\gamma$ ) de Fl(G) dans Fl(Coeg($\varphi , \psi$ )) n’est en général pas surjective.

### 3. Comparaison des groupes d’isotropie du cohomotopeur et du coégalisateur

Soit H un carquois, soit G un groupoïde, soient $\varphi$ et $\psi$ des morphismes de carquois de H dans G. Notons $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ), $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) et $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) les morphismes canoniques de groupoïdes, et $h$ l’homotopie canonique reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$. On résume ces notations par le diagramme suivant

$\gamma$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )$^{\beta}$ Coeg($\varphi , \psi$ ) .

Dans toute la suite de ce n$^o$, on suppose que l’armature du couple $(\varphi , \psi )$ est un carquois connexe et on fixe un sommet $a_0$ de G. Par suite, les groupoïdes Coh($\varphi , \psi$ ) et Coeg($\varphi , \psi$ ) sont transitifs.

Notons Γ le carquois (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )), $\widetilde{\Gamma}$ le graphe associé à Γ et soit $\Omega (\widetilde{\Gamma})$ l’ensemble des suites finies $(z_1, . . . , z_n)$ de flèches de $\widetilde{\Gamma}$, avec $n\geqslant 1$, telles que le terme de $z_i$ soit l’origine de $z_{i+1}$ si $1\leqslant i < n$ et que le terme de $z_n$ soit l’origine de $z_1$. On a construit au n$^o1$ une application $\mathbf{z}\mapsto c(\mathbf{z})$ de l’ensemble $\Omega (\widetilde{\Gamma})$ dans l’ensemble des classes de conjugaison du groupe Coh($\varphi , \psi$ )$_{a_0}$.

Notons $H\times_GH$ l’égalisateur dans $H\times H$ des morphismes de carquois $\psi \circ$pr$_1$ et $\varphi \circ$pr$_2$. L’ensemble de ses sommets est l’ensemble des couples $(a, b)$ de sommets de H tels que $\psi (a) =\varphi (b)$ ; l’ensemble de ses flèches est l’ensemble des couples $(f, g)$ de flèches de H telles que $\psi (f) =\varphi (g)$ ; l’origine d’une flèche $(f, g)$ est le sommet $(o(f), o(g))$ et son terme est le sommet $(t(f), t(g))$ (cf. II, p. 153).

Notons enfin Ker($\varphi , \psi$ ) l’égalisateur de $\varphi$ et $\psi$; rappelons (II, p. 165, exemple 2) que c’est le sous-carquois de H dont les sommets $a$ sont ceux tels que $\varphi (a) =\psi (a)$ et dont les flèches sont les $f\in$ Fl(H) telles que $\varphi (f) =\psi (f)$.

#### Proposition 4 {#ta-ii-s5-prop-4 .statement tag=01US}

Soit $\mu: H\times_GH\rightarrow H$ un morphisme de carquois tel que $\varphi \circ \mu=\varphi \circ$ pr$_1$ et $\psi \circ \mu=\psi \circ$ pr$_2$. Supposons que, pour tout couple $(a, b)$ de sommets de H tels que $\varphi (a) =\varphi (b)$, il existe un sommet $c$ de H tel que $\varphi (c) =\psi (b)$ et $a=\mu(b, c)$.

Soit $A_1$ un ensemble de sommets de Ker($\varphi , \psi$ ) rencontrant chacune de ses composantes connexes et soit $Z_1$ l’ensemble des éléments de $\Omega (\widetilde{\Gamma})$ de la forme $((a,1))$, où $a\in A_1$. Soit aussi $A_2$ un ensemble de sommets de $H\times_GH$ rencontrant chaque composante connexe de $H\times_GH$ et soit $Z_2$ l’ensemble des triplets de la forme $((a,1),(b,1),(\mu(a, b),-1))$, pour $(a, b)$ décrivant $A_2$.

Alors, $\Omega (\widetilde{\Gamma})$ est la plus petite partie distinguée de $\Omega (\widetilde{\Gamma})$ qui contient $Z_1\cup Z_2$. En particulier, les classes de conjugaison $c(\mathbf{z})$ dans Coh($\varphi , \psi$ )$_{a_0}$, où $\mathbf{z}$ parcourt $Z_1\cup Z_2$, engendrent le noyau de l’homomorphisme canonique $\beta_a$ de Coh($\varphi , \psi$ )$_{a_0}$ dans Coeg($\varphi , \psi$ )$_{\beta(a_0)}$.

Notons $Z'_1,Z'_2$ et $Z'$ les plus petites parties distinguées de $\Omega (\widetilde{\Gamma})$ contenant respectivement $Z_1,Z_2$ et $Z_1\cup Z_2($II, p. 197, déf. 1). Il s’agit de démontrer que $Z'$ est égal à $\Omega (\widetilde{\Gamma})$; D’après II, p. 199, corollaire 1 de la prop. 1 de II, p. 197, la dernière assertion de la proposition en découlera.

#### Lemme 1 {#ta-ii-s5-lem-1 .statement tag=01UT}

a) Pour tout sommet $a$ de Ker($\varphi , \psi$ ), $((a,1))$ appartient à $Z'_1$.

b) Pour tout sommet $(a, b)$ de $H\times_GH$, $((a,1),(b,1),(\mu(a, b),-1))$ appartient à $Z'_2$.

a) Soit $A'_1$ l’ensemble des sommets $a$ de Ker($\varphi , \psi$ ) tels que $((a,1))$ appartienne à $Z'_1$. On a $A_1\subset A'_1$, par définition de $Z'_1$. Soit $f$ une flèche de Ker($\varphi , \psi$ ), soit $a$ son origine et $b$ son terme. Il résulte de la propriété (iv) dans la définition d’une partie distinguée (II, p. 197, déf. 1) appliquée à la suite $((f,1))$ que $a\in A'_1$ équivaut à $b\in A'_1$. Puisque $A_1$ rencontre toute composante connexe de Ker($\varphi , \psi$ ), on a $A'_1=$ Som(Ker($\varphi , \psi$ )), ce qu’il fallait démontrer.

b) Soit $A'_2$ l’ensemble des sommets $(a, b)$ de $H\times_GH$ tels que le triplet $((a,1),(b,1),(\mu(a, b),-1))$ appartienne à $Z'_2$. Par hypothèse, on a $A_2\subset A'_2$. Comme $A_2$ rencontre chaque composante connexe de $H\times_GH$, il suffit d’établir que, s’il existe une flèche $(f, f')$ reliant un sommet $(a', b')$ à un sommet $(a, b)$, alors $(a, b)$ appartient à $A'_2$ si et seulement s’il en est de même de $(a', b')$.

Posons $f''=\mu(f, f')$ ; c’est une flèche reliant $\mu(a', b')$ à $\mu(a, b)$ et l’on a $\varphi (f'') =\varphi (f)$ et $\psi (f'') =\psi (f')$. D’après la condition (iv) dans la définition d’une partie distinguée de $\Omega (\widetilde{\Gamma})$ (loc. cit.) appliquée à la suite $((f,1),(f',1),(f'',-1))$, les deux conditions

(i) le triplet $((a,1),(b,1),(\mu(a, b),-1))$ appartient à $Z'$;

(ii) le triplet $((a',1),(b',1),(\mu(a', b'),-1))$ appartient à $Z'$;

sont équivalentes. Cela montre que $(a, b)$ appartient à $A'_2$ si et seulement si $(a', b')$ appartient à $A'_2$ et conclut la démonstration du lemme.

Démontrons maintenant par récurrence sur l’entier $n\geqslant 1$ que tout élément $((a_1, \varepsilon_1),(a_2, \varepsilon_2), . . . ,(a_n, \varepsilon_n))$ de $\Omega (\widetilde{\Gamma})$ appartient à $Z'$.

A) Cas où $n= 1$.

Soit $((a, \varepsilon ))$ un élément de $\Omega (\widetilde{\Gamma})$ de longueur 1. On a $\varphi (a) =\psi (a)$, d’où $((a,1))\in Z'$ d’après le lemme 1. La condition (ii) dans la définition d’une partie distinguée entraîne alors que $((a,-1))$ appartient à $Z'$.

B) Cas où $n\geqslant 2$.

Grâce à la condition (ii) d’une partie distinguée, il suffit de traiter le cas où $\varepsilon_2= 1$. Supposons que $\varepsilon_1= 1$; alors, $(a_1, a_2)$ est un sommet de $H\times_GH$ ; posons $a=\mu(a_1, a_2)$ ; d’après le lemme 1, le triplet $((a_1,1),(a_2,1),(a,-1))$ appartient donc à $Z'$. Dans le cas où $\varepsilon_1=-1$, on a $\varphi (a_1) =\varphi (a_2)$ ; on peut donc choisir un sommet $a$ de H tel que $\mu(a_2, a) =a_1$ et le triplet $((a_2,1),(a,1),(a_1,-1))$ appartient à $Z'$, donc le triplet $((a_1,-1),(a_2,1),(a,1))$ aussi, grâce à la condition (ii) dans la définition d’une partie distinguée.

Alors, $((a, \varepsilon_1),(a_3, \varepsilon_3), . . . ,(a_n, \varepsilon_n))$ appartient à $\Omega (\widetilde{\Gamma})$ et est de longueur $n-1$. Par récurrence, c’est un élément de $Z'$. Grâce aux conditions (i), (ii) et (iii) de la définition d’une partie distinguée, on en déduit successivement que les éléments

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

appartiennent à $Z'$. Cela termine la démonstration de la proposition.

#### Corollaire {#ta-ii-s5-n3-cor-1 .statement tag=01UU}

a) Avec les notations de la proposition 4, supposons en outre que l’application (Som($\varphi$ ), Som($\psi$ )) de Som(H) dans Som(G) $\times$ Som(G) soit injective et que son image soit le graphe d’une relation d’équivalence dans Som(G). Alors, pour tout sommet $(a, b)$ de $H\times_GH$, il existe un unique sommet $c_{a,b}$ de H tel que $\varphi (c_{a,b}) =\varphi (a)$ et $\psi (c_{a,b}) =\psi (b)$.

b) Supposons de plus que pour toute flèche $(f, f')$ de $H\times_GH$, il existe une flèche $f''$ de H telle que $\varphi (f'') =\varphi (f)$ et $\psi (f'') =\psi (f')$.

Soit A un ensemble de sommets de $H\times_GH$ rencontrant chacune de ses composantes connexes. Alors, le noyau du morphisme $\beta_{a_0}$ est le plus petit sous-groupe distingué de Coh($\varphi , \psi$ )$_{a_0}$ qui contient les classes de conjugaison $c((a,1),(b,1),(c_{a,b},-1))$, pour $(a, b)\in A$.

Soit R la relation d’équivalence dans Som(G) dont le graphe est l’image de l’application (Som($\varphi$ ), Som($\psi$ )). Soit $(a, b)$ un sommet de $H\times_GH$. On a ainsi $R\{\varphi (a), \psi (a)\}$ et $R\{\varphi (b), \psi (b)\}$, d’où $R\{\varphi (a), \psi (b)\}$ puisque $\psi (a) =\varphi (b)$. Par suite, il existe un unique sommet $c$ de H tel que $\varphi (c) =\varphi (a)$ et $\psi (c) =\psi (b)$ ; on le note $\mu(a, b)$.

Pour toute flèche $(f, f')$ de $H\times_GH$, choisissons une flèche $f''$ de H telle que $\varphi (f'') =\varphi (f)$ et $\psi (f'') =\psi (f)$ et notons-la $\mu(f, f')$.

On a ainsi défini un morphisme de carquois $\mu: H\times_GH\rightarrow H$ tel que $\varphi \circ \mu=\varphi \circ$ pr$_1$ et $\psi \circ \mu=\psi \circ$ pr$_2$.

Soit $(a, b)$ un couple de sommets de H tel que $\varphi (a) =\varphi (b)$. On a $R\{\varphi (a), \psi (a)\}$ et $R\{\varphi (b), \psi (b)\}$, donc $R\{\psi (b), \psi (a)\}$. Il existe par suite un unique sommet $c$ de H tel que $\varphi (c) =\psi (b)$ et $\psi (c) =\psi (a)$. Le sommet $\mu(b, c)$ vérifie $\varphi (\mu(b, c)) =\varphi (b) =\varphi (a)$ et $\psi (\mu(b, c)) =$ $\psi (c) =\psi (a)$. On a donc $\mu(b, c) =a$ car l’application (Som($\varphi$ ), Som($\psi$ )) de Som(H) dans Som(G) $\times$ Som(G) est injective.

Soit $A_1$ l’ensemble des sommets de Ker($\varphi , \psi$ ) et soit $Z_1$ l’ensemble des éléments de $\Omega (\widetilde{\Gamma})$ de la forme $((a,1))$, pour $a\in A_1$. Posons $A_2= A$ et soit $Z_2$ l’ensemble des éléments $((a,1),(b,1),(\mu(a, b),-1))$ de $\Omega (\widetilde{\Gamma})$, pour $(a, b)\in A_2$. Notons $\widetilde{Z}$ (resp. $\widetilde{Z}_1$, resp. $\widetilde{Z}_2)$ la plus petite partie distinguée de $\Omega (\widetilde{\Gamma})$ contenant $Z_1\cup Z_2$ (resp. $Z_1$, resp. $Z_2)$.

Soit $a\in A_1$; on a $\varphi (a) =\psi (a)$ ; posons $x=\varphi (a)$. Le sommet $a$ est l’unique sommet de H tel que $\varphi (a) =\psi (a) =x$; en particulier, on a $\mu(a, a) =a$. Le triplet $((a,1),(a,1),(a,-1))$ appartient donc à $Z_2$. Il résulte alors des conditions (i) et (iii) dans la définition d’une partie distinguée que $((a,1))$ appartient à $\widetilde{Z}_2$. Par suite, on a $Z_1\subset \widetilde{Z}_2$, d’où $\widetilde{Z} =\widetilde{Z}_2$.

D’après la proposition 4, $\Omega (\widetilde{\Gamma})$ est la plus petite partie distinguée de $\Omega (\widetilde{\Gamma})$ contenant $Z_2$ et le noyau de $\beta_{a_0}$ est le plus petit sous-groupe distingué de Coh($\varphi , \psi$ )$_{a_0}$ qui contient les classes de conjugaison $c(\mathbf{z})$, pour $\mathbf{z}\in Z_2$, d’où le corollaire.

#### Exemple {#ta-ii-s5-n3-exa-1 .statement tag=01UV}

Soient X et R des espaces topologiques, soient $o$ et $t$ des applications continues de R dans X, soit C l’ensemble des couples $(f, g)\in R^2$ tels que $t(f) =o(g)$ dans R et soit $m$ une application continue de C dans R qui fait du carquois $(X,R, o, t)$ un groupoïde ; supposons en outre que l’application $f\mapsto f^{-1}$ de R dans R est continue. Les hypothèses de la proposition sont alors vérifiées si l’on pose $H =\varpi (R)$, $G =\varpi (X),\varphi =\varpi (o),\psi =\varpi (t)$ et $\mu=\varpi (m)$.

Supposons de plus que R soit le graphe d’une relation d’équivalence dans X, les applications $o$ et $t$ étant déduites des projections de $X\times X$ dans X par passage aux sous-espaces. Les hypothèses du corollaire sont alors satisfaites.

#### Remarque {#ta-ii-s5-n3-rem-1 .statement tag=01UW}

*Plus généralement, les hypothèses de la proposition sont satisfaites lorsque $(G,H, \varphi , \psi , \mu)$ est un « groupoïde de groupoïdes. » Cela signifie que G et H sont des groupoïdes, $\varphi$ et $\psi$ sont des morphismes de groupoïdes de H dans G, faisant du quadruplet $(G,H, \varphi , \psi )$ un « carquois en groupoïdes » ; enfin, $\mu$ est une loi de composition dans ce « carquois » donnée par un morphisme de groupoïdes $H\times_GH\rightarrow H$, vérifiant un certain nombre de propriétés exprimant l’associativité de la loi et le fait que toute « flèche » soit inversible. Le lecteur remarquera d’ailleurs que les applications au groupoïde fondamental étudiées dans cet ouvrage se placent toutes dans ce cas.*

### 4. Groupe d’isotropie d’un coégalisateur

Soient G et H des groupoïdes ; soient $\varphi$ et $\psi$ des morphismes de groupoïdes de H dans G. Le but de ce n$^o$ est de résumer le calcul des groupes d’isotropie du cohomotopeur (II, p. 193, prop. 6) et la comparaison des groupes d’isotropie du cohomotopeur et du coégalisateur faite au n$^o$ précédent pour en déduire le calcul des groupes d’isotropie du coégalisateur Coeg($\varphi , \psi$ ).

Notons $\alpha : G\rightarrow$ Coh($\varphi , \psi$ )$,\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) et $\gamma =\beta \circ$ $\alpha : G\rightarrow$ Coeg($\varphi , \psi$ ) les morphismes de groupoïdes canoniques. Notons $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) l’homotopie canonique ; rappelons que l’ensemble des sommets de Coh($\varphi , \psi$ ) est égal à Som(G).

Notons Γ le carquois (Som(G), Som(H), Som($\varphi$ ), Som($\psi$ )), notons alors $\varphi_0$ et $\psi_0$ les applications déduites de $\varphi$ et $\psi$ par passage aux orbites et $\Gamma_0$ l’armature (Orb(G), Orb(H)$, \varphi_0, \psi_0)$ du couple $(\varphi , \psi )$. Nous supposerons que le carquois $\Gamma_0$ est connexe et que l’ensemble de ses sommets n’est pas vide, ce qui revient à supposer que les groupoïdes Coh($\varphi , \psi$ ) et Coeg($\varphi , \psi$ ) sont transitifs.

Rappelons (cf. II, p. 192, définition 4) qu’un équipement de base consiste en la donnée d’une famille $(a, b, c_1, c_2,T, i_0)$ où : pour tout $i\in$ Orb(G)$,a(i)$ est un sommet dans l’orbite $i$ de G; pour tout $j\in$ Orb(H)$,b(j)$ est un sommet dans l’orbite $j$ de H$,c_1(j)$ et $c_2(j)$ sont des flèches de G reliant respectivement $\varphi (b(j))$ à $a(\varphi_0(j))$ et $\psi (b(j))$ à $a(\psi_0(j))$ ; T est un sous-carquois de $\Gamma_0$ dont l’arbre associé est un arbre maximal du graphe $\widetilde{\Gamma}_0$; enfin, $i_0$ est une orbite de G et on pose $a_0=a(i_0)$.

On définit alors un morphisme de carquois $\tau_0$ de $\Gamma_0$ dans Coh($\varphi , \psi$ ) tel que $\tau_0(i) =\beta (a(i))$ et $\tau_0(j) =\alpha (c_1(j))^{-1}h(b(j))\alpha (c_2(j))$ pour $i\in$ Orb(G) et $j\in$ Orb(H). Si $i$ appartient à Orb(G), soit $d_i$ l’unique classe de chemins dans le graphe $\widetilde{T}$ reliant $i_0$ à $i$ et notons $\delta_i$ son image dans Coh($\varphi , \psi$ ) par le morphisme de groupoïdes $\tau_0$.

De ces données, la prop. 6 (II, p. 193) fournit un homomorphisme surjectif

Λ: $_{i\in\pi}*_{_0(G)}G_{a(i)}*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

et décrit des générateurs de son noyau, fournissant ainsi une présentation du groupe Coh($\varphi , \psi$ )$_{a_0}$.

L’ensemble des lacets de longueur $\geqslant 1$ dans le graphe $\widetilde{\Gamma}$ associé à Γ est identifié à l’ensemble $\Omega (\widetilde{\Gamma})$ des suites $(z_1, . . . , z_n)$ de flèches de $\widetilde{\Gamma}$, indexées par $\mathbf{Z}/n\mathbf{Z}$, où $n$ parcourt l’ensemble des entiers $\geqslant 1$, telles que pour tout $k\in \mathbf{Z}/n\mathbf{Z}$, le terme de $z_k$ soit l’origine de $z_{k+1}$. Soit Z une partie de $\Omega (\widetilde{\Gamma})$ telle que les classes de conjugaison $c(z)$, pour $z\in Z$, engendrent le noyau de l’homomorphisme surjectif $\beta_{a_0}$. L’homomorphisme $\beta_{a_0}\circ \Lambda$ est surjectif ; pour en déduire son noyau, c’est-à-dire une présentation du groupe Coeg($\varphi , \psi$ )$_{\beta(a_0)}$, il reste à choisir, pour tout $z\in Z$, un élément $C(z)$ dans le groupe $*G_{a(i)}*F(\pi_0(H))$

$i\in$Orb(G)

tel que $\Lambda (C(z))$ appartienne à la classe de conjugaison $c(z)$.

Soit donc $z= (z_1, . . . , z_n)$ un élément de $\Omega (\widetilde{\Gamma})$; posons $z_k= (y_k, \varepsilon_k)$, où $y_k\in$ Fl(Γ) = Som(H) et $\varepsilon_k\in  \{\pm 1\}$. Par définition, $c(z)$ est la classe de conjugaison de l’élément

$$
gh(y_1)^{\varepsilon_1}. . . h(y_n)^{\varepsilon_n}g^{-1}
$$

du groupe Coh($\varphi , \psi$ )$_{a_0}$, où $g$ est une flèche arbitraire dans Coh($\varphi , \psi$ ) reliant $a_0$ à l’origine de $z_1$. Pour $k\in \mathbf{Z}/n\mathbf{Z}$, soit $j_k$ l’orbite de $y_k$ dans H et choisissons une flèche $f_k$ de H reliant $y_k$ au sommet $b(j_k)$. Par définition d’une homotopie, on a alors la relation

$$
h(y_k)(\alpha \circ \psi )(f_k) = (\alpha \circ \varphi )(f_k)h(b(j_k))
$$

dans le groupoïde Coh($\varphi , \psi$ ). Par suite, utilisant la définition du morphisme de carquois $\tau_0$, on a

$$
h(y_k) = (\alpha \circ \varphi )(f_k)\cdot h(b(j_k))\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \tau_0(j_k)\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
= (\alpha \circ \varphi )(f_k)\cdot (\alpha \circ c_1)(j_k)\cdot \delta_{\varphi}^{-_01}_{(j_k)}\cdot
$$

$$
\cdot \delta_{\varphi_0(j_k)}\cdot \tau_0(j_k)\cdot \delta_{\psi}^{-_01}_{(j_k)}\cdot
$$

$$
\cdot \delta_{\psi_0(j_k)}\cdot (\alpha \circ c_2)(j_k)^{-1}\cdot (\alpha \circ \psi )(f_k)^{-1}
$$

$$
=u_k\Lambda (j_k)v_k
$$

où l’on a posé

$u_k=\alpha (\varphi (f_k)c_1(j_k))\cdot \delta_{\varphi}^{-_01}_{(j_k)}$ et $v_k=\delta_{\psi_0(j_k)}\cdot \alpha (\psi (f_k)c_2(j_k))^{-1}$. Pour tout élément $k\in \mathbf{Z}/n\mathbf{Z}$, définissons des flèches $\widetilde{u}_k,\widetilde{v}_k$ dans G par

$$
h(y_k)^{\varepsilon_k}=\widetilde{u}_k\Lambda (j_k)^{\varepsilon_k}\widetilde{v}_k
$$

de sorte que

$(u_k, v_k)$ si $\varepsilon_k= 1$ ;

$$
(\widetilde{u}_k,\widetilde{v}_k) =_{--}
$$

$(v_k^1, u_k^1)$ si $\varepsilon_k=-1$.

Notons $x_k$ l’origine de la flèche $h(y_k)^{\varepsilon_k}$; son terme est alors $x_{k+1}$; soit $i_k$ l’orbite de $x_k$. Définissons alors un lacet $\lambda_k(z)$ en $a(i_k)$ dans le groupoïde G par la formule

(1)

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ si $(\varepsilon_{k-1}, \varepsilon_k) = (1,1)$;

$c_2(j_{k-1})^{-1}\psi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ si $(\varepsilon_{k-1}, \varepsilon_k) = (1,-1)$; $\lambda_k(z) =$

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\varphi (f_k)c_1(j_k)$ si $(\varepsilon_{k-1}, \varepsilon_k) = (-1,1)$;

$c_1(j_{k-1})^{-1}\varphi (f_{k-1})^{-1}\psi (f_k)c_2(j_k)$ si $(\varepsilon_{k-1}, \varepsilon_k) = (-1,-1)$. Par construction, on a

$$
\Lambda (\lambda_k(z)) =\widetilde{v}_{k-1}\widetilde{u}_k
$$

si bien que l’image par l’homomorphisme Λ de l’élément

$$
C(z) =\lambda_1(z)(j_1)^{\varepsilon_1}\lambda_2(z)(j_2)^{\varepsilon_2}. . . \lambda_n(z)(j_n)^{\varepsilon_n} \tag{2}
$$

appartient à la classe de conjugaison $c(z)$.

#### Définition 3 {#ta-ii-s5-def-3 .statement tag=01UX}

Soient G et H des groupoïdes ; soient $\varphi$ et $\psi$ des morphismes de groupoïdes de H dans G. On suppose que le groupoïde Coeg($\varphi , \psi$ ) est transitif. Soit $(a, b, c_1, c_2,T, i_0)$ un équipement de base du couple $(\varphi , \psi )$.

On appelle équipement complémentaire la donnée d’une partie Z de $\Omega (\widetilde{\Gamma})$ telle que les classes de conjugaison $c(\mathbf{z})$ pour $\mathbf{z}\in$ Z engendrent le noyau de l’homomorphisme $\beta_{a(i_0)}$ et, pour tout élément $\mathbf{z}= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))$ de Z, d’une suite $f(\mathbf{z}) = (f_1, . . . , f_n)$ de flèches dans H telle que $f_k$ relie $y_k$ au sommet $b(j_k)$, $j_k$ désignant l’orbite de $y_k$ dans H.

Un équipement complet du couple $(\varphi , \psi )$ est la donnée d’un équipement de base et d’un équipement complémentaire.

#### Proposition 5 {#ta-ii-s5-prop-5 .statement tag=01UY}

Soient G et H des groupoïdes ; soient $\varphi$ et $\psi$ des morphismes de groupoïdes de H dans G. Supposons que le groupoïde Coeg($\varphi , \psi$ ) soit transitif. Notons $\gamma : G\rightarrow$ Coeg($\varphi , \psi$ ) le morphisme de groupoïdes canonique.

Munissons le couple $(\varphi , \psi )$ d’un équipement complet

$$
(a, b, c_1, c_2,T, i_0,Z,(f(\mathbf{z}))_{\mathbf{z}\in Z})
$$

Pour $j\in$ Orb(H), soient $\varphi_j: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$ et $\psi_j: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$ les morphismes de groupes Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}$ et Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}$ respectivement, où $\varphi_0$ et $\psi_0$ désignent les applications canoniques déduites de $\varphi$ et $\psi$ par passage aux orbites. Soit $\tau$ le morphisme de l’armature $\Gamma_0$ du couple $(\varphi , \psi )$ dans Coeg($\varphi , \psi$ ) défini par Som($\tau$ )$(i) =\gamma (a(i))$ si $i\in$ Orb(G) et tel que Fl($\tau$ )$(j)$ soit le chemin $\gamma (c_1(j))^{-1}\gamma (c_2(j))$ dans Coeg($\varphi , \psi$ ). Si $i$ est une orbite de G, soit $c_i$ l’unique classe de chemins dans $\widetilde{T}$ reliant $i_0$ à $i$ et posons $\delta_i=\widetilde{\tau}(c_i)$, où $\widetilde{\tau}:$ Grp(G) $\rightarrow$ Coeg($\varphi , \psi$ ) est le morphisme de groupoïdes canonique déduit de $\tau$.

Il existe alors un unique homomorphisme de groupes

$\lambda :*G_{a(i)}*$ F(Orb(H)) $\rightarrow$ Coeg($\varphi , \psi$ )$_{\gamma(a(i_0))}$

$i\in$Orb(G)

tel que

$\lambda (f) =\delta_i\gamma_{a(i)}(f)\delta_i^{-1}$ pour $i\in$ Orb(G) et $f\in G_{a(i)}$,

$\lambda (j) =\delta_{\varphi_0(j)}\tau (j)\delta_{\psi}^{-_01}_{(j)}$ pour $j\in$ Orb(H).

L’homomorphisme $\lambda$ est surjectif ; son noyau est le plus petit sous-groupe distingué contenant les éléments suivants :

($R_1$)$r_1(j) =j$ pour $j$ dans Fl(T) ;

($R_2$)$r_2(j, f) =\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$

pour $j\in$ Orb(H) et $f\in H_{b(j)}$;

($R_3$)$r_3(z) =\lambda_1(z)j_1^{\varepsilon_1}\lambda_2(z)j_2^{\varepsilon_2}. . . \lambda_n(z)j_n^{\varepsilon_n}$

pour $z= ((y_1, \varepsilon_1), . . . ,(y_n, \varepsilon_n))\in Z$,

où les lacets $\lambda_i(z)$ sont définis par la formule (1), p. 208.

L’existence et l’unicité d’un tel morphisme résulte de la propriété universelle du produit libre d’une famille de groupes (A, I, p. 85, prop. 8). Notons $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) et $\beta :$ Coh($\varphi , \psi$ )$\rightarrow$ Coeg($\varphi , \psi$ ) les morphismes canoniques, de sorte que $\gamma$ = $\beta \circ \alpha$. Soit aussi $h:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )) l’homotopie canonique reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$. Comme $\beta$ est le morphisme de groupoïdes obtenu par contraction des flèches de l’image de $h$, on a

Fl($\tau$ )$(j) =\gamma (c_1(j))^{-1}\gamma (c_2(j)) =\gamma (c_1(j)^{-1})\beta (h(j))\gamma (c_2(j)) =\beta (\tau_0(j))$ dans Coeg($\varphi , \psi$ ), où $\tau_0: \Gamma_0\rightarrow$ Coh($\varphi , \psi$ ) désigne le morphisme de carquois déduit de l’équipement de base $(a, b, c_1, c_2,T, i_0)$. Par suite, l’homomorphisme $\lambda$ est le composé de l’homomorphisme Λ défini dans la prop. 6 (II, p. 193) et de l’homomorphisme surjectif $\beta_{a(i_0)}$. Il est en particulier surjectif.

Soit $z\in Z$ ; par construction, $\Lambda (r_3(z))$ appartient à la classe de conjugaison $c(z)$. Par définition d’un équipement complémentaire, le noyau de l’homomorphisme $\beta_{a(i_0)}$ est donc le plus petit sous-groupe distingué de Coh($\varphi , \psi$ )$_{a(i_0)}$ contenant les éléments $\Lambda (r_3(z))$ pour $z\in Z$. Comme l’homomorphisme Λ est surjectif, le noyau de l’homomorphisme $\lambda =\beta_{a(i_0)}\circ \Lambda$ est donc le plus petit sous-groupe distingué du groupe $*G_{a(i)}*F(\pi_0(H))$ contenant les générateurs du noyau

$i\in$Orb(G)

de Λ donnés par les formules ($R_1$)$, (R_2)$, ainsi que les éléments définis par les formules ($R_3$). La proposition est ainsi démontrée.

### 5. Quotient d’un groupoïde par l’action d’un groupe

Soit G un groupoïde transitif, soit K un groupe et soit $\theta : K\rightarrow$ Aut(G)$^{\circ}$ un homomorphisme de groupes de K dans le groupe opposé au groupe des automorphismes du groupoïde G. On dira que le groupe K agit à droite sur G. Si $k\in K$, on notera parfois $k^*x$ (resp. $k^*f)$ l’image d’un sommet $x$ (resp. d’une flèche $f)$ de G par l’automorphisme de groupoïdes $\theta (k)$.

Soit $|K|$ le groupoïde dont l’ensemble des sommets est K et dont l’ensemble des flèches reliant deux sommets est vide si ces sommets sont distincts, et est réduit à un élément sinon. Soit H le groupoïde produit $G\times  |K|$; un sommet de H est un couple $(a, k)$, où $a$ est un sommet de G et $k$ est un élément de K; si $f$ est une flèche de G reliant un sommet $a$ à un sommet $b$, on notera $(f, k)$ l’unique flèche de H reliant $(a, k)$ à $(b, k)$. Soit $\varphi : H\rightarrow G$ le morphisme de groupoïdes donné par la première projection et soit $\psi : H\rightarrow G$ le morphisme de groupoïdes tel que Som($\psi$ )$((a, k)) =k^*a$ et Fl($\psi$ )$((f, k)) =k^*f$ si $k\in K,a\in$ Som(G) et $f\in$ Fl(G).

Notons $G/K$ le coégalisateur Coeg($\varphi , \psi$ ) et soit $\gamma : G\rightarrow G/K$ le morphisme de groupoïdes canonique.

Soit $o$ un sommet de G. Pour $k\in K$, choisissons une flèche $c_k$ reliant $k^*o$ à $o$ dans G; il en existe car G est transitif. Pour $k\in K$, notons Fix($k$) le sous-groupoïde de G dont les sommets (resp. les flèches) sont les éléments de Som(G) (resp. de Fl(G)) fixés par $k$; choisissons un ensemble $A_k$ de sommets de Fix($k$) qui rencontrent toutes les orbites de ce groupoïde. Pour $k\in K$ et $a\in A_k$, on choisit aussi une flèche $f_{(a,k)}$ dans G reliant le sommet $a$ au sommet $o$.

#### Proposition 6 {#ta-ii-s5-prop-6 .statement tag=01UZ}

L’unique homomorphisme de groupes

$$
\lambda : G_o*F(K)\rightarrow (G/K)_{\gamma(o)}
$$

tel que $\lambda (f) =\gamma_o(f)$ pour $f\in G_o$ et $\lambda ([k]) =\gamma (c_k)$ pour $k\in K$ est surjectif. Son noyau est le plus petit sous-groupe distingué de $G_o*F(K)$ contenant les éléments suivants :

($R_2$)$r_2(k, f) = [k]^{-1}f[k](c^{-1}_kk^*(f)^{-1}c_k)$

pour $k\in K$ et $f\in G_o$;

($R'_3$)$r'_3(k, a) = [k](c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)}))$

pour $k\in K-\{e\}$ et $a\in A_k$

($R''_3$)$r''_3(k, h) = [kh]^{-1}[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})$

pour $k$ et $h\in K$.

Comme G est transitif, l’application qui à un élément $k\in K$ associe l’orbite de $(o, k)$ est une bijection de K dans l’ensemble des orbites de H. On identifie ainsi Orb(G) à $\{o\}$ et Orb(H) à K. L’armature $\Gamma_0$ du couple $(\varphi , \psi )$ s’identifie alors au carquois ayant un unique sommet $o$ et dont l’ensemble des flèches est K. Soit T le sous-carquois de $\Gamma_0$ d’ensemble de sommets $\{o\}$ et dont l’ensemble des flèches est vide ; le graphe associé est l’unique arbre maximal du graphe $\widetilde{\Gamma}_0$.

La famille $(o,(o, k)_{k\in K},(e_o)_{k\in K},(c_k)_{k\in K},T, o)$ est un équipement de base du couple $(\varphi , \psi )$.

L’application $f\mapsto (f, k)$ définit un isomorphisme du groupe d’isotropie $G_o$ sur le groupe d’isotropie $H_{(o,k)}$; par cet isomorphisme, les homomorphismes $\varphi_k$ et $\psi_k$ de $H_{(o,k)}$ dans $G_o$ définis par la prop. 5 de II, p. 208 sont donnés par

(3) $\varphi_k(f, k) =f$ et $\psi_k(f, k) =c^{-1}_kk^*(f)c_k$,

pour $k\in K$ et $f\in G_o$.

Le carquois $H\times_GH$ est l’égalisateur dans $H\times H$ des morphismes de carquois $\psi \circ$ pr$_1$ et $\varphi \circ$ pr$_2$. Il a pour sommets les couples $((a, k),(b, h))$ où $a$ et $b$ sont des sommets de G et $k$ et $h$ des éléments de K tels que $b=k^*a$, et pour flèches les couples $((f, k),(g, h))$ où $f$ et $g$ sont des flèches de G, et $k$ et $h$ des éléments de K tels que $g=k^*f$; l’origine de la flèche $((f, k),(g, h))$ est égale à $((o(f), k),(o(g), h))$ ; son terme est égal à $((t(f), k),(t(g), h))$.

On définit alors un morphisme de carquois $\mu$ de $H\times_GH$ dans H en posant $\mu((a, k),(b, h)) = (a, kh)$ et $\mu((f, k),(g, h)) = (f, kh)$. On a $\varphi \circ \mu=\varphi \circ$ pr$_1$ et $\psi \circ \mu=\psi \circ$ pr$_2$.

Soient $x$ et $y$ des sommets de H tels que $\varphi (x) =\varphi (y)$. Il existe ainsi un sommet $a$ de G et des éléments $k$ et $h$ de K tels que $x= (a, k)$ et $y= (a, h)$. Posons $z= (h^*a, h^{-1}k)$ ; on a $\mu(y, z) =x$. Cela montre que le couple $(\varphi , \psi )$ vérifie les hypothèses de la prop. 4 (II, p. 202).

Un sommet $(a, k)$ de H appartient au groupoïde Ker($\varphi , \psi$ ), égalisateur de $\varphi$ et $\psi$, si et seulement si $k^*a=a$, c’est-à-dire si $k$ appartient au fixateur du sommet $a$ dans le groupe K. Soit $A_1$ l’ensemble des couples $(a, k)$, pour $k\in K$ et $a\in A_k$; il rencontre toutes les orbites du sous-groupoïde Ker($\varphi , \psi$ ) de H. Soit $Z_1$ la partie de $\Omega (\widetilde{\Gamma})$ formée des suites de la forme $(((a, k),1))$, pour $(a, k)\in A_1$. Pour $\mathbf{z}= ((a, k),1)\in Z_1,(f_{(a,k)}, k)$ est une flèche de H qui relie $(a, k)$ à $(o, k)$. Posons $f(\mathbf{z}) = ((f_{(a,k)}, k))$.

L’ensemble $A_2$ des sommets de $H\times_GH$ de la forme $((o, k),(k^*o, h))$, pour $(k, h)\in K^2$, rencontre toutes les orbites de $H\times_GH$. Observons aussi que l’on a $\mu((o, k),(k^*o, h)) = (o, kh)$. Les flèches $(e_o, k)$, $(c_k, h)$, $(e_o, kh)$ dans H relient respectivement $(o, k)$, $(k^*o, h)$, $(o, kh)$ à $(o, k)$, $(o, h)$ et $(o, kh)$. Notons $Z_2$ l’ensemble des suites de la forme $(((o, k),1),((k^*o, h),1),((o, kh),-1))$ dans $\Omega (\widetilde{\Gamma})$ ; pour un tel élément $\mathbf{z}$ de $Z_2$, posons $f(\mathbf{z}) = ((e_o, k),(c_k, h),(e_o, kh))$.

D’après la prop. 4 de II, p. 202, l’ensemble $Z = Z_1\cup Z_2$ et la famille $(f(\mathbf{z}))_{z\in Z}$ est un équipement complémentaire.

Soit $k\in K$ et soit $a\in A_k$. L’élément $C((a, k),1)$ du groupe $G_o*F(K)$ défini par la formule (2) de II, p. 208 est égal à

$$
c^{-1}_k\psi ((f_{(a,k)}, k))^{-1}\varphi (f_{(a,k)})e_o[k] =c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)}[k] \tag{4}
$$

Soient $k$ et $h\in K$. On vérifie que l’élément

$$
C(((o, k),1),((k^*o, h),1),((o, kh),-1))
$$

du groupe $G_o*F(K)$ défini par la formule (2) de II, p. 208 est égal à

$$
[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})[kh]^{-1} \tag{5}
$$

Les éléments $r'_3(e, a)$ donnés par les relations ($R'_3$) pour $k=e$ sont tous égaux à $[e]c^{-1}_e$, élément du groupe $G_o*F(K)$ qu’on obtient en appliquant la relation ($R''_3$) à $k=h=e$. Compte tenu des relations (3), (4) et (5), la proposition résulte donc de II, p. 208, prop. 5.

#### Corollaire 1 {#ta-ii-s5-prop-6-cor-1 .statement tag=01V0}

Supposons que le groupe K soit engendré par les fixateurs des sommets de G. Alors, l’homomorphisme de groupes $\gamma_o: G_o\rightarrow (G/K)_{\gamma(o)}$ est surjectif. En outre, si le groupoïde G est simplement transitif, il en est de même du groupoïde $G/K$.

La relation ($R''_3$) implique $\lambda ([e]) =\lambda (c_e) =\gamma_o(c_e)$. Les relations ($R''_3$) entraînent alors que l’ensemble des $k\in K$ tels que $\lambda ([k])$ appartienne à l’image de $\gamma_o$ est un sous-groupe de K. Enfin, les relations ($R'_3$) montrent que, pour tout élément $k\in K$ dont le fixateur n’est pas vide, $\lambda ([k])$ appartient à l’image de $\gamma_o$. Le corollaire en résulte.

#### Remarque 1 {#ta-ii-s5-n5-rem-1 .statement tag=01V1}

On peut donner une autre description, parfois plus commode, du groupe $(G/K)_{\gamma(o)}$. Pour cela, posons $M = K\times G_o$ et définissons une loi de composition dans M par la formule

$$
(k, a)\cdot (h, b) = (kh, c^{-1}_{kh}h^*(c_ka)c_hb)
$$

pour $k,h\in K$ et $a,b\in G_o$. On vérifie que cette loi de composition est associative, que $(e, c^{-1}_e)$ est un élément neutre et que l’élément $(k^{-1}, c^{-1_1}_{k^-}(k^{-1})^*(c_ka)^{-1}c_e)$ est l’inverse de $(k, a)$. Elle munit donc M d’une structure de groupe. En outre, l’application $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ définie par $(k, a)\mapsto \lambda ([k]a)$ est un homomorphisme de groupes. Soit $\alpha '$ l’unique morphisme de groupes de $G_o*F(K)$ dans M tel que $\alpha '(f) =$ $(e, f)$ si $f\in G_o$ et $\alpha '([k]) = (k, e_o)$ si $k\in K$ ; on a $\lambda '\circ \alpha '=\lambda$.

Les relations ($R_2$) et ($R''_3$) montrent que tout élément de $(G/K)_{\gamma(o)}$ est l’image par l’homomorphisme $\lambda$ d’un élément de $G_o*F(K)$ de la forme $[k]f$, avec $f\in G_o$ et $k\in K$. Par suite, l’homomorphisme $\lambda '$ est surjectif. On vérifie en outre que l’image par $\alpha '$ d’un élément de $G_o*$ F(K) de la forme $(R_2)$ ou $(R''_3)$ est nulle. Par conséquent, le noyau de l’homomorphisme $\lambda '$ est le plus petit sous-groupe distingué de M contenant les images par $\alpha '$ des éléments de $G_o*F(K)$ de la forme ($R'_3$).

#### Corollaire 2 {#ta-ii-s5-prop-6-cor-2 .statement tag=01V2}

Supposons que le groupe K opère librement dans Som(G). Il existe alors un unique morphisme de groupes $\pi : (G/K)_{\gamma(o)}\rightarrow$ K dont le noyau contient l’image de $\gamma_o$ et tel que $\pi (\lambda ([k])) =k$ pour tout $k\in K$. De plus, $G_o\longrightarrow^{\gamma_o}(G/K)_{\gamma(o)}-\rightarrow^{\pi}$ K est une extension de K par $G_o$.

Si un tel homomorphisme de groupes $\pi$ existe, l’homomorphisme de groupes $\pi \circ \lambda$ est nécessairement égal à l’unique homomorphisme de groupes $p$ de $G_o*F(K)$ dans K tel que $p(f) =e$ pour $f\in G_o$ et $p([k]) =k$. Il est immédiat de vérifier que les éléments de $G_o*F(K)$ définis par les formules ($R_2$) et ($R''_3$) appartiennent au noyau de $p$. Par hypothèse, il n’y a pas d’élément du type ($R'_3$). Ainsi, le noyau du morphisme $\lambda$ contient celui de $p$. Par suite, il existe un unique homomorphisme de groupes $\pi : (G/K)_{\gamma(o)}\rightarrow K$ tel que $\pi \circ \lambda =p$.

Il est évident que l’homomorphisme $\pi$ est surjectif. Pour montrer que l’homomorphisme $\gamma_o$ est injectif et que son image est exactement le noyau de $\pi$, remarquons que l’homomorphisme $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ (II, p. 213, remarque 1) est un isomorphisme, car on a supposé que K opère librement dans Som(G). L’homomorphisme composé $(\lambda ')^{-1}\circ \gamma_o$ de $G_o$ dans M est donné par $f\mapsto (e, f)$, tandis l’homomorphisme $\pi \circ \lambda ': M\rightarrow K$ applique $(k, f)$ sur $k$. Le corollaire en résulte.

#### Corollaire 3 {#ta-ii-s5-prop-6-cor-3 .statement tag=01V3}

Supposons que le groupoïde G soit simplement transitif. Soit $K_0$ le sous-groupe de K engendré par les fixateurs des sommets de G. L’application de K dans $(G/K)_{\gamma(o)}$ qui à $k\in K$ associe $\gamma (c_k)$ est un homomorphisme de groupes surjectif, de noyau $K_0$.

Si un élément $k\in K$ fixe un sommet $a$ de G, l’élément $g^{-1}kg$ fixe le sommet $g^*a$; cela entraîne que $K_0$ est un sous-groupe distingué de K.

D’après la proposition 5, l’unique homomorphisme $\lambda : F(K)\rightarrow$ $(G/K)_{\gamma(o)}$ tel que $\lambda ([k]) =\gamma (c_k)$ est surjectif, et son noyau est le plus petit sous-groupe distingué de F(K) contenant les éléments $[k]$, où $k$ est un élément de K qui fixe un sommet de G, et les éléments $[kh]^{-1}[k][h]$, où $(k, h)\in K^2$. En particulier, l’application $\lambda ': K\rightarrow (G/K)_{\gamma(o)}$, définie par $\lambda '(k) =\gamma (c_k) =\lambda ([k])$ pour $k\in K$, est un homomorphisme de groupes. On a $\lambda =\lambda '\circ p$, où $p: F(K)\rightarrow K$ désigne l’homomorphisme de groupes surjectif canonique. Par suite, l’homomorphisme $\lambda '$ est surjectif et son noyau est le plus petit sous-groupe distingué de K qui contient les éléments $k$, pour $k$ fixant un sommet de G, c’est-à-dire $K_0$. Cela démontre la proposition.

## EXERCICES {#ta-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
